# Comparing `tmp/pycrashreport-1.0.6.tar.gz` & `tmp/pycrashreport-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycrashreport-1.0.6.tar", last modified: Thu Mar  9 06:39:56 2023, max compression
+gzip compressed data, was "pycrashreport-1.0.7.tar", last modified: Sun May 14 07:39:58 2023, max compression
```

## Comparing `pycrashreport-1.0.6.tar` & `pycrashreport-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 06:39:55.997898 pycrashreport-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-03-09 06:39:48.000000 pycrashreport-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-03-09 06:39:55.997898 pycrashreport-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-03-09 06:39:48.000000 pycrashreport-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 06:39:55.997898 pycrashreport-1.0.6/pycrashreport/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 06:39:48.000000 pycrashreport-1.0.6/pycrashreport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-09 06:39:48.000000 pycrashreport-1.0.6/pycrashreport/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-03-09 06:39:48.000000 pycrashreport-1.0.6/pycrashreport/crash_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 06:39:55.997898 pycrashreport-1.0.6/pycrashreport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-03-09 06:39:55.000000 pycrashreport-1.0.6/pycrashreport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-09 06:39:55.000000 pycrashreport-1.0.6/pycrashreport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 06:39:55.000000 pycrashreport-1.0.6/pycrashreport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-09 06:39:55.000000 pycrashreport-1.0.6/pycrashreport.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 06:39:55.000000 pycrashreport-1.0.6/pycrashreport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-09 06:39:55.000000 pycrashreport-1.0.6/pycrashreport.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 06:39:55.997898 pycrashreport-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-03-09 06:39:48.000000 pycrashreport-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:39:58.351113 pycrashreport-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-14 07:39:37.000000 pycrashreport-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    45245 2023-05-14 07:39:58.351113 pycrashreport-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-05-14 07:39:37.000000 pycrashreport-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:39:58.347113 pycrashreport-1.0.7/pycrashreport/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 07:39:37.000000 pycrashreport-1.0.7/pycrashreport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-14 07:39:37.000000 pycrashreport-1.0.7/pycrashreport/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-05-14 07:39:37.000000 pycrashreport-1.0.7/pycrashreport/crash_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:39:58.351113 pycrashreport-1.0.7/pycrashreport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    45245 2023-05-14 07:39:58.000000 pycrashreport-1.0.7/pycrashreport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-14 07:39:58.000000 pycrashreport-1.0.7/pycrashreport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 07:39:58.000000 pycrashreport-1.0.7/pycrashreport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-14 07:39:58.000000 pycrashreport-1.0.7/pycrashreport.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-14 07:39:58.000000 pycrashreport-1.0.7/pycrashreport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 07:39:58.000000 pycrashreport-1.0.7/pycrashreport.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-14 07:39:37.000000 pycrashreport-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 07:39:37.000000 pycrashreport-1.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 07:39:58.351113 pycrashreport-1.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:39:58.351113 pycrashreport-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-05-14 07:39:37.000000 pycrashreport-1.0.7/tests/test_parse.py
```

### Comparing `pycrashreport-1.0.6/LICENSE` & `pycrashreport-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pycrashreport-1.0.6/README.md` & `pycrashreport-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pycrashreport-1.0.6/pycrashreport/crash_report.py` & `pycrashreport-1.0.7/pycrashreport/crash_report.py`

 * *Files identical despite different names*

