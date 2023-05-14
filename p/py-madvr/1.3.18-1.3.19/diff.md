# Comparing `tmp/py_madvr-1.3.18.tar.gz` & `tmp/py_madvr-1.3.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_madvr-1.3.18.tar", last modified: Sun May 14 18:26:08 2023, max compression
+gzip compressed data, was "py_madvr-1.3.19.tar", last modified: Sun May 14 18:38:55 2023, max compression
```

## Comparing `py_madvr-1.3.18.tar` & `py_madvr-1.3.19.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:26:08.754089 py_madvr-1.3.18/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-14 18:25:55.000000 py_madvr-1.3.18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 18:26:08.754089 py_madvr-1.3.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-14 18:25:55.000000 py_madvr-1.3.18/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:26:08.754089 py_madvr-1.3.18/madvr/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-14 18:25:55.000000 py_madvr-1.3.18/madvr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-14 18:25:55.000000 py_madvr-1.3.18/madvr/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-14 18:25:55.000000 py_madvr-1.3.18/madvr/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15727 2023-05-14 18:25:55.000000 py_madvr-1.3.18/madvr/madvr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:26:08.754089 py_madvr-1.3.18/py_madvr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 18:26:08.000000 py_madvr-1.3.18/py_madvr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-14 18:26:08.000000 py_madvr-1.3.18/py_madvr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 18:26:08.000000 py_madvr-1.3.18/py_madvr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 18:26:08.000000 py_madvr-1.3.18/py_madvr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 18:26:08.754089 py_madvr-1.3.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-14 18:25:55.000000 py_madvr-1.3.18/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:26:08.754089 py_madvr-1.3.18/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 18:25:55.000000 py_madvr-1.3.18/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-14 18:25:55.000000 py_madvr-1.3.18/tests/testMadVR.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:38:55.624011 py_madvr-1.3.19/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-14 18:38:44.000000 py_madvr-1.3.19/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 18:38:55.620011 py_madvr-1.3.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-14 18:38:44.000000 py_madvr-1.3.19/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:38:55.620011 py_madvr-1.3.19/madvr/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-14 18:38:44.000000 py_madvr-1.3.19/madvr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-14 18:38:44.000000 py_madvr-1.3.19/madvr/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-14 18:38:44.000000 py_madvr-1.3.19/madvr/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16162 2023-05-14 18:38:44.000000 py_madvr-1.3.19/madvr/madvr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:38:55.620011 py_madvr-1.3.19/py_madvr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 18:38:55.000000 py_madvr-1.3.19/py_madvr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-14 18:38:55.000000 py_madvr-1.3.19/py_madvr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 18:38:55.000000 py_madvr-1.3.19/py_madvr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 18:38:55.000000 py_madvr-1.3.19/py_madvr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 18:38:55.624011 py_madvr-1.3.19/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-14 18:38:44.000000 py_madvr-1.3.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:38:55.620011 py_madvr-1.3.19/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 18:38:44.000000 py_madvr-1.3.19/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-14 18:38:44.000000 py_madvr-1.3.19/tests/testMadVR.py
```

### Comparing `py_madvr-1.3.18/LICENSE` & `py_madvr-1.3.19/LICENSE`

 * *Files identical despite different names*

### Comparing `py_madvr-1.3.18/PKG-INFO` & `py_madvr-1.3.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_madvr
-Version: 1.3.18
+Version: 1.3.19
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.3.18/madvr/commands.py` & `py_madvr-1.3.19/madvr/commands.py`

 * *Files identical despite different names*

### Comparing `py_madvr-1.3.18/madvr/madvr.py` & `py_madvr-1.3.19/madvr/madvr.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,38 +163,49 @@
         """
         Send a heartbeat to keep connection open
 
         You should wrap this in try with OSError and asyncio.TimeoutError exceptions
 
         Raises HeartBeatError exception
         """
+        if once:
+            try:
+                async with self.writer_lock:
+                    self.writer.write(self.HEARTBEAT)
+                    await self.writer.drain()
+
+                self.logger.debug("heartbeat complete")
+            except asyncio.TimeoutError:
+                self.logger.error("timeout when sending heartbeat")
+            except OSError:
+                self.logger.error("error when sending heartbeat")
+                await self._reconnect()
+
+            return
+
         while True:
             await self.connection_event.wait()
             # confirm can send heartbeat, ready for commands
             self.logger.debug("Sending heartbeats")
             try:
                 async with self.writer_lock:
                     self.writer.write(self.HEARTBEAT)
                     await self.writer.drain()
 
                 self.logger.debug("heartbeat complete")
-                if once:
-                    break
             except asyncio.TimeoutError:
                 self.logger.error("timeout when sending heartbeat")
             except OSError:
                 self.logger.error("error when sending heartbeat")
                 await self._reconnect()
             finally:
                 # Wait some time before the next heartbeat
                 await asyncio.sleep(15)
 
-    async def _construct_command(
-        self, raw_command: list[str]
-    ) -> tuple[bytes, str]:
+    async def _construct_command(self, raw_command: list[str]) -> tuple[bytes, str]:
         """
         Transform commands into their byte values from the string value
 
         Raises NotImplementedError
 
         Return:
             bytes: the value to send in bytes
```

### Comparing `py_madvr-1.3.18/py_madvr.egg-info/PKG-INFO` & `py_madvr-1.3.19/py_madvr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-madvr
-Version: 1.3.18
+Version: 1.3.19
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.3.18/setup.py` & `py_madvr-1.3.19/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_madvr",
-    version="1.3.18",
+    version="1.3.19",
     author="iloveicedgreentea",
     description="A package to control MadVR Envy over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/py-madvr",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `py_madvr-1.3.18/tests/testMadVR.py` & `py_madvr-1.3.19/tests/testMadVR.py`

 * *Files identical despite different names*

