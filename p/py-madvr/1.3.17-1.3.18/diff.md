# Comparing `tmp/py_madvr-1.3.17.tar.gz` & `tmp/py_madvr-1.3.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_madvr-1.3.17.tar", last modified: Sun May 14 18:17:49 2023, max compression
+gzip compressed data, was "py_madvr-1.3.18.tar", last modified: Sun May 14 18:26:08 2023, max compression
```

## Comparing `py_madvr-1.3.17.tar` & `py_madvr-1.3.18.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:17:49.334386 py_madvr-1.3.17/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-14 18:17:35.000000 py_madvr-1.3.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 18:17:49.334386 py_madvr-1.3.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-14 18:17:35.000000 py_madvr-1.3.17/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:17:49.330386 py_madvr-1.3.17/madvr/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-14 18:17:35.000000 py_madvr-1.3.17/madvr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-14 18:17:35.000000 py_madvr-1.3.17/madvr/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-14 18:17:35.000000 py_madvr-1.3.17/madvr/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-05-14 18:17:35.000000 py_madvr-1.3.17/madvr/madvr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:17:49.334386 py_madvr-1.3.17/py_madvr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 18:17:49.000000 py_madvr-1.3.17/py_madvr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-14 18:17:49.000000 py_madvr-1.3.17/py_madvr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 18:17:49.000000 py_madvr-1.3.17/py_madvr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 18:17:49.000000 py_madvr-1.3.17/py_madvr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 18:17:49.334386 py_madvr-1.3.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-14 18:17:35.000000 py_madvr-1.3.17/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:17:49.334386 py_madvr-1.3.17/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 18:17:35.000000 py_madvr-1.3.17/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-14 18:17:35.000000 py_madvr-1.3.17/tests/testMadVR.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:26:08.754089 py_madvr-1.3.18/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-14 18:25:55.000000 py_madvr-1.3.18/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 18:26:08.754089 py_madvr-1.3.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-14 18:25:55.000000 py_madvr-1.3.18/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:26:08.754089 py_madvr-1.3.18/madvr/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-14 18:25:55.000000 py_madvr-1.3.18/madvr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-14 18:25:55.000000 py_madvr-1.3.18/madvr/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-14 18:25:55.000000 py_madvr-1.3.18/madvr/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15727 2023-05-14 18:25:55.000000 py_madvr-1.3.18/madvr/madvr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:26:08.754089 py_madvr-1.3.18/py_madvr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 18:26:08.000000 py_madvr-1.3.18/py_madvr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-14 18:26:08.000000 py_madvr-1.3.18/py_madvr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 18:26:08.000000 py_madvr-1.3.18/py_madvr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 18:26:08.000000 py_madvr-1.3.18/py_madvr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 18:26:08.754089 py_madvr-1.3.18/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-14 18:25:55.000000 py_madvr-1.3.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:26:08.754089 py_madvr-1.3.18/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 18:25:55.000000 py_madvr-1.3.18/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-14 18:25:55.000000 py_madvr-1.3.18/tests/testMadVR.py
```

### Comparing `py_madvr-1.3.17/LICENSE` & `py_madvr-1.3.18/LICENSE`

 * *Files identical despite different names*

### Comparing `py_madvr-1.3.17/PKG-INFO` & `py_madvr-1.3.18/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_madvr
-Version: 1.3.17
+Version: 1.3.18
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.3.17/madvr/commands.py` & `py_madvr-1.3.18/madvr/commands.py`

 * *Files identical despite different names*

### Comparing `py_madvr-1.3.17/madvr/madvr.py` & `py_madvr-1.3.18/madvr/madvr.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
                     )
 
                 self.logger.info("Waiting for envy to be available")
                 # envy needs some time to setup new connections
                 await asyncio.sleep(3)
 
                 # handshake func
-                await self.send_heartbeat()
+                await self.send_heartbeat(True)
 
                 self.logger.info("Connection established")
 
                 self.is_on = True
                 self.is_closed = False
 
                 self.connection_event.set()
@@ -155,15 +155,15 @@
             # backoff to not spam HA
             except OSError as err:
                 self.logger.warning("Connecting failed, retrying in %s seconds", 2)
                 self.logger.debug(err)
                 await asyncio.sleep(2)
                 continue
 
-    async def send_heartbeat(self) -> None:
+    async def send_heartbeat(self, once=False) -> None:
         """
         Send a heartbeat to keep connection open
 
         You should wrap this in try with OSError and asyncio.TimeoutError exceptions
 
         Raises HeartBeatError exception
         """
@@ -173,14 +173,16 @@
             self.logger.debug("Sending heartbeats")
             try:
                 async with self.writer_lock:
                     self.writer.write(self.HEARTBEAT)
                     await self.writer.drain()
 
                 self.logger.debug("heartbeat complete")
+                if once:
+                    break
             except asyncio.TimeoutError:
                 self.logger.error("timeout when sending heartbeat")
             except OSError:
                 self.logger.error("error when sending heartbeat")
                 await self._reconnect()
             finally:
                 # Wait some time before the next heartbeat
```

### Comparing `py_madvr-1.3.17/py_madvr.egg-info/PKG-INFO` & `py_madvr-1.3.18/py_madvr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-madvr
-Version: 1.3.17
+Version: 1.3.18
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.3.17/setup.py` & `py_madvr-1.3.18/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_madvr",
-    version="1.3.17",
+    version="1.3.18",
     author="iloveicedgreentea",
     description="A package to control MadVR Envy over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/py-madvr",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `py_madvr-1.3.17/tests/testMadVR.py` & `py_madvr-1.3.18/tests/testMadVR.py`

 * *Files identical despite different names*

