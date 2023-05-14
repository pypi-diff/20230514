# Comparing `tmp/zyncify-0.1.3-py2.py3-none-any.whl.zip` & `tmp/zyncify-0.1.4-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 17174 bytes, number of entries: 12
--rw-r--r--  2.0 unx      232 b- defN 23-May-14 03:37 zync/__init__.py
--rw-r--r--  2.0 unx     5242 b- defN 23-May-14 04:45 zync/logger.py
+Zip file size: 17046 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      146 b- defN 23-May-14 14:49 zync/__init__.py
+-rw-r--r--  2.0 unx     2655 b- defN 23-May-14 15:17 zync/logger.py
 -rw-r--r--  2.0 unx      480 b- defN 23-May-13 13:21 zync/logging.py
--rw-r--r--  2.0 unx     1470 b- defN 23-May-14 04:46 zync/main.py
+-rw-r--r--  2.0 unx     1470 b- defN 23-May-14 15:28 zync/main.py
 -rw-r--r--  2.0 unx      838 b- defN 23-May-13 13:15 zync/slugify.py
 -rw-r--r--  2.0 unx      966 b- defN 23-May-13 14:31 zync/zync.py
--rw-r--r--  2.0 unx    35149 b- defN 23-May-14 04:47 zyncify-0.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     1645 b- defN 23-May-14 04:47 zyncify-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-14 04:47 zyncify-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       40 b- defN 23-May-14 04:47 zyncify-0.1.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-May-14 04:47 zyncify-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      904 b- defN 23-May-14 04:47 zyncify-0.1.3.dist-info/RECORD
-12 files, 47081 bytes uncompressed, 15674 bytes compressed:  66.7%
+-rw-r--r--  2.0 unx    35149 b- defN 23-May-14 15:32 zyncify-0.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1639 b- defN 23-May-14 15:32 zyncify-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-14 15:32 zyncify-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       40 b- defN 23-May-14 15:32 zyncify-0.1.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-May-14 15:32 zyncify-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      904 b- defN 23-May-14 15:32 zyncify-0.1.4.dist-info/RECORD
+12 files, 44402 bytes uncompressed, 15546 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: zync/slugify.py
 Comment: 
 
 Filename: zync/zync.py
 Comment: 
 
-Filename: zyncify-0.1.3.dist-info/LICENSE
+Filename: zyncify-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: zyncify-0.1.3.dist-info/METADATA
+Filename: zyncify-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: zyncify-0.1.3.dist-info/WHEEL
+Filename: zyncify-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: zyncify-0.1.3.dist-info/entry_points.txt
+Filename: zyncify-0.1.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: zyncify-0.1.3.dist-info/top_level.txt
+Filename: zyncify-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: zyncify-0.1.3.dist-info/RECORD
+Filename: zyncify-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zync/__init__.py

```diff
@@ -1,13 +1,9 @@
-from .logger import logger, bugger, wagger, egger, critter, fatal
+from .logger import logger, bugger
 from .slugify import Slugger, slugger
 
 __all__ = [
     "bugger",
     "logger",
-    "wagger",
-    "egger",
-    "critter",
-    "fatal",
     "Slugger",
     "slugger",
 ]
```

## zync/logger.py

```diff
@@ -1,163 +1,97 @@
 import logging
 import inspect
+import os
 
 
-WHITE = "\033[39m"
-BLUE = "\033[94m"
-GREEN = "\033[92m"
-YELLOW = "\033[93m"
-RED = "\033[91m"
-BOLD_RED = "\033[31;1m"
-RESET = "\033[0m"
+W = "\033[39m"
+B = "\033[94m"
+G = "\033[92m"
+Y = "\033[33m"
+R = "\033[91m"
+M = "\033[35m"
+C = "\033[36m"
+X = "\033[0m"
+
+
+class BuggerFormat(logging.Formatter):
+    def format(self, record):
+        record.levelname = "bugger"
+        levelname = record.levelname.upper()
+        record.levelname = levelname
+        return super().format(record)
+
+
+class LoggerFormat(logging.Formatter):
+    def format(self, record):
+        record.levelname = "logger"
+        levelname = record.levelname.upper()
+        record.levelname = levelname
+        return super().format(record)
 
 
 class Bugger:
     def __init__(self, name):
         self.logger = logging.getLogger(name)
         self.logger.setLevel(logging.DEBUG)
-        file_handler = logging.FileHandler("zync.log")
-        formatter = logging.Formatter(
-            f"{WHITE}[%(levelname)s] %(asctime)s "
-            f"@ %(location)s (line %(line)s): %(message)s{RESET}",
+        file_handler = logging.FileHandler(".zync.log")
+        formatter = BuggerFormat(
+            f"{G}[{X}"
+            f"{G}%(levelname)s{X}"
+            f"{R}:{X}"
+            f"{C}%(line)s{X}"
+            f"{G}@{X}"
+            f"{M}%(location)s{X}"
+            f"{G}%(asctime)s{X}"
+            f"{G}]{X}"
+            f"{G}> {X}"
+            f"%(message)s{X}",
             datefmt="%H:%M:%S",
         )
         file_handler.setFormatter(formatter)
         self.logger.addHandler(file_handler)
 
     def __call__(self, log, line, location):
         self.logger.debug(log, extra={"line": line, "location": location})
 
 
 class Logger:
     def __init__(self, name):
         self.logger = logging.getLogger(name)
         self.logger.setLevel(logging.INFO)
-        file_handler = logging.FileHandler("zync.log")
-        formatter = logging.Formatter(
-            f"{BLUE}[%(levelname)s] %(asctime)s "
-            f"@ %(location)s (line %(line)s): %(message)s{RESET}",
+        file_handler = logging.FileHandler(".zync.log")
+        formatter = LoggerFormat(
+            f"{Y}[{X}"
+            f"{Y}%(levelname)s{X}"
+            f"{R}:{X}"
+            f"{C}%(line)s{X}"
+            f"{Y}@{X}"
+            f"{M}%(location)s{X}"
+            f"{Y}%(asctime)s{X}"
+            f"{Y}]{X}"
+            f"{Y}> {X}"
+            f"%(message)s{X}",
             datefmt="%H:%M:%S",
         )
         file_handler.setFormatter(formatter)
         self.logger.addHandler(file_handler)
 
     def __call__(self, log, line, location):
         self.logger.info(log, extra={"line": line, "location": location})
 
 
-class Wagger:
-    def __init__(self, name):
-        self.logger = logging.getLogger(name)
-        self.logger.setLevel(logging.WARNING)
-        file_handler = logging.FileHandler("zync.log")
-        formatter = logging.Formatter(
-            f"{GREEN}[%(levelname)s] %(asctime)s "
-            f"@ %(location)s (line %(line)s): %(message)s{RESET}",
-            datefmt="%H:%M:%S",
-        )
-        file_handler.setFormatter(formatter)
-        self.logger.addHandler(file_handler)
-
-    def __call__(self, log, line, location):
-        self.logger.warning(log, extra={"line": line, "location": location})
-
-
-class Egger:
-    def __init__(self, name):
-        self.logger = logging.getLogger(name)
-        self.logger.setLevel(logging.ERROR)
-        file_handler = logging.FileHandler("zync.log")
-        formatter = logging.Formatter(
-            f"{YELLOW}[%(levelname)s] %(asctime)s "
-            f"@ %(location)s (line %(line)s): %(message)s{RESET}",
-            datefmt="%H:%M:%S",
-        )
-        file_handler.setFormatter(formatter)
-        self.logger.addHandler(file_handler)
-
-    def __call__(self, log, line, location):
-        self.logger.error(log, extra={"line": line, "location": location})
-
-
-class Critter:
-    def __init__(self, name):
-        self.logger = logging.getLogger(name)
-        self.logger.setLevel(logging.CRITICAL)
-        file_handler = logging.FileHandler("zync.log")
-        formatter = logging.Formatter(
-            f"{RED}[%(levelname)s] %(asctime)s "
-            f"@ %(location)s (line %(line)s): %(message)s{RESET}",
-            datefmt="%H:%M:%S",
-        )
-        file_handler.setFormatter(formatter)
-        self.logger.addHandler(file_handler)
-
-    def __call__(self, log, line, location):
-        self.logger.critical(log, extra={"line": line, "location": location})
-
-
-class Fatal:
-    def __init__(self, name):
-        self.logger = logging.getLogger(name)
-        self.logger.setLevel(logging.FATAL)
-        file_handler = logging.FileHandler("zync.log")
-        formatter = logging.Formatter(
-            f"{BOLD_RED}[%(levelname)s] %(asctime)s "
-            f"@ %(location)s (line %(line)s): %(message)s{RESET}",
-            datefmt="%H:%M:%S",
-        )
-        file_handler.setFormatter(formatter)
-        self.logger.addHandler(file_handler)
-
-    def __call__(self, log, line, location):
-        self.logger.fatal(log, extra={"line": line, "location": location})
-
-
 bugger_base = Bugger("bugger")
 logger_base = Logger("logger")
-wagger_base = Wagger("wagger")
-egger_base = Egger("egger")
-critter_base = Critter("critter")
-fatal_base = Fatal("fatal")
 
 
 def bugger(log):
     frame = inspect.currentframe().f_back
     line = inspect.getframeinfo(frame).positions.lineno
-    location = inspect.getframeinfo(frame).filename
+    location = os.path.basename(inspect.getframeinfo(frame).filename)
     return bugger_base(log, line, location)
 
 
 def logger(log):
     frame = inspect.currentframe().f_back
     line = inspect.getframeinfo(frame).positions.lineno
-    location = inspect.getframeinfo(frame).filename
+    location = os.path.basename(inspect.getframeinfo(frame).filename)
     return logger_base(log, line, location)
-
-
-def wagger(log):
-    frame = inspect.currentframe().f_back
-    line = inspect.getframeinfo(frame).positions.lineno
-    location = inspect.getframeinfo(frame).filename
-    return wagger_base(log, line, location)
-
-
-def egger(log):
-    frame = inspect.currentframe().f_back
-    line = inspect.getframeinfo(frame).positions.lineno
-    location = inspect.getframeinfo(frame).filename
-    return egger_base(log, line, location)
-
-
-def critter(log):
-    frame = inspect.currentframe().f_back
-    line = inspect.getframeinfo(frame).positions.lineno
-    location = inspect.getframeinfo(frame).filename
-    return critter_base(log, line, location)
-
-
-def fatal(log):
-    frame = inspect.currentframe().f_back
-    line = inspect.getframeinfo(frame).positions.lineno
-    location = inspect.getframeinfo(frame).filename
-    return fatal_base(log, line, location)
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
-VERSION = "0.1.3"
+VERSION = "0.1.4"
 AUTHOR = "TJ Bredemeyer"
 AUTHOR_EMAIL = "tj@teicor.com"
 LICENSE = "GNU Public License v3"
 
 info_string = (
     "\n"
     f"name: {DISPLAY_NAME}\n"
```

## Comparing `zyncify-0.1.3.dist-info/LICENSE` & `zyncify-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `zyncify-0.1.3.dist-info/METADATA` & `zyncify-0.1.4.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zyncify
-Version: 0.1.3
+Version: 0.1.4
 Summary: zync is a utility tool for python operations
 Home-page: https://github.com/tjbredemeyer/zync
 Author: TJ Bredemeyer
 Author-email: tj@teicor.com
 License: GNU Public License v3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -73,15 +73,15 @@
 from zync import Slugger
 
 # Slugging a string with Caps
 Slugger("Test String")
 
 # Slugging a variable with caps
 string = "Test String"
-Slugger = (string)
+Slugger(string)
 
 ###
 # returns: Test-String
 ```  
   
 #### 4. slugger  
 
@@ -91,15 +91,15 @@
 from zync import slugger
 
 # Slugging a string without Caps
 slugger("Test String")
 
 # Slugging a variable without caps
 string = "Test String"
-slugger = (string)
+slugger(string)
 
 ###
 # returns: test-string
 ```  
 
 ## Author
```

