# Comparing `tmp/pythoncoloringaddonsV2-1.0.0.tar.gz` & `tmp/pythoncoloringaddonsV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythoncoloringaddonsV2-1.0.0.tar", last modified: Sun May 14 18:17:11 2023, max compression
+gzip compressed data, was "pythoncoloringaddonsV2-1.1.0.tar", last modified: Sun May 14 18:19:18 2023, max compression
```

## Comparing `pythoncoloringaddonsV2-1.0.0.tar` & `pythoncoloringaddonsV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:17:11.973870 pythoncoloringaddonsV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      355 2023-05-14 18:17:11.973870 pythoncoloringaddonsV2-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:17:11.973870 pythoncoloringaddonsV2-1.0.0/pythoncoloringaddonsV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-14 18:17:11.000000 pythoncoloringaddonsV2-1.0.0/pythoncoloringaddonsV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:17:11.973870 pythoncoloringaddonsV2-1.0.0/pythoncoloringaddonsV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      355 2023-05-14 18:17:11.000000 pythoncoloringaddonsV2-1.0.0/pythoncoloringaddonsV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-05-14 18:17:11.000000 pythoncoloringaddonsV2-1.0.0/pythoncoloringaddonsV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 18:17:11.000000 pythoncoloringaddonsV2-1.0.0/pythoncoloringaddonsV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-14 18:17:11.000000 pythoncoloringaddonsV2-1.0.0/pythoncoloringaddonsV2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 18:17:11.973870 pythoncoloringaddonsV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      568 2023-05-14 18:17:11.000000 pythoncoloringaddonsV2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:19:18.168514 pythoncoloringaddonsV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      355 2023-05-14 18:19:18.168514 pythoncoloringaddonsV2-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:19:18.164514 pythoncoloringaddonsV2-1.1.0/pythoncoloringaddonsV2/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-05-14 18:19:17.000000 pythoncoloringaddonsV2-1.1.0/pythoncoloringaddonsV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:19:18.164514 pythoncoloringaddonsV2-1.1.0/pythoncoloringaddonsV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      355 2023-05-14 18:19:18.000000 pythoncoloringaddonsV2-1.1.0/pythoncoloringaddonsV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2023-05-14 18:19:18.000000 pythoncoloringaddonsV2-1.1.0/pythoncoloringaddonsV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 18:19:18.000000 pythoncoloringaddonsV2-1.1.0/pythoncoloringaddonsV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-14 18:19:18.000000 pythoncoloringaddonsV2-1.1.0/pythoncoloringaddonsV2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 18:19:18.168514 pythoncoloringaddonsV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      568 2023-05-14 18:19:17.000000 pythoncoloringaddonsV2-1.1.0/setup.py
```

### Comparing `pythoncoloringaddonsV2-1.0.0/setup.py` & `pythoncoloringaddonsV2-1.1.0/setup.py`

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
     name="pythoncoloringaddonsV2",
     version=VERSION,
```

