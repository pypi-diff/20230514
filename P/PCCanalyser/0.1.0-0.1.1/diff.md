# Comparing `tmp/PCCanalyser-0.1.0.tar.gz` & `tmp/PCCanalyser-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PCCanalyser-0.1.0.tar", last modified: Sun May 14 20:07:31 2023, max compression
+gzip compressed data, was "PCCanalyser-0.1.1.tar", last modified: Sun May 14 21:37:34 2023, max compression
```

## Comparing `PCCanalyser-0.1.0.tar` & `PCCanalyser-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-05-14 20:07:31.104398 PCCanalyser-0.1.0/
--rw-r--r--   0 v94623eb2   (504) staff       (20)    35149 2022-09-08 11:03:35.000000 PCCanalyser-0.1.0/LICENSE
-drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-05-14 20:07:31.099744 PCCanalyser-0.1.0/PCCanalyser.egg-info/
--rw-r--r--   0 v94623eb2   (504) staff       (20)       77 2023-05-14 20:07:31.000000 PCCanalyser-0.1.0/PCCanalyser.egg-info/PKG-INFO
--rw-r--r--   0 v94623eb2   (504) staff       (20)      463 2023-05-14 20:07:31.000000 PCCanalyser-0.1.0/PCCanalyser.egg-info/SOURCES.txt
--rw-r--r--   0 v94623eb2   (504) staff       (20)        1 2023-05-14 20:07:31.000000 PCCanalyser-0.1.0/PCCanalyser.egg-info/dependency_links.txt
--rw-r--r--   0 v94623eb2   (504) staff       (20)      172 2023-05-14 20:07:31.000000 PCCanalyser-0.1.0/PCCanalyser.egg-info/entry_points.txt
--rw-r--r--   0 v94623eb2   (504) staff       (20)       39 2023-05-14 20:07:31.000000 PCCanalyser-0.1.0/PCCanalyser.egg-info/requires.txt
--rw-r--r--   0 v94623eb2   (504) staff       (20)       13 2023-05-14 20:07:31.000000 PCCanalyser-0.1.0/PCCanalyser.egg-info/top_level.txt
--rw-r--r--   0 v94623eb2   (504) staff       (20)       77 2023-05-14 20:07:31.104123 PCCanalyser-0.1.0/PKG-INFO
--rw-r--r--   0 v94623eb2   (504) staff       (20)    15312 2023-02-27 16:00:34.000000 PCCanalyser-0.1.0/README.md
-drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-05-14 20:07:31.102983 PCCanalyser-0.1.0/matgen/
--rw-r--r--   0 v94623eb2   (504) staff       (20)        0 2022-09-08 11:03:35.000000 PCCanalyser-0.1.0/matgen/__init__.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)    63479 2023-04-26 12:13:35.000000 PCCanalyser-0.1.0/matgen/base.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)     2368 2023-02-27 16:00:34.000000 PCCanalyser-0.1.0/matgen/characterise.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)    22427 2023-05-04 12:15:07.000000 PCCanalyser-0.1.0/matgen/matutils.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)     1567 2023-05-03 12:47:14.000000 PCCanalyser-0.1.0/matgen/ndisangles.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)     3034 2023-05-03 12:47:22.000000 PCCanalyser-0.1.0/matgen/ndisorientquat.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)    12073 2023-05-03 12:39:22.000000 PCCanalyser-0.1.0/matgen/sparsemat.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)     2145 2023-04-26 12:13:35.000000 PCCanalyser-0.1.0/matgen/utils.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)      620 2023-05-14 20:05:52.000000 PCCanalyser-0.1.0/pyproject.toml
--rw-r--r--   0 v94623eb2   (504) staff       (20)       38 2023-05-14 20:07:31.104455 PCCanalyser-0.1.0/setup.cfg
-drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-05-14 20:07:31.103756 PCCanalyser-0.1.0/tests/
--rw-r--r--   0 v94623eb2   (504) staff       (20)        0 2022-09-08 11:03:35.000000 PCCanalyser-0.1.0/tests/__init__.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)      298 2023-02-27 16:00:35.000000 PCCanalyser-0.1.0/tests/test_base.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)      466 2023-05-03 12:11:10.000000 PCCanalyser-0.1.0/tests/test_sparsemat.py
+drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-05-14 21:37:34.951014 PCCanalyser-0.1.1/
+-rw-r--r--   0 v94623eb2   (504) staff       (20)    35149 2022-09-08 11:03:35.000000 PCCanalyser-0.1.1/LICENSE
+drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-05-14 21:37:34.948017 PCCanalyser-0.1.1/PCCanalyser.egg-info/
+-rw-r--r--   0 v94623eb2   (504) staff       (20)      130 2023-05-14 21:37:34.000000 PCCanalyser-0.1.1/PCCanalyser.egg-info/PKG-INFO
+-rw-r--r--   0 v94623eb2   (504) staff       (20)      463 2023-05-14 21:37:34.000000 PCCanalyser-0.1.1/PCCanalyser.egg-info/SOURCES.txt
+-rw-r--r--   0 v94623eb2   (504) staff       (20)        1 2023-05-14 21:37:34.000000 PCCanalyser-0.1.1/PCCanalyser.egg-info/dependency_links.txt
+-rw-r--r--   0 v94623eb2   (504) staff       (20)      172 2023-05-14 21:37:34.000000 PCCanalyser-0.1.1/PCCanalyser.egg-info/entry_points.txt
+-rw-r--r--   0 v94623eb2   (504) staff       (20)       39 2023-05-14 21:37:34.000000 PCCanalyser-0.1.1/PCCanalyser.egg-info/requires.txt
+-rw-r--r--   0 v94623eb2   (504) staff       (20)       13 2023-05-14 21:37:34.000000 PCCanalyser-0.1.1/PCCanalyser.egg-info/top_level.txt
+-rw-r--r--   0 v94623eb2   (504) staff       (20)      130 2023-05-14 21:37:34.950805 PCCanalyser-0.1.1/PKG-INFO
+-rw-r--r--   0 v94623eb2   (504) staff       (20)    15312 2023-02-27 16:00:34.000000 PCCanalyser-0.1.1/README.md
+drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-05-14 21:37:34.949924 PCCanalyser-0.1.1/matgen/
+-rw-r--r--   0 v94623eb2   (504) staff       (20)        0 2022-09-08 11:03:35.000000 PCCanalyser-0.1.1/matgen/__init__.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)    63479 2023-04-26 12:13:35.000000 PCCanalyser-0.1.1/matgen/base.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)     2368 2023-02-27 16:00:34.000000 PCCanalyser-0.1.1/matgen/characterise.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)    22427 2023-05-04 12:15:07.000000 PCCanalyser-0.1.1/matgen/matutils.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)     1567 2023-05-03 12:47:14.000000 PCCanalyser-0.1.1/matgen/ndisangles.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)     3034 2023-05-03 12:47:22.000000 PCCanalyser-0.1.1/matgen/ndisorientquat.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)    12073 2023-05-03 12:39:22.000000 PCCanalyser-0.1.1/matgen/sparsemat.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)     2145 2023-04-26 12:13:35.000000 PCCanalyser-0.1.1/matgen/utils.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)      680 2023-05-14 21:37:24.000000 PCCanalyser-0.1.1/pyproject.toml
+-rw-r--r--   0 v94623eb2   (504) staff       (20)       38 2023-05-14 21:37:34.951065 PCCanalyser-0.1.1/setup.cfg
+drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-05-14 21:37:34.950592 PCCanalyser-0.1.1/tests/
+-rw-r--r--   0 v94623eb2   (504) staff       (20)        0 2022-09-08 11:03:35.000000 PCCanalyser-0.1.1/tests/__init__.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)      298 2023-02-27 16:00:35.000000 PCCanalyser-0.1.1/tests/test_base.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)      466 2023-05-03 12:11:10.000000 PCCanalyser-0.1.1/tests/test_sparsemat.py
```

### Comparing `PCCanalyser-0.1.0/LICENSE` & `PCCanalyser-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.1.0/README.md` & `PCCanalyser-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.1.0/matgen/base.py` & `PCCanalyser-0.1.1/matgen/base.py`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.1.0/matgen/characterise.py` & `PCCanalyser-0.1.1/matgen/characterise.py`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.1.0/matgen/matutils.py` & `PCCanalyser-0.1.1/matgen/matutils.py`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.1.0/matgen/ndisangles.py` & `PCCanalyser-0.1.1/matgen/ndisangles.py`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.1.0/matgen/ndisorientquat.py` & `PCCanalyser-0.1.1/matgen/ndisorientquat.py`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.1.0/matgen/sparsemat.py` & `PCCanalyser-0.1.1/matgen/sparsemat.py`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.1.0/matgen/utils.py` & `PCCanalyser-0.1.1/matgen/utils.py`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.1.0/pyproject.toml` & `PCCanalyser-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PCCanalyser"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
     "numpy", "scipy", "tqdm", "jupyterlab", 
     "matplotlib",
 ]
+description = "Polyhedral Cell Complex (PCC) Analysis tool"
 
 [tool.setuptools.packages.find]
 # All the following settings are optional:
 where = ["."]  # ["."] by default
 include = ["*"]  # ["*"] by default
 exclude = ["tutorial"]  # empty by default
 namespaces = false  # true by default
```

