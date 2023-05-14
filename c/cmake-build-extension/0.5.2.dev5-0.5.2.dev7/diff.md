# Comparing `tmp/cmake-build-extension-0.5.2.dev5.tar.gz` & `tmp/cmake-build-extension-0.5.2.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmake-build-extension-0.5.2.dev5.tar", last modified: Sun May 14 17:35:09 2023, max compression
+gzip compressed data, was "cmake-build-extension-0.5.2.dev7.tar", last modified: Sun May 14 17:39:33 2023, max compression
```

## Comparing `cmake-build-extension-0.5.2.dev5.tar` & `cmake-build-extension-0.5.2.dev7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:35:09.588104 cmake-build-extension-0.5.2.dev5/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:35:09.584104 cmake-build-extension-0.5.2.dev5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:35:09.584104 cmake-build-extension-0.5.2.dev5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     3334 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/.github/workflows/python.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1845 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    11298 2023-05-14 17:35:09.588104 cmake-build-extension-0.5.2.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9836 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:35:09.584104 cmake-build-extension-0.5.2.dev5/example/
--rw-r--r--   0 runner    (1001) docker     (122)     3112 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/.clang-format
--rw-r--r--   0 runner    (1001) docker     (122)     3723 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:35:09.584104 cmake-build-extension-0.5.2.dev5/example/bindings_pybind11/
--rw-r--r--   0 runner    (1001) docker     (122)      753 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/bindings_pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)      888 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/bindings_pybind11/bindings.cpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:35:09.588104 cmake-build-extension-0.5.2.dev5/example/bindings_swig/
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/bindings_swig/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1990 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/bindings_swig/bindings.i
--rw-r--r--   0 runner    (1001) docker     (122)   109459 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/bindings_swig/numpy.i
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5293 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:35:09.588104 cmake-build-extension-0.5.2.dev5/example/src/
--rw-r--r--   0 runner    (1001) docker     (122)     1052 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/src/mymath.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      907 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/src/mymath.h
--rw-r--r--   0 runner    (1001) docker     (122)      197 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/src/print_answer.cpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:35:09.588104 cmake-build-extension-0.5.2.dev5/example/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/tests/test_pybind11.py
--rw-r--r--   0 runner    (1001) docker     (122)     1512 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/example/tests/test_swig.py
--rw-r--r--   0 runner    (1001) docker     (122)      273 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-05-14 17:35:09.592104 cmake-build-extension-0.5.2.dev5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:35:09.584104 cmake-build-extension-0.5.2.dev5/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:35:09.588104 cmake-build-extension-0.5.2.dev5/src/cmake_build_extension/
--rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/src/cmake_build_extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1535 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/src/cmake_build_extension/build_ext_option.py
--rw-r--r--   0 runner    (1001) docker     (122)    10946 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/src/cmake_build_extension/build_extension.py
--rw-r--r--   0 runner    (1001) docker     (122)     2455 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/src/cmake_build_extension/cmake_extension.py
--rw-r--r--   0 runner    (1001) docker     (122)     5585 2023-05-14 17:34:55.000000 cmake-build-extension-0.5.2.dev5/src/cmake_build_extension/sdist_command.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:35:09.588104 cmake-build-extension-0.5.2.dev5/src/cmake_build_extension.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    11298 2023-05-14 17:35:09.000000 cmake-build-extension-0.5.2.dev5/src/cmake_build_extension.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-05-14 17:35:09.000000 cmake-build-extension-0.5.2.dev5/src/cmake_build_extension.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-14 17:35:09.000000 cmake-build-extension-0.5.2.dev5/src/cmake_build_extension.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-14 17:35:09.000000 cmake-build-extension-0.5.2.dev5/src/cmake_build_extension.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-14 17:35:09.000000 cmake-build-extension-0.5.2.dev5/src/cmake_build_extension.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-14 17:35:09.000000 cmake-build-extension-0.5.2.dev5/src/cmake_build_extension.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:39:33.942957 cmake-build-extension-0.5.2.dev7/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:39:33.938957 cmake-build-extension-0.5.2.dev7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:39:33.938957 cmake-build-extension-0.5.2.dev7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     3334 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/.github/workflows/python.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1845 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    11298 2023-05-14 17:39:33.942957 cmake-build-extension-0.5.2.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9836 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:39:33.942957 cmake-build-extension-0.5.2.dev7/example/
+-rw-r--r--   0 runner    (1001) docker     (122)     3112 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (122)     3723 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:39:33.942957 cmake-build-extension-0.5.2.dev7/example/bindings_pybind11/
+-rw-r--r--   0 runner    (1001) docker     (122)      753 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/bindings_pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      888 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/bindings_pybind11/bindings.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:39:33.942957 cmake-build-extension-0.5.2.dev7/example/bindings_swig/
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/bindings_swig/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1990 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/bindings_swig/bindings.i
+-rw-r--r--   0 runner    (1001) docker     (122)   109459 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/bindings_swig/numpy.i
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5293 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:39:33.942957 cmake-build-extension-0.5.2.dev7/example/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     1052 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/src/mymath.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      907 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/src/mymath.h
+-rw-r--r--   0 runner    (1001) docker     (122)      197 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/src/print_answer.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:39:33.942957 cmake-build-extension-0.5.2.dev7/example/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/tests/test_pybind11.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1512 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/example/tests/test_swig.py
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-05-14 17:39:33.946957 cmake-build-extension-0.5.2.dev7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:39:33.938957 cmake-build-extension-0.5.2.dev7/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:39:33.942957 cmake-build-extension-0.5.2.dev7/src/cmake_build_extension/
+-rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/src/cmake_build_extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1535 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/src/cmake_build_extension/build_ext_option.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11054 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/src/cmake_build_extension/build_extension.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2455 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/src/cmake_build_extension/cmake_extension.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5585 2023-05-14 17:39:23.000000 cmake-build-extension-0.5.2.dev7/src/cmake_build_extension/sdist_command.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 17:39:33.942957 cmake-build-extension-0.5.2.dev7/src/cmake_build_extension.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    11298 2023-05-14 17:39:33.000000 cmake-build-extension-0.5.2.dev7/src/cmake_build_extension.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-05-14 17:39:33.000000 cmake-build-extension-0.5.2.dev7/src/cmake_build_extension.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-14 17:39:33.000000 cmake-build-extension-0.5.2.dev7/src/cmake_build_extension.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-14 17:39:33.000000 cmake-build-extension-0.5.2.dev7/src/cmake_build_extension.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-14 17:39:33.000000 cmake-build-extension-0.5.2.dev7/src/cmake_build_extension.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-14 17:39:33.000000 cmake-build-extension-0.5.2.dev7/src/cmake_build_extension.egg-info/top_level.txt
```

### Comparing `cmake-build-extension-0.5.2.dev5/.github/workflows/python.yml` & `cmake-build-extension-0.5.2.dev7/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev5/.gitignore` & `cmake-build-extension-0.5.2.dev7/.gitignore`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev5/LICENSE` & `cmake-build-extension-0.5.2.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev5/PKG-INFO` & `cmake-build-extension-0.5.2.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmake-build-extension
-Version: 0.5.2.dev5
+Version: 0.5.2.dev7
 Summary: Setuptools extension to build and package CMake projects.
 Home-page: https://github.com/diegoferigo/cmake-build-extension
 Author: Diego Ferigo
 Author-email: dgferigo@gmail.com
 License: MIT
 Project-URL: Changelog, https://github.com/diegoferigo/cmake-build-extension/releases
 Project-URL: Source, https://github.com/diegoferigo/cmake-build-extension
```

### Comparing `cmake-build-extension-0.5.2.dev5/README.md` & `cmake-build-extension-0.5.2.dev7/README.md`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev5/example/.clang-format` & `cmake-build-extension-0.5.2.dev7/example/.clang-format`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev5/example/CMakeLists.txt` & `cmake-build-extension-0.5.2.dev7/example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev5/example/bindings_pybind11/CMakeLists.txt` & `cmake-build-extension-0.5.2.dev7/example/bindings_pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev5/example/bindings_pybind11/bindings.cpp` & `cmake-build-extension-0.5.2.dev7/example/bindings_pybind11/bindings.cpp`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev5/example/bindings_swig/CMakeLists.txt` & `cmake-build-extension-0.5.2.dev7/example/bindings_swig/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev5/example/bindings_swig/bindings.i` & `cmake-build-extension-0.5.2.dev7/example/bindings_swig/bindings.i`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev5/example/bindings_swig/numpy.i` & `cmake-build-extension-0.5.2.dev7/example/bindings_swig/numpy.i`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev5/example/setup.cfg` & `cmake-build-extension-0.5.2.dev7/example/setup.cfg`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev5/example/setup.py` & `cmake-build-extension-0.5.2.dev7/example/setup.py`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev5/example/src/mymath.cpp` & `cmake-build-extension-0.5.2.dev7/example/src/mymath.cpp`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev5/example/src/mymath.h` & `cmake-build-extension-0.5.2.dev7/example/src/mymath.h`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev5/example/tests/test_pybind11.py` & `cmake-build-extension-0.5.2.dev7/example/tests/test_pybind11.py`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev5/example/tests/test_swig.py` & `cmake-build-extension-0.5.2.dev7/example/tests/test_swig.py`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev5/setup.cfg` & `cmake-build-extension-0.5.2.dev7/setup.cfg`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev5/src/cmake_build_extension/__init__.py` & `cmake-build-extension-0.5.2.dev7/src/cmake_build_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev5/src/cmake_build_extension/build_ext_option.py` & `cmake-build-extension-0.5.2.dev7/src/cmake_build_extension/build_ext_option.py`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev5/src/cmake_build_extension/build_extension.py` & `cmake-build-extension-0.5.2.dev7/src/cmake_build_extension/build_extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,14 +165,17 @@
 
         # Extend the configure arguments with those passed from the extension
         configure_args += ext.cmake_configure_options
 
         # CMake build arguments
         build_args = ["--config", ext.cmake_build_type]
 
+        # CMake install arguments
+        install_args = ["--config", ext.cmake_build_type]
+
         if platform.system() == "Windows":
 
             configure_args += []
 
         elif platform.system() in {"Linux", "Darwin"}:
 
             configure_args += []
@@ -205,15 +208,15 @@
             build_folder,
         ] + configure_args
 
         # 2. Compose CMake build command
         build_command = ["cmake", "--build", build_folder] + build_args
 
         # 3. Compose CMake install command
-        install_command = ["cmake", "--install", build_folder]
+        install_command = ["cmake", "--install", build_folder] + install_args
 
         # If the cmake_component option of the CMakeExtension is used, install just
         # the specified component.
         if self.component is None and ext.cmake_component is not None:
             install_command.extend(["--component", ext.cmake_component])
 
         # Instead, if the `--component` command line option is used, install just
```

### Comparing `cmake-build-extension-0.5.2.dev5/src/cmake_build_extension/cmake_extension.py` & `cmake-build-extension-0.5.2.dev7/src/cmake_build_extension/cmake_extension.py`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev5/src/cmake_build_extension/sdist_command.py` & `cmake-build-extension-0.5.2.dev7/src/cmake_build_extension/sdist_command.py`

 * *Files identical despite different names*

### Comparing `cmake-build-extension-0.5.2.dev5/src/cmake_build_extension.egg-info/PKG-INFO` & `cmake-build-extension-0.5.2.dev7/src/cmake_build_extension.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmake-build-extension
-Version: 0.5.2.dev5
+Version: 0.5.2.dev7
 Summary: Setuptools extension to build and package CMake projects.
 Home-page: https://github.com/diegoferigo/cmake-build-extension
 Author: Diego Ferigo
 Author-email: dgferigo@gmail.com
 License: MIT
 Project-URL: Changelog, https://github.com/diegoferigo/cmake-build-extension/releases
 Project-URL: Source, https://github.com/diegoferigo/cmake-build-extension
```

### Comparing `cmake-build-extension-0.5.2.dev5/src/cmake_build_extension.egg-info/SOURCES.txt` & `cmake-build-extension-0.5.2.dev7/src/cmake_build_extension.egg-info/SOURCES.txt`

 * *Files identical despite different names*

