# Comparing `tmp/benchmarx-0.0.2.tar.gz` & `tmp/benchmarx-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benchmarx-0.0.2.tar", last modified: Sun May 14 21:11:57 2023, max compression
+gzip compressed data, was "benchmarx-0.0.3.tar", last modified: Sun May 14 21:27:36 2023, max compression
```

## Comparing `benchmarx-0.0.2.tar` & `benchmarx-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 aleksandrtrisin   (501) staff       (20)        0 2023-05-14 21:11:57.757991 benchmarx-0.0.2/
--rw-r--r--   0 aleksandrtrisin   (501) staff       (20)     1074 2023-05-12 10:09:01.000000 benchmarx-0.0.2/LICENSE
--rw-r--r--   0 aleksandrtrisin   (501) staff       (20)      601 2023-05-14 21:11:57.757856 benchmarx-0.0.2/PKG-INFO
--rw-r--r--   0 aleksandrtrisin   (501) staff       (20)       12 2023-05-13 21:44:46.000000 benchmarx-0.0.2/README.md
-drwxr-xr-x   0 aleksandrtrisin   (501) staff       (20)        0 2023-05-14 21:11:57.756205 benchmarx-0.0.2/benchmarx/
-drwxr-xr-x   0 aleksandrtrisin   (501) staff       (20)        0 2023-05-14 21:11:57.757653 benchmarx-0.0.2/benchmarx/benchmarx.egg-info/
--rw-r--r--   0 aleksandrtrisin   (501) staff       (20)      601 2023-05-14 21:11:57.000000 benchmarx-0.0.2/benchmarx/benchmarx.egg-info/PKG-INFO
--rw-r--r--   0 aleksandrtrisin   (501) staff       (20)      255 2023-05-14 21:11:57.000000 benchmarx-0.0.2/benchmarx/benchmarx.egg-info/SOURCES.txt
--rw-r--r--   0 aleksandrtrisin   (501) staff       (20)        1 2023-05-14 21:11:57.000000 benchmarx-0.0.2/benchmarx/benchmarx.egg-info/dependency_links.txt
--rw-r--r--   0 aleksandrtrisin   (501) staff       (20)      117 2023-05-14 21:11:57.000000 benchmarx-0.0.2/benchmarx/benchmarx.egg-info/requires.txt
--rw-r--r--   0 aleksandrtrisin   (501) staff       (20)        1 2023-05-14 21:11:57.000000 benchmarx-0.0.2/benchmarx/benchmarx.egg-info/top_level.txt
--rw-r--r--   0 aleksandrtrisin   (501) staff       (20)      572 2023-05-14 21:11:55.000000 benchmarx-0.0.2/pyproject.toml
--rw-r--r--   0 aleksandrtrisin   (501) staff       (20)       38 2023-05-14 21:11:57.758035 benchmarx-0.0.2/setup.cfg
--rw-r--r--   0 aleksandrtrisin   (501) staff       (20)      975 2023-05-14 21:11:49.000000 benchmarx-0.0.2/setup.py
+drwxr-xr-x   0 aleksandrtrisin   (501) staff       (20)        0 2023-05-14 21:27:36.699464 benchmarx-0.0.3/
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)     1074 2023-05-12 10:09:01.000000 benchmarx-0.0.3/LICENSE
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)      601 2023-05-14 21:27:36.699318 benchmarx-0.0.3/PKG-INFO
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)       12 2023-05-13 21:44:46.000000 benchmarx-0.0.3/README.md
+drwxr-xr-x   0 aleksandrtrisin   (501) staff       (20)        0 2023-05-14 21:27:36.697655 benchmarx-0.0.3/benchmarx/
+drwxr-xr-x   0 aleksandrtrisin   (501) staff       (20)        0 2023-05-14 21:27:36.699107 benchmarx-0.0.3/benchmarx/benchmarx.egg-info/
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)      601 2023-05-14 21:27:36.000000 benchmarx-0.0.3/benchmarx/benchmarx.egg-info/PKG-INFO
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)      255 2023-05-14 21:27:36.000000 benchmarx-0.0.3/benchmarx/benchmarx.egg-info/SOURCES.txt
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)        1 2023-05-14 21:27:36.000000 benchmarx-0.0.3/benchmarx/benchmarx.egg-info/dependency_links.txt
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)      117 2023-05-14 21:27:36.000000 benchmarx-0.0.3/benchmarx/benchmarx.egg-info/requires.txt
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)        1 2023-05-14 21:27:36.000000 benchmarx-0.0.3/benchmarx/benchmarx.egg-info/top_level.txt
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)      572 2023-05-14 21:26:34.000000 benchmarx-0.0.3/pyproject.toml
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)       38 2023-05-14 21:27:36.699513 benchmarx-0.0.3/setup.cfg
+-rw-r--r--   0 aleksandrtrisin   (501) staff       (20)      975 2023-05-14 21:27:34.000000 benchmarx-0.0.3/setup.py
```

### Comparing `benchmarx-0.0.2/LICENSE` & `benchmarx-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `benchmarx-0.0.2/PKG-INFO` & `benchmarx-0.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: benchmarx
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tools for benchmarking optimization methods
 Home-page: https://github.com/AlexToW/benchmarx
 Author: AlexToW
 Author-email: Salex <31salex31@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/AlexToW/benchmarx
 Project-URL: Bug Tracker, https://github.com/AlexToW/benchmarx/issues
```

### Comparing `benchmarx-0.0.2/benchmarx/benchmarx.egg-info/PKG-INFO` & `benchmarx-0.0.3/benchmarx/benchmarx.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: benchmarx
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tools for benchmarking optimization methods
 Home-page: https://github.com/AlexToW/benchmarx
 Author: AlexToW
 Author-email: Salex <31salex31@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/AlexToW/benchmarx
 Project-URL: Bug Tracker, https://github.com/AlexToW/benchmarx/issues
```

### Comparing `benchmarx-0.0.2/pyproject.toml` & `benchmarx-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "benchmarx"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Salex", email="31salex31@gmail.com" },
 ]
 description = "Tools for benchmarking optimization methods"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `benchmarx-0.0.2/setup.py` & `benchmarx-0.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 setup(
     name="benchmarx",
-    version="0.0.2",
+    version="0.0.3",
     description="Tools for benchmarking optimization methods",
     package_dir={"" : "benchmarx"},
     packages=find_packages(where="benchmarx"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AlexToW/benchmarx",
     author="AlexToW",
@@ -23,14 +23,14 @@
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "jax",
         "jaxopt >= 0.6",
         "typing-extensions >= 4.5.0",
         "wandb >= 0.14.2",
-        "pandas >= 2.0.1",
+        "pandas == 1.5.3",
         "plotly >= 5.14.1",
         "flax >= 0.6.10",
         "tensorflow_datasets"
     ],
     python_requires=">=3.7",
 )
```

