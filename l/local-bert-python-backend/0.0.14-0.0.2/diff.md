# Comparing `tmp/local-bert-python-backend-0.0.14.tar.gz` & `tmp/local-bert-python-backend-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local-bert-python-backend-0.0.14.tar", last modified: Sun May 14 14:11:27 2023, max compression
+gzip compressed data, was "local-bert-python-backend-0.0.2.tar", last modified: Sun May 14 13:56:23 2023, max compression
```

## Comparing `local-bert-python-backend-0.0.14.tar` & `local-bert-python-backend-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:11:27.527026 local-bert-python-backend-0.0.14/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:11:27.527026 local-bert-python-backend-0.0.14/CirclesBertPython/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:11:16.000000 local-bert-python-backend-0.0.14/CirclesBertPython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-14 14:11:16.000000 local-bert-python-backend-0.0.14/CirclesBertPython/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-14 14:11:16.000000 local-bert-python-backend-0.0.14/CirclesBertPython/test_bert.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-14 14:11:27.527026 local-bert-python-backend-0.0.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-14 14:11:16.000000 local-bert-python-backend-0.0.14/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:11:27.527026 local-bert-python-backend-0.0.14/local_bert_python_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-14 14:11:27.000000 local-bert-python-backend-0.0.14/local_bert_python_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-14 14:11:27.000000 local-bert-python-backend-0.0.14/local_bert_python_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 14:11:27.000000 local-bert-python-backend-0.0.14/local_bert_python_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-14 14:11:27.000000 local-bert-python-backend-0.0.14/local_bert_python_backend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 14:11:27.527026 local-bert-python-backend-0.0.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-14 14:11:16.000000 local-bert-python-backend-0.0.14/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 13:56:23.786797 local-bert-python-backend-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-14 13:56:23.786797 local-bert-python-backend-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-14 13:56:12.000000 local-bert-python-backend-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 13:56:23.782796 local-bert-python-backend-0.0.2/local_bert_python_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-14 13:56:23.000000 local-bert-python-backend-0.0.2/local_bert_python_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-14 13:56:23.000000 local-bert-python-backend-0.0.2/local_bert_python_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 13:56:23.000000 local-bert-python-backend-0.0.2/local_bert_python_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-14 13:56:23.000000 local-bert-python-backend-0.0.2/local_bert_python_backend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 13:56:23.786797 local-bert-python-backend-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-14 13:56:12.000000 local-bert-python-backend-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 13:56:23.782796 local-bert-python-backend-0.0.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 13:56:12.000000 local-bert-python-backend-0.0.2/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-14 13:56:12.000000 local-bert-python-backend-0.0.2/src/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-14 13:56:12.000000 local-bert-python-backend-0.0.2/src/test_bert.py
```

### Comparing `local-bert-python-backend-0.0.14/CirclesBertPython/bert.py` & `local-bert-python-backend-0.0.2/src/bert.py`

 * *Files identical despite different names*

### Comparing `local-bert-python-backend-0.0.14/CirclesBertPython/test_bert.py` & `local-bert-python-backend-0.0.2/src/test_bert.py`

 * *Files identical despite different names*

### Comparing `local-bert-python-backend-0.0.14/setup.py` & `local-bert-python-backend-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
      name='local-bert-python-backend',  
-     version='0.0.14',
+     version='0.0.2',
      author="Circles",
      author_email="info@bubbelz.life",
      description="PyPI Package for Circles Local Bert Python",
      long_description="This is a package for sharing common Logger function used in different repositories",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

