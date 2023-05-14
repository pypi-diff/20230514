# Comparing `tmp/pyvantage-0.0.49.tar.gz` & `tmp/pyvantage-0.0.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvantage-0.0.49.tar", last modified: Sun May 14 06:27:44 2023, max compression
+gzip compressed data, was "pyvantage-0.0.50.tar", last modified: Sun May 14 06:46:09 2023, max compression
```

## Comparing `pyvantage-0.0.49.tar` & `pyvantage-0.0.50.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-05-14 06:27:44.616868 pyvantage-0.0.49/
--rw-r--r--   0 greg       (501) staff       (20)     1179 2022-07-01 22:35:08.000000 pyvantage-0.0.49/LICENSE
--rw-r--r--   0 greg       (501) staff       (20)      604 2023-05-14 06:27:44.616992 pyvantage-0.0.49/PKG-INFO
--rw-r--r--   0 greg       (501) staff       (20)     2164 2022-07-01 22:35:08.000000 pyvantage-0.0.49/README.md
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-05-14 06:27:44.614520 pyvantage-0.0.49/pyvantage/
--rw-r--r--   0 greg       (501) staff       (20)   100189 2023-05-14 06:24:06.000000 pyvantage-0.0.49/pyvantage/__init__.py
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-05-14 06:27:44.616300 pyvantage-0.0.49/pyvantage.egg-info/
--rw-r--r--   0 greg       (501) staff       (20)      604 2023-05-14 06:27:44.000000 pyvantage-0.0.49/pyvantage.egg-info/PKG-INFO
--rw-r--r--   0 greg       (501) staff       (20)      218 2023-05-14 06:27:44.000000 pyvantage-0.0.49/pyvantage.egg-info/SOURCES.txt
--rw-r--r--   0 greg       (501) staff       (20)        1 2023-05-14 06:27:44.000000 pyvantage-0.0.49/pyvantage.egg-info/dependency_links.txt
--rw-r--r--   0 greg       (501) staff       (20)       10 2023-05-14 06:27:44.000000 pyvantage-0.0.49/pyvantage.egg-info/top_level.txt
--rw-r--r--   0 greg       (501) staff       (20)        1 2022-07-01 22:35:59.000000 pyvantage-0.0.49/pyvantage.egg-info/zip-safe
--rw-r--r--   0 greg       (501) staff       (20)       79 2023-05-14 06:27:44.617437 pyvantage-0.0.49/setup.cfg
--rw-r--r--   0 greg       (501) staff       (20)      769 2023-05-14 06:27:31.000000 pyvantage-0.0.49/setup.py
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-05-14 06:46:09.270359 pyvantage-0.0.50/
+-rw-r--r--   0 greg       (501) staff       (20)     1179 2022-07-01 22:35:08.000000 pyvantage-0.0.50/LICENSE
+-rw-r--r--   0 greg       (501) staff       (20)      604 2023-05-14 06:46:09.270479 pyvantage-0.0.50/PKG-INFO
+-rw-r--r--   0 greg       (501) staff       (20)     2164 2022-07-01 22:35:08.000000 pyvantage-0.0.50/README.md
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-05-14 06:46:09.267681 pyvantage-0.0.50/pyvantage/
+-rw-r--r--   0 greg       (501) staff       (20)   100189 2023-05-14 06:44:28.000000 pyvantage-0.0.50/pyvantage/__init__.py
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-05-14 06:46:09.269732 pyvantage-0.0.50/pyvantage.egg-info/
+-rw-r--r--   0 greg       (501) staff       (20)      604 2023-05-14 06:46:09.000000 pyvantage-0.0.50/pyvantage.egg-info/PKG-INFO
+-rw-r--r--   0 greg       (501) staff       (20)      218 2023-05-14 06:46:09.000000 pyvantage-0.0.50/pyvantage.egg-info/SOURCES.txt
+-rw-r--r--   0 greg       (501) staff       (20)        1 2023-05-14 06:46:09.000000 pyvantage-0.0.50/pyvantage.egg-info/dependency_links.txt
+-rw-r--r--   0 greg       (501) staff       (20)       10 2023-05-14 06:46:09.000000 pyvantage-0.0.50/pyvantage.egg-info/top_level.txt
+-rw-r--r--   0 greg       (501) staff       (20)        1 2022-07-01 22:35:59.000000 pyvantage-0.0.50/pyvantage.egg-info/zip-safe
+-rw-r--r--   0 greg       (501) staff       (20)       79 2023-05-14 06:46:09.270937 pyvantage-0.0.50/setup.cfg
+-rw-r--r--   0 greg       (501) staff       (20)      769 2023-05-14 06:44:58.000000 pyvantage-0.0.50/setup.py
```

### Comparing `pyvantage-0.0.49/LICENSE` & `pyvantage-0.0.50/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvantage-0.0.49/PKG-INFO` & `pyvantage-0.0.50/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvantage
-Version: 0.0.49
+Version: 0.0.50
 Summary: Python library for Vantage Controller (for Home Assistant)
 Home-page: http://github.com/gjbadros/pyvantage
 Author: Greg J. Badros
 Author-email: badros@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyvantage-0.0.49/README.md` & `pyvantage-0.0.50/README.md`

 * *Files identical despite different names*

### Comparing `pyvantage-0.0.49/pyvantage/__init__.py` & `pyvantage-0.0.50/pyvantage/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -235,20 +235,20 @@
             if not cmd.startswith("GET"):
                 self._iconn = (self._iconn + 1) % self._num_connections
 
     def _read_until(self, delimiter, i):
         """Read data from a socket until a delimiter is found."""
         try:
             while True:
+                if delimiter in self._chunk:
+                    break
                 new_chunk = self._sockets[i].recv(1024)
                 if not new_chunk:
                     break
                 self._chunk += new_chunk
-                if delimiter in self._chunk:
-                    break
         except socket.timeout:
             pass
         [data, self._chunk] = self._chunk.split(delimiter, 1)
         return data
 
     def _do_login_locked(self, i):
         """Executes the login procedure as well as setting up some
```

### Comparing `pyvantage-0.0.49/pyvantage.egg-info/PKG-INFO` & `pyvantage-0.0.50/pyvantage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvantage
-Version: 0.0.49
+Version: 0.0.50
 Summary: Python library for Vantage Controller (for Home Assistant)
 Home-page: http://github.com/gjbadros/pyvantage
 Author: Greg J. Badros
 Author-email: badros@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyvantage-0.0.49/setup.py` & `pyvantage-0.0.50/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
     name='pyvantage',
-    version='0.0.49',
+    version='0.0.50',
     license='MIT',
     description='Python library for Vantage Controller (for Home Assistant)',
     author='Greg J. Badros',
     author_email='badros@gmail.com',
     url='http://github.com/gjbadros/pyvantage',
     packages=find_packages(),
     classifiers=[
```

