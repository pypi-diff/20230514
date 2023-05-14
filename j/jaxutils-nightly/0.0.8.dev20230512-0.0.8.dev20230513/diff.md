# Comparing `tmp/jaxutils-nightly-0.0.8.dev20230512.tar.gz` & `tmp/jaxutils-nightly-0.0.8.dev20230513.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jaxutils-nightly-0.0.8.dev20230512.tar", last modified: Fri May 12 00:06:33 2023, max compression
+gzip compressed data, was "dist/jaxutils-nightly-0.0.8.dev20230513.tar", last modified: Sat May 13 00:06:39 2023, max compression
```

## Comparing `jaxutils-nightly-0.0.8.dev20230512.tar` & `jaxutils-nightly-0.0.8.dev20230513.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-12 00:06:33.310334 jaxutils-nightly-0.0.8.dev20230512/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2023-05-12 00:06:33.310334 jaxutils-nightly-0.0.8.dev20230512/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3004 2023-05-12 00:06:26.000000 jaxutils-nightly-0.0.8.dev20230512/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-12 00:06:33.314334 jaxutils-nightly-0.0.8.dev20230512/jaxutils/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1701 2023-05-12 00:06:26.000000 jaxutils-nightly-0.0.8.dev20230512/jaxutils/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      509 2023-05-12 00:06:33.314334 jaxutils-nightly-0.0.8.dev20230512/jaxutils/_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4944 2023-05-12 00:06:26.000000 jaxutils-nightly-0.0.8.dev20230512/jaxutils/config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3831 2023-05-12 00:06:26.000000 jaxutils-nightly-0.0.8.dev20230512/jaxutils/data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3536 2023-05-12 00:06:26.000000 jaxutils-nightly-0.0.8.dev20230512/jaxutils/dict.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13713 2023-05-12 00:06:26.000000 jaxutils-nightly-0.0.8.dev20230512/jaxutils/parameters.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2802 2023-05-12 00:06:26.000000 jaxutils-nightly-0.0.8.dev20230512/jaxutils/pytree.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-12 00:06:33.310334 jaxutils-nightly-0.0.8.dev20230512/jaxutils_nightly.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2023-05-12 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230512/jaxutils_nightly.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2023-05-12 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230512/jaxutils_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-12 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230512/jaxutils_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-05-12 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230512/jaxutils_nightly.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-05-12 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230512/jaxutils_nightly.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      233 2023-05-12 00:06:33.310334 jaxutils-nightly-0.0.8.dev20230512/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2389 2023-05-12 00:06:26.000000 jaxutils-nightly-0.0.8.dev20230512/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    83607 2023-05-12 00:06:26.000000 jaxutils-nightly-0.0.8.dev20230512/versioneer.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-13 00:06:39.841747 jaxutils-nightly-0.0.8.dev20230513/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2023-05-13 00:06:39.841747 jaxutils-nightly-0.0.8.dev20230513/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3004 2023-05-13 00:06:32.000000 jaxutils-nightly-0.0.8.dev20230513/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-13 00:06:39.841747 jaxutils-nightly-0.0.8.dev20230513/jaxutils/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1701 2023-05-13 00:06:32.000000 jaxutils-nightly-0.0.8.dev20230513/jaxutils/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      509 2023-05-13 00:06:39.841747 jaxutils-nightly-0.0.8.dev20230513/jaxutils/_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4944 2023-05-13 00:06:32.000000 jaxutils-nightly-0.0.8.dev20230513/jaxutils/config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3831 2023-05-13 00:06:32.000000 jaxutils-nightly-0.0.8.dev20230513/jaxutils/data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3536 2023-05-13 00:06:32.000000 jaxutils-nightly-0.0.8.dev20230513/jaxutils/dict.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13713 2023-05-13 00:06:32.000000 jaxutils-nightly-0.0.8.dev20230513/jaxutils/parameters.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2802 2023-05-13 00:06:32.000000 jaxutils-nightly-0.0.8.dev20230513/jaxutils/pytree.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-13 00:06:39.841747 jaxutils-nightly-0.0.8.dev20230513/jaxutils_nightly.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2023-05-13 00:06:39.000000 jaxutils-nightly-0.0.8.dev20230513/jaxutils_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2023-05-13 00:06:39.000000 jaxutils-nightly-0.0.8.dev20230513/jaxutils_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-13 00:06:39.000000 jaxutils-nightly-0.0.8.dev20230513/jaxutils_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-05-13 00:06:39.000000 jaxutils-nightly-0.0.8.dev20230513/jaxutils_nightly.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-05-13 00:06:39.000000 jaxutils-nightly-0.0.8.dev20230513/jaxutils_nightly.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      233 2023-05-13 00:06:39.841747 jaxutils-nightly-0.0.8.dev20230513/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2389 2023-05-13 00:06:32.000000 jaxutils-nightly-0.0.8.dev20230513/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    83607 2023-05-13 00:06:32.000000 jaxutils-nightly-0.0.8.dev20230513/versioneer.py
```

### Comparing `jaxutils-nightly-0.0.8.dev20230512/PKG-INFO` & `jaxutils-nightly-0.0.8.dev20230513/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxutils-nightly
-Version: 0.0.8.dev20230512
+Version: 0.0.8.dev20230513
 Summary: Utility functions for JaxGaussianProcesses
 Home-page: UNKNOWN
 Author: Daniel Dodd and Thomas Pinder
 Author-email: tompinder@live.co.uk
 License: LICENSE
 Project-URL: Documentation, https://JaxUitls.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/JaxGaussianProcesses/JaxUitls
```

### Comparing `jaxutils-nightly-0.0.8.dev20230512/README.md` & `jaxutils-nightly-0.0.8.dev20230513/README.md`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230512/jaxutils/__init__.py` & `jaxutils-nightly-0.0.8.dev20230513/jaxutils/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230512/jaxutils/config.py` & `jaxutils-nightly-0.0.8.dev20230513/jaxutils/config.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230512/jaxutils/data.py` & `jaxutils-nightly-0.0.8.dev20230513/jaxutils/data.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230512/jaxutils/dict.py` & `jaxutils-nightly-0.0.8.dev20230513/jaxutils/dict.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230512/jaxutils/parameters.py` & `jaxutils-nightly-0.0.8.dev20230513/jaxutils/parameters.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230512/jaxutils/pytree.py` & `jaxutils-nightly-0.0.8.dev20230513/jaxutils/pytree.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230512/jaxutils_nightly.egg-info/PKG-INFO` & `jaxutils-nightly-0.0.8.dev20230513/jaxutils_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxutils-nightly
-Version: 0.0.8.dev20230512
+Version: 0.0.8.dev20230513
 Summary: Utility functions for JaxGaussianProcesses
 Home-page: UNKNOWN
 Author: Daniel Dodd and Thomas Pinder
 Author-email: tompinder@live.co.uk
 License: LICENSE
 Project-URL: Documentation, https://JaxUitls.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/JaxGaussianProcesses/JaxUitls
```

### Comparing `jaxutils-nightly-0.0.8.dev20230512/setup.py` & `jaxutils-nightly-0.0.8.dev20230513/setup.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230512/versioneer.py` & `jaxutils-nightly-0.0.8.dev20230513/versioneer.py`

 * *Files identical despite different names*

