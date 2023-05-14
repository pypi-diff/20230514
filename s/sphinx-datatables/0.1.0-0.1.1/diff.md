# Comparing `tmp/sphinx-datatables-0.1.0.tar.gz` & `tmp/sphinx-datatables-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-datatables-0.1.0.tar", last modified: Sat May 13 23:21:07 2023, max compression
+gzip compressed data, was "sphinx-datatables-0.1.1.tar", last modified: Sun May 14 00:10:00 2023, max compression
```

## Comparing `sphinx-datatables-0.1.0.tar` & `sphinx-datatables-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 varunsh   (1000) varunsh   (1000)        0 2023-05-13 23:21:07.079064 sphinx-datatables-0.1.0/
--rw-r--r--   0 varunsh   (1000) varunsh   (1000)     1069 2023-05-09 05:32:05.000000 sphinx-datatables-0.1.0/LICENSE
--rw-r--r--   0 varunsh   (1000) varunsh   (1000)       37 2023-05-13 21:50:12.000000 sphinx-datatables-0.1.0/MANIFEST.in
--rw-r--r--   0 varunsh   (1000) varunsh   (1000)     2748 2023-05-13 23:21:07.079064 sphinx-datatables-0.1.0/PKG-INFO
--rw-r--r--   0 varunsh   (1000) varunsh   (1000)      859 2023-05-13 23:20:59.000000 sphinx-datatables-0.1.0/README.rst
--rw-r--r--   0 varunsh   (1000) varunsh   (1000)     1124 2023-05-13 22:59:57.000000 sphinx-datatables-0.1.0/pyproject.toml
--rw-r--r--   0 varunsh   (1000) varunsh   (1000)       38 2023-05-13 23:21:07.079064 sphinx-datatables-0.1.0/setup.cfg
-drwxr-xr-x   0 varunsh   (1000) varunsh   (1000)        0 2023-05-13 23:21:07.079064 sphinx-datatables-0.1.0/src/
-drwxr-xr-x   0 varunsh   (1000) varunsh   (1000)        0 2023-05-13 23:21:07.079064 sphinx-datatables-0.1.0/src/sphinx_datatables/
--rw-r--r--   0 varunsh   (1000) varunsh   (1000)      128 2023-05-09 05:32:05.000000 sphinx-datatables-0.1.0/src/sphinx_datatables/__init__.py
--rw-r--r--   0 varunsh   (1000) varunsh   (1000)      156 2023-05-13 21:24:13.000000 sphinx-datatables-0.1.0/src/sphinx_datatables/activate_datatables.js.in
--rw-r--r--   0 varunsh   (1000) varunsh   (1000)     2250 2023-05-13 22:21:01.000000 sphinx-datatables-0.1.0/src/sphinx_datatables/sphinx_datatables.py
-drwxr-xr-x   0 varunsh   (1000) varunsh   (1000)        0 2023-05-13 23:21:07.079064 sphinx-datatables-0.1.0/src/sphinx_datatables.egg-info/
--rw-r--r--   0 varunsh   (1000) varunsh   (1000)     2748 2023-05-13 23:21:07.000000 sphinx-datatables-0.1.0/src/sphinx_datatables.egg-info/PKG-INFO
--rw-r--r--   0 varunsh   (1000) varunsh   (1000)      394 2023-05-13 23:21:07.000000 sphinx-datatables-0.1.0/src/sphinx_datatables.egg-info/SOURCES.txt
--rw-r--r--   0 varunsh   (1000) varunsh   (1000)        1 2023-05-13 23:21:07.000000 sphinx-datatables-0.1.0/src/sphinx_datatables.egg-info/dependency_links.txt
--rw-r--r--   0 varunsh   (1000) varunsh   (1000)       58 2023-05-13 23:21:07.000000 sphinx-datatables-0.1.0/src/sphinx_datatables.egg-info/requires.txt
--rw-r--r--   0 varunsh   (1000) varunsh   (1000)       18 2023-05-13 23:21:07.000000 sphinx-datatables-0.1.0/src/sphinx_datatables.egg-info/top_level.txt
+drwxr-xr-x   0 varunsh   (1000) varunsh   (1000)        0 2023-05-14 00:10:00.318411 sphinx-datatables-0.1.1/
+-rw-r--r--   0 varunsh   (1000) varunsh   (1000)     1069 2023-05-09 05:32:05.000000 sphinx-datatables-0.1.1/LICENSE
+-rw-r--r--   0 varunsh   (1000) varunsh   (1000)       37 2023-05-13 21:50:12.000000 sphinx-datatables-0.1.1/MANIFEST.in
+-rw-r--r--   0 varunsh   (1000) varunsh   (1000)     2812 2023-05-14 00:10:00.318411 sphinx-datatables-0.1.1/PKG-INFO
+-rw-r--r--   0 varunsh   (1000) varunsh   (1000)      859 2023-05-13 23:34:37.000000 sphinx-datatables-0.1.1/README.rst
+-rw-r--r--   0 varunsh   (1000) varunsh   (1000)     1195 2023-05-13 23:44:43.000000 sphinx-datatables-0.1.1/pyproject.toml
+-rw-r--r--   0 varunsh   (1000) varunsh   (1000)       38 2023-05-14 00:10:00.318411 sphinx-datatables-0.1.1/setup.cfg
+drwxr-xr-x   0 varunsh   (1000) varunsh   (1000)        0 2023-05-14 00:10:00.318411 sphinx-datatables-0.1.1/src/
+drwxr-xr-x   0 varunsh   (1000) varunsh   (1000)        0 2023-05-14 00:10:00.318411 sphinx-datatables-0.1.1/src/sphinx_datatables/
+-rw-r--r--   0 varunsh   (1000) varunsh   (1000)      128 2023-05-14 00:08:33.000000 sphinx-datatables-0.1.1/src/sphinx_datatables/__init__.py
+-rw-r--r--   0 varunsh   (1000) varunsh   (1000)      156 2023-05-13 21:24:13.000000 sphinx-datatables-0.1.1/src/sphinx_datatables/activate_datatables.js.in
+-rw-r--r--   0 varunsh   (1000) varunsh   (1000)     2250 2023-05-13 22:21:01.000000 sphinx-datatables-0.1.1/src/sphinx_datatables/sphinx_datatables.py
+drwxr-xr-x   0 varunsh   (1000) varunsh   (1000)        0 2023-05-14 00:10:00.318411 sphinx-datatables-0.1.1/src/sphinx_datatables.egg-info/
+-rw-r--r--   0 varunsh   (1000) varunsh   (1000)     2812 2023-05-14 00:10:00.000000 sphinx-datatables-0.1.1/src/sphinx_datatables.egg-info/PKG-INFO
+-rw-r--r--   0 varunsh   (1000) varunsh   (1000)      394 2023-05-14 00:10:00.000000 sphinx-datatables-0.1.1/src/sphinx_datatables.egg-info/SOURCES.txt
+-rw-r--r--   0 varunsh   (1000) varunsh   (1000)        1 2023-05-14 00:10:00.000000 sphinx-datatables-0.1.1/src/sphinx_datatables.egg-info/dependency_links.txt
+-rw-r--r--   0 varunsh   (1000) varunsh   (1000)       58 2023-05-14 00:10:00.000000 sphinx-datatables-0.1.1/src/sphinx_datatables.egg-info/requires.txt
+-rw-r--r--   0 varunsh   (1000) varunsh   (1000)       18 2023-05-14 00:10:00.000000 sphinx-datatables-0.1.1/src/sphinx_datatables.egg-info/top_level.txt
```

### Comparing `sphinx-datatables-0.1.0/LICENSE` & `sphinx-datatables-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-datatables-0.1.0/PKG-INFO` & `sphinx-datatables-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: sphinx-datatables
-Version: 0.1.0
+Version: 0.1.1
+Summary: Searchable and sortable tables in Sphinx documentation
 Author-email: Varun Sharma <29899983+sharm294@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2023 Varun Sharma
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -28,15 +29,15 @@
 Project-URL: Documentation, https://sharm294.github.io/sphinx-datatables/
 Keywords: sphinx,table,datatables
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 License-File: LICENSE
 
 ..
     Copyright (c) 2023 Varun Sharma
```

### Comparing `sphinx-datatables-0.1.0/README.rst` & `sphinx-datatables-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx-datatables-0.1.0/pyproject.toml` & `sphinx-datatables-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sphinx-datatables"
 authors = [{name = "Varun Sharma", email = "29899983+sharm294@users.noreply.github.com"}]
 readme = "README.rst"
+description = "Searchable and sortable tables in Sphinx documentation"
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: Sphinx :: Extension",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["sphinx", "table", "datatables"]
 dynamic = ["version"]
-requires-python = ">=3.8"
+requires-python = ">=3.6"
 dependencies = [
     "sphinx>4",
     "sphinxcontrib_jquery>=4.1"
 ]
 
 [tool.setuptools.dynamic]
 version = {attr = "sphinx_datatables.__version__"}
```

### Comparing `sphinx-datatables-0.1.0/src/sphinx_datatables/sphinx_datatables.py` & `sphinx-datatables-0.1.1/src/sphinx_datatables/sphinx_datatables.py`

 * *Files identical despite different names*

### Comparing `sphinx-datatables-0.1.0/src/sphinx_datatables.egg-info/PKG-INFO` & `sphinx-datatables-0.1.1/src/sphinx_datatables.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: sphinx-datatables
-Version: 0.1.0
+Version: 0.1.1
+Summary: Searchable and sortable tables in Sphinx documentation
 Author-email: Varun Sharma <29899983+sharm294@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2023 Varun Sharma
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -28,15 +29,15 @@
 Project-URL: Documentation, https://sharm294.github.io/sphinx-datatables/
 Keywords: sphinx,table,datatables
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 License-File: LICENSE
 
 ..
     Copyright (c) 2023 Varun Sharma
```

