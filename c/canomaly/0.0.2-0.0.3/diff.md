# Comparing `tmp/canomaly-0.0.2.tar.gz` & `tmp/canomaly-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canomaly-0.0.2.tar", last modified: Sun May 14 01:57:15 2023, max compression
+gzip compressed data, was "canomaly-0.0.3.tar", last modified: Sun May 14 02:12:42 2023, max compression
```

## Comparing `canomaly-0.0.2.tar` & `canomaly-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 01:57:15.673350 canomaly-0.0.2/
--rw-rw-r--   0 galen     (1000) galen     (1000)    35149 2023-05-13 19:23:41.000000 canomaly-0.0.2/LICENSE
--rw-rw-r--   0 galen     (1000) galen     (1000)      631 2023-05-14 01:57:15.673350 canomaly-0.0.2/PKG-INFO
--rw-rw-r--   0 galen     (1000) galen     (1000)      112 2023-05-13 19:23:41.000000 canomaly-0.0.2/README.md
--rw-rw-r--   0 galen     (1000) galen     (1000)      593 2023-05-14 01:56:17.000000 canomaly-0.0.2/pyproject.toml
--rw-rw-r--   0 galen     (1000) galen     (1000)       38 2023-05-14 01:57:15.673350 canomaly-0.0.2/setup.cfg
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 01:57:15.669350 canomaly-0.0.2/src/
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 01:57:15.673350 canomaly-0.0.2/src/canomaly/
--rw-rw-r--   0 galen     (1000) galen     (1000)        0 2023-05-13 19:24:11.000000 canomaly-0.0.2/src/canomaly/__init__.py
--rw-rw-r--   0 galen     (1000) galen     (1000)     2575 2023-05-14 01:36:21.000000 canomaly-0.0.2/src/canomaly/searchtools.py
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 01:57:15.673350 canomaly-0.0.2/src/canomaly.egg-info/
--rw-rw-r--   0 galen     (1000) galen     (1000)      631 2023-05-14 01:57:15.000000 canomaly-0.0.2/src/canomaly.egg-info/PKG-INFO
--rw-rw-r--   0 galen     (1000) galen     (1000)      260 2023-05-14 01:57:15.000000 canomaly-0.0.2/src/canomaly.egg-info/SOURCES.txt
--rw-rw-r--   0 galen     (1000) galen     (1000)        1 2023-05-14 01:57:15.000000 canomaly-0.0.2/src/canomaly.egg-info/dependency_links.txt
--rw-rw-r--   0 galen     (1000) galen     (1000)        9 2023-05-14 01:57:15.000000 canomaly-0.0.2/src/canomaly.egg-info/top_level.txt
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 01:57:15.673350 canomaly-0.0.2/tests/
--rw-rw-r--   0 galen     (1000) galen     (1000)     1204 2023-05-14 01:39:34.000000 canomaly-0.0.2/tests/test_cumulative_regex.py
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 02:12:42.405759 canomaly-0.0.3/
+-rw-rw-r--   0 galen     (1000) galen     (1000)    35149 2023-05-13 19:23:41.000000 canomaly-0.0.3/LICENSE
+-rw-rw-r--   0 galen     (1000) galen     (1000)      631 2023-05-14 02:12:42.405759 canomaly-0.0.3/PKG-INFO
+-rw-rw-r--   0 galen     (1000) galen     (1000)      112 2023-05-13 19:23:41.000000 canomaly-0.0.3/README.md
+-rw-rw-r--   0 galen     (1000) galen     (1000)      593 2023-05-14 02:12:01.000000 canomaly-0.0.3/pyproject.toml
+-rw-rw-r--   0 galen     (1000) galen     (1000)       83 2023-05-14 02:12:42.405759 canomaly-0.0.3/setup.cfg
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 02:12:42.397759 canomaly-0.0.3/src/
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 02:12:42.397759 canomaly-0.0.3/src/canomaly/
+-rw-rw-r--   0 galen     (1000) galen     (1000)        0 2023-05-13 19:24:11.000000 canomaly-0.0.3/src/canomaly/__init__.py
+-rw-rw-r--   0 galen     (1000) galen     (1000)     2575 2023-05-14 01:36:21.000000 canomaly-0.0.3/src/canomaly/searchtools.py
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 02:12:42.401759 canomaly-0.0.3/src/canomaly.egg-info/
+-rw-rw-r--   0 galen     (1000) galen     (1000)      631 2023-05-14 02:12:42.000000 canomaly-0.0.3/src/canomaly.egg-info/PKG-INFO
+-rw-rw-r--   0 galen     (1000) galen     (1000)      305 2023-05-14 02:12:42.000000 canomaly-0.0.3/src/canomaly.egg-info/SOURCES.txt
+-rw-rw-r--   0 galen     (1000) galen     (1000)        1 2023-05-14 02:12:42.000000 canomaly-0.0.3/src/canomaly.egg-info/dependency_links.txt
+-rw-rw-r--   0 galen     (1000) galen     (1000)       12 2023-05-14 02:12:42.000000 canomaly-0.0.3/src/canomaly.egg-info/requires.txt
+-rw-rw-r--   0 galen     (1000) galen     (1000)        9 2023-05-14 02:12:42.000000 canomaly-0.0.3/src/canomaly.egg-info/top_level.txt
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 02:12:42.401759 canomaly-0.0.3/tests/
+-rw-rw-r--   0 galen     (1000) galen     (1000)     1204 2023-05-14 01:39:34.000000 canomaly-0.0.3/tests/test_cumulative_regex.py
```

### Comparing `canomaly-0.0.2/LICENSE` & `canomaly-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `canomaly-0.0.2/PKG-INFO` & `canomaly-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canomaly
-Version: 0.0.2
+Version: 0.0.3
 Summary: Detecting cumulative changes in data.
 Author-email: Galen Seilis <galen.seilis@seilis.ca>
 Project-URL: Homepage, https://github.com/galenseilis/canomaly
 Project-URL: Bug Tracker, https://github.com/galenseilis/canomaly/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `canomaly-0.0.2/pyproject.toml` & `canomaly-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "canomaly"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Galen Seilis", email="galen.seilis@seilis.ca" },
 ]
 description = "Detecting cumulative changes in data."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `canomaly-0.0.2/src/canomaly/searchtools.py` & `canomaly-0.0.3/src/canomaly/searchtools.py`

 * *Files identical despite different names*

### Comparing `canomaly-0.0.2/src/canomaly.egg-info/PKG-INFO` & `canomaly-0.0.3/src/canomaly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canomaly
-Version: 0.0.2
+Version: 0.0.3
 Summary: Detecting cumulative changes in data.
 Author-email: Galen Seilis <galen.seilis@seilis.ca>
 Project-URL: Homepage, https://github.com/galenseilis/canomaly
 Project-URL: Bug Tracker, https://github.com/galenseilis/canomaly/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `canomaly-0.0.2/tests/test_cumulative_regex.py` & `canomaly-0.0.3/tests/test_cumulative_regex.py`

 * *Files identical despite different names*

