# Comparing `tmp/configzen-0.1.2.tar.gz` & `tmp/configzen-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.1.2.tar", max compression
+gzip compressed data, was "configzen-0.1.3.tar", max compression
```

## Comparing `configzen-0.1.2.tar` & `configzen-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      135 2023-05-14 02:04:46.442804 configzen-0.1.2/configzen/__init__.py
--rw-r--r--   0        0        0    32122 2023-05-14 02:36:01.959219 configzen-0.1.2/configzen/config.py
--rw-r--r--   0        0        0      853 2023-05-14 02:32:13.602772 configzen-0.1.2/configzen/errors.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.2/LICENSE
--rw-r--r--   0        0        0      590 2023-05-14 02:44:13.804655 configzen-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2434 2023-05-14 02:41:15.994125 configzen-0.1.2/README.md
--rw-r--r--   0        0        0     3277 1970-01-01 00:00:00.000000 configzen-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      135 2023-05-14 02:04:46.442804 configzen-0.1.3/configzen/__init__.py
+-rw-r--r--   0        0        0    44763 2023-05-14 04:18:18.892124 configzen-0.1.3/configzen/config.py
+-rw-r--r--   0        0        0      925 2023-05-14 03:58:18.183363 configzen-0.1.3/configzen/errors.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.3/configzen/py.typed
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.3/LICENSE
+-rw-r--r--   0        0        0      702 2023-05-14 04:31:39.025554 configzen-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3029 2023-05-14 04:41:22.077344 configzen-0.1.3/README.md
+-rw-r--r--   0        0        0     3872 1970-01-01 00:00:00.000000 configzen-0.1.3/PKG-INFO
```

### Comparing `configzen-0.1.2/configzen/config.py` & `configzen-0.1.3/configzen/config.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,63 @@
-"""Core configuration classes and functions."""
+"""
+The core module of the _configzen_ library.
+
+This module provides a way to manage configuration files and resources
+in a consistent way. It also provides a way to load and save configuration
+files in a type-safe way.
+
+.. code-block:: python
+
+    from configzen import ConfigModel, ConfigResource, Meta
+
+    class DatabaseConfig(ConfigModel):
+        host: str
+        port: int
+        user: str
+        password: str = Field(exclude=True)
+
+        class Config(Meta):
+            resource = "examples/database.json"
+
+    db_config = DatabaseConfig.load()
+    db_config.host = "newhost"
+    db_config.port = 5432
+
+    db_config.save()
+
+    db_config = DatabaseConfig.load()
+    print(db_config.host)
+    print(db_config.port)
+
+    # Output:
+    # newhost
+    # 5432
+
+    db_config.host = "otherhost"
+    db_config.port = 5433
+
+    db_config.at("host").save()
+
+    print(db_config.host)
+    print(db_config.port)
+
+    # Output:
+    # otherhost
+    # 5432  # <- not 5433, because we saved only host
+
+    db_config.host = "anotherhost"
+    db_config.at("port").reload()
+
+    print(db_config.host)
+    print(db_config.port)
+
+    # Output:
+    # otherhost  # <- not anotherhost, because we reloaded only port
+    # 5432
+"""
 
 from __future__ import annotations
 
 import abc
 import collections.abc
 import contextlib
 import copy
@@ -10,23 +65,15 @@
 import functools
 import io
 import os
 import pathlib
 import urllib.parse
 import urllib.request
 from collections.abc import Callable, Generator
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Generic,
-    Literal,
-    NamedTuple,
-    TypeVar,
-    cast,
-)
+from typing import TYPE_CHECKING, Any, Generic, Literal, NamedTuple, TypeVar, cast
 
 import anyconfig
 import pydantic
 from pydantic.main import ModelMetaclass
 
 from configzen.errors import ConfigItemAccessError, UnknownParserError
 
@@ -67,15 +114,15 @@
 
 ContextT = TypeVar("ContextT", bound="AnyContext")
 ConfigModelBaseT = TypeVar("ConfigModelBaseT", bound="ConfigModelBase")
 ConfigModelT = TypeVar("ConfigModelT", bound="ConfigModel")
 AsyncConfigModelT = TypeVar("AsyncConfigModelT", bound="AsyncConfigModel")
 
 OpenedT = contextlib.AbstractContextManager
-ResourceT = OpenedT | str | os.PathLike | pathlib.Path
+RawResourceT = OpenedT | str | os.PathLike | pathlib.Path
 
 
 def _get_defaults_from_model_class(
     model: type[pydantic.BaseSettings],
 ) -> dict[str, Any]:
     defaults = {}
     for field in model.__fields__.values():
@@ -102,27 +149,67 @@
         hasattr(obj, "_asdict") and
         hasattr(obj, "_fields")
     )
 
 
 @functools.singledispatch
 def convert(obj: Any) -> Any:
-    """Convert a value to a format that can be safely serialized."""
+    """
+    Convert a value to a format that can be safely serialized.
+
+    This function is used to convert values that are not supported by
+    `anyconfig` to a format that can be safely serialized. It is used
+    internally by `ConfigModel` and `AsyncConfigModel` to convert
+    values before saving them to a file.
+
+    Parameters
+    ----------
+    obj
+        The value to convert.
+
+    Returns
+    -------
+    Any
+    """
     if dataclasses.is_dataclass(obj):
         return dataclasses.asdict(obj)
     if _is_namedtuple(obj):
         return convert_namedtuple(obj)
     return obj
 
 
 _convert_register = convert.register
 
 
 def converter(func: Callable[[T], Any], cls: type[T] | None = None) -> type[T] | Any:
-    """Register a converter function for a type."""
+    """
+    Register a converter function for a type.
+
+    Parameters
+    ----------
+    func
+        The converter function.
+
+    cls
+        The type to register the converter for.
+        Optional for the decoration syntax.
+
+    Returns
+    -------
+    The conversion result class.
+
+    Usage
+    -----
+    .. code-block:: python
+
+        @converter(converter_func)
+        class MyClass:
+            ...
+
+    """
     if cls is None:
         return functools.partial(converter, func)
 
     _convert_register(cls, func)
 
     if not hasattr(cls, "__get_validators__"):
         def validator_gen() -> Generator[Callable[[Any], Any], None, None]:
@@ -131,42 +218,98 @@
         cls.__get_validators__ = validator_gen  # type: ignore[attr-defined]
 
     return cls
 
 
 @functools.singledispatch
 def load(cls: Any, value: Any) -> Any:
+    """
+    Load a value into a type.
+
+    This function is used to load values that are not supported by
+    `anyconfig` to a format that can be used at runtime. It is used
+    by pydantic while performing validation.
+
+    Parameters
+    ----------
+    cls
+        The type to load the value into.
+
+    value
+        The value to load.
+
+    Returns
+    -------
+    The loaded value.
+    """
     if isinstance(value, cls):
         return value
     return cls(value)
 
 
 def loader(func: Callable[[Any], T], cls: type[T] | None = None) -> type[T] | Any:
-    """Register a loader function for a type."""
+    """
+    Register a loader function for a type.
+
+    Parameters
+    ----------
+    func
+        The loader function.
+    cls
+        The type to register the loader for.
+
+    Returns
+    -------
+    The loading result class.
+    """
+
     if cls is None:
         return functools.partial(loader, func)
 
     load.register(cls, func)
     return cls
 
 
 @convert.register
 def convert_mapping(obj: collections.abc.Mapping) -> dict[str, Any]:
+    """
+    Convert a mapping to safely-serializable form.
+
+    Parameters
+    ----------
+    obj
+        The mapping to convert.
+
+    Returns
+    -------
+    The converted mapping.
+    """
     return {k: convert(v) for k, v in obj.items()}
 
 
 @functools.singledispatch
 def convert_namedtuple(obj: tuple) -> dict[str, Any]:
+    """
+    Convert a namedtuple to safely-serializable form.
+
+    Parameters
+    ----------
+    obj
+        The namedtuple to convert.
+
+    Returns
+    -------
+    The converted namedtuple (likely a list).
+    """
     # Initially I wanted it to be convert(obj._asdict()), but
     # pydantic doesn't seem to be friends with custom NamedTuples.
     return convert(list(obj))
 
 
-def split_ac_options(options: dict[str, Any]) -> tuple[dict[str, Any], dict[str, Any]]:
-    """Split a dictionary of options into those for loading and those for dumping."""
+def _split_ac_options(options: dict[str, Any]) -> tuple[dict[str, Any], dict[str, Any]]:
     load_options: dict[str, Any] = {}
     dump_options: dict[str, Any] = {}
     for key, value in options.items():
         final_key = key
         if key.startswith("dump_"):
             final_key = key.removeprefix("dump_")
             targets = [dump_options]
@@ -184,28 +327,65 @@
                 raise ValueError(msg)
             target[final_key] = value
 
     return load_options, dump_options
 
 
 class ConfigResource:
-    """A configuration resource to read from/write to."""
+    """
+    A configuration resource.
+
+    This class is used to represent a configuration resource, which
+    can be a file, a URL, or a file-like object. It is used internally
+    by `ConfigModel` and `AsyncConfigModel` to load and save
+    configuration files.
+
+    Parameters
+    ----------
+    resource
+        The resource to load the configuration from.
+    ac_parser
+        The name of the engines to use for loading and saving the
+        configuration. If not specified, the parser will be guessed
+        from the file extension.
+    create_if_missing
+        Whether to create the file if it doesn't exist.
+    use_pydantic_json
+        Whether to use pydantic's JSON serialization for saving the
+        configuration. This is useful for preserving the type of
+        values that are not supported by `anyconfig`.
+    options
+        Additional options to pass to `anyconfig` API functions.
+
+    Attributes
+    ----------
+    create_if_missing
+        Whether to create the file if it doesn't exist.
+    ac_parser
+        The name of the engines to use for loading and saving the
+        configuration. If not specified, the parser will be guessed
+        from the file extension.
+    allowed_url_schemes
+        The URL schemes that are allowed to be used.
+
+    Raises
+    ------
+    ValueError
+    """
 
     _resource: OpenedT | str | os.PathLike | pathlib.Path
-    defaults: dict[str, Any]
     create_if_missing: bool
     ac_parser: str | None
     _ac_load_options: dict[str, Any]
     _ac_dump_options: dict[str, Any]
-    cache_engine: bool
     allowed_url_schemes: set[str] = _URL_SCHEMES
 
     def __init__(
         self: ConfigResource,
-        resource: ResourceT,
+        resource: RawResourceT,
         ac_parser: str | None = None,
         *,
         create_if_missing: bool = False,
         use_pydantic_json: bool = True,
         **options: Any,
     ) -> None:
         """Parameters
@@ -220,26 +400,55 @@
         use_pydantic_json : bool, optional
             Whether to use Pydantic's JSON encoder/decoder instead of the default
             anyconfig one.
         **options
             Additional keyword arguments to pass to
             `anyconfig.loads()` and `anyconfig.dumps()`.
         """
+        if (
+            not options.get("ac_safe")
+            and options.get("load_ac_safe") is None
+            and options.get("dump_ac_safe") is None
+        ):
+            # Business is business.
+            options["ac_safe"] = True
         self.ac_parser = ac_parser
         self.resource = resource
         self.create_if_missing = create_if_missing
         self.use_pydantic_json = use_pydantic_json
-        self._ac_load_options, self._ac_dump_options = split_ac_options(options)
+        self._ac_load_options, self._ac_dump_options = _split_ac_options(options)
 
     @property
-    def resource(self) -> ResourceT:
+    def resource(self) -> RawResourceT:
+        """
+        The resource of the configuration.
+
+        This can be a file path, a URL, or a file-like object.
+
+        Returns
+        -------
+        The resource of the configuration.
+        """
         return self._resource
 
     @resource.setter
-    def resource(self, value: ResourceT) -> None:
+    def resource(self, value: RawResourceT) -> None:
+        """
+        The resource of the configuration.
+
+        This can be a file path, a URL, or a file-like object.
+
+        .. note::
+            If the resource is a file path, the parser will be guessed
+            from the file extension.
+
+        Returns
+        -------
+        The resource of the configuration.
+        """
         self._resource = value
         self.ac_parser = self.ac_parser or self._guess_ac_parser()
 
     def _guess_ac_parser(self) -> str | None:
         ac_parser = None
         if isinstance(self.resource, str):
             ac_parser = pathlib.Path(self.resource).suffix[1:].casefold()
@@ -253,75 +462,148 @@
     def load_into(
         self,
         config_class: type[ConfigModelBaseT],
         blob: str,
         ac_parser: str | None = None,
         **kwargs: Any,
     ) -> ConfigModelBaseT:
+        """
+        Load the configuration into a `ConfigModel` subclass.
+
+        Parameters
+        ----------
+        config_class
+            The `ConfigModel` subclass to load the configuration into.
+        blob
+            The configuration to load.
+        ac_parser
+            The name of the engines to use for loading the configuration.
+        **kwargs
+            Additional keyword arguments to pass to `anyconfig.loads()`.
+
+        Returns
+        -------
+        The loaded configuration.
+        """
         config = self.load_into_dict(blob, ac_parser=ac_parser, **kwargs)
         if config is None:
             config = {}
         return config_class(**config)
 
     def load_into_dict(
         self,
         blob: str,
         ac_parser: str | None = None,
         **kwargs: Any,
-    ) -> dict[str, Any]:
+    ) -> dict[str, Any] | None:
+        """
+        Load the configuration into a dictionary. The dictionary is
+        usually used to initialize a `ConfigModel` subclass. If the
+        configuration is empty, None might be returned instead of a dictionary.
+
+        Parameters
+        ----------
+        blob
+            The configuration to load.
+        ac_parser
+            The name of the anyconfig parser to use for loading the configuration.
+        **kwargs
+            Additional keyword arguments to pass to `anyconfig.loads()`.
+
+        Returns
+        -------
+        The loaded configuration dictionary.
+        """
         if ac_parser is None:
             ac_parser = self.ac_parser
         kwargs = {**self._ac_load_options, **kwargs}
         return anyconfig.loads(blob, ac_parser=ac_parser, **kwargs)
 
     def dump_config(
         self,
         config: ConfigModelBaseT,
         ac_parser: str | None = None,
         **kwargs: Any,
     ) -> str:
+        """
+        Dump the configuration to a string.
+
+        Parameters
+        ----------
+        config
+            The configuration to dump.
+        ac_parser
+            The name of the anyconfig parser to use for saving the configuration.
+        **kwargs
+            Additional keyword arguments to pass to `anyconfig.dumps()`.
+
+        Returns
+        -------
+        The dumped configuration.
+        """
         if ac_parser is None:
             ac_parser = self.ac_parser
         if ac_parser == "json" and self.use_pydantic_json:
             return config.json(**kwargs)
         data = config.dict()
         return self.dump_data(data, ac_parser=ac_parser, **kwargs)
 
     def dump_data(
         self,
         data: dict[str, Any],
         ac_parser: str | None = None,
         **kwargs: Any,
     ) -> str:
+        """
+        Dump data to a string.
+
+        Parameters
+        ----------
+        data
+            The data to dump.
+        ac_parser
+            The name of the anyconfig parser to use for saving the configuration.
+        kwargs
+            Additional keyword arguments to pass to `anyconfig.dumps()`.
+
+        Returns
+        -------
+        The dumped configuration.
+        """
         if ac_parser is None:
             ac_parser = self.ac_parser
         kwargs = {**self._ac_dump_options, **kwargs}
         return anyconfig.dumps(
             convert(data),
             ac_parser=ac_parser,
             **kwargs,
         )
 
     @property
     def is_url(self) -> bool:
-        """Whether the entrypoint is a URL."""
+        """Whether the resource is a URL."""
         return (
             isinstance(self.resource, str)
             and urllib.parse.urlparse(self.resource).scheme in _URL_SCHEMES
         )
 
     def open_resource(self, **kwds: Any) -> OpenedT:
-        """Open the configuration file.
+        """
+        Open the configuration file.
 
         Parameters
         ----------
         **kwds
             Keyword arguments to pass to the opening routine.
             For URLs, these are passed to ``urllib.request.urllib.request.urlopen()``.
             For local files, these are passed to ``builtins.open()``.
+
+        Returns
+        -------
+        The opened resource.
         """
         if self.resource is None:
             return io.StringIO()
         if self.is_url:
             url = cast(str, self.resource)
             if urllib.parse.urlparse(url).scheme not in self.allowed_url_schemes:
                 msg = (
@@ -333,20 +615,25 @@
                 urllib.request.Request(url), **kwds
             )
         if isinstance(self.resource, str | os.PathLike | pathlib.Path):
             return pathlib.Path(self.resource).open(**kwds)
         return self.resource
 
     def open_resource_async(self, **kwds: Any) -> Any:
-        """Open the configuration file asynchronously.
+        """
+        Open the configuration file asynchronously.
 
         Parameters
         ----------
         **kwds
             Keyword arguments to pass to the opening routine.
+
+        Returns
+        -------
+        The opened resource.
         """
         if self.is_url:
             msg = "asynchronous URL opening is not supported"
             raise NotImplementedError(msg)
         if not AIOFILES_AVAILABLE:
             msg = (
                 "aiofiles is not available, cannot open file "
@@ -374,24 +661,30 @@
     def read(
         self,
         *,
         config_class: type[ConfigModelBaseT],
         create_kwargs: dict[str, Any] | None = None,
         **kwargs: Any,
     ) -> ConfigModelBaseT:
-        """Read the configuration file.
+        """
+        Read the configuration file.
 
         Parameters
         ----------
         config_class
-        create_kwargs : dict, optional
+            The configuration model class to load the configuration into.
+        create_kwargs
             Keyword arguments to pass to the open method
             when optionally creating the file.
         **kwargs
             Keyword arguments to pass to the open method.
+
+        Returns
+        -------
+        The loaded configuration.
         """
         kwargs = self._get_default_kwargs("read", kwargs=kwargs)
         try:
             with self.open_resource(**kwargs) as fp:
                 blob = fp.read()
         except FileNotFoundError:
             blob = None
@@ -399,34 +692,55 @@
                 defaults = _get_defaults_from_model_class(config_class)
                 blob = self.dump_data(defaults)
                 create_kwargs = self._get_default_kwargs("write", kwargs=create_kwargs)
                 self.write(blob, **create_kwargs)
         return self.load_into(config_class, blob, **self._ac_load_options)
 
     def write(self, blob: str | collections.abc.ByteString, **kwds: Any) -> int:
+        """
+        Write the configuration file.
+
+        Parameters
+        ----------
+        blob
+            The string/bytes to write into the resource.
+        kwds
+            Keyword arguments to pass to the opening routine.
+
+        Returns
+        -------
+        The number of bytes written.
+        """
+        kwds = self._get_default_kwargs("write", kwds)
         with self.open_resource(**kwds) as fp:
             return fp.write(blob)
 
     async def read_async(
         self,
         *,
         config_class: type[AsyncConfigModelT],
         create_kwargs: dict[str, Any] | None = None,
         **kwargs: Any,
     ) -> AsyncConfigModelT:
-        """Read the configuration file asynchronously.
+        """
+        Read the configuration file asynchronously.
 
         Parameters
         ----------
         config_class
-        create_kwargs : dict, optional
+            The configuration model class to load the configuration into.
+        create_kwargs
             Keyword arguments to pass to the open method
             when optionally creating the file.
         **kwargs
             Keyword arguments to pass to the open method.
+
+        Returns
+        -------
+        The loaded configuration.
         """
         kwargs = self._get_default_kwargs("read", kwargs=kwargs)
         try:
             async with self.open_resource_async(**kwargs) as fp:
                 blob = await fp.read()
         except FileNotFoundError:
             if self.create_if_missing:
@@ -436,14 +750,28 @@
                 await self.write_async(blob, **create_kwargs)
         return self.load_into(config_class, blob, **self._ac_load_options)
 
     async def write_async(
         self,
         blob: str | collections.abc.ByteString, **kwds: Any,
     ) -> int:
+        """
+        Write the configuration file asynchronously.
+
+        Parameters
+        ----------
+        blob
+            The string/bytes to write into the resource.
+        kwds
+            Keyword arguments to pass to the opening routine.
+
+        Returns
+        -------
+        The number of bytes written.
+        """
         async with self.open_resource_async(**kwds) as fp:
             return await fp.write(blob)
 
 
 if TYPE_CHECKING:
 
     class ConfigAt(NamedTuple, Generic[ConfigModelBaseT]):
@@ -462,168 +790,367 @@
 
         def save(self) -> int:
             ...
 
 
 else:
     class ConfigAt(NamedTuple):
-        """Metadata for a configuration item."""
+        """
+        A configuration item at a specific location.
+
+        Attributes
+        ----------
+        owner
+            The configuration model instance.
+        mapping
+            The mapping to use.
+        route
+            The route to the item.
+        """
 
         owner: ConfigModelBaseT
         mapping: dict[str, Any] | None
         route: list[str]
 
         def get(self) -> Any:
+            """
+            Get the value of the item.
+
+            Returns
+            -------
+            The value of the item.
+            """
             scope = _vars(self.mapping or self.owner.dict())
             route_here = []
             try:
                 for part in self.route:
                     route_here.append(part)
                     scope = _vars(scope)[part]
             except KeyError:
                 raise ConfigItemAccessError(self.owner, route_here) from None
             return scope
 
         def update(self, value: Any) -> collections.abc.MutableMapping:
+            """
+            Update the value of the item with regard to this item mapping.
+
+            Parameters
+            ----------
+            value
+                The new value.
+
+            Returns
+            -------
+            The updated mapping.
+            """
             route = list(self.route)
             mapping = self.mapping or self.owner.dict()
             key = route.pop()
             submapping = _vars(mapping)
             route_here = []
             try:
                 for part in route:
                     route_here.append(part)
                     submapping = _vars(submapping[part])
                 submapping[key] = value
             except KeyError:
                 raise ConfigItemAccessError(self.owner, route_here) from None
             return mapping
 
-        async def save_async(self) -> int:
-            return await save_async(self)
+        async def save_async(self, **kwargs: Any) -> int:
+            """
+            Save the configuration asynchronously.
+
+            Parameters
+            ----------
+            **kwargs
+                Keyword arguments to pass to the saving function.
 
-        def save(self) -> int:
-            return save(self)
-
-        async def reload_async(self) -> Any:
-            return await reload_async(self)
+            Returns
+            -------
+            The number of bytes written.
+            """
+            return await save_async(self, **kwargs)
 
-        def reload(self) -> Any:
-            return reload(self)
+        def save(self, **kwargs: Any) -> int:
+            """
+            Save the configuration.
+
+            Parameters
+            ----------
+            **kwargs
+                Keyword arguments to pass to the saving function.
 
+            Returns
+            -------
+            The number of bytes written.
+            """
+            return save(self, **kwargs)
 
-def save(section: ConfigModelT | ConfigAt) -> int:
+        async def reload_async(self, **kwargs: Any) -> Any:
+            """
+            Reload the configuration asynchronously.
+
+            Parameters
+            ----------
+            kwargs
+                Keyword arguments to pass to the reloading function.
+
+            Returns
+            -------
+            The reloaded configuration or its belonging item.
+            """
+            return await reload_async(self, **kwargs)
+
+        def reload(self, **kwargs: Any) -> Any:
+            """
+            Reload the configuration.
+
+            Parameters
+            ----------
+            kwargs
+                Keyword arguments to pass to the reloading function.
+
+            Returns
+            -------
+            The reloaded configuration or its belonging item.
+            """
+            return reload(self, **kwargs)
+
+
+def save(section: ConfigModelT | ConfigAt, **kwargs: Any) -> int:
+    """
+    Save the configuration.
+
+    Parameters
+    ----------
+    section
+        The configuration model instance or the configuration item.
+    **kwargs
+        Keyword arguments to pass to the saving function.
+
+    Returns
+    -------
+    The number of bytes written.
+    """
     if isinstance(section, ConfigModel):
         config = section
         return config.save()
 
     config = section.owner
-    data = config.original
+    data = config.initial_state
     at = ConfigAt(config, data, section.route)
     data = at.update(section.get())
     context = get_context(config)
     blob = context.resource.dump_config(config.copy(update=data))
-    result = config.write(blob)
-    context.original = data
+    result = config.write(blob, **kwargs)
+    context.initial_state = data
     return result
 
 
-async def save_async(section: AsyncConfigModelT | ConfigAt) -> int:
+async def save_async(section: AsyncConfigModelT | ConfigAt, **kwargs: Any) -> int:
+    """
+    Save the configuration asynchronously.
+
+    Parameters
+    ----------
+    section
+        The configuration model instance or the configuration item.
+    **kwargs
+        Keyword arguments to pass to the saving function.
+
+    Returns
+    -------
+    The number of bytes written.
+    """
     if isinstance(section, AsyncConfigModel):
         config = section
-        return await config.save_async()
+        return await config.save_async(**kwargs)
 
     config = section.owner
-    data = config.original
+    data = config.initial_state
     at = ConfigAt(config, data, section.route)
     data = at.update(section.get())
     context = get_context(config)
     blob = context.resource.dump_config(config.copy(update=data))
-    result = await config.write_async(blob)
-    context.original = data
+    result = await config.write_async(blob, **kwargs)
+    context.initial_state = data
     return result
 
 
-def reload(section: ConfigModelT | ConfigAt) -> Any:
+def reload(section: ConfigModelT | ConfigAt, **kwargs: Any) -> Any:
+    """
+    Reload the configuration.
+
+    Parameters
+    ----------
+    section
+        The configuration model instance or the configuration item.
+    **kwargs
+        Keyword arguments to pass to the reloading function.
+
+    Returns
+    -------
+    The reloaded configuration or its belonging item.
+    """
     if isinstance(section, ConfigModel):
         config = section
         return config.reload()
 
     config = section.owner
     context = get_context(config)
     data = config.dict()
-    newest = context.resource.read(config_class=type(config))
+    newest = context.resource.read(config_class=type(config), **kwargs)
     section_data = ConfigAt(newest, newest.dict(), section.route).get()
     new_mapping = ConfigAt(config, data, section.route).update(section_data)
     config.__dict__.update(new_mapping)
     return section_data
 
 
-async def reload_async(section: AsyncConfigModelT | ConfigAt) -> Any:
+async def reload_async(section: AsyncConfigModelT | ConfigAt, **kwargs: Any) -> Any:
+    """
+    Reload the configuration asynchronously.
+
+    Parameters
+    ----------
+    section
+        The configuration model instance or the configuration item.
+    kwargs
+        Keyword arguments to pass to the reloading function.
+
+    Returns
+    -------
+    The reloaded configuration or its belonging item.
+    """
     if isinstance(section, AsyncConfigModel):
         config = section
         return await config.reload_async()
 
     config = section.owner
     context = get_context(config)
     data = config.dict()
-    newest = await context.resource.read_async(config_class=type(config))
+    newest = await context.resource.read_async(config_class=type(config), **kwargs)
     section_data = ConfigAt(newest, newest.dict(), section.route).get()
     new_mapping = ConfigAt(config, data, section.route).update(section_data)
     config.__dict__.update(new_mapping)
     return new_mapping
 
 
 class AnyContext(abc.ABC, Generic[ConfigModelBaseT]):
-    original: dict[str, Any]
-    _original: dict[str, Any]
-    loaded: bool
+    """
+    The base class for configuration context.
+    Contexts are used to
+    - store configuration resource information,
+    - link configuration items to the configuration models they belong to,
+    - keep track of the route leading to particular configuration
+      items that are also ConfigModel subclasses.
+
+    Attributes
+    ----------
+    initial_state
+        The initial configuration state.
+
+    """
+    initial_state: dict[str, Any]
+    _initial_state: dict[str, Any]
 
     @abc.abstractmethod
     def trace_route(self) -> collections.abc.Generator[str, None, None]:
         """Trace the route to the configuration context."""
 
     @staticmethod
     def get(config: ConfigModelBaseT) -> AnyContext[ConfigModelBaseT]:
+        """
+        Get the context of the configuration model.
+
+        Parameters
+        ----------
+        config
+            The configuration model instance.
+
+        Returns
+        -------
+        The context of the configuration model.
+        """
         return object.__getattribute__(config, _CONTEXT)
 
     def bind_to(self, config: ConfigModelBaseT) -> None:
+        """
+        Bind the context to the configuration model.
+
+        Parameters
+        ----------
+        config
+            The configuration model instance.
+
+        Returns
+        -------
+        None
+        """
         if config is None:
             return
         object.__setattr__(config, _CONTEXT, self)
 
-    def enter(self, key: str) -> Subcontext[ConfigModelBaseT]:
-        return Subcontext(self, key)
+    def enter(self, part: str) -> Subcontext[ConfigModelBaseT]:
+        """
+        Enter a subcontext.
+
+        Parameters
+        ----------
+        part
+            The name of the item nested in the item this context points to.
+
+        Returns
+        -------
+        The new subcontext.
+        """
+        return Subcontext(self, part)
 
     @property
     @abc.abstractmethod
     def resource(self) -> ConfigResource:
-        ...
+        """The configuration resource."""
 
     @property
     @abc.abstractmethod
     def owner(self) -> ConfigModelBaseT | None:
-        ...
+        """
+        The top-level configuration model instance,
+        holding all adjacent contexts.
+        """
 
     @property
     @abc.abstractmethod
     def section(self) -> ConfigModelBaseT | ConfigAt[ConfigModelBaseT]:
-        ...
+        """
+        The configuration model instance or the configuration item
+        this context points to.
+        """
 
 
 class Context(AnyContext, Generic[ConfigModelBaseT]):
+    """
+    The context of a configuration model.
+
+    Parameters
+    ----------
+    resource
+        The configuration resource.
+    owner
+        The top-level configuration model instance,
+        holding all belonging subcontexts.
+    """
     def __init__(
         self,
         resource: ConfigResource,
         owner: ConfigModelBaseT | None = None,
     ) -> None:
         self._resource = resource
         self._owner = None
-        self._original = {}
-        self._loaded = False
+        self._initial_state = {}
 
         self.owner = owner
 
     def trace_route(self) -> collections.abc.Generator[str, None, None]:
         yield from ()
 
     @property
@@ -642,88 +1169,95 @@
     def owner(self, config: ConfigModelBaseT | None) -> None:
         if config is None:
             return
         self.bind_to(config)
         self._owner = config
 
     @property
-    def original(self) -> dict[str, Any]:
-        return copy.deepcopy(self._original)
-
-    @original.setter
-    def original(self, original: dict[str, Any]) -> None:
-        self._original = copy.deepcopy(original)
-
-    @property
-    def loaded(self) -> bool:
-        return self._loaded
+    def initial_state(self) -> dict[str, Any]:
+        return copy.deepcopy(self._initial_state)
 
-    @loaded.setter
-    def loaded(self, value: bool) -> None:
-        self._loaded = value
+    @initial_state.setter
+    def initial_state(self, initial_state: dict[str, Any]) -> None:
+        self._initial_state = copy.deepcopy(initial_state)
 
 
 class Subcontext(AnyContext, Generic[ConfigModelBaseT]):
-    def __init__(self, parent: AnyContext[ConfigModelBaseT], key: str) -> None:
-        self.parent = parent
-        self.key = key
+    """
+    The subcontext of a configuration model.
+
+    Parameters
+    ----------
+    parent
+        The parent context.
+    part
+        The name of the item nested in the item the parent context points to.
+    """
+
+    def __init__(self, parent: AnyContext[ConfigModelBaseT], part: str) -> None:
+        self._parent = parent
+        self._part = part
 
     @property
     def resource(self) -> ConfigResource:
-        return self.parent.resource
+        return self._parent.resource
 
     def trace_route(self) -> collections.abc.Generator[str, None, None]:
-        yield from self.parent.trace_route()
-        yield self.key
+        yield from self._parent.trace_route()
+        yield self._part
 
     @property
     def section(self) -> ConfigAt[ConfigModelBaseT]:
         if self.owner is None:
             msg = "Cannot get section for unbound context"
             raise ValueError(msg)
         return ConfigAt(self.owner, None, list(self.trace_route()))
 
     @property
     def owner(self) -> ConfigModelBaseT | None:
-        return self.parent.owner
-
-    @property
-    def original(self) -> dict[str, Any]:
-        return self.parent.original
-
-    @original.setter
-    def original(self, value: dict[str, Any]) -> None:
-        data = self.parent.original
-        data[self.key] = copy.deepcopy(value)
-        self.parent.original = data
+        return self._parent.owner
 
     @property
-    def loaded(self) -> bool:
-        return self.parent.loaded
+    def initial_state(self) -> dict[str, Any]:
+        return self._parent.initial_state
 
-    @loaded.setter
-    def loaded(self, value: bool) -> None:
-        self.parent.loaded = value
+    @initial_state.setter
+    def initial_state(self, value: dict[str, Any]) -> None:
+        data = self._parent.initial_state
+        data[self._part] = copy.deepcopy(value)
+        self._parent.initial_state = data
 
 
 def get_context(config: ConfigModelBaseT) -> AnyContext[ConfigModelBaseT]:
+    """
+    Get the context of the configuration model.
+
+    Parameters
+    ----------
+    config
+        The configuration model instance.
+
+    Returns
+    -------
+    The context of the configuration model.
+    """
     context = AnyContext.get(config)
     if context is None:
         msg = "Cannot get context for unbound configuration"
         raise RuntimeError(msg)
     return context
 
 
-def json_encoder(
+def _json_encoder(
     model_encoder: Callable,
     value: Any, **kwargs: Any
 ) -> Any:
-    original_type = type(value)
+    initial_state_type = type(value)
     converted_value = convert(value)
-    if isinstance(converted_value, original_type):
+    if isinstance(converted_value, initial_state_type):
         return model_encoder(value, **kwargs)
     return converted_value
 
 
 class CMBMetaclass(ModelMetaclass):
     def __new__(
         cls,
@@ -733,31 +1267,36 @@
         **kwargs: Any
     ) -> type:
         namespace[_CONTEXT] = pydantic.PrivateAttr()
         if kwargs.pop("root", None):
             return type.__new__(cls, name, bases, namespace, **kwargs)
         new_class = super().__new__(cls, name, bases, namespace, **kwargs)
         new_class.__json_encoder__ = functools.partial(
-            json_encoder,
+            _json_encoder,
             new_class.__json_encoder__,
         )
         return new_class
 
 
 class ConfigModelBase(
     pydantic.BaseSettings,
     metaclass=CMBMetaclass,
     root=True,
 ):
-    """A configuration dictionary."""
+    """
+    The base class for configuration models.
+
+    It is not recommended to inherit from this class directly for basic usage.
+    Instead, use either :class:`ConfigModel` or :class:`AsyncConfigModel`.
+    """
 
     @classmethod
     def _resolve_resource(
         cls,
-        resource_argument: ConfigResource | ResourceT | None = None,
+        resource_argument: ConfigResource | RawResourceT | None = None,
         *,
         create_if_missing: bool | None = None,
     ) -> ConfigResource:
         if resource_argument is None:
             resource_argument = getattr(cls.__config__, "resource", None)
         if resource_argument is None:
             raise ValueError("No resource specified")
@@ -766,63 +1305,62 @@
         else:
             resource = resource_argument
         if create_if_missing is not None:
             resource.create_if_missing = create_if_missing
         return resource
 
     @property
-    def was_loaded(self) -> bool:
-        """Whether the configuration has been loaded.
-
-        Returns
-        -------
-        bool
+    def initial_state(self) -> dict[str, Any]:
         """
-        return get_context(self).loaded
+        The initial configuration state.
 
-    @property
-    def original(self) -> dict[str, Any]:
-        """The original configuration dictionary."""
-        return get_context(self).original
+        It is a copy of the configuration state
+        at the last time of loading, reloading or saving.
+        """
+        return get_context(self).initial_state
 
     def at(
         self: ConfigModelBaseT,
         route: str | list[str],
         *,
         parse_dotlist: bool = True,
     ) -> ConfigAt[ConfigModelBaseT]:
-        """Return the configuration section metadata.
+        """
+        Lazily point to a specific item in the configuration.
 
         Parameters
         ----------
         route
-            Route to the key of the item.
+            The access route to the item in this configuration.
 
-        parse_dotlist : bool, optional
-            Whether to parse the route as a dotlist, by default True
+        parse_dotlist
+            Whether to parse the route as a dotlist, by default True.
 
 
         Returns
         -------
-        ConfigAt
-            The item metadata.
+        The configuration accessor.
         """
         if isinstance(route, str):
             if parse_dotlist:
                 [*route] = route.split(".")
             else:
                 route = [route]
         return ConfigAt(self, None, route)
 
     def rollback(self) -> None:
-        """Rollback the configuration to its original state."""
+        """
+        Rollback the configuration to its initial state.
+
+        Returns
+        -------
+        None
+        """
         context = get_context(self)
-        context.loaded = False
-        self.__dict__ = context.original
-        context.loaded = True
+        self.__dict__ = context.initial_state
 
     def _ensure_settings_with_context(
         self,
         name: str,
         value: ConfigModelBaseT
     ) -> ConfigModelBaseT:
         context = get_context(self)
@@ -843,124 +1381,121 @@
 
 
 class ConfigModel(ConfigModelBase, root=True):
 
     @classmethod
     def load(
         cls: type[ConfigModelT],
-        resource: ConfigResource | ResourceT | None = None,
+        resource: ConfigResource | RawResourceT | None = None,
         create_if_missing: bool | None = None,
         **kwargs: Any,
     ) -> ConfigModelT:
-        """Load the configuration file.
-        To reload the configuration, use the ``reload`` method.
+        """
+        Load the configuration file.
+        To reload the configuration, use the `reload()` method.
 
         Parameters
         ----------
-        resource : ConfigResource
+        resource
             The configuration resource to read from/write to.
-        create_if_missing : bool
+        create_if_missing
             Whether to create the configuration file if it does not exist.
         **kwargs
             Keyword arguments to pass to the read method.
 
         Returns
         -------
         self
         """
         cls.update_forward_refs()
         resource = cls._resolve_resource(resource, create_if_missing=create_if_missing)
         context = Context(resource)  # type: Context[ConfigModelT]
         config = resource.read(config_class=cls, **kwargs)
         context.owner = config
-        context.loaded = True
-        context.original = config.dict()
+        context.initial_state = config.dict()
         return config
 
     def reload(self: ConfigModelT, **kwargs: Any) -> ConfigModelT:
-        """Reload the configuration file.
-        If the configuration is not loaded, a ValueError is raised.
+        """
+        Reload the configuration file.
 
         Parameters
         ----------
         **kwargs
             Keyword arguments to pass to the read method.
 
         Returns
         -------
         self
         """
         context = get_context(self)
-        if not context.loaded:
-            msg = "Configuration has not been loaded, use load() instead"
-            raise ValueError(msg)
         if context.owner is self:
-            context.loaded = False
-            kwargs.setdefault("mode", "r")
             new_config = context.resource.read(**kwargs)
             context.bind_to(new_config)
-            context.original = new_config.dict()
+            context.initial_state = new_config.dict()
             new_config.rollback()
-            context.loaded = True
             return new_config
         return reload(context.section)
 
     def save(self, **kwargs: Any) -> int:
-        """Save the configuration to the configuration file.
+        """
+        Save the configuration to the configuration file.
 
         Parameters
         ----------
         **kwargs
             Keyword arguments to pass to the write method.
 
+        Returns
+        -------
+        The number of bytes written.
         """
         context = get_context(self)
         if context.owner is self:
             blob = context.resource.dump_config(self)
             result = self.write(blob, **kwargs)
-            context.original = self.dict()
+            context.initial_state = self.dict()
             return result
         return save(context.section)
 
     def write(self, blob: str | collections.abc.ByteString, **kwargs: Any) -> int:
-        """Overwrite the configuration file with the given blob
-        (config dump as string or bytes).
+        """
+        Overwrite the configuration file with the given string or bytes.
 
         Parameters
         ----------
-        blob : str | bytes
+        blob
             The blob to write to the configuration file.
         **kwargs
             Keyword arguments to pass to the open method.
 
         Returns
         -------
-        int
-            The number of bytes written.
+        The number of bytes written.
         """
         context = get_context(self)
         if context.resource.is_url:
             msg = "Saving to URLs is not yet supported"
             raise NotImplementedError(msg)
-        kwargs.setdefault("mode", "w")
         return context.resource.write(blob, **kwargs)
 
 
 class AsyncConfigModel(ConfigModelBase, root=True):
 
     @classmethod
     async def load_async(
         cls: type[AsyncConfigModelT],
-        resource: ConfigResource | ResourceT | None,
+        resource: ConfigResource | RawResourceT | None,
         *,
         create_if_missing: bool = False,
         **kwargs: Any,
     ) -> AsyncConfigModelT:
-        """Load the configuration file asynchronously.
-        To reload the configuration, use the ``reload`` method.
+        """
+        Load the configuration file asynchronously.
+        To reload the configuration, use the `reload()` method.
 
         Parameters
         ----------
         resource : ConfigResource
             The configuration resource.
         create_if_missing : bool
             Whether to create the configuration file if it does not exist.
@@ -968,89 +1503,95 @@
             Keyword arguments to pass to the read method.
 
         Returns
         -------
         self
         """
         resource = cls._resolve_resource(resource, create_if_missing=create_if_missing)
-        kwargs.setdefault("mode", "r")
         context = Context(resource)  # type: Context[AsyncConfigModelT]
         config = resource.read(config_class=cls, **kwargs)
         context.owner = config
-        context.loaded = True
         return config
 
     async def reload_async(self: AsyncConfigModelT, **kwargs: Any) -> AsyncConfigModelT:
-        """Reload the configuration file.
-        If the configuration is not loaded, a ValueError is raised.
+        """
+        Reload the configuration file asynchronously.
 
         Parameters
         ----------
         **kwargs
             Keyword arguments to pass to the read method.
 
         Returns
         -------
         self
         """
         context = get_context(self)
-        if not context.loaded:
-            msg = "Configuration has not been loaded, use load() instead"
-            raise ValueError(msg)
         if context.owner is self:
-            context.loaded = False
-            kwargs.setdefault("mode", "r")
             new_async_config = await context.resource.read_async(**kwargs)
             context.bind_to(new_async_config)
-            context.original = new_async_config.dict()
+            context.initial_state = new_async_config.dict()
             self.rollback()
-            context.loaded = True
             return new_async_config
         return await reload_async(context.section)
 
     async def save_async(self, **kwargs: Any) -> int:
-        """Save the configuration to the configuration file asynchronously.
+        """
+        Save the configuration to the configuration file asynchronously.
 
         Parameters
         ----------
         **kwargs
             Keyword arguments to pass to the write method.
 
+        Returns
+        -------
+        The number of bytes written.
         """
         context = get_context(self)
         if context.owner is self:
             blob = context.resource.dump_config(self)
             result = await self.write_async(blob, **kwargs)
-            context.original = self.dict()
+            context.initial_state = self.dict()
             return result
         return await save_async(context.section)
 
     async def write_async(
         self,
         blob: str | collections.abc.ByteString,
         **kwargs: Any
     ) -> int:
-        """Overwrite the configuration file asynchronously with the given blob
-        (config dump as string or bytes).
+        """
+        Overwrite the configuration file asynchronously with the given string or bytes.
 
         Parameters
         ----------
-        blob : str | bytes
+        blob
             The blob to write to the configuration file.
         **kwargs
             Keyword arguments to pass to the open method.
 
         Returns
         -------
-        int
-            The number of bytes written.
+        The number of bytes written.
         """
         context = get_context(self)
         if context.resource.is_url:
             msg = "Saving to URLs is not yet supported"
             raise NotImplementedError(msg)
-        kwargs.setdefault("mode", "w")
         return await context.resource.write_async(blob, **kwargs)
 
 
 class Meta(pydantic.BaseSettings.Config):
-    resource: ConfigResource | str | None = None
+    """
+    Meta-configuration for the `ConfigModel` class.
+
+    Attributes
+    ----------
+    resource
+        The configuration resource to read from/write to.
+
+        If a string, it will be interpreted as a path to a file.
+
+    And all other attributes from `pydantic.BaseSettings.Config`.
+    """
+    resource: ConfigResource | RawResourceT | None = None
```

### Comparing `configzen-0.1.2/configzen/errors.py` & `configzen-0.1.3/configzen/errors.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""This module contains all the custom errors raised by _configzen_."""
+
 from __future__ import annotations
 
 import typing
 
 import anyconfig
 
 if typing.TYPE_CHECKING:
@@ -25,8 +27,7 @@
 
     def __init__(self, config: ConfigModelBaseT, route: str | list[str]) -> None:
         if not isinstance(route, str):
             route = ".".join(route)
         super().__init__(
             f"could not get {type(config).__name__}.{route}",
         )
-
```

### Comparing `configzen-0.1.2/LICENSE` & `configzen-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.1.2/pyproject.toml` & `configzen-0.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.1.2"
+version = "0.1.3"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -14,10 +14,16 @@
 pydantic = "^1.10.7"
 anyconfig = "^0.13.0"
 
 [tool.poetry.extras]
 yaml = ["pyyaml"]
 json = ["orjson"]
 
+[tool.poetry.group.dev.dependencies]
+ruff = "^0.0.267"
+mypy = "^1.3.0"
+black = "^23.3.0"
+pre-commit = "^3.3.1"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `configzen-0.1.2/PKG-INFO` & `configzen-0.1.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,17 @@
-Metadata-Version: 2.1
-Name: configzen
-Version: 0.1.2
-Summary: The easiest way to manage configuration files in Python
-License: MIT
-Author: bswck
-Author-email: bswck.dev@gmail.com
-Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: json
-Provides-Extra: yaml
-Requires-Dist: anyconfig (>=0.13.0,<0.14.0)
-Requires-Dist: orjson (>=3.8.12,<4.0.0) ; extra == "json"
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
-Requires-Dist: pyyaml (>=6.0,<7.0) ; extra == "yaml"
-Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) ; python_version >= "3.9" and python_version < "3.11"
-Description-Content-Type: text/markdown
-
 # configzen
 _configzen_ – managing configuration files easily.
 
-## 📖 About
+## What is it?
 _configzen_ combines the power of [pydantic](https://pydantic-docs.helpmanual.io/) 
 and [anyconfig](https://github.com/ssato/python-anyconfig) to provide the most simplistic
 way on Earth of managing configuration files in your Python projects.
 
 Thanks to this, instead of manually using 
-`pyyaml` for YAML configuration files, `configparser` for `ini` files, `json` for JSON files, etc. 
+`pyyaml` for YAML configuration files, `configparser` for INI files, `json` for JSON files, etc. 
 you can create a data model of your configuration and let _configzen_ do the rest and provide you 
 with some extra features on top of that, such as both synchronous and asynchronous, 
 preferably full or partial reloading and saving of your structured configuration.
 
 Let's see how it looks like in practice. Let's say you have a YAML configuration file like this:
 ```yaml
 # database.yaml
@@ -108,14 +86,29 @@
 or save the whole configuration:
 
 ```python
 >>> db_config.save()
 ```
 
 ## Setup
+For using _configzen_ in your project, you need to install it first:
+```bash
+pip install configzen
+```
+
+For development, you can clone the repository and install its dependencies with [poetry](https://python-poetry.org/):
+```bash
+poetry install --with dev
+```
+
 ## License
 [MIT License](https://choosealicense.com/licenses/mit/)
+
 ## Contributing
-## 📧 Contact
-* [bswck](https://github.com/bswck)
-## 🔗 Related Projects 
+Contributions are welcome! Feel free to [open an issue](https://github.com/bswck/configzen/issues/new/choose) 
+or [submit a pull request](https://github.com/bswck/configzen/compare).
 
+## Credits
+* [@Lunarmagpie](https://github.com/Lunarmagpie) for _crucial_ design tips and ideas.
+ 
+## Author
+* [bswck](https://github.com/bswck) (contact: bswck.dev@gmail.com or via [Discord](https://discord.com/) `bswck#8238`)
```

