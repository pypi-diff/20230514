# Comparing `tmp/SuperDuperEasyAuth-0.1.1.tar.gz` & `tmp/SuperDuperEasyAuth-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SuperDuperEasyAuth-0.1.1.tar", last modified: Sat May 13 17:06:02 2023, max compression
+gzip compressed data, was "SuperDuperEasyAuth-0.2.1.tar", last modified: Sun May 14 17:43:33 2023, max compression
```

## Comparing `SuperDuperEasyAuth-0.1.1.tar` & `SuperDuperEasyAuth-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 noah      (1000) noah      (1000)        0 2023-05-13 17:06:02.389558 SuperDuperEasyAuth-0.1.1/
--rw-r--r--   0 noah      (1000) noah      (1000)       57 2023-05-13 17:03:13.000000 SuperDuperEasyAuth-0.1.1/CHANGELOG.txt
--rw-r--r--   0 noah      (1000) noah      (1000)     1063 2023-05-13 17:03:13.000000 SuperDuperEasyAuth-0.1.1/LICENSE.txt
--rw-r--r--   0 noah      (1000) noah      (1000)       25 2023-05-13 17:03:13.000000 SuperDuperEasyAuth-0.1.1/MANIFEST.in
--rw-r--r--   0 noah      (1000) noah      (1000)      996 2023-05-13 17:06:02.389558 SuperDuperEasyAuth-0.1.1/PKG-INFO
--rw-r--r--   0 noah      (1000) noah      (1000)      657 2023-05-13 17:03:13.000000 SuperDuperEasyAuth-0.1.1/README.md
-drwxr-xr-x   0 noah      (1000) noah      (1000)        0 2023-05-13 17:06:02.389558 SuperDuperEasyAuth-0.1.1/SuperDuperEasyAuth.egg-info/
--rw-r--r--   0 noah      (1000) noah      (1000)      996 2023-05-13 17:06:02.000000 SuperDuperEasyAuth-0.1.1/SuperDuperEasyAuth.egg-info/PKG-INFO
--rw-r--r--   0 noah      (1000) noah      (1000)      236 2023-05-13 17:06:02.000000 SuperDuperEasyAuth-0.1.1/SuperDuperEasyAuth.egg-info/SOURCES.txt
--rw-r--r--   0 noah      (1000) noah      (1000)        1 2023-05-13 17:06:02.000000 SuperDuperEasyAuth-0.1.1/SuperDuperEasyAuth.egg-info/dependency_links.txt
--rw-r--r--   0 noah      (1000) noah      (1000)        1 2023-05-13 17:06:02.000000 SuperDuperEasyAuth-0.1.1/SuperDuperEasyAuth.egg-info/top_level.txt
--rw-r--r--   0 noah      (1000) noah      (1000)      396 2023-05-13 17:03:13.000000 SuperDuperEasyAuth-0.1.1/__init__.py
--rw-r--r--   0 noah      (1000) noah      (1000)       38 2023-05-13 17:06:02.389558 SuperDuperEasyAuth-0.1.1/setup.cfg
--rw-r--r--   0 noah      (1000) noah      (1000)      683 2023-05-13 17:05:03.000000 SuperDuperEasyAuth-0.1.1/setup.py
+drwxr-xr-x   0 noah      (1000) noah      (1000)        0 2023-05-14 17:43:33.628823 SuperDuperEasyAuth-0.2.1/
+-rw-r--r--   0 noah      (1000) noah      (1000)       57 2023-05-14 17:21:51.000000 SuperDuperEasyAuth-0.2.1/CHANGELOG.txt
+-rw-r--r--   0 noah      (1000) noah      (1000)     1063 2023-05-14 17:21:51.000000 SuperDuperEasyAuth-0.2.1/LICENSE.txt
+-rw-r--r--   0 noah      (1000) noah      (1000)       25 2023-05-14 17:21:51.000000 SuperDuperEasyAuth-0.2.1/MANIFEST.in
+-rw-r--r--   0 noah      (1000) noah      (1000)      996 2023-05-14 17:43:33.628823 SuperDuperEasyAuth-0.2.1/PKG-INFO
+-rw-r--r--   0 noah      (1000) noah      (1000)      657 2023-05-14 17:21:51.000000 SuperDuperEasyAuth-0.2.1/README.md
+drwxr-xr-x   0 noah      (1000) noah      (1000)        0 2023-05-14 17:43:33.628823 SuperDuperEasyAuth-0.2.1/SuperDuperEasyAuth.egg-info/
+-rw-r--r--   0 noah      (1000) noah      (1000)      996 2023-05-14 17:43:33.000000 SuperDuperEasyAuth-0.2.1/SuperDuperEasyAuth.egg-info/PKG-INFO
+-rw-r--r--   0 noah      (1000) noah      (1000)      236 2023-05-14 17:43:33.000000 SuperDuperEasyAuth-0.2.1/SuperDuperEasyAuth.egg-info/SOURCES.txt
+-rw-r--r--   0 noah      (1000) noah      (1000)        1 2023-05-14 17:43:33.000000 SuperDuperEasyAuth-0.2.1/SuperDuperEasyAuth.egg-info/dependency_links.txt
+-rw-r--r--   0 noah      (1000) noah      (1000)        1 2023-05-14 17:43:33.000000 SuperDuperEasyAuth-0.2.1/SuperDuperEasyAuth.egg-info/top_level.txt
+-rw-r--r--   0 noah      (1000) noah      (1000)      398 2023-05-14 17:42:25.000000 SuperDuperEasyAuth-0.2.1/__init__.py
+-rw-r--r--   0 noah      (1000) noah      (1000)       38 2023-05-14 17:43:33.632824 SuperDuperEasyAuth-0.2.1/setup.cfg
+-rw-r--r--   0 noah      (1000) noah      (1000)      683 2023-05-14 17:24:30.000000 SuperDuperEasyAuth-0.2.1/setup.py
```

### Comparing `SuperDuperEasyAuth-0.1.1/LICENSE.txt` & `SuperDuperEasyAuth-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SuperDuperEasyAuth-0.1.1/PKG-INFO` & `SuperDuperEasyAuth-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SuperDuperEasyAuth
-Version: 0.1.1
+Version: 0.2.1
 Summary: UNKNOWN
 Home-page: https://github.com/noah560/EasyAuth
 Author: Noah C. C. S.
 Author-email: noahisontheinternet@outlook.com
 License: UNKNOWN
 Description: This is a simple Python library that enables simple authentication.
         For each authentication, the server generates a new and different number with the function authrand().
```

### Comparing `SuperDuperEasyAuth-0.1.1/README.md` & `SuperDuperEasyAuth-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `SuperDuperEasyAuth-0.1.1/SuperDuperEasyAuth.egg-info/PKG-INFO` & `SuperDuperEasyAuth-0.2.1/SuperDuperEasyAuth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SuperDuperEasyAuth
-Version: 0.1.1
+Version: 0.2.1
 Summary: UNKNOWN
 Home-page: https://github.com/noah560/EasyAuth
 Author: Noah C. C. S.
 Author-email: noahisontheinternet@outlook.com
 License: UNKNOWN
 Description: This is a simple Python library that enables simple authentication.
         For each authentication, the server generates a new and different number with the function authrand().
```

### Comparing `SuperDuperEasyAuth-0.1.1/setup.py` & `SuperDuperEasyAuth-0.2.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 
 setup(
     name="SuperDuperEasyAuth",
-    version="0.1.1",
+    version="0.2.1",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/noah560/EasyAuth",
     author="Noah C. C. S.",
     author_email="noahisontheinternet@outlook.com",
     install_requires=[]
 )
```

