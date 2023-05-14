# Comparing `tmp/chaanbot-3.1.0.tar.gz` & `tmp/chaanbot-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\chaanbot-3.1.0.tar", last modified: Sun May 14 14:07:25 2023, max compression
+gzip compressed data, was "dist\chaanbot-3.1.1.tar", last modified: Sun May 14 14:11:37 2023, max compression
```

## Comparing `chaanbot-3.1.0.tar` & `chaanbot-3.1.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 14:07:25.922562 chaanbot-3.1.0/
--rw-rw-rw-   0        0        0    35804 2020-01-04 14:14:41.000000 chaanbot-3.1.0/LICENSE
--rw-rw-rw-   0        0        0     3312 2023-05-14 14:07:25.922562 chaanbot-3.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2462 2023-05-14 13:45:28.000000 chaanbot-3.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 14:07:25.907508 chaanbot-3.1.0/chaanbot/
--rw-rw-rw-   0        0        0      140 2023-05-14 13:55:46.000000 chaanbot-3.1.0/chaanbot/__init__.py
--rw-rw-rw-   0        0        0     3885 2023-05-14 13:45:28.000000 chaanbot-3.1.0/chaanbot/client.py
--rw-rw-rw-   0        0        0     1677 2020-01-04 14:14:42.000000 chaanbot-3.1.0/chaanbot/command_utility.py
--rw-rw-rw-   0        0        0      271 2020-01-04 14:14:42.000000 chaanbot-3.1.0/chaanbot/database.py
--rw-rw-rw-   0        0        0     4618 2023-05-14 13:45:28.000000 chaanbot-3.1.0/chaanbot/matrix.py
--rw-rw-rw-   0        0        0     4488 2021-07-16 07:12:21.000000 chaanbot-3.1.0/chaanbot/module_loader.py
--rw-rw-rw-   0        0        0     1141 2023-05-14 13:45:28.000000 chaanbot-3.1.0/chaanbot/module_runner.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:07:25.914548 chaanbot-3.1.0/chaanbot/modules/
--rw-rw-rw-   0        0        0     1335 2023-05-14 14:06:39.000000 chaanbot-3.1.0/chaanbot/modules/RevAMP.py
--rw-rw-rw-   0        0        0        0 2020-01-04 14:14:42.000000 chaanbot-3.1.0/chaanbot/modules/__init__.py
--rw-rw-rw-   0        0        0     1067 2023-05-14 13:45:28.000000 chaanbot-3.1.0/chaanbot/modules/alive.py
--rw-rw-rw-   0        0        0     4353 2023-05-14 13:45:28.000000 chaanbot-3.1.0/chaanbot/modules/chan_save.py
--rw-rw-rw-   0        0        0    10965 2023-05-14 13:45:28.000000 chaanbot-3.1.0/chaanbot/modules/highlight.py
--rw-rw-rw-   0        0        0     1423 2023-05-14 13:45:28.000000 chaanbot-3.1.0/chaanbot/modules/rewrite_youtube_shorts.py
--rw-rw-rw-   0        0        0     2001 2023-05-14 13:45:28.000000 chaanbot-3.1.0/chaanbot/modules/twitter.py
--rw-rw-rw-   0        0        0     7722 2023-05-14 13:45:28.000000 chaanbot-3.1.0/chaanbot/modules/weather.py
--rw-rw-rw-   0        0        0     3163 2023-05-14 13:45:28.000000 chaanbot-3.1.0/chaanbot/start.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:07:25.910513 chaanbot-3.1.0/chaanbot.egg-info/
--rw-rw-rw-   0        0        0     3312 2023-05-14 14:07:25.000000 chaanbot-3.1.0/chaanbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      998 2023-05-14 14:07:25.000000 chaanbot-3.1.0/chaanbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 14:07:25.000000 chaanbot-3.1.0/chaanbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-05-14 14:07:25.000000 chaanbot-3.1.0/chaanbot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2023-05-14 14:07:25.000000 chaanbot-3.1.0/chaanbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-14 14:07:25.000000 chaanbot-3.1.0/chaanbot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 14:07:25.923565 chaanbot-3.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1944 2023-05-14 13:45:28.000000 chaanbot-3.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:07:25.922562 chaanbot-3.1.0/tests/
--rw-rw-rw-   0        0        0        0 2020-01-04 14:14:42.000000 chaanbot-3.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0     1559 2023-05-14 13:45:28.000000 chaanbot-3.1.0/tests/test_alive.py
--rw-rw-rw-   0        0        0     5393 2023-05-14 13:45:28.000000 chaanbot-3.1.0/tests/test_chan_save.py
--rw-rw-rw-   0        0        0     1692 2023-05-14 13:45:28.000000 chaanbot-3.1.0/tests/test_client.py
--rw-rw-rw-   0        0        0     3125 2020-01-04 14:14:42.000000 chaanbot-3.1.0/tests/test_command_utility.py
--rw-rw-rw-   0        0        0      351 2020-01-04 14:14:42.000000 chaanbot-3.1.0/tests/test_database.py
--rw-rw-rw-   0        0        0     7799 2023-05-14 13:45:28.000000 chaanbot-3.1.0/tests/test_highlight.py
--rw-rw-rw-   0        0        0     4802 2023-05-14 13:45:28.000000 chaanbot-3.1.0/tests/test_matrix.py
--rw-rw-rw-   0        0        0     5075 2020-01-04 14:14:42.000000 chaanbot-3.1.0/tests/test_module_loader.py
--rw-rw-rw-   0        0        0     2608 2023-05-14 13:45:28.000000 chaanbot-3.1.0/tests/test_module_runner.py
--rw-rw-rw-   0        0        0     1763 2023-05-14 14:04:40.000000 chaanbot-3.1.0/tests/test_revAMP.py
--rw-rw-rw-   0        0        0     2246 2023-05-14 13:45:28.000000 chaanbot-3.1.0/tests/test_rewrite_youtube_shorts.py
--rw-rw-rw-   0        0        0     2745 2023-05-14 13:45:28.000000 chaanbot-3.1.0/tests/test_start.py
--rw-rw-rw-   0        0        0     3134 2023-05-14 13:45:28.000000 chaanbot-3.1.0/tests/test_twitter.py
--rw-rw-rw-   0        0        0     7566 2023-05-14 13:45:28.000000 chaanbot-3.1.0/tests/test_weather.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:11:37.066560 chaanbot-3.1.1/
+-rw-rw-rw-   0        0        0    35804 2020-01-04 14:14:41.000000 chaanbot-3.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3312 2023-05-14 14:11:37.066560 chaanbot-3.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2462 2023-05-14 13:45:28.000000 chaanbot-3.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 14:11:37.050320 chaanbot-3.1.1/chaanbot/
+-rw-rw-rw-   0        0        0      140 2023-05-14 14:11:18.000000 chaanbot-3.1.1/chaanbot/__init__.py
+-rw-rw-rw-   0        0        0     3885 2023-05-14 13:45:28.000000 chaanbot-3.1.1/chaanbot/client.py
+-rw-rw-rw-   0        0        0     1677 2020-01-04 14:14:42.000000 chaanbot-3.1.1/chaanbot/command_utility.py
+-rw-rw-rw-   0        0        0      271 2020-01-04 14:14:42.000000 chaanbot-3.1.1/chaanbot/database.py
+-rw-rw-rw-   0        0        0     4618 2023-05-14 13:45:28.000000 chaanbot-3.1.1/chaanbot/matrix.py
+-rw-rw-rw-   0        0        0     4488 2021-07-16 07:12:21.000000 chaanbot-3.1.1/chaanbot/module_loader.py
+-rw-rw-rw-   0        0        0     1141 2023-05-14 13:45:28.000000 chaanbot-3.1.1/chaanbot/module_runner.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:11:37.058347 chaanbot-3.1.1/chaanbot/modules/
+-rw-rw-rw-   0        0        0     1335 2023-05-14 14:11:18.000000 chaanbot-3.1.1/chaanbot/modules/RevAMP.py
+-rw-rw-rw-   0        0        0        0 2020-01-04 14:14:42.000000 chaanbot-3.1.1/chaanbot/modules/__init__.py
+-rw-rw-rw-   0        0        0     1067 2023-05-14 13:45:28.000000 chaanbot-3.1.1/chaanbot/modules/alive.py
+-rw-rw-rw-   0        0        0     4353 2023-05-14 13:45:28.000000 chaanbot-3.1.1/chaanbot/modules/chan_save.py
+-rw-rw-rw-   0        0        0    10965 2023-05-14 13:45:28.000000 chaanbot-3.1.1/chaanbot/modules/highlight.py
+-rw-rw-rw-   0        0        0     1423 2023-05-14 13:45:28.000000 chaanbot-3.1.1/chaanbot/modules/rewrite_youtube_shorts.py
+-rw-rw-rw-   0        0        0     2001 2023-05-14 13:45:28.000000 chaanbot-3.1.1/chaanbot/modules/twitter.py
+-rw-rw-rw-   0        0        0     7722 2023-05-14 13:45:28.000000 chaanbot-3.1.1/chaanbot/modules/weather.py
+-rw-rw-rw-   0        0        0     3163 2023-05-14 14:10:08.000000 chaanbot-3.1.1/chaanbot/start.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:11:37.053330 chaanbot-3.1.1/chaanbot.egg-info/
+-rw-rw-rw-   0        0        0     3312 2023-05-14 14:11:36.000000 chaanbot-3.1.1/chaanbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1025 2023-05-14 14:11:36.000000 chaanbot-3.1.1/chaanbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 14:11:36.000000 chaanbot-3.1.1/chaanbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-14 14:11:36.000000 chaanbot-3.1.1/chaanbot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2023-05-14 14:11:36.000000 chaanbot-3.1.1/chaanbot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-14 14:11:36.000000 chaanbot-3.1.1/chaanbot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 14:11:37.066560 chaanbot-3.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1944 2023-05-14 13:45:28.000000 chaanbot-3.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:11:37.065557 chaanbot-3.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2020-01-04 14:14:42.000000 chaanbot-3.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     1559 2023-05-14 13:45:28.000000 chaanbot-3.1.1/tests/test_alive.py
+-rw-rw-rw-   0        0        0     5393 2023-05-14 13:45:28.000000 chaanbot-3.1.1/tests/test_chan_save.py
+-rw-rw-rw-   0        0        0     1692 2023-05-14 13:45:28.000000 chaanbot-3.1.1/tests/test_client.py
+-rw-rw-rw-   0        0        0     3125 2020-01-04 14:14:42.000000 chaanbot-3.1.1/tests/test_command_utility.py
+-rw-rw-rw-   0        0        0      351 2020-01-04 14:14:42.000000 chaanbot-3.1.1/tests/test_database.py
+-rw-rw-rw-   0        0        0     7799 2023-05-14 13:45:28.000000 chaanbot-3.1.1/tests/test_highlight.py
+-rw-rw-rw-   0        0        0     4802 2023-05-14 13:45:28.000000 chaanbot-3.1.1/tests/test_matrix.py
+-rw-rw-rw-   0        0        0     5075 2020-01-04 14:14:42.000000 chaanbot-3.1.1/tests/test_module_loader.py
+-rw-rw-rw-   0        0        0     2608 2023-05-14 13:45:28.000000 chaanbot-3.1.1/tests/test_module_runner.py
+-rw-rw-rw-   0        0        0     1763 2023-05-14 14:11:18.000000 chaanbot-3.1.1/tests/test_revAMP.py
+-rw-rw-rw-   0        0        0     2246 2023-05-14 13:45:28.000000 chaanbot-3.1.1/tests/test_rewrite_youtube_shorts.py
+-rw-rw-rw-   0        0        0     2745 2023-05-14 13:45:28.000000 chaanbot-3.1.1/tests/test_start.py
+-rw-rw-rw-   0        0        0     3134 2023-05-14 13:45:28.000000 chaanbot-3.1.1/tests/test_twitter.py
+-rw-rw-rw-   0        0        0     7566 2023-05-14 13:45:28.000000 chaanbot-3.1.1/tests/test_weather.py
```

### Comparing `chaanbot-3.1.0/LICENSE` & `chaanbot-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chaanbot-3.1.0/PKG-INFO` & `chaanbot-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaanbot
-Version: 3.1.0
+Version: 3.1.1
 Summary: A Matrix chat bot
 Home-page: https://github.com/RichardNysater/chaanbot
 Author: Richard Nysäter
 Author-email: richard@nysater.org
 License: GPLv3+
 Keywords: m,a,t,r,i,x, ,c,h,a,t, ,b,o,t
 Platform: UNKNOWN
```

### Comparing `chaanbot-3.1.0/README.md` & `chaanbot-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `chaanbot-3.1.0/chaanbot/client.py` & `chaanbot-3.1.1/chaanbot/client.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.1.0/chaanbot/command_utility.py` & `chaanbot-3.1.1/chaanbot/command_utility.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.1.0/chaanbot/matrix.py` & `chaanbot-3.1.1/chaanbot/matrix.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.1.0/chaanbot/module_loader.py` & `chaanbot-3.1.1/chaanbot/module_loader.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.1.0/chaanbot/module_runner.py` & `chaanbot-3.1.1/chaanbot/module_runner.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.1.0/chaanbot/modules/RevAMP.py` & `chaanbot-3.1.1/chaanbot/modules/RevAMP.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" The revAMP module turns AMP urls into normal URLS
+""" The revamp module turns AMP urls into normal URLS
 Available commands:
 None, will trigger on any AMP link.
 Usage example:
 [Xhark]: https://news.com/amp/russia-loses-ukraine-war
 Would results in:
 "Bot: https://news.com/russia-loses-ukraine-war"
 """
@@ -12,22 +12,22 @@
 
 from nio import RoomMessage, MatrixRoom
 
 from chaanbot.database import Database
 from chaanbot.matrix import Matrix
 
 
-class RevAMP:
+class Revamp:
     always_run = True  # Run on all messages, even if other modules has activated
     output_message_prefix = ""
 
     def __init__(self, config, matrix: Matrix, database: Database, requests):
         self.matrix = matrix
         self.requests = requests
-        self.output_message_prefix = config.get("revAMP", "prefix_message",
+        self.output_message_prefix = config.get("revamp", "prefix_message",
                                                 fallback="Fixed your link(s): ")
 
     async def run(self, room: MatrixRoom, event: RoomMessage, message) -> bool:
         links = re.findall(r"http[s]*://[^\s]+/amp/[^\s]+", message, re.IGNORECASE)
         hits = [link.replace("/amp/", "/") for link in links]
         if hits:
             msg = self.output_message_prefix + os.linesep.join(hits)
```

### Comparing `chaanbot-3.1.0/chaanbot/modules/alive.py` & `chaanbot-3.1.1/chaanbot/modules/alive.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.1.0/chaanbot/modules/chan_save.py` & `chaanbot-3.1.1/chaanbot/modules/chan_save.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.1.0/chaanbot/modules/highlight.py` & `chaanbot-3.1.1/chaanbot/modules/highlight.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.1.0/chaanbot/modules/rewrite_youtube_shorts.py` & `chaanbot-3.1.1/chaanbot/modules/rewrite_youtube_shorts.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.1.0/chaanbot/modules/twitter.py` & `chaanbot-3.1.1/chaanbot/modules/twitter.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.1.0/chaanbot/modules/weather.py` & `chaanbot-3.1.1/chaanbot/modules/weather.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.1.0/chaanbot/start.py` & `chaanbot-3.1.1/chaanbot/start.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.1.0/chaanbot.egg-info/PKG-INFO` & `chaanbot-3.1.1/chaanbot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaanbot
-Version: 3.1.0
+Version: 3.1.1
 Summary: A Matrix chat bot
 Home-page: https://github.com/RichardNysater/chaanbot
 Author: Richard Nysäter
 Author-email: richard@nysater.org
 License: GPLv3+
 Keywords: m,a,t,r,i,x, ,c,h,a,t, ,b,o,t
 Platform: UNKNOWN
```

### Comparing `chaanbot-3.1.0/chaanbot.egg-info/SOURCES.txt` & `chaanbot-3.1.1/chaanbot.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 chaanbot.egg-info/requires.txt
 chaanbot.egg-info/top_level.txt
 chaanbot/modules/RevAMP.py
 chaanbot/modules/__init__.py
 chaanbot/modules/alive.py
 chaanbot/modules/chan_save.py
 chaanbot/modules/highlight.py
+chaanbot/modules/revamp.py
 chaanbot/modules/rewrite_youtube_shorts.py
 chaanbot/modules/twitter.py
 chaanbot/modules/weather.py
 tests/__init__.py
 tests/test_alive.py
 tests/test_chan_save.py
 tests/test_client.py
```

### Comparing `chaanbot-3.1.0/setup.py` & `chaanbot-3.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.1.0/tests/test_alive.py` & `chaanbot-3.1.1/tests/test_alive.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.1.0/tests/test_chan_save.py` & `chaanbot-3.1.1/tests/test_chan_save.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.1.0/tests/test_client.py` & `chaanbot-3.1.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.1.0/tests/test_command_utility.py` & `chaanbot-3.1.1/tests/test_command_utility.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.1.0/tests/test_highlight.py` & `chaanbot-3.1.1/tests/test_highlight.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.1.0/tests/test_matrix.py` & `chaanbot-3.1.1/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.1.0/tests/test_module_loader.py` & `chaanbot-3.1.1/tests/test_module_loader.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.1.0/tests/test_module_runner.py` & `chaanbot-3.1.1/tests/test_module_runner.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.1.0/tests/test_revAMP.py` & `chaanbot-3.1.1/tests/test_revAMP.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import os
 from unittest import IsolatedAsyncioTestCase
 from unittest.mock import AsyncMock, Mock
 
-from chaanbot.modules.RevAMP import RevAMP
+from chaanbot.modules.revamp import Revamp
 
 
-class TestRevAMP(IsolatedAsyncioTestCase):
+class TestRevamp(IsolatedAsyncioTestCase):
     config_prefix_message = "prefix "
 
     def setUp(self) -> None:
         config = Mock()
         config.get.return_value = self.config_prefix_message
         self.event = Mock()
         self.event.sender = "user_id"
         self.room = AsyncMock()
         self.room.room_id = 1234
         self.matrix = AsyncMock()
-        self.module = RevAMP(config, self.matrix, Mock(), None)
+        self.module = Revamp(config, self.matrix, Mock(), None)
 
     async def test_rewrite_amp(self):
         ran = await self.module.run(self.room, None, "Check this out: https://www.youtube.com/amp/6j6ksOu1231")
 
         self.assertFalse(ran)
         self.matrix.send_text_to_room.assert_any_call(
             self.config_prefix_message + "https://www.youtube.com/6j6ksOu1231",
```

### Comparing `chaanbot-3.1.0/tests/test_rewrite_youtube_shorts.py` & `chaanbot-3.1.1/tests/test_rewrite_youtube_shorts.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.1.0/tests/test_start.py` & `chaanbot-3.1.1/tests/test_start.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.1.0/tests/test_twitter.py` & `chaanbot-3.1.1/tests/test_twitter.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.1.0/tests/test_weather.py` & `chaanbot-3.1.1/tests/test_weather.py`

 * *Files identical despite different names*

