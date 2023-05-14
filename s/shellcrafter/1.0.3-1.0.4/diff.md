# Comparing `tmp/shellcrafter-1.0.3.tar.gz` & `tmp/shellcrafter-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellcrafter-1.0.3.tar", last modified: Sun Apr 30 12:07:35 2023, max compression
+gzip compressed data, was "shellcrafter-1.0.4.tar", last modified: Sun May 14 00:02:10 2023, max compression
```

## Comparing `shellcrafter-1.0.3.tar` & `shellcrafter-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:07:35.443284 shellcrafter-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-30 12:07:35.443284 shellcrafter-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-30 12:07:14.000000 shellcrafter-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-30 12:07:14.000000 shellcrafter-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 12:07:35.443284 shellcrafter-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-30 12:07:14.000000 shellcrafter-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:07:35.443284 shellcrafter-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:07:35.443284 shellcrafter-1.0.3/src/shellcrafter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 12:07:14.000000 shellcrafter-1.0.3/src/shellcrafter/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1121 2023-04-30 12:07:14.000000 shellcrafter-1.0.3/src/shellcrafter/ascii_hex_stack_push_converter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11958 2023-04-30 12:07:14.000000 shellcrafter-1.0.3/src/shellcrafter/find_gadgets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7011 2023-04-30 12:07:14.000000 shellcrafter-1.0.3/src/shellcrafter/keyst_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1082 2023-04-30 12:07:14.000000 shellcrafter-1.0.3/src/shellcrafter/ror_hash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:07:35.443284 shellcrafter-1.0.3/src/shellcrafter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-30 12:07:35.000000 shellcrafter-1.0.3/src/shellcrafter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-30 12:07:35.000000 shellcrafter-1.0.3/src/shellcrafter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 12:07:35.000000 shellcrafter-1.0.3/src/shellcrafter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-30 12:07:35.000000 shellcrafter-1.0.3/src/shellcrafter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-30 12:07:35.000000 shellcrafter-1.0.3/src/shellcrafter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-30 12:07:35.000000 shellcrafter-1.0.3/src/shellcrafter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 00:02:10.443976 shellcrafter-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-14 00:02:10.443976 shellcrafter-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-14 00:01:48.000000 shellcrafter-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-14 00:01:48.000000 shellcrafter-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 00:02:10.443976 shellcrafter-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-14 00:01:48.000000 shellcrafter-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 00:02:10.443976 shellcrafter-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 00:02:10.443976 shellcrafter-1.0.4/src/shellcrafter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 00:01:48.000000 shellcrafter-1.0.4/src/shellcrafter/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1121 2023-05-14 00:01:48.000000 shellcrafter-1.0.4/src/shellcrafter/ascii_hex_stack_push_converter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11958 2023-05-14 00:01:48.000000 shellcrafter-1.0.4/src/shellcrafter/find_gadgets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7011 2023-05-14 00:01:48.000000 shellcrafter-1.0.4/src/shellcrafter/keyst_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1082 2023-05-14 00:01:48.000000 shellcrafter-1.0.4/src/shellcrafter/ror_hash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 00:02:10.443976 shellcrafter-1.0.4/src/shellcrafter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-14 00:02:10.000000 shellcrafter-1.0.4/src/shellcrafter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-14 00:02:10.000000 shellcrafter-1.0.4/src/shellcrafter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 00:02:10.000000 shellcrafter-1.0.4/src/shellcrafter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-14 00:02:10.000000 shellcrafter-1.0.4/src/shellcrafter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-14 00:02:10.000000 shellcrafter-1.0.4/src/shellcrafter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-14 00:02:10.000000 shellcrafter-1.0.4/src/shellcrafter.egg-info/top_level.txt
```

### Comparing `shellcrafter-1.0.3/PKG-INFO` & `shellcrafter-1.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-Metadata-Version: 2.1
-Name: shellcrafter
-Version: 1.0.3
-Summary: A package containing scripts for developing and generating shellcode
-Author: totekuh
-Author-email: totekuh@protonmail.com
-
 # Shellcrafter
 
 Shellcrafter is a package containing scripts for developing and generating shellcode. 
 
 It provides a collection of utilities for working with shellcode in various ways, such as generating shellcode from assembly instructions, computing hashes from function names, converting ASCII text to hex stack push instructions, and finding ROP gadgets.
 
 ## Installation
```

### Comparing `shellcrafter-1.0.3/README.md` & `shellcrafter-1.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: shellcrafter
+Version: 1.0.4
+Summary: A package containing scripts for developing and generating shellcode
+Home-page: https://github.com/totekuh/shellcrafter
+Author: totekuh
+Author-email: totekuh@protonmail.com
+Project-URL: Bug Reports, https://github.com/totekuh/shellcrafter/issues
+Project-URL: Source, https://github.com/totekuh/shellcrafter
+
 # Shellcrafter
 
 Shellcrafter is a package containing scripts for developing and generating shellcode. 
 
 It provides a collection of utilities for working with shellcode in various ways, such as generating shellcode from assembly instructions, computing hashes from function names, converting ASCII text to hex stack push instructions, and finding ROP gadgets.
 
 ## Installation
```

### Comparing `shellcrafter-1.0.3/src/shellcrafter/ascii_hex_stack_push_converter.py` & `shellcrafter-1.0.4/src/shellcrafter/ascii_hex_stack_push_converter.py`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.0.3/src/shellcrafter/find_gadgets.py` & `shellcrafter-1.0.4/src/shellcrafter/find_gadgets.py`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.0.3/src/shellcrafter/keyst_api.py` & `shellcrafter-1.0.4/src/shellcrafter/keyst_api.py`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.0.3/src/shellcrafter/ror_hash.py` & `shellcrafter-1.0.4/src/shellcrafter/ror_hash.py`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.0.3/src/shellcrafter.egg-info/PKG-INFO` & `shellcrafter-1.0.4/src/shellcrafter.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: shellcrafter
-Version: 1.0.3
+Version: 1.0.4
 Summary: A package containing scripts for developing and generating shellcode
+Home-page: https://github.com/totekuh/shellcrafter
 Author: totekuh
 Author-email: totekuh@protonmail.com
+Project-URL: Bug Reports, https://github.com/totekuh/shellcrafter/issues
+Project-URL: Source, https://github.com/totekuh/shellcrafter
 
 # Shellcrafter
 
 Shellcrafter is a package containing scripts for developing and generating shellcode. 
 
 It provides a collection of utilities for working with shellcode in various ways, such as generating shellcode from assembly instructions, computing hashes from function names, converting ASCII text to hex stack push instructions, and finding ROP gadgets.
```

