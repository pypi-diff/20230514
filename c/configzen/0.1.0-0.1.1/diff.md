# Comparing `tmp/configzen-0.1.0.tar.gz` & `tmp/configzen-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.1.0.tar", max compression
+gzip compressed data, was "configzen-0.1.1.tar", max compression
```

## Comparing `configzen-0.1.0.tar` & `configzen-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,7 @@
--rw-r--r--   0        0        0      199 2023-05-06 22:29:21.750508 configzen-0.1.0/configzen/__init__.py
--rw-r--r--   0        0        0    30443 2023-05-09 17:55:11.331986 configzen-0.1.0/configzen/config.py
--rw-r--r--   0        0        0     5682 2023-05-09 16:43:59.406224 configzen-0.1.0/configzen/engine.py
--rw-r--r--   0        0        0      288 2023-05-02 23:54:25.044063 configzen-0.1.0/configzen/engines/configparser_engine.py
--rw-r--r--   0        0        0     1717 2023-05-09 17:59:20.431270 configzen-0.1.0/configzen/engines/json_engine.py
--rw-r--r--   0        0        0        0 2023-04-05 18:08:49.057819 configzen-0.1.0/configzen/engines/orm_engine.py
--rw-r--r--   0        0        0      983 2023-05-09 18:00:25.291934 configzen-0.1.0/configzen/engines/yaml_engine.py
--rw-r--r--   0        0        0      304 2023-05-09 17:20:29.589794 configzen-0.1.0/configzen/errors.py
--rw-r--r--   0        0        0     1085 2023-05-09 16:10:00.173126 configzen-0.1.0/configzen/recipes.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.0/LICENSE
--rw-r--r--   0        0        0      547 2023-05-09 17:27:09.939469 configzen-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      368 2023-05-06 21:08:45.825874 configzen-0.1.0/README.md
--rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 configzen-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      135 2023-05-14 02:04:46.442804 configzen-0.1.1/configzen/__init__.py
+-rw-r--r--   0        0        0    32122 2023-05-14 02:36:01.959219 configzen-0.1.1/configzen/config.py
+-rw-r--r--   0        0        0      853 2023-05-14 02:32:13.602772 configzen-0.1.1/configzen/errors.py
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.1/LICENSE
+-rw-r--r--   0        0        0      590 2023-05-14 02:38:37.575944 configzen-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2407 2023-05-14 02:01:48.926739 configzen-0.1.1/README.md
+-rw-r--r--   0        0        0     3250 1970-01-01 00:00:00.000000 configzen-0.1.1/PKG-INFO
```

### Comparing `configzen-0.1.0/configzen/config.py` & `configzen-0.1.1/configzen/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,184 +1,346 @@
 """Core configuration classes and functions."""
 
 from __future__ import annotations
 
 import abc
+import collections.abc
 import contextlib
 import copy
 import dataclasses
-import inspect
+import functools
 import io
 import os
 import pathlib
-import sys
-from collections.abc import ByteString, Callable, Generator, Iterator, MutableMapping
+import urllib.parse
+import urllib.request
+from collections.abc import Callable, Generator
 from typing import (
     TYPE_CHECKING,
     Any,
-    ClassVar,
     Generic,
+    Literal,
     NamedTuple,
     TypeVar,
-    cast
+    cast,
 )
-from urllib.parse import urlparse, uses_netloc, uses_params, uses_relative
-from urllib.request import Request, urlopen
 
-from configzen.engine import Engine, convert, get_engine_class, load, loaders
-from configzen.recipes import dataclass_load
+import anyconfig
+import pydantic
+from pydantic.main import ModelMetaclass
 
-if sys.version_info >= (3, 11):
-    from typing import dataclass_transform
-else:
-    from typing_extensions import dataclass_transform
-
-if TYPE_CHECKING:
-    from collections.abc import ItemsView, Mapping
+from configzen.errors import ConfigItemAccessError, UnknownParserError
 
 try:
     import aiofiles
 
     AIOFILES_AVAILABLE = True
 except ImportError:
     aiofiles = None  # type: ignore[assignment]
     AIOFILES_AVAILABLE = False
 
 __all__ = (
-    "ConfigSpec",
-    "BaseConfig",
-    "Config",
-    "AsyncConfig",
-    "BaseLoader",
-    "DefaultLoader",
+    "ConfigResource",
+    "ConfigModelBase",
+    "ConfigModel",
+    "AsyncConfigModel",
+    "Meta",
     "save",
+    "save_async",
+    "reload",
+    "reload_async",
+    "convert",
+    "converter",
+    "convert_namedtuple",
+    "convert_mapping",
+    "load",
+    "loader",
 )
 
-_URL_SCHEMES: set[str] = set(uses_relative + uses_netloc + uses_params) - {""}
-_CONTEXT_ATTRIBUTE: str = "_context"
+_URL_SCHEMES: set[str] = set(
+    urllib.parse.uses_relative
+    + urllib.parse.uses_netloc
+    + urllib.parse.uses_params,
+) - {""}
+_CONTEXT: str = "__config_context__"
+
+T = TypeVar("T")
+
+ContextT = TypeVar("ContextT", bound="AnyContext")
+ConfigModelBaseT = TypeVar("ConfigModelBaseT", bound="ConfigModelBase")
+ConfigModelT = TypeVar("ConfigModelT", bound="ConfigModel")
+AsyncConfigModelT = TypeVar("AsyncConfigModelT", bound="AsyncConfigModel")
 
-ContextT = TypeVar("ContextT", bound="BaseConfigContext")
-if sys.version_info >= (3, 10):
-    BlobT = TypeVar("BlobT", str, ByteString)
-else:
-    BlobT = TypeVar("BlobT", str, bytes, bytearray, memoryview)
-LoaderFactoryT = Callable[[dict[str, Callable]], "BaseLoader"]
-BaseConfigT = TypeVar("BaseConfigT", bound="BaseConfig")
-ConfigT = TypeVar("ConfigT", bound="Config")
-AsyncConfigT = TypeVar("AsyncConfigT", bound="AsyncConfig")
 OpenedT = contextlib.AbstractContextManager
+ResourceT = OpenedT | str | os.PathLike | pathlib.Path
+
+
+def _get_defaults_from_model_class(
+    model: type[pydantic.BaseSettings],
+) -> dict[str, Any]:
+    defaults = {}
+    for field in model.__fields__.values():
+        default = field.default
+        if not field.field_info.exclude and not field.required:
+            if isinstance(default, pydantic.BaseSettings):
+                default = default.dict()
+            defaults[field.name] = default
+    return defaults
+
+
+def _vars(obj: Any) -> dict[str, Any]:
+    obj_dict = obj
+    if not isinstance(obj, dict):
+        obj_dict = vars(obj)
+    return obj_dict
+
+
+def _is_namedtuple(
+    obj: Any,
+) -> bool:
+    return (
+        isinstance(obj, tuple) and
+        hasattr(obj, "_asdict") and
+        hasattr(obj, "_fields")
+    )
+
+
+@functools.singledispatch
+def convert(obj: Any) -> Any:
+    """Convert a value to a format that can be safely serialized."""
+    if dataclasses.is_dataclass(obj):
+        return dataclasses.asdict(obj)
+    if _is_namedtuple(obj):
+        return convert_namedtuple(obj)
+    return obj
+
+
+_convert_register = convert.register
+
+
+def converter(func: Callable[[T], Any], cls: type[T] | None = None) -> type[T] | Any:
+    """Register a converter function for a type."""
+    if cls is None:
+        return functools.partial(converter, func)
+
+    _convert_register(cls, func)
+
+    if not hasattr(cls, "__get_validators__"):
+        def validator_gen() -> Generator[Callable[[Any], Any], None, None]:
+            yield lambda value: load.dispatch(cls)(cls, value)
+
+        cls.__get_validators__ = validator_gen  # type: ignore[attr-defined]
+
+    return cls
+
+
+@functools.singledispatch
+def load(cls: Any, value: Any) -> Any:
+    if isinstance(value, cls):
+        return value
+    return cls(value)
+
+
+def loader(func: Callable[[Any], T], cls: type[T] | None = None) -> type[T] | Any:
+    """Register a loader function for a type."""
+    if cls is None:
+        return functools.partial(loader, func)
+
+    load.register(cls, func)
+    return cls
+
+
+@convert.register
+def convert_mapping(obj: collections.abc.Mapping) -> dict[str, Any]:
+    return {k: convert(v) for k, v in obj.items()}
+
+
+@functools.singledispatch
+def convert_namedtuple(obj: tuple) -> dict[str, Any]:
+    # Initially I wanted it to be convert(obj._asdict()), but
+    # pydantic doesn't seem to be friends with custom NamedTuples.
+    return convert(list(obj))
 
 
-class ConfigSpec(Generic[BlobT]):
-    """A specification for a configuration file."""
+def split_ac_options(options: dict[str, Any]) -> tuple[dict[str, Any], dict[str, Any]]:
+    """Split a dictionary of options into those for loading and those for dumping."""
+    load_options: dict[str, Any] = {}
+    dump_options: dict[str, Any] = {}
+    for key, value in options.items():
+        final_key = key
+        if key.startswith("dump_"):
+            final_key = key.removeprefix("dump_")
+            targets = [dump_options]
+        elif key.startswith("load_"):
+            final_key = key.removeprefix("load_")
+            targets = [dump_options]
+        else:
+            targets = [load_options, dump_options]
+        for target in targets:
+            if final_key in target:
+                msg = (
+                    f"option {key}={value!r} overlaps with "
+                    f"defined {final_key}={target[final_key]!r}"
+                )
+                raise ValueError(msg)
+            target[final_key] = value
+
+    return load_options, dump_options
 
-    filepath_or_stream: OpenedT | str | os.PathLike | pathlib.Path
+
+class ConfigResource:
+    """A configuration resource to read from/write to."""
+
+    _resource: OpenedT | str | os.PathLike | pathlib.Path
     defaults: dict[str, Any]
-    create_missing: bool
-    engine_name: str
-    _engine: Engine | None
-    _engine_options: dict[str, Any]
+    create_if_missing: bool
+    ac_parser: str | None
+    _ac_load_options: dict[str, Any]
+    _ac_dump_options: dict[str, Any]
     cache_engine: bool
     allowed_url_schemes: set[str] = _URL_SCHEMES
 
     def __init__(
-        self: ConfigSpec[BlobT],
-        filepath_or_stream: OpenedT[BlobT] | str,
-        engine_name: str,
+        self: ConfigResource,
+        resource: ResourceT,
+        ac_parser: str | None = None,
         *,
-        cache_engine: bool = True,
-        defaults: dict[str, Any] | None = None,
-        create_missing: bool = False,
-        **engine_options: Any,
+        create_if_missing: bool = False,
+        use_pydantic_json: bool = True,
+        **options: Any,
     ) -> None:
         """Parameters
         ----------
-        filepath_or_stream : str or file-like object, optional
-            The path to the configuration file, or a file-like object.
-            If not provided, an empty configuration will be created.
-        engine_name : str, optional
-            The name of the engine to use for loading and saving the configuration.
+        resource : str or file-like object, optional
+            The URL to the configuration file, or a file-like object.
+        ac_parser : str, optional
+            The name of the engines to use for loading and saving the configuration.
             Defaults to 'yaml'.
-        cache_engine : bool, optional
-            Whether to cache the engine instance. Defaults to True.
-            If False, a new engine instance will be created for each load and dump.
-        defaults : dict, optional
-            A dictionary of default values to use when loading the configuration.
-        create_missing : bool, optional
+        create_if_missing : bool, optional
             Whether to automatically create missing keys when loading the configuration.
-        **engine_options
-            Additional keyword arguments to pass to the engine.
+        use_pydantic_json : bool, optional
+            Whether to use Pydantic's JSON encoder/decoder instead of the default
+            anyconfig one.
+        **options
+            Additional keyword arguments to pass to
+            `anyconfig.loads()` and `anyconfig.dumps()`.
         """
-        self.filepath_or_stream = filepath_or_stream
-        self.defaults = defaults or {}
+        self.ac_parser = ac_parser
+        self.resource = resource
+        self.create_if_missing = create_if_missing
+        self.use_pydantic_json = use_pydantic_json
+        self._ac_load_options, self._ac_dump_options = split_ac_options(options)
 
-        self.engine_name = engine_name
-        self._engine = None
-        self._engine_options = engine_options
-        if cache_engine:
-            self._engine = get_engine_class(self.engine_name)(**engine_options)
-        self.cache_engine = cache_engine
-
-        self.create_missing = create_missing
-
-    def _get_engine(self) -> Engine:
-        """Get the engine instance to use for loading and saving the configuration."""
-        engine = self._engine
-        if engine is None:
-            engine_class = get_engine_class(self.engine_name)
-            engine = engine_class(**self._engine_options)
-        if self.cache_engine:
-            self._engine = engine
-        return engine
-
-    @property
-    def engine(self) -> Engine:
-        """The engine instance to use for loading and saving the configuration."""
-        return self._get_engine()
+    @property
+    def resource(self) -> ResourceT:
+        return self._resource
+
+    @resource.setter
+    def resource(self, value: ResourceT) -> None:
+        self._resource = value
+        self.ac_parser = self.ac_parser or self._guess_ac_parser()
+
+    def _guess_ac_parser(self) -> str | None:
+        ac_parser = None
+        if isinstance(self.resource, str):
+            ac_parser = pathlib.Path(self.resource).suffix[1:].casefold()
+            if not ac_parser:
+                msg = f"Could not guess the engine to use for {self.resource!r}."
+                raise UnknownParserError(
+                    msg,
+                )
+        return ac_parser
+
+    def load_into(
+        self,
+        config_class: type[ConfigModelBaseT],
+        blob: str,
+        ac_parser: str | None = None,
+        **kwargs: Any,
+    ) -> ConfigModelBaseT:
+        config = self.load_into_dict(blob, ac_parser=ac_parser, **kwargs)
+        if config is None:
+            config = {}
+        return config_class(**config)
+
+    def load_into_dict(
+        self,
+        blob: str,
+        ac_parser: str | None = None,
+        **kwargs: Any,
+    ) -> dict[str, Any]:
+        if ac_parser is None:
+            ac_parser = self.ac_parser
+        kwargs = {**self._ac_load_options, **kwargs}
+        return anyconfig.loads(blob, ac_parser=ac_parser, **kwargs)
+
+    def dump_config(
+        self,
+        config: ConfigModelBaseT,
+        ac_parser: str | None = None,
+        **kwargs: Any,
+    ) -> str:
+        if ac_parser is None:
+            ac_parser = self.ac_parser
+        if ac_parser == "json" and self.use_pydantic_json:
+            return config.json(**kwargs)
+        data = config.dict()
+        return self.dump_data(data, ac_parser=ac_parser, **kwargs)
+
+    def dump_data(
+        self,
+        data: dict[str, Any],
+        ac_parser: str | None = None,
+        **kwargs: Any,
+    ) -> str:
+        if ac_parser is None:
+            ac_parser = self.ac_parser
+        kwargs = {**self._ac_dump_options, **kwargs}
+        return anyconfig.dumps(
+            convert(data),
+            ac_parser=ac_parser,
+            **kwargs,
+        )
 
     @property
     def is_url(self) -> bool:
-        """Whether the filepath_or_stream is a URL."""
+        """Whether the entrypoint is a URL."""
         return (
-            isinstance(self.filepath_or_stream, str)
-            and urlparse(self.filepath_or_stream).scheme in _URL_SCHEMES
+            isinstance(self.resource, str)
+            and urllib.parse.urlparse(self.resource).scheme in _URL_SCHEMES
         )
 
-    @classmethod
-    def from_str(cls, spec: str, **kwargs: Any) -> ConfigSpec:
-        """Create a ConfigSpec from a string."""
-        kwargs.setdefault("engine_name", pathlib.Path(spec).suffix[1:])
-        return cls(spec, **kwargs)
-
-    def open_sync(self, **kwds: Any) -> OpenedT:
+    def open_resource(self, **kwds: Any) -> OpenedT:
         """Open the configuration file.
 
         Parameters
         ----------
         **kwds
             Keyword arguments to pass to the opening routine.
-            For URLs, these are passed to ``urllib.request.urlopen()``.
+            For URLs, these are passed to ``urllib.request.urllib.request.urlopen()``.
             For local files, these are passed to ``builtins.open()``.
         """
-        if self.filepath_or_stream is None:
+        if self.resource is None:
             return io.StringIO()
         if self.is_url:
-            url = cast(str, self.filepath_or_stream)
-            if urlparse(url).scheme not in self.allowed_url_schemes:
+            url = cast(str, self.resource)
+            if urllib.parse.urlparse(url).scheme not in self.allowed_url_schemes:
                 msg = (
-                    f"URL scheme {urlparse(url).scheme!r} is not allowed, "
+                    f"URL scheme {urllib.parse.urlparse(url).scheme!r} is not allowed, "
                     f"must be one of {self.allowed_url_schemes!r}"
                 )
                 raise ValueError(msg)
-            return urlopen(Request(url), **kwds)  # noqa: S310, ^
-        if isinstance(self.filepath_or_stream, (str, os.PathLike, pathlib.Path)):
-            return pathlib.Path(self.filepath_or_stream).open(**kwds)
-        return self.filepath_or_stream
+            return urllib.request.urlopen(  # noqa: S310, ^
+                urllib.request.Request(url), **kwds
+            )
+        if isinstance(self.resource, str | os.PathLike | pathlib.Path):
+            return pathlib.Path(self.resource).open(**kwds)
+        return self.resource
 
-    def open_async(self, **kwds: Any) -> Any:
+    def open_resource_async(self, **kwds: Any) -> Any:
         """Open the configuration file asynchronously.
 
         Parameters
         ----------
         **kwds
             Keyword arguments to pass to the opening routine.
         """
@@ -186,518 +348,452 @@
             msg = "asynchronous URL opening is not supported"
             raise NotImplementedError(msg)
         if not AIOFILES_AVAILABLE:
             msg = (
                 "aiofiles is not available, cannot open file "
                 "asynchronously (install with `pip install aiofiles`)"
             )
-            raise RuntimeError(
-                msg,
-            )
-        return aiofiles.open(cast(str, self.filepath_or_stream), **kwds)
+            raise RuntimeError(msg)
+        return aiofiles.open(cast(str, self.resource), **kwds)
+
+    def _get_default_kwargs(
+        self, operation: Literal["read", "write"],
+        kwargs: dict[str, Any] | None = None,
+    ) -> dict[str, Any]:
+        if kwargs is None:
+            kwargs = {}
+        if not self.is_url:
+            if operation == "read":
+                kwargs.setdefault("mode", "r")
+            elif operation == "write":
+                kwargs.setdefault("mode", "w")
+            else:
+                msg = f"invalid method {operation!r}"
+                raise ValueError(msg)
+        return kwargs
 
     def read(
         self,
         *,
-        create_kwds: dict[str, Any] | None = None,
-        **kwds: Any,
-    ) -> dict[str, Any]:
+        config_class: type[ConfigModelBaseT],
+        create_kwargs: dict[str, Any] | None = None,
+        **kwargs: Any,
+    ) -> ConfigModelBaseT:
         """Read the configuration file.
 
         Parameters
         ----------
-        create_kwds : dict, optional
+        config_class
+        create_kwargs : dict, optional
             Keyword arguments to pass to the open method
             when optionally creating the file.
-        **kwds
+        **kwargs
             Keyword arguments to pass to the open method.
         """
-        blob: str | ByteString | None
+        kwargs = self._get_default_kwargs("read", kwargs=kwargs)
         try:
-            with self.open_sync(**kwds) as fp:
+            with self.open_resource(**kwargs) as fp:
                 blob = fp.read()
         except FileNotFoundError:
             blob = None
-            if self.create_missing:
-                blob = self.engine.dump(config_convert(self.defaults))
-                if create_kwds is None:
-                    create_kwds = {}
-                self.write(blob, **create_kwds)
-        return self.engine.load(blob, defaults=self.defaults)
+            if self.create_if_missing:
+                defaults = _get_defaults_from_model_class(config_class)
+                blob = self.dump_data(defaults)
+                create_kwargs = self._get_default_kwargs("write", kwargs=create_kwargs)
+                self.write(blob, **create_kwargs)
+        return self.load_into(config_class, blob, **self._ac_load_options)
 
-    def write(self, blob: str | ByteString, **kwds: Any) -> int:
-        with self.open_sync(**kwds) as fp:
+    def write(self, blob: str | collections.abc.ByteString, **kwds: Any) -> int:
+        with self.open_resource(**kwds) as fp:
             return fp.write(blob)
 
     async def read_async(
         self,
         *,
-        create_kwds: dict[str, Any] | None = None,
-        **kwds: Any,
-    ) -> dict[str, Any]:
+        config_class: type[AsyncConfigModelT],
+        create_kwargs: dict[str, Any] | None = None,
+        **kwargs: Any,
+    ) -> AsyncConfigModelT:
         """Read the configuration file asynchronously.
 
         Parameters
         ----------
-        create_kwds : dict, optional
+        config_class
+        create_kwargs : dict, optional
             Keyword arguments to pass to the open method
             when optionally creating the file.
-        **kwds
+        **kwargs
             Keyword arguments to pass to the open method.
         """
+        kwargs = self._get_default_kwargs("read", kwargs=kwargs)
         try:
-            async with self.open_async(**kwds) as fp:
+            async with self.open_resource_async(**kwargs) as fp:
                 blob = await fp.read()
         except FileNotFoundError:
-            if self.create_missing:
-                blob = self.engine.dump(config_convert(self.defaults))
-                if create_kwds is None:
-                    create_kwds = {}
-                await self.write_async(blob, **create_kwds)
-        return self.engine.load(blob, defaults=self.defaults)
-
-    async def write_async(self, blob: str | ByteString, **kwds: Any) -> int:
-        async with self.open_async(**kwds) as fp:
-            return await fp.write(blob)
-
-
-class BaseLoader:
-    """A strategy for loading a configuration to a dictionary of objects.
+            if self.create_if_missing:
+                defaults = _get_defaults_from_model_class(config_class)
+                blob = self.dump_data(defaults)
+                create_kwargs = self._get_default_kwargs("write", kwargs=create_kwargs)
+                await self.write_async(blob, **create_kwargs)
+        return self.load_into(config_class, blob, **self._ac_load_options)
 
-    Parameters
-    ----------
-    sections : dict, optional
-        A dictionary of configuration keys and their corresponding types.
-        If not provided, the sections must be provided as keyword arguments.
-    """
-
-    sections: dict[str, Callable[[Any], Any]]
-
-    def __init__(self, sections: dict[str, Callable[[Any], Any]] | None = None) -> None:
-        self.sections = sections or {}
-
-    @classmethod
-    def with_sections(cls, sections: dict[str, Callable[[Any], Any]]) -> BaseLoader:
-        return cls(sections=sections)
-
-    async def load_async(
+    async def write_async(
         self,
-        data: MutableMapping[str, Any],
-        context: ConfigContext,
-    ) -> MutableMapping[str, Any]:
-        """Dispatch the configuration to a dictionary of objects.
-
-        Parameters
-        ----------
-        data : dict
-            The configuration data.
-
-        context : ConfigContext
-            The configuration context.
-
-        Returns
-        -------
-        dict
-            The ready-to-use configuration dictionary.
-
-        """
-        raise NotImplementedError
-
-    def load(
-        self,
-        data: MutableMapping[str, Any],
-        context: ConfigContext,
-    ) -> MutableMapping[str, Any]:
-        """Dispatch the configuration to a dictionary of objects.
-
-        Parameters
-        ----------
-        data : dict
-            The configuration data.
-
-        context : ConfigContext
-            The configuration context.
-
-        Returns
-        -------
-        dict
-            The ready-to-use configuration dictionary.
-
-        """
-        raise NotImplementedError
+        blob: str | collections.abc.ByteString, **kwds: Any,
+    ) -> int:
+        async with self.open_resource_async(**kwds) as fp:
+            return await fp.write(blob)
 
 
 if TYPE_CHECKING:
-    MutableMappingType = TypeVar("MutableMappingType", bound="MutableMapping")  # Y001
 
-
-    class ConfigAt(NamedTuple, Generic[MutableMappingType]):
-        config: MutableMappingType
+    class ConfigAt(NamedTuple, Generic[ConfigModelBaseT]):
+        owner: ConfigModelBaseT
+        mapping: dict[str, Any] | None
         route: list[str]
 
         def get(self) -> Any:
             ...
 
-        def update(self, _value: Any) -> None:
+        def update(self, _value: Any) -> dict[str, Any]:
             ...
 
         async def save_async(self) -> int:
             ...
 
         def save(self) -> int:
             ...
 
 
 else:
     class ConfigAt(NamedTuple):
         """Metadata for a configuration item."""
 
-        config: MutableMapping
+        owner: ConfigModelBaseT
+        mapping: dict[str, Any] | None
         route: list[str]
 
         def get(self) -> Any:
-            value = self.config
-            for key in self.route:
-                value = value[key]
-            return value
+            scope = _vars(self.mapping or self.owner.dict())
+            route_here = []
+            try:
+                for part in self.route:
+                    route_here.append(part)
+                    scope = _vars(scope)[part]
+            except KeyError:
+                raise ConfigItemAccessError(self.owner, route_here) from None
+            return scope
 
-        def update(self, value: Any) -> None:
+        def update(self, value: Any) -> collections.abc.MutableMapping:
             route = list(self.route)
-            if len(route) == 1:
-                self.config[route[0]] = value
-            else:
-                key = route.pop()
-                self._replace(route=route).get()[key] = value
+            mapping = self.mapping or self.owner.dict()
+            key = route.pop()
+            submapping = _vars(mapping)
+            route_here = []
+            try:
+                for part in route:
+                    route_here.append(part)
+                    submapping = _vars(submapping[part])
+                submapping[key] = value
+            except KeyError:
+                raise ConfigItemAccessError(self.owner, route_here) from None
+            return mapping
 
         async def save_async(self) -> int:
             return await save_async(self)
 
         def save(self) -> int:
             return save(self)
 
+        async def reload_async(self) -> Any:
+            return await reload_async(self)
 
-class DefaultLoader(BaseLoader):
-    def __init__(
-        self,
-        sections: dict[str, Callable[[Any], Any]] | None = None,
-        *,
-        strict: bool = False,
-    ) -> None:
-        super().__init__(sections)
-        self.strict = strict
-        self._deferred_items: dict[str, Any] = {}
-
-    @classmethod
-    def strict_with_sections(cls, sections: dict[str, Callable]) -> DefaultLoader:
-        return cls(sections=sections, strict=True)
-
-    def load_deferred_items(self) -> None:
-        for key, (value, context) in self._deferred_items.items():
-            self._load_item(key, value, context)
-
-    def _load_item(self, key: str, value: Any, context: ContextT) -> Any:
-        try:
-            factory = self.sections[key]
-        except KeyError:
-            self._deferred_items.update({key: (value, context)})
-            return value
-        self._deferred_items.pop(key, None)
-        return load(factory, value, context)
-
-    async def _async_load_item(self, key: str, value: Any, context: ContextT) -> Any:
-        data = self._load_item(key, value, context)
-        if inspect.isawaitable(data):
-            data = await data
-        return data
-
-    def load(self, data: Mapping | None, context: ContextT) -> Any:
-        return {
-            key: self._load_item(key, value, context.enter(key))
-            for key, value in (data or {}).items()
-        }
-
-    async def load_async(self, data: Mapping | None, context: ContextT) -> Any:
-        return {
-            key: await self._async_load_item(key, value, context.enter(key))
-            for key, value in (data or {}).items()
-        }
+        def reload(self) -> Any:
+            return reload(self)
 
 
-def save(section: ConfigT | ConfigAt[ConfigT]) -> int:
-    if isinstance(section, Config):
+def save(section: ConfigModelT | ConfigAt) -> int:
+    if isinstance(section, ConfigModel):
         config = section
         return config.save()
 
-    section = cast(ConfigAt[ConfigT], section)
-    config = cast(ConfigT, section.config)
+    config = section.owner
     data = config.original
-    at = ConfigAt(data, section.route)
-    at.update(section.get())
-    context = ConfigContext.get(config)
-    spec = cast(ConfigSpec, context.spec)
-    blob = spec.engine.dump(config_convert(data))
+    at = ConfigAt(config, data, section.route)
+    data = at.update(section.get())
+    context = get_context(config)
+    blob = context.resource.dump_config(config.copy(update=data))
     result = config.write(blob)
     context.original = data
     return result
 
 
-async def save_async(section: AsyncConfigT | ConfigAt[AsyncConfigT]) -> int:
-    if isinstance(section, AsyncConfig):
+async def save_async(section: AsyncConfigModelT | ConfigAt) -> int:
+    if isinstance(section, AsyncConfigModel):
         config = section
         return await config.save_async()
 
-    if TYPE_CHECKING:
-        section = cast(ConfigAt[AsyncConfigT], section)
-    config = section.config
+    config = section.owner
     data = config.original
-    ConfigAt(data, section.route).update(section.get())
-    context = ConfigContext.get(config)
-    spec = cast(ConfigSpec, context.spec)
-    blob = spec.engine.dump(config_convert(data))
+    at = ConfigAt(config, data, section.route)
+    data = at.update(section.get())
+    context = get_context(config)
+    blob = context.resource.dump_config(config.copy(update=data))
     result = await config.write_async(blob)
     context.original = data
     return result
 
 
-class BaseConfigContext(abc.ABC, Generic[ConfigT]):
+def reload(section: ConfigModelT | ConfigAt) -> Any:
+    if isinstance(section, ConfigModel):
+        config = section
+        return config.reload()
+
+    config = section.owner
+    context = get_context(config)
+    data = config.dict()
+    newest = context.resource.read(config_class=type(config))
+    section_data = ConfigAt(newest, newest.dict(), section.route).get()
+    new_mapping = ConfigAt(config, data, section.route).update(section_data)
+    config.__dict__.update(new_mapping)
+    return section_data
+
+
+async def reload_async(section: AsyncConfigModelT | ConfigAt) -> Any:
+    if isinstance(section, AsyncConfigModel):
+        config = section
+        return await config.reload_async()
+
+    config = section.owner
+    context = get_context(config)
+    data = config.dict()
+    newest = await context.resource.read_async(config_class=type(config))
+    section_data = ConfigAt(newest, newest.dict(), section.route).get()
+    new_mapping = ConfigAt(config, data, section.route).update(section_data)
+    config.__dict__.update(new_mapping)
+    return new_mapping
+
+
+class AnyContext(abc.ABC, Generic[ConfigModelBaseT]):
     original: dict[str, Any]
     _original: dict[str, Any]
     loaded: bool
 
     @abc.abstractmethod
-    def trace_route(self) -> Generator[str, None, None]:
+    def trace_route(self) -> collections.abc.Generator[str, None, None]:
         """Trace the route to the configuration context."""
 
-    @classmethod
-    def get(cls, config: ConfigT) -> BaseConfigContext[ConfigT]:
-        return object.__getattribute__(config, _CONTEXT_ATTRIBUTE)
+    @staticmethod
+    def get(config: ConfigModelBaseT) -> AnyContext[ConfigModelBaseT]:
+        return object.__getattribute__(config, _CONTEXT)
 
-    def bind_to(self, config: ConfigT) -> None:
+    def bind_to(self, config: ConfigModelBaseT) -> None:
         if config is None:
             return
-        object.__setattr__(config, _CONTEXT_ATTRIBUTE, self)
+        object.__setattr__(config, _CONTEXT, self)
 
-    def enter(self, key: str) -> ConfigSubcontext[ConfigT]:
-        return ConfigSubcontext(self, key)
+    def enter(self, key: str) -> Subcontext[ConfigModelBaseT]:
+        return Subcontext(self, key)
 
     @property
     @abc.abstractmethod
-    def spec(self) -> ConfigSpec | None:
+    def resource(self) -> ConfigResource:
         ...
 
     @property
     @abc.abstractmethod
-    def owner(self) -> ConfigT | None:
+    def owner(self) -> ConfigModelBaseT | None:
         ...
 
     @property
     @abc.abstractmethod
-    def section(self) -> ConfigT | ConfigAt[ConfigT]:
+    def section(self) -> ConfigModelBaseT | ConfigAt[ConfigModelBaseT]:
         ...
 
 
-class ConfigSubcontext(BaseConfigContext, Generic[ConfigT]):
-    def __init__(self, parent: BaseConfigContext[ConfigT], key: str) -> None:
-        self.parent = parent
-        self.key = key
-
-    @property
-    def spec(self) -> None:
-        return None  # ???
-
-    def trace_route(self) -> Generator[str, None, None]:
-        yield from self.parent.trace_route()
-        yield self.key
-
-    @property
-    def section(self) -> ConfigAt[ConfigT]:
-        if self.owner is None:
-            msg = "Cannot get section for unbound context"
-            raise ValueError(msg)
-        return ConfigAt(self.owner, list(self.trace_route()))
-
-    @property
-    def owner(self) -> ConfigT | None:
-        return self.parent.owner
-
-    @property
-    def original(self) -> dict[str, Any]:
-        return self.parent.original
-
-    @original.setter
-    def original(self, value: dict[str, Any]) -> None:
-        data = self.parent.original
-        data[self.key] = value
-        self.parent.original = data
-
-    @property
-    def loaded(self) -> bool:
-        return self.parent.loaded
-
-    @loaded.setter
-    def loaded(self, value: bool) -> None:
-        self.parent.loaded = value
-
-
-class ConfigContext(BaseConfigContext, Generic[BaseConfigT]):
-    def __init__(self, spec: ConfigSpec, owner: BaseConfigT | None = None) -> None:
-        self._spec = spec
+class Context(AnyContext, Generic[ConfigModelBaseT]):
+    def __init__(
+        self,
+        resource: ConfigResource,
+        owner: ConfigModelBaseT | None = None,
+    ) -> None:
+        self._resource = resource
         self._owner = None
         self._original = {}
         self._loaded = False
 
         self.owner = owner
 
-    def trace_route(self) -> Generator[str, None, None]:
+    def trace_route(self) -> collections.abc.Generator[str, None, None]:
         yield from ()
 
     @property
-    def spec(self) -> ConfigSpec:
-        return self._spec
+    def resource(self) -> ConfigResource:
+        return self._resource
 
     @property
-    def section(self) -> BaseConfigT | None:
+    def section(self) -> ConfigModelBaseT | None:
         return self.owner
 
     @property
-    def owner(self) -> BaseConfigT | None:
+    def owner(self) -> ConfigModelBaseT | None:
         return self._owner
 
     @owner.setter
-    def owner(self, config: BaseConfigT | None) -> None:
+    def owner(self, config: ConfigModelBaseT | None) -> None:
         if config is None:
             return
         self.bind_to(config)
         self._owner = config
 
     @property
     def original(self) -> dict[str, Any]:
         return copy.deepcopy(self._original)
 
     @original.setter
     def original(self, original: dict[str, Any]) -> None:
-        self._original = dict(original)
+        self._original = copy.deepcopy(original)
 
     @property
     def loaded(self) -> bool:
         return self._loaded
 
     @loaded.setter
     def loaded(self, value: bool) -> None:
         self._loaded = value
 
 
-FieldWatcherBase: type = type(MutableMapping)
+class Subcontext(AnyContext, Generic[ConfigModelBaseT]):
+    def __init__(self, parent: AnyContext[ConfigModelBaseT], key: str) -> None:
+        self.parent = parent
+        self.key = key
 
+    @property
+    def resource(self) -> ConfigResource:
+        return self.parent.resource
 
-class FieldWatcher(FieldWatcherBase):
-    _loader_factory: LoaderFactoryT
-    _loader: BaseLoader
+    def trace_route(self) -> collections.abc.Generator[str, None, None]:
+        yield from self.parent.trace_route()
+        yield self.key
 
-    def __setattr__(self, key: str, value: Any) -> None:
-        super().__setattr__(key, value)
-        if key == "__dataclass_fields__":
-            self._on_dataclass_fields(value)
+    @property
+    def section(self) -> ConfigAt[ConfigModelBaseT]:
+        if self.owner is None:
+            msg = "Cannot get section for unbound context"
+            raise ValueError(msg)
+        return ConfigAt(self.owner, None, list(self.trace_route()))
 
-    def _on_dataclass_fields(
-        self,
-        dataclass_fields: dict[str, dataclasses.Field],
-    ) -> None:
-        sections = {
-            name: cast(Callable, field.type)
-            for name, field in dataclass_fields.items()
-        }
-        self._loader = self._loader_factory(sections)
-        loaders.register(self, config_load)
-        convert.register(self, config_convert)
-
-
-@dataclass_transform()
-class BaseConfig(MutableMapping[str, Any], metaclass=FieldWatcher):
-    """A configuration dictionary.
-
-    Notes
-    -----
-    Either ``loader`` or ``sections`` must be provided.
-    If both are provided, a ValueError is raised.
-    """
-
-    _loader: ClassVar[BaseLoader]
-    _context: ConfigContext
-    __dataclass_fields__: ClassVar[dict[str, dataclasses.Field]]
-
-    if TYPE_CHECKING:
-        # Because PyCharm doesn't understand
-        def __init__(self, *_args: Any, **_kwargs: Any) -> None:
-            ...
+    @property
+    def owner(self) -> ConfigModelBaseT | None:
+        return self.parent.owner
 
-    @abc.abstractmethod
-    def __call__(self, **config: Any) -> Any:
-        """Update the configuration with the given keyword arguments."""
+    @property
+    def original(self) -> dict[str, Any]:
+        return self.parent.original
 
-    def __iter__(self) -> Iterator[str]:
-        return iter(self.as_dict())
+    @original.setter
+    def original(self, value: dict[str, Any]) -> None:
+        data = self.parent.original
+        data[self.key] = copy.deepcopy(value)
+        self.parent.original = data
 
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.update({key: value})
+    @property
+    def loaded(self) -> bool:
+        return self.parent.loaded
 
-    def __getitem__(self, item: str) -> Any:
-        return self.as_dict()[item]
+    @loaded.setter
+    def loaded(self, value: bool) -> None:
+        self.parent.loaded = value
 
-    def __delitem__(self, key: str) -> None:
-        delattr(self, key)
 
-    def __len__(self) -> int:
-        return len(self.as_dict())
+def get_context(config: ConfigModelBaseT) -> AnyContext[ConfigModelBaseT]:
+    context = AnyContext.get(config)
+    if context is None:
+        msg = "Cannot get context for unbound configuration"
+        raise RuntimeError(msg)
+    return context
+
+
+def json_encoder(
+    model_encoder: Callable,
+    value: Any, **kwargs: Any
+) -> Any:
+    original_type = type(value)
+    converted_value = convert(value)
+    if isinstance(converted_value, original_type):
+        return model_encoder(value, **kwargs)
+    return converted_value
 
-    def as_dict(self) -> dict[str, Any]:
-        return dataclasses.asdict(self)
 
-    def items(self) -> ItemsView[str, Any]:
-        return self.as_dict().items()
+class CMBMetaclass(ModelMetaclass):
+    def __new__(
+        cls,
+        name: str,
+        bases: tuple[type, ...],
+        namespace: dict[str, Any],
+        **kwargs: Any
+    ) -> type:
+        namespace[_CONTEXT] = pydantic.PrivateAttr()
+        if kwargs.pop("root", None):
+            return type.__new__(cls, name, bases, namespace, **kwargs)
+        new_class = super().__new__(cls, name, bases, namespace, **kwargs)
+        new_class.__json_encoder__ = functools.partial(
+            json_encoder,
+            new_class.__json_encoder__,
+        )
+        return new_class
+
+
+class ConfigModelBase(
+    pydantic.BaseSettings,
+    metaclass=CMBMetaclass,
+    root=True,
+):
+    """A configuration dictionary."""
 
     @classmethod
-    def get_defaults(cls) -> dict[str, Any]:
-        return config_convert({
-            field.name: field.default
-            for field in dataclasses.fields(cls)
-            if field.default is not dataclasses.MISSING
-        })
+    def _resolve_resource(
+        cls,
+        resource_argument: ConfigResource | ResourceT | None = None,
+        *,
+        create_if_missing: bool | None = None,
+    ) -> ConfigResource:
+        if resource_argument is None:
+            resource_argument = getattr(cls.__config__, "resource", None)
+        if resource_argument is None:
+            raise ValueError("No resource specified")
+        if not isinstance(resource_argument, ConfigResource):
+            resource = ConfigResource(resource_argument)
+        else:
+            resource = resource_argument
+        if create_if_missing is not None:
+            resource.create_if_missing = create_if_missing
+        return resource
 
     @property
     def was_loaded(self) -> bool:
         """Whether the configuration has been loaded.
 
         Returns
         -------
         bool
         """
-        return self._context.loaded
-
-    @property
-    def sections(self) -> dict[str, Any]:
-        """The configuration sections."""
-        return self._loader.sections
-
-    @sections.setter
-    def sections(self, value: dict[str, Any]) -> None:
-        """Set the configuration sections."""
-        self._loader.sections = value
+        return get_context(self).loaded
 
     @property
     def original(self) -> dict[str, Any]:
         """The original configuration dictionary."""
-        return self._context.original
+        return get_context(self).original
 
     def at(
-        self: BaseConfigT,
+        self: ConfigModelBaseT,
         route: str | list[str],
         *,
         parse_dotlist: bool = True,
-    ) -> ConfigAt[BaseConfigT]:
+    ) -> ConfigAt[ConfigModelBaseT]:
         """Return the configuration section metadata.
 
         Parameters
         ----------
         route
             Route to the key of the item.
 
@@ -711,154 +807,125 @@
             The item metadata.
         """
         if isinstance(route, str):
             if parse_dotlist:
                 [*route] = route.split(".")
             else:
                 route = [route]
-        return ConfigAt(self, route)
-
-    def update(  # type: ignore[override]
-        self,
-        data: Mapping[str, Any],
-        /,
-        **kw_data: Any,
-    ) -> None:
-        """Update the configuration with the given data, without loading."""
-        data = {**data, **kw_data}
-        for attr, value in data.items():
-            setattr(self, attr, value)
+        return ConfigAt(self, None, route)
 
     def rollback(self) -> None:
         """Rollback the configuration to its original state."""
-        self._context.loaded = False
-        self.update(self._context.original)
-        self._context.loaded = True
-
-    def __init_subclass__(
-        cls,
-        loader_factory: LoaderFactoryT = DefaultLoader.strict_with_sections,
-        *,
-        root: bool = False,
-        make_dataclass: bool = True,
-        **dataclass_params: Any,
-    ) -> None:
-        if root:
-            return
-        cls._loader_factory = loader_factory
-        if make_dataclass:
-            dataclasses.dataclass(cls, **dataclass_params)  # type: ignore
-
-
-@dataclass_transform()
-class Config(BaseConfig, root=True):
+        context = get_context(self)
+        context.loaded = False
+        self.__dict__ = context.original
+        context.loaded = True
 
-    def __call__(self: ConfigT, **new_config: Any) -> ConfigT:
-        """Update the configuration with the given configuration, with loading.
+    def _ensure_settings_with_context(
+        self,
+        name: str,
+        value: ConfigModelBaseT
+    ) -> ConfigModelBaseT:
+        context = get_context(self)
+        if (
+            context
+            # pydantic.BaseModel.__instancecheck__() and __subclasscheck__()...
+            and ConfigModelBase in type(value).mro()
+            and not hasattr(value, _CONTEXT)
+        ):
+            context.enter(name).bind_to(value)
+        return value
+
+    def __getattribute__(self, attr: str) -> Any:
+        value = super().__getattribute__(attr)
+        if isinstance(value, ConfigModelBase):
+            return self._ensure_settings_with_context(attr, value)
+        return value
 
-        Parameters
-        ----------
-        **new_config : Any
-            The configuration keyword arguments to update with.
 
-        Returns
-        -------
-        self
-        """
-        self.update(self._loader.load(new_config, self._context))
-        return self
+class ConfigModel(ConfigModelBase, root=True):
 
     @classmethod
     def load(
-        cls: type[ConfigT],
-        spec: ConfigSpec | str,
-        create_missing: bool | None = None,
+        cls: type[ConfigModelT],
+        resource: ConfigResource | ResourceT | None = None,
+        create_if_missing: bool | None = None,
         **kwargs: Any,
-    ) -> ConfigT:
+    ) -> ConfigModelT:
         """Load the configuration file.
         To reload the configuration, use the ``reload`` method.
 
         Parameters
         ----------
-        spec : ConfigSpec
-            The configuration specification.
-        create_missing : bool
+        resource : ConfigResource
+            The configuration resource to read from/write to.
+        create_if_missing : bool
             Whether to create the configuration file if it does not exist.
         **kwargs
             Keyword arguments to pass to the read method.
 
         Returns
         -------
         self
         """
-        if isinstance(spec, str):
-            spec = ConfigSpec.from_str(
-                spec,
-                defaults=cls.get_defaults(),
-            )
-        if create_missing is not None:
-            spec.create_missing = create_missing
-        kwargs.setdefault("mode", "r")
-        if create_missing:
-            kwargs.setdefault("create_kwds", {"mode": "w"})
-        loader = cls._loader
-        context: ConfigContext[ConfigT] = ConfigContext(spec)
-        data = loader.load(spec.read(**kwargs), context)
-        config = load(cls, data, context)
+        cls.update_forward_refs()
+        resource = cls._resolve_resource(resource, create_if_missing=create_if_missing)
+        context = Context(resource)  # type: Context[ConfigModelT]
+        config = resource.read(config_class=cls, **kwargs)
         context.owner = config
         context.loaded = True
-        context.original = config.as_dict()
+        context.original = config.dict()
         return config
 
-    def reload(self: ConfigT, **kwargs: Any) -> ConfigT:
+    def reload(self: ConfigModelT, **kwargs: Any) -> ConfigModelT:
         """Reload the configuration file.
         If the configuration is not loaded, a ValueError is raised.
 
         Parameters
         ----------
         **kwargs
             Keyword arguments to pass to the read method.
 
         Returns
         -------
         self
         """
-        if not self._context.loaded:
+        context = get_context(self)
+        if not context.loaded:
             msg = "Configuration has not been loaded, use load() instead"
             raise ValueError(msg)
-        if self._context.owner is self:
-            self._context.loaded = False
+        if context.owner is self:
+            context.loaded = False
             kwargs.setdefault("mode", "r")
-            kwargs.setdefault("create_kwds", {"mode": "w"})
-            new_config = self._context.spec.read(**kwargs)
-            self._context.original = new_config
-            config = cast(ConfigT, self(**new_config))
-            self._context.loaded = True
-            return config
-        msg = "partial reloading is not supported yet"
-        raise ValueError(msg)
+            new_config = context.resource.read(**kwargs)
+            context.bind_to(new_config)
+            context.original = new_config.dict()
+            new_config.rollback()
+            context.loaded = True
+            return new_config
+        return reload(context.section)
 
     def save(self, **kwargs: Any) -> int:
         """Save the configuration to the configuration file.
 
         Parameters
         ----------
         **kwargs
             Keyword arguments to pass to the write method.
 
         """
-        if self._context.owner is self:
-            data = self.as_dict()
-            blob = self._context.spec.engine.dump(data)
+        context = get_context(self)
+        if context.owner is self:
+            blob = context.resource.dump_config(self)
             result = self.write(blob, **kwargs)
-            self._context.original = data
+            context.original = self.dict()
             return result
-        return save(self._context.section)
+        return save(context.section)
 
-    def write(self, blob: str | ByteString, **kwargs: Any) -> int:
+    def write(self, blob: str | collections.abc.ByteString, **kwargs: Any) -> int:
         """Overwrite the configuration file with the given blob
         (config dump as string or bytes).
 
         Parameters
         ----------
         blob : str | bytes
             The blob to write to the configuration file.
@@ -866,121 +933,106 @@
             Keyword arguments to pass to the open method.
 
         Returns
         -------
         int
             The number of bytes written.
         """
-        if self._context.spec.is_url:
+        context = get_context(self)
+        if context.resource.is_url:
             msg = "Saving to URLs is not yet supported"
             raise NotImplementedError(msg)
         kwargs.setdefault("mode", "w")
-        return self._context.spec.write(blob, **kwargs)
-
+        return context.resource.write(blob, **kwargs)
 
-@dataclass_transform()
-class AsyncConfig(BaseConfig, root=True):
 
-    async def __call__(self: AsyncConfigT, **config: Any) -> AsyncConfigT:
-        """Update the configuration with the given configuration, asynchronously.
-
-        Parameters
-        ----------
-        config
-
-        Returns
-        -------
-
-        """
-        objects = await self._loader.load_async(config, self._context)
-        self.update(objects)
-        return self
+class AsyncConfigModel(ConfigModelBase, root=True):
 
     @classmethod
     async def load_async(
-        cls: type[AsyncConfigT],
-        spec: ConfigSpec | str,
+        cls: type[AsyncConfigModelT],
+        resource: ConfigResource | ResourceT | None,
         *,
-        create_missing: bool = False,
+        create_if_missing: bool = False,
         **kwargs: Any,
-    ) -> AsyncConfigT:
+    ) -> AsyncConfigModelT:
         """Load the configuration file asynchronously.
         To reload the configuration, use the ``reload`` method.
 
         Parameters
         ----------
-        spec : ConfigSpec
-            The configuration specification.
-        create_missing : bool
+        resource : ConfigResource
+            The configuration resource.
+        create_if_missing : bool
             Whether to create the configuration file if it does not exist.
         **kwargs
             Keyword arguments to pass to the read method.
 
         Returns
         -------
         self
         """
-        if isinstance(spec, str):
-            spec = ConfigSpec.from_str(spec, defaults=cls.get_defaults())
+        resource = cls._resolve_resource(resource, create_if_missing=create_if_missing)
         kwargs.setdefault("mode", "r")
-        if create_missing:
-            kwargs.setdefault("create_kwds", {"mode": "w"})
-        context: ConfigContext[AsyncConfigT] = ConfigContext(spec)
-        config = load(
-            cls,
-            await cls._loader.load_async(spec.read(**kwargs), context),
-            context,
-        )
+        context = Context(resource)  # type: Context[AsyncConfigModelT]
+        config = resource.read(config_class=cls, **kwargs)
         context.owner = config
         context.loaded = True
         return config
 
-    async def reload_async(self: AsyncConfigT, **kwargs: Any) -> AsyncConfigT:
+    async def reload_async(self: AsyncConfigModelT, **kwargs: Any) -> AsyncConfigModelT:
         """Reload the configuration file.
         If the configuration is not loaded, a ValueError is raised.
 
         Parameters
         ----------
         **kwargs
             Keyword arguments to pass to the read method.
 
         Returns
         -------
         self
         """
-        if not self._context.loaded:
+        context = get_context(self)
+        if not context.loaded:
             msg = "Configuration has not been loaded, use load() instead"
             raise ValueError(msg)
-        self._context.loaded = False
-        kwargs.setdefault("mode", "r")
-        kwargs.setdefault("create_kwds", {"mode": "w"})
-        new_async_config = await self._context.spec.read_async(**kwargs)
-        self._context.original = new_async_config
-        async_config = cast(AsyncConfigT, await self(**new_async_config))
-        self._context.loaded = True
-        return async_config
+        if context.owner is self:
+            context.loaded = False
+            kwargs.setdefault("mode", "r")
+            new_async_config = await context.resource.read_async(**kwargs)
+            context.bind_to(new_async_config)
+            context.original = new_async_config.dict()
+            self.rollback()
+            context.loaded = True
+            return new_async_config
+        return await reload_async(context.section)
 
     async def save_async(self, **kwargs: Any) -> int:
         """Save the configuration to the configuration file asynchronously.
 
         Parameters
         ----------
         **kwargs
             Keyword arguments to pass to the write method.
 
         """
-        if self._context.owner is self:
-            data = self.as_dict()
-            blob = self._context.spec.engine.dump(data)
+        context = get_context(self)
+        if context.owner is self:
+            blob = context.resource.dump_config(self)
             result = await self.write_async(blob, **kwargs)
-            self._context.original = data
+            context.original = self.dict()
             return result
-        return await save_async(self._context.section)
+        return await save_async(context.section)
 
-    async def write_async(self, blob: str | ByteString, **kwargs: Any) -> int:
+    async def write_async(
+        self,
+        blob: str | collections.abc.ByteString,
+        **kwargs: Any
+    ) -> int:
         """Overwrite the configuration file asynchronously with the given blob
         (config dump as string or bytes).
 
         Parameters
         ----------
         blob : str | bytes
             The blob to write to the configuration file.
@@ -988,27 +1040,17 @@
             Keyword arguments to pass to the open method.
 
         Returns
         -------
         int
             The number of bytes written.
         """
-        if self._context.spec.is_url:
+        context = get_context(self)
+        if context.resource.is_url:
             msg = "Saving to URLs is not yet supported"
             raise NotImplementedError(msg)
         kwargs.setdefault("mode", "w")
-        return await self._context.spec.write_async(blob, **kwargs)
-
-
-def config_load(
-    cls: type[BaseConfigT],
-    value: MutableMapping[str, Any],
-    context: ConfigContext[BaseConfigT],
-) -> BaseConfigT:
-    value = cls._loader.load(value, context)
-    config = dataclass_load(cls, value, context)
-    context.bind_to(config)
-    return config
+        return await context.resource.write_async(blob, **kwargs)
 
 
-def config_convert(config: MutableMapping[str, Any]) -> dict[str, Any]:
-    return {key: convert(value) for key, value in config.items()}
+class Meta(pydantic.BaseSettings.Config):
+    resource: ConfigResource | str | None = None
```

### Comparing `configzen-0.1.0/LICENSE` & `configzen-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.1.0/pyproject.toml` & `configzen-0.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 [tool.poetry]
 name = "configzen"
-version = "0.1.0"
+version = "0.1.1"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 typing-extensions = {version = "^4.5.0", python = ">=3.9,<3.11"}
 pyyaml = {version = "^6.0", optional = true}
 orjson = {version = "^3.8.12", optional = true}
+pydantic = "^1.10.7"
+anyconfig = "^0.13.0"
 
 [tool.poetry.extras]
 yaml = ["pyyaml"]
 json = ["orjson"]
 
 [build-system]
 requires = ["poetry-core"]
```

