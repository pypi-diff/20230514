# Comparing `tmp/xicorpy-0.2.tar.gz` & `tmp/xicorpy-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xicorpy-0.2.tar", max compression
+gzip compressed data, was "xicorpy-0.3.tar", max compression
```

## Comparing `xicorpy-0.2.tar` & `xicorpy-0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1076 2023-05-14 02:14:45.142979 xicorpy-0.2/LICENSE
--rw-r--r--   0        0        0     1479 2023-05-14 02:14:45.142979 xicorpy-0.2/README.md
--rw-r--r--   0        0        0     1562 2023-05-14 02:14:45.142979 xicorpy-0.2/pyproject.toml
--rw-r--r--   0        0        0      256 2023-05-14 02:14:45.142979 xicorpy-0.2/xicorpy/__init__.py
--rw-r--r--   0        0        0     1175 2023-05-14 02:14:45.142979 xicorpy-0.2/xicorpy/_utils.py
--rw-r--r--   0        0        0     8832 2023-05-14 02:14:45.142979 xicorpy-0.2/xicorpy/conditional_dependence.py
--rw-r--r--   0        0        0    12440 2023-05-14 02:14:45.142979 xicorpy-0.2/xicorpy/correlation.py
--rw-r--r--   0        0        0     4324 2023-05-14 02:14:45.142979 xicorpy-0.2/xicorpy/foci.py
--rw-r--r--   0        0        0     2962 1970-01-01 00:00:00.000000 xicorpy-0.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-14 02:50:32.949022 xicorpy-0.3/LICENSE
+-rw-r--r--   0        0        0     1479 2023-05-14 02:50:32.949022 xicorpy-0.3/README.md
+-rw-r--r--   0        0        0     1534 2023-05-14 02:50:32.949022 xicorpy-0.3/pyproject.toml
+-rw-r--r--   0        0        0      256 2023-05-14 02:50:32.949022 xicorpy-0.3/xicorpy/__init__.py
+-rw-r--r--   0        0        0     1175 2023-05-14 02:50:32.949022 xicorpy-0.3/xicorpy/_utils.py
+-rw-r--r--   0        0        0     8832 2023-05-14 02:50:32.949022 xicorpy-0.3/xicorpy/conditional_dependence.py
+-rw-r--r--   0        0        0    12440 2023-05-14 02:50:32.949022 xicorpy-0.3/xicorpy/correlation.py
+-rw-r--r--   0        0        0     4324 2023-05-14 02:50:32.949022 xicorpy-0.3/xicorpy/foci.py
+-rw-r--r--   0        0        0     2967 1970-01-01 00:00:00.000000 xicorpy-0.3/PKG-INFO
```

### Comparing `xicorpy-0.2/LICENSE` & `xicorpy-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xicorpy-0.2/README.md` & `xicorpy-0.3/README.md`

 * *Files identical despite different names*

### Comparing `xicorpy-0.2/pyproject.toml` & `xicorpy-0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xicorpy"
-version = "0.2"
+version = "0.3"
 description = "Python implementation of Chatterjee's Rank Correlation, its modifications, and other offshoots"
 authors = ["Swarna Vallabhaneni <swarnakumar@gmail.com>"]
 maintainers = ["Swarna Vallabhaneni <swarnakumar@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/swarnakumar/xicorpy"
 homepage = "https://swarnakumar.github.io/xicorpy"
@@ -16,29 +16,28 @@
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules"
     ]
 
 
 [tool.poetry.dependencies]
-python = ">=3.7.1,<3.11"
-pandas = "^1.2"
-numpy = "^1.17"
-scipy = "^1.7"
-scikit-learn = "^1.0.2"
-mypy = "0.931"
-mkdocstrings = {version = "~0.17", optional = true}
-mkdocs-material = {version = "~8.1", optional = true}
+python = ">=3.8,<3.12"
+pandas = "^2"
+numpy = "^1.24"
+scikit-learn = "^1.2"
+mypy = "1.2"
+mkdocstrings = {version = "~0.20", optional = true}
+mkdocs-material = {version = "~9.1", optional = true}
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2.5"
-pytest-cov = "^3.0.0"
+pytest = "^7.2"
+pytest-cov = "^4.0.0"
 pre-commit = "^2.16.0"
-coverage = {extras = ["toml"], version = "^6.2"}
-mypy = "^0.931"
+coverage = {extras = ["toml"], version = "^7.2"}
+mypy = "1.2"
 
 [tool.poetry.extras]
 docs = ["mkdocstrings", "mkdocs-material"]
 typings = ["mypy"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `xicorpy-0.2/xicorpy/_utils.py` & `xicorpy-0.3/xicorpy/_utils.py`

 * *Files identical despite different names*

### Comparing `xicorpy-0.2/xicorpy/conditional_dependence.py` & `xicorpy-0.3/xicorpy/conditional_dependence.py`

 * *Files identical despite different names*

### Comparing `xicorpy-0.2/xicorpy/correlation.py` & `xicorpy-0.3/xicorpy/correlation.py`

 * *Files identical despite different names*

### Comparing `xicorpy-0.2/xicorpy/foci.py` & `xicorpy-0.3/xicorpy/foci.py`

 * *Files identical despite different names*

### Comparing `xicorpy-0.2/PKG-INFO` & `xicorpy-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: xicorpy
-Version: 0.2
+Version: 0.3
 Summary: Python implementation of Chatterjee's Rank Correlation, its modifications, and other offshoots
 Home-page: https://swarnakumar.github.io/xicorpy
 License: MIT
 Author: Swarna Vallabhaneni
 Author-email: swarnakumar@gmail.com
 Maintainer: Swarna Vallabhaneni
 Maintainer-email: swarnakumar@gmail.com
-Requires-Python: >=3.7.1,<3.11
+Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: docs
 Provides-Extra: typings
-Requires-Dist: mkdocs-material (>=8.1,<8.2) ; extra == "docs"
-Requires-Dist: mkdocstrings (>=0.17,<0.18) ; extra == "docs"
-Requires-Dist: mypy (==0.931) ; extra == "typings"
-Requires-Dist: numpy (>=1.17,<2.0)
-Requires-Dist: pandas (>=1.2,<2.0)
-Requires-Dist: scikit-learn (>=1.0.2,<2.0.0)
-Requires-Dist: scipy (>=1.7,<2.0)
+Requires-Dist: mkdocs-material (>=9.1,<9.2) ; extra == "docs"
+Requires-Dist: mkdocstrings (>=0.20,<0.21) ; extra == "docs"
+Requires-Dist: mypy (==1.2) ; extra == "typings"
+Requires-Dist: numpy (>=1.24,<2.0)
+Requires-Dist: pandas (>=2,<3)
+Requires-Dist: scikit-learn (>=1.2,<2.0)
 Project-URL: Repository, https://github.com/swarnakumar/xicorpy
 Description-Content-Type: text/markdown
 
 # Chatterjee's Xi, its Applications, and Offshoots
 
 XicorPy is a Python package implementing **Chatterjee's Xi**, and its various offshoots. You can use the package with raw python objects, NumPy arrays, or Pandas DataFrames.
```

