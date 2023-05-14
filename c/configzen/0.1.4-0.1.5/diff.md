# Comparing `tmp/configzen-0.1.4.tar.gz` & `tmp/configzen-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.1.4.tar", max compression
+gzip compressed data, was "configzen-0.1.5.tar", max compression
```

## Comparing `configzen-0.1.4.tar` & `configzen-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      156 2023-05-14 04:52:55.424220 configzen-0.1.4/configzen/__init__.py
--rw-r--r--   0        0        0    44782 2023-05-14 04:52:55.442208 configzen-0.1.4/configzen/config.py
--rw-r--r--   0        0        0      925 2023-05-14 03:58:18.183363 configzen-0.1.4/configzen/errors.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.4/configzen/py.typed
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.4/LICENSE
--rw-r--r--   0        0        0      702 2023-05-14 04:53:44.258144 configzen-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3029 2023-05-14 04:41:22.077344 configzen-0.1.4/README.md
--rw-r--r--   0        0        0     3872 1970-01-01 00:00:00.000000 configzen-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      156 2023-05-14 04:52:55.424220 configzen-0.1.5/configzen/__init__.py
+-rw-r--r--   0        0        0    44794 2023-05-14 04:56:23.831879 configzen-0.1.5/configzen/config.py
+-rw-r--r--   0        0        0      925 2023-05-14 03:58:18.183363 configzen-0.1.5/configzen/errors.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.5/configzen/py.typed
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.5/LICENSE
+-rw-r--r--   0        0        0      702 2023-05-14 04:55:46.786393 configzen-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3053 2023-05-14 04:56:23.836878 configzen-0.1.5/README.md
+-rw-r--r--   0        0        0     3896 1970-01-01 00:00:00.000000 configzen-0.1.5/PKG-INFO
```

### Comparing `configzen-0.1.4/configzen/config.py` & `configzen-0.1.5/configzen/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     AIOFILES_AVAILABLE = False
 
 __all__ = (
     "ConfigResource",
     "ConfigModelBase",
     "ConfigModel",
     "AsyncConfigModel",
-    "Meta",
+    "ConfigMeta",
     "save",
     "save_async",
     "reload",
     "reload_async",
     "convert",
     "converter",
     "convert_namedtuple",
@@ -1577,15 +1577,15 @@
         context = get_context(self)
         if context.resource.is_url:
             msg = "Saving to URLs is not yet supported"
             raise NotImplementedError(msg)
         return await context.resource.write_async(blob, **kwargs)
 
 
-class Meta(pydantic.BaseSettings.Config):
+class ConfigMeta(pydantic.BaseSettings.Config):
     """
     Meta-configuration for the `ConfigModel` class.
 
     Attributes
     ----------
     resource
         The configuration resource to read from/write to.
```

### Comparing `configzen-0.1.4/configzen/errors.py` & `configzen-0.1.5/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.4/LICENSE` & `configzen-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.1.4/pyproject.toml` & `configzen-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.1.4"
+version = "0.1.5"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `configzen-0.1.4/README.md` & `configzen-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,24 +21,24 @@
 ```
 You can create a data model for it like this:
 
 ```python
 # config.py
 from ipaddress import IPv4Address, IPv6Address
 from typing import Literal
-from configzen import ConfigModel, Meta, Field
+from configzen import ConfigModel, ConfigMeta, ConfigField
 
 
 class DatabaseConfig(ConfigModel):
     host: IPv4Address | IPv6Address | Literal['localhost']
     port: int
     user: str
-    password: str = Field(exclude=True)
+    password: str = ConfigField(exclude=True)
 
-    class Config(Meta):
+    class Config(ConfigMeta):
         resource = "database.yaml"
         env_prefix = "DB_"
 
 
 db_config = DatabaseConfig.load()
 # Optionally change your config or just persist it, excluding the `password` field.
 db_config.save()
```

### Comparing `configzen-0.1.4/PKG-INFO` & `configzen-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.1.4
+Version: 0.1.5
 Summary: The easiest way to manage configuration files in Python
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -43,24 +43,24 @@
 ```
 You can create a data model for it like this:
 
 ```python
 # config.py
 from ipaddress import IPv4Address, IPv6Address
 from typing import Literal
-from configzen import ConfigModel, Meta, Field
+from configzen import ConfigModel, ConfigMeta, ConfigField
 
 
 class DatabaseConfig(ConfigModel):
     host: IPv4Address | IPv6Address | Literal['localhost']
     port: int
     user: str
-    password: str = Field(exclude=True)
+    password: str = ConfigField(exclude=True)
 
-    class Config(Meta):
+    class Config(ConfigMeta):
         resource = "database.yaml"
         env_prefix = "DB_"
 
 
 db_config = DatabaseConfig.load()
 # Optionally change your config or just persist it, excluding the `password` field.
 db_config.save()
```

