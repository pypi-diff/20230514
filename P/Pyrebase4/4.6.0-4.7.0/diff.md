# Comparing `tmp/Pyrebase4-4.6.0.tar.gz` & `tmp/Pyrebase4-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pyrebase4-4.6.0.tar", last modified: Wed Nov 30 18:51:32 2022, max compression
+gzip compressed data, was "Pyrebase4-4.7.0.tar", last modified: Sun May 14 14:18:54 2023, max compression
```

## Comparing `Pyrebase4-4.6.0.tar` & `Pyrebase4-4.7.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxr-x   0 nhorvath  (1001) nhorvath  (1001)        0 2022-11-30 18:51:32.511210 Pyrebase4-4.6.0/
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)      412 2022-11-30 18:51:32.507210 Pyrebase4-4.6.0/PKG-INFO
-drwxrwxr-x   0 nhorvath  (1001) nhorvath  (1001)        0 2022-11-30 18:51:32.507210 Pyrebase4-4.6.0/Pyrebase4.egg-info/
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)      412 2022-11-30 18:51:32.000000 Pyrebase4-4.6.0/Pyrebase4.egg-info/PKG-INFO
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)      251 2022-11-30 18:51:32.000000 Pyrebase4-4.6.0/Pyrebase4.egg-info/SOURCES.txt
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)        1 2022-11-30 18:51:32.000000 Pyrebase4-4.6.0/Pyrebase4.egg-info/dependency_links.txt
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)      115 2022-11-30 18:51:32.000000 Pyrebase4-4.6.0/Pyrebase4.egg-info/requires.txt
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)        9 2022-11-30 18:51:32.000000 Pyrebase4-4.6.0/Pyrebase4.egg-info/top_level.txt
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)    13753 2022-11-30 18:49:25.000000 Pyrebase4-4.6.0/README.md
-drwxrwxr-x   0 nhorvath  (1001) nhorvath  (1001)        0 2022-11-30 18:51:32.507210 Pyrebase4-4.6.0/pyrebase/
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)       36 2022-11-30 18:49:25.000000 Pyrebase4-4.6.0/pyrebase/__init__.py
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)     5395 2022-11-30 18:49:25.000000 Pyrebase4-4.6.0/pyrebase/pyre_sseclient.py
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)    26225 2022-11-30 18:49:25.000000 Pyrebase4-4.6.0/pyrebase/pyrebase.py
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)       38 2022-11-30 18:51:32.511210 Pyrebase4-4.6.0/setup.cfg
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)      761 2022-11-30 18:50:30.000000 Pyrebase4-4.6.0/setup.py
+drwxrwxr-x   0 nhorvath  (1001) nhorvath  (1001)        0 2023-05-14 14:18:54.042466 Pyrebase4-4.7.0/
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)      412 2023-05-14 14:18:54.042466 Pyrebase4-4.7.0/PKG-INFO
+drwxrwxr-x   0 nhorvath  (1001) nhorvath  (1001)        0 2023-05-14 14:18:54.042466 Pyrebase4-4.7.0/Pyrebase4.egg-info/
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)      412 2023-05-14 14:18:54.000000 Pyrebase4-4.7.0/Pyrebase4.egg-info/PKG-INFO
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)      294 2023-05-14 14:18:54.000000 Pyrebase4-4.7.0/Pyrebase4.egg-info/SOURCES.txt
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)        1 2023-05-14 14:18:54.000000 Pyrebase4-4.7.0/Pyrebase4.egg-info/dependency_links.txt
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)      115 2023-05-14 14:18:54.000000 Pyrebase4-4.7.0/Pyrebase4.egg-info/requires.txt
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)        9 2023-05-14 14:18:54.000000 Pyrebase4-4.7.0/Pyrebase4.egg-info/top_level.txt
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)    13752 2023-05-14 14:05:14.000000 Pyrebase4-4.7.0/README.md
+drwxrwxr-x   0 nhorvath  (1001) nhorvath  (1001)        0 2023-05-14 14:18:54.042466 Pyrebase4-4.7.0/pyrebase/
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)       36 2022-11-30 18:49:25.000000 Pyrebase4-4.7.0/pyrebase/__init__.py
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)     5395 2022-11-30 18:49:25.000000 Pyrebase4-4.7.0/pyrebase/pyre_sseclient.py
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)    26616 2023-05-14 13:59:31.000000 Pyrebase4-4.7.0/pyrebase/pyrebase.py
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)       38 2023-05-14 14:18:54.042466 Pyrebase4-4.7.0/setup.cfg
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)      761 2023-05-14 14:18:28.000000 Pyrebase4-4.7.0/setup.py
+drwxrwxr-x   0 nhorvath  (1001) nhorvath  (1001)        0 2023-05-14 14:18:54.042466 Pyrebase4-4.7.0/tests/
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)     5247 2022-11-30 18:49:25.000000 Pyrebase4-4.7.0/tests/test_database.py
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)       95 2022-11-30 18:49:25.000000 Pyrebase4-4.7.0/tests/test_setup.py
```

### Comparing `Pyrebase4-4.6.0/README.md` & `Pyrebase4-4.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Pyrebase4
 
 A simple python wrapper for the [Firebase API](https://firebase.google.com).
 
 ## Installation
 
-```python
+```shell
 pip install pyrebase4
 ```
 
 ## Getting Started
 
 ### Python Version
```

### Comparing `Pyrebase4-4.6.0/pyrebase/pyre_sseclient.py` & `Pyrebase4-4.7.0/pyrebase/pyre_sseclient.py`

 * *Files identical despite different names*

### Comparing `Pyrebase4-4.6.0/pyrebase/pyrebase.py` & `Pyrebase4-4.7.0/pyrebase/pyrebase.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from .pyre_sseclient import SSEClient
 import threading
 import socket
 from oauth2client.service_account import ServiceAccountCredentials
 from gcloud import storage
 from requests.packages.urllib3.contrib.appengine import is_appengine_sandbox
 from requests_toolbelt.adapters import appengine
+from uuid import uuid4
 
 import python_jwt as jwt
 from Crypto.PublicKey import RSA
 import datetime
 
 
 def initialize_app(config):
@@ -450,15 +451,15 @@
             self.path += "/{}".format(new_path)
         else:
             if new_path.startswith("/"):
                 new_path = new_path[1:]
             self.path = new_path
         return self
 
-    def put(self, file, token=None):
+    def put(self, file, token=None, content_type=None):
         # reset path
         path = self.path
         self.path = None
         if isinstance(file, str):
             file_object = open(file, 'rb')
         else:
             file_object = file
@@ -466,18 +467,25 @@
         if token:
             headers = {"Authorization": "Firebase " + token}
             request_object = self.requests.post(request_ref, headers=headers, data=file_object)
             raise_detailed_error(request_object)
             return request_object.json()
         elif self.credentials:
             blob = self.bucket.blob(path)
+
+            # Add metadata to enable file previews in console
+            blob.metadata = {"firebaseStorageDownloadTokens": str(uuid4())}
             if isinstance(file, str):
                 return blob.upload_from_filename(filename=file)
             else:
-                return blob.upload_from_file(file_obj=file)
+                # If the file is not a string we need to patch the blob after upload to set the content type
+                blob.upload_from_string(file)
+                if content_type:
+                    blob.content_type = content_type
+                blob.patch()
         else:
             request_object = self.requests.post(request_ref, data=file_object)
             raise_detailed_error(request_object)
             return request_object.json()
 
     def delete(self, name, token):
         if self.credentials:
```

### Comparing `Pyrebase4-4.6.0/setup.py` & `Pyrebase4-4.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Pyrebase4',
-    version='4.6.0',
+    version='4.7.0',
     url='https://github.com/nhorvath/Pyrebase4',
     description='A simple python wrapper for the Firebase API with current deps',
     author='nhorvath',
     license='MIT',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

