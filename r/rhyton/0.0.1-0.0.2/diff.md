# Comparing `tmp/rhyton-0.0.1.tar.gz` & `tmp/rhyton-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rhyton-0.0.1.tar", max compression
+gzip compressed data, was "rhyton-0.0.2.tar", max compression
```

## Comparing `rhyton-0.0.1.tar` & `rhyton-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      577 2023-05-13 21:54:01.218330 rhyton-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-13 21:45:15.999822 rhyton-0.0.1/README.md
--rw-r--r--   0        0        0       71 2023-05-13 21:48:39.813612 rhyton-0.0.1/src/rhyton/__init__.py
--rw-r--r--   0        0        0      277 2023-05-13 21:53:43.320193 rhyton-0.0.1/src/rhyton/dev.py
--rw-r--r--   0        0        0      549 2023-05-13 21:47:23.613813 rhyton-0.0.1/src/rhyton/test.py
--rw-r--r--   0        0        0        0 2023-05-13 13:54:03.144657 rhyton-0.0.1/src/rhyton/transpile_test/for_statement.r
--rw-r--r--   0        0        0      110 2023-05-13 15:00:20.914975 rhyton-0.0.1/src/rhyton/transpile_test/func.r
--rw-r--r--   0        0        0      145 2023-05-13 11:31:18.316591 rhyton-0.0.1/src/rhyton/transpile_test/if_statement.r
--rw-r--r--   0        0        0       28 2023-05-13 09:59:30.744924 rhyton-0.0.1/src/rhyton/transpile_test/var_definition.r
--rw-r--r--   0        0        0     9462 2023-05-13 21:29:39.820365 rhyton-0.0.1/src/rhyton/transpiler.py
--rw-r--r--   0        0        0      853 1970-01-01 00:00:00.000000 rhyton-0.0.1/setup.py
--rw-r--r--   0        0        0      669 1970-01-01 00:00:00.000000 rhyton-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      577 2023-05-13 22:00:48.215062 rhyton-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       96 2023-05-13 22:00:31.726628 rhyton-0.0.2/README.md
+-rw-r--r--   0        0        0       72 2023-05-13 22:00:52.942803 rhyton-0.0.2/src/rhyton/__init__.py
+-rw-r--r--   0        0        0      277 2023-05-13 21:53:43.320193 rhyton-0.0.2/src/rhyton/dev.py
+-rw-r--r--   0        0        0      549 2023-05-13 21:47:23.613813 rhyton-0.0.2/src/rhyton/test.py
+-rw-r--r--   0        0        0        0 2023-05-13 13:54:03.144657 rhyton-0.0.2/src/rhyton/transpile_test/for_statement.r
+-rw-r--r--   0        0        0      110 2023-05-13 15:00:20.914975 rhyton-0.0.2/src/rhyton/transpile_test/func.r
+-rw-r--r--   0        0        0      145 2023-05-13 11:31:18.316591 rhyton-0.0.2/src/rhyton/transpile_test/if_statement.r
+-rw-r--r--   0        0        0       28 2023-05-13 09:59:30.744924 rhyton-0.0.2/src/rhyton/transpile_test/var_definition.r
+-rw-r--r--   0        0        0     9462 2023-05-13 21:29:39.820365 rhyton-0.0.2/src/rhyton/transpiler.py
+-rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 rhyton-0.0.2/setup.py
+-rw-r--r--   0        0        0      761 1970-01-01 00:00:00.000000 rhyton-0.0.2/PKG-INFO
```

### Comparing `rhyton-0.0.1/pyproject.toml` & `rhyton-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Rhyton"
-version = "0.0.1"
+version = "0.0.2"
 description = "R to Python transpiler"
 authors = ["Dmitriy Din <dmitriy1d01@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 rich = "^13.3.5"
```

### Comparing `rhyton-0.0.1/src/rhyton/test.py` & `rhyton-0.0.2/src/rhyton/test.py`

 * *Files identical despite different names*

### Comparing `rhyton-0.0.1/src/rhyton/transpiler.py` & `rhyton-0.0.2/src/rhyton/transpiler.py`

 * *Files identical despite different names*

### Comparing `rhyton-0.0.1/setup.py` & `rhyton-0.0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,17 +16,17 @@
  'rich>=13.3.5,<14.0.0',
  'sexpdata>=1.0.0,<2.0.0',
  'tree-sitter-languages>=1.5.0,<2.0.0',
  'tree-sitter>=0.20.1,<0.21.0']
 
 setup_kwargs = {
     'name': 'rhyton',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': 'R to Python transpiler',
-    'long_description': '',
+    'long_description': '\n# Rhyton - R to Python transpiler\n\nThe library that helps you to move R codebase to Python\n',
     'author': 'Dmitriy Din',
     'author_email': 'dmitriy1d01@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `rhyton-0.0.1/PKG-INFO` & `rhyton-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhyton
-Version: 0.0.1
+Version: 0.0.2
 Summary: R to Python transpiler
 Author: Dmitriy Din
 Author-email: dmitriy1d01@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -14,7 +14,11 @@
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Requires-Dist: sexpdata (>=1.0.0,<2.0.0)
 Requires-Dist: tree-sitter (>=0.20.1,<0.21.0)
 Requires-Dist: tree-sitter-languages (>=1.5.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 
+# Rhyton - R to Python transpiler
+
+The library that helps you to move R codebase to Python
+
```

