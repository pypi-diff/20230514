# Comparing `tmp/py_madvr-1.3.11.tar.gz` & `tmp/py_madvr-1.3.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_madvr-1.3.11.tar", last modified: Fri May 12 23:58:54 2023, max compression
+gzip compressed data, was "py_madvr-1.3.12.tar", last modified: Sun May 14 15:43:01 2023, max compression
```

## Comparing `py_madvr-1.3.11.tar` & `py_madvr-1.3.12.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:58:54.245922 py_madvr-1.3.11/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-12 23:58:40.000000 py_madvr-1.3.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-12 23:58:54.245922 py_madvr-1.3.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-12 23:58:40.000000 py_madvr-1.3.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:58:54.241922 py_madvr-1.3.11/madvr/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-12 23:58:40.000000 py_madvr-1.3.11/madvr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-12 23:58:40.000000 py_madvr-1.3.11/madvr/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-12 23:58:40.000000 py_madvr-1.3.11/madvr/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    14573 2023-05-12 23:58:40.000000 py_madvr-1.3.11/madvr/madvr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:58:54.245922 py_madvr-1.3.11/py_madvr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-12 23:58:54.000000 py_madvr-1.3.11/py_madvr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-12 23:58:54.000000 py_madvr-1.3.11/py_madvr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 23:58:54.000000 py_madvr-1.3.11/py_madvr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-12 23:58:54.000000 py_madvr-1.3.11/py_madvr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 23:58:54.245922 py_madvr-1.3.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-12 23:58:40.000000 py_madvr-1.3.11/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 23:58:54.245922 py_madvr-1.3.11/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 23:58:40.000000 py_madvr-1.3.11/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-12 23:58:40.000000 py_madvr-1.3.11/tests/testMadVR.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:43:01.518143 py_madvr-1.3.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-14 15:42:50.000000 py_madvr-1.3.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 15:43:01.518143 py_madvr-1.3.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-14 15:42:50.000000 py_madvr-1.3.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:43:01.514143 py_madvr-1.3.12/madvr/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-14 15:42:50.000000 py_madvr-1.3.12/madvr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-14 15:42:50.000000 py_madvr-1.3.12/madvr/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-14 15:42:50.000000 py_madvr-1.3.12/madvr/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14948 2023-05-14 15:42:50.000000 py_madvr-1.3.12/madvr/madvr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:43:01.514143 py_madvr-1.3.12/py_madvr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 15:43:01.000000 py_madvr-1.3.12/py_madvr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-14 15:43:01.000000 py_madvr-1.3.12/py_madvr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 15:43:01.000000 py_madvr-1.3.12/py_madvr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 15:43:01.000000 py_madvr-1.3.12/py_madvr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 15:43:01.518143 py_madvr-1.3.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-14 15:42:50.000000 py_madvr-1.3.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:43:01.518143 py_madvr-1.3.12/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:42:50.000000 py_madvr-1.3.12/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-14 15:42:50.000000 py_madvr-1.3.12/tests/testMadVR.py
```

### Comparing `py_madvr-1.3.11/LICENSE` & `py_madvr-1.3.12/LICENSE`

 * *Files identical despite different names*

### Comparing `py_madvr-1.3.11/PKG-INFO` & `py_madvr-1.3.12/py_madvr.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py_madvr
-Version: 1.3.11
+Name: py-madvr
+Version: 1.3.12
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.3.11/madvr/commands.py` & `py_madvr-1.3.12/madvr/commands.py`

 * *Files identical despite different names*

### Comparing `py_madvr-1.3.11/madvr/madvr.py` & `py_madvr-1.3.12/madvr/madvr.py`

 * *Files 2% similar despite different names*

```diff
@@ -295,38 +295,46 @@
 
         return ""
 
     async def read_notifications(self) -> None:
         """
         Read notifications from the server and update attributes
         """
-        # read notifications
-        try:
-            async with self.reader_lock:
-                msg = await asyncio.wait_for(
-                    self.reader.read(self.read_limit),
-                    timeout=self.command_read_timeout,
-                )
-
-        except asyncio.TimeoutError:
-            self.logger.warning("Reading notifications timed out")
-            return
-
-        except OSError:
-            self.logger.warning("Reading notifications failed")
-            return
-
-        # if the msg is empty, then the connection is closed
-        if not msg:
-            # self.logger.warning("Connection closed")
-            # await self.close_connection()
-            return
+        while True:
+            # read notifications
+            try:
+                async with self.reader_lock:
+                    msg = await asyncio.wait_for(
+                        self.reader.read(self.read_limit),
+                        timeout=self.command_read_timeout,
+                    )
+            except AttributeError:
+                self.logger.warning("not connected")
+                asyncio.sleep(2)
+                continue
+
+            except asyncio.TimeoutError:
+                self.logger.warning("Reading notifications timed out")
+                await asyncio.sleep(1)
+                continue
+
+            except OSError:
+                self.logger.warning("Reading notifications failed")
+                await asyncio.sleep(1)
+                continue
+
+            # if the msg is empty, then the connection could be closed
+            if not msg:
+                # self.logger.warning("Connection closed")
+                # await self.close_connection()
+                await asyncio.sleep(1)
+                continue
 
-        # if the msg is not empty, process it
-        await self._process_notifications(msg.decode("utf-8"))
+            # if the msg is not empty, process it
+            await self._process_notifications(msg.decode("utf-8"))
 
     async def _process_notifications(self, msg: str) -> None:
         """Parse a message and store the attributes and values in a dictionary"""
         self.logger.debug("Processing notifications: %s", msg)
         notifications = msg.split("\r\n")
         # for each /r/n split it by title, then the rest are values
         for notification in notifications:
```

### Comparing `py_madvr-1.3.11/py_madvr.egg-info/PKG-INFO` & `py_madvr-1.3.12/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py-madvr
-Version: 1.3.11
+Name: py_madvr
+Version: 1.3.12
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.3.11/setup.py` & `py_madvr-1.3.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_madvr",
-    version="1.3.11",
+    version="1.3.12",
     author="iloveicedgreentea",
     description="A package to control MadVR Envy over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/py-madvr",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `py_madvr-1.3.11/tests/testMadVR.py` & `py_madvr-1.3.12/tests/testMadVR.py`

 * *Files identical despite different names*

