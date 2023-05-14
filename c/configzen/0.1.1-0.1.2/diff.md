# Comparing `tmp/configzen-0.1.1.tar.gz` & `tmp/configzen-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.1.1.tar", max compression
+gzip compressed data, was "configzen-0.1.2.tar", max compression
```

## Comparing `configzen-0.1.1.tar` & `configzen-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      135 2023-05-14 02:04:46.442804 configzen-0.1.1/configzen/__init__.py
--rw-r--r--   0        0        0    32122 2023-05-14 02:36:01.959219 configzen-0.1.1/configzen/config.py
--rw-r--r--   0        0        0      853 2023-05-14 02:32:13.602772 configzen-0.1.1/configzen/errors.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.1/LICENSE
--rw-r--r--   0        0        0      590 2023-05-14 02:38:37.575944 configzen-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2407 2023-05-14 02:01:48.926739 configzen-0.1.1/README.md
--rw-r--r--   0        0        0     3250 1970-01-01 00:00:00.000000 configzen-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      135 2023-05-14 02:04:46.442804 configzen-0.1.2/configzen/__init__.py
+-rw-r--r--   0        0        0    32122 2023-05-14 02:36:01.959219 configzen-0.1.2/configzen/config.py
+-rw-r--r--   0        0        0      853 2023-05-14 02:32:13.602772 configzen-0.1.2/configzen/errors.py
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.2/LICENSE
+-rw-r--r--   0        0        0      590 2023-05-14 02:44:13.804655 configzen-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2434 2023-05-14 02:41:15.994125 configzen-0.1.2/README.md
+-rw-r--r--   0        0        0     3277 1970-01-01 00:00:00.000000 configzen-0.1.2/PKG-INFO
```

### Comparing `configzen-0.1.1/configzen/config.py` & `configzen-0.1.2/configzen/config.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.1/configzen/errors.py` & `configzen-0.1.2/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.1/LICENSE` & `configzen-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.1.1/pyproject.toml` & `configzen-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.1.1"
+version = "0.1.2"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `configzen-0.1.1/README.md` & `configzen-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,22 +25,22 @@
 # config.py
 from ipaddress import IPv4Address, IPv6Address
 from typing import Literal
 from configzen import ConfigModel, Meta, Field
 
 
 class DatabaseConfig(ConfigModel):
-	host: IPv4Address | IPv6Address | Literal['localhost']
-	port: int
-	user: str
-	password: str = Field(exclude=True)
-
-	class Config(Meta):
-		resource = "database.yaml"
-		env_prefix = "DB_"
+    host: IPv4Address | IPv6Address | Literal['localhost']
+    port: int
+    user: str
+    password: str = Field(exclude=True)
+
+    class Config(Meta):
+        resource = "database.yaml"
+        env_prefix = "DB_"
 
 
 db_config = DatabaseConfig.load()
 # Optionally change your config or just persist it, excluding the `password` field.
 db_config.save()
 ```
```

### Comparing `configzen-0.1.1/PKG-INFO` & `configzen-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.1.1
+Version: 0.1.2
 Summary: The easiest way to manage configuration files in Python
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -47,22 +47,22 @@
 # config.py
 from ipaddress import IPv4Address, IPv6Address
 from typing import Literal
 from configzen import ConfigModel, Meta, Field
 
 
 class DatabaseConfig(ConfigModel):
-	host: IPv4Address | IPv6Address | Literal['localhost']
-	port: int
-	user: str
-	password: str = Field(exclude=True)
-
-	class Config(Meta):
-		resource = "database.yaml"
-		env_prefix = "DB_"
+    host: IPv4Address | IPv6Address | Literal['localhost']
+    port: int
+    user: str
+    password: str = Field(exclude=True)
+
+    class Config(Meta):
+        resource = "database.yaml"
+        env_prefix = "DB_"
 
 
 db_config = DatabaseConfig.load()
 # Optionally change your config or just persist it, excluding the `password` field.
 db_config.save()
 ```
```

