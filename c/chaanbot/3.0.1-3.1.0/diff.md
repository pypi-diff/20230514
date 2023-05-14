# Comparing `tmp/chaanbot-3.0.1.tar.gz` & `tmp/chaanbot-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\chaanbot-3.0.1.tar", last modified: Wed Apr  5 13:49:39 2023, max compression
+gzip compressed data, was "dist\chaanbot-3.1.0.tar", last modified: Sun May 14 14:07:25 2023, max compression
```

## Comparing `chaanbot-3.0.1.tar` & `chaanbot-3.1.0.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 13:49:39.523938 chaanbot-3.0.1/
--rw-rw-rw-   0        0        0    35804 2020-01-04 14:14:41.000000 chaanbot-3.0.1/LICENSE
--rw-rw-rw-   0        0        0     3312 2023-04-05 13:49:39.522932 chaanbot-3.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2462 2021-07-18 10:10:15.000000 chaanbot-3.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 13:49:39.509365 chaanbot-3.0.1/chaanbot/
--rw-rw-rw-   0        0        0      140 2023-04-05 13:48:55.000000 chaanbot-3.0.1/chaanbot/__init__.py
--rw-rw-rw-   0        0        0     3885 2021-07-16 09:48:35.000000 chaanbot-3.0.1/chaanbot/client.py
--rw-rw-rw-   0        0        0     1677 2020-01-04 14:14:42.000000 chaanbot-3.0.1/chaanbot/command_utility.py
--rw-rw-rw-   0        0        0      271 2020-01-04 14:14:42.000000 chaanbot-3.0.1/chaanbot/database.py
--rw-rw-rw-   0        0        0     4618 2021-07-16 20:56:42.000000 chaanbot-3.0.1/chaanbot/matrix.py
--rw-rw-rw-   0        0        0     4488 2021-07-16 07:12:21.000000 chaanbot-3.0.1/chaanbot/module_loader.py
--rw-rw-rw-   0        0        0     1141 2021-11-15 09:51:45.000000 chaanbot-3.0.1/chaanbot/module_runner.py
-drwxrwxrwx   0        0        0        0 2023-04-05 13:49:39.516512 chaanbot-3.0.1/chaanbot/modules/
--rw-rw-rw-   0        0        0        0 2020-01-04 14:14:42.000000 chaanbot-3.0.1/chaanbot/modules/__init__.py
--rw-rw-rw-   0        0        0     1067 2021-07-16 07:14:48.000000 chaanbot-3.0.1/chaanbot/modules/alive.py
--rw-rw-rw-   0        0        0     4353 2022-05-07 08:45:56.000000 chaanbot-3.0.1/chaanbot/modules/chan_save.py
--rw-rw-rw-   0        0        0    10965 2022-04-26 21:28:17.000000 chaanbot-3.0.1/chaanbot/modules/highlight.py
--rw-rw-rw-   0        0        0     1423 2022-08-07 12:16:47.000000 chaanbot-3.0.1/chaanbot/modules/rewrite_youtube_shorts.py
--rw-rw-rw-   0        0        0     2001 2023-03-12 13:10:08.000000 chaanbot-3.0.1/chaanbot/modules/twitter.py
--rw-rw-rw-   0        0        0     7722 2023-04-05 13:28:59.000000 chaanbot-3.0.1/chaanbot/modules/weather.py
--rw-rw-rw-   0        0        0     3163 2023-04-05 13:48:55.000000 chaanbot-3.0.1/chaanbot/start.py
-drwxrwxrwx   0        0        0        0 2023-04-05 13:49:39.512881 chaanbot-3.0.1/chaanbot.egg-info/
--rw-rw-rw-   0        0        0     3312 2023-04-05 13:49:39.000000 chaanbot-3.0.1/chaanbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      950 2023-04-05 13:49:39.000000 chaanbot-3.0.1/chaanbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 13:49:39.000000 chaanbot-3.0.1/chaanbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-04-05 13:49:39.000000 chaanbot-3.0.1/chaanbot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2023-04-05 13:49:39.000000 chaanbot-3.0.1/chaanbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-05 13:49:39.000000 chaanbot-3.0.1/chaanbot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-05 13:49:39.523938 chaanbot-3.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1944 2023-03-12 13:22:59.000000 chaanbot-3.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-05 13:49:39.522932 chaanbot-3.0.1/tests/
--rw-rw-rw-   0        0        0        0 2020-01-04 14:14:42.000000 chaanbot-3.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0     1559 2021-07-16 09:12:30.000000 chaanbot-3.0.1/tests/test_alive.py
--rw-rw-rw-   0        0        0     5393 2022-05-07 08:42:41.000000 chaanbot-3.0.1/tests/test_chan_save.py
--rw-rw-rw-   0        0        0     1692 2021-07-16 09:52:18.000000 chaanbot-3.0.1/tests/test_client.py
--rw-rw-rw-   0        0        0     3125 2020-01-04 14:14:42.000000 chaanbot-3.0.1/tests/test_command_utility.py
--rw-rw-rw-   0        0        0      351 2020-01-04 14:14:42.000000 chaanbot-3.0.1/tests/test_database.py
--rw-rw-rw-   0        0        0     7799 2021-07-16 21:02:46.000000 chaanbot-3.0.1/tests/test_highlight.py
--rw-rw-rw-   0        0        0     4802 2021-07-16 10:54:29.000000 chaanbot-3.0.1/tests/test_matrix.py
--rw-rw-rw-   0        0        0     5075 2020-01-04 14:14:42.000000 chaanbot-3.0.1/tests/test_module_loader.py
--rw-rw-rw-   0        0        0     2608 2021-11-15 08:58:24.000000 chaanbot-3.0.1/tests/test_module_runner.py
--rw-rw-rw-   0        0        0     2246 2023-03-12 11:19:04.000000 chaanbot-3.0.1/tests/test_rewrite_youtube_shorts.py
--rw-rw-rw-   0        0        0     2745 2021-07-17 11:33:09.000000 chaanbot-3.0.1/tests/test_start.py
--rw-rw-rw-   0        0        0     3134 2023-03-12 13:10:48.000000 chaanbot-3.0.1/tests/test_twitter.py
--rw-rw-rw-   0        0        0     7566 2023-04-05 13:38:22.000000 chaanbot-3.0.1/tests/test_weather.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:07:25.922562 chaanbot-3.1.0/
+-rw-rw-rw-   0        0        0    35804 2020-01-04 14:14:41.000000 chaanbot-3.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3312 2023-05-14 14:07:25.922562 chaanbot-3.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2462 2023-05-14 13:45:28.000000 chaanbot-3.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 14:07:25.907508 chaanbot-3.1.0/chaanbot/
+-rw-rw-rw-   0        0        0      140 2023-05-14 13:55:46.000000 chaanbot-3.1.0/chaanbot/__init__.py
+-rw-rw-rw-   0        0        0     3885 2023-05-14 13:45:28.000000 chaanbot-3.1.0/chaanbot/client.py
+-rw-rw-rw-   0        0        0     1677 2020-01-04 14:14:42.000000 chaanbot-3.1.0/chaanbot/command_utility.py
+-rw-rw-rw-   0        0        0      271 2020-01-04 14:14:42.000000 chaanbot-3.1.0/chaanbot/database.py
+-rw-rw-rw-   0        0        0     4618 2023-05-14 13:45:28.000000 chaanbot-3.1.0/chaanbot/matrix.py
+-rw-rw-rw-   0        0        0     4488 2021-07-16 07:12:21.000000 chaanbot-3.1.0/chaanbot/module_loader.py
+-rw-rw-rw-   0        0        0     1141 2023-05-14 13:45:28.000000 chaanbot-3.1.0/chaanbot/module_runner.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:07:25.914548 chaanbot-3.1.0/chaanbot/modules/
+-rw-rw-rw-   0        0        0     1335 2023-05-14 14:06:39.000000 chaanbot-3.1.0/chaanbot/modules/RevAMP.py
+-rw-rw-rw-   0        0        0        0 2020-01-04 14:14:42.000000 chaanbot-3.1.0/chaanbot/modules/__init__.py
+-rw-rw-rw-   0        0        0     1067 2023-05-14 13:45:28.000000 chaanbot-3.1.0/chaanbot/modules/alive.py
+-rw-rw-rw-   0        0        0     4353 2023-05-14 13:45:28.000000 chaanbot-3.1.0/chaanbot/modules/chan_save.py
+-rw-rw-rw-   0        0        0    10965 2023-05-14 13:45:28.000000 chaanbot-3.1.0/chaanbot/modules/highlight.py
+-rw-rw-rw-   0        0        0     1423 2023-05-14 13:45:28.000000 chaanbot-3.1.0/chaanbot/modules/rewrite_youtube_shorts.py
+-rw-rw-rw-   0        0        0     2001 2023-05-14 13:45:28.000000 chaanbot-3.1.0/chaanbot/modules/twitter.py
+-rw-rw-rw-   0        0        0     7722 2023-05-14 13:45:28.000000 chaanbot-3.1.0/chaanbot/modules/weather.py
+-rw-rw-rw-   0        0        0     3163 2023-05-14 13:45:28.000000 chaanbot-3.1.0/chaanbot/start.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:07:25.910513 chaanbot-3.1.0/chaanbot.egg-info/
+-rw-rw-rw-   0        0        0     3312 2023-05-14 14:07:25.000000 chaanbot-3.1.0/chaanbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      998 2023-05-14 14:07:25.000000 chaanbot-3.1.0/chaanbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 14:07:25.000000 chaanbot-3.1.0/chaanbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-14 14:07:25.000000 chaanbot-3.1.0/chaanbot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2023-05-14 14:07:25.000000 chaanbot-3.1.0/chaanbot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-14 14:07:25.000000 chaanbot-3.1.0/chaanbot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 14:07:25.923565 chaanbot-3.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1944 2023-05-14 13:45:28.000000 chaanbot-3.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:07:25.922562 chaanbot-3.1.0/tests/
+-rw-rw-rw-   0        0        0        0 2020-01-04 14:14:42.000000 chaanbot-3.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     1559 2023-05-14 13:45:28.000000 chaanbot-3.1.0/tests/test_alive.py
+-rw-rw-rw-   0        0        0     5393 2023-05-14 13:45:28.000000 chaanbot-3.1.0/tests/test_chan_save.py
+-rw-rw-rw-   0        0        0     1692 2023-05-14 13:45:28.000000 chaanbot-3.1.0/tests/test_client.py
+-rw-rw-rw-   0        0        0     3125 2020-01-04 14:14:42.000000 chaanbot-3.1.0/tests/test_command_utility.py
+-rw-rw-rw-   0        0        0      351 2020-01-04 14:14:42.000000 chaanbot-3.1.0/tests/test_database.py
+-rw-rw-rw-   0        0        0     7799 2023-05-14 13:45:28.000000 chaanbot-3.1.0/tests/test_highlight.py
+-rw-rw-rw-   0        0        0     4802 2023-05-14 13:45:28.000000 chaanbot-3.1.0/tests/test_matrix.py
+-rw-rw-rw-   0        0        0     5075 2020-01-04 14:14:42.000000 chaanbot-3.1.0/tests/test_module_loader.py
+-rw-rw-rw-   0        0        0     2608 2023-05-14 13:45:28.000000 chaanbot-3.1.0/tests/test_module_runner.py
+-rw-rw-rw-   0        0        0     1763 2023-05-14 14:04:40.000000 chaanbot-3.1.0/tests/test_revAMP.py
+-rw-rw-rw-   0        0        0     2246 2023-05-14 13:45:28.000000 chaanbot-3.1.0/tests/test_rewrite_youtube_shorts.py
+-rw-rw-rw-   0        0        0     2745 2023-05-14 13:45:28.000000 chaanbot-3.1.0/tests/test_start.py
+-rw-rw-rw-   0        0        0     3134 2023-05-14 13:45:28.000000 chaanbot-3.1.0/tests/test_twitter.py
+-rw-rw-rw-   0        0        0     7566 2023-05-14 13:45:28.000000 chaanbot-3.1.0/tests/test_weather.py
```

### Comparing `chaanbot-3.0.1/LICENSE` & `chaanbot-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chaanbot-3.0.1/PKG-INFO` & `chaanbot-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaanbot
-Version: 3.0.1
+Version: 3.1.0
 Summary: A Matrix chat bot
 Home-page: https://github.com/RichardNysater/chaanbot
 Author: Richard Nysäter
 Author-email: richard@nysater.org
 License: GPLv3+
 Keywords: m,a,t,r,i,x, ,c,h,a,t, ,b,o,t
 Platform: UNKNOWN
```

### Comparing `chaanbot-3.0.1/README.md` & `chaanbot-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `chaanbot-3.0.1/chaanbot/client.py` & `chaanbot-3.1.0/chaanbot/client.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.0.1/chaanbot/command_utility.py` & `chaanbot-3.1.0/chaanbot/command_utility.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.0.1/chaanbot/matrix.py` & `chaanbot-3.1.0/chaanbot/matrix.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.0.1/chaanbot/module_loader.py` & `chaanbot-3.1.0/chaanbot/module_loader.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.0.1/chaanbot/module_runner.py` & `chaanbot-3.1.0/chaanbot/module_runner.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.0.1/chaanbot/modules/alive.py` & `chaanbot-3.1.0/chaanbot/modules/alive.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.0.1/chaanbot/modules/chan_save.py` & `chaanbot-3.1.0/chaanbot/modules/chan_save.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.0.1/chaanbot/modules/highlight.py` & `chaanbot-3.1.0/chaanbot/modules/highlight.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.0.1/chaanbot/modules/rewrite_youtube_shorts.py` & `chaanbot-3.1.0/chaanbot/modules/rewrite_youtube_shorts.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.0.1/chaanbot/modules/twitter.py` & `chaanbot-3.1.0/chaanbot/modules/twitter.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.0.1/chaanbot/modules/weather.py` & `chaanbot-3.1.0/chaanbot/modules/weather.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.0.1/chaanbot/start.py` & `chaanbot-3.1.0/chaanbot/start.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.0.1/chaanbot.egg-info/PKG-INFO` & `chaanbot-3.1.0/chaanbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaanbot
-Version: 3.0.1
+Version: 3.1.0
 Summary: A Matrix chat bot
 Home-page: https://github.com/RichardNysater/chaanbot
 Author: Richard Nysäter
 Author-email: richard@nysater.org
 License: GPLv3+
 Keywords: m,a,t,r,i,x, ,c,h,a,t, ,b,o,t
 Platform: UNKNOWN
```

### Comparing `chaanbot-3.0.1/chaanbot.egg-info/SOURCES.txt` & `chaanbot-3.1.0/chaanbot.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 chaanbot/start.py
 chaanbot.egg-info/PKG-INFO
 chaanbot.egg-info/SOURCES.txt
 chaanbot.egg-info/dependency_links.txt
 chaanbot.egg-info/entry_points.txt
 chaanbot.egg-info/requires.txt
 chaanbot.egg-info/top_level.txt
+chaanbot/modules/RevAMP.py
 chaanbot/modules/__init__.py
 chaanbot/modules/alive.py
 chaanbot/modules/chan_save.py
 chaanbot/modules/highlight.py
 chaanbot/modules/rewrite_youtube_shorts.py
 chaanbot/modules/twitter.py
 chaanbot/modules/weather.py
@@ -28,11 +29,12 @@
 tests/test_client.py
 tests/test_command_utility.py
 tests/test_database.py
 tests/test_highlight.py
 tests/test_matrix.py
 tests/test_module_loader.py
 tests/test_module_runner.py
+tests/test_revAMP.py
 tests/test_rewrite_youtube_shorts.py
 tests/test_start.py
 tests/test_twitter.py
 tests/test_weather.py
```

### Comparing `chaanbot-3.0.1/setup.py` & `chaanbot-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.0.1/tests/test_alive.py` & `chaanbot-3.1.0/tests/test_alive.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.0.1/tests/test_chan_save.py` & `chaanbot-3.1.0/tests/test_chan_save.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.0.1/tests/test_client.py` & `chaanbot-3.1.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.0.1/tests/test_command_utility.py` & `chaanbot-3.1.0/tests/test_command_utility.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.0.1/tests/test_highlight.py` & `chaanbot-3.1.0/tests/test_highlight.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.0.1/tests/test_matrix.py` & `chaanbot-3.1.0/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.0.1/tests/test_module_loader.py` & `chaanbot-3.1.0/tests/test_module_loader.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.0.1/tests/test_module_runner.py` & `chaanbot-3.1.0/tests/test_module_runner.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.0.1/tests/test_rewrite_youtube_shorts.py` & `chaanbot-3.1.0/tests/test_rewrite_youtube_shorts.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.0.1/tests/test_start.py` & `chaanbot-3.1.0/tests/test_start.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.0.1/tests/test_twitter.py` & `chaanbot-3.1.0/tests/test_twitter.py`

 * *Files identical despite different names*

### Comparing `chaanbot-3.0.1/tests/test_weather.py` & `chaanbot-3.1.0/tests/test_weather.py`

 * *Files identical despite different names*

