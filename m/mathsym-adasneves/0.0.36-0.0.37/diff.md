# Comparing `tmp/mathsym_adasneves-0.0.36.tar.gz` & `tmp/mathsym_adasneves-0.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathsym_adasneves-0.0.36.tar", last modified: Sun May 14 18:32:13 2023, max compression
+gzip compressed data, was "mathsym_adasneves-0.0.37.tar", last modified: Sun May 14 18:34:20 2023, max compression
```

## Comparing `mathsym_adasneves-0.0.36.tar` & `mathsym_adasneves-0.0.37.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:32:13.902671 mathsym_adasneves-0.0.36/
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1073 2023-05-13 19:33:38.000000 mathsym_adasneves-0.0.36/LICENSE
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1014 2023-05-14 18:32:13.898671 mathsym_adasneves-0.0.36/PKG-INFO
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      495 2023-05-14 18:07:21.000000 mathsym_adasneves-0.0.36/README.md
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      592 2023-05-14 18:32:03.000000 mathsym_adasneves-0.0.36/pyproject.toml
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       38 2023-05-14 18:32:13.902671 mathsym_adasneves-0.0.36/setup.cfg
-drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:32:13.894671 mathsym_adasneves-0.0.36/src/
-drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:32:13.898671 mathsym_adasneves-0.0.36/src/mathsym_adasneves.egg-info/
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1014 2023-05-14 18:32:13.000000 mathsym_adasneves-0.0.36/src/mathsym_adasneves.egg-info/PKG-INFO
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      429 2023-05-14 18:32:13.000000 mathsym_adasneves-0.0.36/src/mathsym_adasneves.egg-info/SOURCES.txt
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)        1 2023-05-14 18:32:13.000000 mathsym_adasneves-0.0.36/src/mathsym_adasneves.egg-info/dependency_links.txt
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       21 2023-05-14 18:32:13.000000 mathsym_adasneves-0.0.36/src/mathsym_adasneves.egg-info/top_level.txt
-drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:32:13.898671 mathsym_adasneves-0.0.36/src/symMath_adasneves127/
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       31 2023-05-14 18:31:51.000000 mathsym_adasneves-0.0.36/src/symMath_adasneves127/__init__.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      101 2023-05-13 19:33:38.000000 mathsym_adasneves-0.0.36/src/symMath_adasneves127/eq_token.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      238 2023-05-14 18:31:50.000000 mathsym_adasneves-0.0.36/src/symMath_adasneves127/equation.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1815 2023-05-13 19:33:38.000000 mathsym_adasneves-0.0.36/src/symMath_adasneves127/lexer.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     4213 2023-05-14 18:08:12.000000 mathsym_adasneves-0.0.36/src/symMath_adasneves127/parse.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1580 2023-05-14 17:32:52.000000 mathsym_adasneves-0.0.36/src/symMath_adasneves127/tree_node.py
+drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:34:20.127937 mathsym_adasneves-0.0.37/
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1073 2023-05-13 19:33:38.000000 mathsym_adasneves-0.0.37/LICENSE
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1014 2023-05-14 18:34:20.127937 mathsym_adasneves-0.0.37/PKG-INFO
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      495 2023-05-14 18:07:21.000000 mathsym_adasneves-0.0.37/README.md
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      592 2023-05-14 18:34:04.000000 mathsym_adasneves-0.0.37/pyproject.toml
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       38 2023-05-14 18:34:20.127937 mathsym_adasneves-0.0.37/setup.cfg
+drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:34:20.123937 mathsym_adasneves-0.0.37/src/
+drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:34:20.123937 mathsym_adasneves-0.0.37/src/mathsym_adasneves.egg-info/
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1014 2023-05-14 18:34:20.000000 mathsym_adasneves-0.0.37/src/mathsym_adasneves.egg-info/PKG-INFO
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      429 2023-05-14 18:34:20.000000 mathsym_adasneves-0.0.37/src/mathsym_adasneves.egg-info/SOURCES.txt
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)        1 2023-05-14 18:34:20.000000 mathsym_adasneves-0.0.37/src/mathsym_adasneves.egg-info/dependency_links.txt
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       21 2023-05-14 18:34:20.000000 mathsym_adasneves-0.0.37/src/mathsym_adasneves.egg-info/top_level.txt
+drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:34:20.127937 mathsym_adasneves-0.0.37/src/symMath_adasneves127/
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       30 2023-05-14 18:33:18.000000 mathsym_adasneves-0.0.37/src/symMath_adasneves127/__init__.py
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      101 2023-05-13 19:33:38.000000 mathsym_adasneves-0.0.37/src/symMath_adasneves127/eq_token.py
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      238 2023-05-14 18:31:50.000000 mathsym_adasneves-0.0.37/src/symMath_adasneves127/equation.py
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1815 2023-05-13 19:33:38.000000 mathsym_adasneves-0.0.37/src/symMath_adasneves127/lexer.py
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     4213 2023-05-14 18:08:12.000000 mathsym_adasneves-0.0.37/src/symMath_adasneves127/parse.py
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1580 2023-05-14 17:32:52.000000 mathsym_adasneves-0.0.37/src/symMath_adasneves127/tree_node.py
```

### Comparing `mathsym_adasneves-0.0.36/LICENSE` & `mathsym_adasneves-0.0.37/LICENSE`

 * *Files identical despite different names*

### Comparing `mathsym_adasneves-0.0.36/PKG-INFO` & `mathsym_adasneves-0.0.37/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathsym_adasneves
-Version: 0.0.36
+Version: 0.0.37
 Summary: A small example package
 Author-email: Alex Dasneves <adasneves@adasneves.info>
 Project-URL: Homepage, https://github.com/adasneves127/Symmath
 Project-URL: Bug Tracker, https://github.com/adasneves127/Symmath/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mathsym_adasneves-0.0.36/pyproject.toml` & `mathsym_adasneves-0.0.37/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mathsym_adasneves"
-version = "0.0.36"
+version = "0.0.37"
 authors = [
   { name="Alex Dasneves", email="adasneves@adasneves.info" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `mathsym_adasneves-0.0.36/src/mathsym_adasneves.egg-info/PKG-INFO` & `mathsym_adasneves-0.0.37/src/mathsym_adasneves.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathsym-adasneves
-Version: 0.0.36
+Version: 0.0.37
 Summary: A small example package
 Author-email: Alex Dasneves <adasneves@adasneves.info>
 Project-URL: Homepage, https://github.com/adasneves127/Symmath
 Project-URL: Bug Tracker, https://github.com/adasneves127/Symmath/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mathsym_adasneves-0.0.36/src/symMath_adasneves127/lexer.py` & `mathsym_adasneves-0.0.37/src/symMath_adasneves127/lexer.py`

 * *Files identical despite different names*

### Comparing `mathsym_adasneves-0.0.36/src/symMath_adasneves127/parse.py` & `mathsym_adasneves-0.0.37/src/symMath_adasneves127/parse.py`

 * *Files identical despite different names*

### Comparing `mathsym_adasneves-0.0.36/src/symMath_adasneves127/tree_node.py` & `mathsym_adasneves-0.0.37/src/symMath_adasneves127/tree_node.py`

 * *Files identical despite different names*

