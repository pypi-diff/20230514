# Comparing `tmp/xhs_2_album-0.0.1.tar.gz` & `tmp/xhs_2_album-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xhs_2_album-0.0.1.tar", last modified: Sat May 13 02:05:49 2023, max compression
+gzip compressed data, was "xhs_2_album-0.0.2.tar", last modified: Sat May 13 23:48:27 2023, max compression
```

## Comparing `xhs_2_album-0.0.1.tar` & `xhs_2_album-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-13 02:05:49.000000 xhs_2_album-0.0.1/
--rw-r--r--   0 user       (501) staff       (20)     1071 2023-05-12 13:42:34.000000 xhs_2_album-0.0.1/LICENSE
--rw-r--r--   0 user       (501) staff       (20)      709 2023-05-13 02:05:49.000000 xhs_2_album-0.0.1/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      213 2023-05-12 13:49:56.000000 xhs_2_album-0.0.1/README.md
--rw-r--r--   0 user       (501) staff       (20)       38 2023-05-13 02:05:49.000000 xhs_2_album-0.0.1/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      766 2023-05-12 14:00:51.000000 xhs_2_album-0.0.1/setup.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-13 02:05:49.000000 xhs_2_album-0.0.1/xhs_2_album/
--rw-r--r--   0 user       (501) staff       (20)     1811 2023-05-13 02:03:22.000000 xhs_2_album-0.0.1/xhs_2_album/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-13 02:05:49.000000 xhs_2_album-0.0.1/xhs_2_album.egg-info/
--rw-r--r--   0 user       (501) staff       (20)      709 2023-05-13 02:05:49.000000 xhs_2_album-0.0.1/xhs_2_album.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      224 2023-05-13 02:05:49.000000 xhs_2_album-0.0.1/xhs_2_album.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-05-13 02:05:49.000000 xhs_2_album-0.0.1/xhs_2_album.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       29 2023-05-13 02:05:49.000000 xhs_2_album-0.0.1/xhs_2_album.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)       12 2023-05-13 02:05:49.000000 xhs_2_album-0.0.1/xhs_2_album.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-13 23:48:27.000000 xhs_2_album-0.0.2/
+-rw-r--r--   0 user       (501) staff       (20)     1071 2023-05-12 13:42:34.000000 xhs_2_album-0.0.2/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)      709 2023-05-13 23:48:27.000000 xhs_2_album-0.0.2/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      213 2023-05-12 13:49:56.000000 xhs_2_album-0.0.2/README.md
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-05-13 23:48:27.000000 xhs_2_album-0.0.2/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      766 2023-05-13 23:48:25.000000 xhs_2_album-0.0.2/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-13 23:48:27.000000 xhs_2_album-0.0.2/xhs_2_album/
+-rw-r--r--   0 user       (501) staff       (20)     1727 2023-05-13 23:48:18.000000 xhs_2_album-0.0.2/xhs_2_album/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-13 23:48:27.000000 xhs_2_album-0.0.2/xhs_2_album.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)      709 2023-05-13 23:48:27.000000 xhs_2_album-0.0.2/xhs_2_album.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      224 2023-05-13 23:48:27.000000 xhs_2_album-0.0.2/xhs_2_album.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-13 23:48:27.000000 xhs_2_album-0.0.2/xhs_2_album.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       29 2023-05-13 23:48:27.000000 xhs_2_album-0.0.2/xhs_2_album.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)       12 2023-05-13 23:48:27.000000 xhs_2_album-0.0.2/xhs_2_album.egg-info/top_level.txt
```

### Comparing `xhs_2_album-0.0.1/LICENSE` & `xhs_2_album-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xhs_2_album-0.0.1/PKG-INFO` & `xhs_2_album-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhs_2_album
-Version: 0.0.1
+Version: 0.0.2
 Summary: Return photo list and caption (markdown format) from xhs.
 Home-page: https://github.com/gaoyunzhi/xhs_2_album
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `xhs_2_album-0.0.1/setup.py` & `xhs_2_album-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="xhs_2_album",
-    version="0.0.1",
+    version="0.0.2",
     author="Yunzhi Gao",
     author_email="gaoyunzhi@gmail.com",
     description="Return photo list and caption (markdown format) from xhs.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gaoyunzhi/xhs_2_album",
     packages=setuptools.find_packages(),
```

### Comparing `xhs_2_album-0.0.1/xhs_2_album/__init__.py` & `xhs_2_album-0.0.2/xhs_2_album/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 
 from telegram_util import AlbumResult as Result
 from bs4 import BeautifulSoup
 import re
 import cached_url
 import yaml
 import time
-with open('credential') as f:
-    credential = yaml.load(f, Loader=yaml.FullLoader)
 
 def formatUrl(url):
     if url.startswith("http://xhslink"):
         json = cached_url.get('http://api.dwzjh.com/api/reduction?url=' + url, force_cache=True)
         json = yaml.load(json, Loader=yaml.FullLoader)
         url = json.get('longurl')
         url = url.split('?')[0]
```

### Comparing `xhs_2_album-0.0.1/xhs_2_album.egg-info/PKG-INFO` & `xhs_2_album-0.0.2/xhs_2_album.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhs-2-album
-Version: 0.0.1
+Version: 0.0.2
 Summary: Return photo list and caption (markdown format) from xhs.
 Home-page: https://github.com/gaoyunzhi/xhs_2_album
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

