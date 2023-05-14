# Comparing `tmp/pipsqlitelib-1.0.0.tar.gz` & `tmp/pipsqlitelib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipsqlitelib-1.0.0.tar", last modified: Sun May 14 18:29:42 2023, max compression
+gzip compressed data, was "pipsqlitelib-1.1.0.tar", last modified: Sun May 14 18:31:47 2023, max compression
```

## Comparing `pipsqlitelib-1.0.0.tar` & `pipsqlitelib-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:29:42.041866 pipsqlitelib-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      345 2023-05-14 18:29:42.041866 pipsqlitelib-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:29:42.041866 pipsqlitelib-1.0.0/pipsqlitelib/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-14 18:29:41.000000 pipsqlitelib-1.0.0/pipsqlitelib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:29:42.041866 pipsqlitelib-1.0.0/pipsqlitelib.egg-info/
--rw-r--r--   0 root         (0) root         (0)      345 2023-05-14 18:29:41.000000 pipsqlitelib-1.0.0/pipsqlitelib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      177 2023-05-14 18:29:42.000000 pipsqlitelib-1.0.0/pipsqlitelib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 18:29:41.000000 pipsqlitelib-1.0.0/pipsqlitelib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-14 18:29:41.000000 pipsqlitelib-1.0.0/pipsqlitelib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 18:29:42.041866 pipsqlitelib-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      558 2023-05-14 18:29:41.000000 pipsqlitelib-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:31:47.504535 pipsqlitelib-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      345 2023-05-14 18:31:47.504535 pipsqlitelib-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:31:47.504535 pipsqlitelib-1.1.0/pipsqlitelib/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-05-14 18:31:47.000000 pipsqlitelib-1.1.0/pipsqlitelib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:31:47.504535 pipsqlitelib-1.1.0/pipsqlitelib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      345 2023-05-14 18:31:47.000000 pipsqlitelib-1.1.0/pipsqlitelib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      177 2023-05-14 18:31:47.000000 pipsqlitelib-1.1.0/pipsqlitelib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 18:31:47.000000 pipsqlitelib-1.1.0/pipsqlitelib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-14 18:31:47.000000 pipsqlitelib-1.1.0/pipsqlitelib.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 18:31:47.504535 pipsqlitelib-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      558 2023-05-14 18:31:47.000000 pipsqlitelib-1.1.0/setup.py
```

### Comparing `pipsqlitelib-1.0.0/setup.py` & `pipsqlitelib-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pipsqlitelib",
     version=VERSION,
```

