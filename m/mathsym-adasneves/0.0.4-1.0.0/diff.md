# Comparing `tmp/mathsym_adasneves-0.0.4.tar.gz` & `tmp/mathsym_adasneves-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathsym_adasneves-0.0.4.tar", last modified: Sun May 14 18:45:25 2023, max compression
+gzip compressed data, was "mathsym_adasneves-1.0.0.tar", last modified: Sun May 14 18:47:52 2023, max compression
```

## Comparing `mathsym_adasneves-0.0.4.tar` & `mathsym_adasneves-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:45:25.867306 mathsym_adasneves-0.0.4/
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1073 2023-05-13 19:33:38.000000 mathsym_adasneves-0.0.4/LICENSE
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1013 2023-05-14 18:45:25.867306 mathsym_adasneves-0.0.4/PKG-INFO
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      495 2023-05-14 18:40:24.000000 mathsym_adasneves-0.0.4/README.md
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      591 2023-05-14 18:45:13.000000 mathsym_adasneves-0.0.4/pyproject.toml
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       38 2023-05-14 18:45:25.867306 mathsym_adasneves-0.0.4/setup.cfg
-drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:45:25.863306 mathsym_adasneves-0.0.4/src/
-drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:45:25.863306 mathsym_adasneves-0.0.4/src/mathsym_adasneves.egg-info/
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1013 2023-05-14 18:45:25.000000 mathsym_adasneves-0.0.4/src/mathsym_adasneves.egg-info/PKG-INFO
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      286 2023-05-14 18:45:25.000000 mathsym_adasneves-0.0.4/src/mathsym_adasneves.egg-info/SOURCES.txt
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)        1 2023-05-14 18:45:25.000000 mathsym_adasneves-0.0.4/src/mathsym_adasneves.egg-info/dependency_links.txt
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       21 2023-05-14 18:45:25.000000 mathsym_adasneves-0.0.4/src/mathsym_adasneves.egg-info/top_level.txt
-drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:45:25.867306 mathsym_adasneves-0.0.4/src/symMath_adasneves127/
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:38:36.000000 mathsym_adasneves-0.0.4/src/symMath_adasneves127/__init__.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     7362 2023-05-14 18:45:02.000000 mathsym_adasneves-0.0.4/src/symMath_adasneves127/equation.py
+drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:47:52.553814 mathsym_adasneves-1.0.0/
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1073 2023-05-13 19:33:38.000000 mathsym_adasneves-1.0.0/LICENSE
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1013 2023-05-14 18:47:52.553814 mathsym_adasneves-1.0.0/PKG-INFO
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      495 2023-05-14 18:40:24.000000 mathsym_adasneves-1.0.0/README.md
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      591 2023-05-14 18:47:31.000000 mathsym_adasneves-1.0.0/pyproject.toml
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       38 2023-05-14 18:47:52.553814 mathsym_adasneves-1.0.0/setup.cfg
+drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:47:52.549813 mathsym_adasneves-1.0.0/src/
+drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:47:52.549813 mathsym_adasneves-1.0.0/src/mathsym_adasneves.egg-info/
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1013 2023-05-14 18:47:52.000000 mathsym_adasneves-1.0.0/src/mathsym_adasneves.egg-info/PKG-INFO
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      286 2023-05-14 18:47:52.000000 mathsym_adasneves-1.0.0/src/mathsym_adasneves.egg-info/SOURCES.txt
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)        1 2023-05-14 18:47:52.000000 mathsym_adasneves-1.0.0/src/mathsym_adasneves.egg-info/dependency_links.txt
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       21 2023-05-14 18:47:52.000000 mathsym_adasneves-1.0.0/src/mathsym_adasneves.egg-info/top_level.txt
+drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:47:52.553814 mathsym_adasneves-1.0.0/src/symMath_adasneves127/
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:38:36.000000 mathsym_adasneves-1.0.0/src/symMath_adasneves127/__init__.py
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     7362 2023-05-14 18:45:02.000000 mathsym_adasneves-1.0.0/src/symMath_adasneves127/equation.py
```

### Comparing `mathsym_adasneves-0.0.4/LICENSE` & `mathsym_adasneves-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mathsym_adasneves-0.0.4/PKG-INFO` & `mathsym_adasneves-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathsym_adasneves
-Version: 0.0.4
+Version: 1.0.0
 Summary: A small example package
 Author-email: Alex Dasneves <adasneves@adasneves.info>
 Project-URL: Homepage, https://github.com/adasneves127/Symmath
 Project-URL: Bug Tracker, https://github.com/adasneves127/Symmath/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mathsym_adasneves-0.0.4/pyproject.toml` & `mathsym_adasneves-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mathsym_adasneves"
-version = "0.0.4"
+version = "1.0.0"
 authors = [
   { name="Alex Dasneves", email="adasneves@adasneves.info" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `mathsym_adasneves-0.0.4/src/mathsym_adasneves.egg-info/PKG-INFO` & `mathsym_adasneves-1.0.0/src/mathsym_adasneves.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathsym-adasneves
-Version: 0.0.4
+Version: 1.0.0
 Summary: A small example package
 Author-email: Alex Dasneves <adasneves@adasneves.info>
 Project-URL: Homepage, https://github.com/adasneves127/Symmath
 Project-URL: Bug Tracker, https://github.com/adasneves127/Symmath/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mathsym_adasneves-0.0.4/src/symMath_adasneves127/equation.py` & `mathsym_adasneves-1.0.0/src/symMath_adasneves127/equation.py`

 * *Files identical despite different names*

