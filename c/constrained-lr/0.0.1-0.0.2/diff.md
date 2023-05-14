# Comparing `tmp/constrained-lr-0.0.1.tar.gz` & `tmp/constrained_lr-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "constrained-lr-0.0.1.tar", last modified: Sat May 13 18:43:08 2023, max compression
+gzip compressed data, was "constrained_lr-0.0.2.tar", last modified: Sun May 14 19:16:38 2023, max compression
```

## Comparing `constrained-lr-0.0.1.tar` & `constrained_lr-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-13 18:43:09.245447 constrained-lr-0.0.1/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1089 2023-04-29 16:41:09.000000 constrained-lr-0.0.1/LICENCE
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)      979 2023-05-13 18:43:09.238439 constrained-lr-0.0.1/PKG-INFO
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-13 18:43:09.143443 constrained-lr-0.0.1/constrained_lr.egg-info/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)      979 2023-05-13 18:43:08.000000 constrained-lr-0.0.1/constrained_lr.egg-info/PKG-INFO
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)      229 2023-05-13 18:43:08.000000 constrained-lr-0.0.1/constrained_lr.egg-info/SOURCES.txt
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        1 2023-05-13 18:43:08.000000 constrained-lr-0.0.1/constrained_lr.egg-info/dependency_links.txt
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       48 2023-05-13 18:43:08.000000 constrained-lr-0.0.1/constrained_lr.egg-info/requires.txt
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       15 2023-05-13 18:43:08.000000 constrained-lr-0.0.1/constrained_lr.egg-info/top_level.txt
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1294 2023-05-13 18:42:21.000000 constrained-lr-0.0.1/pyproject.toml
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       38 2023-05-13 18:43:09.248439 constrained-lr-0.0.1/setup.cfg
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-13 18:43:09.192454 constrained-lr-0.0.1/tests/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2762 2023-05-13 18:42:44.000000 constrained-lr-0.0.1/tests/test_fit.py
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-14 19:16:38.776689 constrained_lr-0.0.2/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1089 2023-04-29 16:41:09.000000 constrained_lr-0.0.2/LICENCE
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2011 2023-05-14 19:16:38.769925 constrained_lr-0.0.2/PKG-INFO
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1020 2023-05-14 13:41:44.000000 constrained_lr-0.0.2/README.md
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-14 19:16:38.672693 constrained_lr-0.0.2/constrained_lr.egg-info/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2011 2023-05-14 19:16:38.000000 constrained_lr-0.0.2/constrained_lr.egg-info/PKG-INFO
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)      239 2023-05-14 19:16:38.000000 constrained_lr-0.0.2/constrained_lr.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        1 2023-05-14 19:16:38.000000 constrained_lr-0.0.2/constrained_lr.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       48 2023-05-14 19:16:38.000000 constrained_lr-0.0.2/constrained_lr.egg-info/requires.txt
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       15 2023-05-14 19:16:38.000000 constrained_lr-0.0.2/constrained_lr.egg-info/top_level.txt
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1305 2023-05-14 19:16:19.000000 constrained_lr-0.0.2/pyproject.toml
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       38 2023-05-14 19:16:38.786714 constrained_lr-0.0.2/setup.cfg
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-14 19:16:38.710688 constrained_lr-0.0.2/tests/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2762 2023-05-13 18:42:44.000000 constrained_lr-0.0.2/tests/test_fit.py
```

### Comparing `constrained-lr-0.0.1/LICENCE` & `constrained_lr-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `constrained-lr-0.0.1/pyproject.toml` & `constrained_lr-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
-name = 'constrained-lr'
-version = '0.0.1'
+name = 'constrained_lr'
+version = '0.0.2'
 description = 'Constrained Linear Regression with sklearn-compatible API'
 readme = 'README.md'
 authors = [
   { name = 'Theodore Tsitsimis', email='th.tsitsimis@gmail.com' },
 ]
 license = {file = 'LICENSE'}
 requires-python = '>=3.8'
@@ -30,15 +30,15 @@
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'Topic :: Software Development :: Libraries',
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/tsitsimis/clr"
+"Homepage" = "https://github.com/tsitsimis/constrained_lr"
 
 [tool.setuptools]
 py-modules = ["constrained_lr"]
 
 [tool.black]
 line-length = 120
 target-version = ['py37', 'py38', 'py39']
```

### Comparing `constrained-lr-0.0.1/tests/test_fit.py` & `constrained_lr-0.0.2/tests/test_fit.py`

 * *Files identical despite different names*

