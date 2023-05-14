# Comparing `tmp/cmake-build-extension-0.5.2.dev7.tar.gz` & `tmp/cmake-build-extension-0.5.2.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmake-build-extension-0.5.2.dev7.tar", last modified: Sun May 14 17:39:33 2023, max compression
+gzip compressed data, was "cmake-build-extension-0.5.2.dev9.tar", last modified: Sun May 14 18:03:40 2023, max compression
```

## Comparing `cmake-build-extension-0.5.2.dev7.tar` & `cmake-build-extension-0.5.2.dev9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:39:33.942957 cmake-build-extension-0.5.2.dev7/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:39:33.938957 cmake-build-extension-0.5.2.dev7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:39:33.938957 cmake-build-extension-0.5.2.dev7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     3334 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/.github/workflows/python.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1845 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    11298 2023-05-14 17:39:33.942957 cmake-build-extension-0.5.2.dev7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9836 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:39:33.942957 cmake-build-extension-0.5.2.dev7/example/
--rw-r--r--   0 runner    (1001) docker     (122)     3112 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/.clang-format
--rw-r--r--   0 runner    (1001) docker     (122)     3723 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:39:33.942957 cmake-build-extension-0.5.2.dev7/example/bindings_pybind11/
--rw-r--r--   0 runner    (1001) docker     (122)      753 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/bindings_pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)      888 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/bindings_pybind11/bindings.cpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:39:33.942957 cmake-build-extension-0.5.2.dev7/example/bindings_swig/
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/bindings_swig/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1990 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/bindings_swig/bindings.i
--rw-r--r--   0 runner    (1001) docker     (122)   109459 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/bindings_swig/numpy.i
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5293 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:39:33.942957 cmake-build-extension-0.5.2.dev7/example/src/
--rw-r--r--   0 runner    (1001) docker     (122)     1052 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/src/mymath.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      907 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/src/mymath.h
--rw-r--r--   0 runner    (1001) docker     (122)      197 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/src/print_answer.cpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:39:33.942957 cmake-build-extension-0.5.2.dev7/example/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/tests/test_pybind11.py
--rw-r--r--   0 runner    (1001) docker     (122)     1512 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/tests/test_swig.py
--rw-r--r--   0 runner    (1001) docker     (122)      273 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-05-14 17:39:33.946957 cmake-build-extension-0.5.2.dev7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:39:33.938957 cmake-build-extension-0.5.2.dev7/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:39:33.942957 cmake-build-extension-0.5.2.dev7/src/cmake_build_extension/
--rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/src/cmake_build_extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1535 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/src/cmake_build_extension/build_ext_option.py
--rw-r--r--   0 runner    (1001) docker     (122)    11054 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/src/cmake_build_extension/build_extension.py
--rw-r--r--   0 runner    (1001) docker     (122)     2455 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/src/cmake_build_extension/cmake_extension.py
--rw-r--r--   0 runner    (1001) docker     (122)     5585 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/src/cmake_build_extension/sdist_command.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:39:33.942957 cmake-build-extension-0.5.2.dev7/src/cmake_build_extension.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    11298 2023-05-14 17:39:33.000000 cmake-build-extension-0.5.2.dev7/src/cmake_build_extension.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-05-14 17:39:33.000000 cmake-build-extension-0.5.2.dev7/src/cmake_build_extension.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-14 17:39:33.000000 cmake-build-extension-0.5.2.dev7/src/cmake_build_extension.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-14 17:39:33.000000 cmake-build-extension-0.5.2.dev7/src/cmake_build_extension.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-14 17:39:33.000000 cmake-build-extension-0.5.2.dev7/src/cmake_build_extension.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-14 17:39:33.000000 cmake-build-extension-0.5.2.dev7/src/cmake_build_extension.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 18:03:40.028265 cmake-build-extension-0.5.2.dev9/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 18:03:40.024265 cmake-build-extension-0.5.2.dev9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 18:03:40.024265 cmake-build-extension-0.5.2.dev9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     3334 2023-05-14 18:03:29.000000 cmake-build-extension-0.5.2.dev9/.github/workflows/python.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1845 2023-05-14 18:03:29.000000 cmake-build-extension-0.5.2.dev9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-05-14 18:03:29.000000 cmake-build-extension-0.5.2.dev9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    11298 2023-05-14 18:03:40.028265 cmake-build-extension-0.5.2.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9836 2023-05-14 18:03:29.000000 cmake-build-extension-0.5.2.dev9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 18:03:40.024265 cmake-build-extension-0.5.2.dev9/example/
+-rw-r--r--   0 runner    (1001) docker     (122)     3112 2023-05-14 18:03:29.000000 cmake-build-extension-0.5.2.dev9/example/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (122)     3723 2023-05-14 18:03:29.000000 cmake-build-extension-0.5.2.dev9/example/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 18:03:29.000000 cmake-build-extension-0.5.2.dev9/example/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 18:03:40.024265 cmake-build-extension-0.5.2.dev9/example/bindings_pybind11/
+-rw-r--r--   0 runner    (1001) docker     (122)      753 2023-05-14 18:03:29.000000 cmake-build-extension-0.5.2.dev9/example/bindings_pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      888 2023-05-14 18:03:29.000000 cmake-build-extension-0.5.2.dev9/example/bindings_pybind11/bindings.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 18:03:40.024265 cmake-build-extension-0.5.2.dev9/example/bindings_swig/
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-05-14 18:03:29.000000 cmake-build-extension-0.5.2.dev9/example/bindings_swig/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1990 2023-05-14 18:03:29.000000 cmake-build-extension-0.5.2.dev9/example/bindings_swig/bindings.i
+-rw-r--r--   0 runner    (1001) docker     (122)   109459 2023-05-14 18:03:29.000000 cmake-build-extension-0.5.2.dev9/example/bindings_swig/numpy.i
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-05-14 18:03:29.000000 cmake-build-extension-0.5.2.dev9/example/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-05-14 18:03:29.000000 cmake-build-extension-0.5.2.dev9/example/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5293 2023-05-14 18:03:29.000000 cmake-build-extension-0.5.2.dev9/example/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 18:03:40.028265 cmake-build-extension-0.5.2.dev9/example/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     1052 2023-05-14 18:03:29.000000 cmake-build-extension-0.5.2.dev9/example/src/mymath.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      907 2023-05-14 18:03:29.000000 cmake-build-extension-0.5.2.dev9/example/src/mymath.h
+-rw-r--r--   0 runner    (1001) docker     (122)      197 2023-05-14 18:03:29.000000 cmake-build-extension-0.5.2.dev9/example/src/print_answer.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 18:03:40.028265 cmake-build-extension-0.5.2.dev9/example/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-05-14 18:03:29.000000 cmake-build-extension-0.5.2.dev9/example/tests/test_pybind11.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1512 2023-05-14 18:03:29.000000 cmake-build-extension-0.5.2.dev9/example/tests/test_swig.py
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-05-14 18:03:29.000000 cmake-build-extension-0.5.2.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-05-14 18:03:40.028265 cmake-build-extension-0.5.2.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-14 18:03:29.000000 cmake-build-extension-0.5.2.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 18:03:40.024265 cmake-build-extension-0.5.2.dev9/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 18:03:40.028265 cmake-build-extension-0.5.2.dev9/src/cmake_build_extension/
+-rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-05-14 18:03:29.000000 cmake-build-extension-0.5.2.dev9/src/cmake_build_extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1535 2023-05-14 18:03:29.000000 cmake-build-extension-0.5.2.dev9/src/cmake_build_extension/build_ext_option.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11097 2023-05-14 18:03:29.000000 cmake-build-extension-0.5.2.dev9/src/cmake_build_extension/build_extension.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2455 2023-05-14 18:03:29.000000 cmake-build-extension-0.5.2.dev9/src/cmake_build_extension/cmake_extension.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5585 2023-05-14 18:03:29.000000 cmake-build-extension-0.5.2.dev9/src/cmake_build_extension/sdist_command.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 18:03:40.028265 cmake-build-extension-0.5.2.dev9/src/cmake_build_extension.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    11298 2023-05-14 18:03:39.000000 cmake-build-extension-0.5.2.dev9/src/cmake_build_extension.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-05-14 18:03:40.000000 cmake-build-extension-0.5.2.dev9/src/cmake_build_extension.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-14 18:03:39.000000 cmake-build-extension-0.5.2.dev9/src/cmake_build_extension.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-14 18:03:39.000000 cmake-build-extension-0.5.2.dev9/src/cmake_build_extension.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-14 18:03:39.000000 cmake-build-extension-0.5.2.dev9/src/cmake_build_extension.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-14 18:03:39.000000 cmake-build-extension-0.5.2.dev9/src/cmake_build_extension.egg-info/top_level.txt
```

### Comparing `cmake-build-extension-0.5.2.dev7/.github/workflows/python.yml` & `cmake-build-extension-0.5.2.dev9/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev7/.gitignore` & `cmake-build-extension-0.5.2.dev9/.gitignore`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev7/LICENSE` & `cmake-build-extension-0.5.2.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev7/PKG-INFO` & `cmake-build-extension-0.5.2.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmake-build-extension
-Version: 0.5.2.dev7
+Version: 0.5.2.dev9
 Summary: Setuptools extension to build and package CMake projects.
 Home-page: https://github.com/diegoferigo/cmake-build-extension
 Author: Diego Ferigo
 Author-email: dgferigo@gmail.com
 License: MIT
 Project-URL: Changelog, https://github.com/diegoferigo/cmake-build-extension/releases
 Project-URL: Source, https://github.com/diegoferigo/cmake-build-extension
```

### Comparing `cmake-build-extension-0.5.2.dev7/README.md` & `cmake-build-extension-0.5.2.dev9/README.md`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev7/example/.clang-format` & `cmake-build-extension-0.5.2.dev9/example/.clang-format`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev7/example/CMakeLists.txt` & `cmake-build-extension-0.5.2.dev9/example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev7/example/bindings_pybind11/CMakeLists.txt` & `cmake-build-extension-0.5.2.dev9/example/bindings_pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev7/example/bindings_pybind11/bindings.cpp` & `cmake-build-extension-0.5.2.dev9/example/bindings_pybind11/bindings.cpp`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev7/example/bindings_swig/CMakeLists.txt` & `cmake-build-extension-0.5.2.dev9/example/bindings_swig/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev7/example/bindings_swig/bindings.i` & `cmake-build-extension-0.5.2.dev9/example/bindings_swig/bindings.i`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev7/example/bindings_swig/numpy.i` & `cmake-build-extension-0.5.2.dev9/example/bindings_swig/numpy.i`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev7/example/setup.cfg` & `cmake-build-extension-0.5.2.dev9/example/setup.cfg`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev7/example/setup.py` & `cmake-build-extension-0.5.2.dev9/example/setup.py`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev7/example/src/mymath.cpp` & `cmake-build-extension-0.5.2.dev9/example/src/mymath.cpp`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev7/example/src/mymath.h` & `cmake-build-extension-0.5.2.dev9/example/src/mymath.h`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev7/example/tests/test_pybind11.py` & `cmake-build-extension-0.5.2.dev9/example/tests/test_pybind11.py`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev7/example/tests/test_swig.py` & `cmake-build-extension-0.5.2.dev9/example/tests/test_swig.py`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev7/setup.cfg` & `cmake-build-extension-0.5.2.dev9/setup.cfg`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev7/src/cmake_build_extension/__init__.py` & `cmake-build-extension-0.5.2.dev9/src/cmake_build_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev7/src/cmake_build_extension/build_ext_option.py` & `cmake-build-extension-0.5.2.dev9/src/cmake_build_extension/build_ext_option.py`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev7/src/cmake_build_extension/build_extension.py` & `cmake-build-extension-0.5.2.dev9/src/cmake_build_extension/build_extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             raise ValueError("No CMakeExtension objects found")
 
         # Check that CMake is installed
         if shutil.which("cmake") is None:
             raise RuntimeError("Required command 'cmake' not found")
 
         # Check that Ninja is installed
-        if shutil.which("ninja") is None:
+        if ext.cmake_generator.lower() == "ninja" and shutil.which("ninja") is None:
             raise RuntimeError("Required command 'ninja' not found")
 
         for ext in cmake_extensions:
 
             # Disable the extension if specified in the command line
             if (
                 ext.name in self.no_cmake_extensions
```

### Comparing `cmake-build-extension-0.5.2.dev7/src/cmake_build_extension/cmake_extension.py` & `cmake-build-extension-0.5.2.dev9/src/cmake_build_extension/cmake_extension.py`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev7/src/cmake_build_extension/sdist_command.py` & `cmake-build-extension-0.5.2.dev9/src/cmake_build_extension/sdist_command.py`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev7/src/cmake_build_extension.egg-info/PKG-INFO` & `cmake-build-extension-0.5.2.dev9/src/cmake_build_extension.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmake-build-extension
-Version: 0.5.2.dev7
+Version: 0.5.2.dev9
 Summary: Setuptools extension to build and package CMake projects.
 Home-page: https://github.com/diegoferigo/cmake-build-extension
 Author: Diego Ferigo
 Author-email: dgferigo@gmail.com
 License: MIT
 Project-URL: Changelog, https://github.com/diegoferigo/cmake-build-extension/releases
 Project-URL: Source, https://github.com/diegoferigo/cmake-build-extension
```

### Comparing `cmake-build-extension-0.5.2.dev7/src/cmake_build_extension.egg-info/SOURCES.txt` & `cmake-build-extension-0.5.2.dev9/src/cmake_build_extension.egg-info/SOURCES.txt`

 * *Files identical despite different names*

