# Comparing `tmp/homeduino-0.0.6.tar.gz` & `tmp/homeduino-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homeduino-0.0.6.tar", last modified: Fri May 12 15:02:50 2023, max compression
+gzip compressed data, was "homeduino-0.0.7.tar", last modified: Sun May 14 11:35:23 2023, max compression
```

## Comparing `homeduino-0.0.6.tar` & `homeduino-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:02:50.867834 homeduino-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-05-12 15:02:35.000000 homeduino-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-12 15:02:50.867834 homeduino-0.0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:02:50.863834 homeduino-0.0.6/homeduino/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-12 15:02:35.000000 homeduino-0.0.6/homeduino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-12 15:02:35.000000 homeduino-0.0.6/homeduino/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-05-12 15:02:35.000000 homeduino-0.0.6/homeduino/homeduino.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:02:50.867834 homeduino-0.0.6/homeduino.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-12 15:02:50.000000 homeduino-0.0.6/homeduino.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-12 15:02:50.000000 homeduino-0.0.6/homeduino.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 15:02:50.000000 homeduino-0.0.6/homeduino.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-12 15:02:50.000000 homeduino-0.0.6/homeduino.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-12 15:02:50.000000 homeduino-0.0.6/homeduino.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-12 15:02:35.000000 homeduino-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 15:02:50.867834 homeduino-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:35:23.680281 homeduino-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-05-14 11:35:07.000000 homeduino-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-14 11:35:23.680281 homeduino-0.0.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:35:23.676281 homeduino-0.0.7/homeduino/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-14 11:35:07.000000 homeduino-0.0.7/homeduino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-14 11:35:07.000000 homeduino-0.0.7/homeduino/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11651 2023-05-14 11:35:07.000000 homeduino-0.0.7/homeduino/homeduino.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:35:23.680281 homeduino-0.0.7/homeduino.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-14 11:35:23.000000 homeduino-0.0.7/homeduino.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-14 11:35:23.000000 homeduino-0.0.7/homeduino.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 11:35:23.000000 homeduino-0.0.7/homeduino.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-14 11:35:23.000000 homeduino-0.0.7/homeduino.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-14 11:35:23.000000 homeduino-0.0.7/homeduino.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-14 11:35:07.000000 homeduino-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 11:35:23.680281 homeduino-0.0.7/setup.cfg
```

### Comparing `homeduino-0.0.6/LICENSE` & `homeduino-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `homeduino-0.0.6/PKG-INFO` & `homeduino-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeduino
-Version: 0.0.6
+Version: 0.0.7
 Summary: Homeduino library
 Author: Rogier van Staveren
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rrooggiieerr/homeduino.py
 Project-URL: Bug Tracker, https://github.com/rrooggiieerr/homeduino.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `homeduino-0.0.6/homeduino/__main__.py` & `homeduino-0.0.7/homeduino/__main__.py`

 * *Files identical despite different names*

### Comparing `homeduino-0.0.6/homeduino/homeduino.py` & `homeduino-0.0.7/homeduino/homeduino.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 import asyncio
 import logging
 import os
+import re
 import sys
 import time
 from asyncio.transports import BaseTransport
 from collections import deque
 from datetime import datetime
 from functools import partial
-from typing import Any, Optional
+from typing import Any, Final, Optional
 
 import serial_asyncio
 from rfcontrol import controller
 from serial.serialutil import SerialException
 from serial_asyncio import SerialTransport
 
 logger = logging.getLogger(__name__)
 
+DEFAULT_BAUD_RATE: Final = 115200
+BAUD_RATES: Final = [57600, DEFAULT_BAUD_RATE]
+DEFAULT_RECEIVE_PIN: Final = 2
+DEFAULT_SEND_PIN: Final = 4
+
 _RESPONSE_TIMEOUT = 1
+_READY_TIMEOUT = 5
 _BUSY_TIMEOUT = 1
 
 
 class HomeduinoError(Exception):
     """Generic Homeduino error."""
 
 
@@ -98,14 +105,16 @@
                     self.handle_ready()
                 elif line.startswith("RF receive "):
                     self.handle_rf_receive(line)
                 elif line.startswith("KP "):
                     self.handle_key_press(line)
                 elif line != "" and self._tx_busy:
                     self.str_buffer.append(line)
+                elif line != "":
+                    logger.error("Unhandled data received '%s'", line)
 
     def handle_ready(self) -> None:
         self.ready = True
         logger.info("Homeduino is connected")
 
     def handle_rf_receive(self, line: str) -> None:
         logger.debug(line)
@@ -193,25 +202,26 @@
 class Homeduino:
     protocol: HomeduinoProtocol = None
     rf_receive_callbacks = []
 
     def __init__(
         self,
         serial_port: str,
-        receive_pin: int,
-        send_pin: int,
+        baud_rate: int = DEFAULT_BAUD_RATE,
+        receive_pin: int = DEFAULT_RECEIVE_PIN,
+        send_pin: int = DEFAULT_SEND_PIN,
         dht_pin: int = None,
         loop=None,
     ):
         # Test if the device exists
         if not os.path.exists(serial_port):
             logger.warning("No such file or directory: '%s'", serial_port)
 
         self.serial_port = serial_port
-        # self.receive_pin = receive_pin
+        self.baud_rate = baud_rate
         self.receive_interrupt = receive_pin - 2
         self.send_pin = send_pin
         self.dht_pin = dht_pin
 
         if loop is None:
             loop = asyncio.get_event_loop()
         self.loop = loop
@@ -224,45 +234,65 @@
                 (
                     _transport,
                     self.protocol,
                 ) = await serial_asyncio.create_serial_connection(
                     self.loop,
                     protocol_factory,
                     self.serial_port,
-                    baudrate=115200,
+                    baudrate=self.baud_rate,
                     bytesize=serial_asyncio.serial.EIGHTBITS,
                     parity=serial_asyncio.serial.PARITY_NONE,
                     stopbits=serial_asyncio.serial.STOPBITS_ONE,
                 )
 
-                while not self.protocol.ready:
-                    await asyncio.sleep(0.1)
+                start_time = datetime.now()
+                while (datetime.now() - start_time).total_seconds() < _READY_TIMEOUT:
+                    if self.protocol.ready:
+                        await self.protocol.set_receive_interrupt(
+                            self.receive_interrupt
+                        )
 
-                await self.protocol.set_receive_interrupt(self.receive_interrupt)
+                        for rf_receive_callback in self.rf_receive_callbacks:
+                            self.protocol.add_rf_receive_callback(rf_receive_callback)
 
-                for rf_receive_callback in self.rf_receive_callbacks:
-                    self.protocol.add_rf_receive_callback(rf_receive_callback)
+                        return True
+
+                    logger.debug("Waiting for Homeduino to become ready")
+                    await asyncio.sleep(0.1)
 
-                return True
+                logger.error("Timeout while waiting for Homeduino to become ready")
+                raise ResponseTimeoutError(
+                    "Timeout while waiting for Homeduino to become ready"
+                )
             except SerialException as ex:
                 logger.error(ex)
 
         return False
 
     def connected(self) -> bool:
         if self.protocol is None or self.protocol.transport is None:
             return False
 
         return True
 
-    def disconnect(self) -> None:
+    async def disconnect(self) -> bool:
         if self.connected():
             logger.debug("Disconnecting Homeduino")
             self.protocol.transport.close()
-            self.protocol = None
+
+            start_time = datetime.now()
+            while (datetime.now() - start_time).total_seconds() < _READY_TIMEOUT:
+                if not self.protocol.ready:
+                    self.protocol = None
+                    return True
+
+                logger.debug("Waiting for Homeduino to disconnect")
+                await asyncio.sleep(0.1)
+
+        return False
 
     async def ping(self) -> bool:
         if not self.connected():
             raise DisconnectedError("Homeduino is not connected")
 
         logger.debug("Pinging Homeduino")
         message = f"PING {time.time()}"
@@ -305,7 +335,21 @@
         return False
 
     async def send(self, command) -> str:
         if not self.connected():
             raise DisconnectedError("Homeduino is not connected")
 
         return await self.protocol.send(command)
+
+    @staticmethod
+    def get_protocols() -> []:
+        def convert(text):
+            return int(text) if text.isdigit() else text.lower()
+
+        def alphanum_key(key: str):
+            return [convert(c) for c in re.split("([0-9]+)", key)]
+
+        def natural_sort(li):
+            return sorted(li, key=alphanum_key)
+
+        protocol_names = [protocol.name for protocol in controller.get_all_protocols()]
+        return natural_sort(protocol_names)
```

### Comparing `homeduino-0.0.6/homeduino.egg-info/PKG-INFO` & `homeduino-0.0.7/homeduino.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeduino
-Version: 0.0.6
+Version: 0.0.7
 Summary: Homeduino library
 Author: Rogier van Staveren
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rrooggiieerr/homeduino.py
 Project-URL: Bug Tracker, https://github.com/rrooggiieerr/homeduino.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `homeduino-0.0.6/pyproject.toml` & `homeduino-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "homeduino"
-version = "0.0.6"
+version = "0.0.7"
 license = {text = "Apache-2.0"}
 authors = [
     { name="Rogier van Staveren" }
 ]
 description = "Homeduino library"
 readme = "README.md"
 requires-python = ">=3.7"
```

