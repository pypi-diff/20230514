# Comparing `tmp/py_madvr-1.3.16.tar.gz` & `tmp/py_madvr-1.3.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_madvr-1.3.16.tar", last modified: Sun May 14 17:54:46 2023, max compression
+gzip compressed data, was "py_madvr-1.3.17.tar", last modified: Sun May 14 18:17:49 2023, max compression
```

## Comparing `py_madvr-1.3.16.tar` & `py_madvr-1.3.17.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:54:46.448202 py_madvr-1.3.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-14 17:54:34.000000 py_madvr-1.3.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 17:54:46.448202 py_madvr-1.3.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-14 17:54:34.000000 py_madvr-1.3.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:54:46.448202 py_madvr-1.3.16/madvr/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-14 17:54:34.000000 py_madvr-1.3.16/madvr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-14 17:54:34.000000 py_madvr-1.3.16/madvr/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-14 17:54:34.000000 py_madvr-1.3.16/madvr/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15044 2023-05-14 17:54:34.000000 py_madvr-1.3.16/madvr/madvr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:54:46.448202 py_madvr-1.3.16/py_madvr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 17:54:46.000000 py_madvr-1.3.16/py_madvr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-14 17:54:46.000000 py_madvr-1.3.16/py_madvr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 17:54:46.000000 py_madvr-1.3.16/py_madvr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 17:54:46.000000 py_madvr-1.3.16/py_madvr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 17:54:46.448202 py_madvr-1.3.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-14 17:54:34.000000 py_madvr-1.3.16/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:54:46.448202 py_madvr-1.3.16/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:54:34.000000 py_madvr-1.3.16/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-14 17:54:34.000000 py_madvr-1.3.16/tests/testMadVR.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:17:49.334386 py_madvr-1.3.17/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-14 18:17:35.000000 py_madvr-1.3.17/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 18:17:49.334386 py_madvr-1.3.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-14 18:17:35.000000 py_madvr-1.3.17/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:17:49.330386 py_madvr-1.3.17/madvr/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-14 18:17:35.000000 py_madvr-1.3.17/madvr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-14 18:17:35.000000 py_madvr-1.3.17/madvr/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-14 18:17:35.000000 py_madvr-1.3.17/madvr/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-05-14 18:17:35.000000 py_madvr-1.3.17/madvr/madvr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:17:49.334386 py_madvr-1.3.17/py_madvr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 18:17:49.000000 py_madvr-1.3.17/py_madvr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-14 18:17:49.000000 py_madvr-1.3.17/py_madvr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 18:17:49.000000 py_madvr-1.3.17/py_madvr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 18:17:49.000000 py_madvr-1.3.17/py_madvr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 18:17:49.334386 py_madvr-1.3.17/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-14 18:17:35.000000 py_madvr-1.3.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:17:49.334386 py_madvr-1.3.17/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 18:17:35.000000 py_madvr-1.3.17/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-14 18:17:35.000000 py_madvr-1.3.17/tests/testMadVR.py
```

### Comparing `py_madvr-1.3.16/LICENSE` & `py_madvr-1.3.17/LICENSE`

 * *Files identical despite different names*

### Comparing `py_madvr-1.3.16/PKG-INFO` & `py_madvr-1.3.17/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_madvr
-Version: 1.3.16
+Version: 1.3.17
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.3.16/madvr/commands.py` & `py_madvr-1.3.17/madvr/commands.py`

 * *Files identical despite different names*

### Comparing `py_madvr-1.3.16/madvr/madvr.py` & `py_madvr-1.3.17/madvr/madvr.py`

 * *Files 6% similar despite different names*

```diff
@@ -122,15 +122,15 @@
                     )
 
                 self.logger.info("Waiting for envy to be available")
                 # envy needs some time to setup new connections
                 await asyncio.sleep(3)
 
                 # handshake func
-                await self._send_heartbeat()
+                await self.send_heartbeat()
 
                 self.logger.info("Connection established")
 
                 self.is_on = True
                 self.is_closed = False
 
                 self.connection_event.set()
@@ -155,30 +155,40 @@
             # backoff to not spam HA
             except OSError as err:
                 self.logger.warning("Connecting failed, retrying in %s seconds", 2)
                 self.logger.debug(err)
                 await asyncio.sleep(2)
                 continue
 
-    async def _send_heartbeat(self) -> None:
+    async def send_heartbeat(self) -> None:
         """
         Send a heartbeat to keep connection open
 
         You should wrap this in try with OSError and asyncio.TimeoutError exceptions
 
         Raises HeartBeatError exception
         """
-        # confirm can send heartbeat, ready for commands
-        self.logger.debug("Sending heartbeats")
-
-        async with self.writer_lock:
-            self.writer.write(self.HEARTBEAT)
-            await self.writer.drain()
+        while True:
+            await self.connection_event.wait()
+            # confirm can send heartbeat, ready for commands
+            self.logger.debug("Sending heartbeats")
+            try:
+                async with self.writer_lock:
+                    self.writer.write(self.HEARTBEAT)
+                    await self.writer.drain()
 
-        self.logger.debug("Handshakes complete")
+                self.logger.debug("heartbeat complete")
+            except asyncio.TimeoutError:
+                self.logger.error("timeout when sending heartbeat")
+            except OSError:
+                self.logger.error("error when sending heartbeat")
+                await self._reconnect()
+            finally:
+                # Wait some time before the next heartbeat
+                await asyncio.sleep(15)
 
     async def _construct_command(
         self, raw_command: list[str]
     ) -> tuple[bytes, str]:
         """
         Transform commands into their byte values from the string value
 
@@ -218,20 +228,20 @@
             )
             raise NotImplementedError(f"Too many values provided {raw_command}")
         else:
             # else a command was provided as a proper list ['keypress', 'menu']
             # raw command will be a list of 2
             command, value = raw_command
 
-        self.logger.debug("using command %s", command)
+        self.logger.debug("checking command %s", command)
 
         # Check if command is implemented
         if not hasattr(Commands, command):
             raise NotImplementedError(f"Command not implemented: {command}")
-
+        self.logger.debug("Found command")
         # construct the command with nested Enums
         command_name, val, _ = Commands[command].value
 
         # if there is a value to process
         if not skip_val:
             try:
                 command_base: bytes = command_name + b" " + val[value.lstrip(" ")].value
@@ -256,15 +266,16 @@
         command: list - command to send like [KeyPress, MENU]
         Raises RetryExceededError
         """
 
         # Verify the command is supported
         try:
             cmd, enum_type = await self._construct_command(command)
-        except NotImplementedError:
+        except NotImplementedError as err:
+            self.logger.error("command not implemented: %s -- %s", command, err)
             return f"Command not found: {command}"
 
         self.logger.debug("using values: %s %s", cmd, enum_type)
 
         # reconnect if client is not init or its off
         if self.reader is None or self.is_on is False:
             # Don't reconnect if poweroff or standby because HA will complain
```

### Comparing `py_madvr-1.3.16/py_madvr.egg-info/PKG-INFO` & `py_madvr-1.3.17/py_madvr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-madvr
-Version: 1.3.16
+Version: 1.3.17
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.3.16/setup.py` & `py_madvr-1.3.17/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_madvr",
-    version="1.3.16",
+    version="1.3.17",
     author="iloveicedgreentea",
     description="A package to control MadVR Envy over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/py-madvr",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `py_madvr-1.3.16/tests/testMadVR.py` & `py_madvr-1.3.17/tests/testMadVR.py`

 * *Files identical despite different names*

