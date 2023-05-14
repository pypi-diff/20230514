# Comparing `tmp/nitrado-1.0.8.tar.gz` & `tmp/nitrado-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nitrado-1.0.8.tar", last modified: Sun Apr 23 21:52:04 2023, max compression
+gzip compressed data, was "nitrado-1.0.9.tar", last modified: Sun Apr 23 22:13:58 2023, max compression
```

## Comparing `nitrado-1.0.8.tar` & `nitrado-1.0.9.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.955841 nitrado-1.0.8/
--rw-rw-rw-   0        0        0     1093 2023-03-25 00:21:47.000000 nitrado-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     3857 2023-04-23 21:52:04.955841 nitrado-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3004 2023-04-23 21:51:39.000000 nitrado-1.0.8/README.md
--rw-rw-rw-   0        0        0      555 2023-04-16 01:48:34.000000 nitrado-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0     1176 2023-04-23 21:52:04.956429 nitrado-1.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.902125 nitrado-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.918516 nitrado-1.0.8/src/nitrado/
--rw-rw-rw-   0        0        0      332 2023-04-23 06:24:51.000000 nitrado-1.0.8/src/nitrado/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.920945 nitrado-1.0.8/src/nitrado/games/
--rw-rw-rw-   0        0        0       43 2023-04-23 05:14:54.000000 nitrado-1.0.8/src/nitrado/games/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.920945 nitrado-1.0.8/src/nitrado/games/ark/
--rw-rw-rw-   0        0        0       56 2023-04-23 04:53:42.000000 nitrado-1.0.8/src/nitrado/games/ark/__init__.py
--rw-rw-rw-   0        0        0     6598 2023-04-23 21:50:27.000000 nitrado-1.0.8/src/nitrado/games/ark/ark_survival.py
-drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.920945 nitrado-1.0.8/src/nitrado/games/ark/game_specific/
--rw-rw-rw-   0        0        0        0 2023-04-23 05:03:58.000000 nitrado-1.0.8/src/nitrado/games/ark/game_specific/__init__.py
--rw-rw-rw-   0        0        0     1770 2023-04-23 05:44:17.000000 nitrado-1.0.8/src/nitrado/games/ark/game_specific/game_features.py
--rw-rw-rw-   0        0        0     1353 2023-04-23 05:52:11.000000 nitrado-1.0.8/src/nitrado/games/ark/game_specific/game_specific.py
--rw-rw-rw-   0        0        0       98 2023-04-19 12:08:29.000000 nitrado-1.0.8/src/nitrado/games/ark/logs.py
--rw-rw-rw-   0        0        0      893 2023-04-23 04:53:42.000000 nitrado-1.0.8/src/nitrado/games/ark/query.py
-drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.920945 nitrado-1.0.8/src/nitrado/games/ark/settings/
--rw-rw-rw-   0        0        0        0 2023-04-23 05:03:30.000000 nitrado-1.0.8/src/nitrado/games/ark/settings/__init__.py
--rw-rw-rw-   0        0        0    11956 2023-04-23 05:44:17.000000 nitrado-1.0.8/src/nitrado/games/ark/settings/config.py
--rw-rw-rw-   0        0        0      493 2023-04-23 05:06:51.000000 nitrado-1.0.8/src/nitrado/games/ark/settings/feature_settings.py
--rw-rw-rw-   0        0        0    11429 2023-04-23 05:44:17.000000 nitrado-1.0.8/src/nitrado/games/ark/settings/game_ini.py
--rw-rw-rw-   0        0        0     2921 2023-04-23 05:44:17.000000 nitrado-1.0.8/src/nitrado/games/ark/settings/general.py
--rw-rw-rw-   0        0        0     1575 2023-04-23 05:52:11.000000 nitrado-1.0.8/src/nitrado/games/ark/settings/settings.py
--rw-rw-rw-   0        0        0     5798 2023-04-23 05:44:17.000000 nitrado-1.0.8/src/nitrado/games/ark/settings/start_param.py
-drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.935605 nitrado-1.0.8/src/nitrado/gameserver/
--rw-rw-rw-   0        0        0       36 2023-04-23 03:36:03.000000 nitrado-1.0.8/src/nitrado/gameserver/__init__.py
--rw-rw-rw-   0        0        0      511 2023-04-23 04:31:25.000000 nitrado-1.0.8/src/nitrado/gameserver/credentials.py
--rw-rw-rw-   0        0        0    19160 2023-04-23 07:18:43.000000 nitrado-1.0.8/src/nitrado/gameserver/gameserver.py
--rw-rw-rw-   0        0        0      877 2023-04-23 04:39:32.000000 nitrado-1.0.8/src/nitrado/gameserver/host_systems.py
--rw-rw-rw-   0        0        0      608 2023-04-23 04:25:36.000000 nitrado-1.0.8/src/nitrado/gameserver/operating_system.py
--rw-rw-rw-   0        0        0      946 2023-04-23 06:35:04.000000 nitrado-1.0.8/src/nitrado/gameserver/players.py
-drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.935605 nitrado-1.0.8/src/nitrado/globals/
--rw-rw-rw-   0        0        0       29 2023-04-23 04:53:42.000000 nitrado-1.0.8/src/nitrado/globals/__init__.py
--rw-rw-rw-   0        0        0     1272 2023-04-23 07:18:43.000000 nitrado-1.0.8/src/nitrado/globals/globals.py
--rw-rw-rw-   0        0        0      583 2023-04-23 00:50:25.000000 nitrado-1.0.8/src/nitrado/globals/maintenance.py
-drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.935605 nitrado-1.0.8/src/nitrado/lib/
--rw-rw-rw-   0        0        0       30 2023-04-23 03:36:03.000000 nitrado-1.0.8/src/nitrado/lib/__init__.py
--rw-rw-rw-   0        0        0     2430 2023-04-23 07:01:52.000000 nitrado-1.0.8/src/nitrado/lib/client.py
--rw-rw-rw-   0        0        0     1347 2023-04-16 03:40:10.000000 nitrado-1.0.8/src/nitrado/lib/errors.py
--rw-rw-rw-   0        0        0      549 2023-04-23 06:23:45.000000 nitrado-1.0.8/src/nitrado/nitrado.py
-drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.935605 nitrado-1.0.8/src/nitrado/oauth/
--rw-rw-rw-   0        0        0        0 2023-04-23 07:16:16.000000 nitrado-1.0.8/src/nitrado/oauth/__init__.py
--rw-rw-rw-   0        0        0        0 2023-03-25 00:21:47.000000 nitrado-1.0.8/src/nitrado/py.typed
-drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.951835 nitrado-1.0.8/src/nitrado/service/
--rw-rw-rw-   0        0        0       89 2023-04-23 03:36:03.000000 nitrado-1.0.8/src/nitrado/service/__init__.py
--rw-rw-rw-   0        0        0      474 2023-04-23 02:34:26.000000 nitrado-1.0.8/src/nitrado/service/action.py
--rw-rw-rw-   0        0        0      930 2023-04-23 02:34:26.000000 nitrado-1.0.8/src/nitrado/service/arguments.py
--rw-rw-rw-   0        0        0      910 2023-04-23 02:34:26.000000 nitrado-1.0.8/src/nitrado/service/details.py
--rw-rw-rw-   0        0        0      765 2023-04-23 03:22:07.000000 nitrado-1.0.8/src/nitrado/service/log.py
--rw-rw-rw-   0        0        0     1536 2023-04-23 03:17:31.000000 nitrado-1.0.8/src/nitrado/service/logs_page.py
--rw-rw-rw-   0        0        0     1517 2023-04-23 02:24:59.000000 nitrado-1.0.8/src/nitrado/service/notification.py
--rw-rw-rw-   0        0        0     4263 2023-04-23 03:39:31.000000 nitrado-1.0.8/src/nitrado/service/service.py
--rw-rw-rw-   0        0        0     2871 2023-04-23 02:34:26.000000 nitrado-1.0.8/src/nitrado/service/task.py
-drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.952843 nitrado-1.0.8/src/nitrado/tools/
--rw-rw-rw-   0        0        0        0 2023-04-23 00:21:40.000000 nitrado-1.0.8/src/nitrado/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.920945 nitrado-1.0.8/src/nitrado.egg-info/
--rw-rw-rw-   0        0        0     3857 2023-04-23 21:52:04.000000 nitrado-1.0.8/src/nitrado.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1728 2023-04-23 21:52:04.000000 nitrado-1.0.8/src/nitrado.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 21:52:04.000000 nitrado-1.0.8/src/nitrado.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2023-04-23 21:52:04.000000 nitrado-1.0.8/src/nitrado.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-23 21:52:04.000000 nitrado-1.0.8/src/nitrado.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-23 21:52:04.954842 nitrado-1.0.8/tests/
--rw-rw-rw-   0        0        0     1998 2023-04-23 19:58:07.000000 nitrado-1.0.8/tests/test_connection.py
--rw-rw-rw-   0        0        0    19270 2023-04-23 20:12:30.000000 nitrado-1.0.8/tests/test_game_server.py
--rw-rw-rw-   0        0        0     1662 2023-04-23 20:13:19.000000 nitrado-1.0.8/tests/test_service.py
+drwxrwxrwx   0        0        0        0 2023-04-23 22:13:58.043939 nitrado-1.0.9/
+-rw-rw-rw-   0        0        0     1093 2023-03-25 00:21:47.000000 nitrado-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3971 2023-04-23 22:13:58.043939 nitrado-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3118 2023-04-23 22:06:07.000000 nitrado-1.0.9/README.md
+-rw-rw-rw-   0        0        0      584 2023-04-23 22:13:39.000000 nitrado-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0     1199 2023-04-23 22:13:58.043939 nitrado-1.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-23 22:13:57.997064 nitrado-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-04-23 22:13:57.997064 nitrado-1.0.9/src/nitrado/
+-rw-rw-rw-   0        0        0      332 2023-04-23 06:24:51.000000 nitrado-1.0.9/src/nitrado/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 22:13:58.012693 nitrado-1.0.9/src/nitrado/games/
+-rw-rw-rw-   0        0        0       43 2023-04-23 05:14:54.000000 nitrado-1.0.9/src/nitrado/games/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 22:13:58.012693 nitrado-1.0.9/src/nitrado/games/ark/
+-rw-rw-rw-   0        0        0       56 2023-04-23 04:53:42.000000 nitrado-1.0.9/src/nitrado/games/ark/__init__.py
+-rw-rw-rw-   0        0        0     6598 2023-04-23 21:50:27.000000 nitrado-1.0.9/src/nitrado/games/ark/ark_survival.py
+drwxrwxrwx   0        0        0        0 2023-04-23 22:13:58.012693 nitrado-1.0.9/src/nitrado/games/ark/game_specific/
+-rw-rw-rw-   0        0        0        0 2023-04-23 05:03:58.000000 nitrado-1.0.9/src/nitrado/games/ark/game_specific/__init__.py
+-rw-rw-rw-   0        0        0     1770 2023-04-23 05:44:17.000000 nitrado-1.0.9/src/nitrado/games/ark/game_specific/game_features.py
+-rw-rw-rw-   0        0        0     1353 2023-04-23 05:52:11.000000 nitrado-1.0.9/src/nitrado/games/ark/game_specific/game_specific.py
+-rw-rw-rw-   0        0        0       98 2023-04-19 12:08:29.000000 nitrado-1.0.9/src/nitrado/games/ark/logs.py
+-rw-rw-rw-   0        0        0      893 2023-04-23 04:53:42.000000 nitrado-1.0.9/src/nitrado/games/ark/query.py
+drwxrwxrwx   0        0        0        0 2023-04-23 22:13:58.012693 nitrado-1.0.9/src/nitrado/games/ark/settings/
+-rw-rw-rw-   0        0        0        0 2023-04-23 05:03:30.000000 nitrado-1.0.9/src/nitrado/games/ark/settings/__init__.py
+-rw-rw-rw-   0        0        0    11956 2023-04-23 05:44:17.000000 nitrado-1.0.9/src/nitrado/games/ark/settings/config.py
+-rw-rw-rw-   0        0        0      493 2023-04-23 05:06:51.000000 nitrado-1.0.9/src/nitrado/games/ark/settings/feature_settings.py
+-rw-rw-rw-   0        0        0    11429 2023-04-23 05:44:17.000000 nitrado-1.0.9/src/nitrado/games/ark/settings/game_ini.py
+-rw-rw-rw-   0        0        0     2921 2023-04-23 05:44:17.000000 nitrado-1.0.9/src/nitrado/games/ark/settings/general.py
+-rw-rw-rw-   0        0        0     1575 2023-04-23 05:52:11.000000 nitrado-1.0.9/src/nitrado/games/ark/settings/settings.py
+-rw-rw-rw-   0        0        0     5798 2023-04-23 05:44:17.000000 nitrado-1.0.9/src/nitrado/games/ark/settings/start_param.py
+drwxrwxrwx   0        0        0        0 2023-04-23 22:13:58.028315 nitrado-1.0.9/src/nitrado/gameserver/
+-rw-rw-rw-   0        0        0       36 2023-04-23 03:36:03.000000 nitrado-1.0.9/src/nitrado/gameserver/__init__.py
+-rw-rw-rw-   0        0        0      511 2023-04-23 04:31:25.000000 nitrado-1.0.9/src/nitrado/gameserver/credentials.py
+-rw-rw-rw-   0        0        0    19160 2023-04-23 07:18:43.000000 nitrado-1.0.9/src/nitrado/gameserver/gameserver.py
+-rw-rw-rw-   0        0        0      877 2023-04-23 04:39:32.000000 nitrado-1.0.9/src/nitrado/gameserver/host_systems.py
+-rw-rw-rw-   0        0        0      608 2023-04-23 04:25:36.000000 nitrado-1.0.9/src/nitrado/gameserver/operating_system.py
+-rw-rw-rw-   0        0        0      946 2023-04-23 06:35:04.000000 nitrado-1.0.9/src/nitrado/gameserver/players.py
+drwxrwxrwx   0        0        0        0 2023-04-23 22:13:58.028315 nitrado-1.0.9/src/nitrado/globals/
+-rw-rw-rw-   0        0        0       29 2023-04-23 04:53:42.000000 nitrado-1.0.9/src/nitrado/globals/__init__.py
+-rw-rw-rw-   0        0        0     1272 2023-04-23 07:18:43.000000 nitrado-1.0.9/src/nitrado/globals/globals.py
+-rw-rw-rw-   0        0        0      583 2023-04-23 00:50:25.000000 nitrado-1.0.9/src/nitrado/globals/maintenance.py
+drwxrwxrwx   0        0        0        0 2023-04-23 22:13:58.028315 nitrado-1.0.9/src/nitrado/lib/
+-rw-rw-rw-   0        0        0       30 2023-04-23 03:36:03.000000 nitrado-1.0.9/src/nitrado/lib/__init__.py
+-rw-rw-rw-   0        0        0     2430 2023-04-23 07:01:52.000000 nitrado-1.0.9/src/nitrado/lib/client.py
+-rw-rw-rw-   0        0        0     1347 2023-04-16 03:40:10.000000 nitrado-1.0.9/src/nitrado/lib/errors.py
+-rw-rw-rw-   0        0        0      549 2023-04-23 06:23:45.000000 nitrado-1.0.9/src/nitrado/nitrado.py
+drwxrwxrwx   0        0        0        0 2023-04-23 22:13:58.028315 nitrado-1.0.9/src/nitrado/oauth/
+-rw-rw-rw-   0        0        0        0 2023-04-23 07:16:16.000000 nitrado-1.0.9/src/nitrado/oauth/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-03-25 00:21:47.000000 nitrado-1.0.9/src/nitrado/py.typed
+drwxrwxrwx   0        0        0        0 2023-04-23 22:13:58.028315 nitrado-1.0.9/src/nitrado/service/
+-rw-rw-rw-   0        0        0       89 2023-04-23 03:36:03.000000 nitrado-1.0.9/src/nitrado/service/__init__.py
+-rw-rw-rw-   0        0        0      474 2023-04-23 02:34:26.000000 nitrado-1.0.9/src/nitrado/service/action.py
+-rw-rw-rw-   0        0        0      930 2023-04-23 02:34:26.000000 nitrado-1.0.9/src/nitrado/service/arguments.py
+-rw-rw-rw-   0        0        0      910 2023-04-23 02:34:26.000000 nitrado-1.0.9/src/nitrado/service/details.py
+-rw-rw-rw-   0        0        0      765 2023-04-23 03:22:07.000000 nitrado-1.0.9/src/nitrado/service/log.py
+-rw-rw-rw-   0        0        0     1536 2023-04-23 03:17:31.000000 nitrado-1.0.9/src/nitrado/service/logs_page.py
+-rw-rw-rw-   0        0        0     1517 2023-04-23 02:24:59.000000 nitrado-1.0.9/src/nitrado/service/notification.py
+-rw-rw-rw-   0        0        0     4263 2023-04-23 03:39:31.000000 nitrado-1.0.9/src/nitrado/service/service.py
+-rw-rw-rw-   0        0        0     2871 2023-04-23 02:34:26.000000 nitrado-1.0.9/src/nitrado/service/task.py
+drwxrwxrwx   0        0        0        0 2023-04-23 22:13:58.043939 nitrado-1.0.9/src/nitrado/tools/
+-rw-rw-rw-   0        0        0        0 2023-04-23 00:21:40.000000 nitrado-1.0.9/src/nitrado/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 22:13:58.012693 nitrado-1.0.9/src/nitrado.egg-info/
+-rw-rw-rw-   0        0        0     3971 2023-04-23 22:13:57.000000 nitrado-1.0.9/src/nitrado.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1728 2023-04-23 22:13:57.000000 nitrado-1.0.9/src/nitrado.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 22:13:57.000000 nitrado-1.0.9/src/nitrado.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2023-04-23 22:13:57.000000 nitrado-1.0.9/src/nitrado.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-23 22:13:57.000000 nitrado-1.0.9/src/nitrado.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 22:13:58.043939 nitrado-1.0.9/tests/
+-rw-rw-rw-   0        0        0     1998 2023-04-23 19:58:07.000000 nitrado-1.0.9/tests/test_connection.py
+-rw-rw-rw-   0        0        0    19270 2023-04-23 20:12:30.000000 nitrado-1.0.9/tests/test_game_server.py
+-rw-rw-rw-   0        0        0     1662 2023-04-23 20:13:19.000000 nitrado-1.0.9/tests/test_service.py
```

### Comparing `nitrado-1.0.8/LICENSE` & `nitrado-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.8/PKG-INFO` & `nitrado-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitrado
-Version: 1.0.8
+Version: 1.0.9
 Summary: This application accesses the Nitrado API.
 Home-page: https://github.com/mjlomeli/NitradoAPI
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjlomeli/NitradoAPI/issues
 Platform: unix
 Platform: linux
@@ -41,22 +41,24 @@
 # Overview
 
 To have access to this application you must have an account created at [Nitrado](https://server.nitrado.net/)
 and create an API key.
 
 # [Wiki - Full documentation](https://github.com/mjlomeli/NitradoAPI/wiki)
 ### Table of contents
-#### 1. [Introduction](https://github.com/mjlomeli/NitradoAPI/wiki#introduction)
+#### 1. [Generate API Key](https://github.com/mjlomeli/NitradoAPI/wiki/Generate-API-Key)
    > Shows how to get access to your API key.
 #### 2. [Getting Started](https://github.com/mjlomeli/NitradoAPI/wiki/Getting-Started)
    > Shows how to log in to the client and use the basic code interface
 #### 3. [Services](https://github.com/mjlomeli/NitradoAPI/wiki/Services)
    > Data provided outside of the game server. Like server status, user id, and auto extension plan.
 #### 4. [GameServer](https://github.com/mjlomeli/NitradoAPI/wiki/GameServer)
    > Data directly related to the game server. This includes the player list, game settings, etc.
+#### 5. [Games](https://github.com/mjlomeli/NitradoAPI/wiki/Games)
+   > Custom game specific libraries.
 
 <br />
 
 # Examples
 
 ### Connect the Client
 To begin using the API you must have the API key saved as an environment variable.
```

### Comparing `nitrado-1.0.8/README.md` & `nitrado-1.0.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -16,22 +16,24 @@
 # Overview
 
 To have access to this application you must have an account created at [Nitrado](https://server.nitrado.net/)
 and create an API key.
 
 # [Wiki - Full documentation](https://github.com/mjlomeli/NitradoAPI/wiki)
 ### Table of contents
-#### 1. [Introduction](https://github.com/mjlomeli/NitradoAPI/wiki#introduction)
+#### 1. [Generate API Key](https://github.com/mjlomeli/NitradoAPI/wiki/Generate-API-Key)
    > Shows how to get access to your API key.
 #### 2. [Getting Started](https://github.com/mjlomeli/NitradoAPI/wiki/Getting-Started)
    > Shows how to log in to the client and use the basic code interface
 #### 3. [Services](https://github.com/mjlomeli/NitradoAPI/wiki/Services)
    > Data provided outside of the game server. Like server status, user id, and auto extension plan.
 #### 4. [GameServer](https://github.com/mjlomeli/NitradoAPI/wiki/GameServer)
    > Data directly related to the game server. This includes the player list, game settings, etc.
+#### 5. [Games](https://github.com/mjlomeli/NitradoAPI/wiki/Games)
+   > Custom game specific libraries.
 
 <br />
 
 # Examples
 
 ### Connect the Client
 To begin using the API you must have the API key saved as an environment variable.
```

### Comparing `nitrado-1.0.8/pyproject.toml` & `nitrado-1.0.9/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [build-system]
 requires = [
     "setuptools>=42",
     "wheel",
+    "python-dotenv>=1.0.0",
     "requests==2.*"
 ]
 build-backend = "setuptools.build_meta"
 
 
 [too.pytest.ini_options]
 addopts = "--cov=nitrado"
```

### Comparing `nitrado-1.0.8/setup.cfg` & `nitrado-1.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6974 7261 646f 0d0a 7665 7273   = nitrado..vers
-00000020: 696f 6e20 3d20 312e 302e 380d 0a74 6573  ion = 1.0.8..tes
+00000020: 696f 6e20 3d20 312e 302e 390d 0a74 6573  ion = 1.0.9..tes
 00000030: 745f 7665 7273 696f 6e20 3d20 312e 302e  t_version = 1.0.
 00000040: 370d 0a70 726f 6475 6374 696f 6e5f 7665  7..production_ve
-00000050: 7273 696f 6e20 3d20 312e 302e 380d 0a61  rsion = 1.0.8..a
+00000050: 7273 696f 6e20 3d20 312e 302e 390d 0a61  rsion = 1.0.9..a
 00000060: 7574 686f 7220 3d20 4d61 7572 6963 696f  uthor = Mauricio
 00000070: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000080: 2064 6576 2e6d 6175 7269 6369 6f2e 6c6f   dev.mauricio.lo
 00000090: 6d65 6c69 4067 6d61 696c 2e63 6f6d 0d0a  meli@gmail.com..
 000000a0: 6465 7363 7269 7074 696f 6e20 3d20 5468  description = Th
 000000b0: 6973 2061 7070 6c69 6361 7469 6f6e 2061  is application a
 000000c0: 6363 6573 7365 7320 7468 6520 4e69 7472  ccesses the Nitr
@@ -50,25 +50,26 @@
 00000310: 5d0d 0a70 6163 6b61 6765 5f64 6972 203d  ]..package_dir =
 00000320: 200d 0a09 3d20 7372 630d 0a70 6163 6b61   ...= src..packa
 00000330: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
 00000340: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
 00000350: 3d33 2e39 0d0a 696e 7374 616c 6c5f 7265  =3.9..install_re
 00000360: 7175 6972 6573 203d 200d 0a09 7768 6565  quires = ...whee
 00000370: 6c0d 0a09 7265 7175 6573 7473 3d3d 322e  l...requests==2.
-00000380: 2a0d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  *....[options.pa
-00000390: 636b 6167 6573 2e66 696e 645d 0d0a 7768  ckages.find]..wh
-000003a0: 6572 6520 3d20 7372 630d 0a0d 0a5b 6f70  ere = src....[op
-000003b0: 7469 6f6e 732e 6578 7472 6173 5f72 6571  tions.extras_req
-000003c0: 7569 7265 5d0d 0a74 6573 7469 6e67 203d  uire]..testing =
-000003d0: 200d 0a09 7079 7465 7374 3e3d 362e 300d   ...pytest>=6.0.
-000003e0: 0a09 7079 7465 7374 2d63 6f76 3e3d 322e  ..pytest-cov>=2.
-000003f0: 300d 0a09 6d79 7079 3e3d 302e 3931 300d  0...mypy>=0.910.
-00000400: 0a09 666c 616b 6538 3e3d 332e 390d 0a09  ..flake8>=3.9...
-00000410: 746f 783e 3d33 2e32 340d 0a0d 0a5b 6f70  tox>=3.24....[op
-00000420: 7469 6f6e 732e 7061 636b 6167 655f 6461  tions.package_da
-00000430: 7461 5d0d 0a6e 6974 7261 646f 203d 2070  ta]..nitrado = p
-00000440: 792e 7479 7065 640d 0a0d 0a5b 666c 616b  y.typed....[flak
-00000450: 6538 5d0d 0a6d 6178 2d6c 696e 652d 6c65  e8]..max-line-le
-00000460: 6e67 7468 203d 2031 3630 0d0a 0d0a 5b65  ngth = 160....[e
-00000470: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
-00000480: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
-00000490: 203d 2030 0d0a 0d0a                       = 0....
+00000380: 2a0d 0a09 7079 7468 6f6e 2d64 6f74 656e  *...python-doten
+00000390: 763e 3d31 2e30 2e30 0d0a 0d0a 5b6f 7074  v>=1.0.0....[opt
+000003a0: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
+000003b0: 6e64 5d0d 0a77 6865 7265 203d 2073 7263  nd]..where = src
+000003c0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e65 7874  ....[options.ext
+000003d0: 7261 735f 7265 7175 6972 655d 0d0a 7465  ras_require]..te
+000003e0: 7374 696e 6720 3d20 0d0a 0970 7974 6573  sting = ...pytes
+000003f0: 743e 3d36 2e30 0d0a 0970 7974 6573 742d  t>=6.0...pytest-
+00000400: 636f 763e 3d32 2e30 0d0a 096d 7970 793e  cov>=2.0...mypy>
+00000410: 3d30 2e39 3130 0d0a 0966 6c61 6b65 383e  =0.910...flake8>
+00000420: 3d33 2e39 0d0a 0974 6f78 3e3d 332e 3234  =3.9...tox>=3.24
+00000430: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
+00000440: 6b61 6765 5f64 6174 615d 0d0a 6e69 7472  kage_data]..nitr
+00000450: 6164 6f20 3d20 7079 2e74 7970 6564 0d0a  ado = py.typed..
+00000460: 0d0a 5b66 6c61 6b65 385d 0d0a 6d61 782d  ..[flake8]..max-
+00000470: 6c69 6e65 2d6c 656e 6774 6820 3d20 3136  line-length = 16
+00000480: 300d 0a0d 0a5b 6567 675f 696e 666f 5d0d  0....[egg_info].
+00000490: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
+000004a0: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
```

### Comparing `nitrado-1.0.8/src/nitrado/games/ark/ark_survival.py` & `nitrado-1.0.9/src/nitrado/games/ark/ark_survival.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.8/src/nitrado/games/ark/game_specific/game_features.py` & `nitrado-1.0.9/src/nitrado/games/ark/game_specific/game_features.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.8/src/nitrado/games/ark/game_specific/game_specific.py` & `nitrado-1.0.9/src/nitrado/games/ark/game_specific/game_specific.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.8/src/nitrado/games/ark/query.py` & `nitrado-1.0.9/src/nitrado/games/ark/query.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.8/src/nitrado/games/ark/settings/config.py` & `nitrado-1.0.9/src/nitrado/games/ark/settings/config.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.8/src/nitrado/games/ark/settings/game_ini.py` & `nitrado-1.0.9/src/nitrado/games/ark/settings/game_ini.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.8/src/nitrado/games/ark/settings/general.py` & `nitrado-1.0.9/src/nitrado/games/ark/settings/general.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.8/src/nitrado/games/ark/settings/settings.py` & `nitrado-1.0.9/src/nitrado/games/ark/settings/settings.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.8/src/nitrado/games/ark/settings/start_param.py` & `nitrado-1.0.9/src/nitrado/games/ark/settings/start_param.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.8/src/nitrado/gameserver/gameserver.py` & `nitrado-1.0.9/src/nitrado/gameserver/gameserver.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.8/src/nitrado/gameserver/host_systems.py` & `nitrado-1.0.9/src/nitrado/gameserver/host_systems.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.8/src/nitrado/gameserver/operating_system.py` & `nitrado-1.0.9/src/nitrado/gameserver/operating_system.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.8/src/nitrado/gameserver/players.py` & `nitrado-1.0.9/src/nitrado/gameserver/players.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.8/src/nitrado/globals/globals.py` & `nitrado-1.0.9/src/nitrado/globals/globals.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.8/src/nitrado/globals/maintenance.py` & `nitrado-1.0.9/src/nitrado/globals/maintenance.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.8/src/nitrado/lib/client.py` & `nitrado-1.0.9/src/nitrado/lib/client.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.8/src/nitrado/lib/errors.py` & `nitrado-1.0.9/src/nitrado/lib/errors.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.8/src/nitrado/nitrado.py` & `nitrado-1.0.9/src/nitrado/nitrado.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.8/src/nitrado/service/arguments.py` & `nitrado-1.0.9/src/nitrado/service/arguments.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.8/src/nitrado/service/details.py` & `nitrado-1.0.9/src/nitrado/service/details.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.8/src/nitrado/service/log.py` & `nitrado-1.0.9/src/nitrado/service/log.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.8/src/nitrado/service/logs_page.py` & `nitrado-1.0.9/src/nitrado/service/logs_page.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.8/src/nitrado/service/notification.py` & `nitrado-1.0.9/src/nitrado/service/notification.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.8/src/nitrado/service/service.py` & `nitrado-1.0.9/src/nitrado/service/service.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.8/src/nitrado/service/task.py` & `nitrado-1.0.9/src/nitrado/service/task.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.8/src/nitrado.egg-info/PKG-INFO` & `nitrado-1.0.9/src/nitrado.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitrado
-Version: 1.0.8
+Version: 1.0.9
 Summary: This application accesses the Nitrado API.
 Home-page: https://github.com/mjlomeli/NitradoAPI
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjlomeli/NitradoAPI/issues
 Platform: unix
 Platform: linux
@@ -41,22 +41,24 @@
 # Overview
 
 To have access to this application you must have an account created at [Nitrado](https://server.nitrado.net/)
 and create an API key.
 
 # [Wiki - Full documentation](https://github.com/mjlomeli/NitradoAPI/wiki)
 ### Table of contents
-#### 1. [Introduction](https://github.com/mjlomeli/NitradoAPI/wiki#introduction)
+#### 1. [Generate API Key](https://github.com/mjlomeli/NitradoAPI/wiki/Generate-API-Key)
    > Shows how to get access to your API key.
 #### 2. [Getting Started](https://github.com/mjlomeli/NitradoAPI/wiki/Getting-Started)
    > Shows how to log in to the client and use the basic code interface
 #### 3. [Services](https://github.com/mjlomeli/NitradoAPI/wiki/Services)
    > Data provided outside of the game server. Like server status, user id, and auto extension plan.
 #### 4. [GameServer](https://github.com/mjlomeli/NitradoAPI/wiki/GameServer)
    > Data directly related to the game server. This includes the player list, game settings, etc.
+#### 5. [Games](https://github.com/mjlomeli/NitradoAPI/wiki/Games)
+   > Custom game specific libraries.
 
 <br />
 
 # Examples
 
 ### Connect the Client
 To begin using the API you must have the API key saved as an environment variable.
```

### Comparing `nitrado-1.0.8/src/nitrado.egg-info/SOURCES.txt` & `nitrado-1.0.9/src/nitrado.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.8/tests/test_connection.py` & `nitrado-1.0.9/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.8/tests/test_game_server.py` & `nitrado-1.0.9/tests/test_game_server.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.8/tests/test_service.py` & `nitrado-1.0.9/tests/test_service.py`

 * *Files identical despite different names*

