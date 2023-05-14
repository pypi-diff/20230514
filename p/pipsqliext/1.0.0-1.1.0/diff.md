# Comparing `tmp/pipsqliext-1.0.0.tar.gz` & `tmp/pipsqliext-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipsqliext-1.0.0.tar", last modified: Sun May 14 16:19:28 2023, max compression
+gzip compressed data, was "pipsqliext-1.1.0.tar", last modified: Sun May 14 16:21:33 2023, max compression
```

## Comparing `pipsqliext-1.0.0.tar` & `pipsqliext-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 16:19:28.413410 pipsqliext-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      343 2023-05-14 16:19:28.409410 pipsqliext-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 16:19:28.409410 pipsqliext-1.0.0/pipsqliext/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-14 16:19:28.000000 pipsqliext-1.0.0/pipsqliext/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 16:19:28.409410 pipsqliext-1.0.0/pipsqliext.egg-info/
--rw-r--r--   0 root         (0) root         (0)      343 2023-05-14 16:19:28.000000 pipsqliext-1.0.0/pipsqliext.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      167 2023-05-14 16:19:28.000000 pipsqliext-1.0.0/pipsqliext.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 16:19:28.000000 pipsqliext-1.0.0/pipsqliext.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-14 16:19:28.000000 pipsqliext-1.0.0/pipsqliext.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 16:19:28.413410 pipsqliext-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      556 2023-05-14 16:19:28.000000 pipsqliext-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 16:21:33.520131 pipsqliext-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      343 2023-05-14 16:21:33.520131 pipsqliext-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 16:21:33.520131 pipsqliext-1.1.0/pipsqliext/
+-rw-r--r--   0 root         (0) root         (0)    96635 2023-05-14 16:21:33.000000 pipsqliext-1.1.0/pipsqliext/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 16:21:33.520131 pipsqliext-1.1.0/pipsqliext.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      343 2023-05-14 16:21:33.000000 pipsqliext-1.1.0/pipsqliext.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      167 2023-05-14 16:21:33.000000 pipsqliext-1.1.0/pipsqliext.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 16:21:33.000000 pipsqliext-1.1.0/pipsqliext.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-14 16:21:33.000000 pipsqliext-1.1.0/pipsqliext.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 16:21:33.520131 pipsqliext-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      556 2023-05-14 16:21:33.000000 pipsqliext-1.1.0/setup.py
```

### Comparing `pipsqliext-1.0.0/setup.py` & `pipsqliext-1.1.0/setup.py`

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
     name="pipsqliext",
     version=VERSION,
```

