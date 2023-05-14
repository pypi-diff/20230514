# Comparing `tmp/kynaylibs-7.0.3.tar.gz` & `tmp/kynaylibs-7.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kynaylibs-7.0.3.tar", last modified: Sat May  6 10:41:57 2023, max compression
+gzip compressed data, was "kynaylibs-7.0.4.tar", last modified: Sun May 14 19:46:43 2023, max compression
```

## Comparing `kynaylibs-7.0.3.tar` & `kynaylibs-7.0.4.tar`

### file list

```diff
@@ -1,31 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:41:57.658970 kynaylibs-7.0.3/
--rw-r--r--   0 root         (0) root         (0)    35182 2023-05-06 09:59:38.000000 kynaylibs-7.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2464 2023-05-06 10:41:57.658970 kynaylibs-7.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1590 2023-05-06 09:59:38.000000 kynaylibs-7.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:41:57.654969 kynaylibs-7.0.3/kynaylibs/
--rw-r--r--   0 root         (0) root         (0)       46 2023-05-06 10:41:44.000000 kynaylibs-7.0.3/kynaylibs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:41:57.654969 kynaylibs-7.0.3/kynaylibs/core/
--rw-r--r--   0 root         (0) root         (0)      426 2023-05-06 10:35:46.000000 kynaylibs-7.0.3/kynaylibs/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      638 2023-05-06 09:59:38.000000 kynaylibs-7.0.3/kynaylibs/core/ai.py
--rw-r--r--   0 root         (0) root         (0)    15600 2023-05-06 09:59:38.000000 kynaylibs-7.0.3/kynaylibs/core/constants.py
--rw-r--r--   0 root         (0) root         (0)     1861 2023-05-06 09:59:38.000000 kynaylibs-7.0.3/kynaylibs/core/cos_cmd.py
--rw-r--r--   0 root         (0) root         (0)      226 2023-05-06 09:59:38.000000 kynaylibs-7.0.3/kynaylibs/core/data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:41:57.658970 kynaylibs-7.0.3/kynaylibs/core/db/
--rw-r--r--   0 root         (0) root         (0)     9282 2023-05-06 10:41:44.000000 kynaylibs-7.0.3/kynaylibs/core/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2267 2023-05-06 09:59:38.000000 kynaylibs-7.0.3/kynaylibs/core/db/pmpermit.py
--rw-r--r--   0 root         (0) root         (0)     1805 2023-05-06 09:59:38.000000 kynaylibs-7.0.3/kynaylibs/core/filter.py
--rw-r--r--   0 root         (0) root         (0)     4127 2023-05-06 09:59:38.000000 kynaylibs-7.0.3/kynaylibs/core/func.py
--rw-r--r--   0 root         (0) root         (0)     2946 2023-05-06 09:59:38.000000 kynaylibs-7.0.3/kynaylibs/core/inline.py
--rw-r--r--   0 root         (0) root         (0)    17800 2023-05-06 09:59:38.000000 kynaylibs-7.0.3/kynaylibs/core/lgs.py
--rw-r--r--   0 root         (0) root         (0)     2611 2023-05-06 09:59:38.000000 kynaylibs-7.0.3/kynaylibs/core/what.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:41:57.658970 kynaylibs-7.0.3/kynaylibs/nan/
--rw-r--r--   0 root         (0) root         (0)     1275 2023-05-06 10:35:46.000000 kynaylibs-7.0.3/kynaylibs/nan/__init__.py
--rw-r--r--   0 root         (0) root         (0)       46 2023-05-06 09:59:38.000000 kynaylibs-7.0.3/kynaylibs/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:41:57.654969 kynaylibs-7.0.3/kynaylibs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2464 2023-05-06 10:41:57.000000 kynaylibs-7.0.3/kynaylibs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      572 2023-05-06 10:41:57.000000 kynaylibs-7.0.3/kynaylibs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 10:41:57.000000 kynaylibs-7.0.3/kynaylibs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       83 2023-05-06 10:41:57.000000 kynaylibs-7.0.3/kynaylibs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-06 10:41:57.000000 kynaylibs-7.0.3/kynaylibs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 10:41:57.658970 kynaylibs-7.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1569 2023-05-06 10:24:44.000000 kynaylibs-7.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 19:46:43.845492 kynaylibs-7.0.4/
+-rw-r--r--   0 root         (0) root         (0)    35182 2023-05-14 19:46:25.000000 kynaylibs-7.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-05-14 19:46:43.845492 kynaylibs-7.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-05-14 19:46:25.000000 kynaylibs-7.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 19:46:43.841492 kynaylibs-7.0.4/kynaylibs/
+-rw-r--r--   0 root         (0) root         (0)     3438 2023-05-14 19:46:25.000000 kynaylibs-7.0.4/kynaylibs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1814 2023-05-14 19:46:25.000000 kynaylibs-7.0.4/kynaylibs/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     1331 2023-05-14 19:46:25.000000 kynaylibs-7.0.4/kynaylibs/config.py
+-rw-r--r--   0 root         (0) root         (0)      891 2023-05-14 19:46:25.000000 kynaylibs-7.0.4/kynaylibs/logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 19:46:43.841492 kynaylibs-7.0.4/kynaylibs/nan/
+-rw-r--r--   0 root         (0) root         (0)     2071 2023-05-14 19:46:25.000000 kynaylibs-7.0.4/kynaylibs/nan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 19:46:43.845492 kynaylibs-7.0.4/kynaylibs/nan/utils/
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-05-14 19:46:25.000000 kynaylibs-7.0.4/kynaylibs/nan/utils/PyroHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-05-14 19:46:25.000000 kynaylibs-7.0.4/kynaylibs/nan/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-05-14 19:46:25.000000 kynaylibs-7.0.4/kynaylibs/nan/utils/adminHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      646 2023-05-14 19:46:25.000000 kynaylibs-7.0.4/kynaylibs/nan/utils/ai.py
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-05-14 19:46:25.000000 kynaylibs-7.0.4/kynaylibs/nan/utils/aiohttp_helper.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2023-05-14 19:46:25.000000 kynaylibs-7.0.4/kynaylibs/nan/utils/basic.py
+-rw-r--r--   0 root         (0) root         (0)    15599 2023-05-14 19:46:25.000000 kynaylibs-7.0.4/kynaylibs/nan/utils/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 19:46:43.845492 kynaylibs-7.0.4/kynaylibs/nan/utils/db/
+-rw-r--r--   0 root         (0) root         (0)     8088 2023-05-14 19:46:25.000000 kynaylibs-7.0.4/kynaylibs/nan/utils/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2378 2023-05-14 19:46:25.000000 kynaylibs-7.0.4/kynaylibs/nan/utils/db/permit.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-05-14 19:46:25.000000 kynaylibs-7.0.4/kynaylibs/nan/utils/function.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2023-05-14 19:46:25.000000 kynaylibs-7.0.4/kynaylibs/nan/utils/inline.py
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-05-14 19:46:25.000000 kynaylibs-7.0.4/kynaylibs/nan/utils/interval.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2023-05-14 19:46:25.000000 kynaylibs-7.0.4/kynaylibs/nan/utils/misc.py
+-rw-r--r--   0 root         (0) root         (0)      555 2023-05-14 19:46:25.000000 kynaylibs-7.0.4/kynaylibs/nan/utils/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1844 2023-05-14 19:46:25.000000 kynaylibs-7.0.4/kynaylibs/nan/utils/pilter..py
+-rw-r--r--   0 root         (0) root         (0)    17782 2023-05-14 19:46:25.000000 kynaylibs-7.0.4/kynaylibs/nan/utils/tools.py
+-rw-r--r--   0 root         (0) root         (0)     2027 2023-05-14 19:46:25.000000 kynaylibs-7.0.4/kynaylibs/nan/utils/utility.py
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-14 19:46:25.000000 kynaylibs-7.0.4/kynaylibs/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 19:46:43.841492 kynaylibs-7.0.4/kynaylibs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-05-14 19:46:43.000000 kynaylibs-7.0.4/kynaylibs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      872 2023-05-14 19:46:43.000000 kynaylibs-7.0.4/kynaylibs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 19:46:43.000000 kynaylibs-7.0.4/kynaylibs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      335 2023-05-14 19:46:43.000000 kynaylibs-7.0.4/kynaylibs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-14 19:46:43.000000 kynaylibs-7.0.4/kynaylibs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 19:46:43.845492 kynaylibs-7.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-05-14 19:46:25.000000 kynaylibs-7.0.4/setup.py
```

### Comparing `kynaylibs-7.0.3/LICENSE` & `kynaylibs-7.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.3/PKG-INFO` & `kynaylibs-7.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kynaylibs
-Version: 7.0.3
+Version: 7.0.4
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `kynaylibs-7.0.3/README.md` & `kynaylibs-7.0.4/README.md`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.3/kynaylibs/core/constants.py` & `kynaylibs-7.0.4/kynaylibs/nan/utils/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 class Weebify:
     NORMIE_FONT = [
         "a",
         "b",
         "c",
         "d",
         "e",
```

### Comparing `kynaylibs-7.0.3/kynaylibs/core/db/__init__.py` & `kynaylibs-7.0.4/kynaylibs/nan/utils/db/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,23 @@
-
-from pyrogram.filters import chat
-from pyrogram import Client, filters
-from pyrogram.types import Message
-from typing import Dict, List, Union
+import asyncio
 from datetime import datetime, timedelta
-import pymongo.errors
 from platform import python_version as py
-from pyrogram import __version__ as pyro
-from ubotlibs.ubot.utils import *
-from Ubot.modules.basic import ADMINS
-from dateutil.relativedelta import relativedelta
-import asyncio
-import requests
-import asyncio
-from Ubot import *
+from typing import Dict, List, Union
 
-from motor.motor_asyncio import AsyncIOMotorClient as MongoCli
+import pymongo.errors
+import requests
 from config import *
-
+from dateutil.relativedelta import relativedelta
+from motor.motor_asyncio import AsyncIOMotorClient as MongoCli
+from naya import *
+from pyrogram import Client
+from pyrogram import __version__ as pyro
+from pyrogram import filters
+from pyrogram.filters import chat
+from pyrogram.types import Message
 
 mongo = MongoCli(MONGO_URL)
 db = mongo.naya
 
 coupledb = db.couple
 notesdb = db.notes
 filtersdb = db.filters
@@ -29,67 +25,66 @@
 usersdb = db.users
 logdb = db.gruplog
 blchatdb = db.blchat
 pmdb = db.pmpermit
 afkdb = db.afk
 prefdb = db.prefix
 confdb = db.conf
-        
 
-        
+
 async def buat_log(bot):
     user = await bot.get_me()
     user_id = user.id
     user_data = await usersdb.users.find_one({"user_id": user_id})
     botlog_chat_id = None
 
     if user_data:
         botlog_chat_id = user_data.get("bot_log_group_id")
 
     if not user_data or not botlog_chat_id:
-        group_name = 'Naya Premium Log'
-        group_description = 'Jangan Hapus Atau Keluar Dari Grup Ini\n\nCreated By @NayaProjectBot.\nJika menemukan kendala atau ingin menanyakan sesuatu\nHubungi : @kenapanan, @rizzvbss atau bisa ke @KynanSupport.'
+        group_name = "Naya Premium Logs"
+        group_description = "Jangan Hapus Atau Keluar Dari Grup Ini\n\nCreated By @KynanSupport .\nJika menemukan kendala atau ingin menanyakan sesuatu\nHubungi : @kenapanan, @rizzvbss atau bisa ke @KynanSupport."
         group = await bot.create_supergroup(group_name, group_description)
         botlog_chat_id = group.id
-        message_text = 'Grup Log Berhasil Dibuat,\nKetik `setlog` untuk menentapkan grup log ini sebagai tempat log bot\n\n**Notes** : Ini adalah userbot tanpa prefix jadi tidak perlu memakai triger `.`'
+        message_text = "Grup Log Berhasil Dibuat,\nKetik `setlog` untuk menentapkan grup log ini sebagai tempat log bot\n"
         await bot.send_message(botlog_chat_id, message_text)
         await asyncio.sleep(1)
-        
+
         await usersdb.users.insert_one(
             {"user_id": user_id},
             {"$set": {"bot_log_group_id": botlog_chat_id}},
-            upsert=True
+            upsert=True,
         )
-    
+
     if botlog_chat_id is None:
         return None
-    
-    return int(botlog_chat_id)
 
+    return int(botlog_chat_id)
 
 
 async def get_botlog(user_id: int):
     user_data = await logdb.users.find_one({"user_id": user_id})
     botlog_chat_id = user_data.get("bot_log_group_id") if user_data else None
     return botlog_chat_id
 
+
 async def set_botlog(user_id: int, botlog_chat_id: int):
     await logdb.users.update_one(
         {"user_id": user_id},
         {"$set": {"bot_log_group_id": botlog_chat_id}},
-        upsert=True
+        upsert=True,
     )
 
+
 async def get_log_groups(user_id: int):
     user_data = await logdb.users.find_one({"user_id": user_id})
     botlog_chat_id = user_data.get("bot_log_group_id") if user_data else []
     return botlog_chat_id
 
 
-
 async def _get_lovers(chat_id: int):
     lovers = await coupledb.find_one({"chat_id": chat_id})
     if lovers:
         lovers = lovers["couple"]
     else:
         lovers = {}
     return lovers
@@ -176,14 +171,15 @@
     return string
 
 
 def str_to_obj(string: str):
     obj = pickle.loads(codecs.decode(string.encode(), "base64"))
     return obj
 
+
 async def get_filters_count() -> dict:
     chats_count = 0
     filters_count = 0
     async for chat in filtersdb.find({"chat_id": {"$lt": 0}}):
         filters_name = await get_filters_names(chat["chat_id"])
         filters_count += len(filters_name)
         chats_count += 1
@@ -211,25 +207,23 @@
     name = name.lower().strip()
     _filters = await _get_filters(user_id, chat_id)
     if name in _filters:
         return _filters[name]
     return False
 
 
-
 async def save_filter(user_id: int, chat_id: int, name: str, _filter: dict):
     name = name.lower().strip()
     _filters = await _get_filters(user_id, chat_id)
     _filters[name] = _filter
     await filtersdb.update_one(
-    {"user_id": user_id, "chat_id": chat_id},
-    {"$set": {"filters": _filters}},
-    upsert=True
-)
-
+        {"user_id": user_id, "chat_id": chat_id},
+        {"$set": {"filters": _filters}},
+        upsert=True,
+    )
 
 
 async def delete_filter(user_id: int, chat_id: int, name: str) -> bool:
     filtersd = await _get_filters(user_id, chat_id)
     name = name.lower().strip()
     if name in filtersd:
         del filtersd[name]
@@ -237,21 +231,22 @@
             {"user_id": user_id, "chat_id": chat_id},
             {"$set": {"filters": filtersd}},
             upsert=True,
         )
         return True
     return False
 
-        
+
 async def blacklisted_chats(user_id: int) -> list:
     chats_list = []
     async for chat in blchatdb.users.find({"user_id": user_id, "chat_id": {"$lt": 0}}):
         chats_list.append(chat["chat_id"])
     return chats_list
 
+
 async def blacklist_chat(user_id: int, chat_id: int) -> bool:
     if not await blchatdb.users.find_one({"user_id": user_id, "chat_id": chat_id}):
         await blchatdb.users.insert_one({"user_id": user_id, "chat_id": chat_id})
         return True
     return False
 
 
@@ -261,56 +256,24 @@
         return True
     return False
 
 
 async def go_afk(user_id: int, time, reason=""):
     user_data = await afkdb.users.find_one({"user_id": user_id})
     if user_data:
-        await afkdb.users.update_one({"user_id": user_id}, {"$set": {"afk": True, "time": time, "reason": reason}})
+        await afkdb.users.update_one(
+            {"user_id": user_id},
+            {"$set": {"afk": True, "time": time, "reason": reason}},
+        )
     else:
-        await afkdb.users.insert_one({"user_id": user_id, "afk": True, "time": time, "reason": reason})
+        await afkdb.users.insert_one(
+            {"user_id": user_id, "afk": True, "time": time, "reason": reason}
+        )
 
 
 async def no_afk(user_id: int):
     await afkdb.users.delete_one({"user_id": user_id, "afk": True})
 
 
 async def check_afk(user_id: int):
     user_data = await afkdb.users.find_one({"user_id": user_id, "afk": True})
     return user_data
-
-async def set_custom_var(user_id: int, var, value):
-    p_variable = await confdb.users.find_one({"user_id": user_id, "var": var})
-    if p_variable:
-        await confdb.users.update_one(
-            {"user_id": user_id, "var": var},
-            {"$set": {"value": value}}
-        )
-    else:
-        await confdb.users.insert_one({"user_id": user_id, "var": var, "value": value})
-
-
-async def get_custom_var(user_id: int, var):
-    custom_var = await confdb.users.find_one({"user_id": user_id, "var": var})
-    if not custom_var:
-        return None
-    else:
-        g_custom_var = custom_var["value"]
-        return g_custom_var
-
-
-async def del_custom_var(user_id: int, var):
-    custom_var = await confdb.users.find_one({"user_id": user_id, "var": var})
-    if custom_var:
-        await confdb.users.delete_one({"user_id": user_id, "var": var})
-        return True
-    else:
-        return False
-
-
-async def get_cmd_handler(user_id: int):
-    custom_var = await get_custom_var(user_id, "CMD_HNDLR")
-    if custom_var:
-        return custom_var
-    else:
-        return "!"
-
```

### Comparing `kynaylibs-7.0.3/kynaylibs/core/db/pmpermit.py` & `kynaylibs-7.0.4/kynaylibs/nan/utils/db/permit.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,79 +1,80 @@
-from . import pmdb
-
-
-PMPERMIT_MESSAGE = (
-    "**Jangan Spam Atau Anda Akan Diblokir, Jadi Berhati-Hatilah Untuk Mengirim Pesan **"
-)
-
-BLOCKED = "**Anda Telah Melakukan Spam, BLOCKED!**"
-
-LIMIT = 5
-
-
-async def set_pm(user_id: int, value: bool):
-    doc = {"user_id": user_id, "pmpermit": value}
-    doc2 = {"user_id": "Approved", "users": []}
-    r = await pmdb.find_one({"user_id": user_id})
-    r2 = await pmdb.find_one({"user_id": "Approved"})
-    if r:
-        await pmdb.update_one({"user_id": user_id}, {"$set": {"pmpermit": value}})
-    else:
-        await pmdb.insert_one(doc)
-    if not r2:
-        await pmdb.insert_one(doc2)
-
-
-async def set_permit_message(user_id: int, text):
-    await pmdb.update_one({"user_id": user_id}, {"$set": {"pmpermit_message": text}}, upsert=True)
-
-
-
-async def set_block_message(user_id: int, text):
-    await pmdb.update_one({"user_id": user_id}, {"$set": {"block_message": text}}, upsert=True)
-
-
-async def set_limit(user_id: int, limit):
-    await pmdb.update_one({"user_id": user_id}, {"$set": {"limit": limit}}, upsert=True)
-
-
-async def get_pm_settings(user_id: int):
-    result = await pmdb.find_one({"user_id": user_id})
-    if not result:
-        return False
-    pmpermit = result["pmpermit"]
-    pm_message = result.get("pmpermit_message", PMPERMIT_MESSAGE)
-    block_message = result.get("block_message", BLOCKED)
-    limit = result.get("limit", LIMIT)
-    return pmpermit, pm_message, limit, block_message
-
-
-async def allow_user(chat):
-    r = await pmdb.find_one({"user_id": "Approved"})
-    if r:
-        await pmdb.update_one({"user_id": "Approved"}, {"$addToSet": {"users": chat}})
-    else:
-        doc = {"user_id": "Approved", "users": [chat]}
-        await pmdb.insert_one(doc)
-
-
-
-async def get_approved_users(user_id: int):
-    results = await pmdb.find_one({"user_id": "Approved"})
-    if results:
-        return results["users"]
-    else:
-        return []
-
-
-async def deny_user(chat):
-    await pmdb.update_one({"user_id": "Approved"}, {"$addToSet": {"users": chat}}, upsert=True)
-
-
-async def pm_guard(user_id: int):
-    result = await pmdb.find_one({"user_id": user_id})
-    if not result:
-        return False
-    if not result.get("pmpermit", False):
-        return False
-    else:
-        return True
+from . import pmdb
+
+PMPERMIT_MESSAGE = "**Jangan Spam Atau Anda Akan Diblokir, Jadi Berhati-Hatilah Untuk Mengirim Pesan **"
+
+BLOCKED = "**Anda Telah Melakukan Spam, BLOCKED!**"
+
+LIMIT = 5
+
+
+async def set_pm(user_id: int, value: bool):
+    doc = {"user_id": user_id, "pmpermit": value}
+    doc2 = {"user_id": "Approved", "users": []}
+    r = await pmdb.find_one({"user_id": user_id})
+    r2 = await pmdb.find_one({"user_id": "Approved"})
+    if r:
+        await pmdb.update_one({"user_id": user_id}, {"$set": {"pmpermit": value}})
+    else:
+        await pmdb.insert_one(doc)
+    if not r2:
+        await pmdb.insert_one(doc2)
+
+
+async def set_permit_message(user_id: int, text):
+    await pmdb.update_one(
+        {"user_id": user_id}, {"$set": {"pmpermit_message": text}}, upsert=True
+    )
+
+
+async def set_block_message(user_id: int, text):
+    await pmdb.update_one(
+        {"user_id": user_id}, {"$set": {"block_message": text}}, upsert=True
+    )
+
+
+async def set_limit(user_id: int, limit):
+    await pmdb.update_one({"user_id": user_id}, {"$set": {"limit": limit}}, upsert=True)
+
+
+async def get_pm_settings(user_id: int):
+    result = await pmdb.find_one({"user_id": user_id})
+    if not result:
+        return False
+    pmpermit = result["pmpermit"]
+    pm_message = result.get("pmpermit_message", PMPERMIT_MESSAGE)
+    block_message = result.get("block_message", BLOCKED)
+    limit = result.get("limit", LIMIT)
+    return pmpermit, pm_message, limit, block_message
+
+
+async def allow_user(chat):
+    r = await pmdb.find_one({"user_id": "Approved"})
+    if r:
+        await pmdb.update_one({"user_id": "Approved"}, {"$addToSet": {"users": chat}})
+    else:
+        doc = {"user_id": "Approved", "users": [chat]}
+        await pmdb.insert_one(doc)
+
+
+async def get_approved_users(user_id: int):
+    results = await pmdb.find_one({"user_id": "Approved"})
+    if results:
+        return results["users"]
+    else:
+        return []
+
+
+async def deny_user(chat):
+    await pmdb.update_one(
+        {"user_id": "Approved"}, {"$addToSet": {"users": chat}}, upsert=True
+    )
+
+
+async def pm_guard(user_id: int):
+    result = await pmdb.find_one({"user_id": user_id})
+    if not result:
+        return False
+    if not result.get("pmpermit", False):
+        return False
+    else:
+        return True
```

### Comparing `kynaylibs-7.0.3/kynaylibs/core/filter.py` & `kynaylibs-7.0.4/kynaylibs/nan/utils/pilter..py`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,80 @@
-import re
 from re import findall
 from re import sub as re_sub
+
 from pykeyboard import InlineKeyboard
 from pyrogram.types import InlineKeyboardButton as Ikb
 
+
 def ikb(data: dict, row_width: int = 2):
     return keyboard(data.items(), row_width=row_width)
 
+
 def get_urls_from_text(text: str) -> bool:
     regex = r"""(?i)\b((?:https?://|www\d{0,3}[.]|[a-z0-9.\-]
+
                 [.][a-z]{2,4}/)(?:[^\s()<>]+|\(([^\s()<>]+|(
+
                 \([^\s()<>]+\)))*\))+(?:\(([^\s()<>]+|(\([^\
+
                 ()<>]+\)))*\)|[^\s`!()\[\]{};:'".,<>?«»“”‘’]))""".strip()
+
     return [x[0] for x in findall(regex, str(text))]
 
+
 is_url = get_urls_from_text
 
+
 chat_filters_group = 1
 
+
 def keyboard(buttons_list, row_width: int = 2):
     buttons = InlineKeyboard(row_width=row_width)
+
     data = [
         (
             Ikb(text=str(i[0]), callback_data=str(i[1]))
             if not is_url(i[1])
             else Ikb(text=str(i[0]), url=str(i[1]))
         )
         for i in buttons_list
     ]
+
     buttons.add(*data)
+
     return buttons
 
+
 def extract_text_and_keyb(ikb, text: str, row_width: int = 2):
     keyboard = {}
+
     try:
         text = text.strip()
+
         if text.startswith("`"):
             text = text[1:]
+
         if text.endswith("`"):
             text = text[:-1]
 
         text, keyb = text.split("~")
 
         keyb = findall(r"\[.+\,.+\]", keyb)
+
         for btn_str in keyb:
             btn_str = re_sub(r"[\[\]]", "", btn_str)
+
             btn_str = btn_str.split(",")
+
             btn_txt, btn_url = btn_str[0], btn_str[1].strip()
 
             if not get_urls_from_text(btn_url):
                 continue
+
             keyboard[btn_txt] = btn_url
+
         keyboard = ikb(keyboard, row_width)
+
     except Exception:
         return
-    return text, keyboard
+
+    return text, keyboard
```

### Comparing `kynaylibs-7.0.3/kynaylibs/core/func.py` & `kynaylibs-7.0.4/kynaylibs/nan/utils/function.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,258 +1,251 @@
-00000000: 0d0a 0d0a 696d 706f 7274 206f 730d 0a69  ....import os..i
-00000010: 6d70 6f72 7420 7265 0d0a 696d 706f 7274  mport re..import
-00000020: 2073 7973 0d0a 696d 706f 7274 2061 7379   sys..import asy
-00000030: 6e63 696f 0d0a 696d 706f 7274 2074 7261  ncio..import tra
-00000040: 6365 6261 636b 0d0a 696d 706f 7274 2069  ceback..import i
-00000050: 6d70 6f72 746c 6962 0d0a 696d 706f 7274  mportlib..import
-00000060: 2073 7562 7072 6f63 6573 730d 0a66 726f   subprocess..fro
-00000070: 6d20 696f 2069 6d70 6f72 7420 4279 7465  m io import Byte
-00000080: 7349 4f0d 0a66 726f 6d20 7479 7065 7320  sIO..from types 
-00000090: 696d 706f 7274 204d 6f64 756c 6554 7970  import ModuleTyp
-000000a0: 650d 0a66 726f 6d20 7479 7069 6e67 2069  e..from typing i
-000000b0: 6d70 6f72 7420 4469 6374 0d0a 0d0a 6672  mport Dict....fr
-000000c0: 6f6d 2050 494c 2069 6d70 6f72 7420 496d  om PIL import Im
-000000d0: 6167 650d 0a66 726f 6d20 7079 726f 6772  age..from pyrogr
-000000e0: 616d 2069 6d70 6f72 7420 436c 6965 6e74  am import Client
-000000f0: 2c20 6572 726f 7273 2c20 7479 7065 730d  , errors, types.
-00000100: 0a0d 0a0d 0a0d 0a4d 4554 415f 434f 4d4d  .......META_COMM
-00000110: 454e 5453 203d 2072 652e 636f 6d70 696c  ENTS = re.compil
-00000120: 6528 7222 5e20 2a23 202a 6d65 7461 202b  e(r"^ *# *meta +
-00000130: 285c 532b 2920 2a3a 202a 282e 2a3f 295c  (\S+) *: *(.*?)\
-00000140: 732a 2422 2c20 7265 2e4d 554c 5449 4c49  s*$", re.MULTILI
-00000150: 4e45 290d 0a69 6e74 6572 6163 745f 7769  NE)..interact_wi
-00000160: 7468 5f74 6f5f 6465 6c65 7465 203d 205b  th_to_delete = [
-00000170: 5d0d 0a0d 0a0d 0a64 6566 2074 6578 7428  ]......def text(
-00000180: 6d65 7373 6167 653a 2074 7970 6573 2e4d  message: types.M
-00000190: 6573 7361 6765 2920 2d3e 2073 7472 3a0d  essage) -> str:.
-000001a0: 0a20 2020 2022 2222 4669 6e64 2074 6578  .    """Find tex
-000001b0: 7420 696e 2060 7479 7065 732e 4d65 7373  t in `types.Mess
-000001c0: 6167 6560 206f 626a 6563 7422 2222 0d0a  age` object"""..
-000001d0: 2020 2020 7265 7475 726e 206d 6573 7361      return messa
-000001e0: 6765 2e74 6578 7420 6966 206d 6573 7361  ge.text if messa
-000001f0: 6765 2e74 6578 7420 656c 7365 206d 6573  ge.text else mes
-00000200: 7361 6765 2e63 6170 7469 6f6e 0d0a 0d0a  sage.caption....
-00000210: 6173 796e 6320 6465 6620 6165 7865 6328  async def aexec(
-00000220: 636f 6465 2c20 632c 206d 293a 0d0a 2020  code, c, m):..  
-00000230: 2020 6578 6563 280d 0a20 2020 2020 2020    exec(..       
-00000240: 2022 6173 796e 6320 6465 6620 5f5f 6165   "async def __ae
-00000250: 7865 6328 632c 206d 293a 2022 0d0a 2020  xec(c, m): "..  
-00000260: 2020 2020 2020 2b20 2222 2e6a 6f69 6e28        + "".join(
-00000270: 6622 5c6e 207b 6c5f 7d22 2066 6f72 206c  f"\n {l_}" for l
-00000280: 5f20 696e 2063 6f64 652e 7370 6c69 7428  _ in code.split(
-00000290: 225c 6e22 2929 0d0a 2020 2020 290d 0a20  "\n"))..    ).. 
-000002a0: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-000002b0: 6c6f 6361 6c73 2829 5b22 5f5f 6165 7865  locals()["__aexe
-000002c0: 6322 5d28 632c 206d 290d 0a0d 0a0d 0a61  c"](c, m)......a
-000002d0: 7379 6e63 2064 6566 2073 6865 6c6c 5f65  sync def shell_e
-000002e0: 7865 6328 636f 6465 2c20 7472 6561 743d  xec(code, treat=
-000002f0: 5472 7565 293a 0d0a 2020 2020 7072 6f63  True):..    proc
-00000300: 6573 7320 3d20 6177 6169 7420 6173 796e  ess = await asyn
-00000310: 6369 6f2e 6372 6561 7465 5f73 7562 7072  cio.create_subpr
-00000320: 6f63 6573 735f 7368 656c 6c28 0d0a 2020  ocess_shell(..  
-00000330: 2020 2020 2020 636f 6465 2c20 7374 646f        code, stdo
-00000340: 7574 3d61 7379 6e63 696f 2e73 7562 7072  ut=asyncio.subpr
-00000350: 6f63 6573 732e 5049 5045 2c20 7374 6465  ocess.PIPE, stde
-00000360: 7272 3d61 7379 6e63 696f 2e73 7562 7072  rr=asyncio.subpr
-00000370: 6f63 6573 732e 5354 444f 5554 0d0a 2020  ocess.STDOUT..  
-00000380: 2020 290d 0a0d 0a20 2020 2073 7464 6f75    )....    stdou
-00000390: 7420 3d20 2861 7761 6974 2070 726f 6365  t = (await proce
-000003a0: 7373 2e63 6f6d 6d75 6e69 6361 7465 2829  ss.communicate()
-000003b0: 295b 305d 0d0a 2020 2020 6966 2074 7265  )[0]..    if tre
-000003c0: 6174 3a0d 0a20 2020 2020 2020 2073 7464  at:..        std
-000003d0: 6f75 7420 3d20 7374 646f 7574 2e64 6563  out = stdout.dec
-000003e0: 6f64 6528 292e 7374 7269 7028 290d 0a20  ode().strip().. 
-000003f0: 2020 2072 6574 7572 6e20 7374 646f 7574     return stdout
-00000400: 2c20 7072 6f63 6573 730d 0a0d 0a64 6566  , process....def
-00000410: 2066 6f72 6d61 745f 6578 6328 653a 2045   format_exc(e: E
-00000420: 7863 6570 7469 6f6e 2c20 7375 6666 6978  xception, suffix
-00000430: 3d22 2229 202d 3e20 7374 723a 0d0a 2020  ="") -> str:..  
-00000440: 2020 7472 6163 6562 6163 6b2e 7072 696e    traceback.prin
-00000450: 745f 6578 6328 290d 0a20 2020 2069 6620  t_exc()..    if 
-00000460: 6973 696e 7374 616e 6365 2865 2c20 6572  isinstance(e, er
-00000470: 726f 7273 2e52 5043 4572 726f 7229 3a0d  rors.RPCError):.
-00000480: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00000490: 280d 0a20 2020 2020 2020 2020 2020 2066  (..            f
-000004a0: 223c 623e 5465 6c65 6772 616d 2041 5049  "<b>Telegram API
-000004b0: 2065 7272 6f72 213c 2f62 3e5c 6e22 0d0a   error!</b>\n"..
-000004c0: 2020 2020 2020 2020 2020 2020 6622 3c63              f"<c
-000004d0: 6f64 653e 5b7b 652e 434f 4445 7d20 7b65  ode>[{e.CODE} {e
-000004e0: 2e49 4420 6f72 2065 2e4e 414d 457d 5d20  .ID or e.NAME}] 
-000004f0: e280 9420 7b65 2e4d 4553 5341 4745 2e66  ... {e.MESSAGE.f
-00000500: 6f72 6d61 7428 7661 6c75 653d 652e 7661  ormat(value=e.va
-00000510: 6c75 6529 7d3c 2f63 6f64 653e 5c6e 5c6e  lue)}</code>\n\n
-00000520: 3c62 3e7b 7375 6666 6978 7d3c 2f62 3e22  <b>{suffix}</b>"
-00000530: 0d0a 2020 2020 2020 2020 290d 0a20 2020  ..        )..   
-00000540: 2072 6574 7572 6e20 280d 0a20 2020 2020   return (..     
-00000550: 2020 2066 223c 623e 4572 726f 7221 3c2f     f"<b>Error!</
-00000560: 623e 5c6e 220d 0a20 2020 2020 2020 2066  b>\n"..        f
-00000570: 223c 636f 6465 3e7b 652e 5f5f 636c 6173  "<code>{e.__clas
-00000580: 735f 5f2e 5f5f 6e61 6d65 5f5f 7d3a 207b  s__.__name__}: {
-00000590: 657d 3c2f 636f 6465 3e5c 6e5c 6e3c 623e  e}</code>\n\n<b>
-000005a0: 7b73 7566 6669 787d 3c2f 623e 220d 0a20  {suffix}</b>".. 
-000005b0: 2020 2029 0d0a 0d0a 0d0a 6465 6620 7769     )......def wi
-000005c0: 7468 5f72 6570 6c79 2866 756e 6329 3a0d  th_reply(func):.
-000005d0: 0a20 2020 2061 7379 6e63 2064 6566 2077  .    async def w
-000005e0: 7261 7070 6564 2863 6c69 656e 743a 2043  rapped(client: C
-000005f0: 6c69 656e 742c 206d 6573 7361 6765 3a20  lient, message: 
-00000600: 7479 7065 732e 4d65 7373 6167 6529 3a0d  types.Message):.
-00000610: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00000620: 6d65 7373 6167 652e 7265 706c 795f 746f  message.reply_to
-00000630: 5f6d 6573 7361 6765 3a0d 0a20 2020 2020  _message:..     
-00000640: 2020 2020 2020 2061 7761 6974 206d 6573         await mes
-00000650: 7361 6765 2e65 6469 7428 223c 623e 5265  sage.edit("<b>Re
-00000660: 706c 7920 746f 206d 6573 7361 6765 2069  ply to message i
-00000670: 7320 7265 7175 6972 6564 3c2f 623e 2229  s required</b>")
-00000680: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-00000690: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000006a0: 7572 6e20 6177 6169 7420 6675 6e63 2863  urn await func(c
-000006b0: 6c69 656e 742c 206d 6573 7361 6765 290d  lient, message).
-000006c0: 0a0d 0a20 2020 2072 6574 7572 6e20 7772  ...    return wr
-000006d0: 6170 7065 640d 0a0d 0a0d 0a61 7379 6e63  apped......async
-000006e0: 2064 6566 2069 6e74 6572 6163 745f 7769   def interact_wi
-000006f0: 7468 286d 6573 7361 6765 3a20 7479 7065  th(message: type
-00000700: 732e 4d65 7373 6167 6529 202d 3e20 7479  s.Message) -> ty
-00000710: 7065 732e 4d65 7373 6167 653a 0d0a 2020  pes.Message:..  
-00000720: 2020 2222 220d 0a20 2020 2043 6865 636b    """..    Check
-00000730: 2068 6973 746f 7279 2077 6974 6820 626f   history with bo
-00000740: 7420 616e 6420 7265 7475 726e 2062 6f74  t and return bot
-00000750: 2773 2072 6573 706f 6e73 650d 0a0d 0a20  's response.... 
-00000760: 2020 2045 7861 6d70 6c65 3a0d 0a20 2020     Example:..   
-00000770: 202e 2e20 636f 6465 2d62 6c6f 636b 3a3a   .. code-block::
-00000780: 2070 7974 686f 6e0d 0a20 2020 2020 2020   python..       
-00000790: 2062 6f74 5f6d 7367 203d 2061 7761 6974   bot_msg = await
-000007a0: 2069 6e74 6572 6163 745f 7769 7468 2861   interact_with(a
-000007b0: 7761 6974 2062 6f74 2e73 656e 645f 6d65  wait bot.send_me
-000007c0: 7373 6167 6528 2240 426f 7446 6174 6865  ssage("@BotFathe
-000007d0: 7222 2c20 222f 7374 6172 7422 2929 0d0a  r", "/start"))..
-000007e0: 2020 2020 3a70 6172 616d 206d 6573 7361      :param messa
-000007f0: 6765 3a20 616c 7265 6164 7920 7365 6e74  ge: already sent
-00000800: 206d 6573 7361 6765 2074 6f20 626f 740d   message to bot.
-00000810: 0a20 2020 203a 7265 7475 726e 3a20 626f  .    :return: bo
-00000820: 7427 7320 7265 7370 6f6e 7365 0d0a 2020  t's response..  
-00000830: 2020 2222 220d 0a0d 0a20 2020 2061 7761    """....    awa
-00000840: 6974 2061 7379 6e63 696f 2e73 6c65 6570  it asyncio.sleep
-00000850: 2831 290d 0a20 2020 2023 206e 6f69 6e73  (1)..    # noins
-00000860: 7065 6374 696f 6e20 5079 5072 6f74 6563  pection PyProtec
-00000870: 7465 644d 656d 6265 720d 0a20 2020 2072  tedMember..    r
-00000880: 6573 706f 6e73 6520 3d20 5b0d 0a20 2020  esponse = [..   
-00000890: 2020 2020 206d 7367 0d0a 2020 2020 2020       msg..      
-000008a0: 2020 6173 796e 6320 666f 7220 6d73 6720    async for msg 
-000008b0: 696e 206d 6573 7361 6765 2e5f 636c 6965  in message._clie
-000008c0: 6e74 2e67 6574 5f63 6861 745f 6869 7374  nt.get_chat_hist
-000008d0: 6f72 7928 0d0a 2020 2020 2020 2020 2020  ory(..          
-000008e0: 2020 6d65 7373 6167 652e 6368 6174 2e69    message.chat.i
-000008f0: 642c 206c 696d 6974 3d31 0d0a 2020 2020  d, limit=1..    
-00000900: 2020 2020 290d 0a20 2020 205d 0d0a 2020      )..    ]..  
-00000910: 2020 7365 636f 6e64 735f 7761 6974 696e    seconds_waitin
-00000920: 6720 3d20 300d 0a0d 0a20 2020 2077 6869  g = 0....    whi
-00000930: 6c65 2072 6573 706f 6e73 655b 305d 2e66  le response[0].f
-00000940: 726f 6d5f 7573 6572 2e69 735f 7365 6c66  rom_user.is_self
-00000950: 3a0d 0a20 2020 2020 2020 2073 6563 6f6e  :..        secon
-00000960: 6473 5f77 6169 7469 6e67 202b 3d20 310d  ds_waiting += 1.
-00000970: 0a20 2020 2020 2020 2069 6620 7365 636f  .        if seco
-00000980: 6e64 735f 7761 6974 696e 6720 3e3d 2035  nds_waiting >= 5
-00000990: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-000009a0: 6169 7365 2052 756e 7469 6d65 4572 726f  aise RuntimeErro
-000009b0: 7228 2262 6f74 2064 6964 6e27 7420 616e  r("bot didn't an
-000009c0: 7377 6572 2069 6e20 3520 7365 636f 6e64  swer in 5 second
-000009d0: 7322 290d 0a0d 0a20 2020 2020 2020 2061  s")....        a
-000009e0: 7761 6974 2061 7379 6e63 696f 2e73 6c65  wait asyncio.sle
-000009f0: 6570 2831 290d 0a20 2020 2020 2020 2023  ep(1)..        #
-00000a00: 206e 6f69 6e73 7065 6374 696f 6e20 5079   noinspection Py
-00000a10: 5072 6f74 6563 7465 644d 656d 6265 720d  ProtectedMember.
-00000a20: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
-00000a30: 6520 3d20 5b0d 0a20 2020 2020 2020 2020  e = [..         
-00000a40: 2020 206d 7367 0d0a 2020 2020 2020 2020     msg..        
-00000a50: 2020 2020 6173 796e 6320 666f 7220 6d73      async for ms
-00000a60: 6720 696e 206d 6573 7361 6765 2e5f 636c  g in message._cl
-00000a70: 6965 6e74 2e67 6574 5f63 6861 745f 6869  ient.get_chat_hi
-00000a80: 7374 6f72 7928 0d0a 2020 2020 2020 2020  story(..        
-00000a90: 2020 2020 2020 2020 6d65 7373 6167 652e          message.
-00000aa0: 6368 6174 2e69 642c 206c 696d 6974 3d31  chat.id, limit=1
-00000ab0: 0d0a 2020 2020 2020 2020 2020 2020 290d  ..            ).
-00000ac0: 0a20 2020 2020 2020 205d 0d0a 0d0a 2020  .        ]....  
-00000ad0: 2020 696e 7465 7261 6374 5f77 6974 685f    interact_with_
-00000ae0: 746f 5f64 656c 6574 652e 6170 7065 6e64  to_delete.append
-00000af0: 286d 6573 7361 6765 2e69 6429 0d0a 2020  (message.id)..  
-00000b00: 2020 696e 7465 7261 6374 5f77 6974 685f    interact_with_
-00000b10: 746f 5f64 656c 6574 652e 6170 7065 6e64  to_delete.append
-00000b20: 2872 6573 706f 6e73 655b 305d 2e69 6429  (response[0].id)
-00000b30: 0d0a 0d0a 2020 2020 7265 7475 726e 2072  ....    return r
-00000b40: 6573 706f 6e73 655b 305d 0d0a 0d0a 0d0a  esponse[0]......
-00000b50: 0d0a 0d0a 6465 6620 7265 7369 7a65 5f69  ....def resize_i
-00000b60: 6d61 6765 280d 0a20 2020 2069 6e70 7574  mage(..    input
-00000b70: 5f69 6d67 2c20 6f75 7470 7574 3d4e 6f6e  _img, output=Non
-00000b80: 652c 2069 6d67 5f74 7970 653d 2250 4e47  e, img_type="PNG
-00000b90: 222c 2073 697a 653a 2069 6e74 203d 2035  ", size: int = 5
-00000ba0: 3132 2c20 7369 7a65 323a 2069 6e74 203d  12, size2: int =
-00000bb0: 204e 6f6e 650d 0a29 3a0d 0a20 2020 2069   None..):..    i
-00000bc0: 6620 6f75 7470 7574 2069 7320 4e6f 6e65  f output is None
-00000bd0: 3a0d 0a20 2020 2020 2020 206f 7574 7075  :..        outpu
-00000be0: 7420 3d20 4279 7465 7349 4f28 290d 0a20  t = BytesIO().. 
-00000bf0: 2020 2020 2020 206f 7574 7075 742e 6e61         output.na
-00000c00: 6d65 203d 2066 2273 7469 636b 6572 2e7b  me = f"sticker.{
-00000c10: 696d 675f 7479 7065 2e6c 6f77 6572 2829  img_type.lower()
-00000c20: 7d22 0d0a 0d0a 2020 2020 7769 7468 2049  }"....    with I
-00000c30: 6d61 6765 2e6f 7065 6e28 696e 7075 745f  mage.open(input_
-00000c40: 696d 6729 2061 7320 696d 673a 0d0a 2020  img) as img:..  
-00000c50: 2020 2020 2020 2320 5765 2075 7365 6420        # We used 
-00000c60: 746f 2075 7365 2074 6875 6d62 6e61 696c  to use thumbnail
-00000c70: 2873 697a 6529 2068 6572 652c 2062 7574  (size) here, but
-00000c80: 2069 7420 7265 7475 726e 7320 7769 7468   it returns with
-00000c90: 2061 202a 6d61 782a 2064 696d 656e 7369   a *max* dimensi
-00000ca0: 6f6e 206f 6620 3531 322c 3531 320d 0a20  on of 512,512.. 
-00000cb0: 2020 2020 2020 2023 2072 6174 6865 7220         # rather 
-00000cc0: 7468 616e 206d 616b 696e 6720 6f6e 6520  than making one 
-00000cd0: 7369 6465 2065 7861 6374 6c79 2035 3132  side exactly 512
-00000ce0: 2c20 736f 2077 6520 6861 7665 2074 6f20  , so we have to 
-00000cf0: 6361 6c63 756c 6174 6520 6469 6d65 6e73  calculate dimens
-00000d00: 696f 6e73 206d 616e 7561 6c6c 7920 3a28  ions manually :(
-00000d10: 0d0a 2020 2020 2020 2020 6966 2073 697a  ..        if siz
-00000d20: 6532 2069 7320 6e6f 7420 4e6f 6e65 3a0d  e2 is not None:.
-00000d30: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
-00000d40: 6520 3d20 2873 697a 652c 2073 697a 6532  e = (size, size2
-00000d50: 290d 0a20 2020 2020 2020 2065 6c69 6620  )..        elif 
-00000d60: 696d 672e 7769 6474 6820 3d3d 2069 6d67  img.width == img
-00000d70: 2e68 6569 6768 743a 0d0a 2020 2020 2020  .height:..      
-00000d80: 2020 2020 2020 7369 7a65 203d 2028 7369        size = (si
-00000d90: 7a65 2c20 7369 7a65 290d 0a20 2020 2020  ze, size)..     
-00000da0: 2020 2065 6c69 6620 696d 672e 7769 6474     elif img.widt
-00000db0: 6820 3c20 696d 672e 6865 6967 6874 3a0d  h < img.height:.
-00000dc0: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
-00000dd0: 6520 3d20 286d 6178 2873 697a 6520 2a20  e = (max(size * 
-00000de0: 696d 672e 7769 6474 6820 2f2f 2069 6d67  img.width // img
-00000df0: 2e68 6569 6768 742c 2031 292c 2073 697a  .height, 1), siz
-00000e00: 6529 0d0a 2020 2020 2020 2020 656c 7365  e)..        else
-00000e10: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00000e20: 697a 6520 3d20 2873 697a 652c 206d 6178  ize = (size, max
-00000e30: 2873 697a 6520 2a20 696d 672e 6865 6967  (size * img.heig
-00000e40: 6874 202f 2f20 696d 672e 7769 6474 682c  ht // img.width,
-00000e50: 2031 2929 0d0a 0d0a 2020 2020 2020 2020   1))....        
-00000e60: 696d 672e 7265 7369 7a65 2873 697a 6529  img.resize(size)
-00000e70: 2e73 6176 6528 6f75 7470 7574 2c20 696d  .save(output, im
-00000e80: 675f 7479 7065 290d 0a0d 0a20 2020 2072  g_type)....    r
-00000e90: 6574 7572 6e20 6f75 7470 7574 0d0a 0d0a  eturn output....
-00000ea0: 0d0a 6465 6620 7061 7273 655f 6d65 7461  ..def parse_meta
-00000eb0: 5f63 6f6d 6d65 6e74 7328 636f 6465 3a20  _comments(code: 
-00000ec0: 7374 7229 202d 3e20 4469 6374 5b73 7472  str) -> Dict[str
-00000ed0: 2c20 7374 725d 3a0d 0a20 2020 2074 7279  , str]:..    try
-00000ee0: 3a0d 0a20 2020 2020 2020 2067 726f 7570  :..        group
-00000ef0: 7320 3d20 4d45 5441 5f43 4f4d 4d45 4e54  s = META_COMMENT
-00000f00: 532e 7365 6172 6368 2863 6f64 6529 2e67  S.search(code).g
-00000f10: 726f 7570 7328 290d 0a20 2020 2065 7863  roups()..    exc
-00000f20: 6570 7420 4174 7472 6962 7574 6545 7272  ept AttributeErr
-00000f30: 6f72 3a0d 0a20 2020 2020 2020 2072 6574  or:..        ret
-00000f40: 7572 6e20 7b7d 0d0a 0d0a 2020 2020 7265  urn {}....    re
-00000f50: 7475 726e 207b 6772 6f75 7073 5b69 5d3a  turn {groups[i]:
-00000f60: 2067 726f 7570 735b 6920 2b20 315d 2066   groups[i + 1] f
-00000f70: 6f72 2069 2069 6e20 7261 6e67 6528 302c  or i in range(0,
-00000f80: 206c 656e 2867 726f 7570 7329 2c20 3229   len(groups), 2)
-00000f90: 7d0d 0a0d 0a61 7379 6e63 2064 6566 2072  }....async def r
-00000fa0: 6d5f 6d61 726b 646f 776e 2874 6578 743a  m_markdown(text:
-00000fb0: 2073 7472 293a 0d0a 2020 2020 2252 656d   str):..    "Rem
-00000fc0: 6f76 6520 6261 7369 6320 6d61 726b 646f  ove basic markdo
-00000fd0: 776e 2073 796e 7461 7820 6672 6f6d 2061  wn syntax from a
-00000fe0: 2073 7472 696e 6722 0d0a 2020 2020 726d   string"..    rm
-00000ff0: 6564 203d 2072 652e 7375 6228 225b 2a60  ed = re.sub("[*`
-00001000: 5f5d 222c 2022 222c 2074 6578 7429 0d0a  _]", "", text)..
-00001010: 2020 2020 7265 7475 726e 2072 6d65 64        return rmed
+00000000: 696d 706f 7274 2061 7379 6e63 696f 0d0a  import asyncio..
+00000010: 696d 706f 7274 2072 650d 0a69 6d70 6f72  import re..impor
+00000020: 7420 7472 6163 6562 6163 6b0d 0a66 726f  t traceback..fro
+00000030: 6d20 696f 2069 6d70 6f72 7420 4279 7465  m io import Byte
+00000040: 7349 4f0d 0a66 726f 6d20 7479 7069 6e67  sIO..from typing
+00000050: 2069 6d70 6f72 7420 4469 6374 0d0a 0d0a   import Dict....
+00000060: 6672 6f6d 2050 494c 2069 6d70 6f72 7420  from PIL import 
+00000070: 496d 6167 650d 0a66 726f 6d20 7079 726f  Image..from pyro
+00000080: 6772 616d 2069 6d70 6f72 7420 436c 6965  gram import Clie
+00000090: 6e74 2c20 6572 726f 7273 2c20 7479 7065  nt, errors, type
+000000a0: 730d 0a0d 0a4d 4554 415f 434f 4d4d 454e  s....META_COMMEN
+000000b0: 5453 203d 2072 652e 636f 6d70 696c 6528  TS = re.compile(
+000000c0: 7222 5e20 2a23 202a 6d65 7461 202b 285c  r"^ *# *meta +(\
+000000d0: 532b 2920 2a3a 202a 282e 2a3f 295c 732a  S+) *: *(.*?)\s*
+000000e0: 2422 2c20 7265 2e4d 554c 5449 4c49 4e45  $", re.MULTILINE
+000000f0: 290d 0a0d 0a69 6e74 6572 6163 745f 7769  )....interact_wi
+00000100: 7468 5f74 6f5f 6465 6c65 7465 203d 205b  th_to_delete = [
+00000110: 5d0d 0a0d 0a0d 0a64 6566 2074 6578 7428  ]......def text(
+00000120: 6d65 7373 6167 653a 2074 7970 6573 2e4d  message: types.M
+00000130: 6573 7361 6765 2920 2d3e 2073 7472 3a0d  essage) -> str:.
+00000140: 0a20 2020 2022 2222 4669 6e64 2074 6578  .    """Find tex
+00000150: 7420 696e 2060 7479 7065 732e 4d65 7373  t in `types.Mess
+00000160: 6167 6560 206f 626a 6563 7422 2222 0d0a  age` object"""..
+00000170: 0d0a 2020 2020 7265 7475 726e 206d 6573  ..    return mes
+00000180: 7361 6765 2e74 6578 7420 6966 206d 6573  sage.text if mes
+00000190: 7361 6765 2e74 6578 7420 656c 7365 206d  sage.text else m
+000001a0: 6573 7361 6765 2e63 6170 7469 6f6e 0d0a  essage.caption..
+000001b0: 0d0a 0d0a 6173 796e 6320 6465 6620 6165  ....async def ae
+000001c0: 7865 6328 636f 6465 2c20 632c 206d 293a  xec(code, c, m):
+000001d0: 0d0a 2020 2020 6578 6563 2822 6173 796e  ..    exec("asyn
+000001e0: 6320 6465 6620 5f5f 6165 7865 6328 632c  c def __aexec(c,
+000001f0: 206d 293a 2022 202b 2022 222e 6a6f 696e   m): " + "".join
+00000200: 2866 225c 6e20 7b6c 5f7d 2220 666f 7220  (f"\n {l_}" for 
+00000210: 6c5f 2069 6e20 636f 6465 2e73 706c 6974  l_ in code.split
+00000220: 2822 5c6e 2229 2929 0d0a 0d0a 2020 2020  ("\n")))....    
+00000230: 7265 7475 726e 2061 7761 6974 206c 6f63  return await loc
+00000240: 616c 7328 295b 225f 5f61 6578 6563 225d  als()["__aexec"]
+00000250: 2863 2c20 6d29 0d0a 0d0a 0d0a 6173 796e  (c, m)......asyn
+00000260: 6320 6465 6620 7368 656c 6c5f 6578 6563  c def shell_exec
+00000270: 2863 6f64 652c 2074 7265 6174 3d54 7275  (code, treat=Tru
+00000280: 6529 3a0d 0a20 2020 2070 726f 6365 7373  e):..    process
+00000290: 203d 2061 7761 6974 2061 7379 6e63 696f   = await asyncio
+000002a0: 2e63 7265 6174 655f 7375 6270 726f 6365  .create_subproce
+000002b0: 7373 5f73 6865 6c6c 280d 0a20 2020 2020  ss_shell(..     
+000002c0: 2020 2063 6f64 652c 2073 7464 6f75 743d     code, stdout=
+000002d0: 6173 796e 6369 6f2e 7375 6270 726f 6365  asyncio.subproce
+000002e0: 7373 2e50 4950 452c 2073 7464 6572 723d  ss.PIPE, stderr=
+000002f0: 6173 796e 6369 6f2e 7375 6270 726f 6365  asyncio.subproce
+00000300: 7373 2e53 5444 4f55 540d 0a20 2020 2029  ss.STDOUT..    )
+00000310: 0d0a 0d0a 2020 2020 7374 646f 7574 203d  ....    stdout =
+00000320: 2028 6177 6169 7420 7072 6f63 6573 732e   (await process.
+00000330: 636f 6d6d 756e 6963 6174 6528 2929 5b30  communicate())[0
+00000340: 5d0d 0a0d 0a20 2020 2069 6620 7472 6561  ]....    if trea
+00000350: 743a 0d0a 2020 2020 2020 2020 7374 646f  t:..        stdo
+00000360: 7574 203d 2073 7464 6f75 742e 6465 636f  ut = stdout.deco
+00000370: 6465 2829 2e73 7472 6970 2829 0d0a 0d0a  de().strip()....
+00000380: 2020 2020 7265 7475 726e 2073 7464 6f75      return stdou
+00000390: 742c 2070 726f 6365 7373 0d0a 0d0a 0d0a  t, process......
+000003a0: 6465 6620 666f 726d 6174 5f65 7863 2865  def format_exc(e
+000003b0: 3a20 4578 6365 7074 696f 6e2c 2073 7566  : Exception, suf
+000003c0: 6669 783d 2222 2920 2d3e 2073 7472 3a0d  fix="") -> str:.
+000003d0: 0a20 2020 2074 7261 6365 6261 636b 2e70  .    traceback.p
+000003e0: 7269 6e74 5f65 7863 2829 0d0a 0d0a 2020  rint_exc()....  
+000003f0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00000400: 652c 2065 7272 6f72 732e 5250 4345 7272  e, errors.RPCErr
+00000410: 6f72 293a 0d0a 2020 2020 2020 2020 7265  or):..        re
+00000420: 7475 726e 2028 0d0a 2020 2020 2020 2020  turn (..        
+00000430: 2020 2020 6622 3c62 3e54 656c 6567 7261      f"<b>Telegra
+00000440: 6d20 4150 4920 6572 726f 7221 3c2f 623e  m API error!</b>
+00000450: 5c6e 220d 0a20 2020 2020 2020 2020 2020  \n"..           
+00000460: 2066 223c 636f 6465 3e5b 7b65 2e43 4f44   f"<code>[{e.COD
+00000470: 457d 207b 652e 4944 206f 7220 652e 4e41  E} {e.ID or e.NA
+00000480: 4d45 7d5d 20e2 8094 207b 652e 4d45 5353  ME}] ... {e.MESS
+00000490: 4147 452e 666f 726d 6174 2876 616c 7565  AGE.format(value
+000004a0: 3d65 2e76 616c 7565 297d 3c2f 636f 6465  =e.value)}</code
+000004b0: 3e5c 6e5c 6e3c 623e 7b73 7566 6669 787d  >\n\n<b>{suffix}
+000004c0: 3c2f 623e 220d 0a20 2020 2020 2020 2029  </b>"..        )
+000004d0: 0d0a 0d0a 2020 2020 7265 7475 726e 2028  ....    return (
+000004e0: 0d0a 2020 2020 2020 2020 6622 3c62 3e45  ..        f"<b>E
+000004f0: 7272 6f72 213c 2f62 3e5c 6e22 0d0a 2020  rror!</b>\n"..  
+00000500: 2020 2020 2020 6622 3c63 6f64 653e 7b65        f"<code>{e
+00000510: 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e 616d  .__class__.__nam
+00000520: 655f 5f7d 3a20 7b65 7d3c 2f63 6f64 653e  e__}: {e}</code>
+00000530: 5c6e 5c6e 3c62 3e7b 7375 6666 6978 7d3c  \n\n<b>{suffix}<
+00000540: 2f62 3e22 0d0a 2020 2020 290d 0a0d 0a0d  /b>"..    ).....
+00000550: 0a64 6566 2077 6974 685f 7265 706c 7928  .def with_reply(
+00000560: 6675 6e63 293a 0d0a 2020 2020 6173 796e  func):..    asyn
+00000570: 6320 6465 6620 7772 6170 7065 6428 636c  c def wrapped(cl
+00000580: 6965 6e74 3a20 436c 6965 6e74 2c20 6d65  ient: Client, me
+00000590: 7373 6167 653a 2074 7970 6573 2e4d 6573  ssage: types.Mes
+000005a0: 7361 6765 293a 0d0a 2020 2020 2020 2020  sage):..        
+000005b0: 6966 206e 6f74 206d 6573 7361 6765 2e72  if not message.r
+000005c0: 6570 6c79 5f74 6f5f 6d65 7373 6167 653a  eply_to_message:
+000005d0: 0d0a 2020 2020 2020 2020 2020 2020 6177  ..            aw
+000005e0: 6169 7420 6d65 7373 6167 652e 6564 6974  ait message.edit
+000005f0: 2822 3c62 3e52 6570 6c79 2074 6f20 6d65  ("<b>Reply to me
+00000600: 7373 6167 6520 6973 2072 6571 7569 7265  ssage is require
+00000610: 643c 2f62 3e22 290d 0a0d 0a20 2020 2020  d</b>")....     
+00000620: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00000630: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
+00000640: 6974 2066 756e 6328 636c 6965 6e74 2c20  it func(client, 
+00000650: 6d65 7373 6167 6529 0d0a 0d0a 2020 2020  message)....    
+00000660: 7265 7475 726e 2077 7261 7070 6564 0d0a  return wrapped..
+00000670: 0d0a 0d0a 6173 796e 6320 6465 6620 696e  ....async def in
+00000680: 7465 7261 6374 5f77 6974 6828 6d65 7373  teract_with(mess
+00000690: 6167 653a 2074 7970 6573 2e4d 6573 7361  age: types.Messa
+000006a0: 6765 2920 2d3e 2074 7970 6573 2e4d 6573  ge) -> types.Mes
+000006b0: 7361 6765 3a0d 0a20 2020 2022 2222 0d0a  sage:..    """..
+000006c0: 0d0a 2020 2020 4368 6563 6b20 6869 7374  ..    Check hist
+000006d0: 6f72 7920 7769 7468 2062 6f74 2061 6e64  ory with bot and
+000006e0: 2072 6574 7572 6e20 626f 7427 7320 7265   return bot's re
+000006f0: 7370 6f6e 7365 0d0a 0d0a 0d0a 0d0a 2020  sponse........  
+00000700: 2020 4578 616d 706c 653a 0d0a 0d0a 2020    Example:....  
+00000710: 2020 2e2e 2063 6f64 652d 626c 6f63 6b3a    .. code-block:
+00000720: 3a20 7079 7468 6f6e 0d0a 0d0a 2020 2020  : python....    
+00000730: 2020 2020 626f 745f 6d73 6720 3d20 6177      bot_msg = aw
+00000740: 6169 7420 696e 7465 7261 6374 5f77 6974  ait interact_wit
+00000750: 6828 6177 6169 7420 626f 742e 7365 6e64  h(await bot.send
+00000760: 5f6d 6573 7361 6765 2822 4042 6f74 4661  _message("@BotFa
+00000770: 7468 6572 222c 2022 2f73 7461 7274 2229  ther", "/start")
+00000780: 290d 0a0d 0a20 2020 203a 7061 7261 6d20  )....    :param 
+00000790: 6d65 7373 6167 653a 2061 6c72 6561 6479  message: already
+000007a0: 2073 656e 7420 6d65 7373 6167 6520 746f   sent message to
+000007b0: 2062 6f74 0d0a 0d0a 2020 2020 3a72 6574   bot....    :ret
+000007c0: 7572 6e3a 2062 6f74 2773 2072 6573 706f  urn: bot's respo
+000007d0: 6e73 650d 0a0d 0a20 2020 2022 2222 0d0a  nse....    """..
+000007e0: 0d0a 2020 2020 6177 6169 7420 6173 796e  ..    await asyn
+000007f0: 6369 6f2e 736c 6565 7028 3129 0d0a 0d0a  cio.sleep(1)....
+00000800: 2020 2020 2320 6e6f 696e 7370 6563 7469      # noinspecti
+00000810: 6f6e 2050 7950 726f 7465 6374 6564 4d65  on PyProtectedMe
+00000820: 6d62 6572 0d0a 0d0a 2020 2020 7265 7370  mber....    resp
+00000830: 6f6e 7365 203d 205b 0d0a 2020 2020 2020  onse = [..      
+00000840: 2020 6d73 6720 6173 796e 6320 666f 7220    msg async for 
+00000850: 6d73 6720 696e 206d 6573 7361 6765 2e5f  msg in message._
+00000860: 636c 6965 6e74 2e67 6574 5f63 6861 745f  client.get_chat_
+00000870: 6869 7374 6f72 7928 6d65 7373 6167 652e  history(message.
+00000880: 6368 6174 2e69 642c 206c 696d 6974 3d31  chat.id, limit=1
+00000890: 290d 0a20 2020 205d 0d0a 0d0a 2020 2020  )..    ]....    
+000008a0: 7365 636f 6e64 735f 7761 6974 696e 6720  seconds_waiting 
+000008b0: 3d20 300d 0a0d 0a20 2020 2077 6869 6c65  = 0....    while
+000008c0: 2072 6573 706f 6e73 655b 305d 2e66 726f   response[0].fro
+000008d0: 6d5f 7573 6572 2e69 735f 7365 6c66 3a0d  m_user.is_self:.
+000008e0: 0a20 2020 2020 2020 2073 6563 6f6e 6473  .        seconds
+000008f0: 5f77 6169 7469 6e67 202b 3d20 310d 0a0d  _waiting += 1...
+00000900: 0a20 2020 2020 2020 2069 6620 7365 636f  .        if seco
+00000910: 6e64 735f 7761 6974 696e 6720 3e3d 2035  nds_waiting >= 5
+00000920: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00000930: 6169 7365 2052 756e 7469 6d65 4572 726f  aise RuntimeErro
+00000940: 7228 2262 6f74 2064 6964 6e27 7420 616e  r("bot didn't an
+00000950: 7377 6572 2069 6e20 3520 7365 636f 6e64  swer in 5 second
+00000960: 7322 290d 0a0d 0a20 2020 2020 2020 2061  s")....        a
+00000970: 7761 6974 2061 7379 6e63 696f 2e73 6c65  wait asyncio.sle
+00000980: 6570 2831 290d 0a0d 0a20 2020 2020 2020  ep(1)....       
+00000990: 2023 206e 6f69 6e73 7065 6374 696f 6e20   # noinspection 
+000009a0: 5079 5072 6f74 6563 7465 644d 656d 6265  PyProtectedMembe
+000009b0: 720d 0a0d 0a20 2020 2020 2020 2072 6573  r....        res
+000009c0: 706f 6e73 6520 3d20 5b0d 0a20 2020 2020  ponse = [..     
+000009d0: 2020 2020 2020 206d 7367 0d0a 2020 2020         msg..    
+000009e0: 2020 2020 2020 2020 6173 796e 6320 666f          async fo
+000009f0: 7220 6d73 6720 696e 206d 6573 7361 6765  r msg in message
+00000a00: 2e5f 636c 6965 6e74 2e67 6574 5f63 6861  ._client.get_cha
+00000a10: 745f 6869 7374 6f72 7928 6d65 7373 6167  t_history(messag
+00000a20: 652e 6368 6174 2e69 642c 206c 696d 6974  e.chat.id, limit
+00000a30: 3d31 290d 0a20 2020 2020 2020 205d 0d0a  =1)..        ]..
+00000a40: 0d0a 2020 2020 696e 7465 7261 6374 5f77  ..    interact_w
+00000a50: 6974 685f 746f 5f64 656c 6574 652e 6170  ith_to_delete.ap
+00000a60: 7065 6e64 286d 6573 7361 6765 2e69 6429  pend(message.id)
+00000a70: 0d0a 0d0a 2020 2020 696e 7465 7261 6374  ....    interact
+00000a80: 5f77 6974 685f 746f 5f64 656c 6574 652e  _with_to_delete.
+00000a90: 6170 7065 6e64 2872 6573 706f 6e73 655b  append(response[
+00000aa0: 305d 2e69 6429 0d0a 0d0a 2020 2020 7265  0].id)....    re
+00000ab0: 7475 726e 2072 6573 706f 6e73 655b 305d  turn response[0]
+00000ac0: 0d0a 0d0a 0d0a 6465 6620 7265 7369 7a65  ......def resize
+00000ad0: 5f69 6d61 6765 280d 0a20 2020 2069 6e70  _image(..    inp
+00000ae0: 7574 5f69 6d67 2c20 6f75 7470 7574 3d4e  ut_img, output=N
+00000af0: 6f6e 652c 2069 6d67 5f74 7970 653d 2250  one, img_type="P
+00000b00: 4e47 222c 2073 697a 653a 2069 6e74 203d  NG", size: int =
+00000b10: 2035 3132 2c20 7369 7a65 323a 2069 6e74   512, size2: int
+00000b20: 203d 204e 6f6e 650d 0a29 3a0d 0a20 2020   = None..):..   
+00000b30: 2069 6620 6f75 7470 7574 2069 7320 4e6f   if output is No
+00000b40: 6e65 3a0d 0a20 2020 2020 2020 206f 7574  ne:..        out
+00000b50: 7075 7420 3d20 4279 7465 7349 4f28 290d  put = BytesIO().
+00000b60: 0a0d 0a20 2020 2020 2020 206f 7574 7075  ...        outpu
+00000b70: 742e 6e61 6d65 203d 2066 2273 7469 636b  t.name = f"stick
+00000b80: 6572 2e7b 696d 675f 7479 7065 2e6c 6f77  er.{img_type.low
+00000b90: 6572 2829 7d22 0d0a 0d0a 2020 2020 7769  er()}"....    wi
+00000ba0: 7468 2049 6d61 6765 2e6f 7065 6e28 696e  th Image.open(in
+00000bb0: 7075 745f 696d 6729 2061 7320 696d 673a  put_img) as img:
+00000bc0: 0d0a 2020 2020 2020 2020 2320 5765 2075  ..        # We u
+00000bd0: 7365 6420 746f 2075 7365 2074 6875 6d62  sed to use thumb
+00000be0: 6e61 696c 2873 697a 6529 2068 6572 652c  nail(size) here,
+00000bf0: 2062 7574 2069 7420 7265 7475 726e 7320   but it returns 
+00000c00: 7769 7468 2061 202a 6d61 782a 2064 696d  with a *max* dim
+00000c10: 656e 7369 6f6e 206f 6620 3531 322c 3531  ension of 512,51
+00000c20: 320d 0a0d 0a20 2020 2020 2020 2023 2072  2....        # r
+00000c30: 6174 6865 7220 7468 616e 206d 616b 696e  ather than makin
+00000c40: 6720 6f6e 6520 7369 6465 2065 7861 6374  g one side exact
+00000c50: 6c79 2035 3132 2c20 736f 2077 6520 6861  ly 512, so we ha
+00000c60: 7665 2074 6f20 6361 6c63 756c 6174 6520  ve to calculate 
+00000c70: 6469 6d65 6e73 696f 6e73 206d 616e 7561  dimensions manua
+00000c80: 6c6c 7920 3a28 0d0a 0d0a 2020 2020 2020  lly :(....      
+00000c90: 2020 6966 2073 697a 6532 2069 7320 6e6f    if size2 is no
+00000ca0: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+00000cb0: 2020 2020 2073 697a 6520 3d20 2873 697a       size = (siz
+00000cc0: 652c 2073 697a 6532 290d 0a0d 0a20 2020  e, size2)....   
+00000cd0: 2020 2020 2065 6c69 6620 696d 672e 7769       elif img.wi
+00000ce0: 6474 6820 3d3d 2069 6d67 2e68 6569 6768  dth == img.heigh
+00000cf0: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
+00000d00: 7369 7a65 203d 2028 7369 7a65 2c20 7369  size = (size, si
+00000d10: 7a65 290d 0a0d 0a20 2020 2020 2020 2065  ze)....        e
+00000d20: 6c69 6620 696d 672e 7769 6474 6820 3c20  lif img.width < 
+00000d30: 696d 672e 6865 6967 6874 3a0d 0a20 2020  img.height:..   
+00000d40: 2020 2020 2020 2020 2073 697a 6520 3d20           size = 
+00000d50: 286d 6178 2873 697a 6520 2a20 696d 672e  (max(size * img.
+00000d60: 7769 6474 6820 2f2f 2069 6d67 2e68 6569  width // img.hei
+00000d70: 6768 742c 2031 292c 2073 697a 6529 0d0a  ght, 1), size)..
+00000d80: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
+00000d90: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
+00000da0: 6520 3d20 2873 697a 652c 206d 6178 2873  e = (size, max(s
+00000db0: 697a 6520 2a20 696d 672e 6865 6967 6874  ize * img.height
+00000dc0: 202f 2f20 696d 672e 7769 6474 682c 2031   // img.width, 1
+00000dd0: 2929 0d0a 0d0a 2020 2020 2020 2020 696d  ))....        im
+00000de0: 672e 7265 7369 7a65 2873 697a 6529 2e73  g.resize(size).s
+00000df0: 6176 6528 6f75 7470 7574 2c20 696d 675f  ave(output, img_
+00000e00: 7479 7065 290d 0a0d 0a20 2020 2072 6574  type)....    ret
+00000e10: 7572 6e20 6f75 7470 7574 0d0a 0d0a 0d0a  urn output......
+00000e20: 6465 6620 7061 7273 655f 6d65 7461 5f63  def parse_meta_c
+00000e30: 6f6d 6d65 6e74 7328 636f 6465 3a20 7374  omments(code: st
+00000e40: 7229 202d 3e20 4469 6374 5b73 7472 2c20  r) -> Dict[str, 
+00000e50: 7374 725d 3a0d 0a20 2020 2074 7279 3a0d  str]:..    try:.
+00000e60: 0a20 2020 2020 2020 2067 726f 7570 7320  .        groups 
+00000e70: 3d20 4d45 5441 5f43 4f4d 4d45 4e54 532e  = META_COMMENTS.
+00000e80: 7365 6172 6368 2863 6f64 6529 2e67 726f  search(code).gro
+00000e90: 7570 7328 290d 0a0d 0a20 2020 2065 7863  ups()....    exc
+00000ea0: 6570 7420 4174 7472 6962 7574 6545 7272  ept AttributeErr
+00000eb0: 6f72 3a0d 0a20 2020 2020 2020 2072 6574  or:..        ret
+00000ec0: 7572 6e20 7b7d 0d0a 0d0a 2020 2020 7265  urn {}....    re
+00000ed0: 7475 726e 207b 6772 6f75 7073 5b69 5d3a  turn {groups[i]:
+00000ee0: 2067 726f 7570 735b 6920 2b20 315d 2066   groups[i + 1] f
+00000ef0: 6f72 2069 2069 6e20 7261 6e67 6528 302c  or i in range(0,
+00000f00: 206c 656e 2867 726f 7570 7329 2c20 3229   len(groups), 2)
+00000f10: 7d0d 0a0d 0a0d 0a61 7379 6e63 2064 6566  }......async def
+00000f20: 2072 6d5f 6d61 726b 646f 776e 2874 6578   rm_markdown(tex
+00000f30: 743a 2073 7472 293a 0d0a 2020 2020 2252  t: str):..    "R
+00000f40: 656d 6f76 6520 6261 7369 6320 6d61 726b  emove basic mark
+00000f50: 646f 776e 2073 796e 7461 7820 6672 6f6d  down syntax from
+00000f60: 2061 2073 7472 696e 6722 0d0a 0d0a 2020   a string"....  
+00000f70: 2020 726d 6564 203d 2072 652e 7375 6228    rmed = re.sub(
+00000f80: 225b 2a60 5f5d 222c 2022 222c 2074 6578  "[*`_]", "", tex
+00000f90: 7429 0d0a 0d0a 2020 2020 7265 7475 726e  t)....    return
+00000fa0: 2072 6d65 640d 0a                         rmed..
```

### Comparing `kynaylibs-7.0.3/kynaylibs.egg-info/PKG-INFO` & `kynaylibs-7.0.4/kynaylibs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kynaylibs
-Version: 7.0.3
+Version: 7.0.4
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `kynaylibs-7.0.3/kynaylibs.egg-info/SOURCES.txt` & `kynaylibs-7.0.4/kynaylibs.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 kynaylibs/__init__.py
+kynaylibs/__main__.py
+kynaylibs/config.py
+kynaylibs/logging.py
 kynaylibs/version.py
 kynaylibs.egg-info/PKG-INFO
 kynaylibs.egg-info/SOURCES.txt
 kynaylibs.egg-info/dependency_links.txt
 kynaylibs.egg-info/requires.txt
 kynaylibs.egg-info/top_level.txt
-kynaylibs/core/__init__.py
-kynaylibs/core/ai.py
-kynaylibs/core/constants.py
-kynaylibs/core/cos_cmd.py
-kynaylibs/core/data.py
-kynaylibs/core/filter.py
-kynaylibs/core/func.py
-kynaylibs/core/inline.py
-kynaylibs/core/lgs.py
-kynaylibs/core/what.py
-kynaylibs/core/db/__init__.py
-kynaylibs/core/db/pmpermit.py
-kynaylibs/nan/__init__.py
+kynaylibs/nan/__init__.py
+kynaylibs/nan/utils/PyroHelpers.py
+kynaylibs/nan/utils/__init__.py
+kynaylibs/nan/utils/adminHelpers.py
+kynaylibs/nan/utils/ai.py
+kynaylibs/nan/utils/aiohttp_helper.py
+kynaylibs/nan/utils/basic.py
+kynaylibs/nan/utils/constants.py
+kynaylibs/nan/utils/function.py
+kynaylibs/nan/utils/inline.py
+kynaylibs/nan/utils/interval.py
+kynaylibs/nan/utils/misc.py
+kynaylibs/nan/utils/parser.py
+kynaylibs/nan/utils/pilter..py
+kynaylibs/nan/utils/tools.py
+kynaylibs/nan/utils/utility.py
+kynaylibs/nan/utils/db/__init__.py
+kynaylibs/nan/utils/db/permit.py
```

### Comparing `kynaylibs-7.0.3/setup.py` & `kynaylibs-7.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import re
-from sys import argv
 
 import setuptools
 
 with open("requirements.txt", encoding="utf-8") as r:
     requirements = [i.strip() for i in r]
 
-with open("kynaylibs/__init__.py", "rt", encoding="utf8") as x:
+with open("kynaylibs/version.py", "rt", encoding="utf8") as x:
     version = re.search(r'__version__ = "(.*?)"', x.read()).group(1)
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 name = "kynaylibs"
 author = "naya1503"
```

