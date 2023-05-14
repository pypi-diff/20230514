# Comparing `tmp/v4xyz-0.0.5.tar.gz` & `tmp/v4xyz-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "v4xyz-0.0.5.tar", last modified: Sun May 14 09:51:52 2023, max compression
+gzip compressed data, was "v4xyz-0.0.6.tar", last modified: Sun May 14 09:54:53 2023, max compression
```

## Comparing `v4xyz-0.0.5.tar` & `v4xyz-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-14 09:51:51.991528 v4xyz-0.0.5/
--rw-r--r--   0 john      (1000) john      (1000)    11540 2023-05-13 11:27:28.000000 v4xyz-0.0.5/LICENSE
--rw-r--r--   0 john      (1000) john      (1000)     3128 2023-05-14 09:51:51.991528 v4xyz-0.0.5/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)     1863 2023-05-14 09:49:41.000000 v4xyz-0.0.5/README.md
--rw-r--r--   0 john      (1000) john      (1000)       74 2023-05-14 09:51:51.991528 v4xyz-0.0.5/setup.cfg
--rw-r--r--   0 john      (1000) john      (1000)     1429 2023-05-14 09:51:41.000000 v4xyz-0.0.5/setup.py
--rw-r--r--   0 john      (1000) john      (1000)     5242 2023-05-13 14:11:35.000000 v4xyz-0.0.5/v4.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-14 09:51:51.991528 v4xyz-0.0.5/v4xyz.egg-info/
--rw-r--r--   0 john      (1000) john      (1000)     3128 2023-05-14 09:51:51.000000 v4xyz-0.0.5/v4xyz.egg-info/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)      218 2023-05-14 09:51:51.000000 v4xyz-0.0.5/v4xyz.egg-info/SOURCES.txt
--rw-r--r--   0 john      (1000) john      (1000)        1 2023-05-14 09:51:51.000000 v4xyz-0.0.5/v4xyz.egg-info/dependency_links.txt
--rw-r--r--   0 john      (1000) john      (1000)       32 2023-05-14 09:51:51.000000 v4xyz-0.0.5/v4xyz.egg-info/entry_points.txt
--rw-r--r--   0 john      (1000) john      (1000)       50 2023-05-14 09:51:51.000000 v4xyz-0.0.5/v4xyz.egg-info/requires.txt
--rw-r--r--   0 john      (1000) john      (1000)        3 2023-05-14 09:51:51.000000 v4xyz-0.0.5/v4xyz.egg-info/top_level.txt
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-14 09:54:53.751529 v4xyz-0.0.6/
+-rw-r--r--   0 john      (1000) john      (1000)    11540 2023-05-13 11:27:28.000000 v4xyz-0.0.6/LICENSE
+-rw-r--r--   0 john      (1000) john      (1000)     3202 2023-05-14 09:54:53.751529 v4xyz-0.0.6/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)     1863 2023-05-14 09:49:41.000000 v4xyz-0.0.6/README.md
+-rw-r--r--   0 john      (1000) john      (1000)       74 2023-05-14 09:54:53.751529 v4xyz-0.0.6/setup.cfg
+-rw-r--r--   0 john      (1000) john      (1000)     1525 2023-05-14 09:54:51.000000 v4xyz-0.0.6/setup.py
+-rw-r--r--   0 john      (1000) john      (1000)     5242 2023-05-13 14:11:35.000000 v4xyz-0.0.6/v4.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-14 09:54:53.751529 v4xyz-0.0.6/v4xyz.egg-info/
+-rw-r--r--   0 john      (1000) john      (1000)     3202 2023-05-14 09:54:53.000000 v4xyz-0.0.6/v4xyz.egg-info/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)      218 2023-05-14 09:54:53.000000 v4xyz-0.0.6/v4xyz.egg-info/SOURCES.txt
+-rw-r--r--   0 john      (1000) john      (1000)        1 2023-05-14 09:54:53.000000 v4xyz-0.0.6/v4xyz.egg-info/dependency_links.txt
+-rw-r--r--   0 john      (1000) john      (1000)       32 2023-05-14 09:54:53.000000 v4xyz-0.0.6/v4xyz.egg-info/entry_points.txt
+-rw-r--r--   0 john      (1000) john      (1000)       50 2023-05-14 09:54:53.000000 v4xyz-0.0.6/v4xyz.egg-info/requires.txt
+-rw-r--r--   0 john      (1000) john      (1000)        3 2023-05-14 09:54:53.000000 v4xyz-0.0.6/v4xyz.egg-info/top_level.txt
```

### Comparing `v4xyz-0.0.5/LICENSE` & `v4xyz-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `v4xyz-0.0.5/PKG-INFO` & `v4xyz-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: v4xyz
-Version: 0.0.5
+Version: 0.0.6
 Summary: A command line tool to chat with GPT4 and render markdown response.
 Home-page: https://github.com/imhuwq/v4xyz
 Author: imhuwq
 Author-email: imhuwq@gmail.com
-License: UNKNOWN
+License: Apache License 2.0
 Description: # v4xyz
         
         ---
         <div align="center">
         <p align="center">
         
         <!-- prettier-ignore -->
@@ -88,8 +88,9 @@
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Terminals
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
```

### Comparing `v4xyz-0.0.5/README.md` & `v4xyz-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `v4xyz-0.0.5/setup.py` & `v4xyz-0.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.0.5"
+version = "0.0.6"
 description = "A command line tool to chat with GPT4 and render markdown response."
 with open("README.md") as fp:
     long_description = fp.read()
 url = "https://github.com/imhuwq/v4xyz"
 author = "imhuwq"
 author_email = "imhuwq@gmail.com"
 with open("LICENSE") as fp:
@@ -16,24 +16,26 @@
     "Topic :: Communications :: Chat",
     "Topic :: Terminals",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "License :: OSI Approved :: Apache Software License",
 ]
 
 setup(name="v4xyz",
       version=version,  # the package version, it may be different from the release version
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url=url,
       author=author,
       author_email=author_email,
+      license="Apache License 2.0",
       packages=[],
       py_modules=["v4"],
       entry_points={
           "console_scripts": [
               "v4=v4:main",
           ],
       },
```

### Comparing `v4xyz-0.0.5/v4.py` & `v4xyz-0.0.6/v4.py`

 * *Files identical despite different names*

### Comparing `v4xyz-0.0.5/v4xyz.egg-info/PKG-INFO` & `v4xyz-0.0.6/v4xyz.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: v4xyz
-Version: 0.0.5
+Version: 0.0.6
 Summary: A command line tool to chat with GPT4 and render markdown response.
 Home-page: https://github.com/imhuwq/v4xyz
 Author: imhuwq
 Author-email: imhuwq@gmail.com
-License: UNKNOWN
+License: Apache License 2.0
 Description: # v4xyz
         
         ---
         <div align="center">
         <p align="center">
         
         <!-- prettier-ignore -->
@@ -88,8 +88,9 @@
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Terminals
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
```

