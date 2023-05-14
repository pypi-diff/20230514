# Comparing `tmp/jutility-0.0.2.tar.gz` & `tmp/jutility-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Jake\Documents\Programming\jutility\dist\.tmp-x6wipxzi\jutility-0.0.2.tar", last modified: Sat May 13 21:32:23 2023, max compression
+gzip compressed data, was "C:\Users\Jake\Documents\Programming\jutility\dist\.tmp-v_olvpca\jutility-0.0.3.tar", last modified: Sun May 14 16:00:29 2023, max compression
```

## Comparing `jutility-0.0.2.tar` & `jutility-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 21:32:23.000000 jutility-0.0.2/
--rw-rw-rw-   0        0        0     1087 2023-05-13 21:09:33.000000 jutility-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1384 2023-05-13 21:32:23.000000 jutility-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      771 2023-05-13 21:23:26.000000 jutility-0.0.2/README.md
--rw-rw-rw-   0        0        0      673 2023-05-13 21:32:08.000000 jutility-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-13 21:32:23.000000 jutility-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-13 21:32:23.000000 jutility-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-13 21:32:23.000000 jutility-0.0.2/src/jutility/
--rw-rw-rw-   0        0        0        0 2023-05-13 20:59:58.000000 jutility-0.0.2/src/jutility/__init__.py
--rw-rw-rw-   0        0        0    16215 2023-05-13 21:31:01.000000 jutility-0.0.2/src/jutility/plotting.py
--rw-rw-rw-   0        0        0    10048 2023-05-13 21:30:51.000000 jutility-0.0.2/src/jutility/sweep.py
--rw-rw-rw-   0        0        0    13218 2023-05-11 19:23:07.000000 jutility-0.0.2/src/jutility/util.py
-drwxrwxrwx   0        0        0        0 2023-05-13 21:32:23.000000 jutility-0.0.2/src/jutility.egg-info/
--rw-rw-rw-   0        0        0     1384 2023-05-13 21:32:23.000000 jutility-0.0.2/src/jutility.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-13 21:32:23.000000 jutility-0.0.2/src/jutility.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 21:32:23.000000 jutility-0.0.2/src/jutility.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-13 21:32:23.000000 jutility-0.0.2/src/jutility.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 16:00:29.000000 jutility-0.0.3/
+-rw-rw-rw-   0        0        0     1087 2023-05-13 21:09:33.000000 jutility-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2777 2023-05-14 16:00:29.000000 jutility-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2125 2023-05-14 15:59:42.000000 jutility-0.0.3/README.md
+-rw-rw-rw-   0        0        0      766 2023-05-14 15:58:41.000000 jutility-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-14 16:00:29.000000 jutility-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-14 16:00:29.000000 jutility-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-14 16:00:29.000000 jutility-0.0.3/src/jutility/
+-rw-rw-rw-   0        0        0        0 2023-05-13 20:59:58.000000 jutility-0.0.3/src/jutility/__init__.py
+-rw-rw-rw-   0        0        0    16215 2023-05-13 21:31:01.000000 jutility-0.0.3/src/jutility/plotting.py
+-rw-rw-rw-   0        0        0    10048 2023-05-13 21:30:51.000000 jutility-0.0.3/src/jutility/sweep.py
+-rw-rw-rw-   0        0        0    13209 2023-05-14 15:33:41.000000 jutility-0.0.3/src/jutility/util.py
+drwxrwxrwx   0        0        0        0 2023-05-14 16:00:29.000000 jutility-0.0.3/src/jutility.egg-info/
+-rw-rw-rw-   0        0        0     2777 2023-05-14 16:00:29.000000 jutility-0.0.3/src/jutility.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-05-14 16:00:29.000000 jutility-0.0.3/src/jutility.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 16:00:29.000000 jutility-0.0.3/src/jutility.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-14 16:00:29.000000 jutility-0.0.3/src/jutility.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-14 16:00:29.000000 jutility-0.0.3/src/jutility.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 16:00:29.000000 jutility-0.0.3/tests/
+-rw-rw-rw-   0        0        0     9100 2023-05-14 15:22:52.000000 jutility-0.0.3/tests/test_plotting.py
+-rw-rw-rw-   0        0        0     9206 2023-05-13 21:45:28.000000 jutility-0.0.3/tests/test_sweep.py
+-rw-rw-rw-   0        0        0    12140 2023-05-14 15:40:12.000000 jutility-0.0.3/tests/test_util.py
```

### Comparing `jutility-0.0.2/LICENSE` & `jutility-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jutility-0.0.2/src/jutility/plotting.py` & `jutility-0.0.3/src/jutility/plotting.py`

 * *Files identical despite different names*

### Comparing `jutility-0.0.2/src/jutility/sweep.py` & `jutility-0.0.3/src/jutility/sweep.py`

 * *Files identical despite different names*

### Comparing `jutility-0.0.2/src/jutility/util.py` & `jutility-0.0.3/src/jutility/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,22 +26,22 @@
 import pickle
 import json
 import traceback
 import datetime
 import time
 import numpy as np
 
-CURRENT_DIR = os.path.dirname(os.path.abspath(__file__))
+CURRENT_DIR = os.path.abspath(os.getcwd())
 RESULTS_DIR = os.path.join(CURRENT_DIR, "Results")
 
 class Result:
-    def __init__(self, data, filename, dir_name=None):
-        self._data = data
+    def __init__(self, filename, dir_name=None, data=None):
         self._filename = filename
         self._dir_name = dir_name
+        self._data = data
 
     def get_data(self):
         return self._data
 
     def get_context(self, save=True, suppress_exceptions=False):
         return ResultSavingContext(self, save, suppress_exceptions)
```

