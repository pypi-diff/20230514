# Comparing `tmp/wozoxutils-0.2.4.tar.gz` & `tmp/wozoxutils-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wozoxutils-0.2.4.tar", last modified: Wed Apr 19 12:38:13 2023, max compression
+gzip compressed data, was "wozoxutils-0.2.5.tar", last modified: Sun May 14 09:17:32 2023, max compression
```

## Comparing `wozoxutils-0.2.4.tar` & `wozoxutils-0.2.5.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:38:13.131841 wozoxutils-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-19 12:37:57.000000 wozoxutils-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-19 12:38:13.131841 wozoxutils-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-19 12:37:57.000000 wozoxutils-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 12:38:13.131841 wozoxutils-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-19 12:37:57.000000 wozoxutils-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:38:13.127840 wozoxutils-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-19 12:37:57.000000 wozoxutils-0.2.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-19 12:37:57.000000 wozoxutils-0.2.4/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-19 12:37:57.000000 wozoxutils-0.2.4/tests/test_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:38:13.127840 wozoxutils-0.2.4/wozoxutils/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 12:37:57.000000 wozoxutils-0.2.4/wozoxutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-19 12:37:57.000000 wozoxutils-0.2.4/wozoxutils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-19 12:37:57.000000 wozoxutils-0.2.4/wozoxutils/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-19 12:37:57.000000 wozoxutils-0.2.4/wozoxutils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-19 12:37:57.000000 wozoxutils-0.2.4/wozoxutils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:38:13.131841 wozoxutils-0.2.4/wozoxutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-19 12:38:13.000000 wozoxutils-0.2.4/wozoxutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-19 12:38:13.000000 wozoxutils-0.2.4/wozoxutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 12:38:13.000000 wozoxutils-0.2.4/wozoxutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-19 12:38:13.000000 wozoxutils-0.2.4/wozoxutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-19 12:38:13.000000 wozoxutils-0.2.4/wozoxutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:17:32.915646 wozoxutils-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-14 09:17:15.000000 wozoxutils-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-14 09:17:32.915646 wozoxutils-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-14 09:17:15.000000 wozoxutils-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 09:17:32.915646 wozoxutils-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-14 09:17:15.000000 wozoxutils-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:17:32.911646 wozoxutils-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-14 09:17:15.000000 wozoxutils-0.2.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-14 09:17:15.000000 wozoxutils-0.2.5/tests/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-14 09:17:15.000000 wozoxutils-0.2.5/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-14 09:17:15.000000 wozoxutils-0.2.5/tests/test_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:17:32.915646 wozoxutils-0.2.5/wozoxutils/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-14 09:17:15.000000 wozoxutils-0.2.5/wozoxutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-14 09:17:15.000000 wozoxutils-0.2.5/wozoxutils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-14 09:17:15.000000 wozoxutils-0.2.5/wozoxutils/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-14 09:17:15.000000 wozoxutils-0.2.5/wozoxutils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-14 09:17:15.000000 wozoxutils-0.2.5/wozoxutils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:17:32.915646 wozoxutils-0.2.5/wozoxutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-14 09:17:32.000000 wozoxutils-0.2.5/wozoxutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-14 09:17:32.000000 wozoxutils-0.2.5/wozoxutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 09:17:32.000000 wozoxutils-0.2.5/wozoxutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 09:17:32.000000 wozoxutils-0.2.5/wozoxutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 09:17:32.000000 wozoxutils-0.2.5/wozoxutils.egg-info/top_level.txt
```

### Comparing `wozoxutils-0.2.4/LICENSE` & `wozoxutils-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wozoxutils-0.2.4/setup.py` & `wozoxutils-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as f:
     long_description = f.read()
 
 setup(
     name="wozoxutils",
-    version="0.2.4",
+    version="0.2.5",
     packages=find_packages(),
     install_requires=[
         'pyyaml>=6.0',
     ],
     author="illiten",
     author_email="admin@leelib.com",
     description="general-purpose library for Python that contains various commonly used functional modules",
```

### Comparing `wozoxutils-0.2.4/wozoxutils/file.py` & `wozoxutils-0.2.5/wozoxutils/file.py`

 * *Files identical despite different names*

### Comparing `wozoxutils-0.2.4/wozoxutils/hash.py` & `wozoxutils-0.2.5/wozoxutils/hash.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 
 import hashlib
 
 
-def calculate_md5_for_flle(file_path: str) -> str:
+def calculate_md5_for_file(file_path: str) -> str:
     """
     Calculate the MD5 hash of the contents of a file.
 
     :param file_path: File path.
     :return: MD5 hash of the file contents.
     """
     md5_hash = hashlib.md5()
 
     with open(file_path, 'rb') as f:
-        for chunk in iter(lambda: f.read(4096), b''):
+        while chunk := f.read(1024*1024):  # 1MB
             md5_hash.update(chunk)
 
     return md5_hash.hexdigest()
 
 
 def calculate_md5_for_files(file_list: list[str]) -> str:
     """
@@ -25,11 +25,11 @@
     :param file_list: List of file paths.
     :return: MD5 hash of the concatenated file contents.
     """
     md5_hash = hashlib.md5()
 
     for file_path in file_list:
         with open(file_path, 'rb') as f:
-            for chunk in iter(lambda: f.read(4096), b''):
+            while chunk := f.read(1024*1024):  # 1MB
                 md5_hash.update(chunk)
 
     return md5_hash.hexdigest()
```

### Comparing `wozoxutils-0.2.4/wozoxutils/json.py` & `wozoxutils-0.2.5/wozoxutils/json.py`

 * *Files identical despite different names*

### Comparing `wozoxutils-0.2.4/wozoxutils/yaml.py` & `wozoxutils-0.2.5/wozoxutils/yaml.py`

 * *Files identical despite different names*

