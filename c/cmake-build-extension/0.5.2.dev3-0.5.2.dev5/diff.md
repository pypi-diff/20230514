# Comparing `tmp/cmake-build-extension-0.5.2.dev3.tar.gz` & `tmp/cmake-build-extension-0.5.2.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmake-build-extension-0.5.2.dev3.tar", last modified: Mon Sep 19 16:17:42 2022, max compression
+gzip compressed data, was "cmake-build-extension-0.5.2.dev5.tar", last modified: Sun May 14 17:35:09 2023, max compression
```

## Comparing `cmake-build-extension-0.5.2.dev3.tar` & `cmake-build-extension-0.5.2.dev5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 16:17:42.648496 cmake-build-extension-0.5.2.dev3/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 16:17:42.644496 cmake-build-extension-0.5.2.dev3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 16:17:42.648496 cmake-build-extension-0.5.2.dev3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     3334 2022-09-19 16:17:25.000000 cmake-build-extension-0.5.2.dev3/.github/workflows/python.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1845 2022-09-19 16:17:25.000000 cmake-build-extension-0.5.2.dev3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-09-19 16:17:25.000000 cmake-build-extension-0.5.2.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    11298 2022-09-19 16:17:42.652496 cmake-build-extension-0.5.2.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9836 2022-09-19 16:17:25.000000 cmake-build-extension-0.5.2.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 16:17:42.648496 cmake-build-extension-0.5.2.dev3/example/
--rw-r--r--   0 runner    (1001) docker     (121)     3112 2022-09-19 16:17:25.000000 cmake-build-extension-0.5.2.dev3/example/.clang-format
--rw-r--r--   0 runner    (1001) docker     (121)     3723 2022-09-19 16:17:25.000000 cmake-build-extension-0.5.2.dev3/example/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-19 16:17:25.000000 cmake-build-extension-0.5.2.dev3/example/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 16:17:42.648496 cmake-build-extension-0.5.2.dev3/example/bindings_pybind11/
--rw-r--r--   0 runner    (1001) docker     (121)      753 2022-09-19 16:17:25.000000 cmake-build-extension-0.5.2.dev3/example/bindings_pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      888 2022-09-19 16:17:25.000000 cmake-build-extension-0.5.2.dev3/example/bindings_pybind11/bindings.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 16:17:42.648496 cmake-build-extension-0.5.2.dev3/example/bindings_swig/
--rw-r--r--   0 runner    (1001) docker     (121)     1609 2022-09-19 16:17:25.000000 cmake-build-extension-0.5.2.dev3/example/bindings_swig/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-09-19 16:17:25.000000 cmake-build-extension-0.5.2.dev3/example/bindings_swig/bindings.i
--rw-r--r--   0 runner    (1001) docker     (121)   109459 2022-09-19 16:17:25.000000 cmake-build-extension-0.5.2.dev3/example/bindings_swig/numpy.i
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-09-19 16:17:25.000000 cmake-build-extension-0.5.2.dev3/example/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1470 2022-09-19 16:17:25.000000 cmake-build-extension-0.5.2.dev3/example/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5293 2022-09-19 16:17:25.000000 cmake-build-extension-0.5.2.dev3/example/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 16:17:42.648496 cmake-build-extension-0.5.2.dev3/example/src/
--rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-09-19 16:17:25.000000 cmake-build-extension-0.5.2.dev3/example/src/mymath.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-09-19 16:17:25.000000 cmake-build-extension-0.5.2.dev3/example/src/mymath.h
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-09-19 16:17:25.000000 cmake-build-extension-0.5.2.dev3/example/src/print_answer.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 16:17:42.648496 cmake-build-extension-0.5.2.dev3/example/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1628 2022-09-19 16:17:25.000000 cmake-build-extension-0.5.2.dev3/example/tests/test_pybind11.py
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-09-19 16:17:25.000000 cmake-build-extension-0.5.2.dev3/example/tests/test_swig.py
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-09-19 16:17:25.000000 cmake-build-extension-0.5.2.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1523 2022-09-19 16:17:42.652496 cmake-build-extension-0.5.2.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-19 16:17:25.000000 cmake-build-extension-0.5.2.dev3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 16:17:42.648496 cmake-build-extension-0.5.2.dev3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 16:17:42.648496 cmake-build-extension-0.5.2.dev3/src/cmake_build_extension/
--rw-r--r--   0 runner    (1001) docker     (121)     1237 2022-09-19 16:17:25.000000 cmake-build-extension-0.5.2.dev3/src/cmake_build_extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1535 2022-09-19 16:17:25.000000 cmake-build-extension-0.5.2.dev3/src/cmake_build_extension/build_ext_option.py
--rw-r--r--   0 runner    (1001) docker     (121)    10952 2022-09-19 16:17:25.000000 cmake-build-extension-0.5.2.dev3/src/cmake_build_extension/build_extension.py
--rw-r--r--   0 runner    (1001) docker     (121)     2455 2022-09-19 16:17:25.000000 cmake-build-extension-0.5.2.dev3/src/cmake_build_extension/cmake_extension.py
--rw-r--r--   0 runner    (1001) docker     (121)     5585 2022-09-19 16:17:25.000000 cmake-build-extension-0.5.2.dev3/src/cmake_build_extension/sdist_command.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 16:17:42.648496 cmake-build-extension-0.5.2.dev3/src/cmake_build_extension.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11298 2022-09-19 16:17:42.000000 cmake-build-extension-0.5.2.dev3/src/cmake_build_extension.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2022-09-19 16:17:42.000000 cmake-build-extension-0.5.2.dev3/src/cmake_build_extension.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-19 16:17:42.000000 cmake-build-extension-0.5.2.dev3/src/cmake_build_extension.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-19 16:17:42.000000 cmake-build-extension-0.5.2.dev3/src/cmake_build_extension.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-09-19 16:17:42.000000 cmake-build-extension-0.5.2.dev3/src/cmake_build_extension.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-19 16:17:42.000000 cmake-build-extension-0.5.2.dev3/src/cmake_build_extension.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:35:09.588104 cmake-build-extension-0.5.2.dev5/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:35:09.584104 cmake-build-extension-0.5.2.dev5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:35:09.584104 cmake-build-extension-0.5.2.dev5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     3334 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/.github/workflows/python.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1845 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    11298 2023-05-14 17:35:09.588104 cmake-build-extension-0.5.2.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9836 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:35:09.584104 cmake-build-extension-0.5.2.dev5/example/
+-rw-r--r--   0 runner    (1001) docker     (122)     3112 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (122)     3723 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:35:09.584104 cmake-build-extension-0.5.2.dev5/example/bindings_pybind11/
+-rw-r--r--   0 runner    (1001) docker     (122)      753 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/bindings_pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      888 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/bindings_pybind11/bindings.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:35:09.588104 cmake-build-extension-0.5.2.dev5/example/bindings_swig/
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/bindings_swig/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1990 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/bindings_swig/bindings.i
+-rw-r--r--   0 runner    (1001) docker     (122)   109459 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/bindings_swig/numpy.i
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5293 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:35:09.588104 cmake-build-extension-0.5.2.dev5/example/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     1052 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/src/mymath.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      907 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/src/mymath.h
+-rw-r--r--   0 runner    (1001) docker     (122)      197 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/src/print_answer.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:35:09.588104 cmake-build-extension-0.5.2.dev5/example/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/tests/test_pybind11.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1512 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/tests/test_swig.py
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-05-14 17:35:09.592104 cmake-build-extension-0.5.2.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:35:09.584104 cmake-build-extension-0.5.2.dev5/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:35:09.588104 cmake-build-extension-0.5.2.dev5/src/cmake_build_extension/
+-rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/src/cmake_build_extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1535 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/src/cmake_build_extension/build_ext_option.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10946 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/src/cmake_build_extension/build_extension.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2455 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/src/cmake_build_extension/cmake_extension.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5585 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/src/cmake_build_extension/sdist_command.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:35:09.588104 cmake-build-extension-0.5.2.dev5/src/cmake_build_extension.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    11298 2023-05-14 17:35:09.000000 cmake-build-extension-0.5.2.dev5/src/cmake_build_extension.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-05-14 17:35:09.000000 cmake-build-extension-0.5.2.dev5/src/cmake_build_extension.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-14 17:35:09.000000 cmake-build-extension-0.5.2.dev5/src/cmake_build_extension.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-14 17:35:09.000000 cmake-build-extension-0.5.2.dev5/src/cmake_build_extension.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-14 17:35:09.000000 cmake-build-extension-0.5.2.dev5/src/cmake_build_extension.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-14 17:35:09.000000 cmake-build-extension-0.5.2.dev5/src/cmake_build_extension.egg-info/top_level.txt
```

### Comparing `cmake-build-extension-0.5.2.dev3/.github/workflows/python.yml` & `cmake-build-extension-0.5.2.dev5/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev3/.gitignore` & `cmake-build-extension-0.5.2.dev5/.gitignore`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev3/LICENSE` & `cmake-build-extension-0.5.2.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev3/PKG-INFO` & `cmake-build-extension-0.5.2.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmake-build-extension
-Version: 0.5.2.dev3
+Version: 0.5.2.dev5
 Summary: Setuptools extension to build and package CMake projects.
 Home-page: https://github.com/diegoferigo/cmake-build-extension
 Author: Diego Ferigo
 Author-email: dgferigo@gmail.com
 License: MIT
 Project-URL: Changelog, https://github.com/diegoferigo/cmake-build-extension/releases
 Project-URL: Source, https://github.com/diegoferigo/cmake-build-extension
```

### Comparing `cmake-build-extension-0.5.2.dev3/README.md` & `cmake-build-extension-0.5.2.dev5/README.md`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev3/example/.clang-format` & `cmake-build-extension-0.5.2.dev5/example/.clang-format`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev3/example/CMakeLists.txt` & `cmake-build-extension-0.5.2.dev5/example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev3/example/bindings_pybind11/CMakeLists.txt` & `cmake-build-extension-0.5.2.dev5/example/bindings_pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev3/example/bindings_pybind11/bindings.cpp` & `cmake-build-extension-0.5.2.dev5/example/bindings_pybind11/bindings.cpp`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev3/example/bindings_swig/CMakeLists.txt` & `cmake-build-extension-0.5.2.dev5/example/bindings_swig/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev3/example/bindings_swig/bindings.i` & `cmake-build-extension-0.5.2.dev5/example/bindings_swig/bindings.i`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev3/example/bindings_swig/numpy.i` & `cmake-build-extension-0.5.2.dev5/example/bindings_swig/numpy.i`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev3/example/setup.cfg` & `cmake-build-extension-0.5.2.dev5/example/setup.cfg`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev3/example/setup.py` & `cmake-build-extension-0.5.2.dev5/example/setup.py`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev3/example/src/mymath.cpp` & `cmake-build-extension-0.5.2.dev5/example/src/mymath.cpp`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev3/example/src/mymath.h` & `cmake-build-extension-0.5.2.dev5/example/src/mymath.h`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev3/example/tests/test_pybind11.py` & `cmake-build-extension-0.5.2.dev5/example/tests/test_pybind11.py`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev3/example/tests/test_swig.py` & `cmake-build-extension-0.5.2.dev5/example/tests/test_swig.py`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev3/setup.cfg` & `cmake-build-extension-0.5.2.dev5/setup.cfg`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev3/src/cmake_build_extension/__init__.py` & `cmake-build-extension-0.5.2.dev5/src/cmake_build_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev3/src/cmake_build_extension/build_ext_option.py` & `cmake-build-extension-0.5.2.dev5/src/cmake_build_extension/build_ext_option.py`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev3/src/cmake_build_extension/build_extension.py` & `cmake-build-extension-0.5.2.dev5/src/cmake_build_extension/build_extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         cmake_install_prefix = ext_dir / ext.install_prefix
 
         # Initialize the CMake configuration arguments
         configure_args = []
 
         # Select the appropriate generator and accompanying settings
         if ext.cmake_generator is not None:
-            configure_args += [f"-G \"{ext.cmake_generator}\""]
+            configure_args += ["-G", ext.cmake_generator]
 
             if ext.cmake_generator == "Ninja":
                 # Fix #26: https://github.com/diegoferigo/cmake-build-extension/issues/26
                 configure_args += [f"-DCMAKE_MAKE_PROGRAM={shutil.which('ninja')}"]
 
         # CMake configure arguments
         configure_args += [
```

### Comparing `cmake-build-extension-0.5.2.dev3/src/cmake_build_extension/cmake_extension.py` & `cmake-build-extension-0.5.2.dev5/src/cmake_build_extension/cmake_extension.py`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev3/src/cmake_build_extension/sdist_command.py` & `cmake-build-extension-0.5.2.dev5/src/cmake_build_extension/sdist_command.py`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev3/src/cmake_build_extension.egg-info/PKG-INFO` & `cmake-build-extension-0.5.2.dev5/src/cmake_build_extension.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmake-build-extension
-Version: 0.5.2.dev3
+Version: 0.5.2.dev5
 Summary: Setuptools extension to build and package CMake projects.
 Home-page: https://github.com/diegoferigo/cmake-build-extension
 Author: Diego Ferigo
 Author-email: dgferigo@gmail.com
 License: MIT
 Project-URL: Changelog, https://github.com/diegoferigo/cmake-build-extension/releases
 Project-URL: Source, https://github.com/diegoferigo/cmake-build-extension
```

### Comparing `cmake-build-extension-0.5.2.dev3/src/cmake_build_extension.egg-info/SOURCES.txt` & `cmake-build-extension-0.5.2.dev5/src/cmake_build_extension.egg-info/SOURCES.txt`

 * *Files identical despite different names*

