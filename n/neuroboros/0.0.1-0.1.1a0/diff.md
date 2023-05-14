# Comparing `tmp/neuroboros-0.0.1.tar.gz` & `tmp/neuroboros-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroboros-0.0.1.tar", last modified: Fri Nov 11 21:51:40 2022, max compression
+gzip compressed data, was "neuroboros-0.1.1a0.tar", last modified: Sun May 14 00:54:20 2023, max compression
```

## Comparing `neuroboros-0.0.1.tar` & `neuroboros-0.1.1a0.tar`

### file list

```diff
@@ -1,14 +1,44 @@
-drwxr-xr-x   0 feilong    (501) staff       (20)        0 2022-11-11 21:51:40.119729 neuroboros-0.0.1/
--rw-r--r--   0 feilong    (501) staff       (20)     1067 2022-11-11 21:40:29.000000 neuroboros-0.0.1/LICENSE
--rw-r--r--   0 feilong    (501) staff       (20)     1900 2022-11-11 21:51:40.119584 neuroboros-0.0.1/PKG-INFO
--rw-r--r--   0 feilong    (501) staff       (20)      853 2022-11-11 21:50:56.000000 neuroboros-0.0.1/pyproject.toml
--rw-r--r--   0 feilong    (501) staff       (20)       38 2022-11-11 21:51:40.119773 neuroboros-0.0.1/setup.cfg
-drwxr-xr-x   0 feilong    (501) staff       (20)        0 2022-11-11 21:51:40.118508 neuroboros-0.0.1/src/
-drwxr-xr-x   0 feilong    (501) staff       (20)        0 2022-11-11 21:51:40.118845 neuroboros-0.0.1/src/neuroboros/
--rw-r--r--   0 feilong    (501) staff       (20)        0 2022-11-11 21:46:01.000000 neuroboros-0.0.1/src/neuroboros/__init__.py
-drwxr-xr-x   0 feilong    (501) staff       (20)        0 2022-11-11 21:51:40.119423 neuroboros-0.0.1/src/neuroboros.egg-info/
--rw-r--r--   0 feilong    (501) staff       (20)     1900 2022-11-11 21:51:40.000000 neuroboros-0.0.1/src/neuroboros.egg-info/PKG-INFO
--rw-r--r--   0 feilong    (501) staff       (20)      238 2022-11-11 21:51:40.000000 neuroboros-0.0.1/src/neuroboros.egg-info/SOURCES.txt
--rw-r--r--   0 feilong    (501) staff       (20)        1 2022-11-11 21:51:40.000000 neuroboros-0.0.1/src/neuroboros.egg-info/dependency_links.txt
--rw-r--r--   0 feilong    (501) staff       (20)        6 2022-11-11 21:51:40.000000 neuroboros-0.0.1/src/neuroboros.egg-info/requires.txt
--rw-r--r--   0 feilong    (501) staff       (20)       11 2022-11-11 21:51:40.000000 neuroboros-0.0.1/src/neuroboros.egg-info/top_level.txt
+drwxr-xr-x   0 feilong    (501) staff       (20)        0 2023-05-14 00:54:20.615733 neuroboros-0.1.1a0/
+-rw-r--r--   0 feilong    (501) staff       (20)     1067 2023-05-13 20:00:07.000000 neuroboros-0.1.1a0/LICENSE
+-rw-r--r--   0 feilong    (501) staff       (20)       69 2023-05-13 22:37:48.000000 neuroboros-0.1.1a0/MANIFEST.in
+-rw-r--r--   0 feilong    (501) staff       (20)     1908 2023-05-14 00:54:20.615598 neuroboros-0.1.1a0/PKG-INFO
+drwxr-xr-x   0 feilong    (501) staff       (20)        0 2023-05-14 00:54:20.610149 neuroboros-0.1.1a0/bin/
+-rw-r--r--   0 feilong    (501) staff       (20)      771 2023-05-13 20:00:07.000000 neuroboros-0.1.1a0/bin/npls
+-rw-r--r--   0 feilong    (501) staff       (20)      303 2023-05-13 20:00:07.000000 neuroboros-0.1.1a0/bin/rmdirs
+drwxr-xr-x   0 feilong    (501) staff       (20)        0 2023-05-14 00:54:20.608769 neuroboros-0.1.1a0/neuroboros/
+drwxr-xr-x   0 feilong    (501) staff       (20)        0 2023-05-14 00:54:20.611212 neuroboros-0.1.1a0/neuroboros/surface/
+-rw-r--r--   0 feilong    (501) staff       (20)   342667 2023-05-14 00:54:20.000000 neuroboros-0.1.1a0/neuroboros/surface/_barycentric.c
+-rw-r--r--   0 feilong    (501) staff       (20)     2746 2023-05-13 20:00:07.000000 neuroboros-0.1.1a0/neuroboros/surface/_barycentric.pyx
+-rw-r--r--   0 feilong    (501) staff       (20)      968 2023-05-13 22:38:51.000000 neuroboros-0.1.1a0/pyproject.toml
+-rw-r--r--   0 feilong    (501) staff       (20)       38 2023-05-14 00:54:20.615776 neuroboros-0.1.1a0/setup.cfg
+-rw-r--r--   0 feilong    (501) staff       (20)      243 2023-05-13 22:35:03.000000 neuroboros-0.1.1a0/setup.py
+drwxr-xr-x   0 feilong    (501) staff       (20)        0 2023-05-14 00:54:20.608998 neuroboros-0.1.1a0/src/
+drwxr-xr-x   0 feilong    (501) staff       (20)        0 2023-05-14 00:54:20.612197 neuroboros-0.1.1a0/src/neuroboros/
+-rw-r--r--   0 feilong    (501) staff       (20)      802 2023-05-13 20:00:07.000000 neuroboros-0.1.1a0/src/neuroboros/__init__.py
+drwxr-xr-x   0 feilong    (501) staff       (20)        0 2023-05-14 00:54:20.612974 neuroboros-0.1.1a0/src/neuroboros/datasets/
+-rw-r--r--   0 feilong    (501) staff       (20)    14641 2023-05-13 20:00:07.000000 neuroboros-0.1.1a0/src/neuroboros/datasets/__init__.py
+-rw-r--r--   0 feilong    (501) staff       (20)     1623 2023-05-13 20:00:07.000000 neuroboros-0.1.1a0/src/neuroboros/io.py
+-rw-r--r--   0 feilong    (501) staff       (20)     3823 2023-05-13 20:00:07.000000 neuroboros-0.1.1a0/src/neuroboros/linalg.py
+-rw-r--r--   0 feilong    (501) staff       (20)    10008 2023-05-14 00:50:31.000000 neuroboros-0.1.1a0/src/neuroboros/plot2d.py
+-rw-r--r--   0 feilong    (501) staff       (20)     3355 2023-05-13 20:00:07.000000 neuroboros-0.1.1a0/src/neuroboros/searchlights.py
+-rw-r--r--   0 feilong    (501) staff       (20)    12590 2023-05-13 20:00:07.000000 neuroboros-0.1.1a0/src/neuroboros/spaces.py
+drwxr-xr-x   0 feilong    (501) staff       (20)        0 2023-05-14 00:54:20.615236 neuroboros-0.1.1a0/src/neuroboros/surface/
+-rw-r--r--   0 feilong    (501) staff       (20)     5469 2023-05-13 20:00:07.000000 neuroboros-0.1.1a0/src/neuroboros/surface/__init__.py
+-rw-r--r--   0 feilong    (501) staff       (20)   342667 2023-05-14 00:54:20.000000 neuroboros-0.1.1a0/src/neuroboros/surface/_barycentric.c
+-rw-r--r--   0 feilong    (501) staff       (20)     2746 2023-05-13 20:00:07.000000 neuroboros-0.1.1a0/src/neuroboros/surface/_barycentric.pyx
+-rw-r--r--   0 feilong    (501) staff       (20)     2235 2023-05-13 20:00:07.000000 neuroboros-0.1.1a0/src/neuroboros/surface/areal.py
+-rw-r--r--   0 feilong    (501) staff       (20)     1224 2023-05-13 20:00:07.000000 neuroboros-0.1.1a0/src/neuroboros/surface/barycentric.py
+-rw-r--r--   0 feilong    (501) staff       (20)     3439 2023-05-13 20:00:07.000000 neuroboros-0.1.1a0/src/neuroboros/surface/dijkstra.py
+-rw-r--r--   0 feilong    (501) staff       (20)     1004 2023-05-13 20:00:07.000000 neuroboros-0.1.1a0/src/neuroboros/surface/nnfr.py
+-rw-r--r--   0 feilong    (501) staff       (20)     2332 2023-05-13 20:00:07.000000 neuroboros-0.1.1a0/src/neuroboros/surface/properties.py
+-rw-r--r--   0 feilong    (501) staff       (20)     3530 2023-05-13 20:00:07.000000 neuroboros-0.1.1a0/src/neuroboros/surface/subdivision.py
+-rw-r--r--   0 feilong    (501) staff       (20)     1790 2023-05-13 20:00:07.000000 neuroboros-0.1.1a0/src/neuroboros/surface/union.py
+-rw-r--r--   0 feilong    (501) staff       (20)     8286 2023-05-13 20:00:07.000000 neuroboros-0.1.1a0/src/neuroboros/surface/voronoi.py
+drwxr-xr-x   0 feilong    (501) staff       (20)        0 2023-05-14 00:54:20.615401 neuroboros-0.1.1a0/src/neuroboros/utils/
+-rw-r--r--   0 feilong    (501) staff       (20)    14036 2023-05-13 20:00:07.000000 neuroboros-0.1.1a0/src/neuroboros/utils/__init__.py
+drwxr-xr-x   0 feilong    (501) staff       (20)        0 2023-05-14 00:54:20.612858 neuroboros-0.1.1a0/src/neuroboros.egg-info/
+-rw-r--r--   0 feilong    (501) staff       (20)     1908 2023-05-14 00:54:20.000000 neuroboros-0.1.1a0/src/neuroboros.egg-info/PKG-INFO
+-rw-r--r--   0 feilong    (501) staff       (20)      935 2023-05-14 00:54:20.000000 neuroboros-0.1.1a0/src/neuroboros.egg-info/SOURCES.txt
+-rw-r--r--   0 feilong    (501) staff       (20)        1 2023-05-14 00:54:20.000000 neuroboros-0.1.1a0/src/neuroboros.egg-info/dependency_links.txt
+-rw-r--r--   0 feilong    (501) staff       (20)       60 2023-05-14 00:54:20.000000 neuroboros-0.1.1a0/src/neuroboros.egg-info/requires.txt
+-rw-r--r--   0 feilong    (501) staff       (20)       11 2023-05-14 00:54:20.000000 neuroboros-0.1.1a0/src/neuroboros.egg-info/top_level.txt
```

### Comparing `neuroboros-0.0.1/LICENSE` & `neuroboros-0.1.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroboros-0.0.1/PKG-INFO` & `neuroboros-0.1.1a0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuroboros
-Version: 0.0.1
+Version: 0.1.1a0
 Summary: Neuroimaging analysis in Python
 Author-email: Ma Feilong <mafeilong@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Feilong Ma
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,16 +21,16 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/feilong/neuroboros
-Project-URL: Bug Tracker, https://github.com/feilong/neuroboros/issues
+Project-URL: Homepage, https://github.com/neuroboros/neuroboros
+Project-URL: Bug Tracker, https://github.com/neuroboros/neuroboros/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
```

### Comparing `neuroboros-0.0.1/pyproject.toml` & `neuroboros-0.1.1a0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "Cython",
   "numpy",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neuroboros"
-version = "0.0.1"
+version = "0.1.1.alpha"
 authors = [
   { name="Ma Feilong", email="mafeilong@gmail.com" },
 ]
 description = "Neuroimaging analysis in Python"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
@@ -22,15 +22,22 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
 ]
 dependencies = [
     "numpy",
+    "scipy",
+    "nibabel",
+    "datalad",
+    "joblib",
+    "pandas",
+    "Pillow",
+    "matplotlib",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/feilong/neuroboros"
-"Bug Tracker" = "https://github.com/feilong/neuroboros/issues"
+"Homepage" = "https://github.com/neuroboros/neuroboros"
+"Bug Tracker" = "https://github.com/neuroboros/neuroboros/issues"
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `neuroboros-0.0.1/src/neuroboros.egg-info/PKG-INFO` & `neuroboros-0.1.1a0/src/neuroboros.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuroboros
-Version: 0.0.1
+Version: 0.1.1a0
 Summary: Neuroimaging analysis in Python
 Author-email: Ma Feilong <mafeilong@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Feilong Ma
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,16 +21,16 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/feilong/neuroboros
-Project-URL: Bug Tracker, https://github.com/feilong/neuroboros/issues
+Project-URL: Homepage, https://github.com/neuroboros/neuroboros
+Project-URL: Bug Tracker, https://github.com/neuroboros/neuroboros/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
```

