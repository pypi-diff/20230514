# Comparing `tmp/datamultiproc-0.1.1.tar.gz` & `tmp/datamultiproc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamultiproc-0.1.1.tar", max compression
+gzip compressed data, was "datamultiproc-0.1.2.tar", max compression
```

## Comparing `datamultiproc-0.1.1.tar` & `datamultiproc-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,11 @@
--rw-r--r--   0        0        0     1065 2023-05-13 13:52:01.191826 datamultiproc-0.1.1/LICENSE
--rw-r--r--   0        0        0      174 2023-05-13 13:53:41.866068 datamultiproc-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-13 13:52:01.219306 datamultiproc-0.1.1/datamultiproc/__init__.py
--rw-r--r--   0        0        0      361 2023-05-13 13:56:35.293482 datamultiproc-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      706 2023-05-13 13:57:24.164876 datamultiproc-0.1.1/setup.py
--rw-r--r--   0        0        0      600 2023-05-13 13:57:24.164992 datamultiproc-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-13 13:52:01.191826 datamultiproc-0.1.2/LICENSE
+-rw-r--r--   0        0        0      174 2023-05-13 13:53:41.866068 datamultiproc-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-13 13:52:01.219306 datamultiproc-0.1.2/datamultiproc/__init__.py
+-rw-r--r--   0        0        0      232 2023-05-13 14:13:43.961655 datamultiproc-0.1.2/datamultiproc/composer.py
+-rw-r--r--   0        0        0     1908 2023-05-13 14:47:41.097031 datamultiproc-0.1.2/datamultiproc/fileio.py
+-rw-r--r--   0        0        0     1020 2023-05-13 14:52:52.595422 datamultiproc-0.1.2/datamultiproc/processor.py
+-rw-r--r--   0        0        0      712 2023-05-13 14:55:18.750989 datamultiproc-0.1.2/datamultiproc/sample.py
+-rw-r--r--   0        0        0      983 2023-05-13 14:25:27.215286 datamultiproc-0.1.2/datamultiproc/utils.py
+-rw-r--r--   0        0        0      510 2023-05-13 15:06:59.280030 datamultiproc-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      946 2023-05-13 15:07:49.742815 datamultiproc-0.1.2/setup.py
+-rw-r--r--   0        0        0      832 2023-05-13 15:07:49.742938 datamultiproc-0.1.2/PKG-INFO
```

### Comparing `datamultiproc-0.1.1/LICENSE` & `datamultiproc-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datamultiproc-0.1.1/setup.py` & `datamultiproc-0.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,24 +3,31 @@
 
 packages = \
 ['datamultiproc']
 
 package_data = \
 {'': ['*']}
 
+install_requires = \
+['PyYAML>=6.0,<7.0',
+ 'numpy>=1.24.3,<2.0.0',
+ 'pydantic-yaml>=0.11.2,<0.12.0',
+ 'pydantic>=1.10.7,<2.0.0']
+
 setup_kwargs = {
     'name': 'datamultiproc',
-    'version': '0.1.1',
-    'description': '',
+    'version': '0.1.2',
+    'description': 'A Python multiprocessing library for data processing with pipelines.',
     'long_description': "# datamultiproc: A Python multiprocessing data pipeline library\n\nCreate Processors, compose them into pipelines and process your data using Python's \nmultiprocessing library\n",
     'author': 'Magnus Glasder',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/mglasder/datamultiproc',
     'packages': packages,
     'package_data': package_data,
+    'install_requires': install_requires,
     'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

