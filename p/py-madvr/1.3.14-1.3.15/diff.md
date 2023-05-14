# Comparing `tmp/py_madvr-1.3.14.tar.gz` & `tmp/py_madvr-1.3.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_madvr-1.3.14.tar", last modified: Sun May 14 16:37:22 2023, max compression
+gzip compressed data, was "py_madvr-1.3.15.tar", last modified: Sun May 14 17:04:56 2023, max compression
```

## Comparing `py_madvr-1.3.14.tar` & `py_madvr-1.3.15.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:37:22.255258 py_madvr-1.3.14/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-14 16:37:06.000000 py_madvr-1.3.14/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 16:37:22.255258 py_madvr-1.3.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-14 16:37:06.000000 py_madvr-1.3.14/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:37:22.255258 py_madvr-1.3.14/madvr/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-14 16:37:06.000000 py_madvr-1.3.14/madvr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-14 16:37:06.000000 py_madvr-1.3.14/madvr/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-14 16:37:06.000000 py_madvr-1.3.14/madvr/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    14726 2023-05-14 16:37:06.000000 py_madvr-1.3.14/madvr/madvr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:37:22.255258 py_madvr-1.3.14/py_madvr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 16:37:22.000000 py_madvr-1.3.14/py_madvr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-14 16:37:22.000000 py_madvr-1.3.14/py_madvr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 16:37:22.000000 py_madvr-1.3.14/py_madvr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 16:37:22.000000 py_madvr-1.3.14/py_madvr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 16:37:22.255258 py_madvr-1.3.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-14 16:37:06.000000 py_madvr-1.3.14/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:37:22.255258 py_madvr-1.3.14/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:37:06.000000 py_madvr-1.3.14/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-14 16:37:06.000000 py_madvr-1.3.14/tests/testMadVR.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:04:56.359473 py_madvr-1.3.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-14 17:04:37.000000 py_madvr-1.3.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 17:04:56.355472 py_madvr-1.3.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-14 17:04:37.000000 py_madvr-1.3.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:04:56.355472 py_madvr-1.3.15/madvr/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-14 17:04:37.000000 py_madvr-1.3.15/madvr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-14 17:04:37.000000 py_madvr-1.3.15/madvr/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-14 17:04:37.000000 py_madvr-1.3.15/madvr/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15035 2023-05-14 17:04:37.000000 py_madvr-1.3.15/madvr/madvr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:04:56.355472 py_madvr-1.3.15/py_madvr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 17:04:56.000000 py_madvr-1.3.15/py_madvr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-14 17:04:56.000000 py_madvr-1.3.15/py_madvr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 17:04:56.000000 py_madvr-1.3.15/py_madvr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 17:04:56.000000 py_madvr-1.3.15/py_madvr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 17:04:56.359473 py_madvr-1.3.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-14 17:04:37.000000 py_madvr-1.3.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:04:56.355472 py_madvr-1.3.15/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:04:37.000000 py_madvr-1.3.15/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-14 17:04:37.000000 py_madvr-1.3.15/tests/testMadVR.py
```

### Comparing `py_madvr-1.3.14/LICENSE` & `py_madvr-1.3.15/LICENSE`

 * *Files identical despite different names*

### Comparing `py_madvr-1.3.14/PKG-INFO` & `py_madvr-1.3.15/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_madvr
-Version: 1.3.14
+Version: 1.3.15
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.3.14/madvr/commands.py` & `py_madvr-1.3.15/madvr/commands.py`

 * *Files identical despite different names*

### Comparing `py_madvr-1.3.14/madvr/madvr.py` & `py_madvr-1.3.15/madvr/madvr.py`

 * *Files 2% similar despite different names*

```diff
@@ -305,16 +305,23 @@
             await self.connection_event.wait()
             try:
                 async with self.reader_lock:
                     msg = await asyncio.wait_for(
                         self.reader.read(self.read_limit),
                         timeout=self.command_read_timeout,
                     )
+            except ConnectionResetError:
+                self.logger.warning(
+                    "Connection reset by peer. Attempting to reconnect..."
+                )
+                await self._reconnect()
             except (AttributeError, asyncio.TimeoutError, OSError) as err:
-                self.logger.warning(f"Reading notifications failed or timed out: {err}")
+                self.logger.warning(
+                    "Reading notifications failed or timed out: %s", err
+                )
                 await asyncio.sleep(5)
                 continue
 
             if not msg:
                 await asyncio.sleep(1)
                 continue
 
@@ -328,14 +335,16 @@
         for notification in notifications:
             title, *signal_info = notification.split(" ")
             # dont process empty values
             if not signal_info:
                 continue
             # at least madvr sends attributes in a consistent order
             # could use zip here but why? this works and is simple
+            if "NoSignal" in title:
+                return
             if "IncomingSignalInfo" in title:
                 self.msg_dict["incoming_res"] = signal_info[0]
                 self.msg_dict["incoming_frame_rate"] = signal_info[1]
                 self.msg_dict["incoming_color_space"] = signal_info[3]
                 self.msg_dict["incoming_bit_depth"] = signal_info[4]
                 self.msg_dict["hdr_flag"] = "HDR" in signal_info[5]
                 self.msg_dict["incoming_colorimetry"] = signal_info[6]
```

### Comparing `py_madvr-1.3.14/py_madvr.egg-info/PKG-INFO` & `py_madvr-1.3.15/py_madvr.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-madvr
-Version: 1.3.14
+Version: 1.3.15
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.3.14/setup.py` & `py_madvr-1.3.15/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_madvr",
-    version="1.3.14",
+    version="1.3.15",
     author="iloveicedgreentea",
     description="A package to control MadVR Envy over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/py-madvr",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `py_madvr-1.3.14/tests/testMadVR.py` & `py_madvr-1.3.15/tests/testMadVR.py`

 * *Files identical despite different names*

