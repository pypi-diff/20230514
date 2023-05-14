# Comparing `tmp/zyncify-0.1.4-py2.py3-none-any.whl.zip` & `tmp/zyncify-0.1.5-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 17046 bytes, number of entries: 12
+Zip file size: 17198 bytes, number of entries: 12
 -rw-r--r--  2.0 unx      146 b- defN 23-May-14 14:49 zync/__init__.py
--rw-r--r--  2.0 unx     2655 b- defN 23-May-14 15:17 zync/logger.py
+-rw-r--r--  2.0 unx     2862 b- defN 23-May-14 16:52 zync/logger.py
 -rw-r--r--  2.0 unx      480 b- defN 23-May-13 13:21 zync/logging.py
--rw-r--r--  2.0 unx     1470 b- defN 23-May-14 15:28 zync/main.py
+-rw-r--r--  2.0 unx     1470 b- defN 23-May-14 16:53 zync/main.py
 -rw-r--r--  2.0 unx      838 b- defN 23-May-13 13:15 zync/slugify.py
 -rw-r--r--  2.0 unx      966 b- defN 23-May-13 14:31 zync/zync.py
--rw-r--r--  2.0 unx    35149 b- defN 23-May-14 15:32 zyncify-0.1.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     1639 b- defN 23-May-14 15:32 zyncify-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-14 15:32 zyncify-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       40 b- defN 23-May-14 15:32 zyncify-0.1.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-May-14 15:32 zyncify-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      904 b- defN 23-May-14 15:32 zyncify-0.1.4.dist-info/RECORD
-12 files, 44402 bytes uncompressed, 15546 bytes compressed:  65.0%
+-rw-r--r--  2.0 unx    35149 b- defN 23-May-14 16:53 zyncify-0.1.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1844 b- defN 23-May-14 16:53 zyncify-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-14 16:53 zyncify-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       40 b- defN 23-May-14 16:53 zyncify-0.1.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-May-14 16:53 zyncify-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      904 b- defN 23-May-14 16:53 zyncify-0.1.5.dist-info/RECORD
+12 files, 44814 bytes uncompressed, 15698 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: zync/slugify.py
 Comment: 
 
 Filename: zync/zync.py
 Comment: 
 
-Filename: zyncify-0.1.4.dist-info/LICENSE
+Filename: zyncify-0.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: zyncify-0.1.4.dist-info/METADATA
+Filename: zyncify-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: zyncify-0.1.4.dist-info/WHEEL
+Filename: zyncify-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: zyncify-0.1.4.dist-info/entry_points.txt
+Filename: zyncify-0.1.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: zyncify-0.1.4.dist-info/top_level.txt
+Filename: zyncify-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: zyncify-0.1.4.dist-info/RECORD
+Filename: zyncify-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zync/logger.py

```diff
@@ -1,12 +1,14 @@
 import logging
 import inspect
 import os
 
 
+ROOT_PATH = os.getcwd() + "/"
+
 W = "\033[39m"
 B = "\033[94m"
 G = "\033[92m"
 Y = "\033[33m"
 R = "\033[91m"
 M = "\033[35m"
 C = "\033[36m"
@@ -79,19 +81,26 @@
         self.logger.info(log, extra={"line": line, "location": location})
 
 
 bugger_base = Bugger("bugger")
 logger_base = Logger("logger")
 
 
+def strip_root_path(file_path, root_path):
+    relative_path = os.path.relpath(file_path, root_path)
+    return relative_path
+
+
 def bugger(log):
     frame = inspect.currentframe().f_back
     line = inspect.getframeinfo(frame).positions.lineno
-    location = os.path.basename(inspect.getframeinfo(frame).filename)
+    file_path = frame.f_code.co_filename
+    location = strip_root_path(file_path, ROOT_PATH)
     return bugger_base(log, line, location)
 
 
 def logger(log):
     frame = inspect.currentframe().f_back
     line = inspect.getframeinfo(frame).positions.lineno
-    location = os.path.basename(inspect.getframeinfo(frame).filename)
+    file_path = frame.f_code.co_filename
+    location = strip_root_path(file_path, ROOT_PATH)
     return logger_base(log, line, location)
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
-VERSION = "0.1.4"
+VERSION = "0.1.5"
 AUTHOR = "TJ Bredemeyer"
 AUTHOR_EMAIL = "tj@teicor.com"
 LICENSE = "GNU Public License v3"
 
 info_string = (
     "\n"
     f"name: {DISPLAY_NAME}\n"
```

## Comparing `zyncify-0.1.4.dist-info/LICENSE` & `zyncify-0.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `zyncify-0.1.4.dist-info/METADATA` & `zyncify-0.1.5.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: zyncify
-Version: 0.1.4
+Version: 0.1.5
 Summary: zync is a utility tool for python operations
 Home-page: https://github.com/tjbredemeyer/zync
 Author: TJ Bredemeyer
 Author-email: tj@teicor.com
 License: GNU Public License v3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # zync
 
 zync is a utility tool for python operations.
 
+[![zync-ci](https://github.com/tjbredemeyer/zync/actions/workflows/ci.yml/badge.svg)](https://github.com/tjbredemeyer/zync/actions/workflows/ci.yml)
+
 ## INSTALLATION
 
 ```bash
 pip install zyncify
 ```
 
 ## Usage
@@ -97,11 +99,17 @@
 string = "Test String"
 slugger(string)
 
 ###
 # returns: test-string
 ```  
 
+### 3. TAIL LOG FILE
+
+```bash
+tail -f ./.zync.log
+```
+
 ## Author
 
 TJ Bredemeyer  
 twitter: @tjbredemeyer
```

