# Comparing `tmp/wks-0.2.8.tar.gz` & `tmp/wks-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wks-0.2.8.tar", last modified: Sun May 14 09:18:51 2023, max compression
+gzip compressed data, was "wks-0.2.9.tar", last modified: Sun May 14 09:28:54 2023, max compression
```

## Comparing `wks-0.2.8.tar` & `wks-0.2.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-14 09:18:51.612082 wks-0.2.8/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      310 2023-05-14 09:18:51.612082 wks-0.2.8/PKG-INFO
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2480 2023-05-14 09:17:40.000000 wks-0.2.8/README.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       38 2023-05-14 09:18:51.612082 wks-0.2.8/setup.cfg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      629 2023-05-14 09:18:27.000000 wks-0.2.8/setup.py
--rwxrwxr-x   0 gregwar   (1000) gregwar   (1000)      592 2022-09-26 20:46:36.000000 wks-0.2.8/wks
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-14 09:18:51.612082 wks-0.2.8/wks.egg-info/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      310 2023-05-14 09:18:51.000000 wks-0.2.8/wks.egg-info/PKG-INFO
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      489 2023-05-14 09:18:51.000000 wks-0.2.8/wks.egg-info/SOURCES.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        1 2023-05-14 09:18:51.000000 wks-0.2.8/wks.egg-info/dependency_links.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       16 2023-05-14 09:18:51.000000 wks-0.2.8/wks.egg-info/requires.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       10 2023-05-14 09:18:51.000000 wks-0.2.8/wks.egg-info/top_level.txt
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-14 09:18:51.612082 wks-0.2.8/workspace/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       20 2022-09-26 20:46:36.000000 wks-0.2.8/workspace/__init__.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4412 2023-05-14 09:16:16.000000 wks-0.2.8/workspace/cmake.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      914 2022-09-26 20:46:36.000000 wks-0.2.8/workspace/command_build.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      178 2022-09-26 20:46:36.000000 wks-0.2.8/workspace/command_cmake.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      376 2022-09-26 20:46:36.000000 wks-0.2.8/workspace/command_cmd.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1147 2022-09-26 20:46:36.000000 wks-0.2.8/workspace/command_graph.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      716 2022-09-26 20:46:36.000000 wks-0.2.8/workspace/command_help.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      422 2022-09-26 20:46:36.000000 wks-0.2.8/workspace/command_install.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      313 2022-09-26 20:46:36.000000 wks-0.2.8/workspace/command_pull.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1760 2022-09-26 20:46:36.000000 wks-0.2.8/workspace/command_status.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      378 2022-09-26 20:46:36.000000 wks-0.2.8/workspace/commands.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      297 2022-09-26 20:46:36.000000 wks-0.2.8/workspace/env.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5695 2023-05-14 09:18:20.000000 wks-0.2.8/workspace/git.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      620 2022-09-26 20:46:36.000000 wks-0.2.8/workspace/message.py
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-14 09:28:54.444089 wks-0.2.9/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2823 2023-05-14 09:28:54.444089 wks-0.2.9/PKG-INFO
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2480 2023-05-14 09:17:40.000000 wks-0.2.9/README.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       38 2023-05-14 09:28:54.444089 wks-0.2.9/setup.cfg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      625 2023-05-14 09:28:41.000000 wks-0.2.9/setup.py
+-rwxrwxr-x   0 gregwar   (1000) gregwar   (1000)      592 2022-09-26 20:46:36.000000 wks-0.2.9/wks
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-14 09:28:54.444089 wks-0.2.9/wks.egg-info/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2823 2023-05-14 09:28:54.000000 wks-0.2.9/wks.egg-info/PKG-INFO
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      489 2023-05-14 09:28:54.000000 wks-0.2.9/wks.egg-info/SOURCES.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        1 2023-05-14 09:28:54.000000 wks-0.2.9/wks.egg-info/dependency_links.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       16 2023-05-14 09:28:54.000000 wks-0.2.9/wks.egg-info/requires.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       10 2023-05-14 09:28:54.000000 wks-0.2.9/wks.egg-info/top_level.txt
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-14 09:28:54.444089 wks-0.2.9/workspace/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       20 2022-09-26 20:46:36.000000 wks-0.2.9/workspace/__init__.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4412 2023-05-14 09:16:16.000000 wks-0.2.9/workspace/cmake.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      914 2022-09-26 20:46:36.000000 wks-0.2.9/workspace/command_build.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      178 2022-09-26 20:46:36.000000 wks-0.2.9/workspace/command_cmake.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      376 2022-09-26 20:46:36.000000 wks-0.2.9/workspace/command_cmd.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1147 2022-09-26 20:46:36.000000 wks-0.2.9/workspace/command_graph.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      716 2022-09-26 20:46:36.000000 wks-0.2.9/workspace/command_help.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      422 2022-09-26 20:46:36.000000 wks-0.2.9/workspace/command_install.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      313 2022-09-26 20:46:36.000000 wks-0.2.9/workspace/command_pull.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1760 2022-09-26 20:46:36.000000 wks-0.2.9/workspace/command_status.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      378 2022-09-26 20:46:36.000000 wks-0.2.9/workspace/commands.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      297 2022-09-26 20:46:36.000000 wks-0.2.9/workspace/env.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5695 2023-05-14 09:18:20.000000 wks-0.2.9/workspace/git.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      620 2022-09-26 20:46:36.000000 wks-0.2.9/workspace/message.py
```

### Comparing `wks-0.2.8/README.md` & `wks-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `wks-0.2.8/setup.py` & `wks-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="wks",
-    version="0.2.8",
+    version="0.2.9",
     author="Rhoban team",
     author_email="team@rhoban.com",
     description="Simple dependencies manager for cmake projects in your workspace",
-    # long_description=long_description,
-    # long_description_content_type="text/markdown",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     url="https://github.com/rhoban/wks/",
     packages=setuptools.find_packages(),
     scripts=["wks"],
     keywords="wks workspace deps",
     install_requires=["colorama", "pyyaml"],
     include_package_data=True,
     python_requires=">=3.6",
```

### Comparing `wks-0.2.8/wks` & `wks-0.2.9/wks`

 * *Files identical despite different names*

### Comparing `wks-0.2.8/workspace/cmake.py` & `wks-0.2.9/workspace/cmake.py`

 * *Files identical despite different names*

### Comparing `wks-0.2.8/workspace/command_build.py` & `wks-0.2.9/workspace/command_build.py`

 * *Files identical despite different names*

### Comparing `wks-0.2.8/workspace/command_graph.py` & `wks-0.2.9/workspace/command_graph.py`

 * *Files identical despite different names*

### Comparing `wks-0.2.8/workspace/command_help.py` & `wks-0.2.9/workspace/command_help.py`

 * *Files identical despite different names*

### Comparing `wks-0.2.8/workspace/command_status.py` & `wks-0.2.9/workspace/command_status.py`

 * *Files identical despite different names*

### Comparing `wks-0.2.8/workspace/git.py` & `wks-0.2.9/workspace/git.py`

 * *Files identical despite different names*

### Comparing `wks-0.2.8/workspace/message.py` & `wks-0.2.9/workspace/message.py`

 * *Files identical despite different names*

