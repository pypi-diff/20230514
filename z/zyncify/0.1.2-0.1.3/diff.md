# Comparing `tmp/zyncify-0.1.2-py2.py3-none-any.whl.zip` & `tmp/zyncify-0.1.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,14 @@
-Zip file size: 16331 bytes, number of entries: 11
--rw-r--r--  2.0 unx      180 b- defN 23-May-13 15:40 zync/__init__.py
+Zip file size: 17174 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      232 b- defN 23-May-14 03:37 zync/__init__.py
+-rw-r--r--  2.0 unx     5242 b- defN 23-May-14 04:45 zync/logger.py
 -rw-r--r--  2.0 unx      480 b- defN 23-May-13 13:21 zync/logging.py
--rw-r--r--  2.0 unx     1470 b- defN 23-May-13 16:44 zync/main.py
+-rw-r--r--  2.0 unx     1470 b- defN 23-May-14 04:46 zync/main.py
 -rw-r--r--  2.0 unx      838 b- defN 23-May-13 13:15 zync/slugify.py
 -rw-r--r--  2.0 unx      966 b- defN 23-May-13 14:31 zync/zync.py
--rw-r--r--  2.0 unx    35149 b- defN 23-May-13 16:44 zyncify-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1647 b- defN 23-May-13 16:44 zyncify-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-13 16:44 zyncify-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       40 b- defN 23-May-13 16:44 zyncify-0.1.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-May-13 16:44 zyncify-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      833 b- defN 23-May-13 16:44 zyncify-0.1.2.dist-info/RECORD
-11 files, 41718 bytes uncompressed, 14935 bytes compressed:  64.2%
+-rw-r--r--  2.0 unx    35149 b- defN 23-May-14 04:47 zyncify-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1645 b- defN 23-May-14 04:47 zyncify-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-14 04:47 zyncify-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       40 b- defN 23-May-14 04:47 zyncify-0.1.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-May-14 04:47 zyncify-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      904 b- defN 23-May-14 04:47 zyncify-0.1.3.dist-info/RECORD
+12 files, 47081 bytes uncompressed, 15674 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -1,34 +1,37 @@
 Filename: zync/__init__.py
 Comment: 
 
+Filename: zync/logger.py
+Comment: 
+
 Filename: zync/logging.py
 Comment: 
 
 Filename: zync/main.py
 Comment: 
 
 Filename: zync/slugify.py
 Comment: 
 
 Filename: zync/zync.py
 Comment: 
 
-Filename: zyncify-0.1.2.dist-info/LICENSE
+Filename: zyncify-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: zyncify-0.1.2.dist-info/METADATA
+Filename: zyncify-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: zyncify-0.1.2.dist-info/WHEEL
+Filename: zyncify-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: zyncify-0.1.2.dist-info/entry_points.txt
+Filename: zyncify-0.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: zyncify-0.1.2.dist-info/top_level.txt
+Filename: zyncify-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: zyncify-0.1.2.dist-info/RECORD
+Filename: zyncify-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zync/__init__.py

```diff
@@ -1,7 +1,13 @@
-from .logging import logger, bugger
+from .logger import logger, bugger, wagger, egger, critter, fatal
 from .slugify import Slugger, slugger
 
-__all__ = ["logger", "bugger", "Slugger", "slugger"]
-
-__version__ = "0.1.0"
-__author__ = "TJ Bredemeyer"
+__all__ = [
+    "bugger",
+    "logger",
+    "wagger",
+    "egger",
+    "critter",
+    "fatal",
+    "Slugger",
+    "slugger",
+]
```

## zync/main.py

```diff
@@ -5,15 +5,15 @@
 import argparse
 from .__init__ import __all__ as methods
 
 NAME = "zyncify"
 DISPLAY_NAME = "zync"
 DESCRIPTION = "zync is a utility tool for python operations"
 URL = "https://github.com/tjbredemeyer/zync"
-VERSION = "0.1.2"
+VERSION = "0.1.3"
 AUTHOR = "TJ Bredemeyer"
 AUTHOR_EMAIL = "tj@teicor.com"
 LICENSE = "GNU Public License v3"
 
 info_string = (
     "\n"
     f"name: {DISPLAY_NAME}\n"
```

## Comparing `zyncify-0.1.2.dist-info/LICENSE` & `zyncify-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `zyncify-0.1.2.dist-info/METADATA` & `zyncify-0.1.3.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zyncify
-Version: 0.1.2
+Version: 0.1.3
 Summary: zync is a utility tool for python operations
 Home-page: https://github.com/tjbredemeyer/zync
 Author: TJ Bredemeyer
 Author-email: tj@teicor.com
 License: GNU Public License v3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -66,15 +66,15 @@
 ```  
 
 #### 3. Slugger  
 
 Slugger converts a string to slug while maintaining capitalization.  
 
 ```python
-from zynce import Slugger
+from zync import Slugger
 
 # Slugging a string with Caps
 Slugger("Test String")
 
 # Slugging a variable with caps
 string = "Test String"
 Slugger = (string)
@@ -84,15 +84,15 @@
 ```  
   
 #### 4. slugger  
 
 slugger converts a string to a slug with no capitalization.
 
 ```python
-from zynce import Slugger
+from zync import slugger
 
 # Slugging a string without Caps
 slugger("Test String")
 
 # Slugging a variable without caps
 string = "Test String"
 slugger = (string)
```

