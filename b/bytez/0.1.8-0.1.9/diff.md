# Comparing `tmp/bytez-0.1.8.tar.gz` & `tmp/bytez-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytez-0.1.8.tar", last modified: Fri Apr 28 01:02:00 2023, max compression
+gzip compressed data, was "bytez-0.1.9.tar", last modified: Fri Apr 28 01:02:38 2023, max compression
```

## Comparing `bytez-0.1.8.tar` & `bytez-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-04-28 01:02:00.708309 bytez-0.1.8/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      408 2023-04-28 01:02:00.708309 bytez-0.1.8/PKG-INFO
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       73 2023-03-26 07:05:33.000000 bytez-0.1.8/README.md
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-04-28 01:02:00.708309 bytez-0.1.8/bytez/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       32 2023-03-26 06:56:40.000000 bytez-0.1.8/bytez/__init__.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)    79093 2023-03-28 20:09:16.000000 bytez-0.1.8/bytez/main.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1068 2023-04-28 01:01:45.000000 bytez-0.1.8/bytez/pipeline.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-04-28 01:02:00.708309 bytez-0.1.8/bytez.egg-info/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      408 2023-04-28 01:02:00.000000 bytez-0.1.8/bytez.egg-info/PKG-INFO
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      212 2023-04-28 01:02:00.000000 bytez-0.1.8/bytez.egg-info/SOURCES.txt
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        1 2023-04-28 01:02:00.000000 bytez-0.1.8/bytez.egg-info/dependency_links.txt
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       70 2023-04-28 01:02:00.000000 bytez-0.1.8/bytez.egg-info/requires.txt
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        6 2023-04-28 01:02:00.000000 bytez-0.1.8/bytez.egg-info/top_level.txt
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       38 2023-04-28 01:02:00.708309 bytez-0.1.8/setup.cfg
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      662 2023-04-28 01:02:00.000000 bytez-0.1.8/setup.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-04-28 01:02:38.356341 bytez-0.1.9/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      408 2023-04-28 01:02:38.356341 bytez-0.1.9/PKG-INFO
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       73 2023-03-26 07:05:33.000000 bytez-0.1.9/README.md
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-04-28 01:02:38.356341 bytez-0.1.9/bytez/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       32 2023-03-26 06:56:40.000000 bytez-0.1.9/bytez/__init__.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)    79093 2023-03-28 20:09:16.000000 bytez-0.1.9/bytez/main.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1068 2023-04-28 01:01:45.000000 bytez-0.1.9/bytez/pipeline.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-04-28 01:02:38.356341 bytez-0.1.9/bytez.egg-info/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      408 2023-04-28 01:02:38.000000 bytez-0.1.9/bytez.egg-info/PKG-INFO
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      212 2023-04-28 01:02:38.000000 bytez-0.1.9/bytez.egg-info/SOURCES.txt
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        1 2023-04-28 01:02:38.000000 bytez-0.1.9/bytez.egg-info/dependency_links.txt
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       70 2023-04-28 01:02:38.000000 bytez-0.1.9/bytez.egg-info/requires.txt
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        6 2023-04-28 01:02:38.000000 bytez-0.1.9/bytez.egg-info/top_level.txt
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       38 2023-04-28 01:02:38.356341 bytez-0.1.9/setup.cfg
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      662 2023-04-28 01:02:36.000000 bytez-0.1.9/setup.py
```

### Comparing `bytez-0.1.8/bytez/main.py` & `bytez-0.1.9/bytez/main.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.8/bytez/pipeline.py` & `bytez-0.1.9/bytez/pipeline.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.8/setup.py` & `bytez-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 packages = find_packages()
 
 
 setup(
     name='bytez',
-    version='0.1.8',
+    version='0.1.9',
     packages=packages,
     install_requires=[
         'charset-normalizer==3.1.0',
         'idna==3.4',
         'requests==2.28.2',
         'urllib3==1.26.15',
     ],
```

