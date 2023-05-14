# Comparing `tmp/cdk8s-2.7.8.tar.gz` & `tmp/cdk8s-2.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-2.7.8.tar", last modified: Tue Feb 21 21:08:38 2023, max compression
+gzip compressed data, was "cdk8s-2.7.9.tar", last modified: Thu Feb 23 00:28:21 2023, max compression
```

## Comparing `cdk8s-2.7.8.tar` & `cdk8s-2.7.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 21:08:38.844973 cdk8s-2.7.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-21 21:08:25.000000 cdk8s-2.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-21 21:08:25.000000 cdk8s-2.7.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-21 21:08:25.000000 cdk8s-2.7.8/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-02-21 21:08:38.844973 cdk8s-2.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-02-21 21:08:25.000000 cdk8s-2.7.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-21 21:08:25.000000 cdk8s-2.7.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 21:08:38.844973 cdk8s-2.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-02-21 21:08:25.000000 cdk8s-2.7.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 21:08:38.840973 cdk8s-2.7.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 21:08:38.840973 cdk8s-2.7.8/src/cdk8s/
--rw-r--r--   0 runner    (1001) docker     (123)   136004 2023-02-21 21:08:25.000000 cdk8s-2.7.8/src/cdk8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 21:08:38.840973 cdk8s-2.7.8/src/cdk8s/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-02-21 21:08:25.000000 cdk8s-2.7.8/src/cdk8s/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   286741 2023-02-21 21:08:25.000000 cdk8s-2.7.8/src/cdk8s/_jsii/cdk8s@2.7.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 21:08:25.000000 cdk8s-2.7.8/src/cdk8s/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 21:08:38.840973 cdk8s-2.7.8/src/cdk8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-02-21 21:08:38.000000 cdk8s-2.7.8/src/cdk8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-02-21 21:08:38.000000 cdk8s-2.7.8/src/cdk8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 21:08:38.000000 cdk8s-2.7.8/src/cdk8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-21 21:08:38.000000 cdk8s-2.7.8/src/cdk8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-21 21:08:38.000000 cdk8s-2.7.8/src/cdk8s.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 00:28:21.392573 cdk8s-2.7.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-23 00:28:07.000000 cdk8s-2.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-23 00:28:07.000000 cdk8s-2.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-23 00:28:07.000000 cdk8s-2.7.9/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-02-23 00:28:21.392573 cdk8s-2.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-02-23 00:28:07.000000 cdk8s-2.7.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-23 00:28:07.000000 cdk8s-2.7.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 00:28:21.392573 cdk8s-2.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-02-23 00:28:07.000000 cdk8s-2.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 00:28:21.388573 cdk8s-2.7.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 00:28:21.388573 cdk8s-2.7.9/src/cdk8s/
+-rw-r--r--   0 runner    (1001) docker     (123)   136004 2023-02-23 00:28:07.000000 cdk8s-2.7.9/src/cdk8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 00:28:21.392573 cdk8s-2.7.9/src/cdk8s/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-02-23 00:28:07.000000 cdk8s-2.7.9/src/cdk8s/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   286735 2023-02-23 00:28:07.000000 cdk8s-2.7.9/src/cdk8s/_jsii/cdk8s@2.7.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 00:28:07.000000 cdk8s-2.7.9/src/cdk8s/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 00:28:21.392573 cdk8s-2.7.9/src/cdk8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-02-23 00:28:21.000000 cdk8s-2.7.9/src/cdk8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-02-23 00:28:21.000000 cdk8s-2.7.9/src/cdk8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 00:28:21.000000 cdk8s-2.7.9/src/cdk8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-23 00:28:21.000000 cdk8s-2.7.9/src/cdk8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-23 00:28:21.000000 cdk8s-2.7.9/src/cdk8s.egg-info/top_level.txt
```

### Comparing `cdk8s-2.7.8/LICENSE` & `cdk8s-2.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-2.7.8/PKG-INFO` & `cdk8s-2.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s
-Version: 2.7.8
+Version: 2.7.9
 Summary: This is the core library of Cloud Development Kit (CDK) for Kubernetes (cdk8s). cdk8s apps synthesize into standard Kubernetes manifests which can be applied to any Kubernetes cluster.
 Home-page: https://github.com/cdk8s-team/cdk8s-core.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-core.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk8s-2.7.8/README.md` & `cdk8s-2.7.9/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-2.7.8/setup.py` & `cdk8s-2.7.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s",
-    "version": "2.7.8",
+    "version": "2.7.9",
     "description": "This is the core library of Cloud Development Kit (CDK) for Kubernetes (cdk8s). cdk8s apps synthesize into standard Kubernetes manifests which can be applied to any Kubernetes cluster.",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-core.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk8s",
         "cdk8s._jsii"
     ],
     "package_data": {
         "cdk8s._jsii": [
-            "cdk8s@2.7.8.jsii.tgz"
+            "cdk8s@2.7.9.jsii.tgz"
         ],
         "cdk8s": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk8s-2.7.8/src/cdk8s/__init__.py` & `cdk8s-2.7.9/src/cdk8s/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-2.7.8/src/cdk8s.egg-info/PKG-INFO` & `cdk8s-2.7.9/src/cdk8s.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s
-Version: 2.7.8
+Version: 2.7.9
 Summary: This is the core library of Cloud Development Kit (CDK) for Kubernetes (cdk8s). cdk8s apps synthesize into standard Kubernetes manifests which can be applied to any Kubernetes cluster.
 Home-page: https://github.com/cdk8s-team/cdk8s-core.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-core.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

