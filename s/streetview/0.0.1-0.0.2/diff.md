# Comparing `tmp/streetview-0.0.1.tar.gz` & `tmp/streetview-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streetview-0.0.1.tar", last modified: Sun May 14 20:32:55 2023, max compression
+gzip compressed data, was "streetview-0.0.2.tar", last modified: Sun May 14 20:35:26 2023, max compression
```

## Comparing `streetview-0.0.1.tar` & `streetview-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:32:55.494290 streetview-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-14 20:32:38.000000 streetview-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-14 20:32:55.494290 streetview-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-14 20:32:38.000000 streetview-0.0.1/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 20:32:55.494290 streetview-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-14 20:32:38.000000 streetview-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:32:55.490290 streetview-0.0.1/streetview/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-14 20:32:38.000000 streetview-0.0.1/streetview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-14 20:32:38.000000 streetview-0.0.1/streetview/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-14 20:32:38.000000 streetview-0.0.1/streetview/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-14 20:32:38.000000 streetview-0.0.1/streetview/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:32:55.494290 streetview-0.0.1/streetview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-14 20:32:55.000000 streetview-0.0.1/streetview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-14 20:32:55.000000 streetview-0.0.1/streetview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 20:32:55.000000 streetview-0.0.1/streetview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 20:32:55.000000 streetview-0.0.1/streetview.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-14 20:32:55.000000 streetview-0.0.1/streetview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-14 20:32:55.000000 streetview-0.0.1/streetview.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:32:55.494290 streetview-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-14 20:32:38.000000 streetview-0.0.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-14 20:32:38.000000 streetview-0.0.1/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-14 20:32:38.000000 streetview-0.0.1/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 20:32:39.000000 streetview-0.0.1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:35:26.965448 streetview-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-14 20:35:08.000000 streetview-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-14 20:35:26.961448 streetview-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-14 20:35:08.000000 streetview-0.0.2/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 20:35:26.965448 streetview-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-14 20:35:08.000000 streetview-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:35:26.961448 streetview-0.0.2/streetview/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-14 20:35:08.000000 streetview-0.0.2/streetview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-14 20:35:08.000000 streetview-0.0.2/streetview/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-14 20:35:08.000000 streetview-0.0.2/streetview/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-14 20:35:08.000000 streetview-0.0.2/streetview/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:35:26.961448 streetview-0.0.2/streetview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-14 20:35:26.000000 streetview-0.0.2/streetview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-14 20:35:26.000000 streetview-0.0.2/streetview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 20:35:26.000000 streetview-0.0.2/streetview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 20:35:26.000000 streetview-0.0.2/streetview.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-14 20:35:26.000000 streetview-0.0.2/streetview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-14 20:35:26.000000 streetview-0.0.2/streetview.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:35:26.961448 streetview-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-14 20:35:08.000000 streetview-0.0.2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-14 20:35:08.000000 streetview-0.0.2/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-14 20:35:08.000000 streetview-0.0.2/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 20:35:09.000000 streetview-0.0.2/version.py
```

### Comparing `streetview-0.0.1/PKG-INFO` & `streetview-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streetview
-Version: 0.0.1
+Version: 0.0.2
 Summary: Retrieve current and historical photos from Google Street View
 Home-page: https://github.com/robolyst/streetview
 Author: Adrian Letchford
 Author-email: me@dradrian.com
 License: MIT
 Description-Content-Type: text/markdown
 
@@ -21,15 +21,15 @@
 public use. Therefore, this hack may break if Google makes changes to how
 Street View works.*
 
 # Install
 
 Install from pip with:
 
-	pip install git+https://github.com/robolyst/streetview
+	pip install streetview
 
 # Quick start
 
 ## Search for Panoramas
 
 The photos on Google street view are panoramas. Each parnorama has its own
 unique ID. Retrieving photos is a two step process. First, you must translate GPS
```

### Comparing `streetview-0.0.1/readme.md` & `streetview-0.0.2/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 public use. Therefore, this hack may break if Google makes changes to how
 Street View works.*
 
 # Install
 
 Install from pip with:
 
-	pip install git+https://github.com/robolyst/streetview
+	pip install streetview
 
 # Quick start
 
 ## Search for Panoramas
 
 The photos on Google street view are panoramas. Each parnorama has its own
 unique ID. Retrieving photos is a two step process. First, you must translate GPS
```

### Comparing `streetview-0.0.1/setup.py` & `streetview-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `streetview-0.0.1/streetview/api.py` & `streetview-0.0.2/streetview/api.py`

 * *Files identical despite different names*

### Comparing `streetview-0.0.1/streetview/download.py` & `streetview-0.0.2/streetview/download.py`

 * *Files identical despite different names*

### Comparing `streetview-0.0.1/streetview/search.py` & `streetview-0.0.2/streetview/search.py`

 * *Files identical despite different names*

### Comparing `streetview-0.0.1/streetview.egg-info/PKG-INFO` & `streetview-0.0.2/streetview.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streetview
-Version: 0.0.1
+Version: 0.0.2
 Summary: Retrieve current and historical photos from Google Street View
 Home-page: https://github.com/robolyst/streetview
 Author: Adrian Letchford
 Author-email: me@dradrian.com
 License: MIT
 Description-Content-Type: text/markdown
 
@@ -21,15 +21,15 @@
 public use. Therefore, this hack may break if Google makes changes to how
 Street View works.*
 
 # Install
 
 Install from pip with:
 
-	pip install git+https://github.com/robolyst/streetview
+	pip install streetview
 
 # Quick start
 
 ## Search for Panoramas
 
 The photos on Google street view are panoramas. Each parnorama has its own
 unique ID. Retrieving photos is a two step process. First, you must translate GPS
```

### Comparing `streetview-0.0.1/tests/test_api.py` & `streetview-0.0.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `streetview-0.0.1/tests/test_download.py` & `streetview-0.0.2/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `streetview-0.0.1/tests/test_search.py` & `streetview-0.0.2/tests/test_search.py`

 * *Files identical despite different names*

