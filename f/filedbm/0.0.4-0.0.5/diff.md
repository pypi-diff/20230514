# Comparing `tmp/filedbm-0.0.4.tar.gz` & `tmp/filedbm-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filedbm-0.0.4.tar", last modified: Sun May 14 08:51:35 2023, max compression
+gzip compressed data, was "filedbm-0.0.5.tar", last modified: Sun May 14 20:38:05 2023, max compression
```

## Comparing `filedbm-0.0.4.tar` & `filedbm-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-14 08:51:35.451410 filedbm-0.0.4/
--rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2023-05-08 01:46:02.000000 filedbm-0.0.4/LICENSE
--rw-rw-r--   0 mike      (1000) mike      (1000)      663 2023-05-14 08:51:35.451410 filedbm-0.0.4/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      152 2023-05-08 01:50:12.000000 filedbm-0.0.4/README.rst
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-14 08:51:35.451410 filedbm-0.0.4/filedbm/
--rw-rw-r--   0 mike      (1000) mike      (1000)       70 2023-05-08 05:12:10.000000 filedbm-0.0.4/filedbm/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     8321 2023-05-14 08:50:51.000000 filedbm-0.0.4/filedbm/main.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-14 08:51:35.451410 filedbm-0.0.4/filedbm/tests/
--rw-rw-r--   0 mike      (1000) mike      (1000)      208 2023-05-08 01:48:21.000000 filedbm-0.0.4/filedbm/tests/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     5306 2023-05-14 08:48:26.000000 filedbm-0.0.4/filedbm/utils.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-14 08:51:35.451410 filedbm-0.0.4/filedbm.egg-info/
--rw-rw-r--   0 mike      (1000) mike      (1000)      663 2023-05-14 08:51:35.000000 filedbm-0.0.4/filedbm.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      255 2023-05-14 08:51:35.000000 filedbm-0.0.4/filedbm.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-05-14 08:51:35.000000 filedbm-0.0.4/filedbm.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        8 2023-05-14 08:51:35.000000 filedbm-0.0.4/filedbm.egg-info/top_level.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)      104 2023-05-08 01:48:21.000000 filedbm-0.0.4/pyproject.toml
--rw-rw-r--   0 mike      (1000) mike      (1000)       67 2023-05-14 08:51:35.451410 filedbm-0.0.4/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)     7116 2023-05-14 08:50:58.000000 filedbm-0.0.4/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-14 20:38:05.356268 filedbm-0.0.5/
+-rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2023-05-08 01:46:02.000000 filedbm-0.0.5/LICENSE
+-rw-rw-r--   0 mike      (1000) mike      (1000)      663 2023-05-14 20:38:05.356268 filedbm-0.0.5/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      152 2023-05-08 01:50:12.000000 filedbm-0.0.5/README.rst
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-14 20:38:05.356268 filedbm-0.0.5/filedbm/
+-rw-rw-r--   0 mike      (1000) mike      (1000)       70 2023-05-08 05:12:10.000000 filedbm-0.0.5/filedbm/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     8341 2023-05-14 20:37:19.000000 filedbm-0.0.5/filedbm/main.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-14 20:38:05.356268 filedbm-0.0.5/filedbm/tests/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      208 2023-05-08 01:48:21.000000 filedbm-0.0.5/filedbm/tests/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     5306 2023-05-14 08:48:26.000000 filedbm-0.0.5/filedbm/utils.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-14 20:38:05.356268 filedbm-0.0.5/filedbm.egg-info/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      663 2023-05-14 20:38:05.000000 filedbm-0.0.5/filedbm.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      255 2023-05-14 20:38:05.000000 filedbm-0.0.5/filedbm.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-05-14 20:38:05.000000 filedbm-0.0.5/filedbm.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        8 2023-05-14 20:38:05.000000 filedbm-0.0.5/filedbm.egg-info/top_level.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)      104 2023-05-08 01:48:21.000000 filedbm-0.0.5/pyproject.toml
+-rw-rw-r--   0 mike      (1000) mike      (1000)       67 2023-05-14 20:38:05.356268 filedbm-0.0.5/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7116 2023-05-14 20:37:47.000000 filedbm-0.0.5/setup.py
```

### Comparing `filedbm-0.0.4/LICENSE` & `filedbm-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `filedbm-0.0.4/PKG-INFO` & `filedbm-0.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filedbm
-Version: 0.0.4
+Version: 0.0.5
 Summary: A persistent key-value database
 Home-page: https://github.com/mullenkamp/filedbm
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: shelve dbm
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `filedbm-0.0.4/filedbm/main.py` & `filedbm-0.0.5/filedbm/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,21 +28,22 @@
         """
 
         """
         fp = pathlib.Path(db_path)
         fp_exists = fp.exists()
 
         if flag == "r":  # Open existing database for reading only (default)
-            write = False
             if not fp_exists:
                 raise FileNotFoundError(db_path + ' not found.')
+            write = False
+            ttl = None
         elif flag == "w":  # Open existing database for reading and writing
-            write = True
             if not fp_exists:
                 raise FileNotFoundError(db_path + ' not found.')
+            write = True
         elif flag == "c":  # Open database for reading and writing, creating it if it doesn't exist
             write = True
         elif flag == "n":  # Always create a new, empty database, open for reading and writing
             write = True
             if fp_exists:
                 shutil.rmtree(fp, ignore_errors=True)
             fp_exists = False
@@ -210,15 +211,15 @@
     n_bytes_key : int
         The number of bytes to represent an integer of the max length of each key.
 
     n_bytes_value : int
         The number of bytes to represent an integer of the max length of each value.
 
     ttl : int or None
-        Give the database a Time To Live (ttl) lifetime in seconds. All objects will persist in the database for at least this length. The objects will be removed when any query is performed on the database. The default None will not assign a ttl. The ttl will only be changed if the flag parameter is set to anything but "r".
+        Give the database a Time To Live (ttl) lifetime in seconds. All objects will persist in the database for at least this length. The objects will be removed when any query is performed on the database. The default None will not assign a ttl. The ttl will only be used if the flag parameter is set to anything but "r".
 
     Returns
     -------
     FileDBM
 
     The optional *flag* argument can be:
```

### Comparing `filedbm-0.0.4/filedbm/utils.py` & `filedbm-0.0.5/filedbm/utils.py`

 * *Files identical despite different names*

### Comparing `filedbm-0.0.4/filedbm.egg-info/PKG-INFO` & `filedbm-0.0.5/filedbm.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filedbm
-Version: 0.0.4
+Version: 0.0.5
 Summary: A persistent key-value database
 Home-page: https://github.com/mullenkamp/filedbm
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: shelve dbm
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `filedbm-0.0.4/setup.py` & `filedbm-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # General parameters
 name = 'filedbm'
 main_package = 'filedbm'
-version = '0.0.4'
+version = '0.0.5'
 descrip = 'A persistent key-value database'
 
 # The below code is for readthedocs. To have sphinx/readthedocs interact with
 # the contained package, readthedocs needs to build the package. But the dependencies
 # should be installed via the conda yml env file rather than during the package build.
 if os.environ.get('READTHEDOCS', False) == 'True':
     INSTALL_REQUIRES = []
```

