# Comparing `tmp/rhyton-0.0.3.tar.gz` & `tmp/rhyton-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rhyton-0.0.3.tar", max compression
+gzip compressed data, was "rhyton-0.0.4.tar", max compression
```

## Comparing `rhyton-0.0.3.tar` & `rhyton-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      577 2023-05-14 11:23:43.147118 rhyton-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1910 2023-05-14 11:20:38.193764 rhyton-0.0.3/README.md
--rw-r--r--   0        0        0       72 2023-05-14 11:23:39.793340 rhyton-0.0.3/src/rhyton/__init__.py
--rw-r--r--   0        0        0      277 2023-05-13 21:53:43.320193 rhyton-0.0.3/src/rhyton/dev.py
--rw-r--r--   0        0        0      549 2023-05-13 21:47:23.613813 rhyton-0.0.3/src/rhyton/test.py
--rw-r--r--   0        0        0        0 2023-05-13 13:54:03.144657 rhyton-0.0.3/src/rhyton/transpile_test/for_statement.r
--rw-r--r--   0        0        0      110 2023-05-13 15:00:20.914975 rhyton-0.0.3/src/rhyton/transpile_test/func.r
--rw-r--r--   0        0        0      145 2023-05-13 11:31:18.316591 rhyton-0.0.3/src/rhyton/transpile_test/if_statement.r
--rw-r--r--   0        0        0       28 2023-05-13 09:59:30.744924 rhyton-0.0.3/src/rhyton/transpile_test/var_definition.r
--rw-r--r--   0        0        0     9462 2023-05-13 21:29:39.820365 rhyton-0.0.3/src/rhyton/transpiler.py
--rw-r--r--   0        0        0     2770 1970-01-01 00:00:00.000000 rhyton-0.0.3/setup.py
--rw-r--r--   0        0        0     2521 1970-01-01 00:00:00.000000 rhyton-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      577 2023-05-14 11:24:42.259750 rhyton-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1911 2023-05-14 11:24:31.873850 rhyton-0.0.4/README.md
+-rw-r--r--   0        0        0       72 2023-05-14 11:24:35.626996 rhyton-0.0.4/src/rhyton/__init__.py
+-rw-r--r--   0        0        0      277 2023-05-13 21:53:43.320193 rhyton-0.0.4/src/rhyton/dev.py
+-rw-r--r--   0        0        0      549 2023-05-13 21:47:23.613813 rhyton-0.0.4/src/rhyton/test.py
+-rw-r--r--   0        0        0        0 2023-05-13 13:54:03.144657 rhyton-0.0.4/src/rhyton/transpile_test/for_statement.r
+-rw-r--r--   0        0        0      110 2023-05-13 15:00:20.914975 rhyton-0.0.4/src/rhyton/transpile_test/func.r
+-rw-r--r--   0        0        0      145 2023-05-13 11:31:18.316591 rhyton-0.0.4/src/rhyton/transpile_test/if_statement.r
+-rw-r--r--   0        0        0       28 2023-05-13 09:59:30.744924 rhyton-0.0.4/src/rhyton/transpile_test/var_definition.r
+-rw-r--r--   0        0        0     9462 2023-05-13 21:29:39.820365 rhyton-0.0.4/src/rhyton/transpiler.py
+-rw-r--r--   0        0        0     2771 1970-01-01 00:00:00.000000 rhyton-0.0.4/setup.py
+-rw-r--r--   0        0        0     2522 1970-01-01 00:00:00.000000 rhyton-0.0.4/PKG-INFO
```

### Comparing `rhyton-0.0.3/pyproject.toml` & `rhyton-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Rhyton"
-version = "0.0.3"
+version = "0.0.4"
 description = "R to Python transpiler"
 authors = ["Dmitriy Din <dmitriy1d01@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 rich = "^13.3.5"
```

### Comparing `rhyton-0.0.3/README.md` & `rhyton-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <div id="header" align="center">
 <img src="https://i.ibb.co/9mxMf46/rhyton-logo.png" alt="Rhyton logo"/>
   <h1>
     <i>Rhyton</i> - R to Python transpiler
   </h1>
 </div>
 
-##📜 What is _Rhyton_
+## 📜 What is _Rhyton_
 
 __Rhyton__ is a type of ancient Greek drinking vessel that is in the shape of an animal's head or horn and has a hole in the bottom for pouring the liquid. It was often used in religious ceremonies or feasts.
 
 The name came after combination of language names: _R_ and _Python_
 
 This library helps you to move R codebase to Python. Right now it supports conversion of _math equations_, _expressions_, _conditions_, _function definitions_ and _calls_
```

### Comparing `rhyton-0.0.3/src/rhyton/test.py` & `rhyton-0.0.4/src/rhyton/test.py`

 * *Files identical despite different names*

### Comparing `rhyton-0.0.3/src/rhyton/transpiler.py` & `rhyton-0.0.4/src/rhyton/transpiler.py`

 * *Files identical despite different names*

### Comparing `rhyton-0.0.3/setup.py` & `rhyton-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,17 +16,17 @@
  'rich>=13.3.5,<14.0.0',
  'sexpdata>=1.0.0,<2.0.0',
  'tree-sitter-languages>=1.5.0,<2.0.0',
  'tree-sitter>=0.20.1,<0.21.0']
 
 setup_kwargs = {
     'name': 'rhyton',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': 'R to Python transpiler',
-    'long_description': '<div id="header" align="center">\n<img src="https://i.ibb.co/9mxMf46/rhyton-logo.png" alt="Rhyton logo"/>\n  <h1>\n    <i>Rhyton</i> - R to Python transpiler\n  </h1>\n</div>\n\n##📜 What is _Rhyton_\n\n__Rhyton__ is a type of ancient Greek drinking vessel that is in the shape of an animal\'s head or horn and has a hole in the bottom for pouring the liquid. It was often used in religious ceremonies or feasts.\n\nThe name came after combination of language names: _R_ and _Python_\n\nThis library helps you to move R codebase to Python. Right now it supports conversion of _math equations_, _expressions_, _conditions_, _function definitions_ and _calls_\n\n## 🧲 Installation\nThe project is published on [__PyPi__](https://pypi.org/project/rhyton/), so you can install it via __pip__\n\n```shell\n$: pip install rhyton\n```\n\n## 🚀 Launch\nUse _transpile_ or _transpile_file_ to translate your __R__ code\n\n```python\nfrom rhyton import transpile, transpile_file\n\ntranspile(\'x <- 7\') # returns transpiled string\n\n# or\n\ntranspile_file(\n  in_path=\'<path to your R file>.r\', \n  out_path=\'<Path to generated Python file>.py\'\n)\n\n```\n\n## 🛠 How it works\n__Rhyton__ uses tree-sitter under the hood, to compute _AST_ (Abstract Syntax Tree), after that it converts it to new _AST_ that is valid for Python. After that it generates a code, using [_ast module_](https://docs.python.org/3/library/ast.html) and [_astor_](https://astor.readthedocs.io/en/latest/)\n\n## 📊 Feature plan\n* ✅ Add tree parsers\n* ✅ Semantic analysis for _AST_\n  * ✅ Statements and expressions\n  * ✅ Math operations\n  * ✅ Conditions: _if_, _else_\n  * ✅ Function definitions\n  * ✅ Function calls\n  * ❌ Cycles while and for\n  * ❌ Arrays and operations\n  * ❌ Function analogs\n  * ❌ Import statements \n  * ❌ Nested transpilation\n\n* ✅ Package demo publication\n* ✅ Project site\n',
+    'long_description': '<div id="header" align="center">\n<img src="https://i.ibb.co/9mxMf46/rhyton-logo.png" alt="Rhyton logo"/>\n  <h1>\n    <i>Rhyton</i> - R to Python transpiler\n  </h1>\n</div>\n\n## 📜 What is _Rhyton_\n\n__Rhyton__ is a type of ancient Greek drinking vessel that is in the shape of an animal\'s head or horn and has a hole in the bottom for pouring the liquid. It was often used in religious ceremonies or feasts.\n\nThe name came after combination of language names: _R_ and _Python_\n\nThis library helps you to move R codebase to Python. Right now it supports conversion of _math equations_, _expressions_, _conditions_, _function definitions_ and _calls_\n\n## 🧲 Installation\nThe project is published on [__PyPi__](https://pypi.org/project/rhyton/), so you can install it via __pip__\n\n```shell\n$: pip install rhyton\n```\n\n## 🚀 Launch\nUse _transpile_ or _transpile_file_ to translate your __R__ code\n\n```python\nfrom rhyton import transpile, transpile_file\n\ntranspile(\'x <- 7\') # returns transpiled string\n\n# or\n\ntranspile_file(\n  in_path=\'<path to your R file>.r\', \n  out_path=\'<Path to generated Python file>.py\'\n)\n\n```\n\n## 🛠 How it works\n__Rhyton__ uses tree-sitter under the hood, to compute _AST_ (Abstract Syntax Tree), after that it converts it to new _AST_ that is valid for Python. After that it generates a code, using [_ast module_](https://docs.python.org/3/library/ast.html) and [_astor_](https://astor.readthedocs.io/en/latest/)\n\n## 📊 Feature plan\n* ✅ Add tree parsers\n* ✅ Semantic analysis for _AST_\n  * ✅ Statements and expressions\n  * ✅ Math operations\n  * ✅ Conditions: _if_, _else_\n  * ✅ Function definitions\n  * ✅ Function calls\n  * ❌ Cycles while and for\n  * ❌ Arrays and operations\n  * ❌ Function analogs\n  * ❌ Import statements \n  * ❌ Nested transpilation\n\n* ✅ Package demo publication\n* ✅ Project site\n',
     'author': 'Dmitriy Din',
     'author_email': 'dmitriy1d01@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `rhyton-0.0.3/PKG-INFO` & `rhyton-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhyton
-Version: 0.0.3
+Version: 0.0.4
 Summary: R to Python transpiler
 Author: Dmitriy Din
 Author-email: dmitriy1d01@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -20,15 +20,15 @@
 <div id="header" align="center">
 <img src="https://i.ibb.co/9mxMf46/rhyton-logo.png" alt="Rhyton logo"/>
   <h1>
     <i>Rhyton</i> - R to Python transpiler
   </h1>
 </div>
 
-##📜 What is _Rhyton_
+## 📜 What is _Rhyton_
 
 __Rhyton__ is a type of ancient Greek drinking vessel that is in the shape of an animal's head or horn and has a hole in the bottom for pouring the liquid. It was often used in religious ceremonies or feasts.
 
 The name came after combination of language names: _R_ and _Python_
 
 This library helps you to move R codebase to Python. Right now it supports conversion of _math equations_, _expressions_, _conditions_, _function definitions_ and _calls_
```

