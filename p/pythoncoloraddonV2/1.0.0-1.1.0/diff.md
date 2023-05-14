# Comparing `tmp/pythoncoloraddonV2-1.0.0.tar.gz` & `tmp/pythoncoloraddonV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythoncoloraddonV2-1.0.0.tar", last modified: Sun May 14 15:21:56 2023, max compression
+gzip compressed data, was "pythoncoloraddonV2-1.1.0.tar", last modified: Sun May 14 15:24:01 2023, max compression
```

## Comparing `pythoncoloraddonV2-1.0.0.tar` & `pythoncoloraddonV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 15:21:56.105399 pythoncoloraddonV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      351 2023-05-14 15:21:56.105399 pythoncoloraddonV2-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 15:21:56.105399 pythoncoloraddonV2-1.0.0/pythoncoloraddonV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-14 15:21:55.000000 pythoncoloraddonV2-1.0.0/pythoncoloraddonV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 15:21:56.105399 pythoncoloraddonV2-1.0.0/pythoncoloraddonV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      351 2023-05-14 15:21:56.000000 pythoncoloraddonV2-1.0.0/pythoncoloraddonV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      207 2023-05-14 15:21:56.000000 pythoncoloraddonV2-1.0.0/pythoncoloraddonV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 15:21:56.000000 pythoncoloraddonV2-1.0.0/pythoncoloraddonV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-14 15:21:56.000000 pythoncoloraddonV2-1.0.0/pythoncoloraddonV2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 15:21:56.105399 pythoncoloraddonV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      564 2023-05-14 15:21:55.000000 pythoncoloraddonV2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 15:24:01.535918 pythoncoloraddonV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-05-14 15:24:01.535918 pythoncoloraddonV2-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 15:24:01.535918 pythoncoloraddonV2-1.1.0/pythoncoloraddonV2/
+-rw-r--r--   0 root         (0) root         (0)    96635 2023-05-14 15:24:01.000000 pythoncoloraddonV2-1.1.0/pythoncoloraddonV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 15:24:01.535918 pythoncoloraddonV2-1.1.0/pythoncoloraddonV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-05-14 15:24:01.000000 pythoncoloraddonV2-1.1.0/pythoncoloraddonV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      207 2023-05-14 15:24:01.000000 pythoncoloraddonV2-1.1.0/pythoncoloraddonV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 15:24:01.000000 pythoncoloraddonV2-1.1.0/pythoncoloraddonV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-14 15:24:01.000000 pythoncoloraddonV2-1.1.0/pythoncoloraddonV2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 15:24:01.535918 pythoncoloraddonV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      564 2023-05-14 15:24:01.000000 pythoncoloraddonV2-1.1.0/setup.py
```

### Comparing `pythoncoloraddonV2-1.0.0/setup.py` & `pythoncoloraddonV2-1.1.0/setup.py`

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
     name="pythoncoloraddonV2",
     version=VERSION,
```

