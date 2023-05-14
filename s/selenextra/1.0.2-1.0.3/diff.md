# Comparing `tmp/selenextra-1.0.2.tar.gz` & `tmp/selenextra-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenextra-1.0.2.tar", last modified: Mon Apr 17 06:35:59 2023, max compression
+gzip compressed data, was "selenextra-1.0.3.tar", last modified: Sun May 14 05:01:56 2023, max compression
```

## Comparing `selenextra-1.0.2.tar` & `selenextra-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 06:35:59.346557 selenextra-1.0.2/
--rw-rw-rw-   0        0        0    35823 2023-04-17 06:11:14.000000 selenextra-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      627 2023-04-17 06:35:59.345559 selenextra-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-04-17 06:11:14.000000 selenextra-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 06:35:59.339575 selenextra-1.0.2/selenextra/
--rw-rw-rw-   0        0        0     4630 2023-04-17 06:35:09.000000 selenextra-1.0.2/selenextra/__init__.py
--rw-rw-rw-   0        0        0       46 2023-04-17 06:11:14.000000 selenextra-1.0.2/selenextra/exceptions.py
--rw-rw-rw-   0        0        0     1239 2023-04-17 06:11:14.000000 selenextra-1.0.2/selenextra/patcher.py
-drwxrwxrwx   0        0        0        0 2023-04-17 06:35:59.344560 selenextra-1.0.2/selenextra.egg-info/
--rw-rw-rw-   0        0        0      627 2023-04-17 06:35:59.000000 selenextra-1.0.2/selenextra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-04-17 06:35:59.000000 selenextra-1.0.2/selenextra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 06:35:59.000000 selenextra-1.0.2/selenextra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-04-17 06:35:59.000000 selenextra-1.0.2/selenextra.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-17 06:35:59.000000 selenextra-1.0.2/selenextra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 06:35:59.346557 selenextra-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      782 2023-04-17 06:35:20.000000 selenextra-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 05:01:56.034487 selenextra-1.0.3/
+-rw-rw-rw-   0        0        0    35823 2023-05-14 04:52:24.000000 selenextra-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      627 2023-05-14 05:01:56.034487 selenextra-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-05-14 04:52:24.000000 selenextra-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 05:01:55.990605 selenextra-1.0.3/selenextra/
+-rw-rw-rw-   0        0        0     4709 2023-05-14 04:59:16.000000 selenextra-1.0.3/selenextra/__init__.py
+-rw-rw-rw-   0        0        0       46 2023-05-14 04:52:24.000000 selenextra-1.0.3/selenextra/exceptions.py
+-rw-rw-rw-   0        0        0     1030 2023-05-14 04:59:02.000000 selenextra-1.0.3/selenextra/patcher.py
+drwxrwxrwx   0        0        0        0 2023-05-14 05:01:56.033490 selenextra-1.0.3/selenextra.egg-info/
+-rw-rw-rw-   0        0        0      627 2023-05-14 05:01:55.000000 selenextra-1.0.3/selenextra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-05-14 05:01:55.000000 selenextra-1.0.3/selenextra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 05:01:55.000000 selenextra-1.0.3/selenextra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-14 05:01:55.000000 selenextra-1.0.3/selenextra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-14 05:01:55.000000 selenextra-1.0.3/selenextra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 05:01:56.034487 selenextra-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      782 2023-05-14 04:59:54.000000 selenextra-1.0.3/setup.py
```

### Comparing `selenextra-1.0.2/LICENSE` & `selenextra-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `selenextra-1.0.2/PKG-INFO` & `selenextra-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: selenextra
-Version: 1.0.2
+Version: 1.0.3
 Summary: Bringing additional features to Selenium
 Home-page: https://github.com/nguyenvantat1182002/SeleneXtra
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `selenextra-1.0.2/selenextra/__init__.py` & `selenextra-1.0.3/selenextra/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 import random as rnd
 import time
 
 
 class ChromeDriver(Chrome):
     CONNECTION_TIMEOUT = 30
 
-    def __init__(self, **kwargs) -> None:
+    def __init__(self, user_multi_procs: bool = True, **kwargs) -> None:
         self.custom_patcher = CustomPatcher(
             executable_path=kwargs.get('driver_executable_path', None),
             force=kwargs.get('patcher_force_close', False),
-            version_main=kwargs.get('version_main', None)
+            version_main=kwargs.get('version_main', None),
+            user_multi_procs=user_multi_procs
         )
 
         self.custom_patcher.auto()
 
         release = self.custom_patcher.fetch_release_number()
         version = release.version[0]
```

### Comparing `selenextra-1.0.2/selenextra/patcher.py` & `selenextra-1.0.3/selenextra/patcher.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 from undetected_chromedriver.patcher import Patcher
 
-import os
-import secrets
 import string
 import random
 import re
 import io
 
 
 class CustomPatcher(Patcher):
-    def __init__(self, executable_path=None, force=False, version_main: int = 0) -> None:
-        super().__init__(executable_path, force, version_main)
-
-        if not executable_path:
-            exe_name = os.path.basename(self.executable_path)
-            self.executable_path = f'{self.executable_path.replace(exe_name, f"{secrets.token_hex(5)}_{exe_name}")}'
+    def __init__(self, executable_path=None, force=False, version_main: int = 0, user_multi_procs=False):
+        super().__init__(executable_path, force, version_main, user_multi_procs)
 
     @staticmethod
     def gen_random_cdc() -> bytes:
         cdc = random.choices(string.ascii_lowercase, k=26)
         cdc[-6:-4] = map(str.upper, cdc[-6:-4])
         cdc[2] = cdc[0]
         cdc[3] = "_"
```

### Comparing `selenextra-1.0.2/selenextra.egg-info/PKG-INFO` & `selenextra-1.0.3/selenextra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: selenextra
-Version: 1.0.2
+Version: 1.0.3
 Summary: Bringing additional features to Selenium
 Home-page: https://github.com/nguyenvantat1182002/SeleneXtra
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

