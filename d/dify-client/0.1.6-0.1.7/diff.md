# Comparing `tmp/dify-client-0.1.6.tar.gz` & `tmp/dify-client-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dify-client-0.1.6.tar", last modified: Sun May 14 09:08:27 2023, max compression
+gzip compressed data, was "dify-client-0.1.7.tar", last modified: Sun May 14 09:09:33 2023, max compression
```

## Comparing `dify-client-0.1.6.tar` & `dify-client-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 johnwang   (501) staff       (20)        0 2023-05-14 09:08:27.907499 dify-client-0.1.6/
--rw-r--r--   0 johnwang   (501) staff       (20)     1067 2023-05-14 08:36:41.000000 dify-client-0.1.6/LICENSE
--rw-r--r--   0 johnwang   (501) staff       (20)       34 2023-05-14 08:23:26.000000 dify-client-0.1.6/MANIFEST.in
--rw-r--r--   0 johnwang   (501) staff       (20)     2955 2023-05-14 09:08:27.907227 dify-client-0.1.6/PKG-INFO
--rw-r--r--   0 johnwang   (501) staff       (20)     2465 2023-05-14 09:07:25.000000 dify-client-0.1.6/README.md
-drwxr-xr-x   0 johnwang   (501) staff       (20)        0 2023-05-14 09:08:27.903701 dify-client-0.1.6/dify_client/
--rw-r--r--   0 johnwang   (501) staff       (20)       59 2023-05-14 08:23:26.000000 dify-client-0.1.6/dify_client/__init__.py
--rw-r--r--   0 johnwang   (501) staff       (20)     2656 2023-05-14 09:07:25.000000 dify-client-0.1.6/dify_client/client.py
-drwxr-xr-x   0 johnwang   (501) staff       (20)        0 2023-05-14 09:08:27.906858 dify-client-0.1.6/dify_client.egg-info/
--rw-r--r--   0 johnwang   (501) staff       (20)     2955 2023-05-14 09:08:27.000000 dify-client-0.1.6/dify_client.egg-info/PKG-INFO
--rw-r--r--   0 johnwang   (501) staff       (20)      258 2023-05-14 09:08:27.000000 dify-client-0.1.6/dify_client.egg-info/SOURCES.txt
--rw-r--r--   0 johnwang   (501) staff       (20)        1 2023-05-14 09:08:27.000000 dify-client-0.1.6/dify_client.egg-info/dependency_links.txt
--rw-r--r--   0 johnwang   (501) staff       (20)        9 2023-05-14 09:08:27.000000 dify-client-0.1.6/dify_client.egg-info/requires.txt
--rw-r--r--   0 johnwang   (501) staff       (20)       12 2023-05-14 09:08:27.000000 dify-client-0.1.6/dify_client.egg-info/top_level.txt
--rw-r--r--   0 johnwang   (501) staff       (20)       38 2023-05-14 09:08:27.907573 dify-client-0.1.6/setup.cfg
--rw-r--r--   0 johnwang   (501) staff       (20)      805 2023-05-14 09:08:08.000000 dify-client-0.1.6/setup.py
+drwxr-xr-x   0 johnwang   (501) staff       (20)        0 2023-05-14 09:09:33.859919 dify-client-0.1.7/
+-rw-r--r--   0 johnwang   (501) staff       (20)     1067 2023-05-14 08:36:41.000000 dify-client-0.1.7/LICENSE
+-rw-r--r--   0 johnwang   (501) staff       (20)       34 2023-05-14 08:23:26.000000 dify-client-0.1.7/MANIFEST.in
+-rw-r--r--   0 johnwang   (501) staff       (20)     2955 2023-05-14 09:09:33.859576 dify-client-0.1.7/PKG-INFO
+-rw-r--r--   0 johnwang   (501) staff       (20)     2465 2023-05-14 09:07:25.000000 dify-client-0.1.7/README.md
+drwxr-xr-x   0 johnwang   (501) staff       (20)        0 2023-05-14 09:09:33.857084 dify-client-0.1.7/dify_client/
+-rw-r--r--   0 johnwang   (501) staff       (20)       59 2023-05-14 08:23:26.000000 dify-client-0.1.7/dify_client/__init__.py
+-rw-r--r--   0 johnwang   (501) staff       (20)     2655 2023-05-14 09:09:22.000000 dify-client-0.1.7/dify_client/client.py
+drwxr-xr-x   0 johnwang   (501) staff       (20)        0 2023-05-14 09:09:33.859176 dify-client-0.1.7/dify_client.egg-info/
+-rw-r--r--   0 johnwang   (501) staff       (20)     2955 2023-05-14 09:09:33.000000 dify-client-0.1.7/dify_client.egg-info/PKG-INFO
+-rw-r--r--   0 johnwang   (501) staff       (20)      258 2023-05-14 09:09:33.000000 dify-client-0.1.7/dify_client.egg-info/SOURCES.txt
+-rw-r--r--   0 johnwang   (501) staff       (20)        1 2023-05-14 09:09:33.000000 dify-client-0.1.7/dify_client.egg-info/dependency_links.txt
+-rw-r--r--   0 johnwang   (501) staff       (20)        9 2023-05-14 09:09:33.000000 dify-client-0.1.7/dify_client.egg-info/requires.txt
+-rw-r--r--   0 johnwang   (501) staff       (20)       12 2023-05-14 09:09:33.000000 dify-client-0.1.7/dify_client.egg-info/top_level.txt
+-rw-r--r--   0 johnwang   (501) staff       (20)       38 2023-05-14 09:09:33.860033 dify-client-0.1.7/setup.cfg
+-rw-r--r--   0 johnwang   (501) staff       (20)      805 2023-05-14 09:09:29.000000 dify-client-0.1.7/setup.py
```

### Comparing `dify-client-0.1.6/LICENSE` & `dify-client-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dify-client-0.1.6/PKG-INFO` & `dify-client-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dify-client
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package for interacting with the Dify Service-API
 Home-page: https://github.com/langgenius/dify
 Author: Dify
 Author-email: hello@dify.ai
 License: MIT
 Keywords: dify nlp ai language-processing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dify-client-0.1.6/README.md` & `dify-client-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `dify-client-0.1.6/dify_client/client.py` & `dify-client-0.1.7/dify_client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,8 +67,8 @@
 
     def get_conversations(self, user, first_id=None, limit=None, pinned=None):
         params = {"user": user, "first_id": first_id, "limit": limit, "pinned": pinned}
         return self._send_request("GET", "/conversations", params=params)
 
     def rename_conversation(self, conversation_id, name, user):
         data = {"name": name, "user": user}
-        return self._send_request("PATCH", f"/conversations/{conversation_id}/name", data)
+        return self._send_request("POST", f"/conversations/{conversation_id}/name", data)
```

### Comparing `dify-client-0.1.6/dify_client.egg-info/PKG-INFO` & `dify-client-0.1.7/dify_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dify-client
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package for interacting with the Dify Service-API
 Home-page: https://github.com/langgenius/dify
 Author: Dify
 Author-email: hello@dify.ai
 License: MIT
 Keywords: dify nlp ai language-processing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dify-client-0.1.6/setup.py` & `dify-client-0.1.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="dify-client",
-    version="0.1.6",
+    version="0.1.7",
     author="Dify",
     author_email="hello@dify.ai",
     description="A package for interacting with the Dify Service-API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/langgenius/dify",
     license='MIT',
```

