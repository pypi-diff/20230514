# Comparing `tmp/sysfontinglibV2-1.0.0.tar.gz` & `tmp/sysfontinglibV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysfontinglibV2-1.0.0.tar", last modified: Sun May 14 18:47:10 2023, max compression
+gzip compressed data, was "sysfontinglibV2-1.1.0.tar", last modified: Sun May 14 18:49:16 2023, max compression
```

## Comparing `sysfontinglibV2-1.0.0.tar` & `sysfontinglibV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:47:10.918741 sysfontinglibV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      348 2023-05-14 18:47:10.918741 sysfontinglibV2-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 18:47:10.918741 sysfontinglibV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      561 2023-05-14 18:47:10.000000 sysfontinglibV2-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:47:10.918741 sysfontinglibV2-1.0.0/sysfontinglibV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-14 18:47:10.000000 sysfontinglibV2-1.0.0/sysfontinglibV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:47:10.918741 sysfontinglibV2-1.0.0/sysfontinglibV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      348 2023-05-14 18:47:10.000000 sysfontinglibV2-1.0.0/sysfontinglibV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      192 2023-05-14 18:47:10.000000 sysfontinglibV2-1.0.0/sysfontinglibV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 18:47:10.000000 sysfontinglibV2-1.0.0/sysfontinglibV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-14 18:47:10.000000 sysfontinglibV2-1.0.0/sysfontinglibV2.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:49:16.317399 sysfontinglibV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      348 2023-05-14 18:49:16.317399 sysfontinglibV2-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 18:49:16.317399 sysfontinglibV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      561 2023-05-14 18:49:16.000000 sysfontinglibV2-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:49:16.317399 sysfontinglibV2-1.1.0/sysfontinglibV2/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-05-14 18:49:16.000000 sysfontinglibV2-1.1.0/sysfontinglibV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 18:49:16.317399 sysfontinglibV2-1.1.0/sysfontinglibV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      348 2023-05-14 18:49:16.000000 sysfontinglibV2-1.1.0/sysfontinglibV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      192 2023-05-14 18:49:16.000000 sysfontinglibV2-1.1.0/sysfontinglibV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 18:49:16.000000 sysfontinglibV2-1.1.0/sysfontinglibV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-14 18:49:16.000000 sysfontinglibV2-1.1.0/sysfontinglibV2.egg-info/top_level.txt
```

### Comparing `sysfontinglibV2-1.0.0/setup.py` & `sysfontinglibV2-1.1.0/setup.py`

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
     name="sysfontinglibV2",
     version=VERSION,
```

