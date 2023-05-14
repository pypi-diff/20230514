# Comparing `tmp/nonebot_plugin_bilibilibot-2.3.1.tar.gz` & `tmp/nonebot_plugin_bilibilibot-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilibilibot-2.3.1.tar", last modified: Mon Dec 26 03:39:37 2022, max compression
+gzip compressed data, was "nonebot_plugin_bilibilibot-2.3.2.tar", last modified: Sun May 14 05:46:11 2023, max compression
```

## Comparing `nonebot_plugin_bilibilibot-2.3.1.tar` & `nonebot_plugin_bilibilibot-2.3.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 tdk       (1004) tdk       (1004)        0 2022-12-26 03:39:37.377509 nonebot_plugin_bilibilibot-2.3.1/
--rw-rw-r--   0 tdk       (1004) tdk       (1004)    35149 2022-03-08 12:03:37.000000 nonebot_plugin_bilibilibot-2.3.1/LICENSE
--rw-rw-r--   0 tdk       (1004) tdk       (1004)       53 2022-04-15 09:07:46.000000 nonebot_plugin_bilibilibot-2.3.1/MANIFEST.in
--rw-rw-r--   0 tdk       (1004) tdk       (1004)     1230 2022-12-26 03:39:37.377509 nonebot_plugin_bilibilibot-2.3.1/PKG-INFO
--rw-rw-r--   0 tdk       (1004) tdk       (1004)      689 2022-04-17 08:31:02.000000 nonebot_plugin_bilibilibot-2.3.1/README.rst
-drwxrwxr-x   0 tdk       (1004) tdk       (1004)        0 2022-12-26 03:39:37.369509 nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/
--rw-rw-r--   0 tdk       (1004) tdk       (1004)    18711 2022-12-26 03:38:54.000000 nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/__init__.py
-drwxrwxr-x   0 tdk       (1004) tdk       (1004)        0 2022-12-26 03:39:37.373509 nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/bili_src/
--rw-rw-r--   0 tdk       (1004) tdk       (1004)     2736 2022-12-26 03:38:54.000000 nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/bili_src/basicFunc.py
--rw-rw-r--   0 tdk       (1004) tdk       (1004)     9007 2022-12-25 12:47:49.000000 nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/bili_src/biliStream.py
--rw-rw-r--   0 tdk       (1004) tdk       (1004)    10372 2022-12-26 03:38:54.000000 nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/bili_src/biliTelegram.py
--rw-rw-r--   0 tdk       (1004) tdk       (1004)     8853 2022-12-25 12:47:49.000000 nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/bili_src/biliVideo.py
--rw-rw-r--   0 tdk       (1004) tdk       (1004)    36038 2022-12-26 03:38:54.000000 nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/bili_src/bili_client.py
--rw-rw-r--   0 tdk       (1004) tdk       (1004)    13193 2022-12-25 12:47:49.000000 nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/bili_src/bili_dynamic.py
--rw-rw-r--   0 tdk       (1004) tdk       (1004)     8410 2022-12-25 13:05:59.000000 nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/bili_src/bili_dynamic_dbg.py
--rw-rw-r--   0 tdk       (1004) tdk       (1004)    26482 2022-12-26 03:38:54.000000 nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/bili_src/bili_task.py
--rw-rw-r--   0 tdk       (1004) tdk       (1004)    21245 2022-12-26 03:38:54.000000 nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/bili_src/db.py
--rw-rw-r--   0 tdk       (1004) tdk       (1004)     2594 2022-12-25 12:47:49.000000 nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/bili_src/exception.py
--rw-rw-r--   0 tdk       (1004) tdk       (1004)      707 2022-12-25 12:47:49.000000 nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/bili_src/rule.py
--rw-rw-r--   0 tdk       (1004) tdk       (1004)      168 2022-08-27 03:42:13.000000 nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/config.py
-drwxrwxr-x   0 tdk       (1004) tdk       (1004)        0 2022-12-26 03:39:37.365509 nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/file/
-drwxrwxr-x   0 tdk       (1004) tdk       (1004)        0 2022-12-26 03:39:37.377509 nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/file/source/
--rw-rw-r--   0 tdk       (1004) tdk       (1004)      109 2022-04-15 08:25:37.000000 nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/file/source/announcement.json
--rw-rw-r--   0 tdk       (1004) tdk       (1004)      811 2022-10-08 06:58:15.000000 nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/file/source/help.json
-drwxrwxr-x   0 tdk       (1004) tdk       (1004)        0 2022-12-26 03:39:37.369509 nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot.egg-info/
--rw-rw-r--   0 tdk       (1004) tdk       (1004)     1230 2022-12-26 03:39:37.000000 nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot.egg-info/PKG-INFO
--rw-rw-r--   0 tdk       (1004) tdk       (1004)     1013 2022-12-26 03:39:37.000000 nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot.egg-info/SOURCES.txt
--rw-rw-r--   0 tdk       (1004) tdk       (1004)        1 2022-12-26 03:39:37.000000 nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot.egg-info/dependency_links.txt
--rw-rw-r--   0 tdk       (1004) tdk       (1004)       56 2022-12-26 03:39:37.000000 nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot.egg-info/requires.txt
--rw-rw-r--   0 tdk       (1004) tdk       (1004)       27 2022-12-26 03:39:37.000000 nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot.egg-info/top_level.txt
--rw-rw-r--   0 tdk       (1004) tdk       (1004)       38 2022-12-26 03:39:37.377509 nonebot_plugin_bilibilibot-2.3.1/setup.cfg
--rw-rw-r--   0 tdk       (1004) tdk       (1004)      904 2022-12-26 03:39:11.000000 nonebot_plugin_bilibilibot-2.3.1/setup.py
+drwxrwxr-x   0 tdk       (1004) tdk       (1004)        0 2023-05-14 05:46:11.660836 nonebot_plugin_bilibilibot-2.3.2/
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)    35149 2022-03-08 12:03:37.000000 nonebot_plugin_bilibilibot-2.3.2/LICENSE
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)       53 2022-04-15 09:07:46.000000 nonebot_plugin_bilibilibot-2.3.2/MANIFEST.in
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)     1230 2023-05-14 05:46:11.660836 nonebot_plugin_bilibilibot-2.3.2/PKG-INFO
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)      689 2022-04-17 08:31:02.000000 nonebot_plugin_bilibilibot-2.3.2/README.rst
+drwxrwxr-x   0 tdk       (1004) tdk       (1004)        0 2023-05-14 05:46:11.656836 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)    18719 2023-05-14 05:42:08.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/__init__.py
+drwxrwxr-x   0 tdk       (1004) tdk       (1004)        0 2023-05-14 05:46:11.660836 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)     2736 2022-12-26 03:38:54.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/basicFunc.py
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)     9051 2023-05-14 05:42:08.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/biliStream.py
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)    10417 2023-05-14 05:42:08.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/biliTelegram.py
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)     8897 2023-05-14 05:42:08.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/biliVideo.py
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)    36042 2023-05-14 05:42:08.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/bili_client.py
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)    13242 2023-05-14 05:42:08.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/bili_dynamic.py
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)     8410 2022-12-25 13:05:59.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/bili_dynamic_dbg.py
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)    26482 2022-12-26 03:38:54.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/bili_task.py
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)    21245 2022-12-26 03:38:54.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/db.py
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)     2594 2022-12-25 12:47:49.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/exception.py
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)      707 2022-12-25 12:47:49.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/rule.py
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)      168 2022-08-27 03:42:13.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/config.py
+drwxrwxr-x   0 tdk       (1004) tdk       (1004)        0 2023-05-14 05:46:11.656836 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/file/
+drwxrwxr-x   0 tdk       (1004) tdk       (1004)        0 2023-05-14 05:46:11.660836 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/file/source/
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)      109 2022-04-15 08:25:37.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/file/source/announcement.json
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)      815 2023-05-14 05:42:08.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/file/source/help.json
+drwxrwxr-x   0 tdk       (1004) tdk       (1004)        0 2023-05-14 05:46:11.656836 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot.egg-info/
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)     1230 2023-05-14 05:46:11.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot.egg-info/PKG-INFO
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)     1013 2023-05-14 05:46:11.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot.egg-info/SOURCES.txt
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)        1 2023-05-14 05:46:11.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot.egg-info/dependency_links.txt
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)       56 2023-05-14 05:46:11.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot.egg-info/requires.txt
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)       27 2023-05-14 05:46:11.000000 nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot.egg-info/top_level.txt
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)       38 2023-05-14 05:46:11.660836 nonebot_plugin_bilibilibot-2.3.2/setup.cfg
+-rw-rw-r--   0 tdk       (1004) tdk       (1004)      904 2023-05-14 05:42:59.000000 nonebot_plugin_bilibilibot-2.3.2/setup.py
```

### Comparing `nonebot_plugin_bilibilibot-2.3.1/LICENSE` & `nonebot_plugin_bilibilibot-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilibilibot-2.3.1/PKG-INFO` & `nonebot_plugin_bilibilibot-2.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_bilibilibot
-Version: 2.3.1
+Version: 2.3.2
 Summary: 基于Nonebot的bilibili通知插件，可将up主，主播以及番剧的更新/直播动态推送到QQ
 Home-page: https://github.com/TDK1969/nonebot_plugin_bilibilibot
 Author: TDK
 Author-email: tdk1969@foxmail.com
 License: GNU
 Keywords: nonebot
 Platform: UNKNOWN
```

### Comparing `nonebot_plugin_bilibilibot-2.3.1/README.rst` & `nonebot_plugin_bilibilibot-2.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/__init__.py` & `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,15 +346,15 @@
     except BiliInvalidShortUrl:
         await follow_by_share_short_url.finish('关注失败: 非法或不支持的短链接')
     except Exception as _:
         ex_type, ex_val, _ = sys.exc_info()
         logger.error(f'{__PLUGIN_NAME}【错误报告】\n解析短链接 <{short_url}> 时发生错误\n错误类型: {ex_type}\n错误值: {ex_val}\n{traceback.format_exc()}')
         await follow_by_share_short_url.finish('关注失败: 连接错误')
 
-helpCommand = on_command("help", permission=ALL_PERMISSION, aliases={'帮助'})
+helpCommand = on_command("bilihelp", permission=ALL_PERMISSION, aliases={'B站帮助'})
 @helpCommand.handle()
 async def sendHelpMsg(event: MessageEvent):
     await create_user(event)
     helpMsg = ""
     with open(f'{PACKAGEPATH}/file/source/help.json', 'r', encoding='utf-8') as f:
         helpMsg = json.load(f)
     await helpCommand.finish(helpMsg)
```

### Comparing `nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/bili_src/basicFunc.py` & `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/basicFunc.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/bili_src/biliStream.py` & `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/biliStream.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     如果主播开播状态改变,则更新数据库
     ---------
     @param  :
     -------
     @Returns  :
     -------
     """
+    logger.debug("running check_bili_live")
     liver_list = list(bili_task_manager.liver_list.values())
     
     sched_bot = nonebot.get_bot()
     
     """results = await asyncio.gather(
         *[bili_client.get_live_status(liver_info[0], liver_info[3]) for liver_info in liver_list],
         return_exceptions=True
```

### Comparing `nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/bili_src/biliTelegram.py` & `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/biliTelegram.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     @param  :
     无
     -------
     @Returns  :
     无
     -------
     """
-    
+    logger.debug("running check_telegram_update")
     telegram_list = list(bili_task_manager.telegram_list.values())
     telegram_list = [i for i in telegram_list if i["is_finish"] is False]
     sched_bot = nonebot.get_bot()
     # 只对未完结的番剧进行检查
     results = await asyncio.gather(
         *[bili_client.get_telegram_latest_episode(telegram_info["season_id"], telegram_info["episode"]) for telegram_info in telegram_list],
         return_exceptions=True
```

### Comparing `nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/bili_src/biliVideo.py` & `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/biliVideo.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     检查关注UP主是否更新新视频，如果更新则通知用户并写入文件
     ---------
     @param  :
     -------
     @Returns  :
     -------
     """
+    logger.debug("running check_up_update")
     schedBot = nonebot.get_bot()
     #assert status == True, "数据库发生错误"
     check_up_list = bili_task_manager.get_up_check_update_list()
     #logger.debug(f'{__PLUGIN_NAME}check_up_list = {check_up_list}')
     
     results = await asyncio.gather(
         *[bili_client.get_latest_video(uid, bili_task_manager.up_list[uid]["latest_timestamp"]) for uid in check_up_list],
```

### Comparing `nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/bili_src/bili_client.py` & `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/bili_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,16 +64,16 @@
             "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_8_2) AppleWebKit/537.17 (KHTML, like Gecko) Chrome/24.0.1309.0 Safari/537.17"
         ]
         self.__usable_ip_list__ = set()
 
         self.API = {
             # 用于获取临时cookie
             "get_bili_cookie": "https://www.bilibili.com",
-            "get_user_info_by_uid": "https://api.bilibili.com/x/space/acc/info?mid={}&jsonp=jsonp",
-            "get_latest_video_by_uid": "https://api.bilibili.com/x/space/arc/search?mid={}&ps=1&tid=0&pn=1&order=pubdate&jsonp=jsonp",
+            "get_user_info_by_uid": "https://api.bilibili.com/x/space/wbi/acc/info?mid={}",
+            "get_latest_video_by_uid": "https://api.bilibili.com/x/space/wbi/arc/search?mid={}&ps=1&tid=0&pn=1&order=pubdate&jsonp=jsonp",
             "get_live_info_by_room_id": "https://api.live.bilibili.com/room/v1/Room/get_info?room_id={}",
             "get_liver_info_by_uid": "https://api.live.bilibili.com/live_user/v1/Master/info?uid={}",
             "get_telegram_info_by_media_id": "https://api.bilibili.com/pgc/review/user?media_id={}",
             "get_telegram_info_by_ep_id": "https://api.bilibili.com/pgc/view/web/season?ep_id={}",
             "get_telegram_info_by_season_id": "https://api.bilibili.com/pgc/view/web/season?season_id={}",
             "get_telegram_latest_episode": "https://api.bilibili.com/pgc/view/web/season?season_id={}",
             "get_dynamic_list_by_uid": "https://api.bilibili.com/x/polymer/web-dynamic/v1/feed/space?host_mid={}&timezone_offset=-480",
@@ -163,15 +163,15 @@
                 await client.get(self.API["get_bili_cookie"])
                 response1 = await client.get(url=self.API["get_user_info_by_uid"].format(uid))
             except Exception as e:
                 raise BiliConnectionError(0, uid, e.args[0])
 
             if response1.status_code != 200:
                 raise  BiliStatusCodeError(0, uid, response1.status_code)
-    
+            
             response1 = response1.json()
             if response1["code"] == -404:
                 raise BiliAPI404Error()
             elif response1["code"] != 0:
                 raise BiliAPIRetCodeError(0, uid, response1["code"], response1["message"])
             
             user_name = response1["data"]["name"]
```

### Comparing `nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/bili_src/bili_dynamic.py` & `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/bili_dynamic.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     检查关注动态主是否更新新视频，如果更新则通知用户并更新缓存和数据库
     ---------
     @param  :
     -------
     @Returns  :
     -------
     """
+    logger.debug("running check_dynamic_update")
     schedBot = nonebot.get_bot()
     check_dynamic_list = bili_task_manager.get_dynamic_check_update_list()
     #logger.debug(f'{__PLUGIN_NAME}check_dynamic_list = {check_dynamic_list}')
     
     results = await asyncio.gather(
         *[bili_client.get_latest_dynamic(
             uid,
```

### Comparing `nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/bili_src/bili_dynamic_dbg.py` & `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/bili_dynamic_dbg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/bili_src/bili_task.py` & `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/bili_task.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/bili_src/db.py` & `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/bili_src/exception.py` & `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/bili_src/rule.py` & `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/bili_src/rule.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot/file/source/help.json` & `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot/file/source/help.json`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-"命令列表:\n\n获取帮助\n> /help\n> /帮助\n\n关注主播\n> /关注主播 uid\n> 从B站app转发直播间(群不适用)\n\n取关主播\n> /切割主播 uid \n> /取关主播 uid\n\n关注up主\n> /关注up\n> 从B站app转发个人空间(群不适用)\n\n取关up主\n> /取关up主 uid\n\n关注番剧\n> /关注番剧 ep_id或season_id或media_id\n(番剧相关页面,url中以ep,ss,md开头的字符串)\n> 从B站app转发播放页面(推荐)(群不适用)\n\n\n取关番剧\n> /取关番剧 seasonid\n(seasonid: 与epid不同，请通过/查询关注 命令查看番剧的seasonid)\n\n查询关注\n> /查询关注\n> /查询成分\n\nAbout\n> 项目主页: https://github.com/TDK1969/nonebot_plugin_bilibilibot\n> 邮箱: tdk1969@foxmail.com\n> 出现问题请在github开issue或联系邮箱"
+"命令列表:\n\n获取帮助\n> /bilihelp\n> /帮助\n\n关注主播\n> /关注主播 uid\n> 从B站app转发直播间(群不适用)\n\n取关主播\n> /切割主播 uid \n> /取关主播 uid\n\n关注up主\n> /关注up\n> 从B站app转发个人空间(群不适用)\n\n取关up主\n> /取关up主 uid\n\n关注番剧\n> /关注番剧 ep_id或season_id或media_id\n(番剧相关页面,url中以ep,ss,md开头的字符串)\n> 从B站app转发播放页面(推荐)(群不适用)\n\n\n取关番剧\n> /取关番剧 seasonid\n(seasonid: 与epid不同，请通过/查询关注 命令查看番剧的seasonid)\n\n查询关注\n> /查询关注\n> /查询成分\n\nAbout\n> 项目主页: https://github.com/TDK1969/nonebot_plugin_bilibilibot\n> 邮箱: tdk1969@foxmail.com\n> 出现问题请在github开issue或联系邮箱"
```

### Comparing `nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot.egg-info/PKG-INFO` & `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilibilibot
-Version: 2.3.1
+Version: 2.3.2
 Summary: 基于Nonebot的bilibili通知插件，可将up主，主播以及番剧的更新/直播动态推送到QQ
 Home-page: https://github.com/TDK1969/nonebot_plugin_bilibilibot
 Author: TDK
 Author-email: tdk1969@foxmail.com
 License: GNU
 Keywords: nonebot
 Platform: UNKNOWN
```

### Comparing `nonebot_plugin_bilibilibot-2.3.1/nonebot_plugin_bilibilibot.egg-info/SOURCES.txt` & `nonebot_plugin_bilibilibot-2.3.2/nonebot_plugin_bilibilibot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilibilibot-2.3.1/setup.py` & `nonebot_plugin_bilibilibot-2.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import sys
 import os
 
 setup(
     name="nonebot_plugin_bilibilibot",
-    version="2.3.1",
+    version="2.3.2",
     author="TDK",
     author_email="tdk1969@foxmail.com",
     description="基于Nonebot的bilibili通知插件，可将up主，主播以及番剧的更新/直播动态推送到QQ",
     long_description=open("README.rst", "r").read(),
     include_package_data=True,
     license="GNU",
     url="https://github.com/TDK1969/nonebot_plugin_bilibilibot",
```

