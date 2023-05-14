# Comparing `tmp/async_websocket_client-0.0.0a5.tar.gz` & `tmp/async_websocket_client-0.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_websocket_client-0.0.0a5.tar", max compression
+gzip compressed data, was "async_websocket_client-0.0.0a6.tar", max compression
```

## Comparing `async_websocket_client-0.0.0a5.tar` & `async_websocket_client-0.0.0a6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1056 2023-05-08 05:59:55.233187 async_websocket_client-0.0.0a5/LICENSE
--rw-r--r--   0        0        0        0 2023-05-08 05:59:55.337187 async_websocket_client-0.0.0a5/async_websocket_client/__init__.py
--rw-r--r--   0        0        0     2860 2023-05-08 05:59:55.233187 async_websocket_client-0.0.0a5/async_websocket_client/apps.py
--rw-r--r--   0        0        0     1258 2023-05-08 05:59:55.233187 async_websocket_client-0.0.0a5/async_websocket_client/dispatchers.py
--rw-r--r--   0        0        0     1822 2023-05-08 05:59:55.233187 async_websocket_client-0.0.0a5/pyproject.toml
--rw-r--r--   0        0        0     1706 2023-05-08 05:59:55.233187 async_websocket_client-0.0.0a5/readme.md
--rw-r--r--   0        0        0     2279 1970-01-01 00:00:00.000000 async_websocket_client-0.0.0a5/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-05-08 05:59:55.233187 async_websocket_client-0.0.0a6/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-14 19:46:39.511004 async_websocket_client-0.0.0a6/async_websocket_client/__init__.py
+-rw-r--r--   0        0        0     2624 2023-05-10 13:08:56.327036 async_websocket_client-0.0.0a6/async_websocket_client/apps.py
+-rw-r--r--   0        0        0      924 2023-05-11 06:20:55.592215 async_websocket_client-0.0.0a6/async_websocket_client/dispatchers.py
+-rw-r--r--   0        0        0     1822 2023-05-08 05:59:55.233187 async_websocket_client-0.0.0a6/pyproject.toml
+-rw-r--r--   0        0        0     1706 2023-05-08 05:59:55.233187 async_websocket_client-0.0.0a6/readme.md
+-rw-r--r--   0        0        0     2279 1970-01-01 00:00:00.000000 async_websocket_client-0.0.0a6/PKG-INFO
```

### Comparing `async_websocket_client-0.0.0a5/LICENSE` & `async_websocket_client-0.0.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `async_websocket_client-0.0.0a5/async_websocket_client/apps.py` & `async_websocket_client-0.0.0a6/async_websocket_client/apps.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import asyncio
 import logging
 from typing import Any, Coroutine
 
 import websockets
 from websockets.client import WebSocketClientProtocol
+from websockets.exceptions import ConnectionClosedError
 
 from async_websocket_client.dispatchers import BaseDispatcher
 
 # from sdk.client import BaseDispatcher
 
 
 logger = logging.getLogger('async_websocket_client')
@@ -41,46 +42,34 @@
         await self.dispatcher.before_disconnect()
         await self.ws.close()
         await self.dispatcher.on_disconnect()
 
     async def send(self, message: str) -> Any:
         return asyncio.create_task(self.ws.send(message))
 
-    async def ws_recv_message(self) -> str | None:
-        try:
-            return await asyncio.wait_for(self.ws.recv(), 1)
-
-        except asyncio.TimeoutError:
-            return None
-
-    async def ws_ping_loop(self):
-        while self.is_running:
-            ping = await self.ws.ping()
-            await asyncio.sleep(1)
-
-            logger.error([ping, type(ping), ping.result()])
-
     async def ws_recv_loop(self):
         while self.is_running:
-            message = await self.ws_recv_message()
-
+            message = await self.ws.recv()
             if message is None:
                 continue
 
             await self.dispatcher.on_message(message)
 
     async def run(self):
         await self.connect()
 
         try:
             await self.ws_recv_loop()
 
         except asyncio.exceptions.CancelledError as ex:
             logger.error([type(ex), ex])
 
+        except ConnectionClosedError as e:
+            logger.error(f'Connection closed with error: {e}')
+
         self.is_running = False
 
         await self.disconnect()
 
     def asyncio_run(self):
         try:
             asyncio.run(self.run())
```

### Comparing `async_websocket_client-0.0.0a5/async_websocket_client/dispatchers.py` & `async_websocket_client-0.0.0a6/async_websocket_client/dispatchers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from __future__ import annotations
 
 import logging
-import random
+from abc import ABC
 from typing import Any
 
 from websockets.client import WebSocketClientProtocol
 
-# from sdk.client import BaseDispatcher
-
-
 logger = logging.getLogger('async_websocket_client')
 
 
-class BaseDispatcher(object):
+class BaseDispatcher(ABC):
+    """Базовый класс диспетчера"""
 
     app: Any
     ws: WebSocketClientProtocol
 
     def set_app(self, app: Any):
         self.app = app
 
@@ -24,31 +22,17 @@
         self.ws = ws
         self.tasks = getattr(self, 'tasks', [])
 
     async def before_connect(self):
         logger.info('before_connect')
 
     async def on_connect(self):
-        logger.error('on_connect')
-        await self.ws.send('bot on_connect')
+        logger.info('on_connect')
 
     async def before_disconnect(self):
         logger.info('before_disconnect')
 
     async def on_disconnect(self):
         logger.info('on_disconnect')
 
     async def on_message(self, message: str):
-        logger.error(f'client | on_message: {message}')
-
-        if message == 'ping':
-            await self.ws.send('pong')
-            return
-
-        try:
-            await self.ws.send(str(int(message) + 1))
-
-        except Exception:
-            await self.ws.send('-1111111')
-
-    async def make_message(self):
-        return str(random.randint(1, 100))
+        logger.info(f'client | on_message: {message}')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `async_websocket_client-0.0.0a5/pyproject.toml` & `async_websocket_client-0.0.0a6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `async_websocket_client-0.0.0a5/readme.md` & `async_websocket_client-0.0.0a6/readme.md`

 * *Files identical despite different names*

### Comparing `async_websocket_client-0.0.0a5/PKG-INFO` & `async_websocket_client-0.0.0a6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-websocket-client
-Version: 0.0.0a5
+Version: 0.0.0a6
 Summary: 
 Author: irocshers
 Author-email: develop.iam@rocshers.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

