# Comparing `tmp/freeGPT-1.1.tar.gz` & `tmp/freeGPT-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Ruu3f\Downloads\freeGPT\dist\.tmp-wfyzoejr\freeGPT-1.0.1.tar", last modified: Sat May  6 13:21:13 2023, max compression
+gzip compressed data, was "C:\Users\Ruu3f\Downloads\freeGPT\dist\.tmp-ww1yynb8\freeGPT-1.0.2.tar", last modified: Sun May 14 08:45:44 2023, max compression
```

## Comparing `freeGPT-1.1.tar` & `freeGPT-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 13:21:13.776693 freeGPT-1.0.1/
--rw-rw-rw-   0        0        0    35149 2023-05-06 10:58:49.000000 freeGPT-1.0.1/LICENSE.md
--rw-rw-rw-   0        0        0       98 2023-05-06 10:58:49.000000 freeGPT-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2180 2023-05-06 13:21:13.776693 freeGPT-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1119 2023-05-06 13:19:49.000000 freeGPT-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 13:21:13.761068 freeGPT-1.0.1/freeGPT/
--rw-rw-rw-   0        0        0      798 2023-05-06 13:08:01.000000 freeGPT-1.0.1/freeGPT/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:21:13.776693 freeGPT-1.0.1/freeGPT/gpt3/
--rw-rw-rw-   0        0        0     3972 2023-05-06 13:01:18.000000 freeGPT-1.0.1/freeGPT/gpt3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:21:13.776693 freeGPT-1.0.1/freeGPT/gpt4/
--rw-rw-rw-   0        0        0     6391 2023-05-06 13:10:38.000000 freeGPT-1.0.1/freeGPT/gpt4/__init__.py
--rw-rw-rw-   0        0        0      410 2023-05-06 13:11:05.000000 freeGPT-1.0.1/freeGPT/gpt4/typing.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:21:13.776693 freeGPT-1.0.1/freeGPT.egg-info/
--rw-rw-rw-   0        0        0     2180 2023-05-06 13:21:13.000000 freeGPT-1.0.1/freeGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-05-06 13:21:13.000000 freeGPT-1.0.1/freeGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 13:21:13.000000 freeGPT-1.0.1/freeGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 13:21:13.000000 freeGPT-1.0.1/freeGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-06 13:21:13.000000 freeGPT-1.0.1/freeGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 13:21:13.776693 freeGPT-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1434 2023-05-06 13:20:59.000000 freeGPT-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 08:45:44.211287 freeGPT-1.0.2/
+-rw-rw-rw-   0        0        0    35149 2023-05-13 18:23:11.000000 freeGPT-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       98 2023-05-13 18:23:11.000000 freeGPT-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3038 2023-05-14 08:45:44.210272 freeGPT-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1970 2023-05-13 18:23:11.000000 freeGPT-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 08:45:44.204167 freeGPT-1.0.2/freeGPT/
+-rw-rw-rw-   0        0        0      798 2023-05-14 08:45:23.000000 freeGPT-1.0.2/freeGPT/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 08:45:44.208272 freeGPT-1.0.2/freeGPT/gpt3/
+-rw-rw-rw-   0        0        0     3972 2023-05-13 18:23:11.000000 freeGPT-1.0.2/freeGPT/gpt3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 08:45:44.209271 freeGPT-1.0.2/freeGPT/gpt4/
+-rw-rw-rw-   0        0        0     6391 2023-05-13 18:23:11.000000 freeGPT-1.0.2/freeGPT/gpt4/__init__.py
+-rw-rw-rw-   0        0        0      410 2023-05-13 18:23:11.000000 freeGPT-1.0.2/freeGPT/gpt4/typing.py
+drwxrwxrwx   0        0        0        0 2023-05-14 08:45:44.207270 freeGPT-1.0.2/freeGPT.egg-info/
+-rw-rw-rw-   0        0        0     3038 2023-05-14 08:45:44.000000 freeGPT-1.0.2/freeGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-05-14 08:45:44.000000 freeGPT-1.0.2/freeGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 08:45:44.000000 freeGPT-1.0.2/freeGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 08:45:44.000000 freeGPT-1.0.2/freeGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-14 08:45:44.000000 freeGPT-1.0.2/freeGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 08:45:44.212273 freeGPT-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1434 2023-05-14 08:33:06.000000 freeGPT-1.0.2/setup.py
```

### Comparing `freeGPT-1.0.1/LICENSE.md` & `freeGPT-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.1/freeGPT/__init__.py` & `freeGPT-1.0.2/freeGPT/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import Enum
 from freeGPT import gpt3, gpt4
 
 __author__ = "Ruu3f"
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 
 class Provider(Enum):
     gpt3 = 1
     gpt4 = 2
 
 class Completion:
```

### Comparing `freeGPT-1.0.1/freeGPT/gpt3/__init__.py` & `freeGPT-1.0.2/freeGPT/gpt3/__init__.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.1/freeGPT/gpt4/__init__.py` & `freeGPT-1.0.2/freeGPT/gpt4/__init__.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.1/setup.py` & `freeGPT-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="freeGPT",
-    version="1.0.1",
+    version="1.0.2",
     description="A Python package that provides free access to GPT3, GPT4, and more models.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Ruu3f/freeGPT",
     author="Ruu3f",
     license="GPLv3",
     keywords=[
```

