# Comparing `tmp/ctdd-0.0.2a3.tar.gz` & `tmp/ctdd-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctdd-0.0.2a3.tar", max compression
+gzip compressed data, was "ctdd-0.0.3.tar", max compression
```

## Comparing `ctdd-0.0.2a3.tar` & `ctdd-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1108 2023-05-03 17:25:05.122292 ctdd-0.0.2a3/LICENSE
--rw-r--r--   0        0        0     2025 2023-05-08 01:05:44.511002 ctdd-0.0.2a3/README.md
--rw-r--r--   0        0        0       65 2023-05-13 15:01:41.630543 ctdd-0.0.2a3/ctdd/__init__.py
--rw-r--r--   0        0        0     3075 2023-05-13 14:24:30.101636 ctdd-0.0.2a3/ctdd/__main__.py
--rw-r--r--   0        0        0     1167 2023-05-13 15:05:16.441656 ctdd-0.0.2a3/ctdd/ffi_factory.py
--rw-r--r--   0        0        0     1780 2023-05-13 14:55:04.404025 ctdd-0.0.2a3/ctdd/mocker.py
--rw-r--r--   0        0        0     2253 2023-05-13 15:00:31.125767 ctdd-0.0.2a3/ctdd/tester.py
--rw-r--r--   0        0        0     2510 2023-05-13 15:04:05.896870 ctdd-0.0.2a3/ctdd/tester_state.py
--rw-r--r--   0        0        0      738 2023-05-13 18:17:23.102739 ctdd-0.0.2a3/pyproject.toml
--rw-r--r--   0        0        0     2784 1970-01-01 00:00:00.000000 ctdd-0.0.2a3/PKG-INFO
+-rw-r--r--   0        0        0     1108 2023-05-03 17:25:05.122292 ctdd-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2025 2023-05-08 01:05:44.511002 ctdd-0.0.3/README.md
+-rw-r--r--   0        0        0       65 2023-05-13 15:01:41.630543 ctdd-0.0.3/ctdd/__init__.py
+-rw-r--r--   0        0        0     3075 2023-05-13 14:24:30.101636 ctdd-0.0.3/ctdd/__main__.py
+-rw-r--r--   0        0        0     1167 2023-05-13 15:05:16.441656 ctdd-0.0.3/ctdd/ffi_factory.py
+-rw-r--r--   0        0        0     1780 2023-05-13 14:55:04.404025 ctdd-0.0.3/ctdd/mocker.py
+-rw-r--r--   0        0        0     2253 2023-05-13 15:00:31.125767 ctdd-0.0.3/ctdd/tester.py
+-rw-r--r--   0        0        0     2547 2023-05-14 14:21:18.649983 ctdd-0.0.3/ctdd/tester_state.py
+-rw-r--r--   0        0        0      736 2023-05-14 14:28:10.091502 ctdd-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 ctdd-0.0.3/PKG-INFO
```

### Comparing `ctdd-0.0.2a3/LICENSE` & `ctdd-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ctdd-0.0.2a3/README.md` & `ctdd-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ctdd-0.0.2a3/ctdd/__main__.py` & `ctdd-0.0.3/ctdd/__main__.py`

 * *Files identical despite different names*

### Comparing `ctdd-0.0.2a3/ctdd/ffi_factory.py` & `ctdd-0.0.3/ctdd/ffi_factory.py`

 * *Files identical despite different names*

### Comparing `ctdd-0.0.2a3/ctdd/mocker.py` & `ctdd-0.0.3/ctdd/mocker.py`

 * *Files identical despite different names*

### Comparing `ctdd-0.0.2a3/ctdd/tester.py` & `ctdd-0.0.3/ctdd/tester.py`

 * *Files identical despite different names*

### Comparing `ctdd-0.0.2a3/ctdd/tester_state.py` & `ctdd-0.0.3/ctdd/tester_state.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 
         c_filename = f'{test_case_name}.c'
         h_filename = f'{test_case_name}.h'
 
         tube_name = name if name else test_case_name
 
         return CrelmFactory().create_Tube(tube_name) \
+            .save_compiler_temps() \
             .set_source_folder_relative(test_case_filename) \
             .add_source_file(c_filename) \
             .add_header_file(h_filename) \
             .add_externs(self.externs)
 
     def _ensure_tube(self):
         if not self.tube:
```

### Comparing `ctdd-0.0.2a3/pyproject.toml` & `ctdd-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ctdd"
-version = "0.0.2a3"
+version = "0.0.3"
 description = "C test-driven development framework implemented in Python"
 authors = [
   "WideOpenTech <fossie@wideopentech.co.uk>",
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -15,15 +15,15 @@
 
 [project.urls]
 "Homepage" = "https://github.com/wideopensource/ctdd"
 "Bug Tracker" = "https://github.com/wideopensource/ctdd/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-crelm = "^0.0.32"
+crelm = "^0.0.33"
 john = "^0.1.5"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ctdd-0.0.2a3/PKG-INFO` & `ctdd-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ctdd
-Version: 0.0.2a3
+Version: 0.0.3
 Summary: C test-driven development framework implemented in Python
 Home-page: https://github.com/wideopensource/ctdd
 Author: WideOpenTech
 Author-email: fossie@wideopentech.co.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: crelm (>=0.0.32,<0.0.33)
+Requires-Dist: crelm (>=0.0.33,<0.0.34)
 Requires-Dist: john (>=0.1.5,<0.2.0)
 Project-URL: Repository, https://github.com/wideopensource/ctdd
 Description-Content-Type: text/markdown
 
 # ctdd
 
 ## tl:dr
```

