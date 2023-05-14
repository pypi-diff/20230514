# Comparing `tmp/SantorinAI-1.1.1.tar.gz` & `tmp/SantorinAI-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SantorinAI-1.1.1.tar", last modified: Sun May 14 13:39:11 2023, max compression
+gzip compressed data, was "SantorinAI-1.1.2.tar", last modified: Sun May 14 13:43:37 2023, max compression
```

## Comparing `SantorinAI-1.1.1.tar` & `SantorinAI-1.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 tomansion  (1000) tomansion  (1000)        0 2023-05-14 13:39:11.918686 SantorinAI-1.1.1/
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)    11357 2023-05-14 12:45:31.000000 SantorinAI-1.1.1/LICENSE
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)     4768 2023-05-14 13:39:11.918686 SantorinAI-1.1.1/PKG-INFO
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)     4282 2023-05-14 13:23:42.000000 SantorinAI-1.1.1/README.md
-drwxrwxr-x   0 tomansion  (1000) tomansion  (1000)        0 2023-05-14 13:39:11.914685 SantorinAI-1.1.1/SantorinAI.egg-info/
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)     4768 2023-05-14 13:39:11.000000 SantorinAI-1.1.1/SantorinAI.egg-info/PKG-INFO
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)      440 2023-05-14 13:39:11.000000 SantorinAI-1.1.1/SantorinAI.egg-info/SOURCES.txt
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)        1 2023-05-14 13:39:11.000000 SantorinAI-1.1.1/SantorinAI.egg-info/dependency_links.txt
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)       12 2023-05-14 13:39:11.000000 SantorinAI-1.1.1/SantorinAI.egg-info/requires.txt
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)       16 2023-05-14 13:39:11.000000 SantorinAI-1.1.1/SantorinAI.egg-info/top_level.txt
-drwxrwxr-x   0 tomansion  (1000) tomansion  (1000)        0 2023-05-14 13:39:11.914685 SantorinAI-1.1.1/santorinai/
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)        0 2023-05-14 12:35:43.000000 SantorinAI-1.1.1/santorinai/__init__.py
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)    17372 2023-05-14 12:35:43.000000 SantorinAI-1.1.1/santorinai/board.py
-drwxrwxr-x   0 tomansion  (1000) tomansion  (1000)        0 2023-05-14 13:39:11.914685 SantorinAI-1.1.1/santorinai/board_displayer/
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)        0 2023-05-14 13:22:31.000000 SantorinAI-1.1.1/santorinai/board_displayer/__init__.py
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)     6990 2023-05-14 12:35:43.000000 SantorinAI-1.1.1/santorinai/board_displayer/board_displayer.py
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)      863 2023-05-14 12:35:43.000000 SantorinAI-1.1.1/santorinai/pawn.py
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)     1485 2023-05-14 12:35:43.000000 SantorinAI-1.1.1/santorinai/player.py
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)     5194 2023-05-14 12:35:43.000000 SantorinAI-1.1.1/santorinai/tester.py
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)       38 2023-05-14 13:39:11.918686 SantorinAI-1.1.1/setup.cfg
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)      697 2023-05-14 13:38:48.000000 SantorinAI-1.1.1/setup.py
-drwxrwxr-x   0 tomansion  (1000) tomansion  (1000)        0 2023-05-14 13:39:11.918686 SantorinAI-1.1.1/test/
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)        0 2023-05-14 12:27:26.000000 SantorinAI-1.1.1/test/__init__.py
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)    17164 2023-05-14 12:27:26.000000 SantorinAI-1.1.1/test/test_board.py
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)      683 2023-05-14 12:27:26.000000 SantorinAI-1.1.1/test/test_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 13:43:37.897210 SantorinAI-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 13:43:24.000000 SantorinAI-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-14 13:43:37.897210 SantorinAI-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-14 13:43:24.000000 SantorinAI-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 13:43:37.897210 SantorinAI-1.1.2/SantorinAI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-14 13:43:37.000000 SantorinAI-1.1.2/SantorinAI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-14 13:43:37.000000 SantorinAI-1.1.2/SantorinAI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 13:43:37.000000 SantorinAI-1.1.2/SantorinAI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 13:43:37.000000 SantorinAI-1.1.2/SantorinAI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-14 13:43:37.000000 SantorinAI-1.1.2/SantorinAI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 13:43:37.897210 SantorinAI-1.1.2/santorinai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 13:43:24.000000 SantorinAI-1.1.2/santorinai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17372 2023-05-14 13:43:24.000000 SantorinAI-1.1.2/santorinai/board.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 13:43:37.897210 SantorinAI-1.1.2/santorinai/board_displayer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 13:43:24.000000 SantorinAI-1.1.2/santorinai/board_displayer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-14 13:43:24.000000 SantorinAI-1.1.2/santorinai/board_displayer/board_displayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-14 13:43:24.000000 SantorinAI-1.1.2/santorinai/pawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-14 13:43:24.000000 SantorinAI-1.1.2/santorinai/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-05-14 13:43:24.000000 SantorinAI-1.1.2/santorinai/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 13:43:37.897210 SantorinAI-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-14 13:43:24.000000 SantorinAI-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 13:43:37.897210 SantorinAI-1.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 13:43:24.000000 SantorinAI-1.1.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17164 2023-05-14 13:43:24.000000 SantorinAI-1.1.2/test/test_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-14 13:43:24.000000 SantorinAI-1.1.2/test/test_tester.py
```

### Comparing `SantorinAI-1.1.1/LICENSE` & `SantorinAI-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.1.1/PKG-INFO` & `SantorinAI-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SantorinAI
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python library for the Santorini board game
 Home-page: https://github.com/tomansion/santorinai
 Author: Tom Mansion
 Author-email: tomansion@yahoo.fr
 Keywords: santorini,ai,boardgame
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `SantorinAI-1.1.1/README.md` & `SantorinAI-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.1.1/SantorinAI.egg-info/PKG-INFO` & `SantorinAI-1.1.2/SantorinAI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SantorinAI
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python library for the Santorini board game
 Home-page: https://github.com/tomansion/santorinai
 Author: Tom Mansion
 Author-email: tomansion@yahoo.fr
 Keywords: santorini,ai,boardgame
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `SantorinAI-1.1.1/santorinai/board.py` & `SantorinAI-1.1.2/santorinai/board.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.1.1/santorinai/board_displayer/board_displayer.py` & `SantorinAI-1.1.2/santorinai/board_displayer/board_displayer.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.1.1/santorinai/pawn.py` & `SantorinAI-1.1.2/santorinai/pawn.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.1.1/santorinai/player.py` & `SantorinAI-1.1.2/santorinai/player.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.1.1/santorinai/tester.py` & `SantorinAI-1.1.2/santorinai/tester.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.1.1/setup.py` & `SantorinAI-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="SantorinAI",
-    version="1.1.1",
+    version="1.1.2",
     author="Tom Mansion",
     author_email="tomansion@yahoo.fr",
     description="A Python library for the Santorini board game",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tomansion/santorinai",
     packages=find_packages(),
```

### Comparing `SantorinAI-1.1.1/test/test_board.py` & `SantorinAI-1.1.2/test/test_board.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.1.1/test/test_tester.py` & `SantorinAI-1.1.2/test/test_tester.py`

 * *Files identical despite different names*

