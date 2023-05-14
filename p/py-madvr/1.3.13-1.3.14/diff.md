# Comparing `tmp/py_madvr-1.3.13.tar.gz` & `tmp/py_madvr-1.3.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_madvr-1.3.13.tar", last modified: Sun May 14 16:16:52 2023, max compression
+gzip compressed data, was "py_madvr-1.3.14.tar", last modified: Sun May 14 16:37:22 2023, max compression
```

## Comparing `py_madvr-1.3.13.tar` & `py_madvr-1.3.14.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:16:52.563301 py_madvr-1.3.13/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-14 16:16:41.000000 py_madvr-1.3.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 16:16:52.563301 py_madvr-1.3.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-14 16:16:41.000000 py_madvr-1.3.13/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:16:52.563301 py_madvr-1.3.13/madvr/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-14 16:16:41.000000 py_madvr-1.3.13/madvr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-14 16:16:41.000000 py_madvr-1.3.13/madvr/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-14 16:16:41.000000 py_madvr-1.3.13/madvr/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    14516 2023-05-14 16:16:41.000000 py_madvr-1.3.13/madvr/madvr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:16:52.563301 py_madvr-1.3.13/py_madvr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 16:16:52.000000 py_madvr-1.3.13/py_madvr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-14 16:16:52.000000 py_madvr-1.3.13/py_madvr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 16:16:52.000000 py_madvr-1.3.13/py_madvr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 16:16:52.000000 py_madvr-1.3.13/py_madvr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 16:16:52.563301 py_madvr-1.3.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-14 16:16:41.000000 py_madvr-1.3.13/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:16:52.563301 py_madvr-1.3.13/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:16:41.000000 py_madvr-1.3.13/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-14 16:16:41.000000 py_madvr-1.3.13/tests/testMadVR.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:37:22.255258 py_madvr-1.3.14/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-14 16:37:06.000000 py_madvr-1.3.14/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 16:37:22.255258 py_madvr-1.3.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-14 16:37:06.000000 py_madvr-1.3.14/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:37:22.255258 py_madvr-1.3.14/madvr/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-14 16:37:06.000000 py_madvr-1.3.14/madvr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-14 16:37:06.000000 py_madvr-1.3.14/madvr/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-14 16:37:06.000000 py_madvr-1.3.14/madvr/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14726 2023-05-14 16:37:06.000000 py_madvr-1.3.14/madvr/madvr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:37:22.255258 py_madvr-1.3.14/py_madvr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 16:37:22.000000 py_madvr-1.3.14/py_madvr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-14 16:37:22.000000 py_madvr-1.3.14/py_madvr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 16:37:22.000000 py_madvr-1.3.14/py_madvr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 16:37:22.000000 py_madvr-1.3.14/py_madvr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 16:37:22.255258 py_madvr-1.3.14/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-14 16:37:06.000000 py_madvr-1.3.14/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:37:22.255258 py_madvr-1.3.14/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:37:06.000000 py_madvr-1.3.14/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-14 16:37:06.000000 py_madvr-1.3.14/tests/testMadVR.py
```

### Comparing `py_madvr-1.3.13/LICENSE` & `py_madvr-1.3.14/LICENSE`

 * *Files identical despite different names*

### Comparing `py_madvr-1.3.13/madvr/commands.py` & `py_madvr-1.3.14/madvr/commands.py`

 * *Files identical despite different names*

### Comparing `py_madvr-1.3.13/madvr/madvr.py` & `py_madvr-1.3.14/madvr/madvr.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,18 @@
         connect_timeout: int = 5,
     ):
         self.host = host
         self.port = port
         self.connect_timeout: int = connect_timeout
         self.logger = logger
 
+        # used to indicate if connection is ready
+        self.connection_event = asyncio.Event()
+        self.stop_reconnect = asyncio.Event()
+
         # Const values
         self.MADVR_OK: Final = Connections.welcome.value
         self.HEARTBEAT: Final = Connections.heartbeat.value
 
         # stores all attributes
         self.msg_dict = {}
 
@@ -62,42 +66,46 @@
                 await self.writer.wait_closed()
             except AttributeError:
                 # means its already closed
                 pass
 
         self.reader = None
         self.is_closed = True
+        self.connection_event.clear()
 
         # Clear attr
         await self._clear_attr()
 
     async def open_connection(self) -> None:
         """Open a connection"""
         self.logger.debug("Starting open connection")
         try:
             await self._reconnect()
         except AckError as err:
             self.logger.error(err)
 
+    def stop(self):
+        """Stop reconnecting"""
+        self.stop_reconnect.set()
+
     async def _reconnect(self) -> None:
         """
         Initiate keep-alive connection. This should handle any error and reconnect eventually.
 
         Raises AckError
         """
-        i = 0
-        while i < 3:
+        while not self.stop_reconnect.is_set():
             try:
                 self.logger.info("Connecting to Envy: %s:%s", self.host, self.port)
 
                 # Command client
                 async with self.reader_lock:
                     self.reader, self.writer = await asyncio.wait_for(
                         asyncio.open_connection(self.host, self.port),
-                        timeout=self.command_read_timeout,
+                        timeout=2,
                     )
 
                 # Test heartbeat
                 self.logger.debug("Handshaking")
 
                 # Make sure first message says WELCOME
                 async with self.reader_lock:
@@ -121,45 +129,40 @@
                 await self._send_heartbeat()
 
                 self.logger.info("Connection established")
 
                 self.is_on = True
                 self.is_closed = False
 
+                self.connection_event.set()
+
                 return
 
             except HeartBeatError:
                 self.logger.warning(
                     "Error sending heartbeat, retrying in %s seconds", 2
                 )
                 await asyncio.sleep(2)
-                i += 1
                 continue
 
             # includes conn refused
             # backoff to not spam HA
             except asyncio.TimeoutError:
                 self.logger.warning("Connecting timeout, retrying in %s seconds", 2)
                 await asyncio.sleep(2)
-                i += 1
                 continue
 
             # includes conn refused
             # backoff to not spam HA
             except OSError as err:
                 self.logger.warning("Connecting failed, retrying in %s seconds", 2)
                 self.logger.debug(err)
                 await asyncio.sleep(2)
-                i += 1
                 continue
 
-            finally:
-                if i >= 3:
-                    self.logger.error("Failed to reconnect after 3 attempts")
-
     async def _send_heartbeat(self) -> None:
         """
         Send a heartbeat to keep connection open
 
         You should wrap this in try with OSError and asyncio.TimeoutError exceptions
 
         Raises HeartBeatError exception
@@ -294,14 +297,16 @@
         return ""
 
     async def read_notifications(self) -> None:
         """
         Read notifications from the server and update attributes
         """
         while True:
+            # wait until the connection is established
+            await self.connection_event.wait()
             try:
                 async with self.reader_lock:
                     msg = await asyncio.wait_for(
                         self.reader.read(self.read_limit),
                         timeout=self.command_read_timeout,
                     )
             except (AttributeError, asyncio.TimeoutError, OSError) as err:
```

### Comparing `py_madvr-1.3.13/py_madvr.egg-info/PKG-INFO` & `py_madvr-1.3.14/py_madvr.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-madvr
-Version: 1.3.13
+Version: 1.3.14
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.3.13/setup.py` & `py_madvr-1.3.14/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_madvr",
-    version="1.3.13",
+    version="1.3.14",
     author="iloveicedgreentea",
     description="A package to control MadVR Envy over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/py-madvr",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `py_madvr-1.3.13/tests/testMadVR.py` & `py_madvr-1.3.14/tests/testMadVR.py`

 * *Files identical despite different names*

