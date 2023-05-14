# Comparing `tmp/canomaly-0.0.1.tar.gz` & `tmp/canomaly-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canomaly-0.0.1.tar", last modified: Sat May 13 19:29:54 2023, max compression
+gzip compressed data, was "canomaly-0.0.2.tar", last modified: Sun May 14 01:57:15 2023, max compression
```

## Comparing `canomaly-0.0.1.tar` & `canomaly-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-13 19:29:54.755299 canomaly-0.0.1/
--rw-rw-r--   0 galen     (1000) galen     (1000)    35149 2023-05-13 19:23:41.000000 canomaly-0.0.1/LICENSE
--rw-rw-r--   0 galen     (1000) galen     (1000)      631 2023-05-13 19:29:54.755299 canomaly-0.0.1/PKG-INFO
--rw-rw-r--   0 galen     (1000) galen     (1000)      112 2023-05-13 19:23:41.000000 canomaly-0.0.1/README.md
--rw-rw-r--   0 galen     (1000) galen     (1000)      593 2023-05-13 19:29:45.000000 canomaly-0.0.1/pyproject.toml
--rw-rw-r--   0 galen     (1000) galen     (1000)       38 2023-05-13 19:29:54.755299 canomaly-0.0.1/setup.cfg
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-13 19:29:54.751299 canomaly-0.0.1/src/
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-13 19:29:54.755299 canomaly-0.0.1/src/canomaly/
--rw-rw-r--   0 galen     (1000) galen     (1000)        0 2023-05-13 19:24:11.000000 canomaly-0.0.1/src/canomaly/__init__.py
--rw-rw-r--   0 galen     (1000) galen     (1000)        0 2023-05-13 19:27:36.000000 canomaly-0.0.1/src/canomaly/search.py
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-13 19:29:54.755299 canomaly-0.0.1/src/canomaly.egg-info/
--rw-rw-r--   0 galen     (1000) galen     (1000)      631 2023-05-13 19:29:54.000000 canomaly-0.0.1/src/canomaly.egg-info/PKG-INFO
--rw-rw-r--   0 galen     (1000) galen     (1000)      224 2023-05-13 19:29:54.000000 canomaly-0.0.1/src/canomaly.egg-info/SOURCES.txt
--rw-rw-r--   0 galen     (1000) galen     (1000)        1 2023-05-13 19:29:54.000000 canomaly-0.0.1/src/canomaly.egg-info/dependency_links.txt
--rw-rw-r--   0 galen     (1000) galen     (1000)        9 2023-05-13 19:29:54.000000 canomaly-0.0.1/src/canomaly.egg-info/top_level.txt
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 01:57:15.673350 canomaly-0.0.2/
+-rw-rw-r--   0 galen     (1000) galen     (1000)    35149 2023-05-13 19:23:41.000000 canomaly-0.0.2/LICENSE
+-rw-rw-r--   0 galen     (1000) galen     (1000)      631 2023-05-14 01:57:15.673350 canomaly-0.0.2/PKG-INFO
+-rw-rw-r--   0 galen     (1000) galen     (1000)      112 2023-05-13 19:23:41.000000 canomaly-0.0.2/README.md
+-rw-rw-r--   0 galen     (1000) galen     (1000)      593 2023-05-14 01:56:17.000000 canomaly-0.0.2/pyproject.toml
+-rw-rw-r--   0 galen     (1000) galen     (1000)       38 2023-05-14 01:57:15.673350 canomaly-0.0.2/setup.cfg
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 01:57:15.669350 canomaly-0.0.2/src/
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 01:57:15.673350 canomaly-0.0.2/src/canomaly/
+-rw-rw-r--   0 galen     (1000) galen     (1000)        0 2023-05-13 19:24:11.000000 canomaly-0.0.2/src/canomaly/__init__.py
+-rw-rw-r--   0 galen     (1000) galen     (1000)     2575 2023-05-14 01:36:21.000000 canomaly-0.0.2/src/canomaly/searchtools.py
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 01:57:15.673350 canomaly-0.0.2/src/canomaly.egg-info/
+-rw-rw-r--   0 galen     (1000) galen     (1000)      631 2023-05-14 01:57:15.000000 canomaly-0.0.2/src/canomaly.egg-info/PKG-INFO
+-rw-rw-r--   0 galen     (1000) galen     (1000)      260 2023-05-14 01:57:15.000000 canomaly-0.0.2/src/canomaly.egg-info/SOURCES.txt
+-rw-rw-r--   0 galen     (1000) galen     (1000)        1 2023-05-14 01:57:15.000000 canomaly-0.0.2/src/canomaly.egg-info/dependency_links.txt
+-rw-rw-r--   0 galen     (1000) galen     (1000)        9 2023-05-14 01:57:15.000000 canomaly-0.0.2/src/canomaly.egg-info/top_level.txt
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 01:57:15.673350 canomaly-0.0.2/tests/
+-rw-rw-r--   0 galen     (1000) galen     (1000)     1204 2023-05-14 01:39:34.000000 canomaly-0.0.2/tests/test_cumulative_regex.py
```

### Comparing `canomaly-0.0.1/LICENSE` & `canomaly-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `canomaly-0.0.1/PKG-INFO` & `canomaly-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canomaly
-Version: 0.0.1
+Version: 0.0.2
 Summary: Detecting cumulative changes in data.
 Author-email: Galen Seilis <galen.seilis@seilis.ca>
 Project-URL: Homepage, https://github.com/galenseilis/canomaly
 Project-URL: Bug Tracker, https://github.com/galenseilis/canomaly/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `canomaly-0.0.1/pyproject.toml` & `canomaly-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "canomaly"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Galen Seilis", email="galen.seilis@seilis.ca" },
 ]
 description = "Detecting cumulative changes in data."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `canomaly-0.0.1/src/canomaly.egg-info/PKG-INFO` & `canomaly-0.0.2/src/canomaly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canomaly
-Version: 0.0.1
+Version: 0.0.2
 Summary: Detecting cumulative changes in data.
 Author-email: Galen Seilis <galen.seilis@seilis.ca>
 Project-URL: Homepage, https://github.com/galenseilis/canomaly
 Project-URL: Bug Tracker, https://github.com/galenseilis/canomaly/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

