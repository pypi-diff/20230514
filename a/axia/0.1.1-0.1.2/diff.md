# Comparing `tmp/axia-0.1.1.tar.gz` & `tmp/axia-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axia-0.1.1.tar", last modified: Sun May 14 18:24:38 2023, max compression
+gzip compressed data, was "axia-0.1.2.tar", last modified: Sun May 14 18:44:09 2023, max compression
```

## Comparing `axia-0.1.1.tar` & `axia-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 fernandonogueira   (501) staff       (20)        0 2023-05-14 18:24:38.942932 axia-0.1.1/
--rw-rw-r--   0 fernandonogueira   (501) staff       (20)     1074 2023-05-13 22:56:47.000000 axia-0.1.1/LICENSE
--rw-r--r--   0 fernandonogueira   (501) staff       (20)     1881 2023-05-14 18:24:38.942792 axia-0.1.1/PKG-INFO
--rw-rw-r--   0 fernandonogueira   (501) staff       (20)     1349 2023-05-13 23:25:25.000000 axia-0.1.1/README.md
-drwxr-xr-x   0 fernandonogueira   (501) staff       (20)        0 2023-05-14 18:24:38.941361 axia-0.1.1/axia/
--rw-rw-r--   0 fernandonogueira   (501) staff       (20)       38 2023-05-12 20:48:52.000000 axia-0.1.1/axia/__init__.py
--rw-rw-r--   0 fernandonogueira   (501) staff       (20)     4340 2023-05-12 20:48:52.000000 axia-0.1.1/axia/dataset.py
--rw-rw-r--   0 fernandonogueira   (501) staff       (20)     2929 2023-05-12 20:48:52.000000 axia-0.1.1/axia/loader.py
--rw-rw-r--   0 fernandonogueira   (501) staff       (20)     3909 2023-05-12 20:48:52.000000 axia-0.1.1/axia/report.py
--rw-rw-r--   0 fernandonogueira   (501) staff       (20)    16652 2023-05-12 20:48:52.000000 axia-0.1.1/axia/sbg_survival.py
--rw-rw-r--   0 fernandonogueira   (501) staff       (20)    33343 2023-05-12 20:48:52.000000 axia-0.1.1/axia/shifted_beta_geometric.py
--rw-rw-r--   0 fernandonogueira   (501) staff       (20)    34796 2023-05-12 20:48:52.000000 axia-0.1.1/axia/util.py
-drwxr-xr-x   0 fernandonogueira   (501) staff       (20)        0 2023-05-14 18:24:38.942029 axia-0.1.1/axia.egg-info/
--rw-rw-r--   0 fernandonogueira   (501) staff       (20)     1881 2023-05-14 18:24:38.000000 axia-0.1.1/axia.egg-info/PKG-INFO
--rw-rw-r--   0 fernandonogueira   (501) staff       (20)      339 2023-05-14 18:24:38.000000 axia-0.1.1/axia.egg-info/SOURCES.txt
--rw-rw-r--   0 fernandonogueira   (501) staff       (20)        1 2023-05-14 18:24:38.000000 axia-0.1.1/axia.egg-info/dependency_links.txt
--rw-rw-r--   0 fernandonogueira   (501) staff       (20)        5 2023-05-14 18:24:38.000000 axia-0.1.1/axia.egg-info/top_level.txt
--rw-rw-r--   0 fernandonogueira   (501) staff       (20)      606 2023-05-14 18:24:27.000000 axia-0.1.1/pyproject.toml
--rw-r--r--   0 fernandonogueira   (501) staff       (20)       38 2023-05-14 18:24:38.942975 axia-0.1.1/setup.cfg
-drwxr-xr-x   0 fernandonogueira   (501) staff       (20)        0 2023-05-14 18:24:38.942596 axia-0.1.1/tests/
--rw-rw-r--   0 fernandonogueira   (501) staff       (20)     2579 2023-05-13 16:10:24.000000 axia-0.1.1/tests/test_fader_hardie.py
--rw-rw-r--   0 fernandonogueira   (501) staff       (20)     8132 2023-05-12 20:48:52.000000 axia-0.1.1/tests/test_report.py
--rw-rw-r--   0 fernandonogueira   (501) staff       (20)     6627 2023-05-12 20:48:52.000000 axia-0.1.1/tests/test_util.py
+drwxr-xr-x   0 fernandonogueira   (501) staff       (20)        0 2023-05-14 18:44:09.327772 axia-0.1.2/
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)     1074 2023-05-13 22:56:47.000000 axia-0.1.2/LICENSE
+-rw-r--r--   0 fernandonogueira   (501) staff       (20)     1881 2023-05-14 18:44:09.327636 axia-0.1.2/PKG-INFO
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)     1349 2023-05-13 23:25:25.000000 axia-0.1.2/README.md
+drwxr-xr-x   0 fernandonogueira   (501) staff       (20)        0 2023-05-14 18:44:09.326075 axia-0.1.2/axia/
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)       38 2023-05-12 20:48:52.000000 axia-0.1.2/axia/__init__.py
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)     4340 2023-05-12 20:48:52.000000 axia-0.1.2/axia/dataset.py
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)     2929 2023-05-12 20:48:52.000000 axia-0.1.2/axia/loader.py
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)     3909 2023-05-12 20:48:52.000000 axia-0.1.2/axia/report.py
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)    16652 2023-05-12 20:48:52.000000 axia-0.1.2/axia/sbg_survival.py
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)    33343 2023-05-12 20:48:52.000000 axia-0.1.2/axia/shifted_beta_geometric.py
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)    34796 2023-05-12 20:48:52.000000 axia-0.1.2/axia/util.py
+drwxr-xr-x   0 fernandonogueira   (501) staff       (20)        0 2023-05-14 18:44:09.326831 axia-0.1.2/axia.egg-info/
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)     1881 2023-05-14 18:44:09.000000 axia-0.1.2/axia.egg-info/PKG-INFO
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)      339 2023-05-14 18:44:09.000000 axia-0.1.2/axia.egg-info/SOURCES.txt
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)        1 2023-05-14 18:44:09.000000 axia-0.1.2/axia.egg-info/dependency_links.txt
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)        5 2023-05-14 18:44:09.000000 axia-0.1.2/axia.egg-info/top_level.txt
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)      606 2023-05-14 18:43:44.000000 axia-0.1.2/pyproject.toml
+-rw-r--r--   0 fernandonogueira   (501) staff       (20)       38 2023-05-14 18:44:09.327821 axia-0.1.2/setup.cfg
+drwxr-xr-x   0 fernandonogueira   (501) staff       (20)        0 2023-05-14 18:44:09.327442 axia-0.1.2/tests/
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)     2579 2023-05-13 16:10:24.000000 axia-0.1.2/tests/test_fader_hardie.py
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)     8132 2023-05-12 20:48:52.000000 axia-0.1.2/tests/test_report.py
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)     6627 2023-05-12 20:48:52.000000 axia-0.1.2/tests/test_util.py
```

### Comparing `axia-0.1.1/LICENSE` & `axia-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `axia-0.1.1/PKG-INFO` & `axia-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: axia
-Version: 0.1.1
+Version: 0.1.2
 Summary: An alternative to survival analysis using the shifted beta-geometric model.
 Author-email: Fernando Nogueira <author@example.com>
 Project-URL: Homepage, https://github.com/fmfn/axia
 Project-URL: Bug Tracker, https://github.com/fmfn/axia/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `axia-0.1.1/README.md` & `axia-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `axia-0.1.1/axia/dataset.py` & `axia-0.1.2/axia/dataset.py`

 * *Files identical despite different names*

### Comparing `axia-0.1.1/axia/loader.py` & `axia-0.1.2/axia/loader.py`

 * *Files identical despite different names*

### Comparing `axia-0.1.1/axia/report.py` & `axia-0.1.2/axia/report.py`

 * *Files identical despite different names*

### Comparing `axia-0.1.1/axia/sbg_survival.py` & `axia-0.1.2/axia/sbg_survival.py`

 * *Files identical despite different names*

### Comparing `axia-0.1.1/axia/shifted_beta_geometric.py` & `axia-0.1.2/axia/shifted_beta_geometric.py`

 * *Files identical despite different names*

### Comparing `axia-0.1.1/axia/util.py` & `axia-0.1.2/axia/util.py`

 * *Files identical despite different names*

### Comparing `axia-0.1.1/axia.egg-info/PKG-INFO` & `axia-0.1.2/axia.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: axia
-Version: 0.1.1
+Version: 0.1.2
 Summary: An alternative to survival analysis using the shifted beta-geometric model.
 Author-email: Fernando Nogueira <author@example.com>
 Project-URL: Homepage, https://github.com/fmfn/axia
 Project-URL: Bug Tracker, https://github.com/fmfn/axia/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `axia-0.1.1/pyproject.toml` & `axia-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "axia"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Fernando Nogueira", email="author@example.com" },
 ]
 description = "An alternative to survival analysis using the shifted beta-geometric model."
 readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
```

### Comparing `axia-0.1.1/tests/test_fader_hardie.py` & `axia-0.1.2/tests/test_fader_hardie.py`

 * *Files identical despite different names*

### Comparing `axia-0.1.1/tests/test_report.py` & `axia-0.1.2/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `axia-0.1.1/tests/test_util.py` & `axia-0.1.2/tests/test_util.py`

 * *Files identical despite different names*

