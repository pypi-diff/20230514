# Comparing `tmp/SantorinAI-1.0.0.tar.gz` & `tmp/SantorinAI-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SantorinAI-1.0.0.tar", last modified: Sun May 14 13:10:33 2023, max compression
+gzip compressed data, was "SantorinAI-1.1.1.tar", last modified: Sun May 14 13:39:11 2023, max compression
```

## Comparing `SantorinAI-1.0.0.tar` & `SantorinAI-1.1.1.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxr-x   0 tomansion  (1000) tomansion  (1000)        0 2023-05-14 13:10:33.407189 SantorinAI-1.0.0/
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)    11357 2023-05-14 12:45:31.000000 SantorinAI-1.0.0/LICENSE
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)    17686 2023-05-14 13:10:33.407189 SantorinAI-1.0.0/PKG-INFO
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)     4166 2023-05-14 12:27:26.000000 SantorinAI-1.0.0/README.md
-drwxrwxr-x   0 tomansion  (1000) tomansion  (1000)        0 2023-05-14 13:10:33.407189 SantorinAI-1.0.0/SantorinAI.egg-info/
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)    17686 2023-05-14 13:10:33.000000 SantorinAI-1.0.0/SantorinAI.egg-info/PKG-INFO
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)      370 2023-05-14 13:10:33.000000 SantorinAI-1.0.0/SantorinAI.egg-info/SOURCES.txt
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)        1 2023-05-14 13:10:33.000000 SantorinAI-1.0.0/SantorinAI.egg-info/dependency_links.txt
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)       51 2023-05-14 13:10:33.000000 SantorinAI-1.0.0/SantorinAI.egg-info/requires.txt
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)       16 2023-05-14 13:10:33.000000 SantorinAI-1.0.0/SantorinAI.egg-info/top_level.txt
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)      694 2023-05-14 13:10:24.000000 SantorinAI-1.0.0/pyproject.toml
-drwxrwxr-x   0 tomansion  (1000) tomansion  (1000)        0 2023-05-14 13:10:33.407189 SantorinAI-1.0.0/santorinai/
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)        0 2023-05-14 12:35:43.000000 SantorinAI-1.0.0/santorinai/__init__.py
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)    17372 2023-05-14 12:35:43.000000 SantorinAI-1.0.0/santorinai/board.py
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)      863 2023-05-14 12:35:43.000000 SantorinAI-1.0.0/santorinai/pawn.py
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)     1485 2023-05-14 12:35:43.000000 SantorinAI-1.0.0/santorinai/player.py
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)     5194 2023-05-14 12:35:43.000000 SantorinAI-1.0.0/santorinai/tester.py
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)       38 2023-05-14 13:10:33.407189 SantorinAI-1.0.0/setup.cfg
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)      631 2023-05-14 12:42:07.000000 SantorinAI-1.0.0/setup.py
-drwxrwxr-x   0 tomansion  (1000) tomansion  (1000)        0 2023-05-14 13:10:33.407189 SantorinAI-1.0.0/test/
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)        0 2023-05-14 12:27:26.000000 SantorinAI-1.0.0/test/__init__.py
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)    17164 2023-05-14 12:27:26.000000 SantorinAI-1.0.0/test/test_board.py
--rw-rw-r--   0 tomansion  (1000) tomansion  (1000)      683 2023-05-14 12:27:26.000000 SantorinAI-1.0.0/test/test_tester.py
+drwxrwxr-x   0 tomansion  (1000) tomansion  (1000)        0 2023-05-14 13:39:11.918686 SantorinAI-1.1.1/
+-rw-rw-r--   0 tomansion  (1000) tomansion  (1000)    11357 2023-05-14 12:45:31.000000 SantorinAI-1.1.1/LICENSE
+-rw-rw-r--   0 tomansion  (1000) tomansion  (1000)     4768 2023-05-14 13:39:11.918686 SantorinAI-1.1.1/PKG-INFO
+-rw-rw-r--   0 tomansion  (1000) tomansion  (1000)     4282 2023-05-14 13:23:42.000000 SantorinAI-1.1.1/README.md
+drwxrwxr-x   0 tomansion  (1000) tomansion  (1000)        0 2023-05-14 13:39:11.914685 SantorinAI-1.1.1/SantorinAI.egg-info/
+-rw-rw-r--   0 tomansion  (1000) tomansion  (1000)     4768 2023-05-14 13:39:11.000000 SantorinAI-1.1.1/SantorinAI.egg-info/PKG-INFO
+-rw-rw-r--   0 tomansion  (1000) tomansion  (1000)      440 2023-05-14 13:39:11.000000 SantorinAI-1.1.1/SantorinAI.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomansion  (1000) tomansion  (1000)        1 2023-05-14 13:39:11.000000 SantorinAI-1.1.1/SantorinAI.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomansion  (1000) tomansion  (1000)       12 2023-05-14 13:39:11.000000 SantorinAI-1.1.1/SantorinAI.egg-info/requires.txt
+-rw-rw-r--   0 tomansion  (1000) tomansion  (1000)       16 2023-05-14 13:39:11.000000 SantorinAI-1.1.1/SantorinAI.egg-info/top_level.txt
+drwxrwxr-x   0 tomansion  (1000) tomansion  (1000)        0 2023-05-14 13:39:11.914685 SantorinAI-1.1.1/santorinai/
+-rw-rw-r--   0 tomansion  (1000) tomansion  (1000)        0 2023-05-14 12:35:43.000000 SantorinAI-1.1.1/santorinai/__init__.py
+-rw-rw-r--   0 tomansion  (1000) tomansion  (1000)    17372 2023-05-14 12:35:43.000000 SantorinAI-1.1.1/santorinai/board.py
+drwxrwxr-x   0 tomansion  (1000) tomansion  (1000)        0 2023-05-14 13:39:11.914685 SantorinAI-1.1.1/santorinai/board_displayer/
+-rw-rw-r--   0 tomansion  (1000) tomansion  (1000)        0 2023-05-14 13:22:31.000000 SantorinAI-1.1.1/santorinai/board_displayer/__init__.py
+-rw-rw-r--   0 tomansion  (1000) tomansion  (1000)     6990 2023-05-14 12:35:43.000000 SantorinAI-1.1.1/santorinai/board_displayer/board_displayer.py
+-rw-rw-r--   0 tomansion  (1000) tomansion  (1000)      863 2023-05-14 12:35:43.000000 SantorinAI-1.1.1/santorinai/pawn.py
+-rw-rw-r--   0 tomansion  (1000) tomansion  (1000)     1485 2023-05-14 12:35:43.000000 SantorinAI-1.1.1/santorinai/player.py
+-rw-rw-r--   0 tomansion  (1000) tomansion  (1000)     5194 2023-05-14 12:35:43.000000 SantorinAI-1.1.1/santorinai/tester.py
+-rw-rw-r--   0 tomansion  (1000) tomansion  (1000)       38 2023-05-14 13:39:11.918686 SantorinAI-1.1.1/setup.cfg
+-rw-rw-r--   0 tomansion  (1000) tomansion  (1000)      697 2023-05-14 13:38:48.000000 SantorinAI-1.1.1/setup.py
+drwxrwxr-x   0 tomansion  (1000) tomansion  (1000)        0 2023-05-14 13:39:11.918686 SantorinAI-1.1.1/test/
+-rw-rw-r--   0 tomansion  (1000) tomansion  (1000)        0 2023-05-14 12:27:26.000000 SantorinAI-1.1.1/test/__init__.py
+-rw-rw-r--   0 tomansion  (1000) tomansion  (1000)    17164 2023-05-14 12:27:26.000000 SantorinAI-1.1.1/test/test_board.py
+-rw-rw-r--   0 tomansion  (1000) tomansion  (1000)      683 2023-05-14 12:27:26.000000 SantorinAI-1.1.1/test/test_tester.py
```

### Comparing `SantorinAI-1.0.0/LICENSE` & `SantorinAI-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.0.0/README.md` & `SantorinAI-1.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 ![Graphical output example](./images/headban.png)
 
 # SantorinAI
 AI Player tester for the Santorini game
 
 ## How to use
 ### 1. Install
+
+With pip:
+```bash
+pip install santorinai --upgrade
+```
+
+You can also clone the repository and install it manually:
 ```bash
 git clone https://github.com/Tomansion/SantorinAI.git
 cd SantorinAI
 pip install -r requirements.txt
 ```
 
 ### 2. Create a player
```

### Comparing `SantorinAI-1.0.0/santorinai/board.py` & `SantorinAI-1.1.1/santorinai/board.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.0.0/santorinai/pawn.py` & `SantorinAI-1.1.1/santorinai/pawn.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.0.0/santorinai/player.py` & `SantorinAI-1.1.1/santorinai/player.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.0.0/santorinai/tester.py` & `SantorinAI-1.1.1/santorinai/tester.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.0.0/setup.py` & `SantorinAI-1.1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
-    name="SantoriAI",
-    version="1.0.0",
+    name="SantorinAI",
+    version="1.1.1",
     author="Tom Mansion",
     author_email="tomansion@yahoo.fr",
     description="A Python library for the Santorini board game",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tomansion/santorinai",
     packages=find_packages(),
     classifiers=[
-        "Development Status :: 3 - Alpha",
-        "Intended Audience :: Developers",
+        "License :: OSI Approved :: Apache Software License",
+        "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
+    keywords=["santorini", "ai", "boardgame"],
     python_requires=">=3.6",
     install_requires=["pysimplegui"],
 )
```

### Comparing `SantorinAI-1.0.0/test/test_board.py` & `SantorinAI-1.1.1/test/test_board.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.0.0/test/test_tester.py` & `SantorinAI-1.1.1/test/test_tester.py`

 * *Files identical despite different names*

