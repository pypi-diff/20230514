# Comparing `tmp/configzen-0.1.5.tar.gz` & `tmp/configzen-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.1.5.tar", max compression
+gzip compressed data, was "configzen-0.1.6.tar", max compression
```

## Comparing `configzen-0.1.5.tar` & `configzen-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      156 2023-05-14 04:52:55.424220 configzen-0.1.5/configzen/__init__.py
--rw-r--r--   0        0        0    44794 2023-05-14 04:56:23.831879 configzen-0.1.5/configzen/config.py
--rw-r--r--   0        0        0      925 2023-05-14 03:58:18.183363 configzen-0.1.5/configzen/errors.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.5/configzen/py.typed
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.5/LICENSE
--rw-r--r--   0        0        0      702 2023-05-14 04:55:46.786393 configzen-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3053 2023-05-14 04:56:23.836878 configzen-0.1.5/README.md
--rw-r--r--   0        0        0     3896 1970-01-01 00:00:00.000000 configzen-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      156 2023-05-14 04:52:55.424220 configzen-0.1.6/configzen/__init__.py
+-rw-r--r--   0        0        0    44833 2023-05-14 05:18:55.369169 configzen-0.1.6/configzen/config.py
+-rw-r--r--   0        0        0      925 2023-05-14 03:58:18.183363 configzen-0.1.6/configzen/errors.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.6/configzen/py.typed
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.6/LICENSE
+-rw-r--r--   0        0        0      702 2023-05-14 05:21:37.812116 configzen-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3053 2023-05-14 04:56:23.836878 configzen-0.1.6/README.md
+-rw-r--r--   0        0        0     3896 1970-01-01 00:00:00.000000 configzen-0.1.6/PKG-INFO
```

### Comparing `configzen-0.1.5/configzen/config.py` & `configzen-0.1.6/configzen/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
     AIOFILES_AVAILABLE = False
 
 __all__ = (
     "ConfigResource",
     "ConfigModelBase",
     "ConfigModel",
     "AsyncConfigModel",
+    "DualIOConfigModel",
     "ConfigMeta",
     "save",
     "save_async",
     "reload",
     "reload_async",
     "convert",
     "converter",
@@ -368,40 +369,40 @@
         The URL schemes that are allowed to be used.
 
     Raises
     ------
     ValueError
     """
 
-    _resource: OpenedT | str | os.PathLike | pathlib.Path
-    create_if_missing: bool
     ac_parser: str | None
+    create_if_missing: bool
+    allowed_url_schemes: set[str] = _URL_SCHEMES
+    _resource: OpenedT | str | os.PathLike | pathlib.Path
     _ac_load_options: dict[str, Any]
     _ac_dump_options: dict[str, Any]
-    allowed_url_schemes: set[str] = _URL_SCHEMES
 
     def __init__(
         self: ConfigResource,
         resource: RawResourceT,
         ac_parser: str | None = None,
         *,
         create_if_missing: bool = False,
         use_pydantic_json: bool = True,
         **options: Any,
     ) -> None:
         """Parameters
         ----------
-        resource : str or file-like object, optional
+        resource
             The URL to the configuration file, or a file-like object.
-        ac_parser : str, optional
+        ac_parser
             The name of the engines to use for loading and saving the configuration.
             Defaults to 'yaml'.
-        create_if_missing : bool, optional
+        create_if_missing
             Whether to automatically create missing keys when loading the configuration.
-        use_pydantic_json : bool, optional
+        use_pydantic_json
             Whether to use Pydantic's JSON encoder/decoder instead of the default
             anyconfig one.
         **options
             Additional keyword arguments to pass to
             `anyconfig.loads()` and `anyconfig.dumps()`.
         """
         if (
@@ -687,35 +688,34 @@
             with self.open_resource(**kwargs) as fp:
                 blob = fp.read()
         except FileNotFoundError:
             blob = None
             if self.create_if_missing:
                 defaults = _get_defaults_from_model_class(config_class)
                 blob = self.dump_data(defaults)
-                create_kwargs = self._get_default_kwargs("write", kwargs=create_kwargs)
-                self.write(blob, **create_kwargs)
+                self.write(blob, **(create_kwargs or {}))
         return self.load_into(config_class, blob, **self._ac_load_options)
 
-    def write(self, blob: str | collections.abc.ByteString, **kwds: Any) -> int:
+    def write(self, blob: str | collections.abc.ByteString, **kwargs: Any) -> int:
         """
         Write the configuration file.
 
         Parameters
         ----------
         blob
             The string/bytes to write into the resource.
-        kwds
+        kwargs
             Keyword arguments to pass to the opening routine.
 
         Returns
         -------
         The number of bytes written.
         """
-        kwds = self._get_default_kwargs("write", kwds)
-        with self.open_resource(**kwds) as fp:
+        kwargs = self._get_default_kwargs("write", kwargs=kwargs)
+        with self.open_resource(**kwargs) as fp:
             return fp.write(blob)
 
     async def read_async(
         self,
         *,
         config_class: type[AsyncConfigModelT],
         create_kwargs: dict[str, Any] | None = None,
@@ -742,37 +742,38 @@
         try:
             async with self.open_resource_async(**kwargs) as fp:
                 blob = await fp.read()
         except FileNotFoundError:
             if self.create_if_missing:
                 defaults = _get_defaults_from_model_class(config_class)
                 blob = self.dump_data(defaults)
-                create_kwargs = self._get_default_kwargs("write", kwargs=create_kwargs)
-                await self.write_async(blob, **create_kwargs)
+                await self.write_async(blob, **(create_kwargs or {}))
         return self.load_into(config_class, blob, **self._ac_load_options)
 
     async def write_async(
         self,
-        blob: str | collections.abc.ByteString, **kwds: Any,
+        blob: str | collections.abc.ByteString, 
+        **kwargs: Any,
     ) -> int:
         """
         Write the configuration file asynchronously.
 
         Parameters
         ----------
         blob
             The string/bytes to write into the resource.
-        kwds
+        kwargs
             Keyword arguments to pass to the opening routine.
 
         Returns
         -------
         The number of bytes written.
         """
-        async with self.open_resource_async(**kwds) as fp:
+        kwargs = self._get_default_kwargs("write", kwargs=kwargs)
+        async with self.open_resource_async(**kwargs) as fp:
             return await fp.write(blob)
 
 
 if TYPE_CHECKING:
 
     class ConfigAt(NamedTuple, Generic[ConfigModelBaseT]):
         owner: ConfigModelBaseT
@@ -1051,15 +1052,15 @@
 
     """
     initial_state: dict[str, Any]
     _initial_state: dict[str, Any]
 
     @abc.abstractmethod
     def trace_route(self) -> collections.abc.Generator[str, None, None]:
-        """Trace the route to the configuration context."""
+        """Trace the route to where the configuration subcontext points to."""
 
     @staticmethod
     def get(config: ConfigModelBaseT) -> AnyContext[ConfigModelBaseT]:
         """
         Get the context of the configuration model.
 
         Parameters
@@ -1491,17 +1492,17 @@
     ) -> AsyncConfigModelT:
         """
         Load the configuration file asynchronously.
         To reload the configuration, use the `reload()` method.
 
         Parameters
         ----------
-        resource : ConfigResource
+        resource
             The configuration resource.
-        create_if_missing : bool
+        create_if_missing
             Whether to create the configuration file if it does not exist.
         **kwargs
             Keyword arguments to pass to the read method.
 
         Returns
         -------
         self
@@ -1577,14 +1578,20 @@
         context = get_context(self)
         if context.resource.is_url:
             msg = "Saving to URLs is not yet supported"
             raise NotImplementedError(msg)
         return await context.resource.write_async(blob, **kwargs)
 
 
+class DualIOConfigModel(ConfigModel, AsyncConfigModel, root=True):
+    """
+    A configuration model that can be used both synchronously and asynchronously.
+    """
+
+
 class ConfigMeta(pydantic.BaseSettings.Config):
     """
     Meta-configuration for the `ConfigModel` class.
 
     Attributes
     ----------
     resource
```

### Comparing `configzen-0.1.5/configzen/errors.py` & `configzen-0.1.6/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.5/LICENSE` & `configzen-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.1.5/pyproject.toml` & `configzen-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.1.5"
+version = "0.1.6"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `configzen-0.1.5/README.md` & `configzen-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.1.5/PKG-INFO` & `configzen-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.1.5
+Version: 0.1.6
 Summary: The easiest way to manage configuration files in Python
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

