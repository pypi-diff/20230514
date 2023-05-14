# Comparing `tmp/pythonsqladdonV2-1.0.0.tar.gz` & `tmp/pythonsqladdonV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonsqladdonV2-1.0.0.tar", last modified: Sun May 14 12:50:11 2023, max compression
+gzip compressed data, was "pythonsqladdonV2-1.1.0.tar", last modified: Sun May 14 12:52:16 2023, max compression
```

## Comparing `pythonsqladdonV2-1.0.0.tar` & `pythonsqladdonV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 12:50:11.488813 pythonsqladdonV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      349 2023-05-14 12:50:11.488813 pythonsqladdonV2-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 12:50:11.488813 pythonsqladdonV2-1.0.0/pythonsqladdonV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-14 12:50:11.000000 pythonsqladdonV2-1.0.0/pythonsqladdonV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 12:50:11.488813 pythonsqladdonV2-1.0.0/pythonsqladdonV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      349 2023-05-14 12:50:11.000000 pythonsqladdonV2-1.0.0/pythonsqladdonV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      197 2023-05-14 12:50:11.000000 pythonsqladdonV2-1.0.0/pythonsqladdonV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 12:50:11.000000 pythonsqladdonV2-1.0.0/pythonsqladdonV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-14 12:50:11.000000 pythonsqladdonV2-1.0.0/pythonsqladdonV2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 12:50:11.488813 pythonsqladdonV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      562 2023-05-14 12:50:11.000000 pythonsqladdonV2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 12:52:16.743470 pythonsqladdonV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-05-14 12:52:16.743470 pythonsqladdonV2-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 12:52:16.743470 pythonsqladdonV2-1.1.0/pythonsqladdonV2/
+-rw-r--r--   0 root         (0) root         (0)    96635 2023-05-14 12:52:16.000000 pythonsqladdonV2-1.1.0/pythonsqladdonV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 12:52:16.743470 pythonsqladdonV2-1.1.0/pythonsqladdonV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-05-14 12:52:16.000000 pythonsqladdonV2-1.1.0/pythonsqladdonV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      197 2023-05-14 12:52:16.000000 pythonsqladdonV2-1.1.0/pythonsqladdonV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 12:52:16.000000 pythonsqladdonV2-1.1.0/pythonsqladdonV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-14 12:52:16.000000 pythonsqladdonV2-1.1.0/pythonsqladdonV2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 12:52:16.743470 pythonsqladdonV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      562 2023-05-14 12:52:16.000000 pythonsqladdonV2-1.1.0/setup.py
```

### Comparing `pythonsqladdonV2-1.0.0/setup.py` & `pythonsqladdonV2-1.1.0/setup.py`

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
     name="pythonsqladdonV2",
     version=VERSION,
```

