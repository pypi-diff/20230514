# Comparing `tmp/pwl-chat-python-1.4.2.tar.gz` & `tmp/pwl-chat-python-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwl-chat-python-1.4.2.tar", last modified: Thu May 11 06:40:54 2023, max compression
+gzip compressed data, was "pwl-chat-python-1.4.3.tar", last modified: Sun May 14 06:05:33 2023, max compression
```

## Comparing `pwl-chat-python-1.4.2.tar` & `pwl-chat-python-1.4.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-11 06:40:54.259082 pwl-chat-python-1.4.2/
--rw-r--r--   0 fangcong   (501) staff       (20)     1066 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.2/LICENSE
--rw-r--r--   0 fangcong   (501) staff       (20)     2008 2023-05-11 06:40:54.258795 pwl-chat-python-1.4.2/PKG-INFO
--rw-r--r--   0 fangcong   (501) staff       (20)     1409 2023-05-11 06:39:39.000000 pwl-chat-python-1.4.2/README.md
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-11 06:40:54.243081 pwl-chat-python-1.4.2/pwl_chat_python.egg-info/
--rw-r--r--   0 fangcong   (501) staff       (20)     2008 2023-05-11 06:40:54.000000 pwl-chat-python-1.4.2/pwl_chat_python.egg-info/PKG-INFO
--rw-r--r--   0 fangcong   (501) staff       (20)      549 2023-05-11 06:40:54.000000 pwl-chat-python-1.4.2/pwl_chat_python.egg-info/SOURCES.txt
--rw-r--r--   0 fangcong   (501) staff       (20)        1 2023-05-11 06:40:54.000000 pwl-chat-python-1.4.2/pwl_chat_python.egg-info/dependency_links.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       49 2023-05-11 06:40:54.000000 pwl-chat-python-1.4.2/pwl_chat_python.egg-info/entry_points.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       45 2023-05-11 06:40:54.000000 pwl-chat-python-1.4.2/pwl_chat_python.egg-info/requires.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       31 2023-05-11 06:40:54.000000 pwl-chat-python-1.4.2/pwl_chat_python.egg-info/top_level.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       38 2023-05-11 06:40:54.259179 pwl-chat-python-1.4.2/setup.cfg
--rw-r--r--   0 fangcong   (501) staff       (20)     3546 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.2/setup.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-11 06:40:54.243545 pwl-chat-python-1.4.2/src/
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-11 06:40:54.248970 pwl-chat-python-1.4.2/src/api/
--rw-r--r--   0 fangcong   (501) staff       (20)      312 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.2/src/api/__api__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1993 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.2/src/api/__init__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1743 2023-05-10 10:32:27.000000 pwl-chat-python-1.4.2/src/api/chatroom.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1124 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.2/src/api/user.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-11 06:40:54.256760 pwl-chat-python-1.4.2/src/core/
--rw-r--r--   0 fangcong   (501) staff       (20)     2625 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.2/src/core/__init__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1623 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.2/src/core/blacklist.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1960 2023-05-10 01:27:04.000000 pwl-chat-python-1.4.2/src/core/chatroom.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1961 2023-05-09 06:39:45.000000 pwl-chat-python-1.4.2/src/core/cli.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1630 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.2/src/core/config.py
--rw-r--r--   0 fangcong   (501) staff       (20)     4435 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.2/src/core/redpacket.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1360 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.2/src/core/user.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1226 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.2/src/core/websocket.py
--rw-r--r--   0 fangcong   (501) staff       (20)      991 2023-05-10 01:28:45.000000 pwl-chat-python-1.4.2/src/main.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-11 06:40:54.258074 pwl-chat-python-1.4.2/src/utils/
--rw-r--r--   0 fangcong   (501) staff       (20)      739 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.2/src/utils/utils.py
--rw-r--r--   0 fangcong   (501) staff       (20)       21 2023-05-11 06:39:58.000000 pwl-chat-python-1.4.2/src/utils/version.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-14 06:05:33.211877 pwl-chat-python-1.4.3/
+-rw-r--r--   0 fangcong   (501) staff       (20)     1066 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.3/LICENSE
+-rw-r--r--   0 fangcong   (501) staff       (20)     2008 2023-05-14 06:05:33.211429 pwl-chat-python-1.4.3/PKG-INFO
+-rw-r--r--   0 fangcong   (501) staff       (20)     1409 2023-05-11 06:39:39.000000 pwl-chat-python-1.4.3/README.md
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-14 06:05:33.201538 pwl-chat-python-1.4.3/pwl_chat_python.egg-info/
+-rw-r--r--   0 fangcong   (501) staff       (20)     2008 2023-05-14 06:05:33.000000 pwl-chat-python-1.4.3/pwl_chat_python.egg-info/PKG-INFO
+-rw-r--r--   0 fangcong   (501) staff       (20)      549 2023-05-14 06:05:33.000000 pwl-chat-python-1.4.3/pwl_chat_python.egg-info/SOURCES.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)        1 2023-05-14 06:05:33.000000 pwl-chat-python-1.4.3/pwl_chat_python.egg-info/dependency_links.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       49 2023-05-14 06:05:33.000000 pwl-chat-python-1.4.3/pwl_chat_python.egg-info/entry_points.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       45 2023-05-14 06:05:33.000000 pwl-chat-python-1.4.3/pwl_chat_python.egg-info/requires.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       31 2023-05-14 06:05:33.000000 pwl-chat-python-1.4.3/pwl_chat_python.egg-info/top_level.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       38 2023-05-14 06:05:33.212027 pwl-chat-python-1.4.3/setup.cfg
+-rw-r--r--   0 fangcong   (501) staff       (20)     3546 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.3/setup.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-14 06:05:33.201994 pwl-chat-python-1.4.3/src/
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-14 06:05:33.204073 pwl-chat-python-1.4.3/src/api/
+-rw-r--r--   0 fangcong   (501) staff       (20)      312 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.3/src/api/__api__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1762 2023-05-14 04:56:17.000000 pwl-chat-python-1.4.3/src/api/__init__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1743 2023-05-10 10:32:27.000000 pwl-chat-python-1.4.3/src/api/chatroom.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1124 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.3/src/api/user.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-14 06:05:33.209140 pwl-chat-python-1.4.3/src/core/
+-rw-r--r--   0 fangcong   (501) staff       (20)     2817 2023-05-14 05:06:48.000000 pwl-chat-python-1.4.3/src/core/__init__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1623 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.3/src/core/blacklist.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1960 2023-05-14 05:27:58.000000 pwl-chat-python-1.4.3/src/core/chatroom.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1961 2023-05-09 06:39:45.000000 pwl-chat-python-1.4.3/src/core/cli.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1561 2023-05-14 05:06:43.000000 pwl-chat-python-1.4.3/src/core/config.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     5256 2023-05-14 05:47:48.000000 pwl-chat-python-1.4.3/src/core/redpacket.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1360 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.3/src/core/user.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1226 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.3/src/core/websocket.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1329 2023-05-14 04:47:23.000000 pwl-chat-python-1.4.3/src/main.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-14 06:05:33.210486 pwl-chat-python-1.4.3/src/utils/
+-rw-r--r--   0 fangcong   (501) staff       (20)      977 2023-05-14 05:48:56.000000 pwl-chat-python-1.4.3/src/utils/utils.py
+-rw-r--r--   0 fangcong   (501) staff       (20)       21 2023-05-14 05:57:26.000000 pwl-chat-python-1.4.3/src/utils/version.py
```

### Comparing `pwl-chat-python-1.4.2/LICENSE` & `pwl-chat-python-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.2/PKG-INFO` & `pwl-chat-python-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.4.2
+Version: 1.4.3
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pwl-chat-python-1.4.2/README.md` & `pwl-chat-python-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.2/pwl_chat_python.egg-info/PKG-INFO` & `pwl-chat-python-1.4.3/pwl_chat_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.4.2
+Version: 1.4.3
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pwl-chat-python-1.4.2/pwl_chat_python.egg-info/SOURCES.txt` & `pwl-chat-python-1.4.3/pwl_chat_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.2/setup.py` & `pwl-chat-python-1.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.2/src/api/__init__.py` & `pwl-chat-python-1.4.3/src/api/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -47,16 +47,7 @@
             print("登陆失败: " + rsp['msg'])
             sys.exit(1)
 
     def get_yesterday_reward(self) -> dict:
         resp = requests.get(
             HOST + '/activity/yesterday-liveness-reward-api?apiKey=' + self.api_key, headers={'User-Agent': UA})
         return json.loads(resp.text)
-
-
-def from_instance(source: FishPi) -> FishPi:
-    newly = FishPi()
-    newly.user = source.user
-    newly.chatroom = source.chatroom
-    newly.api_key = source.api_key
-    newly.current_user = source.current_user
-    return newly
```

### Comparing `pwl-chat-python-1.4.2/src/api/chatroom.py` & `pwl-chat-python-1.4.3/src/api/chatroom.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.2/src/api/user.py` & `pwl-chat-python-1.4.3/src/api/user.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.2/src/core/__init__.py` & `pwl-chat-python-1.4.3/src/core/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,45 +4,48 @@
 from .chatroom import init_soliloquize
 from .cli import init_sys_in
 from .config import GLOBAL_CONFIG, RedPacketConfig, AuthConfig, RepeatConfig
 import configparser
 import os
 
 
-def __init__(api: FishPi):
-    file_path = f'{os.getcwd()}/config.ini'
+def __init__(api: FishPi, file_path: str = None):
+    if file_path is None:   
+        file_path = f'{os.getcwd()}/config.ini'
     config = configparser.ConfigParser()
     try:
         print("配置读取中")
         if not os.path.exists(file_path):
-            print("config.ini配置文件不存在")
+            print(f'{file_path}配置文件不存在')
             __init_default_config()
         else:
             config.read(file_path, encoding='utf-8')
             GLOBAL_CONFIG.auth_config = __init_login_auth_config(config)
-            GLOBAL_CONFIG.redpacket_config = __int_redpacket_var(config)
+            GLOBAL_CONFIG.redpacket_config = __int_redpacket_config(config)
             GLOBAL_CONFIG.repeat_config = __init_repeat_config(config)
     except:
-        print("config.ini配置文件不合法")
+        print(f'{file_path}配置文件不合法')
         __init_default_config()
     init_soliloquize(api)
     init_sys_in(api)
 
 
 def __init_default_config():
     print("加载默认配置文件")
     GLOBAL_CONFIG.auth_config = AuthConfig()
     GLOBAL_CONFIG.redpacket_config = RedPacketConfig()
     GLOBAL_CONFIG.repeat_config = RepeatConfig()
 
 
-def __int_redpacket_var(config) -> RedPacketConfig:
+def __int_redpacket_config(config) -> RedPacketConfig:
     ret = RedPacketConfig()
     if config.getint('redPacket', 'rate') > 0:
         ret.rate = config.getint('redPacket', 'rate')
+    if config.getint('redPacket', 'rpsLimit') > 0:
+        ret.rps_limit = config.getint('redPacket', 'rpsLimit')            
     ret.red_packet_switch = config.getboolean(
         'redPacket', 'openRedPacket')
     ret.heartbeat = config.getboolean(
         'redPacket', 'heartbeat')
     ret.smart_mode = config.getboolean(
         'redPacket', 'heartbeatSmartMode')
     ret.adventure_mode = config.getboolean(
```

### Comparing `pwl-chat-python-1.4.2/src/core/blacklist.py` & `pwl-chat-python-1.4.3/src/core/blacklist.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.2/src/core/chatroom.py` & `pwl-chat-python-1.4.3/src/core/chatroom.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.2/src/core/cli.py` & `pwl-chat-python-1.4.3/src/core/cli.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.2/src/core/config.py` & `pwl-chat-python-1.4.3/src/core/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 class RedPacketConfig(object):
     def __init__(self, red_packet_switch=True, heartbeat=True, smart_mode=True, threshold=0.5, adventure_mode=True,
-                 timeout=7, rate=3):
+                 timeout=7, rate=3, rps_limit=100):
         self.red_packet_switch = red_packet_switch
         self.heartbeat = heartbeat
         self.smart_mode = smart_mode
         self.threshold = threshold
         self.adventure_mode = adventure_mode
         self.timeout = timeout
         self.rate = rate
+        self.rps_limit = rps_limit
 
 
 class AuthConfig(object):
     def __init__(self, username='', password='', mfa_code=''):
         self.username = username
         self.password = password
         self.mfa_code = mfa_code
 
-    @classmethod
-    def build(cls, map: dict):
-        return cls(map['username'], map['password'], map['2fa_code'])
-
 
 class RepeatConfig(object):
     def __init__(self, blacklist=[], repeat_mode_switch=False, frequency=5, soliloquize_switch=False,
                  soliloquize_frequency=20, sentences=[]):
         self.repeat_mode_switch = repeat_mode_switch
         self.frequency = frequency
         self.soliloquize_switch = soliloquize_switch
```

### Comparing `pwl-chat-python-1.4.2/src/core/redpacket.py` & `pwl-chat-python-1.4.3/src/core/redpacket.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 from src.api import FishPi
 import json
 import time
-
+import enum
+from src.utils import utils
 from .config import GLOBAL_CONFIG
 
+CODE = enum.Enum('REDPACKET_CODE', ['SUCCESS', 'LOSED', 'NOT_ME', "ZERO"])
+
 
-def __open_redpacket_render(username, redpacket: dict) -> None:
+def __open_redpacket_render(username, redpacket: dict) -> CODE:
     who = redpacket['who']
     for i in who:
         if i['userName'] == username:
             if i['userMoney'] < 0:
                 print("红包助手: 悲剧，你竟然被反向抢了红包(" + str(i['userMoney']) + ")!")
+                return CODE.LOSED
             elif i['userMoney'] == 0:
                 print("红包助手: 零溢事件，抢到了一个空的红包(" + str(i['userMoney']) + ")!")
+                return CODE.ZERO
             else:
                 print("红包助手: 恭喜，你抢到了一个红包(" + str(i['userMoney']) + ")!")
-            return i['userMoney']
+                return CODE.SUCCESS
     print("红包助手: 遗憾，比别人慢了一点点，建议换宽带!")
-    return 0
+    return CODE.NOT_ME
 
 
 def open_red_packet(api: FishPi, red_packet_id) -> None:
     resp_json = api.chatroom.open_redpacket(red_packet_id)
     if ('code' in resp_json and resp_json['code'] == -1):
         print(resp_json['msg'])
         return
@@ -29,15 +34,21 @@
 
 
 def open_rock_paper_scissors_packet(api: FishPi, red_packet_id) -> None:
     resp_json = api.chatroom.open_rock_paper_scissors_redpacket(red_packet_id)
     if ('code' in resp_json and resp_json['code'] == -1):
         print(resp_json['msg'])
         return
-    __open_redpacket_render(api.current_user, resp_json)
+    code = __open_redpacket_render(api.current_user, resp_json)
+    if code == CODE.SUCCESS:
+        api.chatroom.send(utils.RPS_SUCCESS)
+    elif code == CODE.LOSED:
+        api.chatroom.send(utils.RPS_LOSED)
+    elif code == CODE.ZERO:
+        api.chatroom.send(utils.RPS_ZERO)    
 
 
 def rush_redpacket(api: FishPi, redpacket):
     sender = redpacket['userName']
     if (GLOBAL_CONFIG.redpacket_config.red_packet_switch == False):
         print('红包助手: '+sender+'发送了一个红包 你错过了这个红包，请开启抢红包模式！')
         return
@@ -50,18 +61,25 @@
                 __analyzeHeartbeatRedPacket(api, redpacket['oId'])
                 return
             open_red_packet(api, redpacket['oId'])
         else:
             print('红包助手: '+sender+' 发送了一个心跳红包, 你选择跳过了这个心跳红包！不尝试赌一下人品吗？')
             return
     if content['type'] == 'rockPaperScissors':
-        print('红包助手: '+sender+' 发送了一个猜拳红包, 红包助手正在帮你猜拳，石头剪刀布！')
-        open_rock_paper_scissors_packet(api, redpacket['oId'])
+        print(
+            f'红包助手: {sender} 发送了一个猜拳红包, 但社区规定，助手抢红包要等{GLOBAL_CONFIG.redpacket_config.rate}秒哦～')
+        time.sleep(GLOBAL_CONFIG.redpacket_config.rate)
+        print('红包助手正在帮你猜拳，石头剪刀布！')
+        money = content['money']
+        if money > GLOBAL_CONFIG.redpacket_config.rps_limit:
+            print(f'红包助手: {sender} 发送了一个积分为({money})的猜拳红包, 怂了 不敢赌～')
+        else:
+            open_rock_paper_scissors_packet(api, redpacket['oId'])
     else:
-        print('红包助手: '+sender+' 发送了一个红包, 但社区规定，助手抢红包要等' +
+        print('红包助手: ' + sender+' 发送了一个红包, 但社区规定，助手抢红包要等' +
               str(GLOBAL_CONFIG.redpacket_config.rate)+'秒哦～')
         time.sleep(GLOBAL_CONFIG.redpacket_config.rate)
         open_red_packet(api, redpacket['oId'])
 
 
 def __analyzeHeartbeatRedPacket(api: FishPi, red_packet_id):
     for data in api.chatroom.more()['data']:
```

### Comparing `pwl-chat-python-1.4.2/src/core/user.py` & `pwl-chat-python-1.4.3/src/core/user.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.2/src/core/websocket.py` & `pwl-chat-python-1.4.3/src/core/websocket.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.2/src/main.py` & `pwl-chat-python-1.4.3/src/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,34 +4,37 @@
 from src.core.config import GLOBAL_CONFIG, AuthConfig
 from src.core.user import login
 from src.core.websocket import start
 from src.utils.version import __version__
 from src.api import FishPi
 
 
-def run(params: dict):
+class CliConfig(object):
+    def __init__(self, username: str = '', password: str = '', code: str = '', file_path: str = None):
+        self.username = username
+        self.password = password
+        self.code = code
+        self.file_path = file_path
+
+
+def run(config: CliConfig):
     api = FishPi()
-    __init__(api)
-    if params:
-        GLOBAL_CONFIG.auth_config = AuthConfig.build(params)
+    __init__(api, config.file_path)
+    if config.username is not None and config.password is not None:
+        GLOBAL_CONFIG.auth_config = AuthConfig(
+            config.username, config.password, config.code)
     login(api)
     start(api)
 
 
 @click.command()
 @click.version_option(__version__)
 @click.option("--username", "-u", type=click.STRING, help="摸鱼派用户名")
 @click.option("--password", "-p", type=click.STRING, help="密码")
 @click.option("--code", "-c", type=click.STRING, help="两步验证码")
-def cli(username: str, password: str, code: str) -> str:
-    if username is None or password is None:
-        run({})
-    else:
-        run({
-            'username': username,
-            'password': password,
-            '2fa_code': code
-        })
+@click.option("--file_path", "-f", type=click.STRING, help="配置文件路径")
+def cli(username: str, password: str, code: str, file_path: str) -> str:
+    run(CliConfig(username, password, code, file_path))
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `pwl-chat-python-1.4.2/src/utils/utils.py` & `pwl-chat-python-1.4.3/src/utils/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,7 +9,11 @@
 [#online-users] 查看当前在线的用户列表
 [#user username] 输入 #user 用户名 可查看此用户详细信息 (#user Gakkiyomi)
 [#blacklist] 查看黑名单列表
 [#ban username] 将某人送入黑名单
 [#unban username] 将某人解除黑名单
 [#liveness] 查看当前活跃度(⚠️慎用，如果频繁请求此命令(最少间隔30s)，登录状态会被直接注销,需要重启脚本！)
 '''
+
+RPS_SUCCESS = '![](https://file.fishpi.cn/2023/01/XN3Y9-cf3997b7.jpeg)'
+RPS_LOSED = '![](https://pwl.stackoverflow.wiki/2022/04/MB2SCYFZFVT2DQ0GI7-c6447c10.jpg)'
+RPS_ZERO = '![](https://file.fishpi.cn/2023/05/1683183148506-4c31497e.png)'
```

