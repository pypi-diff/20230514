# Comparing `tmp/smoloki-0.0.8.tar.gz` & `tmp/smoloki-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smoloki-0.0.8.tar", last modified: Thu May 11 17:24:45 2023, max compression
+gzip compressed data, was "smoloki-0.0.9.tar", last modified: Thu May 11 17:42:33 2023, max compression
```

## Comparing `smoloki-0.0.8.tar` & `smoloki-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:24:45.730966 smoloki-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-11 17:24:45.730966 smoloki-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-11 17:24:30.000000 smoloki-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 17:24:45.730966 smoloki-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-11 17:24:30.000000 smoloki-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:24:45.726966 smoloki-0.0.8/smoloki/
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-05-11 17:24:30.000000 smoloki-0.0.8/smoloki/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-11 17:24:30.000000 smoloki-0.0.8/smoloki/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:24:45.730966 smoloki-0.0.8/smoloki/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-11 17:24:30.000000 smoloki-0.0.8/smoloki/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-11 17:24:30.000000 smoloki-0.0.8/smoloki/wrappers/nodejs.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:24:45.730966 smoloki-0.0.8/smoloki.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-11 17:24:45.000000 smoloki-0.0.8/smoloki.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-11 17:24:45.000000 smoloki-0.0.8/smoloki.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 17:24:45.000000 smoloki-0.0.8/smoloki.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 17:24:45.000000 smoloki-0.0.8/smoloki.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-11 17:24:45.000000 smoloki-0.0.8/smoloki.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 17:24:45.000000 smoloki-0.0.8/smoloki.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:24:45.730966 smoloki-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-11 17:24:30.000000 smoloki-0.0.8/tests/test_logfmt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-11 17:24:30.000000 smoloki-0.0.8/tests/test_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:42:33.051644 smoloki-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-11 17:42:33.051644 smoloki-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-11 17:42:16.000000 smoloki-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 17:42:33.051644 smoloki-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-11 17:42:16.000000 smoloki-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:42:33.047644 smoloki-0.0.9/smoloki/
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-05-11 17:42:16.000000 smoloki-0.0.9/smoloki/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-11 17:42:16.000000 smoloki-0.0.9/smoloki/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:42:33.051644 smoloki-0.0.9/smoloki.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-11 17:42:33.000000 smoloki-0.0.9/smoloki.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-11 17:42:33.000000 smoloki-0.0.9/smoloki.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 17:42:33.000000 smoloki-0.0.9/smoloki.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-11 17:42:33.000000 smoloki-0.0.9/smoloki.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-11 17:42:33.000000 smoloki-0.0.9/smoloki.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 17:42:33.000000 smoloki-0.0.9/smoloki.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:42:33.051644 smoloki-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-11 17:42:16.000000 smoloki-0.0.9/tests/test_logfmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-11 17:42:16.000000 smoloki-0.0.9/tests/test_requests.py
```

### Comparing `smoloki-0.0.8/PKG-INFO` & `smoloki-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smoloki
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tiny library to push logs to `Grafana Loki` in `logfmt` format.
 Home-page: https://github.com/michaelkryukov/smoloki
 Author: Michael Krukov
 Author-email: krukov.michael@ya.ru
 Keywords: library,loki
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -16,32 +16,14 @@
 
 # smoloki
 
 [![PyPI version](https://badge.fury.io/py/smoloki.svg)](https://badge.fury.io/py/smoloki)
 
 Tiny library to push logs to `Grafana Loki` in `logfmt` format.
 
-```py
-import smoloki
-
-
-async def as_request_completed():
-    await smoloki.push(
-        {'service': 'web'},
-        {'level': 'info', 'event': 'request_completed'},
-    )
-
-
-def as_request_completed():
-    smoloki.push_sync(
-        {'service': 'web'},
-        {'level': 'info', 'event': 'request_completed'},
-    )
-```
-
 ## CLI
 
 ```text
 usage: smoloki [-h] [-b BASE_ENDPOINT] labels information
 
 cli for pushing to loki
 
@@ -50,31 +32,42 @@
   information       json-encoded string with information
 
 options:
   -h, --help        show this help message and exit
   -b BASE_ENDPOINT  base address of loki server
 ```
 
-## Usage in NodeJS
+## Usage in Python
+
+```py
+import smoloki
+
+
+async def as_request_completed():
+    await smoloki.push(
+        {'service': 'web'},
+        {'level': 'info', 'event': 'request_completed'},
+    )
 
-Install simple wrapper for installed python module:
 
-```bash
-# In your project's folder
-smoloki-wrappers --install-wrapper-for-nodejs 'node_modules/'
+def as_request_completed():
+    smoloki.push_sync(
+        {'service': 'web'},
+        {'level': 'info', 'event': 'request_completed'},
+    )
 ```
 
-Usage is along this lines:
+## Usage in NodeJS (not yet implemented)
 
 ```js
 const smoloki = require('smoloki');
 
-// This is an async function executing CLI from previous
-// chapter under the hood.
-smoloki.push({ service: 'web' }, { level: 'info', event: 'request_completed' });
+async function as_request_completed() {
+    await smoloki.push({ service: 'web' }, { level: 'info', event: 'request_completed' });
+}
 ```
 
 ## Implementation details
 
 - Calls to `push` method will never throw. Any exception will just be
     logged using `logging`.
 - Keys in labels and information must be strings.
```

### Comparing `smoloki-0.0.8/README.md` & `smoloki-0.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,13 @@
 # smoloki
 
 [![PyPI version](https://badge.fury.io/py/smoloki.svg)](https://badge.fury.io/py/smoloki)
 
 Tiny library to push logs to `Grafana Loki` in `logfmt` format.
 
-```py
-import smoloki
-
-
-async def as_request_completed():
-    await smoloki.push(
-        {'service': 'web'},
-        {'level': 'info', 'event': 'request_completed'},
-    )
-
-
-def as_request_completed():
-    smoloki.push_sync(
-        {'service': 'web'},
-        {'level': 'info', 'event': 'request_completed'},
-    )
-```
-
 ## CLI
 
 ```text
 usage: smoloki [-h] [-b BASE_ENDPOINT] labels information
 
 cli for pushing to loki
 
@@ -34,31 +16,42 @@
   information       json-encoded string with information
 
 options:
   -h, --help        show this help message and exit
   -b BASE_ENDPOINT  base address of loki server
 ```
 
-## Usage in NodeJS
+## Usage in Python
+
+```py
+import smoloki
+
+
+async def as_request_completed():
+    await smoloki.push(
+        {'service': 'web'},
+        {'level': 'info', 'event': 'request_completed'},
+    )
 
-Install simple wrapper for installed python module:
 
-```bash
-# In your project's folder
-smoloki-wrappers --install-wrapper-for-nodejs 'node_modules/'
+def as_request_completed():
+    smoloki.push_sync(
+        {'service': 'web'},
+        {'level': 'info', 'event': 'request_completed'},
+    )
 ```
 
-Usage is along this lines:
+## Usage in NodeJS (not yet implemented)
 
 ```js
 const smoloki = require('smoloki');
 
-// This is an async function executing CLI from previous
-// chapter under the hood.
-smoloki.push({ service: 'web' }, { level: 'info', event: 'request_completed' });
+async function as_request_completed() {
+    await smoloki.push({ service: 'web' }, { level: 'info', event: 'request_completed' });
+}
 ```
 
 ## Implementation details
 
 - Calls to `push` method will never throw. Any exception will just be
     logged using `logging`.
 - Keys in labels and information must be strings.
```

### Comparing `smoloki-0.0.8/setup.py` & `smoloki-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,18 +26,16 @@
     packages=setuptools.find_packages(),
     install_requires=[
         "aiohttp~=3.8.3",
     ],
     entry_points={
         "console_scripts": [
             "smoloki = smoloki.__main__:main",
-            "smoloki-wrappers = smoloki.wrappers:main",
         ],
     },
-    package_data={"smoloki": ["wrappers/*.js"]},
     python_requires=">=3.7",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
```

### Comparing `smoloki-0.0.8/smoloki/__init__.py` & `smoloki-0.0.9/smoloki/__init__.py`

 * *Files identical despite different names*

### Comparing `smoloki-0.0.8/smoloki/__main__.py` & `smoloki-0.0.9/smoloki/__main__.py`

 * *Files identical despite different names*

### Comparing `smoloki-0.0.8/smoloki.egg-info/PKG-INFO` & `smoloki-0.0.9/smoloki.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smoloki
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tiny library to push logs to `Grafana Loki` in `logfmt` format.
 Home-page: https://github.com/michaelkryukov/smoloki
 Author: Michael Krukov
 Author-email: krukov.michael@ya.ru
 Keywords: library,loki
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -16,32 +16,14 @@
 
 # smoloki
 
 [![PyPI version](https://badge.fury.io/py/smoloki.svg)](https://badge.fury.io/py/smoloki)
 
 Tiny library to push logs to `Grafana Loki` in `logfmt` format.
 
-```py
-import smoloki
-
-
-async def as_request_completed():
-    await smoloki.push(
-        {'service': 'web'},
-        {'level': 'info', 'event': 'request_completed'},
-    )
-
-
-def as_request_completed():
-    smoloki.push_sync(
-        {'service': 'web'},
-        {'level': 'info', 'event': 'request_completed'},
-    )
-```
-
 ## CLI
 
 ```text
 usage: smoloki [-h] [-b BASE_ENDPOINT] labels information
 
 cli for pushing to loki
 
@@ -50,31 +32,42 @@
   information       json-encoded string with information
 
 options:
   -h, --help        show this help message and exit
   -b BASE_ENDPOINT  base address of loki server
 ```
 
-## Usage in NodeJS
+## Usage in Python
+
+```py
+import smoloki
+
+
+async def as_request_completed():
+    await smoloki.push(
+        {'service': 'web'},
+        {'level': 'info', 'event': 'request_completed'},
+    )
 
-Install simple wrapper for installed python module:
 
-```bash
-# In your project's folder
-smoloki-wrappers --install-wrapper-for-nodejs 'node_modules/'
+def as_request_completed():
+    smoloki.push_sync(
+        {'service': 'web'},
+        {'level': 'info', 'event': 'request_completed'},
+    )
 ```
 
-Usage is along this lines:
+## Usage in NodeJS (not yet implemented)
 
 ```js
 const smoloki = require('smoloki');
 
-// This is an async function executing CLI from previous
-// chapter under the hood.
-smoloki.push({ service: 'web' }, { level: 'info', event: 'request_completed' });
+async function as_request_completed() {
+    await smoloki.push({ service: 'web' }, { level: 'info', event: 'request_completed' });
+}
 ```
 
 ## Implementation details
 
 - Calls to `push` method will never throw. Any exception will just be
     logged using `logging`.
 - Keys in labels and information must be strings.
```

### Comparing `smoloki-0.0.8/tests/test_logfmt.py` & `smoloki-0.0.9/tests/test_logfmt.py`

 * *Files identical despite different names*

### Comparing `smoloki-0.0.8/tests/test_requests.py` & `smoloki-0.0.9/tests/test_requests.py`

 * *Files identical despite different names*

