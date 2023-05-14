# Comparing `tmp/elefantolib_fastapi-0.2.3.tar.gz` & `tmp/elefantolib_fastapi-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elefantolib_fastapi-0.2.3.tar", max compression
+gzip compressed data, was "elefantolib_fastapi-0.2.4.tar", max compression
```

## Comparing `elefantolib_fastapi-0.2.3.tar` & `elefantolib_fastapi-0.2.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      878 2023-05-13 17:00:22.577011 elefantolib_fastapi-0.2.3/README.md
--rw-r--r--   0        0        0       22 2023-05-13 17:00:22.577011 elefantolib_fastapi-0.2.3/elefantolib_fastapi/__init__.py
--rw-r--r--   0        0        0      247 2023-05-13 17:00:22.577011 elefantolib_fastapi-0.2.3/elefantolib_fastapi/requests.py
--rw-r--r--   0        0        0      898 2023-05-13 17:00:22.577011 elefantolib_fastapi-0.2.3/elefantolib_fastapi/routes.py
--rw-r--r--   0        0        0      890 2023-05-13 17:00:39.993122 elefantolib_fastapi-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 elefantolib_fastapi-0.2.3/setup.py
--rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 elefantolib_fastapi-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      878 2023-05-14 08:45:20.080605 elefantolib_fastapi-0.2.4/README.md
+-rw-r--r--   0        0        0       22 2023-05-14 08:45:20.080605 elefantolib_fastapi-0.2.4/elefantolib_fastapi/__init__.py
+-rw-r--r--   0        0        0      247 2023-05-14 08:45:20.080605 elefantolib_fastapi-0.2.4/elefantolib_fastapi/requests.py
+-rw-r--r--   0        0        0      898 2023-05-14 08:45:20.080605 elefantolib_fastapi-0.2.4/elefantolib_fastapi/routes.py
+-rw-r--r--   0        0        0      890 2023-05-14 08:45:32.112843 elefantolib_fastapi-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 elefantolib_fastapi-0.2.4/setup.py
+-rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 elefantolib_fastapi-0.2.4/PKG-INFO
```

### Comparing `elefantolib_fastapi-0.2.3/README.md` & `elefantolib_fastapi-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `elefantolib_fastapi-0.2.3/elefantolib_fastapi/routes.py` & `elefantolib_fastapi-0.2.4/elefantolib_fastapi/routes.py`

 * *Files identical despite different names*

### Comparing `elefantolib_fastapi-0.2.3/pyproject.toml` & `elefantolib_fastapi-0.2.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "elefantolib-fastapi"
-version = "0.2.3"
+version = "0.2.4"
 description = ""
 authors = ["gglassota <gglassota2@gmail.com>"]
 readme = "README.md"
 packages = [{include = "elefantolib_fastapi"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-elefantolib = "^0.10.1"
 fastapi = "^0.95.1"
 redis = "^4.5.5"
+elefantolib = "^0.11.0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
 pytest-flake8 = "^1.1.1"
```

### Comparing `elefantolib_fastapi-0.2.3/setup.py` & `elefantolib_fastapi-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 packages = \
 ['elefantolib_fastapi']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['elefantolib>=0.10.1,<0.11.0',
+['elefantolib>=0.11.0,<0.12.0',
  'fastapi>=0.95.1,<0.96.0',
  'redis>=4.5.5,<5.0.0']
 
 setup_kwargs = {
     'name': 'elefantolib-fastapi',
-    'version': '0.2.3',
+    'version': '0.2.4',
     'description': '',
     'long_description': '## Elefantolib for FastAPI\n\n> **_NOTE:_**  Only for this library developers. After clone this repository you should run command:\n> \n\n ```console \ngit config core.hooksPath .githooks\n```\n\n\n## Installation\n\n<div class="termy">\n\n```console\npoetry add elefantolib-fastapi\n```\n</div>\n\n## Example\n\n### Prepare\n\n* Add environmental variables\n\n```\nSECRET=\nALGORITHM=\nISSUER=\n```\n* Defaults:\n    \n    - SECRET - not set, this is required\n    - ALGORITHM=HS256\n    - ISSUER=Consumer\n\n### Create it\n\n* Create a file `main.py` with:\n\n```Python\nfrom elefantolib_fastapi.requests import Request\nfrom elefantolib_fastapi.routes import APIRoute\n\nfrom fastapi import FastAPI\n\napp = FastAPI()\n\napp.router.route_class = APIRoute\n\n\n@app.get(\'/\')\ndef index(request: Request):\n    # TODO something\n    response = request.pfm.services.some_service_name.get(\'path-to-endpoint\')\n    return response\n\n```',
     'author': 'gglassota',
     'author_email': 'gglassota2@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `elefantolib_fastapi-0.2.3/PKG-INFO` & `elefantolib_fastapi-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: elefantolib-fastapi
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 Author: gglassota
 Author-email: gglassota2@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: elefantolib (>=0.10.1,<0.11.0)
+Requires-Dist: elefantolib (>=0.11.0,<0.12.0)
 Requires-Dist: fastapi (>=0.95.1,<0.96.0)
 Requires-Dist: redis (>=4.5.5,<5.0.0)
 Description-Content-Type: text/markdown
 
 ## Elefantolib for FastAPI
 
 > **_NOTE:_**  Only for this library developers. After clone this repository you should run command:
```

