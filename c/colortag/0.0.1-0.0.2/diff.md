# Comparing `tmp/colortag-0.0.1.tar.gz` & `tmp/colortag-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colortag-0.0.1.tar", last modified: Sat May 13 20:42:46 2023, max compression
+gzip compressed data, was "colortag-0.0.2.tar", last modified: Sat May 13 22:25:23 2023, max compression
```

## Comparing `colortag-0.0.1.tar` & `colortag-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 wk        (1000) wk        (1001)        0 2023-05-13 20:42:46.098249 colortag-0.0.1/
--rw-r--r--   0 wk        (1000) wk        (1001)      520 2023-05-13 20:42:46.098249 colortag-0.0.1/PKG-INFO
-drwxr-xr-x   0 wk        (1000) wk        (1001)        0 2023-05-13 20:42:46.094916 colortag-0.0.1/colortag/
--rw-r--r--   0 wk        (1000) wk        (1001)       21 2023-05-13 20:23:45.000000 colortag-0.0.1/colortag/__init__.py
--rw-r--r--   0 wk        (1000) wk        (1001)     7491 2023-05-13 20:40:44.000000 colortag-0.0.1/colortag/colortag.py
-drwxr-xr-x   0 wk        (1000) wk        (1001)        0 2023-05-13 20:42:46.098249 colortag-0.0.1/colortag.egg-info/
--rw-r--r--   0 wk        (1000) wk        (1001)      520 2023-05-13 20:42:46.000000 colortag-0.0.1/colortag.egg-info/PKG-INFO
--rw-r--r--   0 wk        (1000) wk        (1001)      178 2023-05-13 20:42:46.000000 colortag-0.0.1/colortag.egg-info/SOURCES.txt
--rw-r--r--   0 wk        (1000) wk        (1001)        1 2023-05-13 20:42:46.000000 colortag-0.0.1/colortag.egg-info/dependency_links.txt
--rw-r--r--   0 wk        (1000) wk        (1001)        9 2023-05-13 20:42:46.000000 colortag-0.0.1/colortag.egg-info/top_level.txt
--rw-r--r--   0 wk        (1000) wk        (1001)       38 2023-05-13 20:42:46.098249 colortag-0.0.1/setup.cfg
--rw-r--r--   0 wk        (1000) wk        (1001)      723 2023-05-13 20:41:39.000000 colortag-0.0.1/setup.py
+drwxr-xr-x   0 wk        (1000) wk        (1001)        0 2023-05-13 22:25:23.394939 colortag-0.0.2/
+-rw-r--r--   0 wk        (1000) wk        (1001)      520 2023-05-13 22:25:23.394939 colortag-0.0.2/PKG-INFO
+drwxr-xr-x   0 wk        (1000) wk        (1001)        0 2023-05-13 22:25:23.394939 colortag-0.0.2/colortag/
+-rw-r--r--   0 wk        (1000) wk        (1001)       31 2023-05-13 22:17:01.000000 colortag-0.0.2/colortag/__init__.py
+-rw-r--r--   0 wk        (1000) wk        (1001)     7478 2023-05-13 22:14:43.000000 colortag-0.0.2/colortag/colortag.py
+drwxr-xr-x   0 wk        (1000) wk        (1001)        0 2023-05-13 22:25:23.394939 colortag-0.0.2/colortag.egg-info/
+-rw-r--r--   0 wk        (1000) wk        (1001)      520 2023-05-13 22:25:23.000000 colortag-0.0.2/colortag.egg-info/PKG-INFO
+-rw-r--r--   0 wk        (1000) wk        (1001)      178 2023-05-13 22:25:23.000000 colortag-0.0.2/colortag.egg-info/SOURCES.txt
+-rw-r--r--   0 wk        (1000) wk        (1001)        1 2023-05-13 22:25:23.000000 colortag-0.0.2/colortag.egg-info/dependency_links.txt
+-rw-r--r--   0 wk        (1000) wk        (1001)        9 2023-05-13 22:25:23.000000 colortag-0.0.2/colortag.egg-info/top_level.txt
+-rw-r--r--   0 wk        (1000) wk        (1001)       38 2023-05-13 22:25:23.394939 colortag-0.0.2/setup.cfg
+-rw-r--r--   0 wk        (1000) wk        (1001)      723 2023-05-13 22:23:18.000000 colortag-0.0.2/setup.py
```

### Comparing `colortag-0.0.1/PKG-INFO` & `colortag-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colortag
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python library for adding ANSI colors to the terminal output using a simple syntax
 Author: Wagner Kauê
 Author-email: <wkmartinst@gmail.com>
 Keywords: python,ansi,colors,color,terminal
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `colortag-0.0.1/colortag/colortag.py` & `colortag-0.0.2/colortag/colortag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from . import re
-from . import sys
+import re
+import sys
 
 ansi_codes = {
     # bg = background
     # l = light
 
     # colors
     "black": "30",
@@ -225,7 +225,8 @@
         string = string[:start] + match.group(1) + string[end:]
     return ColorTag(string, tags)
 
 
 def cprint(*strings, sep=" ", end="\n", file=sys.stdout, flush=False):
     strings = tuple([c(string) for string in strings])
     print(*strings, sep=sep, end=end, file=file, flush=flush)
+
```

### Comparing `colortag-0.0.1/colortag.egg-info/PKG-INFO` & `colortag-0.0.2/colortag.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colortag
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python library for adding ANSI colors to the terminal output using a simple syntax
 Author: Wagner Kauê
 Author-email: <wkmartinst@gmail.com>
 Keywords: python,ansi,colors,color,terminal
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `colortag-0.0.1/setup.py` & `colortag-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Python library for adding ANSI colors to the terminal output using a simple syntax'
 
 setup(
     name="colortag",
     version=VERSION,
     author="Wagner Kauê",
     author_email="<wkmartinst@gmail.com>",
```

