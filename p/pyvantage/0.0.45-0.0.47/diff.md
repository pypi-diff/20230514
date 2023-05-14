# Comparing `tmp/pyvantage-0.0.45.tar.gz` & `tmp/pyvantage-0.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvantage-0.0.45.tar", last modified: Sat May 13 20:33:03 2023, max compression
+gzip compressed data, was "pyvantage-0.0.47.tar", last modified: Sun May 14 01:01:39 2023, max compression
```

## Comparing `pyvantage-0.0.45.tar` & `pyvantage-0.0.47.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-05-13 20:33:03.379623 pyvantage-0.0.45/
--rw-r--r--   0 greg       (501) staff       (20)     1179 2022-07-01 22:35:08.000000 pyvantage-0.0.45/LICENSE
--rw-r--r--   0 greg       (501) staff       (20)      604 2023-05-13 20:33:03.379736 pyvantage-0.0.45/PKG-INFO
--rw-r--r--   0 greg       (501) staff       (20)     2164 2022-07-01 22:35:08.000000 pyvantage-0.0.45/README.md
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-05-13 20:33:03.377123 pyvantage-0.0.45/pyvantage/
--rw-r--r--   0 greg       (501) staff       (20)    99977 2023-05-13 20:31:30.000000 pyvantage-0.0.45/pyvantage/__init__.py
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-05-13 20:33:03.378971 pyvantage-0.0.45/pyvantage.egg-info/
--rw-r--r--   0 greg       (501) staff       (20)      604 2023-05-13 20:33:03.000000 pyvantage-0.0.45/pyvantage.egg-info/PKG-INFO
--rw-r--r--   0 greg       (501) staff       (20)      218 2023-05-13 20:33:03.000000 pyvantage-0.0.45/pyvantage.egg-info/SOURCES.txt
--rw-r--r--   0 greg       (501) staff       (20)        1 2023-05-13 20:33:03.000000 pyvantage-0.0.45/pyvantage.egg-info/dependency_links.txt
--rw-r--r--   0 greg       (501) staff       (20)       10 2023-05-13 20:33:03.000000 pyvantage-0.0.45/pyvantage.egg-info/top_level.txt
--rw-r--r--   0 greg       (501) staff       (20)        1 2022-07-01 22:35:59.000000 pyvantage-0.0.45/pyvantage.egg-info/zip-safe
--rw-r--r--   0 greg       (501) staff       (20)       79 2023-05-13 20:33:03.380250 pyvantage-0.0.45/setup.cfg
--rw-r--r--   0 greg       (501) staff       (20)      769 2023-05-13 20:31:48.000000 pyvantage-0.0.45/setup.py
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-05-14 01:01:39.460224 pyvantage-0.0.47/
+-rw-r--r--   0 greg       (501) staff       (20)     1179 2022-07-01 22:35:08.000000 pyvantage-0.0.47/LICENSE
+-rw-r--r--   0 greg       (501) staff       (20)      604 2023-05-14 01:01:39.460327 pyvantage-0.0.47/PKG-INFO
+-rw-r--r--   0 greg       (501) staff       (20)     2164 2022-07-01 22:35:08.000000 pyvantage-0.0.47/README.md
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-05-14 01:01:39.457820 pyvantage-0.0.47/pyvantage/
+-rw-r--r--   0 greg       (501) staff       (20)   100259 2023-05-14 00:53:40.000000 pyvantage-0.0.47/pyvantage/__init__.py
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-05-14 01:01:39.459626 pyvantage-0.0.47/pyvantage.egg-info/
+-rw-r--r--   0 greg       (501) staff       (20)      604 2023-05-14 01:01:39.000000 pyvantage-0.0.47/pyvantage.egg-info/PKG-INFO
+-rw-r--r--   0 greg       (501) staff       (20)      218 2023-05-14 01:01:39.000000 pyvantage-0.0.47/pyvantage.egg-info/SOURCES.txt
+-rw-r--r--   0 greg       (501) staff       (20)        1 2023-05-14 01:01:39.000000 pyvantage-0.0.47/pyvantage.egg-info/dependency_links.txt
+-rw-r--r--   0 greg       (501) staff       (20)       10 2023-05-14 01:01:39.000000 pyvantage-0.0.47/pyvantage.egg-info/top_level.txt
+-rw-r--r--   0 greg       (501) staff       (20)        1 2022-07-01 22:35:59.000000 pyvantage-0.0.47/pyvantage.egg-info/zip-safe
+-rw-r--r--   0 greg       (501) staff       (20)       79 2023-05-14 01:01:39.460749 pyvantage-0.0.47/setup.cfg
+-rw-r--r--   0 greg       (501) staff       (20)      769 2023-05-14 00:59:55.000000 pyvantage-0.0.47/setup.py
```

### Comparing `pyvantage-0.0.45/LICENSE` & `pyvantage-0.0.47/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvantage-0.0.45/PKG-INFO` & `pyvantage-0.0.47/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvantage
-Version: 0.0.45
+Version: 0.0.47
 Summary: Python library for Vantage Controller (for Home Assistant)
 Home-page: http://github.com/gjbadros/pyvantage
 Author: Greg J. Badros
 Author-email: badros@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyvantage-0.0.45/README.md` & `pyvantage-0.0.47/README.md`

 * *Files identical despite different names*

### Comparing `pyvantage-0.0.45/pyvantage/__init__.py` & `pyvantage-0.0.47/pyvantage/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,14 +185,15 @@
         self._connected = [False] * num_connections
         self._iconn = 0  # index into the _sockets array
         self._lock = threading.RLock()
         self._connect_cond = threading.Condition(lock=self._lock)
         self._recv_cb = recv_callback
         self._done = False
         self._commdebug = commdebug
+        self._chunk = b''
 
         if use_ssl:
             self._ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS)
 
         self.setDaemon(True)
 
     def connect(self):
@@ -232,22 +233,22 @@
         with self._lock:
             self._send_ascii_nl_locked(cmd, self._iconn)
             if not cmd.startswith("GET"):
                 self._iconn = (self._iconn + 1) % self._num_connections
 
     def _read_until(self, delimiter, i):
         """Read data from a socket until a delimiter is found."""
-        data = b''
         while True:
-            chunk = self._sockets[i].recv(1024)
-            if not chunk:
+            new_chunk = self._sockets[i].recv(1024)
+            if not new_chunk:
                 break
-            data += chunk
-            if delimiter in data:
+            self._chunk += new_chunk
+            if delimiter in self._chunk:
                 break
+        [data, self._chunk] = self._chunk.split(delimiter, 1)
         return data
 
     def _do_login_locked(self, i):
         """Executes the login procedure as well as setting up some
         connection defaults like turning off the prompt, etc."""
         while True:
             try:
@@ -322,15 +323,18 @@
                     if sock in exceptional:
                         _LOGGER.error("Exceptional socket #%s: %s", i, t)
                         raise EOFError()
                     if sock in readable:
                         line = self._read_until(b'\r\n', i)
                         lines = line.splitlines()
                         for each_line in lines:
-                            self._recv_cb(each_line.decode('ascii').rstrip(), i)
+                            try:
+                                self._recv_cb(each_line.decode('ascii').rstrip(), i)
+                            except Exception as e:
+                                _LOGGER.error("Exception in recv_cb on line %s: %s", each_line, e)
             except EOFError:
                 _LOGGER.warning("run got EOFError")
                 with self._lock:
                     self._disconnect_locked()
                 continue
             except BrokenPipeError:
                 _LOGGER.warning("run got BrokenPipeError")
```

### Comparing `pyvantage-0.0.45/pyvantage.egg-info/PKG-INFO` & `pyvantage-0.0.47/pyvantage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvantage
-Version: 0.0.45
+Version: 0.0.47
 Summary: Python library for Vantage Controller (for Home Assistant)
 Home-page: http://github.com/gjbadros/pyvantage
 Author: Greg J. Badros
 Author-email: badros@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyvantage-0.0.45/setup.py` & `pyvantage-0.0.47/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
     name='pyvantage',
-    version='0.0.45',
+    version='0.0.47',
     license='MIT',
     description='Python library for Vantage Controller (for Home Assistant)',
     author='Greg J. Badros',
     author_email='badros@gmail.com',
     url='http://github.com/gjbadros/pyvantage',
     packages=find_packages(),
     classifiers=[
```

