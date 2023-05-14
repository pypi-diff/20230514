# Comparing `tmp/worktoy-0.28.4.tar.gz` & `tmp/worktoy-0.28.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "worktoy-0.28.4.tar", last modified: Sun May 14 11:08:44 2023, max compression
+gzip compressed data, was "worktoy-0.28.8.tar", last modified: Sun May 14 11:32:39 2023, max compression
```

## Comparing `worktoy-0.28.4.tar` & `worktoy-0.28.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:08:44.472987 worktoy-0.28.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-14 11:08:35.000000 worktoy-0.28.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-14 11:08:44.472987 worktoy-0.28.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-05-14 11:08:35.000000 worktoy-0.28.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-14 11:08:35.000000 worktoy-0.28.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-14 11:08:44.476987 worktoy-0.28.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:08:44.472987 worktoy-0.28.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:08:44.472987 worktoy-0.28.4/src/worktoy/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-14 11:08:35.000000 worktoy-0.28.4/src/worktoy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-14 11:08:35.000000 worktoy-0.28.4/src/worktoy/_anywayuwantit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-14 11:08:35.000000 worktoy-0.28.4/src/worktoy/_callmemaybe.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-14 11:08:35.000000 worktoy-0.28.4/src/worktoy/_maybe.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-14 11:08:35.000000 worktoy-0.28.4/src/worktoy/_maybeType.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-14 11:08:35.000000 worktoy-0.28.4/src/worktoy/_maybeTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-14 11:08:35.000000 worktoy-0.28.4/src/worktoy/_searchKeys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-14 11:08:35.000000 worktoy-0.28.4/src/worktoy/_stringlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:08:44.472987 worktoy-0.28.4/src/worktoy/mockdata/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-14 11:08:35.000000 worktoy-0.28.4/src/worktoy/mockdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-14 11:08:35.000000 worktoy-0.28.4/src/worktoy/mockdata/_intfactory.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-14 11:08:35.000000 worktoy-0.28.4/src/worktoy/mockdata/_strfactory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:08:44.472987 worktoy-0.28.4/src/worktoy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-14 11:08:44.000000 worktoy-0.28.4/src/worktoy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-14 11:08:44.000000 worktoy-0.28.4/src/worktoy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 11:08:44.000000 worktoy-0.28.4/src/worktoy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-14 11:08:44.000000 worktoy-0.28.4/src/worktoy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:08:44.472987 worktoy-0.28.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-14 11:08:35.000000 worktoy-0.28.4/tests/test__callmemaybe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-14 11:08:35.000000 worktoy-0.28.4/tests/test__intfactory.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-14 11:08:35.000000 worktoy-0.28.4/tests/test__maybe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-14 11:08:35.000000 worktoy-0.28.4/tests/test__maybeType.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-14 11:08:35.000000 worktoy-0.28.4/tests/test__maybeTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-14 11:08:35.000000 worktoy-0.28.4/tests/test__searchKeys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-14 11:08:35.000000 worktoy-0.28.4/tests/test__strfactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-14 11:08:35.000000 worktoy-0.28.4/tests/test__stringlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:32:39.090558 worktoy-0.28.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-14 11:32:30.000000 worktoy-0.28.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-14 11:32:39.090558 worktoy-0.28.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-05-14 11:32:30.000000 worktoy-0.28.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-14 11:32:30.000000 worktoy-0.28.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-14 11:32:39.090558 worktoy-0.28.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:32:39.086558 worktoy-0.28.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:32:39.086558 worktoy-0.28.8/src/worktoy/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-14 11:32:30.000000 worktoy-0.28.8/src/worktoy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-14 11:32:30.000000 worktoy-0.28.8/src/worktoy/_anywayuwantit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-14 11:32:30.000000 worktoy-0.28.8/src/worktoy/_callmemaybe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-14 11:32:30.000000 worktoy-0.28.8/src/worktoy/_maybe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-14 11:32:30.000000 worktoy-0.28.8/src/worktoy/_maybeType.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-14 11:32:30.000000 worktoy-0.28.8/src/worktoy/_maybeTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-14 11:32:30.000000 worktoy-0.28.8/src/worktoy/_searchKeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-14 11:32:30.000000 worktoy-0.28.8/src/worktoy/_stringlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:32:39.090558 worktoy-0.28.8/src/worktoy/mockdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-14 11:32:30.000000 worktoy-0.28.8/src/worktoy/mockdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-14 11:32:30.000000 worktoy-0.28.8/src/worktoy/mockdata/_intfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-14 11:32:30.000000 worktoy-0.28.8/src/worktoy/mockdata/_strfactory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:32:39.090558 worktoy-0.28.8/src/worktoy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-14 11:32:39.000000 worktoy-0.28.8/src/worktoy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-14 11:32:39.000000 worktoy-0.28.8/src/worktoy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 11:32:39.000000 worktoy-0.28.8/src/worktoy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-14 11:32:39.000000 worktoy-0.28.8/src/worktoy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:32:39.090558 worktoy-0.28.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-14 11:32:30.000000 worktoy-0.28.8/tests/test__callmemaybe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-14 11:32:30.000000 worktoy-0.28.8/tests/test__intfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-14 11:32:30.000000 worktoy-0.28.8/tests/test__maybe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-14 11:32:30.000000 worktoy-0.28.8/tests/test__maybeType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-14 11:32:30.000000 worktoy-0.28.8/tests/test__maybeTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-14 11:32:30.000000 worktoy-0.28.8/tests/test__searchKeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-14 11:32:30.000000 worktoy-0.28.8/tests/test__strfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-14 11:32:30.000000 worktoy-0.28.8/tests/test__stringlist.py
```

### Comparing `worktoy-0.28.4/LICENSE` & `worktoy-0.28.8/LICENSE`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.4/PKG-INFO` & `worktoy-0.28.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: worktoy
-Version: 0.28.4
+Version: 0.28.8
 Summary: Collection of Utilities
 Author-email: Asger Jon Vistisen <asgerjon2@gmail.com>
 Project-URL: Homepage, https://github.com/AsgerJon/WorkToy
 Project-URL: Bug Tracker, https://github.com/AsgerJon/WorkToy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `worktoy-0.28.4/README.md` & `worktoy-0.28.8/README.md`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.4/pyproject.toml` & `worktoy-0.28.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ['setuptools>=63.2']
 build-backend = 'setuptools.build_meta'
 
 
 [project]
 name = "worktoy"
-version = "0.28.4"
+version = "0.28.8"
 authors = [
     { name = "Asger Jon Vistisen", email = "asgerjon2@gmail.com" },
 ]
 description = "Collection of Utilities"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `worktoy-0.28.4/setup.cfg` & `worktoy-0.28.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [METADATA]
 name = WorkToy
-version = 0.28.4
+version = 0.28.8
 author = Asger Jon Vistisen
 author_email = asgerjon2@gmail.com
 description = A Collection of Utilities
 long_description = file:README.md,LICENSE
 long_description_content_type = text/markdown
 url = 
 project_urls =
```

### Comparing `worktoy-0.28.4/src/worktoy/_anywayuwantit.py` & `worktoy-0.28.8/src/worktoy/_anywayuwantit.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.4/src/worktoy/_callmemaybe.py` & `worktoy-0.28.8/src/worktoy/_callmemaybe.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.4/src/worktoy/_maybeTypes.py` & `worktoy-0.28.8/src/worktoy/_maybeTypes.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.4/src/worktoy/_searchKeys.py` & `worktoy-0.28.8/src/worktoy/_searchKeys.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.4/src/worktoy/_stringlist.py` & `worktoy-0.28.8/src/worktoy/_stringlist.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.4/src/worktoy/mockdata/_intfactory.py` & `worktoy-0.28.8/src/worktoy/mockdata/_intfactory.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.4/src/worktoy/mockdata/_strfactory.py` & `worktoy-0.28.8/src/worktoy/mockdata/_strfactory.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.4/src/worktoy.egg-info/PKG-INFO` & `worktoy-0.28.8/src/worktoy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: worktoy
-Version: 0.28.4
+Version: 0.28.8
 Summary: Collection of Utilities
 Author-email: Asger Jon Vistisen <asgerjon2@gmail.com>
 Project-URL: Homepage, https://github.com/AsgerJon/WorkToy
 Project-URL: Bug Tracker, https://github.com/AsgerJon/WorkToy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `worktoy-0.28.4/src/worktoy.egg-info/SOURCES.txt` & `worktoy-0.28.8/src/worktoy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.4/tests/test__callmemaybe.py` & `worktoy-0.28.8/tests/test__callmemaybe.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.4/tests/test__intfactory.py` & `worktoy-0.28.8/tests/test__intfactory.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.4/tests/test__maybe.py` & `worktoy-0.28.8/tests/test__maybe.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.4/tests/test__maybeType.py` & `worktoy-0.28.8/tests/test__maybeType.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.4/tests/test__maybeTypes.py` & `worktoy-0.28.8/tests/test__maybeTypes.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.4/tests/test__searchKeys.py` & `worktoy-0.28.8/tests/test__searchKeys.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.4/tests/test__strfactory.py` & `worktoy-0.28.8/tests/test__strfactory.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.28.4/tests/test__stringlist.py` & `worktoy-0.28.8/tests/test__stringlist.py`

 * *Files identical despite different names*

