# Comparing `tmp/elefantolib-0.9.1.tar.gz` & `tmp/elefantolib-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elefantolib-0.9.1.tar", max compression
+gzip compressed data, was "elefantolib-0.9.2.tar", max compression
```

## Comparing `elefantolib-0.9.1.tar` & `elefantolib-0.9.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1073 2023-04-24 16:13:52.984495 elefantolib-0.9.1/LICENSE
--rw-r--r--   0        0        0      146 2023-04-24 16:13:52.984495 elefantolib-0.9.1/README.rst
--rw-r--r--   0        0        0       22 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/__init__.py
--rw-r--r--   0        0        0     1776 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/auth/__init__.py
--rw-r--r--   0        0        0     1139 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/auth/user.py
--rw-r--r--   0        0        0      210 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/constants.py
--rw-r--r--   0        0        0     1849 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/context/__init__.py
--rw-r--r--   0        0        0      663 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/context/context_service.py
--rw-r--r--   0        0        0     1256 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/exceptions.py
--rw-r--r--   0        0        0      577 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/http_client/__init__.py
--rw-r--r--   0        0        0     2367 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/http_client/httpx_client.py
--rw-r--r--   0        0        0      373 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/logger_config.py
--rw-r--r--   0        0        0      889 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/middleware.py
--rw-r--r--   0        0        0      542 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/provider/__init__.py
--rw-r--r--   0        0        0      392 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/provider/django_provider/__init__.py
--rw-r--r--   0        0        0      386 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/provider/fastapi_provider/__init__.py
--rw-r--r--   0        0        0      404 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/websocket_client/__init__.py
--rw-r--r--   0        0        0      380 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/websocket_client/websocket_client.py
--rw-r--r--   0        0        0     1429 2023-04-24 16:14:04.759355 elefantolib-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     1131 1970-01-01 00:00:00.000000 elefantolib-0.9.1/setup.py
--rw-r--r--   0        0        0     1148 1970-01-01 00:00:00.000000 elefantolib-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-24 16:17:28.010882 elefantolib-0.9.2/LICENSE
+-rw-r--r--   0        0        0      146 2023-04-24 16:17:28.014882 elefantolib-0.9.2/README.rst
+-rw-r--r--   0        0        0       22 2023-04-24 16:17:28.014882 elefantolib-0.9.2/elefantolib/__init__.py
+-rw-r--r--   0        0        0     1776 2023-04-24 16:17:28.014882 elefantolib-0.9.2/elefantolib/auth/__init__.py
+-rw-r--r--   0        0        0     1139 2023-04-24 16:17:28.014882 elefantolib-0.9.2/elefantolib/auth/user.py
+-rw-r--r--   0        0        0      210 2023-04-24 16:17:28.014882 elefantolib-0.9.2/elefantolib/constants.py
+-rw-r--r--   0        0        0     1849 2023-04-24 16:17:28.014882 elefantolib-0.9.2/elefantolib/context/__init__.py
+-rw-r--r--   0        0        0      663 2023-04-24 16:17:28.014882 elefantolib-0.9.2/elefantolib/context/context_service.py
+-rw-r--r--   0        0        0     1256 2023-04-24 16:17:28.014882 elefantolib-0.9.2/elefantolib/exceptions.py
+-rw-r--r--   0        0        0      577 2023-04-24 16:17:28.014882 elefantolib-0.9.2/elefantolib/http_client/__init__.py
+-rw-r--r--   0        0        0     2367 2023-04-24 16:17:28.014882 elefantolib-0.9.2/elefantolib/http_client/httpx_client.py
+-rw-r--r--   0        0        0      373 2023-04-24 16:17:28.014882 elefantolib-0.9.2/elefantolib/logger_config.py
+-rw-r--r--   0        0        0      889 2023-04-24 16:17:28.014882 elefantolib-0.9.2/elefantolib/middleware.py
+-rw-r--r--   0        0        0      542 2023-04-24 16:17:28.014882 elefantolib-0.9.2/elefantolib/provider/__init__.py
+-rw-r--r--   0        0        0      392 2023-04-24 16:17:28.014882 elefantolib-0.9.2/elefantolib/provider/django_provider/__init__.py
+-rw-r--r--   0        0        0      386 2023-04-24 16:17:28.014882 elefantolib-0.9.2/elefantolib/provider/fastapi_provider/__init__.py
+-rw-r--r--   0        0        0      404 2023-04-24 16:17:28.014882 elefantolib-0.9.2/elefantolib/websocket_client/__init__.py
+-rw-r--r--   0        0        0      380 2023-04-24 16:17:28.014882 elefantolib-0.9.2/elefantolib/websocket_client/websocket_client.py
+-rw-r--r--   0        0        0     1429 2023-04-24 16:17:46.022883 elefantolib-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     1131 1970-01-01 00:00:00.000000 elefantolib-0.9.2/setup.py
+-rw-r--r--   0        0        0     1148 1970-01-01 00:00:00.000000 elefantolib-0.9.2/PKG-INFO
```

### Comparing `elefantolib-0.9.1/LICENSE` & `elefantolib-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `elefantolib-0.9.1/elefantolib/auth/__init__.py` & `elefantolib-0.9.2/elefantolib/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `elefantolib-0.9.1/elefantolib/auth/user.py` & `elefantolib-0.9.2/elefantolib/auth/user.py`

 * *Files identical despite different names*

### Comparing `elefantolib-0.9.1/elefantolib/context/__init__.py` & `elefantolib-0.9.2/elefantolib/context/__init__.py`

 * *Files identical despite different names*

### Comparing `elefantolib-0.9.1/elefantolib/context/context_service.py` & `elefantolib-0.9.2/elefantolib/context/context_service.py`

 * *Files identical despite different names*

### Comparing `elefantolib-0.9.1/elefantolib/exceptions.py` & `elefantolib-0.9.2/elefantolib/exceptions.py`

 * *Files identical despite different names*

### Comparing `elefantolib-0.9.1/elefantolib/http_client/__init__.py` & `elefantolib-0.9.2/elefantolib/http_client/__init__.py`

 * *Files identical despite different names*

### Comparing `elefantolib-0.9.1/elefantolib/http_client/httpx_client.py` & `elefantolib-0.9.2/elefantolib/http_client/httpx_client.py`

 * *Files identical despite different names*

### Comparing `elefantolib-0.9.1/elefantolib/middleware.py` & `elefantolib-0.9.2/elefantolib/middleware.py`

 * *Files identical despite different names*

### Comparing `elefantolib-0.9.1/elefantolib/provider/__init__.py` & `elefantolib-0.9.2/elefantolib/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `elefantolib-0.9.1/pyproject.toml` & `elefantolib-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "elefantolib"
 description = "Elefanto lib"
-version = "0.9.1"
+version = "0.9.2"
 authors = ["Elefanto <elefanto@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/elefanto-organization/elefantolib"
 repository = "https://github.com/elefanto-organization/elefantolib"
 classifiers = [
     "Operating System :: OS Independent",
```

### Comparing `elefantolib-0.9.1/setup.py` & `elefantolib-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'httpx>=0.23.3,<0.24.0',
  'pyjwt>=2.6.0,<3.0.0',
  'pytest-env>=0.8.1,<0.9.0',
  'websockets>=11.0,<12.0']
 
 setup_kwargs = {
     'name': 'elefantolib',
-    'version': '0.9.1',
+    'version': '0.9.2',
     'description': 'Elefanto lib',
     'long_description': 'Elefantolib\n-----------------------\n\n   **NOTE:** After clone this repository you should run command:\n\n   ``git config core.hooksPath .githooks``\n',
     'author': 'Elefanto',
     'author_email': 'elefanto@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/elefanto-organization/elefantolib',
```

### Comparing `elefantolib-0.9.1/PKG-INFO` & `elefantolib-0.9.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elefantolib
-Version: 0.9.1
+Version: 0.9.2
 Summary: Elefanto lib
 Home-page: https://github.com/elefanto-organization/elefantolib
 License: MIT
 Author: Elefanto
 Author-email: elefanto@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

