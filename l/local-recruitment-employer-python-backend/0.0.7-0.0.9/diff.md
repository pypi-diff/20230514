# Comparing `tmp/local-recruitment-employer-python-backend-0.0.7.tar.gz` & `tmp/local-recruitment-employer-python-backend-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local-recruitment-employer-python-backend-0.0.7.tar", last modified: Sat May 13 17:27:33 2023, max compression
+gzip compressed data, was "local-recruitment-employer-python-backend-0.0.9.tar", last modified: Sun May 14 07:28:19 2023, max compression
```

## Comparing `local-recruitment-employer-python-backend-0.0.7.tar` & `local-recruitment-employer-python-backend-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:27:33.019263 local-recruitment-employer-python-backend-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-13 17:27:33.019263 local-recruitment-employer-python-backend-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-13 17:27:19.000000 local-recruitment-employer-python-backend-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:27:33.019263 local-recruitment-employer-python-backend-0.0.7/local_recruitment_employer_python_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-13 17:27:33.000000 local-recruitment-employer-python-backend-0.0.7/local_recruitment_employer_python_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-13 17:27:33.000000 local-recruitment-employer-python-backend-0.0.7/local_recruitment_employer_python_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 17:27:33.000000 local-recruitment-employer-python-backend-0.0.7/local_recruitment_employer_python_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 17:27:33.000000 local-recruitment-employer-python-backend-0.0.7/local_recruitment_employer_python_backend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-13 17:27:19.000000 local-recruitment-employer-python-backend-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 17:27:33.019263 local-recruitment-employer-python-backend-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:28:19.506249 local-recruitment-employer-python-backend-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-14 07:28:19.506249 local-recruitment-employer-python-backend-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-14 07:28:08.000000 local-recruitment-employer-python-backend-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:28:19.506249 local-recruitment-employer-python-backend-0.0.9/local_recruitment_employer_python_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-14 07:28:19.000000 local-recruitment-employer-python-backend-0.0.9/local_recruitment_employer_python_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-14 07:28:19.000000 local-recruitment-employer-python-backend-0.0.9/local_recruitment_employer_python_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 07:28:19.000000 local-recruitment-employer-python-backend-0.0.9/local_recruitment_employer_python_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 07:28:19.000000 local-recruitment-employer-python-backend-0.0.9/local_recruitment_employer_python_backend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-14 07:28:08.000000 local-recruitment-employer-python-backend-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 07:28:19.506249 local-recruitment-employer-python-backend-0.0.9/setup.cfg
```

### Comparing `local-recruitment-employer-python-backend-0.0.7/pyproject.toml` & `local-recruitment-employer-python-backend-0.0.9/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "local-recruitment-employer-python-backend"
-version = "0.0.7"
+version = "0.0.9"
 authors = [
   { name="circles-zone" , email="info@circles.zone"},
 ]
 description = "local-recruitment-employer-python-backend"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 [tool.setuptools]
-py-modules = []
+py-modules = []
```

