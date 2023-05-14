# Comparing `tmp/configzen-0.1.3.tar.gz` & `tmp/configzen-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.1.3.tar", max compression
+gzip compressed data, was "configzen-0.1.4.tar", max compression
```

## Comparing `configzen-0.1.3.tar` & `configzen-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      135 2023-05-14 02:04:46.442804 configzen-0.1.3/configzen/__init__.py
--rw-r--r--   0        0        0    44763 2023-05-14 04:18:18.892124 configzen-0.1.3/configzen/config.py
--rw-r--r--   0        0        0      925 2023-05-14 03:58:18.183363 configzen-0.1.3/configzen/errors.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.3/configzen/py.typed
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.3/LICENSE
--rw-r--r--   0        0        0      702 2023-05-14 04:31:39.025554 configzen-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3029 2023-05-14 04:41:22.077344 configzen-0.1.3/README.md
--rw-r--r--   0        0        0     3872 1970-01-01 00:00:00.000000 configzen-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      156 2023-05-14 04:52:55.424220 configzen-0.1.4/configzen/__init__.py
+-rw-r--r--   0        0        0    44782 2023-05-14 04:52:55.442208 configzen-0.1.4/configzen/config.py
+-rw-r--r--   0        0        0      925 2023-05-14 03:58:18.183363 configzen-0.1.4/configzen/errors.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.4/configzen/py.typed
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.4/LICENSE
+-rw-r--r--   0        0        0      702 2023-05-14 04:53:44.258144 configzen-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3029 2023-05-14 04:41:22.077344 configzen-0.1.4/README.md
+-rw-r--r--   0        0        0     3872 1970-01-01 00:00:00.000000 configzen-0.1.4/PKG-INFO
```

### Comparing `configzen-0.1.3/configzen/config.py` & `configzen-0.1.4/configzen/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 
 This module provides a way to manage configuration files and resources
 in a consistent way. It also provides a way to load and save configuration
 files in a type-safe way.
 
 .. code-block:: python
 
-    from configzen import ConfigModel, ConfigResource, Meta
+    from configzen import ConfigModel, ConfigResource, ConfigField, Meta
 
     class DatabaseConfig(ConfigModel):
         host: str
         port: int
         user: str
-        password: str = Field(exclude=True)
+        password: str = ConfigField(exclude=True)
 
         class Config(Meta):
             resource = "examples/database.json"
 
     db_config = DatabaseConfig.load()
     db_config.host = "newhost"
     db_config.port = 5432
```

### Comparing `configzen-0.1.3/configzen/errors.py` & `configzen-0.1.4/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.3/LICENSE` & `configzen-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.1.3/pyproject.toml` & `configzen-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.1.3"
+version = "0.1.4"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `configzen-0.1.3/README.md` & `configzen-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.1.3/PKG-INFO` & `configzen-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.1.3
+Version: 0.1.4
 Summary: The easiest way to manage configuration files in Python
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

