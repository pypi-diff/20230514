# Comparing `tmp/ytspider-0.0.0.4.tar.gz` & `tmp/ytspider-0.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytspider-0.0.0.4.tar", last modified: Sun May  7 13:53:08 2023, max compression
+gzip compressed data, was "ytspider-0.0.0.5.tar", last modified: Sun May 14 13:29:07 2023, max compression
```

## Comparing `ytspider-0.0.0.4.tar` & `ytspider-0.0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 13:53:08.211298 ytspider-0.0.0.4/
--rw-rw-rw-   0        0        0      377 2023-05-07 13:53:08.211298 ytspider-0.0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1859 2023-04-30 18:25:19.000000 ytspider-0.0.0.4/README.md
--rw-rw-rw-   0        0        0      115 2023-05-07 13:53:08.212298 ytspider-0.0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      641 2023-05-07 13:52:59.000000 ytspider-0.0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-07 13:53:08.158320 ytspider-0.0.0.4/src/
--rw-rw-rw-   0        0        0       45 2023-04-30 20:45:34.000000 ytspider-0.0.0.4/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-07 13:53:08.194387 ytspider-0.0.0.4/src/utils/
--rw-rw-rw-   0        0        0        0 2023-04-30 20:26:12.000000 ytspider-0.0.0.4/src/utils/__init__.py
--rw-rw-rw-   0        0        0     1969 2023-04-30 11:28:54.000000 ytspider-0.0.0.4/src/utils/client.py
--rw-rw-rw-   0        0        0     1670 2023-05-01 20:14:19.000000 ytspider-0.0.0.4/src/utils/context.py
--rw-rw-rw-   0        0        0     2938 2023-05-01 20:13:59.000000 ytspider-0.0.0.4/src/utils/decorator.py
--rw-rw-rw-   0        0        0     7942 2023-05-07 13:49:20.000000 ytspider-0.0.0.4/src/utils/handler.py
--rw-rw-rw-   0        0        0      707 2023-04-30 11:29:20.000000 ytspider-0.0.0.4/src/utils/playback_context.py
--rw-rw-rw-   0        0        0     2609 2023-05-07 13:23:21.000000 ytspider-0.0.0.4/src/utils/request.py
--rw-rw-rw-   0        0        0      951 2023-04-30 11:18:54.000000 ytspider-0.0.0.4/src/utils/signals_info.py
--rw-rw-rw-   0        0        0     7453 2023-05-07 13:52:15.000000 ytspider-0.0.0.4/src/ytspider.py
-drwxrwxrwx   0        0        0        0 2023-05-07 13:53:08.208758 ytspider-0.0.0.4/ytspider.egg-info/
--rw-rw-rw-   0        0        0      377 2023-05-07 13:53:08.000000 ytspider-0.0.0.4/ytspider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2023-05-07 13:53:08.000000 ytspider-0.0.0.4/ytspider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 13:53:08.000000 ytspider-0.0.0.4/ytspider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-07 13:53:08.000000 ytspider-0.0.0.4/ytspider.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-07 13:53:08.000000 ytspider-0.0.0.4/ytspider.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 13:29:07.507269 ytspider-0.0.0.5/
+-rw-rw-rw-   0        0        0      377 2023-05-14 13:29:07.507269 ytspider-0.0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1859 2023-04-30 18:25:19.000000 ytspider-0.0.0.5/README.md
+-rw-rw-rw-   0        0        0      115 2023-05-14 13:29:07.511525 ytspider-0.0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      641 2023-05-14 13:28:59.000000 ytspider-0.0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 13:29:07.410039 ytspider-0.0.0.5/src/
+-rw-rw-rw-   0        0        0       45 2023-04-30 20:45:34.000000 ytspider-0.0.0.5/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 13:29:07.460261 ytspider-0.0.0.5/src/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-30 20:26:12.000000 ytspider-0.0.0.5/src/utils/__init__.py
+-rw-rw-rw-   0        0        0     1969 2023-04-30 11:28:54.000000 ytspider-0.0.0.5/src/utils/client.py
+-rw-rw-rw-   0        0        0     1670 2023-05-01 20:14:19.000000 ytspider-0.0.0.5/src/utils/context.py
+-rw-rw-rw-   0        0        0     2938 2023-05-01 20:13:59.000000 ytspider-0.0.0.5/src/utils/decorator.py
+-rw-rw-rw-   0        0        0     7969 2023-05-14 13:27:20.000000 ytspider-0.0.0.5/src/utils/handler.py
+-rw-rw-rw-   0        0        0      707 2023-04-30 11:29:20.000000 ytspider-0.0.0.5/src/utils/playback_context.py
+-rw-rw-rw-   0        0        0     2609 2023-05-07 13:23:21.000000 ytspider-0.0.0.5/src/utils/request.py
+-rw-rw-rw-   0        0        0      951 2023-04-30 11:18:54.000000 ytspider-0.0.0.5/src/utils/signals_info.py
+-rw-rw-rw-   0        0        0     7453 2023-05-07 13:52:15.000000 ytspider-0.0.0.5/src/ytspider.py
+drwxrwxrwx   0        0        0        0 2023-05-14 13:29:07.503258 ytspider-0.0.0.5/ytspider.egg-info/
+-rw-rw-rw-   0        0        0      377 2023-05-14 13:29:07.000000 ytspider-0.0.0.5/ytspider.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2023-05-14 13:29:07.000000 ytspider-0.0.0.5/ytspider.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 13:29:07.000000 ytspider-0.0.0.5/ytspider.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-14 13:29:07.000000 ytspider-0.0.0.5/ytspider.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-14 13:29:07.000000 ytspider-0.0.0.5/ytspider.egg-info/top_level.txt
```

### Comparing `ytspider-0.0.0.4/README.md` & `ytspider-0.0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ytspider-0.0.0.4/setup.py` & `ytspider-0.0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='ytspider',
     description="YouTube scraper, videos, channels, playlists, comments and transcriptions",
-    version='0.0.0.4',
+    version='0.0.0.5',
     license='MIT',
     author="Zeyad Khalid",
     maintainer_email='zeyad.khalid@must.edu.eg',
     author_email='zeyadpro99@gmail.com',
     package_dir={"ytspider":"src"},
     packages=find_packages(),#["ytspider","ytspider.utils"],
     py_modules=["ytspider.py"],
```

### Comparing `ytspider-0.0.0.4/src/utils/client.py` & `ytspider-0.0.0.5/src/utils/client.py`

 * *Files identical despite different names*

### Comparing `ytspider-0.0.0.4/src/utils/context.py` & `ytspider-0.0.0.5/src/utils/context.py`

 * *Files identical despite different names*

### Comparing `ytspider-0.0.0.4/src/utils/decorator.py` & `ytspider-0.0.0.5/src/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `ytspider-0.0.0.4/src/utils/handler.py` & `ytspider-0.0.0.5/src/utils/handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         self.request.updateContextState(itemId, additional={"continuation": ""})
         firstTime = True
         token = ""
         all_comments = []
         while token is not None and len(all_comments) < self.n_comments:
             self.request.updateContextState(additional={"continuation": token})
             result = self.request.send(self.url, method="POST")
+            comments = []
             if firstTime:
                 # Try get token for comment retrieval
                 try:
                     token = result["contents"]["twoColumnWatchNextResults"]["results"]["results"]["contents"][3]["itemSectionRenderer"]["contents"][0]["continuationItemRenderer"]["continuationEndpoint"]["continuationCommand"]["token"]
                     firstTime = False
                 # Couldn't get token for comment retrieval
                 except Exception as e:
```

### Comparing `ytspider-0.0.0.4/src/utils/playback_context.py` & `ytspider-0.0.0.5/src/utils/playback_context.py`

 * *Files identical despite different names*

### Comparing `ytspider-0.0.0.4/src/utils/request.py` & `ytspider-0.0.0.5/src/utils/request.py`

 * *Files identical despite different names*

### Comparing `ytspider-0.0.0.4/src/utils/signals_info.py` & `ytspider-0.0.0.5/src/utils/signals_info.py`

 * *Files identical despite different names*

### Comparing `ytspider-0.0.0.4/src/ytspider.py` & `ytspider-0.0.0.5/src/ytspider.py`

 * *Files identical despite different names*

