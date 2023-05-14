# Comparing `tmp/hyped-0.0.1.tar.gz` & `tmp/hyped-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyped-0.0.1.tar", last modified: Sun May 14 15:07:14 2023, max compression
+gzip compressed data, was "hyped-0.0.2.tar", last modified: Sun May 14 16:34:49 2023, max compression
```

## Comparing `hyped-0.0.1.tar` & `hyped-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:07:14.362477 hyped-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 15:07:05.000000 hyped-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-14 15:07:14.362477 hyped-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-14 15:07:05.000000 hyped-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:07:14.362477 hyped-0.0.1/hyped/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-14 15:07:05.000000 hyped-0.0.1/hyped/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:07:14.362477 hyped-0.0.1/hyped.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-14 15:07:14.000000 hyped-0.0.1/hyped.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-14 15:07:14.000000 hyped-0.0.1/hyped.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 15:07:14.000000 hyped-0.0.1/hyped.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-14 15:07:14.000000 hyped-0.0.1/hyped.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 15:07:14.000000 hyped-0.0.1/hyped.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 15:07:14.362477 hyped-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 15:07:05.000000 hyped-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:34:49.418187 hyped-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 16:34:40.000000 hyped-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-14 16:34:49.418187 hyped-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-14 16:34:40.000000 hyped-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:34:49.418187 hyped-0.0.2/hyped/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-14 16:34:40.000000 hyped-0.0.2/hyped/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:34:49.418187 hyped-0.0.2/hyped.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-14 16:34:49.000000 hyped-0.0.2/hyped.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-14 16:34:49.000000 hyped-0.0.2/hyped.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 16:34:49.000000 hyped-0.0.2/hyped.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-14 16:34:49.000000 hyped-0.0.2/hyped.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 16:34:49.000000 hyped-0.0.2/hyped.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 16:34:49.418187 hyped-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 16:34:40.000000 hyped-0.0.2/setup.py
```

### Comparing `hyped-0.0.1/LICENSE` & `hyped-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hyped-0.0.1/setup.py` & `hyped-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name="hyped",
-    version="0.0.1",
+    version="0.0.2",
     description="A collection of data pipelines to ease the training of transformer models",
     long_description=open("README.md", "r").read(),
     long_description_content_type='text/markdown',
     author="Niclas Doll",
     author_email="niclas@amazonis.net",
     url="https://github.com/ndoll1998/hyped/tree/master",
     packages=['hyped'],
```

