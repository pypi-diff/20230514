# Comparing `tmp/tarvis-indicators-webapi-0.9.5.tar.gz` & `tmp/tarvis-indicators-webapi-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarvis-indicators-webapi-0.9.5.tar", last modified: Wed May  3 01:58:42 2023, max compression
+gzip compressed data, was "tarvis-indicators-webapi-0.9.6.tar", last modified: Sun May 14 09:45:35 2023, max compression
```

## Comparing `tarvis-indicators-webapi-0.9.5.tar` & `tarvis-indicators-webapi-0.9.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:58:42.191943 tarvis-indicators-webapi-0.9.5/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-05-03 01:58:33.000000 tarvis-indicators-webapi-0.9.5/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      326 2023-05-03 01:58:42.191943 tarvis-indicators-webapi-0.9.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-03 01:58:33.000000 tarvis-indicators-webapi-0.9.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 01:58:42.191943 tarvis-indicators-webapi-0.9.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      644 2023-05-03 01:58:33.000000 tarvis-indicators-webapi-0.9.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:58:42.187942 tarvis-indicators-webapi-0.9.5/tarvis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:58:42.187942 tarvis-indicators-webapi-0.9.5/tarvis/indicators/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:58:42.187942 tarvis-indicators-webapi-0.9.5/tarvis/indicators/webapi/
--rw-r--r--   0 root         (0) root         (0)     2766 2023-05-03 01:58:33.000000 tarvis-indicators-webapi-0.9.5/tarvis/indicators/webapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:58:42.191943 tarvis-indicators-webapi-0.9.5/tarvis_indicators_webapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      326 2023-05-03 01:58:42.000000 tarvis-indicators-webapi-0.9.5/tarvis_indicators_webapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      306 2023-05-03 01:58:42.000000 tarvis-indicators-webapi-0.9.5/tarvis_indicators_webapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 01:58:42.000000 tarvis-indicators-webapi-0.9.5/tarvis_indicators_webapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 01:58:42.000000 tarvis-indicators-webapi-0.9.5/tarvis_indicators_webapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-03 01:58:42.000000 tarvis-indicators-webapi-0.9.5/tarvis_indicators_webapi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:45:35.876137 tarvis-indicators-webapi-0.9.6/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-05-14 09:45:25.000000 tarvis-indicators-webapi-0.9.6/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      326 2023-05-14 09:45:35.876137 tarvis-indicators-webapi-0.9.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-14 09:45:25.000000 tarvis-indicators-webapi-0.9.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 09:45:35.876137 tarvis-indicators-webapi-0.9.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      644 2023-05-14 09:45:25.000000 tarvis-indicators-webapi-0.9.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:45:35.872137 tarvis-indicators-webapi-0.9.6/tarvis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:45:35.872137 tarvis-indicators-webapi-0.9.6/tarvis/indicators/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:45:35.876137 tarvis-indicators-webapi-0.9.6/tarvis/indicators/webapi/
+-rw-r--r--   0 root         (0) root         (0)     2766 2023-05-14 09:45:25.000000 tarvis-indicators-webapi-0.9.6/tarvis/indicators/webapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:45:35.876137 tarvis-indicators-webapi-0.9.6/tarvis_indicators_webapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      326 2023-05-14 09:45:35.000000 tarvis-indicators-webapi-0.9.6/tarvis_indicators_webapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      306 2023-05-14 09:45:35.000000 tarvis-indicators-webapi-0.9.6/tarvis_indicators_webapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 09:45:35.000000 tarvis-indicators-webapi-0.9.6/tarvis_indicators_webapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 09:45:35.000000 tarvis-indicators-webapi-0.9.6/tarvis_indicators_webapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-14 09:45:35.000000 tarvis-indicators-webapi-0.9.6/tarvis_indicators_webapi.egg-info/top_level.txt
```

### Comparing `tarvis-indicators-webapi-0.9.5/LICENSE.txt` & `tarvis-indicators-webapi-0.9.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tarvis-indicators-webapi-0.9.5/setup.py` & `tarvis-indicators-webapi-0.9.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = requirements_file.read().splitlines()
 
 with open("README.md") as description_file:
     long_description = description_file.read()
 
 setup(
     name="tarvis-indicators-webapi",
-    version="0.9.5",
+    version="0.9.6",
     author="Tarvis Labs",
     author_email="python@tarvislabs.com",
     url="https://tarvislabs.com/",
     description="Tarvis Web API Indicators Library",
     long_description=long_description,
     packages=find_namespace_packages(include=["tarvis.*"]),
     python_requires=">=3.10",
```

### Comparing `tarvis-indicators-webapi-0.9.5/tarvis/indicators/webapi/__init__.py` & `tarvis-indicators-webapi-0.9.6/tarvis/indicators/webapi/__init__.py`

 * *Files identical despite different names*

