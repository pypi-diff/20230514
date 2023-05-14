# Comparing `tmp/arithmetica-py-1.0.203.tar.gz` & `tmp/arithmetica-py-1.0.204.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arithmetica-py-1.0.203.tar", last modified: Fri May 12 20:28:51 2023, max compression
+gzip compressed data, was "arithmetica-py-1.0.204.tar", last modified: Sun May 14 16:48:13 2023, max compression
```

## Comparing `arithmetica-py-1.0.203.tar` & `arithmetica-py-1.0.204.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:28:51.162313 arithmetica-py-1.0.203/
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-05-12 20:28:31.000000 arithmetica-py-1.0.203/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-12 20:28:51.162313 arithmetica-py-1.0.203/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10391 2023-05-12 20:28:31.000000 arithmetica-py-1.0.203/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:28:51.162313 arithmetica-py-1.0.203/arithmetica_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-12 20:28:51.000000 arithmetica-py-1.0.203/arithmetica_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-12 20:28:51.000000 arithmetica-py-1.0.203/arithmetica_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:28:51.000000 arithmetica-py-1.0.203/arithmetica_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-12 20:28:51.000000 arithmetica-py-1.0.203/arithmetica_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 20:28:51.162313 arithmetica-py-1.0.203/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-12 20:28:31.000000 arithmetica-py-1.0.203/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:28:51.158313 arithmetica-py-1.0.203/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:28:51.162313 arithmetica-py-1.0.203/src/python-module/
--rw-r--r--   0 runner    (1001) docker     (123)   184894 2023-05-12 20:28:50.000000 arithmetica-py-1.0.203/src/python-module/libarithmetica.a
--rw-r--r--   0 runner    (1001) docker     (123)    75112 2023-05-12 20:28:50.000000 arithmetica-py-1.0.203/src/python-module/libbasic_math_operations.a
--rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-05-12 20:28:31.000000 arithmetica-py-1.0.203/src/python-module/module.c
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 20:28:50.000000 arithmetica-py-1.0.203/src/python-module/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:48:13.438991 arithmetica-py-1.0.204/
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-05-14 16:47:51.000000 arithmetica-py-1.0.204/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-14 16:48:13.438991 arithmetica-py-1.0.204/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-05-14 16:47:51.000000 arithmetica-py-1.0.204/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:48:13.438991 arithmetica-py-1.0.204/arithmetica_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-14 16:48:13.000000 arithmetica-py-1.0.204/arithmetica_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-14 16:48:13.000000 arithmetica-py-1.0.204/arithmetica_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 16:48:13.000000 arithmetica-py-1.0.204/arithmetica_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-14 16:48:13.000000 arithmetica-py-1.0.204/arithmetica_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 16:48:13.438991 arithmetica-py-1.0.204/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-14 16:47:51.000000 arithmetica-py-1.0.204/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:48:13.434991 arithmetica-py-1.0.204/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:48:13.438991 arithmetica-py-1.0.204/src/python-module/
+-rw-r--r--   0 runner    (1001) docker     (123)   184894 2023-05-14 16:48:13.000000 arithmetica-py-1.0.204/src/python-module/libarithmetica.a
+-rw-r--r--   0 runner    (1001) docker     (123)    75112 2023-05-14 16:48:13.000000 arithmetica-py-1.0.204/src/python-module/libbasic_math_operations.a
+-rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-05-14 16:47:51.000000 arithmetica-py-1.0.204/src/python-module/module.c
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-14 16:48:13.000000 arithmetica-py-1.0.204/src/python-module/version.txt
```

### Comparing `arithmetica-py-1.0.203/LICENSE` & `arithmetica-py-1.0.204/LICENSE`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.203/README.md` & `arithmetica-py-1.0.204/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,17 @@
   <a href='https://github.com/avighnac/arithmetica/actions/workflows/tests.yml'>
     <img src='https://github.com/avighnac/arithmetica/actions/workflows/tests.yml/badge.svg'>
   </a>
 </div>
 <br>
 Arithmetica is a general-purpose infinite precision Linux and windows math library with a wide variety of mathematical functions and features. Currently supported languages are C, C++, and Python.
 
+# Documentation
+The documentation for arithmetica can be found [here](https://avighnac.github.io/arithmetica-docs/)!
+
 # Demonstration
 Using [construct_regular_polygon.c](https://github.com/avighnac/arithmetica/blob/main/src/library/geometry/construct_regular_polygon.c), you can create and render polygons.
 <div align='center'>
   <img width="400" height="400" src='https://user-images.githubusercontent.com/74564976/223171924-53bd642e-425f-4870-aa0e-2da184dd9f52.gif'>
 </div>
 
 The code for this can be found after the usage section.
```

#### html2text {}

```diff
@@ -4,18 +4,19 @@
 benefit other people too.
  If thou dost find this test passing, thou art assured of a library that doth
                         not suffer from memory leaks.
 [https://github.com/avighnac/arithmetica/actions/workflows/tests.yml/badge.svg]
 
 Arithmetica is a general-purpose infinite precision Linux and windows math
 library with a wide variety of mathematical functions and features. Currently
-supported languages are C, C++, and Python. # Demonstration Using
-[construct_regular_polygon.c](https://github.com/avighnac/arithmetica/blob/
-main/src/library/geometry/construct_regular_polygon.c), you can create and
-render polygons.
+supported languages are C, C++, and Python. # Documentation The documentation
+for arithmetica can be found [here](https://avighnac.github.io/arithmetica-
+docs/)! # Demonstration Using [construct_regular_polygon.c](https://github.com/
+avighnac/arithmetica/blob/main/src/library/geometry/
+construct_regular_polygon.c), you can create and render polygons.
  [https://user-images.githubusercontent.com/74564976/223171924-53bd642e-425f-
                           4870-aa0e-2da184dd9f52.gif]
 The code for this can be found after the usage section.
 (Code)
 ## Python ### Using pip! If you're on or above Python 3.10, then pip will work
 for you. See below if not. ```shell pip install arithmetica-py ``` ### Using
 binaries Go to the [project page](https://pypi.org/project/arithmetica-py/) on
```

### Comparing `arithmetica-py-1.0.203/setup.py` & `arithmetica-py-1.0.204/setup.py`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.203/src/python-module/libarithmetica.a` & `arithmetica-py-1.0.204/src/python-module/libarithmetica.a`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.203/src/python-module/libbasic_math_operations.a` & `arithmetica-py-1.0.204/src/python-module/libbasic_math_operations.a`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.203/src/python-module/module.c` & `arithmetica-py-1.0.204/src/python-module/module.c`

 * *Files identical despite different names*

