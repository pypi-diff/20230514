# Comparing `tmp/configzen-0.1.6.tar.gz` & `tmp/configzen-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.1.6.tar", max compression
+gzip compressed data, was "configzen-0.1.7.tar", max compression
```

## Comparing `configzen-0.1.6.tar` & `configzen-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      156 2023-05-14 04:52:55.424220 configzen-0.1.6/configzen/__init__.py
--rw-r--r--   0        0        0    44833 2023-05-14 05:18:55.369169 configzen-0.1.6/configzen/config.py
--rw-r--r--   0        0        0      925 2023-05-14 03:58:18.183363 configzen-0.1.6/configzen/errors.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.6/configzen/py.typed
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.6/LICENSE
--rw-r--r--   0        0        0      702 2023-05-14 05:21:37.812116 configzen-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3053 2023-05-14 04:56:23.836878 configzen-0.1.6/README.md
--rw-r--r--   0        0        0     3896 1970-01-01 00:00:00.000000 configzen-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      156 2023-05-14 04:52:55.424220 configzen-0.1.7/configzen/__init__.py
+-rw-r--r--   0        0        0    44917 2023-05-14 05:55:48.783641 configzen-0.1.7/configzen/config.py
+-rw-r--r--   0        0        0      925 2023-05-14 03:58:18.183363 configzen-0.1.7/configzen/errors.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.7/configzen/py.typed
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.7/LICENSE
+-rw-r--r--   0        0        0      702 2023-05-14 05:57:31.350048 configzen-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3053 2023-05-14 04:56:23.836878 configzen-0.1.7/README.md
+-rw-r--r--   0        0        0     3896 1970-01-01 00:00:00.000000 configzen-0.1.7/PKG-INFO
```

### Comparing `configzen-0.1.6/configzen/config.py` & `configzen-0.1.7/configzen/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 import urllib.request
 from collections.abc import Callable, Generator
 from typing import TYPE_CHECKING, Any, Generic, Literal, NamedTuple, TypeVar, cast
 
 import anyconfig
 import pydantic
 from pydantic.main import ModelMetaclass
+from pydantic.json import ENCODERS_BY_TYPE
 
 from configzen.errors import ConfigItemAccessError, UnknownParserError
 
 try:
     import aiofiles
 
     AIOFILES_AVAILABLE = True
@@ -174,15 +175,16 @@
     if dataclasses.is_dataclass(obj):
         return dataclasses.asdict(obj)
     if _is_namedtuple(obj):
         return convert_namedtuple(obj)
     return obj
 
 
-_convert_register = convert.register
+for obj_type, encoder in ENCODERS_BY_TYPE.items():
+    convert.register(obj_type, encoder)
 
 
 def converter(func: Callable[[T], Any], cls: type[T] | None = None) -> type[T] | Any:
     """
     Register a converter function for a type.
 
     Parameters
@@ -206,15 +208,15 @@
         class MyClass:
             ...
 
     """
     if cls is None:
         return functools.partial(converter, func)
 
-    _convert_register(cls, func)
+    convert.register(cls, func)
 
     if not hasattr(cls, "__get_validators__"):
         def validator_gen() -> Generator[Callable[[Any], Any], None, None]:
             yield lambda value: load.dispatch(cls)(cls, value)
 
         cls.__get_validators__ = validator_gen  # type: ignore[attr-defined]
 
@@ -284,15 +286,15 @@
     -------
     The converted mapping.
     """
     return {k: convert(v) for k, v in obj.items()}
 
 
 @functools.singledispatch
-def convert_namedtuple(obj: tuple) -> dict[str, Any]:
+def convert_namedtuple(obj: tuple) -> Any:
     """
     Convert a namedtuple to safely-serializable form.
 
     Parameters
     ----------
     obj
         The namedtuple to convert.
@@ -747,15 +749,15 @@
                 defaults = _get_defaults_from_model_class(config_class)
                 blob = self.dump_data(defaults)
                 await self.write_async(blob, **(create_kwargs or {}))
         return self.load_into(config_class, blob, **self._ac_load_options)
 
     async def write_async(
         self,
-        blob: str | collections.abc.ByteString, 
+        blob: str | collections.abc.ByteString,
         **kwargs: Any,
     ) -> int:
         """
         Write the configuration file asynchronously.
 
         Parameters
         ----------
```

### Comparing `configzen-0.1.6/configzen/errors.py` & `configzen-0.1.7/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.6/LICENSE` & `configzen-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.1.6/pyproject.toml` & `configzen-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.1.6"
+version = "0.1.7"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `configzen-0.1.6/README.md` & `configzen-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.1.6/PKG-INFO` & `configzen-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.1.6
+Version: 0.1.7
 Summary: The easiest way to manage configuration files in Python
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

