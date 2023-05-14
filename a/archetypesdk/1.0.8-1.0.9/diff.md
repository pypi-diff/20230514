# Comparing `tmp/archetypesdk-1.0.8.tar.gz` & `tmp/archetypesdk-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archetypesdk-1.0.8.tar", last modified: Mon Jan  2 01:38:00 2023, max compression
+gzip compressed data, was "archetypesdk-1.0.9.tar", last modified: Mon Jan  2 01:48:15 2023, max compression
```

## Comparing `archetypesdk-1.0.8.tar` & `archetypesdk-1.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 behailutekletsadik   (501) staff       (20)        0 2023-01-02 01:38:00.530866 archetypesdk-1.0.8/
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)    33819 2022-12-31 19:59:43.000000 archetypesdk-1.0.8/LICENSE
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)     4423 2023-01-02 01:38:00.530704 archetypesdk-1.0.8/PKG-INFO
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)     3977 2022-12-31 21:19:56.000000 archetypesdk-1.0.8/README.md
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)      103 2022-12-31 19:59:35.000000 archetypesdk-1.0.8/pyproject.toml
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)       38 2023-01-02 01:38:00.530902 archetypesdk-1.0.8/setup.cfg
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)      787 2023-01-02 01:37:45.000000 archetypesdk-1.0.8/setup.py
-drwxr-xr-x   0 behailutekletsadik   (501) staff       (20)        0 2023-01-02 01:38:00.524752 archetypesdk-1.0.8/src/
-drwxr-xr-x   0 behailutekletsadik   (501) staff       (20)        0 2023-01-02 01:38:00.527502 archetypesdk-1.0.8/src/archetypesdk/
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)      971 2022-12-31 19:59:35.000000 archetypesdk-1.0.8/src/archetypesdk/__init__.py
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)      383 2022-12-31 19:59:35.000000 archetypesdk-1.0.8/src/archetypesdk/api_request_thread.py
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)     1478 2022-12-31 19:59:35.000000 archetypesdk-1.0.8/src/archetypesdk/api_requestor.py
-drwxr-xr-x   0 behailutekletsadik   (501) staff       (20)        0 2023-01-02 01:38:00.530429 archetypesdk-1.0.8/src/archetypesdk/api_resources/
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)      467 2023-01-02 01:37:28.000000 archetypesdk-1.0.8/src/archetypesdk/api_resources/__init__.py
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)        0 2022-12-31 19:59:35.000000 archetypesdk-1.0.8/src/archetypesdk/api_resources/api.py
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)     2558 2022-12-31 19:59:35.000000 archetypesdk-1.0.8/src/archetypesdk/api_resources/api_resource.py
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)     1961 2022-12-31 19:59:35.000000 archetypesdk-1.0.8/src/archetypesdk/api_resources/auth.py
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)     1523 2022-12-31 19:59:35.000000 archetypesdk-1.0.8/src/archetypesdk/api_resources/billable_metric.py
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)     4670 2022-12-31 19:59:35.000000 archetypesdk-1.0.8/src/archetypesdk/api_resources/client_ip.py
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)     3391 2022-12-31 19:59:35.000000 archetypesdk-1.0.8/src/archetypesdk/api_resources/customer.py
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)     1138 2022-12-31 19:59:35.000000 archetypesdk-1.0.8/src/archetypesdk/api_resources/endpoint.py
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)     1312 2022-12-31 19:59:35.000000 archetypesdk-1.0.8/src/archetypesdk/api_resources/error.py
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)      921 2022-12-31 19:59:35.000000 archetypesdk-1.0.8/src/archetypesdk/api_resources/product.py
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)      396 2023-01-02 00:37:38.000000 archetypesdk-1.0.8/src/archetypesdk/api_resources/token.py
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)      898 2022-12-31 19:59:35.000000 archetypesdk-1.0.8/src/archetypesdk/api_resources/track.py
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)     1795 2022-12-31 19:59:35.000000 archetypesdk-1.0.8/src/archetypesdk/auth_requestor.py
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)      116 2022-12-31 19:59:35.000000 archetypesdk-1.0.8/src/archetypesdk/enums.py
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)     1309 2022-12-31 19:59:35.000000 archetypesdk-1.0.8/src/archetypesdk/fastapi.py
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)      750 2022-12-31 19:59:35.000000 archetypesdk-1.0.8/src/archetypesdk/utils.py
-drwxr-xr-x   0 behailutekletsadik   (501) staff       (20)        0 2023-01-02 01:38:00.528366 archetypesdk-1.0.8/src/archetypesdk.egg-info/
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)     4423 2023-01-02 01:38:00.000000 archetypesdk-1.0.8/src/archetypesdk.egg-info/PKG-INFO
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)     1005 2023-01-02 01:38:00.000000 archetypesdk-1.0.8/src/archetypesdk.egg-info/SOURCES.txt
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)        1 2023-01-02 01:38:00.000000 archetypesdk-1.0.8/src/archetypesdk.egg-info/dependency_links.txt
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)        1 2023-01-02 01:38:00.000000 archetypesdk-1.0.8/src/archetypesdk.egg-info/not-zip-safe
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)       15 2023-01-02 01:38:00.000000 archetypesdk-1.0.8/src/archetypesdk.egg-info/requires.txt
--rw-r--r--   0 behailutekletsadik   (501) staff       (20)       13 2023-01-02 01:38:00.000000 archetypesdk-1.0.8/src/archetypesdk.egg-info/top_level.txt
+drwxr-xr-x   0 behailutekletsadik   (501) staff       (20)        0 2023-01-02 01:48:15.413045 archetypesdk-1.0.9/
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)    33819 2022-12-31 19:59:43.000000 archetypesdk-1.0.9/LICENSE
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)     4423 2023-01-02 01:48:15.412917 archetypesdk-1.0.9/PKG-INFO
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)     3977 2022-12-31 21:19:56.000000 archetypesdk-1.0.9/README.md
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)      103 2022-12-31 19:59:35.000000 archetypesdk-1.0.9/pyproject.toml
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)       38 2023-01-02 01:48:15.413082 archetypesdk-1.0.9/setup.cfg
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)      787 2023-01-02 01:48:02.000000 archetypesdk-1.0.9/setup.py
+drwxr-xr-x   0 behailutekletsadik   (501) staff       (20)        0 2023-01-02 01:48:15.405736 archetypesdk-1.0.9/src/
+drwxr-xr-x   0 behailutekletsadik   (501) staff       (20)        0 2023-01-02 01:48:15.409574 archetypesdk-1.0.9/src/archetypesdk/
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)      971 2022-12-31 19:59:35.000000 archetypesdk-1.0.9/src/archetypesdk/__init__.py
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)      383 2022-12-31 19:59:35.000000 archetypesdk-1.0.9/src/archetypesdk/api_request_thread.py
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)     1478 2022-12-31 19:59:35.000000 archetypesdk-1.0.9/src/archetypesdk/api_requestor.py
+drwxr-xr-x   0 behailutekletsadik   (501) staff       (20)        0 2023-01-02 01:48:15.412448 archetypesdk-1.0.9/src/archetypesdk/api_resources/
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)      467 2023-01-02 01:37:28.000000 archetypesdk-1.0.9/src/archetypesdk/api_resources/__init__.py
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)        0 2022-12-31 19:59:35.000000 archetypesdk-1.0.9/src/archetypesdk/api_resources/api.py
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)     2558 2022-12-31 19:59:35.000000 archetypesdk-1.0.9/src/archetypesdk/api_resources/api_resource.py
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)     1961 2022-12-31 19:59:35.000000 archetypesdk-1.0.9/src/archetypesdk/api_resources/auth.py
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)     1523 2022-12-31 19:59:35.000000 archetypesdk-1.0.9/src/archetypesdk/api_resources/billable_metric.py
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)     4670 2022-12-31 19:59:35.000000 archetypesdk-1.0.9/src/archetypesdk/api_resources/client_ip.py
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)     3391 2022-12-31 19:59:35.000000 archetypesdk-1.0.9/src/archetypesdk/api_resources/customer.py
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)     1138 2022-12-31 19:59:35.000000 archetypesdk-1.0.9/src/archetypesdk/api_resources/endpoint.py
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)     1312 2022-12-31 19:59:35.000000 archetypesdk-1.0.9/src/archetypesdk/api_resources/error.py
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)      921 2022-12-31 19:59:35.000000 archetypesdk-1.0.9/src/archetypesdk/api_resources/product.py
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)      396 2023-01-02 01:47:56.000000 archetypesdk-1.0.9/src/archetypesdk/api_resources/token.py
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)      898 2022-12-31 19:59:35.000000 archetypesdk-1.0.9/src/archetypesdk/api_resources/track.py
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)     1795 2022-12-31 19:59:35.000000 archetypesdk-1.0.9/src/archetypesdk/auth_requestor.py
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)      116 2022-12-31 19:59:35.000000 archetypesdk-1.0.9/src/archetypesdk/enums.py
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)     1309 2022-12-31 19:59:35.000000 archetypesdk-1.0.9/src/archetypesdk/fastapi.py
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)      750 2022-12-31 19:59:35.000000 archetypesdk-1.0.9/src/archetypesdk/utils.py
+drwxr-xr-x   0 behailutekletsadik   (501) staff       (20)        0 2023-01-02 01:48:15.410387 archetypesdk-1.0.9/src/archetypesdk.egg-info/
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)     4423 2023-01-02 01:48:15.000000 archetypesdk-1.0.9/src/archetypesdk.egg-info/PKG-INFO
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)     1005 2023-01-02 01:48:15.000000 archetypesdk-1.0.9/src/archetypesdk.egg-info/SOURCES.txt
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)        1 2023-01-02 01:48:15.000000 archetypesdk-1.0.9/src/archetypesdk.egg-info/dependency_links.txt
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)        1 2023-01-02 01:48:15.000000 archetypesdk-1.0.9/src/archetypesdk.egg-info/not-zip-safe
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)       15 2023-01-02 01:48:15.000000 archetypesdk-1.0.9/src/archetypesdk.egg-info/requires.txt
+-rw-r--r--   0 behailutekletsadik   (501) staff       (20)       13 2023-01-02 01:48:15.000000 archetypesdk-1.0.9/src/archetypesdk.egg-info/top_level.txt
```

### Comparing `archetypesdk-1.0.8/LICENSE` & `archetypesdk-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `archetypesdk-1.0.8/PKG-INFO` & `archetypesdk-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archetypesdk
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python bindings for Archetype. Archetype makes API monetization and usage based billing for APIs easy.
 Home-page: https://github.com/ArchetypeAPI/
 Author: Archetype
 Author-email: hello@archetype.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `archetypesdk-1.0.8/README.md` & `archetypesdk-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `archetypesdk-1.0.8/setup.py` & `archetypesdk-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="archetypesdk",
-    version="1.0.8",
+    version="1.0.9",
     description="Python bindings for Archetype. Archetype makes API monetization and usage based billing for APIs easy.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ArchetypeAPI/",
     author="Archetype",
     author_email="hello@archetype.dev",
     classifiers=[
```

### Comparing `archetypesdk-1.0.8/src/archetypesdk/__init__.py` & `archetypesdk-1.0.9/src/archetypesdk/__init__.py`

 * *Files identical despite different names*

### Comparing `archetypesdk-1.0.8/src/archetypesdk/api_requestor.py` & `archetypesdk-1.0.9/src/archetypesdk/api_requestor.py`

 * *Files identical despite different names*

### Comparing `archetypesdk-1.0.8/src/archetypesdk/api_resources/api_resource.py` & `archetypesdk-1.0.9/src/archetypesdk/api_resources/api_resource.py`

 * *Files identical despite different names*

### Comparing `archetypesdk-1.0.8/src/archetypesdk/api_resources/auth.py` & `archetypesdk-1.0.9/src/archetypesdk/api_resources/auth.py`

 * *Files identical despite different names*

### Comparing `archetypesdk-1.0.8/src/archetypesdk/api_resources/billable_metric.py` & `archetypesdk-1.0.9/src/archetypesdk/api_resources/billable_metric.py`

 * *Files identical despite different names*

### Comparing `archetypesdk-1.0.8/src/archetypesdk/api_resources/client_ip.py` & `archetypesdk-1.0.9/src/archetypesdk/api_resources/client_ip.py`

 * *Files identical despite different names*

### Comparing `archetypesdk-1.0.8/src/archetypesdk/api_resources/customer.py` & `archetypesdk-1.0.9/src/archetypesdk/api_resources/customer.py`

 * *Files identical despite different names*

### Comparing `archetypesdk-1.0.8/src/archetypesdk/api_resources/endpoint.py` & `archetypesdk-1.0.9/src/archetypesdk/api_resources/endpoint.py`

 * *Files identical despite different names*

### Comparing `archetypesdk-1.0.8/src/archetypesdk/api_resources/error.py` & `archetypesdk-1.0.9/src/archetypesdk/api_resources/error.py`

 * *Files identical despite different names*

### Comparing `archetypesdk-1.0.8/src/archetypesdk/api_resources/product.py` & `archetypesdk-1.0.9/src/archetypesdk/api_resources/product.py`

 * *Files identical despite different names*

### Comparing `archetypesdk-1.0.8/src/archetypesdk/api_resources/track.py` & `archetypesdk-1.0.9/src/archetypesdk/api_resources/track.py`

 * *Files identical despite different names*

### Comparing `archetypesdk-1.0.8/src/archetypesdk/auth_requestor.py` & `archetypesdk-1.0.9/src/archetypesdk/auth_requestor.py`

 * *Files identical despite different names*

### Comparing `archetypesdk-1.0.8/src/archetypesdk/fastapi.py` & `archetypesdk-1.0.9/src/archetypesdk/fastapi.py`

 * *Files identical despite different names*

### Comparing `archetypesdk-1.0.8/src/archetypesdk/utils.py` & `archetypesdk-1.0.9/src/archetypesdk/utils.py`

 * *Files identical despite different names*

### Comparing `archetypesdk-1.0.8/src/archetypesdk.egg-info/PKG-INFO` & `archetypesdk-1.0.9/src/archetypesdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archetypesdk
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python bindings for Archetype. Archetype makes API monetization and usage based billing for APIs easy.
 Home-page: https://github.com/ArchetypeAPI/
 Author: Archetype
 Author-email: hello@archetype.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `archetypesdk-1.0.8/src/archetypesdk.egg-info/SOURCES.txt` & `archetypesdk-1.0.9/src/archetypesdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

