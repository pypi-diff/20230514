# Comparing `tmp/py_madvr-1.3.15.tar.gz` & `tmp/py_madvr-1.3.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_madvr-1.3.15.tar", last modified: Sun May 14 17:04:56 2023, max compression
+gzip compressed data, was "py_madvr-1.3.16.tar", last modified: Sun May 14 17:54:46 2023, max compression
```

## Comparing `py_madvr-1.3.15.tar` & `py_madvr-1.3.16.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:04:56.359473 py_madvr-1.3.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-14 17:04:37.000000 py_madvr-1.3.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 17:04:56.355472 py_madvr-1.3.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-14 17:04:37.000000 py_madvr-1.3.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:04:56.355472 py_madvr-1.3.15/madvr/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-14 17:04:37.000000 py_madvr-1.3.15/madvr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-14 17:04:37.000000 py_madvr-1.3.15/madvr/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-14 17:04:37.000000 py_madvr-1.3.15/madvr/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15035 2023-05-14 17:04:37.000000 py_madvr-1.3.15/madvr/madvr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:04:56.355472 py_madvr-1.3.15/py_madvr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 17:04:56.000000 py_madvr-1.3.15/py_madvr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-14 17:04:56.000000 py_madvr-1.3.15/py_madvr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 17:04:56.000000 py_madvr-1.3.15/py_madvr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 17:04:56.000000 py_madvr-1.3.15/py_madvr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 17:04:56.359473 py_madvr-1.3.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-14 17:04:37.000000 py_madvr-1.3.15/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:04:56.355472 py_madvr-1.3.15/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:04:37.000000 py_madvr-1.3.15/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-14 17:04:37.000000 py_madvr-1.3.15/tests/testMadVR.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:54:46.448202 py_madvr-1.3.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-14 17:54:34.000000 py_madvr-1.3.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 17:54:46.448202 py_madvr-1.3.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-14 17:54:34.000000 py_madvr-1.3.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:54:46.448202 py_madvr-1.3.16/madvr/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-14 17:54:34.000000 py_madvr-1.3.16/madvr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-14 17:54:34.000000 py_madvr-1.3.16/madvr/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-14 17:54:34.000000 py_madvr-1.3.16/madvr/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15044 2023-05-14 17:54:34.000000 py_madvr-1.3.16/madvr/madvr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:54:46.448202 py_madvr-1.3.16/py_madvr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 17:54:46.000000 py_madvr-1.3.16/py_madvr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-14 17:54:46.000000 py_madvr-1.3.16/py_madvr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 17:54:46.000000 py_madvr-1.3.16/py_madvr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 17:54:46.000000 py_madvr-1.3.16/py_madvr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 17:54:46.448202 py_madvr-1.3.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-14 17:54:34.000000 py_madvr-1.3.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:54:46.448202 py_madvr-1.3.16/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:54:34.000000 py_madvr-1.3.16/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-14 17:54:34.000000 py_madvr-1.3.16/tests/testMadVR.py
```

### Comparing `py_madvr-1.3.15/LICENSE` & `py_madvr-1.3.16/LICENSE`

 * *Files identical despite different names*

### Comparing `py_madvr-1.3.15/PKG-INFO` & `py_madvr-1.3.16/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_madvr
-Version: 1.3.15
+Version: 1.3.16
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.3.15/madvr/commands.py` & `py_madvr-1.3.16/madvr/commands.py`

 * *Files identical despite different names*

### Comparing `py_madvr-1.3.15/madvr/madvr.py` & `py_madvr-1.3.16/madvr/madvr.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
         async with self.writer_lock:
             self.writer.write(self.HEARTBEAT)
             await self.writer.drain()
 
         self.logger.debug("Handshakes complete")
 
     async def _construct_command(
-        self, raw_command: Union[str, list]
+        self, raw_command: list[str]
     ) -> tuple[bytes, str]:
         """
         Transform commands into their byte values from the string value
 
         Raises NotImplementedError
 
         Return:
@@ -192,28 +192,28 @@
             "raw_command: %s -- raw_command length: %s", raw_command, len(raw_command)
         )
 
         skip_val = False
         # HA seems to always send commands as a list even if you set them as a str
 
         # This lets you use single cmds or something with val like KEYPRESS
-        # If len is 1, then try to split, otherwise its just one word
+        # If len is 1 like ["keypress,val"], then try to split, otherwise its just one word
 
         if len(raw_command) == 1:
             try:
                 # ['key_press, menu']
                 command, raw_value = raw_command[0].split(",")
                 # remove space
                 value = raw_value.strip()
                 self.logger.debug("using command %s and value %s", command, value)
             # if valuerror it means theres just one command like PowerOff, so use that directly
             except ValueError as err:
                 self.logger.debug(err)
                 self.logger.debug("Using raw_command directly")
-                command = raw_command
+                command = raw_command[0]
                 skip_val = True
         # if there are more than two values, this is incorrect, error
         elif len(raw_command) > 2:
             self.logger.error(
                 "More than two command values provided. Envy does not have more than 2 command values e.g KeyPress MENU"
             )
             raise NotImplementedError(f"Too many values provided {raw_command}")
@@ -244,20 +244,20 @@
         else:
             cmd: bytes = command_name + Footer.footer.value
 
         self.logger.debug("constructed command: %s", cmd)
 
         return cmd, val
 
-    async def send_command(self, command: Union[str, list]) -> str:
+    async def send_command(self, command: list) -> str:
         """
         send a given command same as the official madvr ones
         To keep this simple, just send the command without reading response
 
-        command: str - command to send like KeyPress, MENU
+        command: list - command to send like [KeyPress, MENU]
         Raises RetryExceededError
         """
 
         # Verify the command is supported
         try:
             cmd, enum_type = await self._construct_command(command)
         except NotImplementedError:
```

### Comparing `py_madvr-1.3.15/setup.py` & `py_madvr-1.3.16/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_madvr",
-    version="1.3.15",
+    version="1.3.16",
     author="iloveicedgreentea",
     description="A package to control MadVR Envy over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/py-madvr",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `py_madvr-1.3.15/tests/testMadVR.py` & `py_madvr-1.3.16/tests/testMadVR.py`

 * *Files identical despite different names*

