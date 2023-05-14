# Comparing `tmp/pythonsqlitedbmodules-1.0.0.tar.gz` & `tmp/pythonsqlitedbmodules-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonsqlitedbmodules-1.0.0.tar", last modified: Sun May 14 13:21:47 2023, max compression
+gzip compressed data, was "pythonsqlitedbmodules-1.1.0.tar", last modified: Sun May 14 13:23:53 2023, max compression
```

## Comparing `pythonsqlitedbmodules-1.0.0.tar` & `pythonsqlitedbmodules-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 13:21:47.464005 pythonsqlitedbmodules-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      354 2023-05-14 13:21:47.464005 pythonsqlitedbmodules-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 13:21:47.464005 pythonsqlitedbmodules-1.0.0/pythonsqlitedbmodules/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-14 13:21:47.000000 pythonsqlitedbmodules-1.0.0/pythonsqlitedbmodules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 13:21:47.464005 pythonsqlitedbmodules-1.0.0/pythonsqlitedbmodules.egg-info/
--rw-r--r--   0 root         (0) root         (0)      354 2023-05-14 13:21:47.000000 pythonsqlitedbmodules-1.0.0/pythonsqlitedbmodules.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      222 2023-05-14 13:21:47.000000 pythonsqlitedbmodules-1.0.0/pythonsqlitedbmodules.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 13:21:47.000000 pythonsqlitedbmodules-1.0.0/pythonsqlitedbmodules.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-14 13:21:47.000000 pythonsqlitedbmodules-1.0.0/pythonsqlitedbmodules.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 13:21:47.464005 pythonsqlitedbmodules-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      567 2023-05-14 13:21:47.000000 pythonsqlitedbmodules-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 13:23:53.486627 pythonsqlitedbmodules-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      354 2023-05-14 13:23:53.486627 pythonsqlitedbmodules-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 13:23:53.486627 pythonsqlitedbmodules-1.1.0/pythonsqlitedbmodules/
+-rw-r--r--   0 root         (0) root         (0)    96635 2023-05-14 13:23:53.000000 pythonsqlitedbmodules-1.1.0/pythonsqlitedbmodules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 13:23:53.486627 pythonsqlitedbmodules-1.1.0/pythonsqlitedbmodules.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      354 2023-05-14 13:23:53.000000 pythonsqlitedbmodules-1.1.0/pythonsqlitedbmodules.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      222 2023-05-14 13:23:53.000000 pythonsqlitedbmodules-1.1.0/pythonsqlitedbmodules.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 13:23:53.000000 pythonsqlitedbmodules-1.1.0/pythonsqlitedbmodules.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-14 13:23:53.000000 pythonsqlitedbmodules-1.1.0/pythonsqlitedbmodules.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 13:23:53.486627 pythonsqlitedbmodules-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      567 2023-05-14 13:23:53.000000 pythonsqlitedbmodules-1.1.0/setup.py
```

### Comparing `pythonsqlitedbmodules-1.0.0/setup.py` & `pythonsqlitedbmodules-1.1.0/setup.py`

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
     name="pythonsqlitedbmodules",
     version=VERSION,
```

