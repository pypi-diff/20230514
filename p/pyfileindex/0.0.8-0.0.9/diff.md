# Comparing `tmp/pyfileindex-0.0.8.tar.gz` & `tmp/pyfileindex-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfileindex-0.0.8.tar", last modified: Sat May 13 00:14:10 2023, max compression
+gzip compressed data, was "pyfileindex-0.0.9.tar", last modified: Sun May 14 01:51:00 2023, max compression
```

## Comparing `pyfileindex-0.0.8.tar` & `pyfileindex-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:14:10.417634 pyfileindex-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-13 00:14:04.000000 pyfileindex-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-13 00:14:04.000000 pyfileindex-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-13 00:14:10.417634 pyfileindex-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-13 00:14:04.000000 pyfileindex-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:14:10.417634 pyfileindex-0.0.8/pyfileindex/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-13 00:14:04.000000 pyfileindex-0.0.8/pyfileindex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-13 00:14:10.417634 pyfileindex-0.0.8/pyfileindex/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-05-13 00:14:04.000000 pyfileindex-0.0.8/pyfileindex/pyfileindex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:14:10.417634 pyfileindex-0.0.8/pyfileindex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-13 00:14:10.000000 pyfileindex-0.0.8/pyfileindex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-13 00:14:10.000000 pyfileindex-0.0.8/pyfileindex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 00:14:10.000000 pyfileindex-0.0.8/pyfileindex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-13 00:14:10.000000 pyfileindex-0.0.8/pyfileindex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-13 00:14:10.000000 pyfileindex-0.0.8/pyfileindex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-13 00:14:10.417634 pyfileindex-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-13 00:14:09.000000 pyfileindex-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:14:10.417634 pyfileindex-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    15991 2023-05-13 00:14:04.000000 pyfileindex-0.0.8/tests/test_pyfileindex.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-05-13 00:14:04.000000 pyfileindex-0.0.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:51:00.015520 pyfileindex-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-14 01:50:54.000000 pyfileindex-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-14 01:50:54.000000 pyfileindex-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-14 01:51:00.015520 pyfileindex-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-14 01:50:54.000000 pyfileindex-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:51:00.015520 pyfileindex-0.0.9/pyfileindex/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-14 01:50:54.000000 pyfileindex-0.0.9/pyfileindex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-14 01:51:00.015520 pyfileindex-0.0.9/pyfileindex/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-05-14 01:50:54.000000 pyfileindex-0.0.9/pyfileindex/pyfileindex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:51:00.015520 pyfileindex-0.0.9/pyfileindex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-14 01:51:00.000000 pyfileindex-0.0.9/pyfileindex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-14 01:51:00.000000 pyfileindex-0.0.9/pyfileindex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 01:51:00.000000 pyfileindex-0.0.9/pyfileindex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-14 01:51:00.000000 pyfileindex-0.0.9/pyfileindex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 01:51:00.000000 pyfileindex-0.0.9/pyfileindex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-14 01:51:00.015520 pyfileindex-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-14 01:50:59.000000 pyfileindex-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:51:00.015520 pyfileindex-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    16770 2023-05-14 01:50:54.000000 pyfileindex-0.0.9/tests/test_pyfileindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-05-14 01:50:54.000000 pyfileindex-0.0.9/versioneer.py
```

### Comparing `pyfileindex-0.0.8/LICENSE` & `pyfileindex-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfileindex-0.0.8/PKG-INFO` & `pyfileindex-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfileindex
-Version: 0.0.8
+Version: 0.0.9
 Summary: pyfileindex - pythonic file system index
 Home-page: https://github.com/pyfileindex/pyfileindex
 Author: Jan Janssen
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyfileindex
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyfileindex-0.0.8/README.md` & `pyfileindex-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyfileindex-0.0.8/pyfileindex/pyfileindex.py` & `pyfileindex-0.0.9/pyfileindex/pyfileindex.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,17 +16,19 @@
         path (str): file system path
         filter_function (function): function to filter for specific files (optional)
         debug (bool): enable debug print statements (optional)
         df (pandas.DataFrame): DataFrame of a previous PyFileIndex object (optional)
     """
 
     def __init__(self, path=".", filter_function=None, debug=False, df=None):
+        abs_path = os.path.abspath(os.path.expanduser(path))
+        self._check_if_path_exists(path=abs_path)
         self._debug = debug
         self._filter_function = filter_function
-        self._path = os.path.abspath(os.path.expanduser(path))
+        self._path = abs_path
         if df is None:
             self._df = self._create_df_from_lst(
                 list([self._get_lst_entry_from_path(entry=self._path)])
                 + list(self._scandir(path=self._path, df=None, recursive=True))
             )
         else:
             self._df = df
@@ -46,32 +48,36 @@
         Args:
              path (str): subdirectory to open
 
         Returns:
             PyFileIndex: PyFileIndex for subdirectory
         """
         abs_path = os.path.abspath(os.path.expanduser(os.path.join(self._path, path)))
+        self._check_if_path_exists(path=abs_path)
         if abs_path == self._path:
             return self
         elif os.path.commonpath([abs_path, self._path]) == self._path:
             return PyFileIndex(
                 path=abs_path,
                 filter_function=self._filter_function,
                 debug=self._debug,
                 df=self._df[self._df["path"].str.contains(abs_path)],
             )
         else:
             return PyFileIndex(
-                path=abs_path, filter_function=self._filter_function, debug=self._debug
+                path=abs_path,
+                filter_function=self._filter_function,
+                debug=self._debug,
             )
 
     def update(self):
         """
         Update file index
         """
+        self._check_if_path_exists(path=self._path)
         df_new, files_changed_lst, path_deleted_lst = self._get_changes_quick()
         if self._debug:
             print("Changes: ", df_new.path.values, files_changed_lst, path_deleted_lst)
         if len(path_deleted_lst) != 0:
             self._df = self._df[~self._df.path.isin(path_deleted_lst)]
         if len(files_changed_lst) != 0:
             df_updated = self._create_df_from_lst(
@@ -241,14 +247,21 @@
 
         Returns:
             HTML object: iPython notebook representation of the pandas.DataFrame
         """
         return self._df._repr_html_()
 
     @staticmethod
+    def _check_if_path_exists(path):
+        if not os.path.exists(path):
+            raise FileNotFoundError(
+                "The path " + path + " does not exist on your filesystem."
+            )
+
+    @staticmethod
     def _create_df_from_lst(lst):
         """
         Internal function to generate file index as pandas from a list of entries
 
         Args:
             lst (list): list of file index entries
```

### Comparing `pyfileindex-0.0.8/pyfileindex.egg-info/PKG-INFO` & `pyfileindex-0.0.9/pyfileindex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfileindex
-Version: 0.0.8
+Version: 0.0.9
 Summary: pyfileindex - pythonic file system index
 Home-page: https://github.com/pyfileindex/pyfileindex
 Author: Jan Janssen
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyfileindex
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyfileindex-0.0.8/setup.py` & `pyfileindex-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `pyfileindex-0.0.8/tests/test_pyfileindex.py` & `pyfileindex-0.0.9/tests/test_pyfileindex.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import unittest
 import os
+import pandas
 from time import sleep
 from pyfileindex import PyFileIndex
 
 
 def filter_function(file_name):
     return ".txt" in file_name
 
@@ -389,7 +390,25 @@
 
     def test_repr_html(self):
         html_str = self.fi_with_filter._repr_html_()
         self.assertEqual(html_str.count("div"), 2)
         self.assertEqual(html_str.count("table"), 2)
         self.assertEqual(html_str.count("tr"), 8)
         self.assertEqual(html_str.count("td"), 24)
+
+    def test_init_df_lst(self):
+        self.assertEqual(
+            type(self.fi_with_filter._init_df_lst(path_lst=[self.fi_with_filter._path])),
+            pandas.DataFrame
+        )
+
+    def test_get_changes_quick(self):
+        _, files_changed_lst, path_deleted_lst = self.fi_with_filter._get_changes_quick()
+        if os.name != "nt":
+            self.assertEqual(files_changed_lst, [])
+            self.assertEqual(path_deleted_lst.tolist(), [])
+        with self.assertRaises(FileNotFoundError):
+            _, files_changed_lst, path_deleted_lst = self.fi_with_filter.open("no_such_folder")._get_changes_quick()
+
+    def test_folder_does_not_exist(self):
+        with self.assertRaises(FileNotFoundError):
+            PyFileIndex(path="no_such_folder")
```

### Comparing `pyfileindex-0.0.8/versioneer.py` & `pyfileindex-0.0.9/versioneer.py`

 * *Files identical despite different names*

