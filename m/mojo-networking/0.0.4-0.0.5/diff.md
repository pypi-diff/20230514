# Comparing `tmp/mojo_networking-0.0.4.tar.gz` & `tmp/mojo-networking-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_networking-0.0.4.tar", max compression
+gzip compressed data, was "mojo-networking-0.0.5.tar", max compression
```

## Comparing `mojo_networking-0.0.4.tar` & `mojo-networking-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1083 2023-03-20 16:35:27.038935 mojo_networking-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0      117 2023-03-20 16:35:27.038935 mojo_networking-0.0.4/README.md
--rw-r--r--   0        0        0      731 2023-03-21 07:33:24.440402 mojo_networking-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      500 2023-03-18 15:00:54.917241 mojo_networking-0.0.4/source/packages/mojo/networking/__init__.py
--rw-r--r--   0        0        0      613 2023-03-16 19:03:22.304009 mojo_networking-0.0.4/source/packages/mojo/networking/broadcast.py
--rw-r--r--   0        0        0     6959 2023-03-21 03:13:45.813161 mojo_networking-0.0.4/source/packages/mojo/networking/constants.py
--rw-r--r--   0        0        0     2910 2023-03-21 03:23:12.561679 mojo_networking-0.0.4/source/packages/mojo/networking/exceptions.py
--rw-r--r--   0        0        0     9204 2023-03-16 19:03:34.088103 mojo_networking-0.0.4/source/packages/mojo/networking/interfaces.py
--rw-r--r--   0        0        0     8824 2023-03-20 16:43:41.819833 mojo_networking-0.0.4/source/packages/mojo/networking/multicast.py
--rw-r--r--   0        0        0     2381 2023-03-17 14:58:49.355462 mojo_networking-0.0.4/source/packages/mojo/networking/resolution.py
--rw-r--r--   0        0        0     1845 2023-03-19 21:36:12.292413 mojo_networking-0.0.4/source/packages/mojo/networking/trafficcapturecontext.py
--rw-r--r--   0        0        0     4543 2023-03-20 16:43:44.355824 mojo_networking-0.0.4/source/packages/mojo/networking/unicast.py
--rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 mojo_networking-0.0.4/setup.py
--rw-r--r--   0        0        0      867 1970-01-01 00:00:00.000000 mojo_networking-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-03-20 16:35:27.038935 mojo-networking-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0      117 2023-03-20 16:35:27.038935 mojo-networking-0.0.5/README.md
+-rw-r--r--   0        0        0      731 2023-05-13 23:05:47.722493 mojo-networking-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      500 2023-03-18 15:00:54.917241 mojo-networking-0.0.5/source/packages/mojo/networking/__init__.py
+-rw-r--r--   0        0        0      613 2023-03-16 19:03:22.304009 mojo-networking-0.0.5/source/packages/mojo/networking/broadcast.py
+-rw-r--r--   0        0        0     6959 2023-03-21 03:13:45.813161 mojo-networking-0.0.5/source/packages/mojo/networking/constants.py
+-rw-r--r--   0        0        0     2910 2023-03-21 03:23:12.561679 mojo-networking-0.0.5/source/packages/mojo/networking/exceptions.py
+-rw-r--r--   0        0        0     9204 2023-03-16 19:03:34.088103 mojo-networking-0.0.5/source/packages/mojo/networking/interfaces.py
+-rw-r--r--   0        0        0     8824 2023-03-20 16:43:41.819833 mojo-networking-0.0.5/source/packages/mojo/networking/multicast.py
+-rw-r--r--   0        0        0     2381 2023-03-17 14:58:49.355462 mojo-networking-0.0.5/source/packages/mojo/networking/resolution.py
+-rw-r--r--   0        0        0     1845 2023-03-19 21:36:12.292413 mojo-networking-0.0.5/source/packages/mojo/networking/trafficcapturecontext.py
+-rw-r--r--   0        0        0     4543 2023-03-20 16:43:44.355824 mojo-networking-0.0.5/source/packages/mojo/networking/unicast.py
+-rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 mojo-networking-0.0.5/setup.py
+-rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 mojo-networking-0.0.5/PKG-INFO
```

### Comparing `mojo_networking-0.0.4/LICENSE.txt` & `mojo-networking-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mojo_networking-0.0.4/pyproject.toml` & `mojo-networking-0.0.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mojo-networking"
 description = "Automation Mojo Netorking Package (mojo-networking)"
-version = "0.0.4"
+version = "0.0.5"
 authors = []
 readme = "README.md"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX"
@@ -14,15 +14,15 @@
     "python"
 ]
 packages = [{include="mojo", from="source/packages"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 netifaces = "^0.11.0"
-requests = "^2.28.2"
+requests = "^2.29.0"
 
 [tool.poetry.group.dev.dependencies]
 myst-parser = "^0.18.1"
 sphinx = ">=1.6,<6"
 sphinx-rtd-theme = "^1.1.1"
 
 [tool.poetry.group.dbio.dependencies]
```

### Comparing `mojo_networking-0.0.4/source/packages/mojo/networking/broadcast.py` & `mojo-networking-0.0.5/source/packages/mojo/networking/broadcast.py`

 * *Files identical despite different names*

### Comparing `mojo_networking-0.0.4/source/packages/mojo/networking/constants.py` & `mojo-networking-0.0.5/source/packages/mojo/networking/constants.py`

 * *Files identical despite different names*

### Comparing `mojo_networking-0.0.4/source/packages/mojo/networking/exceptions.py` & `mojo-networking-0.0.5/source/packages/mojo/networking/exceptions.py`

 * *Files identical despite different names*

### Comparing `mojo_networking-0.0.4/source/packages/mojo/networking/interfaces.py` & `mojo-networking-0.0.5/source/packages/mojo/networking/interfaces.py`

 * *Files identical despite different names*

### Comparing `mojo_networking-0.0.4/source/packages/mojo/networking/multicast.py` & `mojo-networking-0.0.5/source/packages/mojo/networking/multicast.py`

 * *Files identical despite different names*

### Comparing `mojo_networking-0.0.4/source/packages/mojo/networking/resolution.py` & `mojo-networking-0.0.5/source/packages/mojo/networking/resolution.py`

 * *Files identical despite different names*

### Comparing `mojo_networking-0.0.4/source/packages/mojo/networking/trafficcapturecontext.py` & `mojo-networking-0.0.5/source/packages/mojo/networking/trafficcapturecontext.py`

 * *Files identical despite different names*

### Comparing `mojo_networking-0.0.4/source/packages/mojo/networking/unicast.py` & `mojo-networking-0.0.5/source/packages/mojo/networking/unicast.py`

 * *Files identical despite different names*

### Comparing `mojo_networking-0.0.4/setup.py` & `mojo-networking-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 packages = \
 ['mojo', 'mojo.networking']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['netifaces>=0.11.0,<0.12.0', 'requests>=2.28.2,<3.0.0']
+['netifaces>=0.11.0,<0.12.0', 'requests>=2.29.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'mojo-networking',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': 'Automation Mojo Netorking Package (mojo-networking)',
     'long_description': '# python-package-template\nThis is a template repository that can be used to quickly create a python package project.\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mojo_networking-0.0.4/PKG-INFO` & `mojo-networking-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: mojo-networking
-Version: 0.0.4
+Version: 0.0.5
 Summary: Automation Mojo Netorking Package (mojo-networking)
 License: LICENSE.txt
 Keywords: python
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: netifaces (>=0.11.0,<0.12.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: requests (>=2.29.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # python-package-template
 This is a template repository that can be used to quickly create a python package project.
```

