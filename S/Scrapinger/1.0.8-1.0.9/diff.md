# Comparing `tmp/Scrapinger-1.0.8.tar.gz` & `tmp/Scrapinger-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Scrapinger-1.0.8.tar", last modified: Thu Nov 25 03:47:45 2021, max compression
+gzip compressed data, was "Scrapinger-1.0.9.tar", last modified: Thu Nov 25 03:50:26 2021, max compression
```

## Comparing `Scrapinger-1.0.8.tar` & `Scrapinger-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2021-11-25 03:47:45.925882 Scrapinger-1.0.8/
--rw-rw-rw-   0        0        0      963 2021-11-25 03:47:45.925882 Scrapinger-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       38 2021-11-11 13:12:44.000000 Scrapinger-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2021-11-25 03:47:45.912885 Scrapinger-1.0.8/Scrapinger/
-drwxrwxrwx   0        0        0        0 2021-11-25 03:47:45.923858 Scrapinger-1.0.8/Scrapinger/Library/
--rw-rw-rw-   0        0        0     9307 2021-11-22 17:42:12.000000 Scrapinger-1.0.8/Scrapinger/Library/baseWebDriverController.py
--rw-rw-rw-   0        0        0     3781 2021-11-24 23:36:34.000000 Scrapinger-1.0.8/Scrapinger/Library/browserController.py
--rw-rw-rw-   0        0        0     7389 2021-11-24 09:56:21.000000 Scrapinger-1.0.8/Scrapinger/Library/scrapingConfig.py
--rw-rw-rw-   0        0        0      375 2021-11-15 14:51:03.000000 Scrapinger-1.0.8/Scrapinger/Library/scrapingerGlobals.py
--rw-rw-rw-   0        0        0     2236 2021-11-22 16:44:50.000000 Scrapinger-1.0.8/Scrapinger/Library/webDriverController.py
-drwxrwxrwx   0        0        0        0 2021-11-25 03:47:45.918870 Scrapinger-1.0.8/Scrapinger.egg-info/
--rw-rw-rw-   0        0        0      963 2021-11-25 03:47:45.000000 Scrapinger-1.0.8/Scrapinger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      597 2021-11-25 03:47:45.000000 Scrapinger-1.0.8/Scrapinger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-11-25 03:47:45.000000 Scrapinger-1.0.8/Scrapinger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2021-11-25 03:47:45.000000 Scrapinger-1.0.8/Scrapinger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2021-11-25 03:47:45.000000 Scrapinger-1.0.8/Scrapinger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-11-25 03:47:45.925882 Scrapinger-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2204 2021-11-15 14:51:03.000000 Scrapinger-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-11-25 03:50:26.804688 Scrapinger-1.0.9/
+-rw-rw-rw-   0        0        0      963 2021-11-25 03:50:26.803691 Scrapinger-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       38 2021-11-11 13:12:44.000000 Scrapinger-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2021-11-25 03:50:26.793718 Scrapinger-1.0.9/Scrapinger/
+drwxrwxrwx   0        0        0        0 2021-11-25 03:50:26.801697 Scrapinger-1.0.9/Scrapinger/Library/
+-rw-rw-rw-   0        0        0     9307 2021-11-22 17:42:12.000000 Scrapinger-1.0.9/Scrapinger/Library/baseWebDriverController.py
+-rw-rw-rw-   0        0        0     3747 2021-11-25 03:50:05.000000 Scrapinger-1.0.9/Scrapinger/Library/browserController.py
+-rw-rw-rw-   0        0        0     7389 2021-11-24 09:56:21.000000 Scrapinger-1.0.9/Scrapinger/Library/scrapingConfig.py
+-rw-rw-rw-   0        0        0      375 2021-11-15 14:51:03.000000 Scrapinger-1.0.9/Scrapinger/Library/scrapingerGlobals.py
+-rw-rw-rw-   0        0        0     2236 2021-11-22 16:44:50.000000 Scrapinger-1.0.9/Scrapinger/Library/webDriverController.py
+drwxrwxrwx   0        0        0        0 2021-11-25 03:50:26.797709 Scrapinger-1.0.9/Scrapinger.egg-info/
+-rw-rw-rw-   0        0        0      963 2021-11-25 03:50:26.000000 Scrapinger-1.0.9/Scrapinger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2021-11-25 03:50:26.000000 Scrapinger-1.0.9/Scrapinger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-11-25 03:50:26.000000 Scrapinger-1.0.9/Scrapinger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2021-11-25 03:50:26.000000 Scrapinger-1.0.9/Scrapinger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2021-11-25 03:50:26.000000 Scrapinger-1.0.9/Scrapinger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-11-25 03:50:26.804688 Scrapinger-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2204 2021-11-15 14:51:03.000000 Scrapinger-1.0.9/setup.py
```

### Comparing `Scrapinger-1.0.8/PKG-INFO` & `Scrapinger-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: Scrapinger
-Version: 1.0.8
+Version: 1.0.9
 Summary: Scraping Support
 Home-page: https://github.com/kaioman/LibHanger.git
 Author: Unchain Works
 Author-email: kajin0318@gmail.com
 License: BSD-3-Clause
 Description: # Scrapinger
         Scraping General purpose
```

### Comparing `Scrapinger-1.0.8/Scrapinger/Library/baseWebDriverController.py` & `Scrapinger-1.0.9/Scrapinger/Library/baseWebDriverController.py`

 * *Files identical despite different names*

### Comparing `Scrapinger-1.0.8/Scrapinger/Library/browserController.py` & `Scrapinger-1.0.9/Scrapinger/Library/browserController.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import geckodriver_autoinstaller
 import LibHanger.Library.uwLogger as Logger
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options as chromeOptions
 from selenium.webdriver.firefox.options import Options as firefoxOptions
 from LibHanger.Library.uwGlobals import *
 from Scrapinger.Library.baseWebDriverController import baseWebBrowserController
 from Scrapinger.Library.scrapingConfig import scrapingConfig
```

### Comparing `Scrapinger-1.0.8/Scrapinger/Library/scrapingConfig.py` & `Scrapinger-1.0.9/Scrapinger/Library/scrapingConfig.py`

 * *Files identical despite different names*

### Comparing `Scrapinger-1.0.8/Scrapinger/Library/webDriverController.py` & `Scrapinger-1.0.9/Scrapinger/Library/webDriverController.py`

 * *Files identical despite different names*

### Comparing `Scrapinger-1.0.8/Scrapinger.egg-info/PKG-INFO` & `Scrapinger-1.0.9/Scrapinger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: Scrapinger
-Version: 1.0.8
+Version: 1.0.9
 Summary: Scraping Support
 Home-page: https://github.com/kaioman/LibHanger.git
 Author: Unchain Works
 Author-email: kajin0318@gmail.com
 License: BSD-3-Clause
 Description: # Scrapinger
         Scraping General purpose
```

### Comparing `Scrapinger-1.0.8/Scrapinger.egg-info/SOURCES.txt` & `Scrapinger-1.0.9/Scrapinger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Scrapinger-1.0.8/setup.py` & `Scrapinger-1.0.9/setup.py`

 * *Files identical despite different names*

