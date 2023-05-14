# Comparing `tmp/tarvis-tradingbot-0.9.5.tar.gz` & `tmp/tarvis-tradingbot-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarvis-tradingbot-0.9.5.tar", last modified: Wed May  3 02:17:12 2023, max compression
+gzip compressed data, was "tarvis-tradingbot-0.9.6.tar", last modified: Sun May 14 09:51:20 2023, max compression
```

## Comparing `tarvis-tradingbot-0.9.5.tar` & `tarvis-tradingbot-0.9.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 02:17:12.788482 tarvis-tradingbot-0.9.5/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-05-03 02:17:01.000000 tarvis-tradingbot-0.9.5/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      388 2023-05-03 02:17:12.788482 tarvis-tradingbot-0.9.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-03 02:17:01.000000 tarvis-tradingbot-0.9.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 02:17:12.788482 tarvis-tradingbot-0.9.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      842 2023-05-03 02:17:01.000000 tarvis-tradingbot-0.9.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 02:17:12.784482 tarvis-tradingbot-0.9.5/tarvis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 02:17:12.788482 tarvis-tradingbot-0.9.5/tarvis/tradingbot/
--rw-r--r--   0 root         (0) root         (0)      526 2023-05-03 02:17:01.000000 tarvis-tradingbot-0.9.5/tarvis/tradingbot/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 02:17:12.788482 tarvis-tradingbot-0.9.5/tarvis_tradingbot.egg-info/
--rw-r--r--   0 root         (0) root         (0)      388 2023-05-03 02:17:12.000000 tarvis-tradingbot-0.9.5/tarvis_tradingbot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      308 2023-05-03 02:17:12.000000 tarvis-tradingbot-0.9.5/tarvis_tradingbot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 02:17:12.000000 tarvis-tradingbot-0.9.5/tarvis_tradingbot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-05-03 02:17:12.000000 tarvis-tradingbot-0.9.5/tarvis_tradingbot.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-05-03 02:17:12.000000 tarvis-tradingbot-0.9.5/tarvis_tradingbot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-03 02:17:12.000000 tarvis-tradingbot-0.9.5/tarvis_tradingbot.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:51:20.572299 tarvis-tradingbot-0.9.6/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-05-14 09:51:09.000000 tarvis-tradingbot-0.9.6/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      388 2023-05-14 09:51:20.568298 tarvis-tradingbot-0.9.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-14 09:51:09.000000 tarvis-tradingbot-0.9.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 09:51:20.572299 tarvis-tradingbot-0.9.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      842 2023-05-14 09:51:09.000000 tarvis-tradingbot-0.9.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:51:20.568298 tarvis-tradingbot-0.9.6/tarvis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:51:20.568298 tarvis-tradingbot-0.9.6/tarvis/tradingbot/
+-rw-r--r--   0 root         (0) root         (0)      526 2023-05-14 09:51:09.000000 tarvis-tradingbot-0.9.6/tarvis/tradingbot/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:51:20.568298 tarvis-tradingbot-0.9.6/tarvis_tradingbot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      388 2023-05-14 09:51:20.000000 tarvis-tradingbot-0.9.6/tarvis_tradingbot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      308 2023-05-14 09:51:20.000000 tarvis-tradingbot-0.9.6/tarvis_tradingbot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 09:51:20.000000 tarvis-tradingbot-0.9.6/tarvis_tradingbot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-05-14 09:51:20.000000 tarvis-tradingbot-0.9.6/tarvis_tradingbot.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-05-14 09:51:20.000000 tarvis-tradingbot-0.9.6/tarvis_tradingbot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-14 09:51:20.000000 tarvis-tradingbot-0.9.6/tarvis_tradingbot.egg-info/top_level.txt
```

### Comparing `tarvis-tradingbot-0.9.5/LICENSE.txt` & `tarvis-tradingbot-0.9.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tarvis-tradingbot-0.9.5/setup.py` & `tarvis-tradingbot-0.9.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = requirements_file.read().splitlines()
 
 with open("README.md") as description_file:
     long_description = description_file.read()
 
 setup(
     name="tarvis-tradingbot",
-    version="0.9.5",
+    version="0.9.6",
     author="Tarvis Labs",
     author_email="python@tarvislabs.com",
     url="https://tarvislabs.com/",
     description="Tarvis Basic Trading Bot",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `tarvis-tradingbot-0.9.5/tarvis/tradingbot/__init__.py` & `tarvis-tradingbot-0.9.6/tarvis/tradingbot/__init__.py`

 * *Files identical despite different names*

