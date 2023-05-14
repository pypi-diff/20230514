# Comparing `tmp/pyvantage-0.0.47.tar.gz` & `tmp/pyvantage-0.0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvantage-0.0.47.tar", last modified: Sun May 14 01:01:39 2023, max compression
+gzip compressed data, was "pyvantage-0.0.48.tar", last modified: Sun May 14 05:53:59 2023, max compression
```

## Comparing `pyvantage-0.0.47.tar` & `pyvantage-0.0.48.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-05-14 01:01:39.460224 pyvantage-0.0.47/
--rw-r--r--   0 greg       (501) staff       (20)     1179 2022-07-01 22:35:08.000000 pyvantage-0.0.47/LICENSE
--rw-r--r--   0 greg       (501) staff       (20)      604 2023-05-14 01:01:39.460327 pyvantage-0.0.47/PKG-INFO
--rw-r--r--   0 greg       (501) staff       (20)     2164 2022-07-01 22:35:08.000000 pyvantage-0.0.47/README.md
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-05-14 01:01:39.457820 pyvantage-0.0.47/pyvantage/
--rw-r--r--   0 greg       (501) staff       (20)   100259 2023-05-14 00:53:40.000000 pyvantage-0.0.47/pyvantage/__init__.py
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-05-14 01:01:39.459626 pyvantage-0.0.47/pyvantage.egg-info/
--rw-r--r--   0 greg       (501) staff       (20)      604 2023-05-14 01:01:39.000000 pyvantage-0.0.47/pyvantage.egg-info/PKG-INFO
--rw-r--r--   0 greg       (501) staff       (20)      218 2023-05-14 01:01:39.000000 pyvantage-0.0.47/pyvantage.egg-info/SOURCES.txt
--rw-r--r--   0 greg       (501) staff       (20)        1 2023-05-14 01:01:39.000000 pyvantage-0.0.47/pyvantage.egg-info/dependency_links.txt
--rw-r--r--   0 greg       (501) staff       (20)       10 2023-05-14 01:01:39.000000 pyvantage-0.0.47/pyvantage.egg-info/top_level.txt
--rw-r--r--   0 greg       (501) staff       (20)        1 2022-07-01 22:35:59.000000 pyvantage-0.0.47/pyvantage.egg-info/zip-safe
--rw-r--r--   0 greg       (501) staff       (20)       79 2023-05-14 01:01:39.460749 pyvantage-0.0.47/setup.cfg
--rw-r--r--   0 greg       (501) staff       (20)      769 2023-05-14 00:59:55.000000 pyvantage-0.0.47/setup.py
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-05-14 05:53:59.849878 pyvantage-0.0.48/
+-rw-r--r--   0 greg       (501) staff       (20)     1179 2022-07-01 22:35:08.000000 pyvantage-0.0.48/LICENSE
+-rw-r--r--   0 greg       (501) staff       (20)      604 2023-05-14 05:53:59.849979 pyvantage-0.0.48/PKG-INFO
+-rw-r--r--   0 greg       (501) staff       (20)     2164 2022-07-01 22:35:08.000000 pyvantage-0.0.48/README.md
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-05-14 05:53:59.847585 pyvantage-0.0.48/pyvantage/
+-rw-r--r--   0 greg       (501) staff       (20)   100350 2023-05-14 05:48:28.000000 pyvantage-0.0.48/pyvantage/__init__.py
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-05-14 05:53:59.849237 pyvantage-0.0.48/pyvantage.egg-info/
+-rw-r--r--   0 greg       (501) staff       (20)      604 2023-05-14 05:53:59.000000 pyvantage-0.0.48/pyvantage.egg-info/PKG-INFO
+-rw-r--r--   0 greg       (501) staff       (20)      218 2023-05-14 05:53:59.000000 pyvantage-0.0.48/pyvantage.egg-info/SOURCES.txt
+-rw-r--r--   0 greg       (501) staff       (20)        1 2023-05-14 05:53:59.000000 pyvantage-0.0.48/pyvantage.egg-info/dependency_links.txt
+-rw-r--r--   0 greg       (501) staff       (20)       10 2023-05-14 05:53:59.000000 pyvantage-0.0.48/pyvantage.egg-info/top_level.txt
+-rw-r--r--   0 greg       (501) staff       (20)        1 2022-07-01 22:35:59.000000 pyvantage-0.0.48/pyvantage.egg-info/zip-safe
+-rw-r--r--   0 greg       (501) staff       (20)       79 2023-05-14 05:53:59.850393 pyvantage-0.0.48/setup.cfg
+-rw-r--r--   0 greg       (501) staff       (20)      769 2023-05-14 05:50:41.000000 pyvantage-0.0.48/setup.py
```

### Comparing `pyvantage-0.0.47/LICENSE` & `pyvantage-0.0.48/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvantage-0.0.47/PKG-INFO` & `pyvantage-0.0.48/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvantage
-Version: 0.0.47
+Version: 0.0.48
 Summary: Python library for Vantage Controller (for Home Assistant)
 Home-page: http://github.com/gjbadros/pyvantage
 Author: Greg J. Badros
 Author-email: badros@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyvantage-0.0.47/README.md` & `pyvantage-0.0.48/README.md`

 * *Files identical despite different names*

### Comparing `pyvantage-0.0.47/pyvantage/__init__.py` & `pyvantage-0.0.48/pyvantage/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,22 +233,29 @@
         with self._lock:
             self._send_ascii_nl_locked(cmd, self._iconn)
             if not cmd.startswith("GET"):
                 self._iconn = (self._iconn + 1) % self._num_connections
 
     def _read_until(self, delimiter, i):
         """Read data from a socket until a delimiter is found."""
-        while True:
-            new_chunk = self._sockets[i].recv(1024)
-            if not new_chunk:
-                break
-            self._chunk += new_chunk
-            if delimiter in self._chunk:
-                break
-        [data, self._chunk] = self._chunk.split(delimiter, 1)
+        try:
+            while True:
+                new_chunk = self._sockets[i].recv(1024, socket.MSG_DONTWAIT)
+                if not new_chunk:
+                    break
+                self._chunk += new_chunk
+                if delimiter and delimiter in self._chunk:
+                    break
+        except socket.timeout:
+            pass
+        if delimiter:
+            [data, self._chunk] = self._chunk.split(delimiter, 1)
+        else:
+            data = self._chunk
+            self._chunk = b''
         return data
 
     def _do_login_locked(self, i):
         """Executes the login procedure as well as setting up some
         connection defaults like turning off the prompt, etc."""
         while True:
             try:
@@ -268,27 +275,27 @@
                 time.sleep(3)
                 continue
         if not (self._user is None or self._password is None):
             _LOGGER.debug("Connection #%s is made, logging in", i)
             self._send_ascii_nl_locked("LOGIN " + self._user +
                                        " " + self._password, i)
             _LOGGER.debug("reading login response for #%s", i)
-            self._read_until(b'\r\n', i)
+            self._read_until(False, i)
         if i == 0:
             self._send_ascii_nl_locked("STATUS LOAD", i)
-            self._read_until(b'\r\n', i)
+            self._read_until(False, i)
 
             self._send_ascii_nl_locked("STATUS BLIND", i)
-            self._read_until(b'\r\n', i)
+            self._read_until(False, i)
 
             self._send_ascii_nl_locked("STATUS BTN", i)
-            self._read_until(b'\r\n', i)
+            self._read_until(False, i)
 
             self._send_ascii_nl_locked("STATUS VARIABLE", i)
-            self._read_until(b'\r\n', i)
+            self._read_until(False, i)
         return True
 
     def _disconnect_locked(self):
         self._connected = [False] * self._num_connections
         self._connect_cond.notify_all()
 
         for i in range(0, self._num_connections):
@@ -321,20 +328,18 @@
                 readable, _, exceptional = select.select(self._sockets, [], [])
                 for i, sock in enumerate(self._sockets):
                     if sock in exceptional:
                         _LOGGER.error("Exceptional socket #%s: %s", i, t)
                         raise EOFError()
                     if sock in readable:
                         line = self._read_until(b'\r\n', i)
-                        lines = line.splitlines()
-                        for each_line in lines:
-                            try:
-                                self._recv_cb(each_line.decode('ascii').rstrip(), i)
-                            except Exception as e:
-                                _LOGGER.error("Exception in recv_cb on line %s: %s", each_line, e)
+                        try:
+                            self._recv_cb(line.decode('ascii').rstrip(), i)
+                        except Exception as e:
+                            _LOGGER.error("Exception in recv_cb on line %s: %s", line, e)
             except EOFError:
                 _LOGGER.warning("run got EOFError")
                 with self._lock:
                     self._disconnect_locked()
                 continue
             except BrokenPipeError:
                 _LOGGER.warning("run got BrokenPipeError")
```

### Comparing `pyvantage-0.0.47/pyvantage.egg-info/PKG-INFO` & `pyvantage-0.0.48/pyvantage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvantage
-Version: 0.0.47
+Version: 0.0.48
 Summary: Python library for Vantage Controller (for Home Assistant)
 Home-page: http://github.com/gjbadros/pyvantage
 Author: Greg J. Badros
 Author-email: badros@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyvantage-0.0.47/setup.py` & `pyvantage-0.0.48/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
     name='pyvantage',
-    version='0.0.47',
+    version='0.0.48',
     license='MIT',
     description='Python library for Vantage Controller (for Home Assistant)',
     author='Greg J. Badros',
     author_email='badros@gmail.com',
     url='http://github.com/gjbadros/pyvantage',
     packages=find_packages(),
     classifiers=[
```

