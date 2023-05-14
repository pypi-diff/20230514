# Comparing `tmp/canomaly-0.0.4.tar.gz` & `tmp/canomaly-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canomaly-0.0.4.tar", last modified: Sun May 14 03:39:15 2023, max compression
+gzip compressed data, was "canomaly-0.0.5.tar", last modified: Sun May 14 04:13:29 2023, max compression
```

## Comparing `canomaly-0.0.4.tar` & `canomaly-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 03:39:15.927883 canomaly-0.0.4/
--rw-rw-r--   0 galen     (1000) galen     (1000)    35149 2023-05-13 19:23:41.000000 canomaly-0.0.4/LICENSE
--rw-rw-r--   0 galen     (1000) galen     (1000)     2162 2023-05-14 03:39:15.927883 canomaly-0.0.4/PKG-INFO
--rw-rw-r--   0 galen     (1000) galen     (1000)     1643 2023-05-14 02:43:30.000000 canomaly-0.0.4/README.md
--rw-rw-r--   0 galen     (1000) galen     (1000)      593 2023-05-14 03:39:01.000000 canomaly-0.0.4/pyproject.toml
--rw-rw-r--   0 galen     (1000) galen     (1000)       83 2023-05-14 03:39:15.927883 canomaly-0.0.4/setup.cfg
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 03:39:15.919883 canomaly-0.0.4/src/
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 03:39:15.923883 canomaly-0.0.4/src/canomaly/
--rw-rw-r--   0 galen     (1000) galen     (1000)        0 2023-05-13 19:24:11.000000 canomaly-0.0.4/src/canomaly/__init__.py
--rw-rw-r--   0 galen     (1000) galen     (1000)     2527 2023-05-14 03:35:38.000000 canomaly-0.0.4/src/canomaly/searchtools.py
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 03:39:15.927883 canomaly-0.0.4/src/canomaly.egg-info/
--rw-rw-r--   0 galen     (1000) galen     (1000)     2162 2023-05-14 03:39:15.000000 canomaly-0.0.4/src/canomaly.egg-info/PKG-INFO
--rw-rw-r--   0 galen     (1000) galen     (1000)      305 2023-05-14 03:39:15.000000 canomaly-0.0.4/src/canomaly.egg-info/SOURCES.txt
--rw-rw-r--   0 galen     (1000) galen     (1000)        1 2023-05-14 03:39:15.000000 canomaly-0.0.4/src/canomaly.egg-info/dependency_links.txt
--rw-rw-r--   0 galen     (1000) galen     (1000)       12 2023-05-14 03:39:15.000000 canomaly-0.0.4/src/canomaly.egg-info/requires.txt
--rw-rw-r--   0 galen     (1000) galen     (1000)        9 2023-05-14 03:39:15.000000 canomaly-0.0.4/src/canomaly.egg-info/top_level.txt
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 03:39:15.927883 canomaly-0.0.4/tests/
--rw-rw-r--   0 galen     (1000) galen     (1000)     3365 2023-05-14 03:32:01.000000 canomaly-0.0.4/tests/test_cumulative_regex.py
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 04:13:29.560218 canomaly-0.0.5/
+-rw-rw-r--   0 galen     (1000) galen     (1000)    35149 2023-05-13 19:23:41.000000 canomaly-0.0.5/LICENSE
+-rw-rw-r--   0 galen     (1000) galen     (1000)     4305 2023-05-14 04:13:29.560218 canomaly-0.0.5/PKG-INFO
+-rw-rw-r--   0 galen     (1000) galen     (1000)     3786 2023-05-14 04:10:07.000000 canomaly-0.0.5/README.md
+-rw-rw-r--   0 galen     (1000) galen     (1000)      593 2023-05-14 04:13:14.000000 canomaly-0.0.5/pyproject.toml
+-rw-rw-r--   0 galen     (1000) galen     (1000)       83 2023-05-14 04:13:29.564218 canomaly-0.0.5/setup.cfg
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 04:13:29.556218 canomaly-0.0.5/src/
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 04:13:29.560218 canomaly-0.0.5/src/canomaly/
+-rw-rw-r--   0 galen     (1000) galen     (1000)        0 2023-05-13 19:24:11.000000 canomaly-0.0.5/src/canomaly/__init__.py
+-rw-rw-r--   0 galen     (1000) galen     (1000)     3112 2023-05-14 03:57:12.000000 canomaly-0.0.5/src/canomaly/searchtools.py
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 04:13:29.560218 canomaly-0.0.5/src/canomaly.egg-info/
+-rw-rw-r--   0 galen     (1000) galen     (1000)     4305 2023-05-14 04:13:29.000000 canomaly-0.0.5/src/canomaly.egg-info/PKG-INFO
+-rw-rw-r--   0 galen     (1000) galen     (1000)      305 2023-05-14 04:13:29.000000 canomaly-0.0.5/src/canomaly.egg-info/SOURCES.txt
+-rw-rw-r--   0 galen     (1000) galen     (1000)        1 2023-05-14 04:13:29.000000 canomaly-0.0.5/src/canomaly.egg-info/dependency_links.txt
+-rw-rw-r--   0 galen     (1000) galen     (1000)       12 2023-05-14 04:13:29.000000 canomaly-0.0.5/src/canomaly.egg-info/requires.txt
+-rw-rw-r--   0 galen     (1000) galen     (1000)        9 2023-05-14 04:13:29.000000 canomaly-0.0.5/src/canomaly.egg-info/top_level.txt
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 04:13:29.560218 canomaly-0.0.5/tests/
+-rw-rw-r--   0 galen     (1000) galen     (1000)     3365 2023-05-14 03:32:01.000000 canomaly-0.0.5/tests/test_cumulative_regex.py
```

### Comparing `canomaly-0.0.4/LICENSE` & `canomaly-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `canomaly-0.0.4/pyproject.toml` & `canomaly-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "canomaly"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Galen Seilis", email="galen.seilis@seilis.ca" },
 ]
 description = "Detecting cumulative changes in data."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `canomaly-0.0.4/tests/test_cumulative_regex.py` & `canomaly-0.0.5/tests/test_cumulative_regex.py`

 * *Files identical despite different names*

