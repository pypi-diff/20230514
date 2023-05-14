# Comparing `tmp/mathsym_adasneves-0.0.2.tar.gz` & `tmp/mathsym_adasneves-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathsym_adasneves-0.0.2.tar", last modified: Sun May 14 18:10:38 2023, max compression
+gzip compressed data, was "mathsym_adasneves-0.0.3.tar", last modified: Sun May 14 18:14:11 2023, max compression
```

## Comparing `mathsym_adasneves-0.0.2.tar` & `mathsym_adasneves-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:10:38.235368 mathsym_adasneves-0.0.2/
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1073 2023-05-13 19:33:38.000000 mathsym_adasneves-0.0.2/LICENSE
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1013 2023-05-14 18:10:38.235368 mathsym_adasneves-0.0.2/PKG-INFO
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      495 2023-05-14 18:07:21.000000 mathsym_adasneves-0.0.2/README.md
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      591 2023-05-14 18:10:20.000000 mathsym_adasneves-0.0.2/pyproject.toml
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       38 2023-05-14 18:10:38.235368 mathsym_adasneves-0.0.2/setup.cfg
-drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:10:38.231368 mathsym_adasneves-0.0.2/src/
-drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:10:38.235368 mathsym_adasneves-0.0.2/src/mathsym_adasneves.egg-info/
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1013 2023-05-14 18:10:38.000000 mathsym_adasneves-0.0.2/src/mathsym_adasneves.egg-info/PKG-INFO
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      428 2023-05-14 18:10:38.000000 mathsym_adasneves-0.0.2/src/mathsym_adasneves.egg-info/SOURCES.txt
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)        1 2023-05-14 18:10:38.000000 mathsym_adasneves-0.0.2/src/mathsym_adasneves.egg-info/dependency_links.txt
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       21 2023-05-14 18:10:38.000000 mathsym_adasneves-0.0.2/src/mathsym_adasneves.egg-info/top_level.txt
-drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:10:38.235368 mathsym_adasneves-0.0.2/src/symMath_adasneves127/
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:10:10.000000 mathsym_adasneves-0.0.2/src/symMath_adasneves127/__init__.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      101 2023-05-13 19:33:38.000000 mathsym_adasneves-0.0.2/src/symMath_adasneves127/eq_token.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      238 2023-05-14 18:10:05.000000 mathsym_adasneves-0.0.2/src/symMath_adasneves127/eqation.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1815 2023-05-13 19:33:38.000000 mathsym_adasneves-0.0.2/src/symMath_adasneves127/lexer.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     4213 2023-05-14 18:08:12.000000 mathsym_adasneves-0.0.2/src/symMath_adasneves127/parse.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1580 2023-05-14 17:32:52.000000 mathsym_adasneves-0.0.2/src/symMath_adasneves127/tree_node.py
+drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:14:11.984162 mathsym_adasneves-0.0.3/
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1073 2023-05-13 19:33:38.000000 mathsym_adasneves-0.0.3/LICENSE
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1013 2023-05-14 18:14:11.980162 mathsym_adasneves-0.0.3/PKG-INFO
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      495 2023-05-14 18:07:21.000000 mathsym_adasneves-0.0.3/README.md
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      591 2023-05-14 18:13:57.000000 mathsym_adasneves-0.0.3/pyproject.toml
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       38 2023-05-14 18:14:11.984162 mathsym_adasneves-0.0.3/setup.cfg
+drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:14:11.976162 mathsym_adasneves-0.0.3/src/
+drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:14:11.980162 mathsym_adasneves-0.0.3/src/mathsym_adasneves.egg-info/
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1013 2023-05-14 18:14:11.000000 mathsym_adasneves-0.0.3/src/mathsym_adasneves.egg-info/PKG-INFO
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      428 2023-05-14 18:14:11.000000 mathsym_adasneves-0.0.3/src/mathsym_adasneves.egg-info/SOURCES.txt
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)        1 2023-05-14 18:14:11.000000 mathsym_adasneves-0.0.3/src/mathsym_adasneves.egg-info/dependency_links.txt
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       21 2023-05-14 18:14:11.000000 mathsym_adasneves-0.0.3/src/mathsym_adasneves.egg-info/top_level.txt
+drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:14:11.980162 mathsym_adasneves-0.0.3/src/symMath_adasneves127/
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)        0 2023-05-14 18:10:10.000000 mathsym_adasneves-0.0.3/src/symMath_adasneves127/__init__.py
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      101 2023-05-13 19:33:38.000000 mathsym_adasneves-0.0.3/src/symMath_adasneves127/eq_token.py
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      238 2023-05-14 18:10:05.000000 mathsym_adasneves-0.0.3/src/symMath_adasneves127/eqation.py
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1815 2023-05-13 19:33:38.000000 mathsym_adasneves-0.0.3/src/symMath_adasneves127/lexer.py
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     4213 2023-05-14 18:08:12.000000 mathsym_adasneves-0.0.3/src/symMath_adasneves127/parse.py
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1580 2023-05-14 17:32:52.000000 mathsym_adasneves-0.0.3/src/symMath_adasneves127/tree_node.py
```

### Comparing `mathsym_adasneves-0.0.2/LICENSE` & `mathsym_adasneves-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mathsym_adasneves-0.0.2/PKG-INFO` & `mathsym_adasneves-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathsym_adasneves
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Author-email: Alex Dasneves <adasneves@adasneves.info>
 Project-URL: Homepage, https://github.com/adasneves127/Symmath
 Project-URL: Bug Tracker, https://github.com/adasneves127/Symmath/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mathsym_adasneves-0.0.2/pyproject.toml` & `mathsym_adasneves-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mathsym_adasneves"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Alex Dasneves", email="adasneves@adasneves.info" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `mathsym_adasneves-0.0.2/src/mathsym_adasneves.egg-info/PKG-INFO` & `mathsym_adasneves-0.0.3/src/mathsym_adasneves.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathsym-adasneves
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Author-email: Alex Dasneves <adasneves@adasneves.info>
 Project-URL: Homepage, https://github.com/adasneves127/Symmath
 Project-URL: Bug Tracker, https://github.com/adasneves127/Symmath/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mathsym_adasneves-0.0.2/src/symMath_adasneves127/lexer.py` & `mathsym_adasneves-0.0.3/src/symMath_adasneves127/lexer.py`

 * *Files identical despite different names*

### Comparing `mathsym_adasneves-0.0.2/src/symMath_adasneves127/parse.py` & `mathsym_adasneves-0.0.3/src/symMath_adasneves127/parse.py`

 * *Files identical despite different names*

### Comparing `mathsym_adasneves-0.0.2/src/symMath_adasneves127/tree_node.py` & `mathsym_adasneves-0.0.3/src/symMath_adasneves127/tree_node.py`

 * *Files identical despite different names*

