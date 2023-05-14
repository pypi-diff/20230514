# Comparing `tmp/mathsym_adasneves-0.0.37.tar.gz` & `tmp/mathsym_adasneves-0.0.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathsym_adasneves-0.0.37.tar", last modified: Sun May 14 18:34:20 2023, max compression
+gzip compressed data, was "mathsym_adasneves-0.0.38.tar", last modified: Sun May 14 18:41:12 2023, max compression
```

## Comparing `mathsym_adasneves-0.0.37.tar` & `mathsym_adasneves-0.0.38.tar`

### file list

```diff
@@ -1,19 +1,15 @@
-drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:34:20.127937 mathsym_adasneves-0.0.37/
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1073 2023-05-13 19:33:38.000000 mathsym_adasneves-0.0.37/LICENSE
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1014 2023-05-14 18:34:20.127937 mathsym_adasneves-0.0.37/PKG-INFO
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      495 2023-05-14 18:07:21.000000 mathsym_adasneves-0.0.37/README.md
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      592 2023-05-14 18:34:04.000000 mathsym_adasneves-0.0.37/pyproject.toml
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       38 2023-05-14 18:34:20.127937 mathsym_adasneves-0.0.37/setup.cfg
-drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:34:20.123937 mathsym_adasneves-0.0.37/src/
-drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:34:20.123937 mathsym_adasneves-0.0.37/src/mathsym_adasneves.egg-info/
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1014 2023-05-14 18:34:20.000000 mathsym_adasneves-0.0.37/src/mathsym_adasneves.egg-info/PKG-INFO
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      429 2023-05-14 18:34:20.000000 mathsym_adasneves-0.0.37/src/mathsym_adasneves.egg-info/SOURCES.txt
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)        1 2023-05-14 18:34:20.000000 mathsym_adasneves-0.0.37/src/mathsym_adasneves.egg-info/dependency_links.txt
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       21 2023-05-14 18:34:20.000000 mathsym_adasneves-0.0.37/src/mathsym_adasneves.egg-info/top_level.txt
-drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:34:20.127937 mathsym_adasneves-0.0.37/src/symMath_adasneves127/
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       30 2023-05-14 18:33:18.000000 mathsym_adasneves-0.0.37/src/symMath_adasneves127/__init__.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      101 2023-05-13 19:33:38.000000 mathsym_adasneves-0.0.37/src/symMath_adasneves127/eq_token.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      238 2023-05-14 18:31:50.000000 mathsym_adasneves-0.0.37/src/symMath_adasneves127/equation.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1815 2023-05-13 19:33:38.000000 mathsym_adasneves-0.0.37/src/symMath_adasneves127/lexer.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     4213 2023-05-14 18:08:12.000000 mathsym_adasneves-0.0.37/src/symMath_adasneves127/parse.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1580 2023-05-14 17:32:52.000000 mathsym_adasneves-0.0.37/src/symMath_adasneves127/tree_node.py
+drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:41:12.918211 mathsym_adasneves-0.0.38/
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1073 2023-05-13 19:33:38.000000 mathsym_adasneves-0.0.38/LICENSE
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1014 2023-05-14 18:41:12.918211 mathsym_adasneves-0.0.38/PKG-INFO
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      495 2023-05-14 18:40:24.000000 mathsym_adasneves-0.0.38/README.md
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      592 2023-05-14 18:41:02.000000 mathsym_adasneves-0.0.38/pyproject.toml
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       38 2023-05-14 18:41:12.918211 mathsym_adasneves-0.0.38/setup.cfg
+drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:41:12.914211 mathsym_adasneves-0.0.38/src/
+drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:41:12.918211 mathsym_adasneves-0.0.38/src/mathsym_adasneves.egg-info/
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1014 2023-05-14 18:41:12.000000 mathsym_adasneves-0.0.38/src/mathsym_adasneves.egg-info/PKG-INFO
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      286 2023-05-14 18:41:12.000000 mathsym_adasneves-0.0.38/src/mathsym_adasneves.egg-info/SOURCES.txt
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)        1 2023-05-14 18:41:12.000000 mathsym_adasneves-0.0.38/src/mathsym_adasneves.egg-info/dependency_links.txt
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       21 2023-05-14 18:41:12.000000 mathsym_adasneves-0.0.38/src/mathsym_adasneves.egg-info/top_level.txt
+drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:41:12.918211 mathsym_adasneves-0.0.38/src/symMath_adasneves127/
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:38:36.000000 mathsym_adasneves-0.0.38/src/symMath_adasneves127/__init__.py
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     7433 2023-05-14 18:40:45.000000 mathsym_adasneves-0.0.38/src/symMath_adasneves127/equation.py
```

### Comparing `mathsym_adasneves-0.0.37/LICENSE` & `mathsym_adasneves-0.0.38/LICENSE`

 * *Files identical despite different names*

### Comparing `mathsym_adasneves-0.0.37/PKG-INFO` & `mathsym_adasneves-0.0.38/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathsym_adasneves
-Version: 0.0.37
+Version: 0.0.38
 Summary: A small example package
 Author-email: Alex Dasneves <adasneves@adasneves.info>
 Project-URL: Homepage, https://github.com/adasneves127/Symmath
 Project-URL: Bug Tracker, https://github.com/adasneves127/Symmath/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,11 +28,12 @@
 The 'equation' function will prvide an object with the following methods for use:
 
 * Print
 * Evaluate
   
 Print will print out how the program interpreted the equation given.
 
-Evaluate takes in a parameter 'x', to be used as the variable placeholder. 
+Evaluate takes in a parameter 'x', to be used as the variable placeholder.
 
 ## More info
+
 [Github](https://github.com/adasneves127/mathSym)
```

### Comparing `mathsym_adasneves-0.0.37/pyproject.toml` & `mathsym_adasneves-0.0.38/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mathsym_adasneves"
-version = "0.0.37"
+version = "0.0.38"
 authors = [
   { name="Alex Dasneves", email="adasneves@adasneves.info" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `mathsym_adasneves-0.0.37/src/mathsym_adasneves.egg-info/PKG-INFO` & `mathsym_adasneves-0.0.38/src/mathsym_adasneves.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathsym-adasneves
-Version: 0.0.37
+Version: 0.0.38
 Summary: A small example package
 Author-email: Alex Dasneves <adasneves@adasneves.info>
 Project-URL: Homepage, https://github.com/adasneves127/Symmath
 Project-URL: Bug Tracker, https://github.com/adasneves127/Symmath/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,11 +28,12 @@
 The 'equation' function will prvide an object with the following methods for use:
 
 * Print
 * Evaluate
   
 Print will print out how the program interpreted the equation given.
 
-Evaluate takes in a parameter 'x', to be used as the variable placeholder. 
+Evaluate takes in a parameter 'x', to be used as the variable placeholder.
 
 ## More info
+
 [Github](https://github.com/adasneves127/mathSym)
```

