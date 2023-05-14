# Comparing `tmp/pythonsqlitedbextV1-1.0.0.tar.gz` & `tmp/pythonsqlitedbextV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonsqlitedbextV1-1.0.0.tar", last modified: Sun May 14 14:59:24 2023, max compression
+gzip compressed data, was "pythonsqlitedbextV1-1.1.0.tar", last modified: Sun May 14 15:01:30 2023, max compression
```

## Comparing `pythonsqlitedbextV1-1.0.0.tar` & `pythonsqlitedbextV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 14:59:24.223729 pythonsqlitedbextV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      352 2023-05-14 14:59:24.223729 pythonsqlitedbextV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 14:59:24.223729 pythonsqlitedbextV1-1.0.0/pythonsqlitedbextV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-14 14:59:24.000000 pythonsqlitedbextV1-1.0.0/pythonsqlitedbextV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 14:59:24.223729 pythonsqlitedbextV1-1.0.0/pythonsqlitedbextV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      352 2023-05-14 14:59:24.000000 pythonsqlitedbextV1-1.0.0/pythonsqlitedbextV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      212 2023-05-14 14:59:24.000000 pythonsqlitedbextV1-1.0.0/pythonsqlitedbextV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 14:59:24.000000 pythonsqlitedbextV1-1.0.0/pythonsqlitedbextV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-14 14:59:24.000000 pythonsqlitedbextV1-1.0.0/pythonsqlitedbextV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 14:59:24.223729 pythonsqlitedbextV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      565 2023-05-14 14:59:24.000000 pythonsqlitedbextV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 15:01:30.026426 pythonsqlitedbextV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      352 2023-05-14 15:01:30.026426 pythonsqlitedbextV1-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 15:01:30.026426 pythonsqlitedbextV1-1.1.0/pythonsqlitedbextV1/
+-rw-r--r--   0 root         (0) root         (0)    96635 2023-05-14 15:01:29.000000 pythonsqlitedbextV1-1.1.0/pythonsqlitedbextV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 15:01:30.026426 pythonsqlitedbextV1-1.1.0/pythonsqlitedbextV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      352 2023-05-14 15:01:29.000000 pythonsqlitedbextV1-1.1.0/pythonsqlitedbextV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      212 2023-05-14 15:01:30.000000 pythonsqlitedbextV1-1.1.0/pythonsqlitedbextV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 15:01:29.000000 pythonsqlitedbextV1-1.1.0/pythonsqlitedbextV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-14 15:01:29.000000 pythonsqlitedbextV1-1.1.0/pythonsqlitedbextV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 15:01:30.026426 pythonsqlitedbextV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      565 2023-05-14 15:01:29.000000 pythonsqlitedbextV1-1.1.0/setup.py
```

### Comparing `pythonsqlitedbextV1-1.0.0/setup.py` & `pythonsqlitedbextV1-1.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pythonsqlitedbextV1",
     version=VERSION,
```

