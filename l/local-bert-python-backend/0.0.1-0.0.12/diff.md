# Comparing `tmp/local-bert-python-backend-0.0.1.tar.gz` & `tmp/local-bert-python-backend-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local-bert-python-backend-0.0.1.tar", last modified: Thu Apr 27 18:04:42 2023, max compression
+gzip compressed data, was "local-bert-python-backend-0.0.12.tar", last modified: Sun May 14 09:12:25 2023, max compression
```

## Comparing `local-bert-python-backend-0.0.1.tar` & `local-bert-python-backend-0.0.12.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:04:42.354107 local-bert-python-backend-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-27 18:04:42.354107 local-bert-python-backend-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-27 18:04:31.000000 local-bert-python-backend-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:04:42.354107 local-bert-python-backend-0.0.1/local_bert_python_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-27 18:04:42.000000 local-bert-python-backend-0.0.1/local_bert_python_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-27 18:04:42.000000 local-bert-python-backend-0.0.1/local_bert_python_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 18:04:42.000000 local-bert-python-backend-0.0.1/local_bert_python_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 18:04:42.000000 local-bert-python-backend-0.0.1/local_bert_python_backend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 18:04:42.354107 local-bert-python-backend-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-27 18:04:31.000000 local-bert-python-backend-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:12:25.169283 local-bert-python-backend-0.0.12/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-14 09:12:25.169283 local-bert-python-backend-0.0.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-14 09:12:14.000000 local-bert-python-backend-0.0.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:12:25.169283 local-bert-python-backend-0.0.12/local_bert_python_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-14 09:12:25.000000 local-bert-python-backend-0.0.12/local_bert_python_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-14 09:12:25.000000 local-bert-python-backend-0.0.12/local_bert_python_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 09:12:25.000000 local-bert-python-backend-0.0.12/local_bert_python_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 09:12:25.000000 local-bert-python-backend-0.0.12/local_bert_python_backend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-14 09:12:14.000000 local-bert-python-backend-0.0.12/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 09:12:25.169283 local-bert-python-backend-0.0.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-14 09:12:14.000000 local-bert-python-backend-0.0.12/setup.py
```

### Comparing `local-bert-python-backend-0.0.1/setup.py` & `local-bert-python-backend-0.0.12/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 setuptools.setup(
-     name='local-bert-python-backend',  
-     version='0.0.1',
+     name='local-bert-python-backend',
+     version='0.0.12',
      author="Circles",
-     author_email="info@bubbelz.life",
-     description="PyPI Package for Circles Local Bert Python",
+     author_email="info@circles.life",
+     description="PyPI Package for Circles Local recruitment scrapers Python",
      long_description="This is a package for sharing common Logger function used in different repositories",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
      classifiers=[
          "Programming Language :: Python :: 3",
          "License :: Other/Proprietary License",
          "Operating System :: OS Independent",
      ],
- )
+ )
```

