# Comparing `tmp/teelebot-2.2.0-py3-none-any.whl.zip` & `tmp/teelebot-2.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,22 @@
-Zip file size: 40299 bytes, number of entries: 18
--rw-rw-rw-  2.0 fat     4126 b- defN 23-May-07 14:53 teelebot/__init__.py
+Zip file size: 40240 bytes, number of entries: 20
+-rw-rw-rw-  2.0 fat     4093 b- defN 23-May-14 02:38 teelebot/__init__.py
 -rw-rw-rw-  2.0 fat      165 b- defN 23-May-08 17:02 teelebot/__main__.py
--rw-rw-rw-  2.0 fat    42023 b- defN 23-May-11 15:08 teelebot/bot.py
--rw-rw-rw-  2.0 fat     7835 b- defN 23-May-11 01:50 teelebot/buffer.py
--rw-rw-rw-  2.0 fat    23836 b- defN 23-May-11 15:12 teelebot/handler.py
+-rw-rw-rw-  2.0 fat    32546 b- defN 23-May-14 14:35 teelebot/bot.py
+-rw-rw-rw-  2.0 fat     7128 b- defN 23-May-14 14:32 teelebot/buffer.py
+-rw-rw-rw-  2.0 fat     1556 b- defN 23-May-14 02:12 teelebot/common.py
+-rw-rw-rw-  2.0 fat    23343 b- defN 23-May-14 14:18 teelebot/handler.py
 -rw-rw-rw-  2.0 fat     1807 b- defN 23-May-03 00:00 teelebot/logger.py
--rw-rw-rw-  2.0 fat      721 b- defN 23-May-03 00:01 teelebot/polling.py
--rw-rw-rw-  2.0 fat     3700 b- defN 23-May-07 14:53 teelebot/request.py
--rw-rw-rw-  2.0 fat     4075 b- defN 23-May-09 01:15 teelebot/schedule.py
--rw-rw-rw-  2.0 fat      482 b- defN 23-May-11 02:10 teelebot/version.py
+-rw-rw-rw-  2.0 fat     6391 b- defN 23-May-14 14:33 teelebot/metadata.py
+-rw-rw-rw-  2.0 fat      737 b- defN 23-May-14 14:25 teelebot/polling.py
+-rw-rw-rw-  2.0 fat     3719 b- defN 23-May-14 14:27 teelebot/request.py
+-rw-rw-rw-  2.0 fat     4075 b- defN 23-May-14 14:30 teelebot/schedule.py
+-rw-rw-rw-  2.0 fat      489 b- defN 23-May-14 14:35 teelebot/version.py
 -rw-rw-rw-  2.0 fat     2665 b- defN 23-May-03 15:18 teelebot/webhook.py
--rw-rw-rw-  2.0 fat    35823 b- defN 23-May-11 15:35 teelebot-2.2.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     9624 b- defN 23-May-11 15:35 teelebot-2.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-11 15:35 teelebot-2.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       43 b- defN 23-May-11 15:35 teelebot-2.2.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-11 15:35 teelebot-2.2.0.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-May-11 15:35 teelebot-2.2.0.dist-info/zip-safe
--rw-rw-r--  2.0 fat     1406 b- defN 23-May-11 15:35 teelebot-2.2.0.dist-info/RECORD
-18 files, 138434 bytes uncompressed, 38021 bytes compressed:  72.5%
+-rw-rw-rw-  2.0 fat    35823 b- defN 23-May-14 14:59 teelebot-2.3.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     9630 b- defN 23-May-14 14:59 teelebot-2.3.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-14 14:59 teelebot-2.3.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       43 b- defN 23-May-14 14:59 teelebot-2.3.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-14 14:59 teelebot-2.3.0.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-May-14 14:59 teelebot-2.3.0.dist-info/zip-safe
+-rw-rw-r--  2.0 fat     1558 b- defN 23-May-14 14:59 teelebot-2.3.0.dist-info/RECORD
+20 files, 135871 bytes uncompressed, 37734 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -6,20 +6,26 @@
 
 Filename: teelebot/bot.py
 Comment: 
 
 Filename: teelebot/buffer.py
 Comment: 
 
+Filename: teelebot/common.py
+Comment: 
+
 Filename: teelebot/handler.py
 Comment: 
 
 Filename: teelebot/logger.py
 Comment: 
 
+Filename: teelebot/metadata.py
+Comment: 
+
 Filename: teelebot/polling.py
 Comment: 
 
 Filename: teelebot/request.py
 Comment: 
 
 Filename: teelebot/schedule.py
@@ -27,29 +33,29 @@
 
 Filename: teelebot/version.py
 Comment: 
 
 Filename: teelebot/webhook.py
 Comment: 
 
-Filename: teelebot-2.2.0.dist-info/LICENSE
+Filename: teelebot-2.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: teelebot-2.2.0.dist-info/METADATA
+Filename: teelebot-2.3.0.dist-info/METADATA
 Comment: 
 
-Filename: teelebot-2.2.0.dist-info/WHEEL
+Filename: teelebot-2.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: teelebot-2.2.0.dist-info/entry_points.txt
+Filename: teelebot-2.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: teelebot-2.2.0.dist-info/top_level.txt
+Filename: teelebot-2.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: teelebot-2.2.0.dist-info/zip-safe
+Filename: teelebot-2.3.0.dist-info/zip-safe
 Comment: 
 
-Filename: teelebot-2.2.0.dist-info/RECORD
+Filename: teelebot-2.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## teelebot/__init__.py

```diff
@@ -1,11 +1,11 @@
 # -*- coding:utf-8 -*-
 """
 @creation date: 2019-08-23
-@last modification: 2023-05-06
+@last modification: 2023-05-14
 """
 import os
 import requests
 import urllib3
 
 from .polling import _runUpdates
 from .webhook import _runWebhook
@@ -48,16 +48,15 @@
     pending_update_count = status["pending_update_count"]
     allowed_updates = status.get("allowed_updates", [])
 
     if bot._webhook:
         protocol = "https://"
         if bot._local_api_server != "False":
             protocol = "http://"
-        url = protocol + str(bot._server_address + ":" + str(
-            bot._server_port) + "/bot" + str(bot._key))
+        url = f'{protocol}{str(bot._server_address)}:{str(bot._server_port)}/bot{str(bot._key)}'
         if (bot._drop_pending_updates == True and pending_update_count != 0) \
             or (status["url"] != url) or (status["has_custom_certificate"] != bot._self_signed) \
             or status["max_connections"] != int(bot._pool_size) \
             or allowed_updates != bot._allowed_updates:
             if bot._self_signed:
                 status = bot.setWebhook(
                     url=url,
@@ -104,11 +103,11 @@
             pending_update_count != 0:
             results = bot.getUpdates(
                 offset=bot._offset,
                 limit=100,
                 timeout=bot._timeout,
                 allowed_updates=bot._allowed_updates
             )
-            messages = bot._washUpdates(results)
+            bot._washUpdates(results)
         _runUpdates(bot=bot)
```

## teelebot/bot.py

```diff
@@ -1,40 +1,43 @@
 # -*- coding:utf-8 -*-
 """
-@description:基于Telegram Bot Api 的机器人框架
+@description: A bot framework based on the Telegram Bot API
 @creation date: 2019-08-13
-@last modification: 2023-05-11
+@last modification: 2023-05-14
 @author: Pluto (github:plutobell)
-@version: 2.2.0
+@version: 2.3.0
 """
 import time
 import sys
 import os
 import copy
 import types
 import string
 import random
 import shutil
 import inspect
+import traceback
 import importlib
-import threading
 
 from pathlib import Path
-from typing import Union, Callable, Tuple
+from typing import Union, Callable
 from concurrent.futures import ThreadPoolExecutor
 
 from .handler import _config, _bridge, _plugin_info
 from .logger import _logger
 from .schedule import _Schedule
 from .buffer import _Buffer
 from .request import _Request
+from .metadata import _Metadata
 
 
 class Bot(object):
-    """机器人的基类"""
+    """
+    Bot Class
+    """
 
     def __init__(self, key: str = None, debug: bool = False, proxies: dict = None):
         config = _config()
 
         if key not in [None, "", " "]:
             self._key = key
             self._debug = debug
@@ -49,15 +52,15 @@
 
         self._cloud_api_server = config["cloud_api_server"]
         self._local_api_server = config["local_api_server"]
         if self._local_api_server != "False":
             self._basic_url = config["local_api_server"]
         else:
             self._basic_url = self._cloud_api_server
-        self._url = self._basic_url + r"bot" + self._key + r"/"
+        self._url = f'{self._basic_url}bot{self._key}/'
 
         self._webhook = config["webhook"]
         if self._webhook:
             self._self_signed = config["self_signed"]
             self._cert_key = config["cert_key"]
             self._cert_pub = config["cert_pub"]
             self._server_address = config["server_address"]
@@ -88,18 +91,20 @@
                 "poll_answer",
                 "my_chat_member",
                 "chat_member",
                 "chat_join_request"
             ]
 
         self.__root_id = config["root_id"]
-        self.__bot_id = self._key.split(":")[0]
+        try:
+            self.__bot_id = self._key.split(":")[0]
+        except:
+            self.__bot_id = ""
         self.__common_pkg_prefix = config["common_pkg_prefix"]
         self.__inline_mode_prefix = config["inline_mode_prefix"]
-        self.__metadata_template = config["metadata_template"]
         self.__AUTHOR = config["author"]
         self.__VERSION = config["version"]
         self.__plugin_dir = config["plugin_dir"]
         self.__plugin_bridge = config["plugin_bridge"]
         self.__non_plugin_list = config["non_plugin_list"]
         self.__start_time = int(time.time())
         self.__response_times = 0
@@ -108,136 +113,139 @@
 
         thread_pool_size = round(int(self._pool_size) * 2 / 3)
         schedule_queue_size = int(self._pool_size) - thread_pool_size
         self.request = _Request(thread_pool_size, self._url, self._debug, self.__proxies)
         self.schedule = _Schedule(schedule_queue_size)
         self.buffer = _Buffer(int(self._buffer_size) * 1024 * 1024,
             self.__plugin_bridge.keys(), self.__plugin_dir)
+        self.metadata = _Metadata(self.__plugin_dir)
 
         self.__thread_pool = ThreadPoolExecutor(
             max_workers=thread_pool_size)
         self.__timer_thread_pool = ThreadPoolExecutor(
             max_workers=int(self._pool_size) * 5)
 
         self.__plugin_info = config["plugin_info"]
         self.__non_plugin_info = config["non_plugin_info"]
 
-        self.__method_name = "Unknown"
-        self.__plugin_info_mutex = threading.Lock()
+        self.__method_name = ""
 
         del config
         del thread_pool_size
         del schedule_queue_size
 
     def __del__(self):
         self.__thread_pool.shutdown(wait=True)
         self.__timer_thread_pool.shutdown(wait=True)
         del self.request
         del self.schedule
+        del self.buffer
+        del self.metadata
 
     def __getattr__(self, method_name):
         self.__method_name = method_name
         
         return types.MethodType(self.__method_function, self)
 
     def __method_function(self, *args, **kwargs):
         # command = inspect.stack()[0].function
         if len(args) != 1:
             _logger.error(f"Method '{self.__method_name}' does not accept positional arguments")
+            raise MethodPositionalArgumentError("Method does not accept positional arguments")
 
         return self.request.postEverything(self.__method_name, **kwargs)
 
     def __threadpool_exception(self, fur):
         """
-        线程池异常回调
+        Thread pool exception callback
         """
         if fur.exception() is not None:
             _logger.debug(f"EXCEPTION - {str(fur.result())}")
 
     def __import_module(self, plugin_name):
         """
-        动态导入模块
+        Dynamic import module
         """
-        sys.path.append(self.path_converter(self.__plugin_dir + plugin_name + os.sep))
-        Module = importlib.import_module(plugin_name)  # 模块检测
+        sys.path.append(self.path_converter(f'{self.__plugin_dir}{plugin_name}{os.sep}'))
+        Module = importlib.import_module(plugin_name)  # Module Detection
 
         return Module
 
     def __update_plugin(self, plugin_name, as_plugin=True):
         """
-        热更新插件
+        Hot update plugin
         """
 
         if as_plugin:
             plugin_info = self.__plugin_info
         else:
             plugin_info = self.__non_plugin_info
 
         plugin_uri = self.path_converter(
-            self.__plugin_dir + plugin_name + os.sep + plugin_name + ".py")
+            f'{self.__plugin_dir}{plugin_name}{os.sep}{plugin_name}.py')
         now_mtime = os.stat(plugin_uri).st_mtime
         # print(now_mtime, self.__plugin_info[plugin_name])
-        if now_mtime != plugin_info[plugin_name]:  # 插件热更新
-            if os.path.exists(self.path_converter(self.__plugin_dir + plugin_name + r"/__pycache__")):
-                shutil.rmtree(self.path_converter(self.__plugin_dir + plugin_name + r"/__pycache__"))
+        if now_mtime != plugin_info[plugin_name]:  # Plugin hot update
+            if os.path.exists(self.path_converter(f'{self.__plugin_dir}{plugin_name}{os.sep}__pycache__')):
+                shutil.rmtree(self.path_converter(f'{self.__plugin_dir}{plugin_name}{os.sep}__pycache__'))
             plugin_info[plugin_name] = now_mtime
             Module = self.__import_module(plugin_name)
             importlib.reload(Module)
             _logger.info(f"The plugin {plugin_name} has been updated")
 
     def __load_plugin(self, now_plugin_info, as_plugin=True,
         now_plugin_bridge={}, now_non_plugin_list=[]):
         """
-        动态装载插件
+        Dynamic loading plugin
         """
         if as_plugin:
-            for plugin in list(now_plugin_bridge.keys()): # 动态装载插件
+            for plugin in list(now_plugin_bridge.keys()): # Dynamic Loading Plugin
                 if plugin not in list(self.__plugin_bridge.keys()):
                     _logger.info(f"The plugin {plugin} has been installed")
                     self.__plugin_info[plugin] = now_plugin_info[plugin]
             for plugin in list(self.__plugin_bridge.keys()):
                 if plugin not in list(now_plugin_bridge.keys()):
                     _logger.info(f"The plugin {plugin} has been uninstalled")
                     self.__plugin_info.pop(plugin)
 
-                    if (self.__plugin_dir + plugin) in sys.path:
-                        sys.path.remove(self.__plugin_dir + plugin)
-                    if (self.__plugin_dir + plugin) in sys.modules:
-                        sys.modules.pop(self.__plugin_dir + plugin)
+                    if (f'{self.__plugin_dir}{plugin}') in sys.path:
+                        sys.path.remove(f'{self.__plugin_dir}{plugin}')
+                    if (f'{self.__plugin_dir}{plugin}') in sys.modules:
+                        sys.modules.pop(f'{self.__plugin_dir}{plugin}')
 
             self.__plugin_bridge = now_plugin_bridge
 
-            self.buffer._update(now_plugin_bridge.keys()) # Buffer动态更新
+            self.buffer._update(now_plugin_bridge.keys()) # Dynamic Update Buffer
 
         else:
-            for plugin in list(now_non_plugin_list): # 动态装载非插件包
+            for plugin in list(now_non_plugin_list): # Dynamically loading non-plugin packages
                 if plugin not in list(self.__non_plugin_list):
                     _logger.info(f"The plugin {plugin} has been installed")
                     self.__non_plugin_info[plugin] = now_plugin_info[plugin]
 
-                    if (self.__plugin_dir + plugin) not in sys.path:
-                        sys.path.append(self.__plugin_dir + plugin)
+                    if (f'{self.__plugin_dir}{plugin}') not in sys.path:
+                        sys.path.append(f'{self.__plugin_dir}{plugin}')
 
             for plugin in list(self.__non_plugin_list):
                 if plugin not in list(now_non_plugin_list):
                     _logger.info(f"The plugin {plugin} has been uninstalled")
                     self.__non_plugin_info.pop(plugin)
 
-                    if (self.__plugin_dir + plugin) in sys.path:
-                        sys.path.remove(self.__plugin_dir + plugin)
-                    if (self.__plugin_dir + plugin) in sys.modules:
-                        sys.modules.pop(self.__plugin_dir + plugin)
+                    if (f'{self.__plugin_dir}{plugin}') in sys.path:
+                        sys.path.remove(f'{self.__plugin_dir}{plugin}')
+                    if (f'{self.__plugin_dir}{plugin}') in sys.modules:
+                        sys.modules.pop(f'{self.__plugin_dir}{plugin}')
 
             self.__non_plugin_list = now_non_plugin_list
 
     def __control_plugin(self, plugin_bridge, chat_type, chat_id):
         if chat_type != "private" and "PluginCTL" in plugin_bridge.keys() \
                 and plugin_bridge["PluginCTL"] == "/pluginctl":
-            if os.path.exists(self.path_converter(self.__plugin_dir + "PluginCTL/db/" + str(chat_id) + ".db")):
-                with open(self.path_converter(self.__plugin_dir + "PluginCTL/db/" + str(chat_id) + ".db"), "r") as f:
+            if os.path.exists(self.path_converter(f'{self.__plugin_dir}PluginCTL/db/{str(chat_id)}.db')):
+                with open(self.path_converter(f'{self.__plugin_dir}PluginCTL/db/{str(chat_id)}.db'), "r") as f:
                     plugin_setting = f.read().strip()
                 plugin_list_off = plugin_setting.split(',')
                 plugin_bridge_temp = {}
                 for plugin in list(plugin_bridge.keys()):
                     if plugin not in plugin_list_off:
                         plugin_bridge_temp[plugin] = plugin_bridge[plugin]
                 plugin_bridge = plugin_bridge_temp
@@ -332,15 +340,15 @@
         else:
             message["message_type"] = "unknown"
             message_type = "unknown"
 
         return message_type, message
 
     def __logging_for_pluginRun(self, message, plugin):
-        title = ""  # INFO日志
+        title = ""  # INFO Log
         user_name = ""
 
         if message["chat"]["type"] == "private":
             if "first_name" in message["chat"].keys():
                 title += message["chat"]["first_name"]
             if "last_name" in message["chat"].keys():
                 if "first_name" in message["chat"].keys():
@@ -369,121 +377,136 @@
                 else:
                     user_name += message["from"]["last_name"]
 
         if message["message_type"] == "unknown":
             _logger.info(
                 "From:" + title + "(" + str(message["chat"]["id"]) + ") - " + \
                 "User:" + user_name + "(" + str(from_id) + ") - " + \
-                "Plugin: " + "" + " - " + \
+                "Plugin:" + "" + " - " + \
                 "Type:" + message["message_type"])
         else:
             _logger.info(
                 "From:" + title + "(" + str(message["chat"]["id"]) + ") - " + \
                 "User:" + user_name + "(" + str(from_id) + ") - " + \
-                "Plugin: " + str(plugin) + " - " + \
+                "Plugin:" + str(plugin) + " - " + \
                 "Type:" + message["message_type"])
 
     def __make_token(self, len=64):
         """
-        生成指定长度的token
+        Generate a token of the specified length
         """
         if len > 64:
             return "Specified length is too long."
         else:
-            token = ''.join(random.sample(string.ascii_letters + string.digits + "-_", 64))
+            token = ''.join(random.sample(f'{string.ascii_letters}{string.digits}-_', 64))
             return token
 
     def _pluginRun(self, bot, message):
         """
-        运行插件
+        Run plugin
         """
         if message is None:
             return
 
-        now_plugin_bridge, now_non_plugin_list = _bridge(self.__plugin_dir)
-        now_plugin_info = _plugin_info(now_plugin_bridge.keys(), self.__plugin_dir)
-        now_non_plugin_info = _plugin_info(now_non_plugin_list, self.__plugin_dir)
-
-        if now_plugin_bridge != self.__plugin_bridge: # 动态装载插件
-            self.__load_plugin(now_plugin_info=now_plugin_info, now_plugin_bridge=now_plugin_bridge)
-        if len(now_plugin_info) != len(self.__plugin_info) or \
-            now_plugin_info != self.__plugin_info: # 动态更新插件信息
-            for plugin_name in list(self.__plugin_bridge.keys()):
-                self.__update_plugin(plugin_name) # 热更新插件
-
-        if now_non_plugin_list != self.__non_plugin_list: # 动态装载非插件包
-            self.__load_plugin(now_plugin_info=now_non_plugin_info, as_plugin=False,
-                now_non_plugin_list=now_non_plugin_list)
-        if len(now_non_plugin_info) != len(self.__non_plugin_info) or \
-            now_non_plugin_info != self.__non_plugin_info: # 动态更新非插件包信息
-            for plugin_name in list(self.__non_plugin_list):
-                self.__update_plugin(plugin_name, as_plugin=False) # 热更新非插件包
-
-        if len(self.__plugin_bridge) == 0:
-            os.system("")
-            _logger.warn("\033[1;31mNo plugins installed\033[0m")
-
-        ok, buffer_status = self.buffer.status() # 数据暂存区容量监测
-        if ok and buffer_status["used"] >= buffer_status["size"]:
-            os.system("")
-            _logger.warn("\033[1;31mThe data buffer area is full \033[0m")
-
-        plugin_bridge = self.__control_plugin( # pluginctl控制
-            self.__plugin_bridge, message["chat"]["type"], message["chat"]["id"])
-
-        message_type = ""
-        message_type, message = self.__mark_message_for_pluginRun(message) # 分类标记消息
-
-        if message_type == "unknown":
-            self.__logging_for_pluginRun(message, "unknown")
+        try:
+            now_plugin_bridge, now_non_plugin_list = _bridge(self.__plugin_dir)
+            now_plugin_info = _plugin_info(now_plugin_bridge.keys(), self.__plugin_dir)
+            now_non_plugin_info = _plugin_info(now_non_plugin_list, self.__plugin_dir)
+
+            if now_plugin_bridge != self.__plugin_bridge: # Dynamic Loading Plugin
+                self.__load_plugin(now_plugin_info=now_plugin_info, now_plugin_bridge=now_plugin_bridge)
+            if len(now_plugin_info) != len(self.__plugin_info) or \
+                now_plugin_info != self.__plugin_info: # Dynamically update plugin information
+                for plugin_name in list(self.__plugin_bridge.keys()):
+                    self.__update_plugin(plugin_name) # Hot Update Plugin
+
+            if now_non_plugin_list != self.__non_plugin_list: # Dynamically loading non-plugin packages
+                self.__load_plugin(now_plugin_info=now_non_plugin_info, as_plugin=False,
+                    now_non_plugin_list=now_non_plugin_list)
+            if len(now_non_plugin_info) != len(self.__non_plugin_info) or \
+                now_non_plugin_info != self.__non_plugin_info: # Dynamic update  the information of non-plugin package
+                for plugin_name in list(self.__non_plugin_list):
+                    self.__update_plugin(plugin_name, as_plugin=False) # Hot update non-plugin package
+
+            if len(self.__plugin_bridge) == 0:
+                os.system("")
+                _logger.warn("\033[1;31mNo plugins installed\033[0m")
+
+            ok, buffer_status = self.buffer.status() # Buffer capacity monitoring
+            if ok and buffer_status["used"] >= buffer_status["size"]:
+                os.system("")
+                _logger.warn("\033[1;31mThe data buffer area is full \033[0m")
+
+            plugin_bridge = self.__control_plugin( # pluginctl control
+                self.__plugin_bridge, message["chat"]["type"], message["chat"]["id"])
+
+            message_type = ""
+            message_type, message = self.__mark_message_for_pluginRun(message) # Category tagging messages
+
+            if message_type == "unknown":
+                self.__logging_for_pluginRun(message, "unknown")
+                return
+
+        except Exception as e:
+            _logger.error(f"Run plugin error: {e}")
+            traceback.print_exc()
             return
 
         for plugin, command in plugin_bridge.items():
-            plugin_requires_version = ""
-            plugin_info = self.get_plugin_info(plugin_name=plugin)
-            if plugin_info["status"]:
-                plugin_requires_version = plugin_info.get("metadata", {}).get("data", {}).get("Requires-teelebot", self.version)
-                plugin_requires_version = plugin_requires_version.replace(">", "").replace("<", "").replace("=", "")
-                if plugin_requires_version in [None, "", " "]:
-                    _logger.warn(f"Skip run {plugin} plugin: failed to get the version of the plugin")
+            try:
+                plugin_requires_version = ""
+                ok, data = self.metadata.read(plugin_name=plugin)
+                # plugin_info = self.get_plugin_info(plugin_name=plugin)
+                if ok:
+                    plugin_requires_version = data.get("Requires-teelebot", {})
+                    plugin_requires_version = plugin_requires_version.replace(">", "").replace("<", "").replace("=", "")
+                    if plugin_requires_version in [None, "", " "]:
+                        _logger.warn(f"Skip run {plugin} plugin: failed to get the version of the plugin")
+                        continue
+                else:
+                    _logger.warn(f"Skip run {plugin} plugin: failed to get information about the plugin (error: {data})")
                     continue
-            else:
-                _logger.warn(f"Skip run {plugin} plugin: failed to get information about the plugin (error: {plugin_info['error']})")
-                continue
-            if plugin_requires_version > self.version:
-                _logger.warn(f"Skip run {plugin} plugin: the plugin requires teelebot version >= {plugin_requires_version}")
-                continue
-
-            if message_type == "query":
-                if command in ["", " ", None]:
+                if plugin_requires_version > self.version:
+                    _logger.warn(f"Skip run {plugin} plugin: the plugin requires teelebot version >= {plugin_requires_version}")
                     continue
 
-            if message.get(message_type)[:len(command)] == command:
-                try:
-                    module = self.__import_module(plugin)
-                    pluginFunc = getattr(module, plugin)
-                    fur = self.__thread_pool.submit(pluginFunc, bot, message)
-                    fur.add_done_callback(self.__threadpool_exception)
-                except Exception as e:
-                    _logger.error(f"Run plugin {plugin} error: {str(e)}")
-
-                self.__response_times += 1
-
-                if message["chat"]["type"] != "private" and \
-                message["chat"]["id"] not in self.__response_chats:
-                    self.__response_chats.append(message["chat"]["id"])
-                if message["from"]["id"] not in self.__response_users:
-                    self.__response_users.append(message["from"]["id"])
+                if message_type == "query":
+                    if command in ["", " ", None]:
+                        continue
+
+                if message.get(message_type)[:len(command)] == command:
+                    try:
+                        module = self.__import_module(plugin)
+                        pluginFunc = getattr(module, plugin)
+                        fur = self.__thread_pool.submit(pluginFunc, bot, message)
+                        fur.add_done_callback(self.__threadpool_exception)
+                    except Exception as e:
+                        _logger.error(f"Run {plugin} plugin error: {str(e)}")
+                        traceback.print_exc()
+
+                    self.__response_times += 1
+
+                    if message["chat"]["type"] != "private" and \
+                    message["chat"]["id"] not in self.__response_chats:
+                        self.__response_chats.append(message["chat"]["id"])
+                    if message["from"]["id"] not in self.__response_users:
+                        if not message["from"]["is_bot"]:
+                            self.__response_users.append(message["from"]["id"])
+
+                    self.__logging_for_pluginRun(message, plugin)
 
-                self.__logging_for_pluginRun(message, plugin)
+            except Exception as e:
+                _logger.error(f"Run {plugin} plugin error: {e}")
+                traceback.print_exc()
+                continue
 
     def _washUpdates(self, results):
         """
-        清洗消息队列
-        results应当是一个列表
+        Cleaning the message queue,
+        The results should be a list
         """
         if not results:
             return False
         elif len(results) < 1:
             return None
         update_ids = []
         messages = []
@@ -512,15 +535,15 @@
                 inline_query = result.get(query_or_message)
                 inline_query["message_id"] = result["update_id"]
                 inline_query["chat"] = inline_query.get("from")
                 inline_query["chat"].pop("language_code")
                 inline_query["chat"].pop("is_bot")
                 inline_query["chat"]["type"] = "private"
                 inline_query["text"] = ""
-                inline_query["query"] = self.__inline_mode_prefix + inline_query["query"] # Inline Mode Plugin Prefix
+                inline_query["query"] = f'{self.__inline_mode_prefix}{inline_query["query"]}' # Inline Mode Plugin Prefix
                 messages.append(inline_query)
             elif query_or_message == "callback_query":
                 callback_query = result.get(query_or_message).get("message")
                 callback_query["click_user"] = result.get(query_or_message)[
                     "from"]
                 callback_query["callback_query_id"] = result.get(
                     query_or_message).get("id")
@@ -550,15 +573,15 @@
             return messages
         else:
             return None
     
     # teelebot method
     def message_deletor(self, time_gap: int, chat_id: str, message_id: str) -> str:
         """
-        定时删除一条消息，时间范围：[0, 900],单位秒
+        Timed deletion of a message, time range: [0, 900], in seconds
         """
         if time_gap < 0 or time_gap > 900:
             return "time_gap_error"
         else:
             def message_deletor_func(time_gap, chat_id, message_id):
                 time.sleep(int(time_gap))
                 self.deleteMessage(chat_id=chat_id, message_id=message_id)
@@ -570,15 +593,15 @@
                     message_deletor_func, time_gap, chat_id, message_id)
                 fur.add_done_callback(self.__threadpool_exception)
 
             return "ok"
 
     def timer(self, time_gap: int, func: Callable[..., None], args: tuple) -> str:
         """
-        单次定时器，时间范围：[0, 900],单位秒
+        Single timer, time range: [0, 900], unit seconds
         """
         if time_gap < 0 or time_gap > 900:
             return "time_gap_error"
         elif type(args) is not tuple:
             return "args_must_be_tuple"
         else:
             def timer_func(time_gap, func, args):
@@ -592,285 +615,33 @@
                     timer_func, time_gap, func, args)
                 fur.add_done_callback(self.__threadpool_exception)
 
             return "ok"
 
     def path_converter(self, path: str) -> str:
         """
-        根据操作系统转换URI
+        Convert URI according to operating system
         """
 
         path = str(Path(path))
 
         return path
     
     def join_plugin_path(self, path: str, plugin_name: str = None) -> str:
         """
-        根据提供的路径自动拼接为插件目录的URI
+        Automatically concatenate the provided path into the plugin directory URI
         """
         if plugin_name in [None, "", " "]:
             plugin_name = os.path.splitext(os.path.basename(inspect.stack()[1][1]))[0]
         
         return self.path_converter(f"{self.plugin_dir}{plugin_name}{os.sep}{path}")
-    
-    def get_plugin_info(self, plugin_name: str = None) -> dict:
-        """
-        获取指定插件的信息
-        """
-        if plugin_name in [None, "", " "]:
-            plugin_name = os.path.splitext(os.path.basename(inspect.stack()[1][1]))[0]
-        
-        if plugin_name not in list(self.plugin_bridge.keys()):
-            info  = {
-                "status": False,
-                "error": "PluginNotFound"
-            }
-            return info
-
-        command = ""
-        description = ""
-        buffer_permissions = "Error"
-        with self.__plugin_info_mutex:
-            with open(self.path_converter(f"{self.plugin_dir}{plugin_name}{os.sep}__init__.py"), "r", encoding="utf-8") as init:
-                lines = init.readlines()
-                
-                buffer_permissions_str = "False:False"
-                if len(lines) >= 1:
-                    command = lines[0][1:].strip()
-                if len(lines) >= 2:
-                    description = lines[1][1:].strip()
-                if len(lines) >= 3:
-                    buffer_permissions_str = lines[2][1:].strip()
-
-                bool_true = ["True", "true"]
-                bool_false = ["False", "false"]
-                bool_true_and_false = ["True", "true", "False", "false"]
-                buffer_permissions_list = buffer_permissions_str.split(":", 1)
-                if len(buffer_permissions_list) != 2 and \
-                    buffer_permissions_str not in [None, "", " "]:
-                    info  = {
-                        "status": False,
-                        "error": "BufferPermissionsFormatError"
-                    }
-                    return info
-                if len(buffer_permissions_list) == 2 and \
-                    (buffer_permissions_list[0] not in bool_true_and_false or \
-                    buffer_permissions_list[1] not in bool_true_and_false):
-                    info  = {
-                        "status": False,
-                        "error": "BufferPermissionsFormatError"
-                    }
-                    return info
-
-                if buffer_permissions_str in [None, "", " "]:
-                    buffer_permissions = tuple((False, False))
-                elif len(buffer_permissions_list) == 2:
-                    read = buffer_permissions_list[0]
-                    write = buffer_permissions_list[1]
-
-                    if read in bool_true:
-                        read = True
-                    elif read in bool_false:
-                        read = False
-                    else:
-                        read = False
-                    
-                    if write in bool_true:
-                        write = True
-                    elif write in bool_false:
-                        write = False
-                    else:
-                        read = False
-
-                    buffer_permissions = tuple((read, write))
-        
-        metadata = {}
-        with self.__plugin_info_mutex:
-            with open(self.path_converter(f"{self.plugin_dir}{plugin_name}{os.sep}METADATA"), "r", encoding="utf-8") as meta:
-                lines = meta.readlines()
-                metadata_data = {}
-                for line in lines:
-                    line = line.strip("\n").strip(" ")
-                    if line in [None, "", " "]:
-                        continue
-                    line_list = line.split(":", 1)
-                    if len(line_list) == 2:
-                        metadata_data[line_list[0].replace(" ", "")] = line_list[1].strip(" ")
-                    elif len(line_list) == 1:
-                        metadata_data[line_list[0].replace(" ", "")] = ""
-
-                if not (list(metadata_data.keys()) == list(self.__metadata_template.keys())):
-                    metadata = {
-                        "status": False,
-                        "error": "MetadataFormatError",
-                        "data": {}
-                    }
-                else:
-                    metadata = {
-                        "status": True,
-                        "data": metadata_data
-                    }
-
-            info  = {
-                "status": True,
-                "command": command,
-                "description": description,
-                "buffer_permissions": buffer_permissions,
-                "metadata": metadata
-            }
-
-            return info
-
-    def set_plugin_info(self, plugin_name: str = None,
-                        command: str = None, description: str = None,
-                        buffer_permissions: Tuple[bool, bool] = None,
-                        metadata: dict = None) -> dict:
-        """
-        设置指定插件的信息
-        """
-        if plugin_name in [None, "", " "]:
-            plugin_name = os.path.splitext(os.path.basename(inspect.stack()[1][1]))[0]
-        
-        if plugin_name not in list(self.plugin_bridge.keys()):
-            info  = {
-                "status": False,
-                "error": "PluginNotFound"
-            }
-            return info
-        if command is None and description is None and \
-            buffer_permissions is None and metadata is None:
-            info  = {
-                "status": True,
-                "error": "Skip"
-            }
-            return info
-        only_metadata = False
-        if command is None and description is None and buffer_permissions is None:
-            only_metadata = True
-
-        status = True
-        if not only_metadata:
-            old_info = self.get_plugin_info(plugin_name=plugin_name)
-            if not old_info["status"]:
-                info  = {
-                    "status": False,
-                    "error": "GetOlderPluginInfoError"
-                }
-                return info
-
-            if command is None:
-                command = f'{old_info["command"]}'
-            if description is None:
-                description = f'{old_info["description"]}'
-            
-            buffer_permissions_str = "False:False"
-            if buffer_permissions is not None:
-                if not isinstance(buffer_permissions, tuple) or \
-                    len(buffer_permissions) != 2 or \
-                    not isinstance(buffer_permissions[0], bool) or \
-                    not isinstance(buffer_permissions[0], bool):
-                    info  = {
-                        "status": False,
-                        "error": "BufferPermissionsFormatError"
-                    }
-                    return info
-                read = str(buffer_permissions[0])
-                write = str(buffer_permissions[1])
-                buffer_permissions_str = f'{read}:{write}'
-            else:
-                read = str(old_info["buffer_permissions"][0])
-                write = str(old_info["buffer_permissions"][1])
-                buffer_permissions_str = f'{read}:{write}'
-
-            new_init_info = [
-                f'#{command.strip()}\n',
-                f'#{description.strip()}\n',
-            ]
-            try:
-                with self.__plugin_info_mutex:
-                    with open(self.path_converter(f"{self.plugin_dir}{plugin_name}{os.sep}__init__.py"), "r", encoding="utf-8") as init:
-                        lines = init.readlines()
-                        if len(lines) < 2:
-                            info  = {
-                                "status": False,
-                                "error": "InitFileFormatError"
-                            }
-                            return info
-                        if len(lines) >= 3:
-                            if buffer_permissions is not None or \
-                                lines[2].strip() not in [None, "", " ", "#"]:
-                                new_init_info.append(f'#{buffer_permissions_str.strip()}\n')
-                            else:
-                                new_init_info.append("#\n")
-                        elif buffer_permissions is not None:
-                            new_init_info.append(f'#{buffer_permissions_str.strip()}\n')
-                        else:
-                            new_init_info.append("#\n")
-                        new_init_info.extend(lines[3:])
-                        new_init_info[-1] = new_init_info[-1].strip()
-                with self.__plugin_info_mutex:
-                    with open(self.path_converter(f"{self.plugin_dir}{plugin_name}{os.sep}__init__.py"), "w", encoding="utf-8") as init:
-                        init.writelines(new_init_info)
-
-                status = True
-                if metadata is None:
-                    info  = {
-                        "status": True,
-                    }
-                    return info
-            except Exception as e:
-                print(f"Modify plugin info error: {str(e)}")
-                status = False
-                info  = {
-                    "status": status,
-                    "error": "ModifyPluginInfoError"
-                }
-                return info
-
-        if status and metadata is not None:
-            if not isinstance(metadata, dict):
-                info  = {
-                    "status": False,
-                    "error": "MetadataMustBeDict"
-                }
-                return info
-            if not (list(metadata.keys()) == list(self.__metadata_template.keys())):
-                metadata = {
-                    "status": False,
-                    "error": "MetadataFormatError",
-                }
-                return info
-
-            try:
-                with self.__plugin_info_mutex:
-                    with open(self.path_converter(f"{self.plugin_dir}{plugin_name}{os.sep}METADATA"), "w", encoding="utf-8") as meta:
-                        metadata_list = []
-                        for key, value in metadata.items():
-                                metadata_list.append(f"{key}: {value}\n")
-                        metadata_list[-1] = metadata_list[-1].strip()
-                        if metadata_list[-1].split(":")[1].strip() in [None, ""]:
-                            metadata_list[-1] += " "
-
-                        meta.writelines(metadata_list)
-
-                        info = {
-                            "status": True,
-                        }
-                        return info
-            except Exception as e:
-                print(f"Modify plugin info error: {str(e)}")
-                info  = {
-                    "status": False,
-                    "error": "ModifyPluginInfoError"
-                }
-                return info
             
     def getChatCreator(self, chat_id: str) -> Union[bool, dict]:
         """
-        获取群组创建者信息
+        Get group creator information
         """
         if str(chat_id)[0] == "-":
             req = self.getChatAdministrators(chat_id=str(chat_id))
             if req:
                 creator = []
                 for i, user in enumerate(req):
                     if user["status"] == "creator":
@@ -880,51 +651,51 @@
                 else:
                     return False
         else:
             return False
 
     def getChatMemberStatus(self, chat_id: str, user_id: str) -> Union[bool, str]:
         """
-        获取群组用户状态
-        "creator",
-        "administrator",
-        "member",
-        "restricted",
-        "left",
-        "kicked"
+        Get group user status
+            "creator",
+            "administrator",
+            "member",
+            "restricted",
+            "left",
+            "kicked"
         """
         if str(chat_id)[0] == "-":
             req = self.getChatMember(chat_id=chat_id, user_id=user_id)
 
             if req != False:
                 return req["status"]
         else:
             return False
 
     def getFileDownloadPath(self, file_id: str) -> Union[bool, str]:
         """
-        生成文件下载链接
-        注意：下载链接包含Bot Key
+        Generated file download link,
+        Attention: The download link contains the Bot Key
         """
         req = self.getFile(file_id=file_id)
         if req:
             file_path = req["file_path"]
             if (self._local_api_server != "False" and
                 "telegram.org" not in self._basic_url):
                 return file_path
             else:
-                file_download_path = self._basic_url + "file/bot" + self._key + r"/" + file_path
+                file_download_path = f'{self._basic_url}file/bot{self._key}/{file_path}'
                 return file_download_path
         else:
             return False
 
     def getChatAdminsUseridList(self, chat_id, skip_bot: bool = True,
                                 privilege_users: list = None) -> Union[bool, list]:
         """
-        获取聊天中的管理员user_id列表
+        Get the list of admin user_id in the chat
         """
         admins = []
         results = self.getChatAdministrators(chat_id=chat_id)
         if results != False:
             for result in results:
                 if skip_bot:
                     if str(result["user"]["is_bot"]) == "True":
@@ -944,97 +715,97 @@
             return False
 
         return admins
 
     @property
     def plugin_bridge(self):
         """
-        获取插件桥
+        Get plugin bridge
         """
 
         return copy.deepcopy(self.__plugin_bridge)
 
     @property
     def plugin_dir(self):
         """
-        获取插件路径
+        Get plugin dir
         """
 
         return self.__plugin_dir
 
     @property
     def version(self):
         """
-        获取框架版本号
+        Get the teelebot version number
         """
 
         return self.__VERSION
 
     @property
     def author(self):
         """
-        作者信息
+        Author information
         """
 
         return self.__AUTHOR
 
     @property
     def root_id(self):
         """
-        获取root用户ID
+        Get the user_id of bot admin
         """
 
         return self.__root_id
 
     @property
     def bot_id(self):
         """
-        获取Bot的ID
+        Get the user_id of bot
         """
 
         return self.__bot_id
 
     @property
     def uptime(self):
         """
-        获取框架的持续运行时间(单位为秒)
+        Get the running time of the framework (measured in seconds)
         """
         second = int(time.time()) - self.__start_time
 
         return second
 
     @property
     def response_times(self):
         """
-        获取框架启动后响应指令的统计次数
+        Get the total number of commands responded by the framework since startup
         """
         return self.__response_times
 
     @property
     def response_chats(self):
         """
-        获取框架启动后响应的所有群组ID
+        Get all the chat IDs that the framework has responded to since startup
         """
         return copy.deepcopy(self.__response_chats)
 
     @property
     def response_users(self):
         """
-        获取框架启动后响应的所有用户ID
+        Get all the user IDs that the framework has responded to since startup
         """
         return copy.deepcopy(self.__response_users)
     
     @property
     def proxies(self):
         """
-        获取代理信息
+        Get proxy information
         """
         return copy.deepcopy(self.__proxies)
-    
-    @property
-    def metadata_template(self):
-        """
-        获取插件元素据模板
-        """
-        return copy.deepcopy(self.__metadata_template)
+
+
+class MethodPositionalArgumentError(Exception):
+    def init(self, value):
+        self.value = value
+    def str(self):
+        return f'MethodPositionalArgumentError: {self.value}'
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## teelebot/buffer.py

```diff
@@ -1,10 +1,10 @@
 '''
 @creation date: 2021-04-25
-@last modification: 2023-05-11
+@last modification: 2023-05-14
 '''
 from __future__ import print_function
 from sys import getsizeof, stderr
 from itertools import chain
 from collections import deque
 from pathlib import Path
 from typing import Tuple, Union
@@ -14,36 +14,39 @@
     pass
 
 import threading
 import inspect
 import os
 import copy
 
+from .metadata import _Metadata
 
 class _Buffer(object):
     """
-    数据暂存器类
+    Buffer Class
     """
     def __init__(self, buffer_size, plugin_names, plugin_dir):
         self.__buffer_size = buffer_size
         self.__plugin_names = plugin_names
         self.__plugin_dir = plugin_dir
         self.__buffer_mutex = threading.Lock()
         self.__buffer = {}
+        self.__metadata = _Metadata(self.__plugin_dir)
 
         for plugin_name in self.__plugin_names:
             self.__buffer[plugin_name] = {}
 
     def __del__(self):
         del self.__buffer
+        del self.__buffer_mutex
 
     def status(self) -> Tuple[bool, dict]:
         """
-        获取数据暂存区的使用情况
-        单位为字节
+        Get the usage information of the buffer area,
+        measured in bytes
         """
         try:
             with self.__buffer_mutex:
                 used = self.__total_size(self.__buffer)
                 free = self.__buffer_size - used
                 size = self.__buffer_size
 
@@ -54,29 +57,29 @@
             }
             return True, result
         except Exception as e:
             return False, {"exception": e}
 
     def sizeof(self, plugin_name: str = None) -> Tuple[bool, Union[str, int]]:
         """
-        获取单个插件数据暂存区占用内存大小
-        单位为字节
+        Get the memory size occupied by the buffer area of a single plugin,
+        measured in bytes
         """
         if plugin_name in [None, "", " "]:
             plugin_name = os.path.splitext(os.path.basename(inspect.stack()[1][1]))[0]
 
         if plugin_name in self.__buffer.keys():
             with self.__buffer_mutex:
                 return True, self.__total_size(self.__buffer.get(plugin_name))
         else:
-            return False, "NoPlugin"
+            return False, "PluginNotFound"
 
     def read(self, plugin_name: str = None) -> Tuple[bool, Union[str, tuple, any]]:
         """
-        从暂存区读取数据
+        Read data from buffer area
         """
         isSelf = False
         if plugin_name in [None, "", " "]:
             isSelf = True
             plugin_name = os.path.splitext(os.path.basename(inspect.stack()[1][1]))[0]
 
         if plugin_name in self.__buffer.keys():
@@ -88,19 +91,19 @@
                     return False, "NoPermissionToRead"
             else:
                 return False, permissions
 
             with self.__buffer_mutex:
                 return True, copy.deepcopy(self.__buffer.get(plugin_name, {}))
         else:
-            return False, "NoPlugin"
+            return False, "PluginNotFound"
 
     def write(self, buffer: any, plugin_name: str = None) -> Tuple[bool, Union[str, tuple]]:
         """
-        写入数据到暂存区
+        Write data into the buffer area
         """
         isSelf = False
         if plugin_name in [None, "", " "]:
             isSelf = True
             plugin_name = os.path.splitext(os.path.basename(inspect.stack()[1][1]))[0]
 
         if plugin_name in self.__buffer.keys():
@@ -121,68 +124,51 @@
                 if (old_total_used - old_buffer_used) + new_buffer_used > self.__buffer_size:
                     return False, "BufferAreaIsFull"
                 else:
                     self.__buffer[plugin_name] = copy.deepcopy(buffer)
                     changed_size = self.__total_size(buffer)
                     return True, str(changed_size)
         else:
-            return False, "NoPlugin"
+            return False, "PluginNotFound"
 
     def _update(self, plugin_names):
         if str(inspect.stack()[1][3]) == "__load_plugin":
             with self.__buffer_mutex:
-                for plugin_name in list(self.__buffer.keys()): # 清理已卸载插件
+                for plugin_name in list(self.__buffer.keys()): # Clean up uninstalled plugins
                     if plugin_name not in plugin_names:
                         self.__buffer.pop(plugin_name)
 
                 for plugin_name in list(plugin_names):
-                    if plugin_name not in self.__buffer.keys(): # 添加新插件
+                    if plugin_name not in self.__buffer.keys(): # Add new plugins
                         self.__buffer[plugin_name] = {}
 
             return True
         else:
             return False
 
     def __permissions_check(self, plugin_name):
         if plugin_name in self.__buffer.keys():
-            if plugin_name != os.path.splitext(os.path.basename(inspect.stack()[1][1]))[0]: # 读写权限检查
-                with open(Path(self.__plugin_dir + plugin_name + os.sep + "__init__.py"), "r", encoding="utf-8") as init:
-                    lines = init.readlines()
-
-                for i, _ in enumerate(lines):
-                    lines[i] = lines[i].strip("\n")
-                    lines[i] = lines[i].strip("\r")
-                    lines[i] = lines[i].strip("")
-                    lines[i] = lines[i].strip()
-
-                if len(lines) > 2:
-                    permissions = lines[2][1:]
-                    if lines[2] == "#":
-                        permissions = "False:False"
-                else:
-                    permissions = "False:False" # 格式 读:写
+            if plugin_name != os.path.splitext(os.path.basename(inspect.stack()[1][1]))[0]: # Read/write access check
+                permissions = "False:False"
+                ok, data = self.__metadata.read(plugin_name=plugin_name)
+                if ok:
+                    if data["Buffer-permissions"] not in [None, "", " "]:
+                        permissions = data["Buffer-permissions"]
+                    bool_dict = {
+                        "True": True,
+                        "true": True,
+                        "False": False,
+                        "false": False
+                    }
+                    permissions_read = bool_dict[permissions.split(":")[0]]
+                    permissions_write = bool_dict[permissions.split(":")[1]]
 
-                if len(permissions.split(":")) == 2:
-                    permissions_read = permissions.split(":")[0]
-                    permissions_write = permissions.split(":")[1]
-                    if permissions_read in ["True", "False", "true", "false"] and \
-                        permissions_write in ["True", "False", "true", "false"]:
-                        bool_dict = {
-                            "True": True,
-                            "true": True,
-                            "False": False,
-                            "false": False
-                        }
-                        permissions_read = bool_dict[permissions_read]
-                        permissions_write = bool_dict[permissions_write]
-                        return True, tuple((permissions_read, permissions_write))
-                    else:
-                        return False, "PermissionFormatError"
+                    return True, tuple((permissions_read, permissions_write))
                 else:
-                    return False, "PermissionFormatError"
+                    return False, data
 
     def __total_size(self, o, handlers={}, verbose=False):
         dict_handler = lambda d: chain.from_iterable(d.items())
         all_handlers = {tuple: iter,
                         list: iter,
                         deque: iter,
                         dict: dict_handler,
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## teelebot/handler.py

```diff
@@ -1,40 +1,37 @@
 # -*- coding:utf-8 -*-
 '''
 @creation date: 2019-08-23
-@last modification: 2023-05-10
+@last modification: 2023-05-14
 '''
 import configparser
 import argparse
 import os
 import sys
 import copy
 import shutil
 import requests
 
 from pathlib import Path
+from .metadata import _Metadata
 from .version import __author__, __github__, __version__
+from .common import (
+    __metadata_templates__,
+    __metadata_version_in_use__,
+    __cloud_api_server__,
+    __common_pkg_prefix__,
+    __inline_mode_prefix__,
+    __config_template__
+)
+
+cloud_api_server = __cloud_api_server__
+common_pkg_prefix = __common_pkg_prefix__
+inline_mode_prefix = __inline_mode_prefix__
+metadata_template = __metadata_templates__[__metadata_version_in_use__]
 
-cloud_api_server = "https://api.telegram.org/"
-common_pkg_prefix = "~~"
-inline_mode_prefix = "?:"
-metadata_template = { # METADATA v1.0
-    "Metadata-version": "1.0",
-    "Plugin-name": "",
-    "Version": "",
-    "Summary": "",
-    "Home-page": "",
-    "Author": "",
-    "Author-email": "",
-    "License": "",
-    "Keywords": "",
-    "Requires-teelebot": "",
-    "Requires-dist": "",
-    "Source": ""
-}
 
 parser = argparse.ArgumentParser(description="teelebot console command list")
 parser.add_argument("-c", "--config", type=str,
                     help="specify the configuration file")
 parser.add_argument("-k", "--key", type=str,
                     help="specify the bot api token")
 parser.add_argument("-r", "--root", type=str,
@@ -60,23 +57,23 @@
     print("Author: " + __author__)
     print("Project: " + __github__)
     os._exit(0)
 
 
 def _config():
     '''
-    获取bot配置信息及初始化
+    Get the bot configuration information and initialize
     '''
     config = {}
 
     if args.config:
         config_dir = os.path.abspath(str(Path(args.config)))
     else:
-        config_dir = str(Path(os.path.abspath(
-                os.path.expanduser('~')) + "/.teelebot/config.cfg"))
+        config_dir = str(Path(
+            f"{os.path.abspath(os.path.expanduser('~'))}/.teelebot/config.cfg"))
     (path, filename) = os.path.split(config_dir)
     (filename_, extension) = os.path.splitext(filename)
     if extension != ".cfg":
         print("Only support configuration files with .cfg suffix.")
         os._exit(0)
     if not os.path.exists(str(Path(path))):
         os.makedirs(str(Path(path)))
@@ -91,38 +88,34 @@
         root = ""
         if args.root:
             root = args.root
         debug = "False"
         if args.debug:
             debug = "True"
         with open(config_dir, "w", encoding="utf-8") as conf_file:
-            conf_file.writelines([
-                "[config]" + "\n",
-                "key = " + str(key) + "\n",
-                "root_id = " + str(root) + "\n",
-                "plugin_dir = " + str(plugin_dir) + "\n",
-                "pool_size = 40" + "\n",
-                "buffer_size = 16" + "\n",
-                "debug = " + str(debug) + "\n",
-                "local_api_server = False" + "\n",
-                "drop_pending_updates = False" + "\n",
-                "updates_chat_member = False" + "\n",
-                "webhook = False" + "\n",
-                "self_signed = False" + "\n",
-                "cert_key = " + "\n",
-                "cert_pub = " + "\n",
-                "server_address = " + "\n",
-                "server_port = " + "\n",
-                "local_address = " + "\n",
-                "local_port = " + "\n",
-                "proxy = "
-            ])
+            config_data = copy.deepcopy(__config_template__)
+            config_data["key"] = str(key)
+            config_data["root_id"] = str(root)
+            config_data["plugin_dir"] = str(plugin_dir)
+            config_data["debug"] = str(debug)
+
+            config_list = []
+            for key, value in config_data.items():
+                if key == "[config]":
+                    config_list.append(f"{key}\n")
+                else:
+                    config_list.append(f"{key} = {value}\n")
+            config_list[-1] = config_list[-1].strip()
+            if config_list[-1].split("=")[1].strip() in [None, ""]:
+                    config_list[-1] += " "
+
+            conf_file.writelines(config_list)
             os.system("")
             print("The configuration file has been created automatically.")
-            print("Configuration file path: \033[1;32m" + str(config_dir) + "\033[0m") # Green
+            print(f"Configuration file path: \033[1;32m{str(config_dir)}\033[0m") # Green
         if not args.key or not args.root:
             print("Please modify the relevant parameters and restart the teelebot.")
             os._exit(0)
         # else:
         #     print("\n")
 
     conf = configparser.ConfigParser()
@@ -155,15 +148,15 @@
         config[str(option)] = conf.get("config", option)
 
     none_count = 0
     for default_arg in default_args:
         if config[default_arg] == "" or\
             config[default_arg] == None:
             none_count += 1
-            print("Field " + default_arg + " is not set in configuration file.")
+            print(f"Field {default_arg} is not set in configuration file.")
     if none_count != 0:
         os._exit(0)
 
     if any(["version" in config.keys(), "author" in config.keys()]):
         print("Error in configuration file.")
         os._exit(0)
 
@@ -186,41 +179,36 @@
         else:
             plugin_dir = str(Path(os.path.abspath(config["plugin_dir"]))) + os.sep
             plugin_dir_in_config = True
     else:
         print("Field plugin_dir does not exist in configuration file.")
         os._exit(0)
 
-    if os.path.exists(str(Path(os.path.dirname(
-        os.path.abspath(__file__)) + r"/__pycache__"))):
-        shutil.rmtree(str(Path(os.path.dirname(
-            os.path.abspath(__file__)) + r"/__pycache__")))
+    pycache_path = f'{os.path.dirname(os.path.abspath(__file__))}/__pycache__'
+    if os.path.exists(str(Path(pycache_path))):
+        shutil.rmtree(str(Path(pycache_path)))
 
-    if not os.path.isdir(plugin_dir):  # 插件目录检测
+    if not os.path.isdir(plugin_dir):  # Plugin directory detection
         os.makedirs(plugin_dir)
         # os.mkdir(plugin_dir)
-        with open(str(Path(plugin_dir + "__init__.py")), "w", encoding="utf-8") as f:
+        with open(str(Path(f'{plugin_dir}__init__.py')), "w", encoding="utf-8") as f:
             pass
-    elif not os.path.exists(str(Path(plugin_dir + "__init__.py"))):
-        with open(str(Path(plugin_dir + "__init__.py")), "w", encoding="utf-8") as f:
+    elif not os.path.exists(str(Path(f'{plugin_dir}__init__.py'))):
+        with open(str(Path(f'{plugin_dir}__init__.py')), "w", encoding="utf-8") as f:
             pass
 
-    if args.make_plugin and plugin_dir_in_config: #插件模板创建
+    if args.make_plugin and plugin_dir_in_config: # Plugin template creation
         plugin_name = args.make_plugin
         if not os.path.exists(str(Path(plugin_dir + plugin_name))):
             os.mkdir(str(Path(plugin_dir + plugin_name)))
-            if not os.path.exists(str(Path(plugin_dir + plugin_name + os.sep + "__init__.py"))):
-                with open(str(Path(plugin_dir + plugin_name + os.sep + "__init__.py")), "w", encoding="utf-8") as init:
-                    init.writelines([
-                        "#/" + plugin_name.lower() + "\n",
-                        "#" + plugin_name + " Plugin\n",
-                        "#"
-                    ])
-            if not os.path.exists(str(Path(plugin_dir + plugin_name + os.sep + plugin_name + ".py"))):
-                with open(str(Path(plugin_dir + plugin_name + os.sep + plugin_name + ".py")), "w", encoding="utf-8") as enter:
+            if not os.path.exists(str(Path(f'{plugin_dir}{plugin_name}{os.sep}__init__.py'))):
+                with open(str(Path(f'{plugin_dir}{plugin_name}{os.sep}__init__.py')), "w", encoding="utf-8") as init:
+                    pass
+            if not os.path.exists(str(Path(f'{plugin_dir}{plugin_name}{os.sep}{plugin_name}.py'))):
+                with open(str(Path(f'{plugin_dir}{plugin_name}{os.sep}{plugin_name}.py')), "w", encoding="utf-8") as enter:
                     enter.writelines([
                         "# -*- coding: utf-8 -*-\n",
                         "\n",
                         "def " + plugin_name + "(bot, message):\n",
                         "\n" + \
                         "    # root_id = bot.root_id\n" + \
                         "    # bot_id = bot.bot_id\n" + \
@@ -233,54 +221,56 @@
                         "\n" + \
                         "    # uptime = bot.uptime\n" + \
                         "    # response_times = bot.response_times\n" + \
                         "    # response_chats = bot.response_chats\n" + \
                         "    # response_users = bot.response_users\n" + \
                         "\n" + \
                         "    # proxies = bot.proxies\n" + \
-                        "    # metadata_template = bot.metadata_template\n" + \
                         "\n" + \
                         '    chat_id = message["chat"]["id"]\n' + \
                         '    user_id = message["from"]["id"]\n' + \
                         '    message_id = message["message_id"]\n' + \
                         "\n" + \
                         '    message_type = message["message_type"]\n' + \
                         '    chat_type = message["chat"]["type"]\n' + \
                         "\n" + \
-                        '    plugin_info = bot.get_plugin_info()\n' + \
                         '    command = ""\n' + \
-                        '    if plugin_info.get("status", False):\n' + \
-                        '        command = plugin_info.get("command", "")\n' + \
+                        '    ok, metadata = bot.metadata.read()\n' + \
+                        '    if ok:\n' + \
+                        '        command = metadata.get("Command", "")\n' + \
                         "\n\n" + \
                         "    # Write your plugin code below"
                     ])
-            if not os.path.exists(str(Path(plugin_dir + plugin_name + os.sep + "README.md"))):
-                with open(str(Path(plugin_dir + plugin_name + os.sep + "README.md")), "w", encoding='utf-8') as readme:
+            if not os.path.exists(str(Path(f'{plugin_dir}{plugin_name}{os.sep}README.md'))):
+                with open(str(Path(f'{plugin_dir}{plugin_name}{os.sep}README.md')), "w", encoding='utf-8') as readme:
                     readme.writelines([
-                        "# " + plugin_name + "\n"
+                        f"# {plugin_name}\n"
                     ])
-            if not os.path.exists(str(Path(plugin_dir + plugin_name + os.sep + "METADATA"))):
-                with open(str(Path(plugin_dir + plugin_name + os.sep + "METADATA")), "w", encoding='utf-8') as metadata:
+            if not os.path.exists(str(Path(f'{plugin_dir}{plugin_name}{os.sep}METADATA'))):
+                with open(str(Path(f'{plugin_dir}{plugin_name}{os.sep}METADATA')), "w", encoding='utf-8') as meta:
                     metadata_data = copy.deepcopy(metadata_template)
                     metadata_data["Plugin-name"] = plugin_name
+                    metadata_data["Command"] = f"/{plugin_name.lower()}"
+                    metadata_data["Buffer-permissions"] = "False:False"
                     metadata_data["Version"] = "0.1.0"
+                    metadata_data["Summary"] = f"{plugin_name} Plugin"
                     metadata_data["Requires-teelebot"] = f">={__version__}"
 
                     metadata_list = []
                     for key, value in metadata_data.items():
                         metadata_list.append(f"{key}: {value}\n")
                     metadata_list[-1] = metadata_list[-1].strip()
                     if metadata_list[-1].split(":")[1].strip() in [None, ""]:
                             metadata_list[-1] += " "
 
-                    metadata.writelines(metadata_list)
+                    meta.writelines(metadata_list)
 
-            print("Plugin " + plugin_name + " was created successfully.")
+            print(f"Plugin {plugin_name} was created successfully.")
         else:
-            print("Plugin " + plugin_name + " already exists.")
+            print(f"Plugin {plugin_name} already exists.")
         os._exit(0)
     elif args.make_plugin and not plugin_dir_in_config:
         print("The plugin_dir is not set in the configuration file.")
         os._exit(0)
 
     if "pool_size" in config.keys():
         if int(config["pool_size"]) < 1 or int(config["pool_size"]) > 100:
@@ -384,31 +374,33 @@
     config["plugin_info"] = _plugin_info(
         config["plugin_bridge"].keys(), config["plugin_dir"])
     config["non_plugin_info"] = _plugin_info(
         config["non_plugin_list"], config["plugin_dir"])
     config["cloud_api_server"] = cloud_api_server
     config["common_pkg_prefix"] = common_pkg_prefix
     config["inline_mode_prefix"] = inline_mode_prefix
-    config["metadata_template"] = metadata_template
 
     # print(config)
     return config
 
 def _bridge(plugin_dir):
     '''
-    获取插件和指令的映射
+    Get the mapping between plugins and commands
     '''
     plugin_bridge = {}
     non_plugin_list = []
     plugin_list = []
     corrupted_plugin_list = []
 
     plugin_lis = os.listdir(plugin_dir)
     for plugi in plugin_lis:
-        if os.path.isdir(str(Path(plugin_dir + plugi))) and plugi != "__pycache__" and plugi[0] != '.':
+        if os.path.isdir(str(Path(f'{plugin_dir}{plugi}'))) and plugi != "__pycache__" and plugi[0] != '.':
+            if not os.path.exists(Path(f"{plugin_dir}{plugi}{os.sep}__init__.py")):
+                with open(Path(f"{plugin_dir}{plugi}{os.sep}__init__.py"), "w", encoding="utf-8") as init: pass
+            
             entrance_exist = False
             entrance_count = 0
             try:
                 with open(str(Path(f"{plugin_dir}{plugi}{os.sep}{plugi}.py")), "r", encoding="utf-8") as e:
                     content = e.read()
                     if f"def {plugi}(bot, message):" in content or \
                         f"def {plugi}(message, bot):" in content or \
@@ -422,35 +414,24 @@
                         entrance_count += content.count(f"def {plugi}(bot,message):")
                         entrance_count += content.count(f"def {plugi}(message,bot):")
             except Exception as e:
                 os.system("")
                 print("\033[1;31mThe " + plugi + " plugin is corrupted: " + "\033[0m" + str(e))
 
             metadata_ok = False
-            try:
-                with open(str(Path(f"{plugin_dir}{plugi}{os.sep}METADATA")), "r", encoding="utf-8") as meta:
-                    lines = meta.readlines()
-                    metadata_data = {}
-                    for line in lines:
-                        line = line.strip("\n").strip(" ")
-                        if line in [None, "", " "]:
-                            continue
-                        line_list = line.split(":", 1)
-                        if len(line_list) == 2:
-                            metadata_data[line_list[0].replace(" ", "")] = line_list[1].strip(" ")
-                        elif len(line_list) == 1:
-                            metadata_data[line_list[0].replace(" ", "")] = ""
-
-                    if list(metadata_data.keys()) == list(metadata_template.keys()):
-                        metadata_ok = True
-            except Exception as e:
+            metadata = _Metadata(plugin_dir=plugin_dir)
+            ok, metadata_data = metadata.read(plugin_name=plugi)
+            if ok:
+                if list(metadata_data.keys()) == list(metadata_template.keys()):
+                    metadata_ok = True
+            else:
                 os.system("")
-                print("\033[1;31mThe " + plugi + " plugin is corrupted: " + "\033[0m" + str(e))
+                print(f"\033[1;31mThe {plugi} plugin is corrupted: \033[0m{str(metadata_data)}")
 
-            package_file_list = os.listdir(str(Path(plugin_dir + plugi)))
+            package_file_list = os.listdir(str(Path(f'{plugin_dir}{plugi}')))
             if plugi + ".py" in package_file_list and \
                 "__init__.py" in package_file_list and \
                 "METADATA" in package_file_list and \
                 entrance_exist and entrance_count == 1 and metadata_ok:
                 plugin_list.append(plugi)
             else:
                 corrupted_plugin_list.append(plugi)
@@ -464,57 +445,66 @@
                     error += "'__init__.py' "
                     missing_files_count += 1
                 if "METADATA" not in package_file_list:
                     error += "'METADATA' "
                     missing_files_count += 1
                 if missing_files_count != 0:
                     os.system("")
-                    print("\033[1;31mThe " + plugi + " plugin is corrupted: " + "\033[0m" + error)
+                    print(f"\033[1;31mThe {plugi} plugin is corrupted: \033[0m{error}")
                 
                 if not entrance_exist:
                     error = f"plugin not found entrance function '{plugi}'"
                     os.system("")
-                    print("\033[1;31mThe " + plugi + " plugin is corrupted: " + "\033[0m" + error)
+                    print(f"\033[1;31mThe {plugi} plugin is corrupted: \033[0m{error}")
                 elif entrance_exist and entrance_count != 1:
                     error = f"multiple entrance functions exist in plugin"
                     os.system("")
-                    print("\033[1;31mThe " + plugi + " plugin is corrupted: " + "\033[0m" + error)
+                    print(f"\033[1;31mThe {plugi} plugin is corrupted: \033[0m{error}")
 
                 if not metadata_ok:
                     error = f"metadata format error"
                     os.system("")
-                    print("\033[1;31mThe " + plugi + " plugin is corrupted: " + "\033[0m" + error)
+                    print(f"\033[1;31mThe {plugi} plugin is corrupted: \033[0m{error}")
 
     for plugin in plugin_list:
-        with open(str(Path(plugin_dir + plugin + r"/__init__.py")), encoding="utf-8") as f:
-            row_one = f.readline().strip()[1:]
-            if row_one != common_pkg_prefix:  # Hidden plugin
-                plugin_bridge[plugin] = row_one
+        metadata_data = {}
+        metadata = _Metadata(plugin_dir=plugin_dir)
+        ok, data = metadata.read(plugin_name=plugin)
+        if ok:
+            if list(data.keys()) == list(metadata_template.keys()):
+                metadata_data = data
+        else:
+            os.system("")
+            print(f"\033[1;31mThe {plugi} plugin is corrupted: \033[0m{data}")
+            continue
+        
+        if metadata_data["Command"] != common_pkg_prefix:  # Hidden plugin
+            plugin_bridge[plugin] = metadata_data["Command"]
+        else:
+            if plugin in corrupted_plugin_list:
+                if (f'{plugin_dir}{plugin}') in sys.path:
+                    sys.path.remove(f'{plugin_dir}{plugin}')
+                if (f'{plugin_dir}{plugin}') in sys.modules:
+                    sys.modules.pop(f'{plugin_dir}{plugin}')
             else:
-                if plugin in corrupted_plugin_list:
-                    if (plugin_dir + plugin) in sys.path:
-                        sys.path.remove(plugin_dir + plugin)
-                    if (plugin_dir + plugin) in sys.modules:
-                        sys.modules.pop(plugin_dir + plugin)
-                else:
-                    non_plugin_list.append(plugin)
-                    if (plugin_dir + plugin) not in sys.path:
-                        sys.path.append(plugin_dir + plugin)
+                non_plugin_list.append(plugin)
+                if (f'{plugin_dir}{plugin}') not in sys.path:
+                    sys.path.append(f'{plugin_dir}{plugin}')
 
     # print(sys.path)
     # print(plugin_bridge, non_plugin_list)
     return plugin_bridge, non_plugin_list
 
 def _plugin_info(plugin_list, plugin_dir):
     '''
-    获取插件修改状态
+    Get the status of the plugin modification
     '''
     plugin_info = {}
     for plugin in plugin_list:
-        mtime = os.stat(str(Path(plugin_dir + plugin + "/" + plugin + ".py"))).st_mtime
+        mtime = os.stat(str(Path(f"{plugin_dir}{plugin}{os.sep}{plugin}.py"))).st_mtime
         plugin_info[plugin] = mtime
 
     return plugin_info
 
 
 if args.close and args.logout:
     print("Only one of logout and close can be used at the same time.")
@@ -550,11 +540,11 @@
         print("Error request the the local API server.")
         os._exit(0)
     if req.json().get("ok"):
         print("Successfully close from the local API server.")
     elif not req.json().get("ok"):
         print("Error close from the local API server.")
         if req.json().get("error_code") == 429:
-            print("Too many requests, please retry after " + str(req.json().get("parameters")["retry_after"]) + " seconds.")
+            print(f'Too many requests, please retry after {str(req.json().get("parameters")["retry_after"])} seconds.')
     os._exit(0)
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## teelebot/polling.py

```diff
@@ -1,30 +1,30 @@
 # -*- coding:utf-8 -*-
 '''
 @creation date: 2020-06-23
-@last modification: 2023-05-03
+@last modification: 2023-05-14
 '''
 import os
 import signal
 
 
 def _runUpdates(bot):
 
     signal.signal(signal.SIGINT, __exit)
     while True:
         results = bot.getUpdates(
             offset=bot._offset,
             limit=100,
             timeout=bot._timeout,
             allowed_updates=bot._allowed_updates
-        ) # 获取消息队列messages
+        ) # Get the message queue 'messages'
         messages = bot._washUpdates(results)
         if messages is None or not messages:
             continue
-        for message in messages:  # 获取单条消息message
+        for message in messages:  # Retrieve a single message 'message'
             bot._pluginRun(bot, message)
 
 
 def __exit(signum, frame):
     print("Bot Exit.")
     os._exit(0)
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## teelebot/request.py

```diff
@@ -1,21 +1,22 @@
 # -*- coding:utf-8 -*-
 '''
 @creation date: 2019-11-15
-@last modification: 2023-05-06
+@last modification: 2023-05-14
 '''
 import json
 import requests
+
 from .logger import _logger
 from traceback import extract_stack
 
 
 class _Request(object):
     """
-    接口请求类
+    Request Class
     """
     def __init__(self, thread_pool_size, url, debug=False, proxies={"all": None}):
         self.__url = url
         self.__debug = debug
         self.__proxies = proxies
         self.__session = self.__connection_session(
             pool_connections=thread_pool_size,
@@ -23,44 +24,44 @@
         )
 
     def __del__(self):
         self.__session.close()
 
     def __connection_session(self, pool_connections=10, pool_maxsize=10, max_retries=5):
         """
-        连接池
+        Connection Pool
         """
         session = requests.Session()
         session.verify = False
-        session.trust_env = False
+        # session.trust_env = False
         session.proxies.update(self.__proxies)
         
 
         adapter = requests.adapters.HTTPAdapter(pool_connections=pool_connections,
                                                 pool_maxsize=pool_maxsize, max_retries=max_retries)
         session.mount('http://', adapter)
         session.mount('https://', adapter)
 
         return session
 
     def __debug_info(self, method_name, result):
         """
-        debug模式
+        Debug mode
         """
         if self.__debug and not result.get("ok"):
             stack_info = extract_stack()
-            if len(stack_info) > 8:  # 插件内
+            if len(stack_info) > 8:  # Plugin internal call
                 _logger.error(
                     "Request failed" + " - " + \
                     "From:" + stack_info[-3][2] + " - " + \
                     "Path:" + stack_info[5][0] + " - " + \
                     "Line:" + str(stack_info[5][1]) + " - " + \
                     "Method:" + method_name + " - " + \
                     "Result:" + str(result)) # function name: stack_info[6][2]
-            elif len(stack_info) > 3:  # 外部调用
+            elif len(stack_info) > 3:  # External call
                 _logger.error(
                     "Request failed" + " - " + \
                     "From:" + stack_info[0][0] + " - " + \
                     "Path:" + stack_info[1][0] + " - " + \
                     "Line:" + str(stack_info[0][1]) + " - " + \
                     "Method:" + method_name + " - " + \
                     "Result:" + str(result)) # function name: stack_info[6][2]
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## teelebot/schedule.py

```diff
@@ -1,19 +1,19 @@
 # -*- coding:utf-8 -*-
 '''
 @creation date: 2019-11-15
-@last modification: 2023-05-09
+@last modification: 2023-05-14
 '''
 import threading
 from uuid import uuid4
 from typing import Tuple, Callable
 
 class _Schedule(object):
     """
-    周期性任务类
+    Schedule Class
     """
     def __init__(self, queue_size):
         self.__queue_size = queue_size
         self.__queue_mutex = threading.Lock()
         self.__queue = {}
 
     def __del__(self):
@@ -31,15 +31,15 @@
             return True, t
         except Exception as e:
             print("Error:", str(e))
             return False, str(e)
 
     def add(self, gap: int, func: Callable[..., None], args: tuple) -> Tuple[bool, str]:
         """
-        添加周期性任务
+        Add schedule task
         """
         def __short_uuid():
             uuidChars = ("a", "b", "c", "d", "e", "f",
                     "g", "h", "i", "j", "k", "l", "m", "n", "o", "p", "q", "r", "s",
                     "t", "u", "v", "w", "x", "y", "z", "0", "1", "2", "3", "4", "5",
                     "6", "7", "8", "9", "A", "B", "C", "D", "E", "F", "G", "H", "I",
                     "J", "K", "L", "M", "N", "O", "P", "Q", "R", "S", "T", "U", "V",
@@ -64,15 +64,15 @@
 
             return True, uid
         else:
             return False, t
 
     def status(self) -> Tuple[bool, dict]:
         """
-        获取周期性任务池的使用情况
+        Retrieve usage statistics of the Schedule task pool
         """
         try:
             with self.__queue_mutex:
                 used = len(self.__queue)
                 free = self.__queue_size - used
                 size = self.__queue_size
 
@@ -83,28 +83,28 @@
             }
             return True, result
         except Exception as e:
             return False, {"exception": e}
 
     def find(self, uid: str) -> Tuple[bool, str]:
         """
-        查找周期性任务
+        Find schedule tasks
         """
         with self.__queue_mutex:
             if len(self.__queue) <= 0:
                 return False, "Empty"
 
             if str(uid) in self.__queue.keys():
                 return True, str(uid)
             else:
                 return False, "NotFound"
 
     def delete(self, uid: str) -> Tuple[bool, str]:
         """
-        移除周期性任务
+        Remove schedule tasks
         """
         if len(self.__queue) <= 0:
             return False, "Empty"
 
         if str(uid) in self.__queue.keys():
             self.__queue[str(uid)].cancel()
             with self.__queue_mutex:
@@ -112,15 +112,15 @@
 
             return True, str(uid)
         else:
             return False, "NotFound"
 
     def clear(self) -> Tuple[bool, str]:
         """
-        移除所有周期性任务
+        Remove all schedule tasks
         """
         if len(self.__queue) == 0:
             return False, "Empty"
         else:
             try:
                 for uid in list(self.__queue.keys()):
                     self.__queue[str(uid)].cancel()
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## teelebot/version.py

```diff
@@ -1,17 +1,18 @@
 # -*- coding:utf-8 -*-
 """
-@description:基于Telegram Bot Api 的机器人框架
+@description: A bot framework based on the Telegram Bot API
 @creation date: 2019-11-15
-@last modification: 2023-05-11
+@last modification: 2023-05-14
 @author: Pluto (github:plutobell)
-@version: 2.2.0
+@version: 2.3.0
 """
 
-__version__ = "2.2.0"
+__version__ = "2.3.0"
+
 __author__ = "Pluto"
 __email__ = "hi@ojoll.com"
 __blog__ = "https://ojoll.com"
 __github__ = "https://github.com/plutobell/teelebot"
 __description__ = "teelebot is a robot framework based on Telegram Bot API, with plug-in system, easy to extend."
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## Comparing `teelebot-2.2.0.dist-info/LICENSE` & `teelebot-2.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `teelebot-2.2.0.dist-info/METADATA` & `teelebot-2.3.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teelebot
-Version: 2.2.0
+Version: 2.3.0
 Summary: teelebot is a robot framework based on Telegram Bot API, with plug-in system, easy to extend.
 Home-page: https://ojoll.com
 Author: Pluto
 Author-email: hi@ojoll.com
 License: GPLv3
 Keywords: teelebot telegram bot telegram bot api telegram
 Classifier: Programming Language :: Python :: 3
@@ -327,15 +327,15 @@
 
 ```python
 # 导入Bot类
 from teelebot import Bot
 
 # 实例化Bot类
 # 不传参数时会使用teelebot默认配置文件路径下的配置文件实例化Bot类
-# 在v2.2.0及以上版本，可传递参数覆盖配置文件的设定，可用参数:
+# 在v2.2.0及以上版本，可传递参数覆盖配置文件的设定，可覆盖的参数:
 #     Bot(key: str = None, debug: bool = False, proxies: dict = None)
 bot = Bot()
 
 # 使用Bot类
 bot.sendMessage(chat_id="chat_id", text="Hello World!")
 ```
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: teelebot Version: 2.2.0 Summary: teelebot is a
+Metadata-Version: 2.1 Name: teelebot Version: 2.3.0 Summary: teelebot is a
 robot framework based on Telegram Bot API, with plug-in system, easy to extend.
 Home-page: https://ojoll.com Author: Pluto Author-email: hi@ojoll.com License:
 GPLv3 Keywords: teelebot telegram bot telegram bot api telegram Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Classifier: License :: OSI Approved :: GNU General Public License
 v3 (GPLv3) Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: requests
@@ -108,15 +108,15 @@
 é½å¯å¨å½ä»¤è¡éè¿åæ°æå¨æå®éç½®æä»¶è·¯å¾ï¼å½ä»¤æ ¼å¼ï¼
 ``` teelebot -c/--config  ```
 è·¯å¾å¿é¡»ä¸ºç»å¯¹è·¯å¾ï¼å¹¶ä¸éç½®æä»¶åä¹åºå½åå«å¨è·¯å¾åï¼æ­¤æåµä¸ä¼å¨æå®çéç½®æä»¶ä¸å­å¨æ¶èªå¨çæéç½®æä»¶
 ã #### åãå¯¼å¥ä½¿ç¨ ```python # å¯¼å¥Botç±» from teelebot import Bot #
 å®ä¾åBotç±» #
 ä¸ä¼ åæ°æ¶ä¼ä½¿ç¨teeleboté»è®¤éç½®æä»¶è·¯å¾ä¸çéç½®æä»¶å®ä¾åBotç±»
 #
-å¨v2.2.0åä»¥ä¸çæ¬ï¼å¯ä¼ éåæ°è¦çéç½®æä»¶çè®¾å®ï¼å¯ç¨åæ°:
+å¨v2.2.0åä»¥ä¸çæ¬ï¼å¯ä¼ éåæ°è¦çéç½®æä»¶çè®¾å®ï¼å¯è¦ççåæ°:
 # Bot(key: str = None, debug: bool = False, proxies: dict = None) bot = Bot() #
 ä½¿ç¨Botç±» bot.sendMessage(chat_id="chat_id", text="Hello World!") ``` **Tip:
 å¯¼å¥ä½¿ç¨æ¶éè¦ç¡®ä¿é»è®¤éç½®æä»¶è·¯å¾ä¸­å­å¨éç½®æä»¶,å¹¶ä¸å¿é¡»çå­æ®µå·²ç»å¡«å**
 ## èç³»æ * Emailï¼hi#ojoll.com ( # == @ ) * Blog: [åå](https://
 ojoll.com) * Telegram Groupï¼[teelebot official](https://t.me/
 teelebot_official)ï¼t.me/teelebot_officialï¼ * ~~Telegram Groupï¼
 [teelebotä½éªç¾¤](http://t.me/teelebot_chat)ï¼t.me/teelebot_chatï¼~~ *
```

## Comparing `teelebot-2.2.0.dist-info/RECORD` & `teelebot-2.3.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-teelebot/__init__.py,sha256=_RulqeVSYAqRhTaljCZfWctBfVdmjCIC8Qp-ewpeOY4,4126
+teelebot/__init__.py,sha256=URjjM0wAafWAgeVlGRPfxRxInNzgFcWyc0vDC-Cznx0,4093
 teelebot/__main__.py,sha256=_j6f3hj0VtlcCsabcIvuS0uBI0NVbCVwmH138tqYGFo,165
-teelebot/bot.py,sha256=Gepj4s9ZPL2yNZAR_Df7PfJfWPMqvQr5LVy2NGGoiRU,42023
-teelebot/buffer.py,sha256=2h1dT2bz6G7H69dpclDZoGBWsFcoXbNUh2ytsXMrXGc,7835
-teelebot/handler.py,sha256=RHmXCz_Ooqqci_JN_KYQgAYtcM9HiJAB3gxPe_OsZEg,23836
+teelebot/bot.py,sha256=myIYPOuGJe-IIQRPuu_iVa5tpoShals5_oCurXm8-4g,32546
+teelebot/buffer.py,sha256=DkGfV_cfjYI7_FK-W34Wvcwox68I4w2Opqwe2-iDY-A,7128
+teelebot/common.py,sha256=HeLCXah603-WhNM77QmNci1ZZDaF_KnE6n32aOAzPNY,1556
+teelebot/handler.py,sha256=Q0BbUmucv2LxMW6bbR4le8Z5GK-2IlPF-G1YRFkxlLE,23343
 teelebot/logger.py,sha256=_QWA2Kbj-JWNYDtgeK6IE7q34Brxrq6cUgHEH4YTu2M,1807
-teelebot/polling.py,sha256=7lPDDeVInhk8MH-ZQhzGXYW-uI5t-F0XtMYkMrcEDEU,721
-teelebot/request.py,sha256=aYrdPV-IRJPdiZgZlIjU4es8QokOzs8Jn_bZVd_aI3I,3700
-teelebot/schedule.py,sha256=GGcFlEwpfO254D-2-ALBdAv539i97r_nAUnCJLBnA4o,4075
-teelebot/version.py,sha256=KH4QIKWu9j8DbB2tEDDblnkbRd_m351qOb0dSkLTuxc,482
+teelebot/metadata.py,sha256=q5hEzWW4SQ6hyAgwfltjgkhYoK7NcRkEFsieYHiXug8,6391
+teelebot/polling.py,sha256=yZPVAN3TxjGskf2jngdIpaA0Pi1SFzQSUt3WVJb6TuA,737
+teelebot/request.py,sha256=GQxJyyn2IZY6PuXqK-LJn_s6qjutEgxAIakCtumCNy8,3719
+teelebot/schedule.py,sha256=egn4EsUNPrtSkgOj1hxjNf1MQwJb95m5454rGatTpU8,4075
+teelebot/version.py,sha256=2t1PQKqgB7E9QegJ_jW0S28Ydttfd4J29uJmuOI4MOw,489
 teelebot/webhook.py,sha256=IomyaLxak_caDNYKNnLaTLtqkFToYq4sHWsD7kahV4Y,2665
-teelebot-2.2.0.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
-teelebot-2.2.0.dist-info/METADATA,sha256=9MF5dBUKrbWOcXCSUiTz8U7L0LM4N3X640XmZjW1z24,9624
-teelebot-2.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-teelebot-2.2.0.dist-info/entry_points.txt,sha256=IZHSiwFVJ6BPPTW3j7I1i34AESCOPaTYiC1qoWfpj6k,43
-teelebot-2.2.0.dist-info/top_level.txt,sha256=vMgTMVZJd4P3KjMwVpgWfIUvNLYKqfyHO4Cul-YwuyQ,9
-teelebot-2.2.0.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-teelebot-2.2.0.dist-info/RECORD,,
+teelebot-2.3.0.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
+teelebot-2.3.0.dist-info/METADATA,sha256=Jl0IdOHagoTVaVG7BQhMjBj_oYeJMVP_bSRbgDW20zI,9630
+teelebot-2.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+teelebot-2.3.0.dist-info/entry_points.txt,sha256=IZHSiwFVJ6BPPTW3j7I1i34AESCOPaTYiC1qoWfpj6k,43
+teelebot-2.3.0.dist-info/top_level.txt,sha256=vMgTMVZJd4P3KjMwVpgWfIUvNLYKqfyHO4Cul-YwuyQ,9
+teelebot-2.3.0.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+teelebot-2.3.0.dist-info/RECORD,,
```

