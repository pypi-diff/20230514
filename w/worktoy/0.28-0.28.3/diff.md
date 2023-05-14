# Comparing `tmp/worktoy-0.28.tar.gz` & `tmp/worktoy-0.28.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "worktoy-0.28.tar", last modified: Sun May 14 09:41:35 2023, max compression
+gzip compressed data, was "worktoy-0.28.3.tar", last modified: Sun May 14 10:58:45 2023, max compression
```

## Comparing `worktoy-0.28.tar` & `worktoy-0.28.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:41:35.142263 worktoy-0.28/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-14 09:41:23.000000 worktoy-0.28/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-05-14 09:41:35.142263 worktoy-0.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-05-14 09:41:23.000000 worktoy-0.28/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-14 09:41:23.000000 worktoy-0.28/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-14 09:41:35.142263 worktoy-0.28/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:41:35.138263 worktoy-0.28/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:41:35.138263 worktoy-0.28/src/worktoy/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-14 09:41:23.000000 worktoy-0.28/src/worktoy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-14 09:41:23.000000 worktoy-0.28/src/worktoy/_anywayuwantit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-14 09:41:23.000000 worktoy-0.28/src/worktoy/_callmemaybe.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-14 09:41:23.000000 worktoy-0.28/src/worktoy/_maybe.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-14 09:41:23.000000 worktoy-0.28/src/worktoy/_maybeType.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-14 09:41:23.000000 worktoy-0.28/src/worktoy/_maybeTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-14 09:41:23.000000 worktoy-0.28/src/worktoy/_searchKeys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-14 09:41:23.000000 worktoy-0.28/src/worktoy/_stringlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:41:35.142263 worktoy-0.28/src/worktoy/mockdata/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-14 09:41:23.000000 worktoy-0.28/src/worktoy/mockdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-14 09:41:23.000000 worktoy-0.28/src/worktoy/mockdata/_intfactory.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-14 09:41:23.000000 worktoy-0.28/src/worktoy/mockdata/_strfactory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:41:35.138263 worktoy-0.28/src/worktoy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-05-14 09:41:35.000000 worktoy-0.28/src/worktoy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-14 09:41:35.000000 worktoy-0.28/src/worktoy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 09:41:35.000000 worktoy-0.28/src/worktoy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-14 09:41:35.000000 worktoy-0.28/src/worktoy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:41:35.142263 worktoy-0.28/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-14 09:41:23.000000 worktoy-0.28/tests/test__callmemaybe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-14 09:41:23.000000 worktoy-0.28/tests/test__intfactory.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-14 09:41:23.000000 worktoy-0.28/tests/test__maybe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-14 09:41:23.000000 worktoy-0.28/tests/test__maybeType.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-14 09:41:23.000000 worktoy-0.28/tests/test__maybeTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-14 09:41:23.000000 worktoy-0.28/tests/test__searchKeys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-14 09:41:23.000000 worktoy-0.28/tests/test__strfactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-14 09:41:23.000000 worktoy-0.28/tests/test__stringlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:58:45.396385 worktoy-0.28.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-14 10:58:36.000000 worktoy-0.28.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-14 10:58:45.396385 worktoy-0.28.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-05-14 10:58:36.000000 worktoy-0.28.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-14 10:58:36.000000 worktoy-0.28.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-14 10:58:45.400385 worktoy-0.28.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:58:45.396385 worktoy-0.28.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:58:45.396385 worktoy-0.28.3/src/worktoy/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-14 10:58:36.000000 worktoy-0.28.3/src/worktoy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-14 10:58:36.000000 worktoy-0.28.3/src/worktoy/_anywayuwantit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-14 10:58:36.000000 worktoy-0.28.3/src/worktoy/_callmemaybe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-14 10:58:36.000000 worktoy-0.28.3/src/worktoy/_maybe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-14 10:58:36.000000 worktoy-0.28.3/src/worktoy/_maybeType.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-14 10:58:36.000000 worktoy-0.28.3/src/worktoy/_maybeTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-14 10:58:36.000000 worktoy-0.28.3/src/worktoy/_searchKeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-14 10:58:36.000000 worktoy-0.28.3/src/worktoy/_stringlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:58:45.396385 worktoy-0.28.3/src/worktoy/mockdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-14 10:58:36.000000 worktoy-0.28.3/src/worktoy/mockdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-14 10:58:36.000000 worktoy-0.28.3/src/worktoy/mockdata/_intfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-14 10:58:36.000000 worktoy-0.28.3/src/worktoy/mockdata/_strfactory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:58:45.396385 worktoy-0.28.3/src/worktoy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-14 10:58:45.000000 worktoy-0.28.3/src/worktoy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-14 10:58:45.000000 worktoy-0.28.3/src/worktoy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 10:58:45.000000 worktoy-0.28.3/src/worktoy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-14 10:58:45.000000 worktoy-0.28.3/src/worktoy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:58:45.396385 worktoy-0.28.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-14 10:58:36.000000 worktoy-0.28.3/tests/test__callmemaybe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-14 10:58:36.000000 worktoy-0.28.3/tests/test__intfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-14 10:58:36.000000 worktoy-0.28.3/tests/test__maybe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-14 10:58:36.000000 worktoy-0.28.3/tests/test__maybeType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-14 10:58:36.000000 worktoy-0.28.3/tests/test__maybeTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-14 10:58:36.000000 worktoy-0.28.3/tests/test__searchKeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-14 10:58:36.000000 worktoy-0.28.3/tests/test__strfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-14 10:58:36.000000 worktoy-0.28.3/tests/test__stringlist.py
```

### Comparing `worktoy-0.28/LICENSE` & `worktoy-0.28.3/LICENSE`

 * *Files identical despite different names*

### Comparing `worktoy-0.28/PKG-INFO` & `worktoy-0.28.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: worktoy
-Version: 0.28
+Version: 0.28.3
 Summary: Collection of Utilities
 Author-email: Asger Jon Vistisen <asgerjon2@gmail.com>
 Project-URL: Homepage, https://github.com/AsgerJon/WorkToy
 Project-URL: Bug Tracker, https://github.com/AsgerJon/WorkToy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # WorkToy
 
 Collection of General Utilities
+```
+pip install worktoy
+```
 
 ## The None-aware 'maybe'
 
 In a programming language which shall rename nameless as well as typeless,
 the following syntax is available:
 
     const func = (arg = null) => {
```

### Comparing `worktoy-0.28/README.md` & `worktoy-0.28.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # WorkToy
 
 Collection of General Utilities
+```
+pip install worktoy
+```
 
 ## The None-aware 'maybe'
 
 In a programming language which shall rename nameless as well as typeless,
 the following syntax is available:
 
     const func = (arg = null) => {
```

### Comparing `worktoy-0.28/pyproject.toml` & `worktoy-0.28.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ['setuptools>=63.2']
 build-backend = 'setuptools.build_meta'
 
 
 [project]
 name = "worktoy"
-version = "0.28"
+version = "0.28.3"
 authors = [
     { name = "Asger Jon Vistisen", email = "asgerjon2@gmail.com" },
 ]
 description = "Collection of Utilities"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `worktoy-0.28/setup.cfg` & `worktoy-0.28.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [METADATA]
 name = WorkToy
-version = 0.28
+version = 0.28.3
 author = Asger Jon Vistisen
 author_email = asgerjon2@gmail.com
 description = A Collection of Utilities
 long_description = file:README.md,LICENSE
 long_description_content_type = text/markdown
 url = 
 project_urls =
```

### Comparing `worktoy-0.28/src/worktoy/_anywayuwantit.py` & `worktoy-0.28.3/src/worktoy/_anywayuwantit.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28/src/worktoy/_callmemaybe.py` & `worktoy-0.28.3/src/worktoy/_callmemaybe.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28/src/worktoy/_maybeTypes.py` & `worktoy-0.28.3/src/worktoy/_maybeTypes.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28/src/worktoy/_searchKeys.py` & `worktoy-0.28.3/src/worktoy/_searchKeys.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28/src/worktoy/_stringlist.py` & `worktoy-0.28.3/src/worktoy/_stringlist.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28/src/worktoy/mockdata/_intfactory.py` & `worktoy-0.28.3/src/worktoy/mockdata/_intfactory.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28/src/worktoy/mockdata/_strfactory.py` & `worktoy-0.28.3/src/worktoy/mockdata/_strfactory.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28/src/worktoy.egg-info/PKG-INFO` & `worktoy-0.28.3/src/worktoy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: worktoy
-Version: 0.28
+Version: 0.28.3
 Summary: Collection of Utilities
 Author-email: Asger Jon Vistisen <asgerjon2@gmail.com>
 Project-URL: Homepage, https://github.com/AsgerJon/WorkToy
 Project-URL: Bug Tracker, https://github.com/AsgerJon/WorkToy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # WorkToy
 
 Collection of General Utilities
+```
+pip install worktoy
+```
 
 ## The None-aware 'maybe'
 
 In a programming language which shall rename nameless as well as typeless,
 the following syntax is available:
 
     const func = (arg = null) => {
```

### Comparing `worktoy-0.28/src/worktoy.egg-info/SOURCES.txt` & `worktoy-0.28.3/src/worktoy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `worktoy-0.28/tests/test__callmemaybe.py` & `worktoy-0.28.3/tests/test__callmemaybe.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28/tests/test__intfactory.py` & `worktoy-0.28.3/tests/test__intfactory.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28/tests/test__maybe.py` & `worktoy-0.28.3/tests/test__maybe.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28/tests/test__maybeType.py` & `worktoy-0.28.3/tests/test__maybeType.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28/tests/test__maybeTypes.py` & `worktoy-0.28.3/tests/test__maybeTypes.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28/tests/test__searchKeys.py` & `worktoy-0.28.3/tests/test__searchKeys.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28/tests/test__strfactory.py` & `worktoy-0.28.3/tests/test__strfactory.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28/tests/test__stringlist.py` & `worktoy-0.28.3/tests/test__stringlist.py`

 * *Files identical despite different names*

