# Comparing `tmp/uc_sgsim-1.2.0.tar.gz` & `tmp/uc_sgsim-1.2.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uc_sgsim-1.2.0.tar", last modified: Sun May 14 06:56:45 2023, max compression
+gzip compressed data, was "uc_sgsim-1.2.0rc0.tar", last modified: Sat May 13 07:21:17 2023, max compression
```

## Comparing `uc_sgsim-1.2.0.tar` & `uc_sgsim-1.2.0rc0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:56:45.734581 uc_sgsim-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-14 06:56:34.000000 uc_sgsim-1.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-05-14 06:56:45.734581 uc_sgsim-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-05-14 06:56:34.000000 uc_sgsim-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-14 06:56:45.734581 uc_sgsim-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-14 06:56:34.000000 uc_sgsim-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:56:45.730581 uc_sgsim-1.2.0/uc_sgsim/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-14 06:56:34.000000 uc_sgsim-1.2.0/uc_sgsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:56:45.730581 uc_sgsim-1.2.0/uc_sgsim/c_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 06:56:34.000000 uc_sgsim-1.2.0/uc_sgsim/c_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    85331 2023-05-14 06:56:34.000000 uc_sgsim-1.2.0/uc_sgsim/c_core/uc_sgsim.dll
--rwxr-xr-x   0 runner    (1001) docker     (123)    41272 2023-05-14 06:56:34.000000 uc_sgsim-1.2.0/uc_sgsim/c_core/uc_sgsim.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:56:45.730581 uc_sgsim-1.2.0/uc_sgsim/cov_model/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-14 06:56:34.000000 uc_sgsim-1.2.0/uc_sgsim/cov_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-14 06:56:34.000000 uc_sgsim-1.2.0/uc_sgsim/cov_model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-14 06:56:34.000000 uc_sgsim-1.2.0/uc_sgsim/cov_model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-14 06:56:34.000000 uc_sgsim-1.2.0/uc_sgsim/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:56:45.734581 uc_sgsim-1.2.0/uc_sgsim/krige/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-14 06:56:34.000000 uc_sgsim-1.2.0/uc_sgsim/krige/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-14 06:56:34.000000 uc_sgsim-1.2.0/uc_sgsim/krige/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-14 06:56:34.000000 uc_sgsim-1.2.0/uc_sgsim/krige/kriging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:56:45.734581 uc_sgsim-1.2.0/uc_sgsim/plot/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-14 06:56:34.000000 uc_sgsim-1.2.0/uc_sgsim/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-14 06:56:34.000000 uc_sgsim-1.2.0/uc_sgsim/plot/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-05-14 06:56:34.000000 uc_sgsim-1.2.0/uc_sgsim/plot/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-14 06:56:34.000000 uc_sgsim-1.2.0/uc_sgsim/random_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-05-14 06:56:34.000000 uc_sgsim-1.2.0/uc_sgsim/sgsim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-14 06:56:34.000000 uc_sgsim-1.2.0/uc_sgsim/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:56:45.730581 uc_sgsim-1.2.0/uc_sgsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-05-14 06:56:45.000000 uc_sgsim-1.2.0/uc_sgsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-14 06:56:45.000000 uc_sgsim-1.2.0/uc_sgsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 06:56:45.000000 uc_sgsim-1.2.0/uc_sgsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 06:56:45.000000 uc_sgsim-1.2.0/uc_sgsim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-14 06:56:45.000000 uc_sgsim-1.2.0/uc_sgsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-14 06:56:45.000000 uc_sgsim-1.2.0/uc_sgsim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:21:17.248176 uc_sgsim-1.2.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-05-13 07:21:17.248176 uc_sgsim-1.2.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-13 07:21:17.248176 uc_sgsim-1.2.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:21:17.248176 uc_sgsim-1.2.0rc0/uc_sgsim/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:21:17.248176 uc_sgsim-1.2.0rc0/uc_sgsim/c_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/c_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85331 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/c_core/uc_sgsim.dll
+-rwxr-xr-x   0 runner    (1001) docker     (123)    41272 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/c_core/uc_sgsim.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:21:17.248176 uc_sgsim-1.2.0rc0/uc_sgsim/cov_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/cov_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/cov_model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/cov_model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:21:17.248176 uc_sgsim-1.2.0rc0/uc_sgsim/krige/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/krige/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/krige/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/krige/kriging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:21:17.248176 uc_sgsim-1.2.0rc0/uc_sgsim/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/plot/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/plot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/random_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/sgsim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:21:17.248176 uc_sgsim-1.2.0rc0/uc_sgsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-05-13 07:21:17.000000 uc_sgsim-1.2.0rc0/uc_sgsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-13 07:21:17.000000 uc_sgsim-1.2.0rc0/uc_sgsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 07:21:17.000000 uc_sgsim-1.2.0rc0/uc_sgsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 07:21:17.000000 uc_sgsim-1.2.0rc0/uc_sgsim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-13 07:21:17.000000 uc_sgsim-1.2.0rc0/uc_sgsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-13 07:21:17.000000 uc_sgsim-1.2.0rc0/uc_sgsim.egg-info/top_level.txt
```

### Comparing `uc_sgsim-1.2.0/LICENSE.md` & `uc_sgsim-1.2.0rc0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.0/PKG-INFO` & `uc_sgsim-1.2.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uc_sgsim
-Version: 1.2.0
+Version: 1.2.0rc0
 Summary: Random Field Generation
 Home-page: https://github.com/Zncl2222/Stochastic_UC_SGSIM
 Author: Zncl2222
 Author-email: 3002shinning@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `uc_sgsim-1.2.0/README.md` & `uc_sgsim-1.2.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.0/setup.cfg` & `uc_sgsim-1.2.0rc0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = uc_sgsim
-version = 1.2.0
+version = 1.2.0rc0
 description = Random Field Generation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Zncl2222/Stochastic_UC_SGSIM
 author = Zncl2222
 author_email = 3002shinning@gmail.com
 license = MIT
```

### Comparing `uc_sgsim-1.2.0/uc_sgsim/c_core/uc_sgsim.dll` & `uc_sgsim-1.2.0rc0/uc_sgsim/c_core/uc_sgsim.dll`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.0/uc_sgsim/c_core/uc_sgsim.so` & `uc_sgsim-1.2.0rc0/uc_sgsim/c_core/uc_sgsim.so`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.0/uc_sgsim/cov_model/base.py` & `uc_sgsim-1.2.0rc0/uc_sgsim/cov_model/base.py`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.0/uc_sgsim/krige/base.py` & `uc_sgsim-1.2.0rc0/uc_sgsim/krige/base.py`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.0/uc_sgsim/krige/kriging.py` & `uc_sgsim-1.2.0rc0/uc_sgsim/krige/kriging.py`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.0/uc_sgsim/plot/base.py` & `uc_sgsim-1.2.0rc0/uc_sgsim/plot/base.py`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.0/uc_sgsim/plot/plot.py` & `uc_sgsim-1.2.0rc0/uc_sgsim/plot/plot.py`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.0/uc_sgsim/random_field.py` & `uc_sgsim-1.2.0rc0/uc_sgsim/random_field.py`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.0/uc_sgsim/sgsim.py` & `uc_sgsim-1.2.0rc0/uc_sgsim/sgsim.py`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.0/uc_sgsim/utils.py` & `uc_sgsim-1.2.0rc0/uc_sgsim/utils.py`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.0/uc_sgsim.egg-info/PKG-INFO` & `uc_sgsim-1.2.0rc0/uc_sgsim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uc-sgsim
-Version: 1.2.0
+Version: 1.2.0rc0
 Summary: Random Field Generation
 Home-page: https://github.com/Zncl2222/Stochastic_UC_SGSIM
 Author: Zncl2222
 Author-email: 3002shinning@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `uc_sgsim-1.2.0/uc_sgsim.egg-info/SOURCES.txt` & `uc_sgsim-1.2.0rc0/uc_sgsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

