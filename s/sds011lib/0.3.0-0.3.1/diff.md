# Comparing `tmp/sds011lib-0.3.0.tar.gz` & `tmp/sds011lib-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sds011lib-0.3.0.tar", max compression
+gzip compressed data, was "sds011lib-0.3.1.tar", max compression
```

## Comparing `sds011lib-0.3.0.tar` & `sds011lib-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1065 2023-05-13 22:51:24.542011 sds011lib-0.3.0/LICENSE
--rw-r--r--   0        0        0     1163 2023-05-13 22:51:24.542011 sds011lib-0.3.0/README.md
--rw-r--r--   0        0        0      977 2023-05-13 22:51:24.542011 sds011lib-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    26710 2023-05-13 22:51:24.542011 sds011lib-0.3.0/sds011lib/__init__.py
--rw-r--r--   0        0        0     1505 2023-05-13 22:51:24.542011 sds011lib-0.3.0/sds011lib/_constants.py
--rw-r--r--   0        0        0     2332 2023-05-13 22:51:24.542011 sds011lib-0.3.0/sds011lib/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-13 22:51:24.542011 sds011lib-0.3.0/sds011lib/py.typed
--rw-r--r--   0        0        0     1974 2023-05-13 22:51:24.542011 sds011lib-0.3.0/sds011lib/responses.py
--rw-r--r--   0        0        0     1650 1970-01-01 00:00:00.000000 sds011lib-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-13 22:54:59.328288 sds011lib-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1163 2023-05-13 22:54:59.328288 sds011lib-0.3.1/README.md
+-rw-r--r--   0        0        0      977 2023-05-13 22:54:59.328288 sds011lib-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0    26710 2023-05-13 22:54:59.328288 sds011lib-0.3.1/sds011lib/__init__.py
+-rw-r--r--   0        0        0     1505 2023-05-13 22:54:59.328288 sds011lib-0.3.1/sds011lib/_constants.py
+-rw-r--r--   0        0        0     2332 2023-05-13 22:54:59.328288 sds011lib-0.3.1/sds011lib/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-13 22:54:59.328288 sds011lib-0.3.1/sds011lib/py.typed
+-rw-r--r--   0        0        0     1974 2023-05-13 22:54:59.328288 sds011lib-0.3.1/sds011lib/responses.py
+-rw-r--r--   0        0        0     1650 1970-01-01 00:00:00.000000 sds011lib-0.3.1/PKG-INFO
```

### Comparing `sds011lib-0.3.0/LICENSE` & `sds011lib-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sds011lib-0.3.0/README.md` & `sds011lib-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `sds011lib-0.3.0/pyproject.toml` & `sds011lib-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sds011lib"
-version = "0.3.0"
+version = "0.3.1"
 description = "SDS011 Library"
 authors = ["Tim Orme <TimothyOrme@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pyserial = "^3.5"
```

### Comparing `sds011lib-0.3.0/sds011lib/__init__.py` & `sds011lib-0.3.1/sds011lib/__init__.py`

 * *Files identical despite different names*

### Comparing `sds011lib-0.3.0/sds011lib/_constants.py` & `sds011lib-0.3.1/sds011lib/_constants.py`

 * *Files identical despite different names*

### Comparing `sds011lib-0.3.0/sds011lib/exceptions.py` & `sds011lib-0.3.1/sds011lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `sds011lib-0.3.0/sds011lib/responses.py` & `sds011lib-0.3.1/sds011lib/responses.py`

 * *Files identical despite different names*

### Comparing `sds011lib-0.3.0/PKG-INFO` & `sds011lib-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sds011lib
-Version: 0.3.0
+Version: 0.3.1
 Summary: SDS011 Library
 Author: Tim Orme
 Author-email: TimothyOrme@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

