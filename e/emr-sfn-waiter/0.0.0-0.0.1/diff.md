# Comparing `tmp/emr-sfn-waiter-0.0.0.tar.gz` & `tmp/emr-sfn-waiter-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emr-sfn-waiter-0.0.0.tar", last modified: Sat May 13 13:58:18 2023, max compression
+gzip compressed data, was "emr-sfn-waiter-0.0.1.tar", last modified: Sun May 14 05:52:34 2023, max compression
```

## Comparing `emr-sfn-waiter-0.0.0.tar` & `emr-sfn-waiter-0.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:58:18.170061 emr-sfn-waiter-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-13 13:58:04.000000 emr-sfn-waiter-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-13 13:58:04.000000 emr-sfn-waiter-0.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-13 13:58:18.166061 emr-sfn-waiter-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-13 13:58:04.000000 emr-sfn-waiter-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-13 13:58:04.000000 emr-sfn-waiter-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 13:58:18.170061 emr-sfn-waiter-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-13 13:58:04.000000 emr-sfn-waiter-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:58:18.166061 emr-sfn-waiter-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:58:18.166061 emr-sfn-waiter-0.0.0/src/emr_sfn_waiter/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:58:18.166061 emr-sfn-waiter-0.0.0/src/emr_sfn_waiter/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-13 13:58:04.000000 emr-sfn-waiter-0.0.0/src/emr_sfn_waiter/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13639 2023-05-13 13:58:04.000000 emr-sfn-waiter-0.0.0/src/emr_sfn_waiter/_jsii/emr-sfn-waiter@0.0.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:58:18.166061 emr-sfn-waiter-0.0.0/src/emr_sfn_waiter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-13 13:58:18.000000 emr-sfn-waiter-0.0.0/src/emr_sfn_waiter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-13 13:58:18.000000 emr-sfn-waiter-0.0.0/src/emr_sfn_waiter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:58:18.000000 emr-sfn-waiter-0.0.0/src/emr_sfn_waiter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-13 13:58:18.000000 emr-sfn-waiter-0.0.0/src/emr_sfn_waiter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-13 13:58:18.000000 emr-sfn-waiter-0.0.0/src/emr_sfn_waiter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:52:34.301724 emr-sfn-waiter-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-14 05:52:18.000000 emr-sfn-waiter-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-14 05:52:18.000000 emr-sfn-waiter-0.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-14 05:52:34.301724 emr-sfn-waiter-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-14 05:52:18.000000 emr-sfn-waiter-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-14 05:52:18.000000 emr-sfn-waiter-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 05:52:34.301724 emr-sfn-waiter-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-14 05:52:18.000000 emr-sfn-waiter-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:52:34.297724 emr-sfn-waiter-0.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:52:34.297724 emr-sfn-waiter-0.0.1/src/emr_sfn_waiter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:52:34.301724 emr-sfn-waiter-0.0.1/src/emr_sfn_waiter/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-14 05:52:18.000000 emr-sfn-waiter-0.0.1/src/emr_sfn_waiter/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13636 2023-05-14 05:52:18.000000 emr-sfn-waiter-0.0.1/src/emr_sfn_waiter/_jsii/emr-sfn-waiter@0.0.1.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:52:34.301724 emr-sfn-waiter-0.0.1/src/emr_sfn_waiter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-14 05:52:34.000000 emr-sfn-waiter-0.0.1/src/emr_sfn_waiter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-14 05:52:34.000000 emr-sfn-waiter-0.0.1/src/emr_sfn_waiter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 05:52:34.000000 emr-sfn-waiter-0.0.1/src/emr_sfn_waiter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-14 05:52:34.000000 emr-sfn-waiter-0.0.1/src/emr_sfn_waiter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-14 05:52:34.000000 emr-sfn-waiter-0.0.1/src/emr_sfn_waiter.egg-info/top_level.txt
```

### Comparing `emr-sfn-waiter-0.0.0/LICENSE` & `emr-sfn-waiter-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `emr-sfn-waiter-0.0.0/PKG-INFO` & `emr-sfn-waiter-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emr-sfn-waiter
-Version: 0.0.0
+Version: 0.0.1
 Summary: CDK library for an SFN workflow that polls for EMR Serverless job completion
 Home-page: https://github.com/alexgelman/emr-sfn-waiter
 Author: Alex Gelman<6887237+alexgelman@users.noreply.github.com>
 License: MIT
 Project-URL: Source, https://github.com/alexgelman/emr-sfn-waiter
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `emr-sfn-waiter-0.0.0/setup.py` & `emr-sfn-waiter-0.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "emr-sfn-waiter",
-    "version": "0.0.0",
+    "version": "0.0.1",
     "description": "CDK library for an SFN workflow that polls for EMR Serverless job completion",
     "license": "MIT",
     "url": "https://github.com/alexgelman/emr-sfn-waiter",
     "long_description_content_type": "text/markdown",
     "author": "Alex Gelman<6887237+alexgelman@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -21,21 +21,21 @@
         "": "src"
     },
     "packages": [
         "emr_sfn_waiter._jsii"
     ],
     "package_data": {
         "emr_sfn_waiter._jsii": [
-            "emr-sfn-waiter@0.0.0.jsii.tgz"
+            "emr-sfn-waiter@0.0.1.jsii.tgz"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib==2.79.1",
-        "constructs>=10.0.0, <11.0.0",
+        "constructs>=10.2.23, <11.0.0",
         "jsii>=1.81.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
```

### Comparing `emr-sfn-waiter-0.0.0/src/emr_sfn_waiter.egg-info/PKG-INFO` & `emr-sfn-waiter-0.0.1/src/emr_sfn_waiter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emr-sfn-waiter
-Version: 0.0.0
+Version: 0.0.1
 Summary: CDK library for an SFN workflow that polls for EMR Serverless job completion
 Home-page: https://github.com/alexgelman/emr-sfn-waiter
 Author: Alex Gelman<6887237+alexgelman@users.noreply.github.com>
 License: MIT
 Project-URL: Source, https://github.com/alexgelman/emr-sfn-waiter
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

