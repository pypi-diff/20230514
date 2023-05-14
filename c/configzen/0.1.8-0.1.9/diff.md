# Comparing `tmp/configzen-0.1.8.tar.gz` & `tmp/configzen-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.1.8.tar", max compression
+gzip compressed data, was "configzen-0.1.9.tar", max compression
```

## Comparing `configzen-0.1.8.tar` & `configzen-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      156 2023-05-14 04:52:55.424220 configzen-0.1.8/configzen/__init__.py
--rw-r--r--   0        0        0    44927 2023-05-14 06:06:46.923010 configzen-0.1.8/configzen/config.py
--rw-r--r--   0        0        0      925 2023-05-14 03:58:18.183363 configzen-0.1.8/configzen/errors.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.8/configzen/py.typed
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.8/LICENSE
--rw-r--r--   0        0        0      702 2023-05-14 06:07:48.493034 configzen-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3053 2023-05-14 04:56:23.836878 configzen-0.1.8/README.md
--rw-r--r--   0        0        0     3896 1970-01-01 00:00:00.000000 configzen-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      156 2023-05-14 04:52:55.424220 configzen-0.1.9/configzen/__init__.py
+-rw-r--r--   0        0        0    44980 2023-05-14 10:20:30.029004 configzen-0.1.9/configzen/config.py
+-rw-r--r--   0        0        0      925 2023-05-14 03:58:18.183363 configzen-0.1.9/configzen/errors.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.9/configzen/py.typed
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.9/LICENSE
+-rw-r--r--   0        0        0      702 2023-05-14 10:22:48.543109 configzen-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3053 2023-05-14 04:56:23.836878 configzen-0.1.9/README.md
+-rw-r--r--   0        0        0     3896 1970-01-01 00:00:00.000000 configzen-0.1.9/PKG-INFO
```

### Comparing `configzen-0.1.8/configzen/config.py` & `configzen-0.1.9/configzen/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
 The core module of the _configzen_ library.
 
-This module provides a way to manage configuration files and resources
-in a consistent way. It also provides a way to load and save configuration
-files in a type-safe way.
+This module provides an API to manage configuration files and resources
+in a consistent way. It also provides tools to load and save configuration
+files in various formats and within a number of advanced methods.
 
 .. code-block:: python
 
-    from configzen import ConfigModel, ConfigResource, ConfigField, Meta
+    from configzen import ConfigModel, ConfigResource, ConfigField, ConfigMeta
 
     class DatabaseConfig(ConfigModel):
         host: str
         port: int
         user: str
         password: str = ConfigField(exclude=True)
 
-        class Config(Meta):
+        class Config(ConfigMeta):
             resource = "examples/database.json"
 
     db_config = DatabaseConfig.load()
     db_config.host = "newhost"
     db_config.port = 5432
 
     db_config.save()
@@ -818,15 +818,15 @@
             """
             Get the value of the item.
 
             Returns
             -------
             The value of the item.
             """
-            scope = _vars(self.mapping or self.owner.dict())
+            scope = _vars(self.mapping or self.owner)
             route_here = []
             try:
                 for part in self.route:
                     route_here.append(part)
                     scope = _vars(scope)[part]
             except KeyError:
                 raise ConfigItemAccessError(self.owner, route_here) from None
@@ -842,15 +842,15 @@
                 The new value.
 
             Returns
             -------
             The updated mapping.
             """
             route = list(self.route)
-            mapping = self.mapping or self.owner.dict()
+            mapping = self.mapping or self.owner
             key = route.pop()
             submapping = _vars(mapping)
             route_here = []
             try:
                 for part in route:
                     route_here.append(part)
                     submapping = _vars(submapping[part])
@@ -997,17 +997,17 @@
     """
     if isinstance(section, ConfigModel):
         config = section
         return config.reload()
 
     config = section.owner
     context = get_context(config)
-    data = config.dict()
+    data = config.__dict__
     newest = context.resource.read(config_class=type(config), **kwargs)
-    section_data = ConfigAt(newest, newest.dict(), section.route).get()
+    section_data = ConfigAt(newest, newest.__dict__, section.route).get()
     new_mapping = ConfigAt(config, data, section.route).update(section_data)
     config.__dict__.update(new_mapping)
     return section_data
 
 
 async def reload_async(section: AsyncConfigModelT | ConfigAt, **kwargs: Any) -> Any:
     """
@@ -1026,17 +1026,17 @@
     """
     if isinstance(section, AsyncConfigModel):
         config = section
         return await config.reload_async()
 
     config = section.owner
     context = get_context(config)
-    data = config.dict()
+    data = config.__dict__
     newest = await context.resource.read_async(config_class=type(config), **kwargs)
-    section_data = ConfigAt(newest, newest.dict(), section.route).get()
+    section_data = ConfigAt(newest, newest.__dict__, section.route).get()
     new_mapping = ConfigAt(config, data, section.route).update(section_data)
     config.__dict__.update(new_mapping)
     return new_mapping
 
 
 class AnyContext(abc.ABC, Generic[ConfigModelBaseT]):
     """
@@ -1355,15 +1355,15 @@
         Rollback the configuration to its initial state.
 
         Returns
         -------
         None
         """
         context = get_context(self)
-        self.__dict__ = context.initial_state
+        self.__dict__.update(context.initial_state)
 
     def _ensure_settings_with_context(
         self,
         name: str,
         value: ConfigModelBaseT
     ) -> ConfigModelBaseT:
         context = get_context(self)
```

### Comparing `configzen-0.1.8/configzen/errors.py` & `configzen-0.1.9/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.8/LICENSE` & `configzen-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.1.8/pyproject.toml` & `configzen-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.1.8"
+version = "0.1.9"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `configzen-0.1.8/README.md` & `configzen-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.1.8/PKG-INFO` & `configzen-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.1.8
+Version: 0.1.9
 Summary: The easiest way to manage configuration files in Python
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

