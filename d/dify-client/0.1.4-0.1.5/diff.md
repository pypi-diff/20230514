# Comparing `tmp/dify-client-0.1.4.tar.gz` & `tmp/dify-client-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dify-client-0.1.4.tar", last modified: Sun May 14 08:35:53 2023, max compression
+gzip compressed data, was "dify-client-0.1.5.tar", last modified: Sun May 14 08:38:27 2023, max compression
```

## Comparing `dify-client-0.1.4.tar` & `dify-client-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 johnwang   (501) staff       (20)        0 2023-05-14 08:35:53.289554 dify-client-0.1.4/
--rw-r--r--   0 johnwang   (501) staff       (20)     1061 2023-05-14 08:23:26.000000 dify-client-0.1.4/LICENSE
--rw-r--r--   0 johnwang   (501) staff       (20)       34 2023-05-14 08:23:26.000000 dify-client-0.1.4/MANIFEST.in
--rw-r--r--   0 johnwang   (501) staff       (20)     1716 2023-05-14 08:35:53.289109 dify-client-0.1.4/PKG-INFO
--rw-r--r--   0 johnwang   (501) staff       (20)     1226 2023-05-14 08:23:26.000000 dify-client-0.1.4/README.md
-drwxr-xr-x   0 johnwang   (501) staff       (20)        0 2023-05-14 08:35:53.286572 dify-client-0.1.4/dify_client/
--rw-r--r--   0 johnwang   (501) staff       (20)       59 2023-05-14 08:23:26.000000 dify-client-0.1.4/dify_client/__init__.py
--rw-r--r--   0 johnwang   (501) staff       (20)     2651 2023-05-14 08:23:26.000000 dify-client-0.1.4/dify_client/client.py
-drwxr-xr-x   0 johnwang   (501) staff       (20)        0 2023-05-14 08:35:53.288432 dify-client-0.1.4/dify_client.egg-info/
--rw-r--r--   0 johnwang   (501) staff       (20)     1716 2023-05-14 08:35:53.000000 dify-client-0.1.4/dify_client.egg-info/PKG-INFO
--rw-r--r--   0 johnwang   (501) staff       (20)      258 2023-05-14 08:35:53.000000 dify-client-0.1.4/dify_client.egg-info/SOURCES.txt
--rw-r--r--   0 johnwang   (501) staff       (20)        1 2023-05-14 08:35:53.000000 dify-client-0.1.4/dify_client.egg-info/dependency_links.txt
--rw-r--r--   0 johnwang   (501) staff       (20)        9 2023-05-14 08:35:53.000000 dify-client-0.1.4/dify_client.egg-info/requires.txt
--rw-r--r--   0 johnwang   (501) staff       (20)       12 2023-05-14 08:35:53.000000 dify-client-0.1.4/dify_client.egg-info/top_level.txt
--rw-r--r--   0 johnwang   (501) staff       (20)       38 2023-05-14 08:35:53.289671 dify-client-0.1.4/setup.cfg
--rw-r--r--   0 johnwang   (501) staff       (20)      805 2023-05-14 08:35:48.000000 dify-client-0.1.4/setup.py
+drwxr-xr-x   0 johnwang   (501) staff       (20)        0 2023-05-14 08:38:27.385939 dify-client-0.1.5/
+-rw-r--r--   0 johnwang   (501) staff       (20)     1067 2023-05-14 08:36:41.000000 dify-client-0.1.5/LICENSE
+-rw-r--r--   0 johnwang   (501) staff       (20)       34 2023-05-14 08:23:26.000000 dify-client-0.1.5/MANIFEST.in
+-rw-r--r--   0 johnwang   (501) staff       (20)     1716 2023-05-14 08:38:27.385652 dify-client-0.1.5/PKG-INFO
+-rw-r--r--   0 johnwang   (501) staff       (20)     1226 2023-05-14 08:23:26.000000 dify-client-0.1.5/README.md
+drwxr-xr-x   0 johnwang   (501) staff       (20)        0 2023-05-14 08:38:27.383504 dify-client-0.1.5/dify_client/
+-rw-r--r--   0 johnwang   (501) staff       (20)       59 2023-05-14 08:23:26.000000 dify-client-0.1.5/dify_client/__init__.py
+-rw-r--r--   0 johnwang   (501) staff       (20)     2651 2023-05-14 08:23:26.000000 dify-client-0.1.5/dify_client/client.py
+drwxr-xr-x   0 johnwang   (501) staff       (20)        0 2023-05-14 08:38:27.385249 dify-client-0.1.5/dify_client.egg-info/
+-rw-r--r--   0 johnwang   (501) staff       (20)     1716 2023-05-14 08:38:27.000000 dify-client-0.1.5/dify_client.egg-info/PKG-INFO
+-rw-r--r--   0 johnwang   (501) staff       (20)      258 2023-05-14 08:38:27.000000 dify-client-0.1.5/dify_client.egg-info/SOURCES.txt
+-rw-r--r--   0 johnwang   (501) staff       (20)        1 2023-05-14 08:38:27.000000 dify-client-0.1.5/dify_client.egg-info/dependency_links.txt
+-rw-r--r--   0 johnwang   (501) staff       (20)        9 2023-05-14 08:38:27.000000 dify-client-0.1.5/dify_client.egg-info/requires.txt
+-rw-r--r--   0 johnwang   (501) staff       (20)       12 2023-05-14 08:38:27.000000 dify-client-0.1.5/dify_client.egg-info/top_level.txt
+-rw-r--r--   0 johnwang   (501) staff       (20)       38 2023-05-14 08:38:27.386021 dify-client-0.1.5/setup.cfg
+-rw-r--r--   0 johnwang   (501) staff       (20)      805 2023-05-14 08:38:22.000000 dify-client-0.1.5/setup.py
```

### Comparing `dify-client-0.1.4/LICENSE` & `dify-client-0.1.5/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Dify
+Copyright (c) 2023 LangGenius
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `dify-client-0.1.4/PKG-INFO` & `dify-client-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dify-client
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package for interacting with the Dify Service-API
 Home-page: https://github.com/langgenius/dify
 Author: Dify
 Author-email: hello@dify.ai
 License: MIT
 Keywords: dify nlp ai language-processing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dify-client-0.1.4/README.md` & `dify-client-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `dify-client-0.1.4/dify_client/client.py` & `dify-client-0.1.5/dify_client/client.py`

 * *Files identical despite different names*

### Comparing `dify-client-0.1.4/dify_client.egg-info/PKG-INFO` & `dify-client-0.1.5/dify_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dify-client
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package for interacting with the Dify Service-API
 Home-page: https://github.com/langgenius/dify
 Author: Dify
 Author-email: hello@dify.ai
 License: MIT
 Keywords: dify nlp ai language-processing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dify-client-0.1.4/setup.py` & `dify-client-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="dify-client",
-    version="0.1.4",
+    version="0.1.5",
     author="Dify",
     author_email="hello@dify.ai",
     description="A package for interacting with the Dify Service-API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/langgenius/dify",
     license='MIT',
```

