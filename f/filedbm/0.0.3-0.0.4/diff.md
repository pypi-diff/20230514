# Comparing `tmp/filedbm-0.0.3.tar.gz` & `tmp/filedbm-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filedbm-0.0.3.tar", last modified: Mon May  8 22:14:59 2023, max compression
+gzip compressed data, was "filedbm-0.0.4.tar", last modified: Sun May 14 08:51:35 2023, max compression
```

## Comparing `filedbm-0.0.3.tar` & `filedbm-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 22:14:59.440277 filedbm-0.0.3/
--rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2023-05-08 01:46:02.000000 filedbm-0.0.3/LICENSE
--rw-rw-r--   0 mike      (1000) mike      (1000)      663 2023-05-08 22:14:59.440277 filedbm-0.0.3/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      152 2023-05-08 01:50:12.000000 filedbm-0.0.3/README.rst
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 22:14:59.440277 filedbm-0.0.3/filedbm/
--rw-rw-r--   0 mike      (1000) mike      (1000)       70 2023-05-08 05:12:10.000000 filedbm-0.0.3/filedbm/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     7265 2023-05-08 22:09:12.000000 filedbm-0.0.3/filedbm/main.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 22:14:59.440277 filedbm-0.0.3/filedbm/tests/
--rw-rw-r--   0 mike      (1000) mike      (1000)      208 2023-05-08 01:48:21.000000 filedbm-0.0.3/filedbm/tests/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     4963 2023-05-08 21:36:23.000000 filedbm-0.0.3/filedbm/utils.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 22:14:59.440277 filedbm-0.0.3/filedbm.egg-info/
--rw-rw-r--   0 mike      (1000) mike      (1000)      663 2023-05-08 22:14:59.000000 filedbm-0.0.3/filedbm.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      255 2023-05-08 22:14:59.000000 filedbm-0.0.3/filedbm.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-05-08 22:14:59.000000 filedbm-0.0.3/filedbm.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        8 2023-05-08 22:14:59.000000 filedbm-0.0.3/filedbm.egg-info/top_level.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)      104 2023-05-08 01:48:21.000000 filedbm-0.0.3/pyproject.toml
--rw-rw-r--   0 mike      (1000) mike      (1000)       67 2023-05-08 22:14:59.440277 filedbm-0.0.3/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)     7116 2023-05-08 22:12:45.000000 filedbm-0.0.3/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-14 08:51:35.451410 filedbm-0.0.4/
+-rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2023-05-08 01:46:02.000000 filedbm-0.0.4/LICENSE
+-rw-rw-r--   0 mike      (1000) mike      (1000)      663 2023-05-14 08:51:35.451410 filedbm-0.0.4/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      152 2023-05-08 01:50:12.000000 filedbm-0.0.4/README.rst
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-14 08:51:35.451410 filedbm-0.0.4/filedbm/
+-rw-rw-r--   0 mike      (1000) mike      (1000)       70 2023-05-08 05:12:10.000000 filedbm-0.0.4/filedbm/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     8321 2023-05-14 08:50:51.000000 filedbm-0.0.4/filedbm/main.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-14 08:51:35.451410 filedbm-0.0.4/filedbm/tests/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      208 2023-05-08 01:48:21.000000 filedbm-0.0.4/filedbm/tests/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     5306 2023-05-14 08:48:26.000000 filedbm-0.0.4/filedbm/utils.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-14 08:51:35.451410 filedbm-0.0.4/filedbm.egg-info/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      663 2023-05-14 08:51:35.000000 filedbm-0.0.4/filedbm.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      255 2023-05-14 08:51:35.000000 filedbm-0.0.4/filedbm.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-05-14 08:51:35.000000 filedbm-0.0.4/filedbm.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        8 2023-05-14 08:51:35.000000 filedbm-0.0.4/filedbm.egg-info/top_level.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)      104 2023-05-08 01:48:21.000000 filedbm-0.0.4/pyproject.toml
+-rw-rw-r--   0 mike      (1000) mike      (1000)       67 2023-05-14 08:51:35.451410 filedbm-0.0.4/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7116 2023-05-14 08:50:58.000000 filedbm-0.0.4/setup.py
```

### Comparing `filedbm-0.0.3/LICENSE` & `filedbm-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `filedbm-0.0.3/PKG-INFO` & `filedbm-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filedbm
-Version: 0.0.3
+Version: 0.0.4
 Summary: A persistent key-value database
 Home-page: https://github.com/mullenkamp/filedbm
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: shelve dbm
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `filedbm-0.0.3/filedbm/main.py` & `filedbm-0.0.4/filedbm/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 
 """
-# import os
+import os
 import io
 import pathlib
 from collections.abc import Mapping, MutableMapping
 from typing import Any, Generic, Iterator, Union, Dict, List
 import shutil
+from time import time
 # from hashlib import blake2b
 
 # import utils
 from . import utils
 
 
 #######################################################
 ### Classes
 
 
 class FileDBM(MutableMapping):
     """
 
     """
-    def __init__(self, db_path: str, flag: str = "r", buffer_size: int=512000, n_bytes_key=2, n_bytes_value=4):
+    def __init__(self, db_path: str, flag: str = "r", buffer_size: int=512000, n_bytes_key: int=2, n_bytes_value: int=4, ttl: int=None):
         """
 
         """
         fp = pathlib.Path(db_path)
         fp_exists = fp.exists()
 
         if flag == "r":  # Open existing database for reading only (default)
@@ -48,57 +49,76 @@
         else:
             raise ValueError("Invalid flag")
 
         self._write = write
         self._buffer_size = buffer_size
         self._n_bytes_key = n_bytes_key
         self._n_bytes_value = n_bytes_value
+        self._ttl = ttl
 
         ## Load or assign encodings and attributes
         if not fp_exists:
             fp.mkdir(parents=True)
 
         self.db_path = fp
 
 
     def keys(self):
-        for key in utils.iter_keys_values(self.db_path, True, False, self._n_bytes_key, self._n_bytes_value):
+        for key in utils.iter_keys_values(self.db_path, True, False, self._n_bytes_key, self._n_bytes_value, self._ttl):
             yield key
 
     def items(self, keys: List[str]=None):
         if keys is None:
-            for key, value in utils.iter_keys_values(self.db_path, True, True, self._n_bytes_key, self._n_bytes_value):
+            for key, value in utils.iter_keys_values(self.db_path, True, True, self._n_bytes_key, self._n_bytes_value, self._ttl):
                 yield key, value
         else:
             for key in keys:
-                value = utils.get_value(self.db_path, key.encode(), self._n_bytes_key, self._n_bytes_value)
+                value = utils.get_value(self.db_path, key.encode(), self._n_bytes_key, self._n_bytes_value, self._ttl)
                 yield key, value
 
     def values(self, keys: List[str]=None):
         if keys is None:
-            for value in utils.iter_keys_values(self.db_path, False, True, self._n_bytes_key, self._n_bytes_value):
+            for value in utils.iter_keys_values(self.db_path, False, True, self._n_bytes_key, self._n_bytes_value, self._ttl):
                 yield value
         else:
             for key in keys:
-                value = utils.get_value(self.db_path, key.encode(), self._n_bytes_key, self._n_bytes_value)
+                value = utils.get_value(self.db_path, key.encode(), self._n_bytes_key, self._n_bytes_value, self._ttl)
                 yield value
 
     def __iter__(self):
         return self.keys()
 
     def __len__(self):
-        return len([file for file in self.db_path.iterdir() if file.is_file()])
+        count = 0
+
+        for file_path in self.db_path.iterdir():
+            if file_path.is_file():
+                if self._ttl is not None:
+                    if (time() - os.path.getmtime(file_path)) > self._ttl:
+                        file_path.unlink()
+                        continue
+                count += 1
+
+        return count
 
     def __contains__(self, key: str):
-        file_hashes = set(file.name for file in self.db_path.iterdir() if file.is_file())
-        key_hash = utils.hash_key(key.encode())
-        return key_hash.hex() in file_hashes
+        key_hash_hex = utils.hash_key(key.encode())
+        file_path = self.db_path.joinpath(key_hash_hex)
+
+        if file_path.is_file():
+            if self._ttl is not None:
+                if (time() - os.path.getmtime(file_path)) > self._ttl:
+                    file_path.unlink()
+                    return False
+            return True
+        else:
+            return False
 
     def get(self, key: str, default=None):
-        value = utils.get_value(self.db_path, key.encode(), self._n_bytes_key, self._n_bytes_value)
+        value = utils.get_value(self.db_path, key.encode(), self._n_bytes_key, self._n_bytes_value, self._ttl)
 
         if value is None:
             return default
         else:
             return value
 
     def update(self, key_value_dict: Union[Dict[str, bytes], Dict[str, io.IOBase]]):
@@ -109,15 +129,15 @@
             for key, value in key_value_dict.items():
                 self[key.encode()] = value
         else:
             raise ValueError('File is open for read only.')
 
 
     def __getitem__(self, key: str):
-        value = utils.get_value(self.db_path, key.encode(), self._n_bytes_key, self._n_bytes_value)
+        value = utils.get_value(self.db_path, key.encode(), self._n_bytes_key, self._n_bytes_value, self._ttl)
 
         if value is None:
             raise KeyError(key)
         else:
             return value
 
 
@@ -126,15 +146,15 @@
             utils.write_data_block(self.db_path, key.encode(), value, self._n_bytes_key, self._n_bytes_value, self._buffer_size)
         else:
             raise ValueError('File is open for read only.')
 
     def __delitem__(self, key: str):
         if self._write:
             key_hash = utils.hash_key(key.encode())
-            file_path = self.db_path.joinpath(key_hash.hex())
+            file_path = self.db_path.joinpath(key_hash)
 
             if not file_path.exists():
                 raise KeyError(key)
 
             file_path.unlink()
         else:
             raise ValueError('File is open for read only.')
@@ -168,17 +188,17 @@
     #         self._mm.write(utils.int_to_bytes(self._n_keys, 4))
     #         self._mm.flush()
     #         self._file.flush()
 
 
 
 def open(
-    db_path: str, flag: str = "r", buffer_size: int=512000, n_bytes_key=2, n_bytes_value=4):
+    db_path: str, flag: str = "r", buffer_size: int=512000, n_bytes_key: int=2, n_bytes_value: int=4, ttl: int=None):
     """
-    Open a persistent dictionary for reading and writing. All keys and values are stored in individual files within the db_path. Keys must be strings and values must be either bytes or file-objects.
+    Open a persistent dictionary for reading and writing. All keys and values are stored in individual files within the db_path. Keys must be strings and values must be either bytes or file-objects. In the future, I might add more flexibility for inputs and outputs.
 
     Parameters
     -----------
     db_path : str or pathlib.Path
         It must be a path to a folder. If the folder doesn't exist, it will be created if flags 'c' or 'n' are passed.
 
     flag : str
@@ -189,17 +209,20 @@
 
     n_bytes_key : int
         The number of bytes to represent an integer of the max length of each key.
 
     n_bytes_value : int
         The number of bytes to represent an integer of the max length of each value.
 
+    ttl : int or None
+        Give the database a Time To Live (ttl) lifetime in seconds. All objects will persist in the database for at least this length. The objects will be removed when any query is performed on the database. The default None will not assign a ttl. The ttl will only be changed if the flag parameter is set to anything but "r".
+
     Returns
     -------
-    Booklet
+    FileDBM
 
     The optional *flag* argument can be:
 
     +---------+-------------------------------------------+
     | Value   | Meaning                                   |
     +=========+===========================================+
     | ``'r'`` | Open existing database for reading only   |
@@ -211,8 +234,8 @@
     | ``'c'`` | Open database for reading and writing,    |
     |         | creating it if it doesn't exist           |
     +---------+-------------------------------------------+
     | ``'n'`` | Always create a new, empty database, open |
     |         | for reading and writing                   |
     +---------+-------------------------------------------+
     """
-    return FileDBM(db_path, flag, buffer_size, n_bytes_key, n_bytes_value)
+    return FileDBM(db_path, flag, buffer_size, n_bytes_key, n_bytes_value, ttl)
```

### Comparing `filedbm-0.0.3/filedbm/utils.py` & `filedbm-0.0.4/filedbm/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 """
 import os
 import io
 from hashlib import blake2b, blake2s
 # from time import time
 from typing import Any, Generic, Iterator, Union
 import mmap
+from time import time
 
 ############################################
 ### Parameters
 
 key_hash_len = 13
 
 
@@ -71,15 +72,15 @@
     return i.to_bytes(byte_len, 'little', signed=signed)
 
 
 def hash_key(key):
     """
 
     """
-    return blake2s(key, digest_size=key_hash_len).digest()
+    return blake2s(key, digest_size=key_hash_len).digest().hex()
 
 
 def determine_obj_size(file_obj):
     """
 
     """
     pos = file_obj.tell()
@@ -119,41 +120,50 @@
         # mm.seek(key_len, 1)
         # value = mm.read(value_len)
         return value
     else:
         raise ValueError('One or both key and value must be True.')
 
 
-def get_value(db_path, key, n_bytes_key, n_bytes_value):
+def get_value(db_path, key, n_bytes_key, n_bytes_value, ttl=None):
     """
 
     """
     key_bytes_len = len(key)
     key_hash = hash_key(key)
-    file_path = db_path.joinpath(key_hash.hex())
+    file_path = db_path.joinpath(key_hash)
     if file_path.exists():
+        if ttl is not None:
+            if (time() - os.path.getmtime(file_path)) > ttl:
+                file_path.unlink()
+                return None
+
         file = io.open(file_path, 'rb')
         mm = mmap.mmap(file.fileno(), 0, access=mmap.ACCESS_READ)
 
         file_len = len(mm)
 
         value_pos = n_bytes_key + n_bytes_value + key_bytes_len
 
         out = FileObjectSlice(mm, value_pos, file_len - value_pos)
-    else:
-        out = None
 
-    return out
+        return out
+    else:
+        return None
 
 
-def iter_keys_values(db_path, key=False, value=False, n_bytes_key=2, n_bytes_value=4):
+def iter_keys_values(db_path, key=False, value=False, n_bytes_key=2, n_bytes_value=4, ttl=None):
     """
 
     """
     for file_path in db_path.iterdir():
+        if ttl is not None:
+            if (time() - os.path.getmtime(file_path)) > ttl:
+                file_path.unlink()
+                continue
         file = io.open(file_path, 'rb')
         mm = mmap.mmap(file.fileno(), 0, access=mmap.ACCESS_READ)
 
         yield get_data_block(mm, key, value, n_bytes_key, n_bytes_value)
 
 
 def write_data_block(db_path, key, value, n_bytes_key, n_bytes_value, buffer_size):
@@ -166,15 +176,15 @@
     if isinstance(value, bytes):
         value = io.BytesIO(value)
 
     value_bytes_len = determine_obj_size(value)
 
     write_init_bytes = int_to_bytes(key_bytes_len, n_bytes_key) + int_to_bytes(value_bytes_len, n_bytes_value) + key
 
-    file_path = db_path.joinpath(key_hash.hex())
+    file_path = db_path.joinpath(key_hash)
 
     file = io.open(file_path, 'w+b')
     _ = file.write(write_init_bytes)
 
     if hasattr(value, '_buffer_size'):
         buffer_size = value._buffer_size
```

### Comparing `filedbm-0.0.3/filedbm.egg-info/PKG-INFO` & `filedbm-0.0.4/filedbm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filedbm
-Version: 0.0.3
+Version: 0.0.4
 Summary: A persistent key-value database
 Home-page: https://github.com/mullenkamp/filedbm
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: shelve dbm
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `filedbm-0.0.3/setup.py` & `filedbm-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # General parameters
 name = 'filedbm'
 main_package = 'filedbm'
-version = '0.0.3'
+version = '0.0.4'
 descrip = 'A persistent key-value database'
 
 # The below code is for readthedocs. To have sphinx/readthedocs interact with
 # the contained package, readthedocs needs to build the package. But the dependencies
 # should be installed via the conda yml env file rather than during the package build.
 if os.environ.get('READTHEDOCS', False) == 'True':
     INSTALL_REQUIRES = []
```

