# Comparing `tmp/wks-0.2.7.tar.gz` & `tmp/wks-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wks-0.2.7.tar", last modified: Mon Apr 17 12:00:16 2023, max compression
+gzip compressed data, was "wks-0.2.8.tar", last modified: Sun May 14 09:18:51 2023, max compression
```

## Comparing `wks-0.2.7.tar` & `wks-0.2.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-17 12:00:16.637341 wks-0.2.7/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      310 2023-04-17 12:00:16.637341 wks-0.2.7/PKG-INFO
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2306 2022-03-24 13:57:35.000000 wks-0.2.7/README.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       38 2023-04-17 12:00:16.637341 wks-0.2.7/setup.cfg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      629 2023-04-17 11:58:08.000000 wks-0.2.7/setup.py
--rwxrwxr-x   0 gregwar   (1000) gregwar   (1000)      592 2021-06-24 13:33:28.000000 wks-0.2.7/wks
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-17 12:00:16.633340 wks-0.2.7/wks.egg-info/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      310 2023-04-17 12:00:16.000000 wks-0.2.7/wks.egg-info/PKG-INFO
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      489 2023-04-17 12:00:16.000000 wks-0.2.7/wks.egg-info/SOURCES.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        1 2023-04-17 12:00:16.000000 wks-0.2.7/wks.egg-info/dependency_links.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       16 2023-04-17 12:00:16.000000 wks-0.2.7/wks.egg-info/requires.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       10 2023-04-17 12:00:16.000000 wks-0.2.7/wks.egg-info/top_level.txt
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-17 12:00:16.637341 wks-0.2.7/workspace/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       20 2022-06-14 09:00:39.000000 wks-0.2.7/workspace/__init__.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4235 2022-06-14 09:00:39.000000 wks-0.2.7/workspace/cmake.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      914 2023-04-17 11:59:39.000000 wks-0.2.7/workspace/command_build.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      178 2022-06-14 09:00:39.000000 wks-0.2.7/workspace/command_cmake.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      376 2022-06-14 09:00:39.000000 wks-0.2.7/workspace/command_cmd.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1147 2022-06-14 09:00:39.000000 wks-0.2.7/workspace/command_graph.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      716 2022-06-14 09:00:39.000000 wks-0.2.7/workspace/command_help.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      422 2022-06-14 09:00:39.000000 wks-0.2.7/workspace/command_install.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      313 2022-10-20 08:37:11.000000 wks-0.2.7/workspace/command_pull.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1760 2022-06-14 09:00:39.000000 wks-0.2.7/workspace/command_status.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      378 2022-06-14 09:00:39.000000 wks-0.2.7/workspace/commands.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      297 2022-06-14 09:00:39.000000 wks-0.2.7/workspace/env.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5695 2023-04-17 11:59:13.000000 wks-0.2.7/workspace/git.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      620 2022-06-14 09:00:39.000000 wks-0.2.7/workspace/message.py
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-14 09:18:51.612082 wks-0.2.8/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      310 2023-05-14 09:18:51.612082 wks-0.2.8/PKG-INFO
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2480 2023-05-14 09:17:40.000000 wks-0.2.8/README.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       38 2023-05-14 09:18:51.612082 wks-0.2.8/setup.cfg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      629 2023-05-14 09:18:27.000000 wks-0.2.8/setup.py
+-rwxrwxr-x   0 gregwar   (1000) gregwar   (1000)      592 2022-09-26 20:46:36.000000 wks-0.2.8/wks
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-14 09:18:51.612082 wks-0.2.8/wks.egg-info/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      310 2023-05-14 09:18:51.000000 wks-0.2.8/wks.egg-info/PKG-INFO
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      489 2023-05-14 09:18:51.000000 wks-0.2.8/wks.egg-info/SOURCES.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        1 2023-05-14 09:18:51.000000 wks-0.2.8/wks.egg-info/dependency_links.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       16 2023-05-14 09:18:51.000000 wks-0.2.8/wks.egg-info/requires.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       10 2023-05-14 09:18:51.000000 wks-0.2.8/wks.egg-info/top_level.txt
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-14 09:18:51.612082 wks-0.2.8/workspace/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       20 2022-09-26 20:46:36.000000 wks-0.2.8/workspace/__init__.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4412 2023-05-14 09:16:16.000000 wks-0.2.8/workspace/cmake.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      914 2022-09-26 20:46:36.000000 wks-0.2.8/workspace/command_build.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      178 2022-09-26 20:46:36.000000 wks-0.2.8/workspace/command_cmake.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      376 2022-09-26 20:46:36.000000 wks-0.2.8/workspace/command_cmd.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1147 2022-09-26 20:46:36.000000 wks-0.2.8/workspace/command_graph.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      716 2022-09-26 20:46:36.000000 wks-0.2.8/workspace/command_help.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      422 2022-09-26 20:46:36.000000 wks-0.2.8/workspace/command_install.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      313 2022-09-26 20:46:36.000000 wks-0.2.8/workspace/command_pull.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1760 2022-09-26 20:46:36.000000 wks-0.2.8/workspace/command_status.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      378 2022-09-26 20:46:36.000000 wks-0.2.8/workspace/commands.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      297 2022-09-26 20:46:36.000000 wks-0.2.8/workspace/env.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5695 2023-05-14 09:18:20.000000 wks-0.2.8/workspace/git.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      620 2022-09-26 20:46:36.000000 wks-0.2.8/workspace/message.py
```

### Comparing `wks-0.2.7/README.md` & `wks-0.2.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 * `vendor/repository@tag`
 
 ## The `wks.yml` file
 
 The `wks.yml` can contain the following sections:
 
 * `deps`: a list of dependencies that the repository want to be installed
+* `optional`: a list of optional dependencies, they will not be installed but it ensure that the projects will appear
+  in the proper order in the generated `CMakeLists.txt`
 * `cmakes`: if the `CMakeLists.txt` for this repository is not at the top level (or not unique), you can specify them
   using this section
 * `install`: a list of shell command that should be run post install
 * `cmake_prefix`: a list of directories to be added to `CMAKE_PREFIX_PATH`
 
 An example is:
```

### Comparing `wks-0.2.7/setup.py` & `wks-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="wks",
-    version="0.2.7",
+    version="0.2.8",
     author="Rhoban team",
     author_email="team@rhoban.com",
     description="Simple dependencies manager for cmake projects in your workspace",
     # long_description=long_description,
     # long_description_content_type="text/markdown",
     url="https://github.com/rhoban/wks/",
     packages=setuptools.find_packages(),
```

### Comparing `wks-0.2.7/wks` & `wks-0.2.8/wks`

 * *Files identical despite different names*

### Comparing `wks-0.2.7/workspace/cmake.py` & `wks-0.2.8/workspace/cmake.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,18 +95,25 @@
 
         if directory not in added:
             added.add(directory)
             config = env.get_config(directory)
             if config and "cmake_prefixes" in config:
                 for entry in config["cmake_prefixes"]:
                     prefix_path.append(directory + "/" + entry)
+
+            dependencies = []
+
             if config and "deps" in config:
-                for dep in config["deps"]:
-                    dep_directory = git.parse_repository_name(dep)["directory"]
-                    add_project(dep_directory)
+                dependencies += config["deps"]
+            if config and "optional" in config:
+                dependencies += config["optional"]
+            
+            for dep in dependencies:
+                dep_directory = git.parse_repository_name(dep)["directory"]
+                add_project(dep_directory)
 
             add_cmake(directory)
 
     for directory in git.get_directories():
         add_project(directory)
 
     prefix_paths = ""
```

### Comparing `wks-0.2.7/workspace/command_build.py` & `wks-0.2.8/workspace/command_build.py`

 * *Files identical despite different names*

### Comparing `wks-0.2.7/workspace/command_graph.py` & `wks-0.2.8/workspace/command_graph.py`

 * *Files identical despite different names*

### Comparing `wks-0.2.7/workspace/command_help.py` & `wks-0.2.8/workspace/command_help.py`

 * *Files identical despite different names*

### Comparing `wks-0.2.7/workspace/command_status.py` & `wks-0.2.8/workspace/command_status.py`

 * *Files identical despite different names*

### Comparing `wks-0.2.7/workspace/git.py` & `wks-0.2.8/workspace/git.py`

 * *Files identical despite different names*

### Comparing `wks-0.2.7/workspace/message.py` & `wks-0.2.8/workspace/message.py`

 * *Files identical despite different names*

