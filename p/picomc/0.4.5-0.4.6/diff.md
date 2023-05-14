# Comparing `tmp/picomc-0.4.5.tar.gz` & `tmp/picomc-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picomc-0.4.5.tar", last modified: Sun Feb 20 20:31:42 2022, max compression
+gzip compressed data, was "picomc-0.4.6.tar", last modified: Sun May 14 13:01:00 2023, max compression
```

## Comparing `picomc-0.4.5.tar` & `picomc-0.4.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 sammko    (1000) sammko    (1000)        0 2022-02-20 20:31:42.631341 picomc-0.4.5/
--rw-r--r--   0 sammko    (1000) sammko    (1000)     1086 2022-02-20 18:20:24.000000 picomc-0.4.5/LICENSE
--rw-r--r--   0 sammko    (1000) sammko    (1000)       23 2020-09-05 11:38:56.000000 picomc-0.4.5/MANIFEST.in
--rw-r--r--   0 sammko    (1000) sammko    (1000)      422 2022-02-20 20:31:42.631341 picomc-0.4.5/PKG-INFO
--rw-r--r--   0 sammko    (1000) sammko    (1000)     1231 2020-06-05 11:41:42.000000 picomc-0.4.5/README.md
--rw-r--r--   0 sammko    (1000) sammko    (1000)     1700 2020-07-10 00:26:29.000000 picomc-0.4.5/distversion.py
-drwxr-xr-x   0 sammko    (1000) sammko    (1000)        0 2022-02-20 20:31:42.631341 picomc-0.4.5/picomc/
--rw-r--r--   0 sammko    (1000) sammko    (1000)      401 2020-09-04 11:03:21.000000 picomc-0.4.5/picomc/__init__.py
--rwxr-xr-x   0 sammko    (1000) sammko    (1000)       82 2020-05-20 00:05:19.000000 picomc-0.4.5/picomc/__main__.py
--rw-r--r--   0 sammko    (1000) sammko    (1000)       64 2022-02-20 20:31:42.631341 picomc-0.4.5/picomc/_version.py
--rw-r--r--   0 sammko    (1000) sammko    (1000)     6598 2022-02-20 18:20:24.000000 picomc-0.4.5/picomc/account.py
-drwxr-xr-x   0 sammko    (1000) sammko    (1000)        0 2022-02-20 20:31:42.630341 picomc-0.4.5/picomc/cli/
--rw-r--r--   0 sammko    (1000) sammko    (1000)      459 2020-07-30 17:28:51.000000 picomc-0.4.5/picomc/cli/__init__.py
--rw-r--r--   0 sammko    (1000) sammko    (1000)     3182 2022-02-20 18:20:24.000000 picomc-0.4.5/picomc/cli/account.py
--rw-r--r--   0 sammko    (1000) sammko    (1000)     1111 2020-07-30 17:28:51.000000 picomc-0.4.5/picomc/cli/config.py
--rw-r--r--   0 sammko    (1000) sammko    (1000)     4403 2020-09-04 10:51:11.000000 picomc-0.4.5/picomc/cli/instance.py
--rw-r--r--   0 sammko    (1000) sammko    (1000)     1378 2021-03-25 00:47:18.000000 picomc-0.4.5/picomc/cli/main.py
--rw-r--r--   0 sammko    (1000) sammko    (1000)     1018 2020-07-30 17:28:51.000000 picomc-0.4.5/picomc/cli/mod.py
--rw-r--r--   0 sammko    (1000) sammko    (1000)     1495 2021-11-06 12:26:11.000000 picomc-0.4.5/picomc/cli/play.py
--rw-r--r--   0 sammko    (1000) sammko    (1000)      701 2020-07-29 10:47:30.000000 picomc-0.4.5/picomc/cli/utils.py
--rw-r--r--   0 sammko    (1000) sammko    (1000)     2728 2020-07-30 17:28:51.000000 picomc-0.4.5/picomc/cli/version.py
--rw-r--r--   0 sammko    (1000) sammko    (1000)     4112 2020-09-05 22:27:57.000000 picomc-0.4.5/picomc/config.py
--rw-r--r--   0 sammko    (1000) sammko    (1000)     5250 2021-04-03 11:50:13.000000 picomc-0.4.5/picomc/downloader.py
--rw-r--r--   0 sammko    (1000) sammko    (1000)      181 2022-02-20 18:20:24.000000 picomc-0.4.5/picomc/errors.py
--rw-r--r--   0 sammko    (1000) sammko    (1000)     9426 2022-02-20 18:20:24.000000 picomc-0.4.5/picomc/instance.py
-drwxr-xr-x   0 sammko    (1000) sammko    (1000)        0 2022-02-20 20:31:42.630341 picomc-0.4.5/picomc/java/
--rw-r--r--   0 sammko    (1000) sammko    (1000)      538 2020-09-05 22:27:57.000000 picomc-0.4.5/picomc/java/SysDump.class
--rw-r--r--   0 sammko    (1000) sammko    (1000)       49 2020-09-05 22:27:57.000000 picomc-0.4.5/picomc/java/__init__.py
--rw-r--r--   0 sammko    (1000) sammko    (1000)     3408 2022-02-20 18:20:24.000000 picomc-0.4.5/picomc/java/javainfo.py
--rw-r--r--   0 sammko    (1000) sammko    (1000)     4128 2021-03-27 19:02:20.000000 picomc-0.4.5/picomc/launcher.py
--rw-r--r--   0 sammko    (1000) sammko    (1000)     4090 2021-03-25 00:51:23.000000 picomc-0.4.5/picomc/library.py
--rw-r--r--   0 sammko    (1000) sammko    (1000)      292 2020-07-24 23:13:32.000000 picomc-0.4.5/picomc/logging.py
-drwxr-xr-x   0 sammko    (1000) sammko    (1000)        0 2022-02-20 20:31:42.631341 picomc-0.4.5/picomc/mod/
--rw-r--r--   0 sammko    (1000) sammko    (1000)       88 2020-08-11 10:20:05.000000 picomc-0.4.5/picomc/mod/__init__.py
--rw-r--r--   0 sammko    (1000) sammko    (1000)     9249 2021-02-04 23:28:01.000000 picomc-0.4.5/picomc/mod/curse.py
--rw-r--r--   0 sammko    (1000) sammko    (1000)     4743 2020-09-05 09:41:27.000000 picomc-0.4.5/picomc/mod/fabric.py
--rw-r--r--   0 sammko    (1000) sammko    (1000)    13863 2021-11-06 12:26:11.000000 picomc-0.4.5/picomc/mod/forge.py
--rw-r--r--   0 sammko    (1000) sammko    (1000)     4941 2020-09-11 21:42:15.000000 picomc-0.4.5/picomc/mod/ftb.py
--rw-r--r--   0 sammko    (1000) sammko    (1000)     5871 2022-02-20 18:20:24.000000 picomc-0.4.5/picomc/msapi.py
--rw-r--r--   0 sammko    (1000) sammko    (1000)     1024 2020-09-05 22:27:57.000000 picomc-0.4.5/picomc/osinfo.py
--rw-r--r--   0 sammko    (1000) sammko    (1000)     1374 2020-07-24 23:13:32.000000 picomc-0.4.5/picomc/rules.py
--rw-r--r--   0 sammko    (1000) sammko    (1000)     1300 2021-03-25 00:46:41.000000 picomc-0.4.5/picomc/utils.py
--rw-r--r--   0 sammko    (1000) sammko    (1000)    15764 2021-06-09 11:43:07.000000 picomc-0.4.5/picomc/version.py
--rw-r--r--   0 sammko    (1000) sammko    (1000)     2678 2021-04-03 11:54:29.000000 picomc-0.4.5/picomc/windows.py
--rw-r--r--   0 sammko    (1000) sammko    (1000)     2548 2022-02-20 18:20:24.000000 picomc-0.4.5/picomc/yggdrasil.py
-drwxr-xr-x   0 sammko    (1000) sammko    (1000)        0 2022-02-20 20:31:42.629341 picomc-0.4.5/picomc.egg-info/
--rw-r--r--   0 sammko    (1000) sammko    (1000)      422 2022-02-20 20:31:42.000000 picomc-0.4.5/picomc.egg-info/PKG-INFO
--rw-r--r--   0 sammko    (1000) sammko    (1000)      933 2022-02-20 20:31:42.000000 picomc-0.4.5/picomc.egg-info/SOURCES.txt
--rw-r--r--   0 sammko    (1000) sammko    (1000)        1 2022-02-20 20:31:42.000000 picomc-0.4.5/picomc.egg-info/dependency_links.txt
--rw-r--r--   0 sammko    (1000) sammko    (1000)       40 2022-02-20 20:31:42.000000 picomc-0.4.5/picomc.egg-info/entry_points.txt
--rw-r--r--   0 sammko    (1000) sammko    (1000)       62 2022-02-20 20:31:42.000000 picomc-0.4.5/picomc.egg-info/requires.txt
--rw-r--r--   0 sammko    (1000) sammko    (1000)        7 2022-02-20 20:31:42.000000 picomc-0.4.5/picomc.egg-info/top_level.txt
--rw-r--r--   0 sammko    (1000) sammko    (1000)      282 2022-02-20 20:31:42.631341 picomc-0.4.5/setup.cfg
--rw-r--r--   0 sammko    (1000) sammko    (1000)      932 2022-02-20 18:20:24.000000 picomc-0.4.5/setup.py
+drwxr-xr-x   0 sammko    (1000) sammko    (1000)        0 2023-05-14 13:01:00.132005 picomc-0.4.6/
+-rw-r--r--   0 sammko    (1000) sammko    (1000)     1086 2022-02-17 13:08:34.000000 picomc-0.4.6/LICENSE
+-rw-r--r--   0 sammko    (1000) sammko    (1000)       23 2022-02-17 23:49:22.000000 picomc-0.4.6/MANIFEST.in
+-rw-r--r--   0 sammko    (1000) sammko    (1000)      394 2023-05-14 13:01:00.132005 picomc-0.4.6/PKG-INFO
+-rw-r--r--   0 sammko    (1000) sammko    (1000)     1231 2022-01-19 15:54:42.000000 picomc-0.4.6/README.md
+-rw-r--r--   0 sammko    (1000) sammko    (1000)     1700 2022-02-17 23:49:22.000000 picomc-0.4.6/distversion.py
+drwxr-xr-x   0 sammko    (1000) sammko    (1000)        0 2023-05-14 13:01:00.132005 picomc-0.4.6/picomc/
+-rw-r--r--   0 sammko    (1000) sammko    (1000)      401 2022-02-17 23:49:22.000000 picomc-0.4.6/picomc/__init__.py
+-rwxr-xr-x   0 sammko    (1000) sammko    (1000)       82 2021-11-01 16:04:48.000000 picomc-0.4.6/picomc/__main__.py
+-rw-r--r--   0 sammko    (1000) sammko    (1000)       64 2023-05-14 13:01:00.132005 picomc-0.4.6/picomc/_version.py
+-rw-r--r--   0 sammko    (1000) sammko    (1000)     6598 2022-02-17 13:08:40.000000 picomc-0.4.6/picomc/account.py
+drwxr-xr-x   0 sammko    (1000) sammko    (1000)        0 2023-05-14 13:01:00.128672 picomc-0.4.6/picomc/cli/
+-rw-r--r--   0 sammko    (1000) sammko    (1000)      459 2021-11-01 16:04:48.000000 picomc-0.4.6/picomc/cli/__init__.py
+-rw-r--r--   0 sammko    (1000) sammko    (1000)     3182 2022-02-17 13:08:40.000000 picomc-0.4.6/picomc/cli/account.py
+-rw-r--r--   0 sammko    (1000) sammko    (1000)     1111 2021-11-01 16:04:48.000000 picomc-0.4.6/picomc/cli/config.py
+-rw-r--r--   0 sammko    (1000) sammko    (1000)     4403 2021-11-01 16:04:48.000000 picomc-0.4.6/picomc/cli/instance.py
+-rw-r--r--   0 sammko    (1000) sammko    (1000)     1378 2021-11-01 16:04:48.000000 picomc-0.4.6/picomc/cli/main.py
+-rw-r--r--   0 sammko    (1000) sammko    (1000)     1018 2021-11-01 16:04:48.000000 picomc-0.4.6/picomc/cli/mod.py
+-rw-r--r--   0 sammko    (1000) sammko    (1000)     1495 2021-11-04 17:28:48.000000 picomc-0.4.6/picomc/cli/play.py
+-rw-r--r--   0 sammko    (1000) sammko    (1000)      701 2021-11-01 16:04:48.000000 picomc-0.4.6/picomc/cli/utils.py
+-rw-r--r--   0 sammko    (1000) sammko    (1000)     2728 2021-11-01 16:04:48.000000 picomc-0.4.6/picomc/cli/version.py
+-rw-r--r--   0 sammko    (1000) sammko    (1000)     4112 2021-11-01 16:04:48.000000 picomc-0.4.6/picomc/config.py
+-rw-r--r--   0 sammko    (1000) sammko    (1000)     5250 2021-11-01 16:04:48.000000 picomc-0.4.6/picomc/downloader.py
+-rw-r--r--   0 sammko    (1000) sammko    (1000)      181 2022-02-17 13:08:40.000000 picomc-0.4.6/picomc/errors.py
+-rw-r--r--   0 sammko    (1000) sammko    (1000)     9426 2022-02-17 13:08:40.000000 picomc-0.4.6/picomc/instance.py
+drwxr-xr-x   0 sammko    (1000) sammko    (1000)        0 2023-05-14 13:01:00.132005 picomc-0.4.6/picomc/java/
+-rw-r--r--   0 sammko    (1000) sammko    (1000)      538 2021-11-01 16:04:48.000000 picomc-0.4.6/picomc/java/SysDump.class
+-rw-r--r--   0 sammko    (1000) sammko    (1000)       49 2021-11-01 16:04:48.000000 picomc-0.4.6/picomc/java/__init__.py
+-rw-r--r--   0 sammko    (1000) sammko    (1000)     3408 2022-02-18 01:18:32.000000 picomc-0.4.6/picomc/java/javainfo.py
+-rw-r--r--   0 sammko    (1000) sammko    (1000)     4128 2021-11-01 16:04:48.000000 picomc-0.4.6/picomc/launcher.py
+-rw-r--r--   0 sammko    (1000) sammko    (1000)     4090 2021-11-01 16:26:56.000000 picomc-0.4.6/picomc/library.py
+-rw-r--r--   0 sammko    (1000) sammko    (1000)      292 2021-11-01 16:04:48.000000 picomc-0.4.6/picomc/logging.py
+drwxr-xr-x   0 sammko    (1000) sammko    (1000)        0 2023-05-14 13:01:00.132005 picomc-0.4.6/picomc/mod/
+-rw-r--r--   0 sammko    (1000) sammko    (1000)       88 2021-11-01 16:04:48.000000 picomc-0.4.6/picomc/mod/__init__.py
+-rw-r--r--   0 sammko    (1000) sammko    (1000)     9470 2022-09-25 19:33:29.000000 picomc-0.4.6/picomc/mod/curse.py
+-rw-r--r--   0 sammko    (1000) sammko    (1000)     4743 2021-11-01 16:04:48.000000 picomc-0.4.6/picomc/mod/fabric.py
+-rw-r--r--   0 sammko    (1000) sammko    (1000)    13863 2021-11-04 16:05:26.000000 picomc-0.4.6/picomc/mod/forge.py
+-rw-r--r--   0 sammko    (1000) sammko    (1000)     4949 2022-09-25 19:33:29.000000 picomc-0.4.6/picomc/mod/ftb.py
+-rw-r--r--   0 sammko    (1000) sammko    (1000)     5871 2022-02-18 01:57:00.000000 picomc-0.4.6/picomc/msapi.py
+-rw-r--r--   0 sammko    (1000) sammko    (1000)     1024 2021-11-01 16:04:48.000000 picomc-0.4.6/picomc/osinfo.py
+-rw-r--r--   0 sammko    (1000) sammko    (1000)     1374 2021-11-01 16:04:48.000000 picomc-0.4.6/picomc/rules.py
+-rw-r--r--   0 sammko    (1000) sammko    (1000)     1300 2021-11-01 16:04:48.000000 picomc-0.4.6/picomc/utils.py
+-rw-r--r--   0 sammko    (1000) sammko    (1000)    15765 2023-01-31 16:59:10.000000 picomc-0.4.6/picomc/version.py
+-rw-r--r--   0 sammko    (1000) sammko    (1000)     2678 2021-11-01 16:04:48.000000 picomc-0.4.6/picomc/windows.py
+-rw-r--r--   0 sammko    (1000) sammko    (1000)     2548 2022-02-17 13:08:40.000000 picomc-0.4.6/picomc/yggdrasil.py
+drwxr-xr-x   0 sammko    (1000) sammko    (1000)        0 2023-05-14 13:01:00.128672 picomc-0.4.6/picomc.egg-info/
+-rw-r--r--   0 sammko    (1000) sammko    (1000)      394 2023-05-14 13:01:00.000000 picomc-0.4.6/picomc.egg-info/PKG-INFO
+-rw-r--r--   0 sammko    (1000) sammko    (1000)      933 2023-05-14 13:01:00.000000 picomc-0.4.6/picomc.egg-info/SOURCES.txt
+-rw-r--r--   0 sammko    (1000) sammko    (1000)        1 2023-05-14 13:01:00.000000 picomc-0.4.6/picomc.egg-info/dependency_links.txt
+-rw-r--r--   0 sammko    (1000) sammko    (1000)       39 2023-05-14 13:01:00.000000 picomc-0.4.6/picomc.egg-info/entry_points.txt
+-rw-r--r--   0 sammko    (1000) sammko    (1000)       62 2023-05-14 13:01:00.000000 picomc-0.4.6/picomc.egg-info/requires.txt
+-rw-r--r--   0 sammko    (1000) sammko    (1000)        7 2023-05-14 13:01:00.000000 picomc-0.4.6/picomc.egg-info/top_level.txt
+-rw-r--r--   0 sammko    (1000) sammko    (1000)      282 2023-05-14 13:01:00.132005 picomc-0.4.6/setup.cfg
+-rw-r--r--   0 sammko    (1000) sammko    (1000)      932 2022-02-18 01:04:57.000000 picomc-0.4.6/setup.py
```

### Comparing `picomc-0.4.5/LICENSE` & `picomc-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `picomc-0.4.5/README.md` & `picomc-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `picomc-0.4.5/distversion.py` & `picomc-0.4.6/distversion.py`

 * *Files identical despite different names*

### Comparing `picomc-0.4.5/picomc/account.py` & `picomc-0.4.6/picomc/account.py`

 * *Files identical despite different names*

### Comparing `picomc-0.4.5/picomc/cli/account.py` & `picomc-0.4.6/picomc/cli/account.py`

 * *Files identical despite different names*

### Comparing `picomc-0.4.5/picomc/cli/config.py` & `picomc-0.4.6/picomc/cli/config.py`

 * *Files identical despite different names*

### Comparing `picomc-0.4.5/picomc/cli/instance.py` & `picomc-0.4.6/picomc/cli/instance.py`

 * *Files identical despite different names*

### Comparing `picomc-0.4.5/picomc/cli/main.py` & `picomc-0.4.6/picomc/cli/main.py`

 * *Files identical despite different names*

### Comparing `picomc-0.4.5/picomc/cli/mod.py` & `picomc-0.4.6/picomc/cli/mod.py`

 * *Files identical despite different names*

### Comparing `picomc-0.4.5/picomc/cli/play.py` & `picomc-0.4.6/picomc/cli/play.py`

 * *Files identical despite different names*

### Comparing `picomc-0.4.5/picomc/cli/utils.py` & `picomc-0.4.6/picomc/cli/utils.py`

 * *Files identical despite different names*

### Comparing `picomc-0.4.5/picomc/cli/version.py` & `picomc-0.4.6/picomc/cli/version.py`

 * *Files identical despite different names*

### Comparing `picomc-0.4.5/picomc/config.py` & `picomc-0.4.6/picomc/config.py`

 * *Files identical despite different names*

### Comparing `picomc-0.4.5/picomc/downloader.py` & `picomc-0.4.6/picomc/downloader.py`

 * *Files identical despite different names*

### Comparing `picomc-0.4.5/picomc/instance.py` & `picomc-0.4.6/picomc/instance.py`

 * *Files identical despite different names*

### Comparing `picomc-0.4.5/picomc/java/SysDump.class` & `picomc-0.4.6/picomc/java/SysDump.class`

 * *Files identical despite different names*

### Comparing `picomc-0.4.5/picomc/java/javainfo.py` & `picomc-0.4.6/picomc/java/javainfo.py`

 * *Files identical despite different names*

### Comparing `picomc-0.4.5/picomc/launcher.py` & `picomc-0.4.6/picomc/launcher.py`

 * *Files identical despite different names*

### Comparing `picomc-0.4.5/picomc/library.py` & `picomc-0.4.6/picomc/library.py`

 * *Files identical despite different names*

### Comparing `picomc-0.4.5/picomc/mod/curse.py` & `picomc-0.4.6/picomc/mod/curse.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,21 @@
         return path
     regex = r"^(https:\/\/|twitch:\/\/)www\.curseforge\.com\/minecraft\/modpacks\/[-a-z0-9]+\/(download|download-client|files)\/(\d+)(\/file|\?client=y|)$"
     match = re.match(regex, path)
     if match:
         file_id = match.group(3)
         return get_file_url(file_id)
     else:
-        raise ValueError("Unsupported URL")
+        regex = r"^curseforge:\/\/install\?addonId=\d+&fileId=(\d+)"
+        match = re.match(regex, path)
+        if match:
+            file_id = match.group(1)
+            return get_file_url(file_id)
+        else:
+            raise ValueError("Unsupported URL")
 
 
 def resolve_ccip(filename):
     xml = ElementTree.parse(filename)
     proj_attr = xml.find("project").attrib
     return get_file_url(proj_attr["file"], proj_attr["id"])
```

### Comparing `picomc-0.4.5/picomc/mod/fabric.py` & `picomc-0.4.6/picomc/mod/fabric.py`

 * *Files identical despite different names*

### Comparing `picomc-0.4.5/picomc/mod/forge.py` & `picomc-0.4.6/picomc/mod/forge.py`

 * *Files identical despite different names*

### Comparing `picomc-0.4.5/picomc/mod/ftb.py` & `picomc-0.4.6/picomc/mod/ftb.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,15 @@
                 version_id = version["id"]
                 break
         else:
             raise InvalidVersionError(pack_version)
     else:
 
         def filt(v):
-            return use_beta or v["type"] == "Release"
+            return use_beta or v["type"].lower() == "release"
 
         filtered_versions = filter(filt, pack_manifest["versions"])
         version_id = max(filtered_versions, key=itemgetter("updated"))["id"]
 
     return pack_manifest, get_version_manifest(pack_id, version_id)
```

### Comparing `picomc-0.4.5/picomc/msapi.py` & `picomc-0.4.6/picomc/msapi.py`

 * *Files identical despite different names*

### Comparing `picomc-0.4.5/picomc/osinfo.py` & `picomc-0.4.6/picomc/osinfo.py`

 * *Files identical despite different names*

### Comparing `picomc-0.4.5/picomc/rules.py` & `picomc-0.4.6/picomc/rules.py`

 * *Files identical despite different names*

### Comparing `picomc-0.4.5/picomc/utils.py` & `picomc-0.4.6/picomc/utils.py`

 * *Files identical despite different names*

### Comparing `picomc-0.4.5/picomc/version.py` & `picomc-0.4.6/picomc/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
             self.assetIndex = LEGACY_ASSETS
         self.libraries = self.attr_reduce("libraries", lambda x, y: y + x)
         self.jar = self.attr_override("jar", default=self.vobj.version_name)
         self.downloads = self.attr_override("downloads", default={})
 
 
 class Version:
-    ASSETS_URL = "http://resources.download.minecraft.net/"
+    ASSETS_URL = "https://resources.download.minecraft.net/"
 
     def __init__(self, version_name, launcher, version_manifest):
         self.version_name = version_name
         self.launcher = launcher
         self.vm = launcher.version_manager
         self.version_manifest = version_manifest
         self._libraries = dict()
```

### Comparing `picomc-0.4.5/picomc/windows.py` & `picomc-0.4.6/picomc/windows.py`

 * *Files identical despite different names*

### Comparing `picomc-0.4.5/picomc/yggdrasil.py` & `picomc-0.4.6/picomc/yggdrasil.py`

 * *Files identical despite different names*

### Comparing `picomc-0.4.5/picomc.egg-info/SOURCES.txt` & `picomc-0.4.6/picomc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `picomc-0.4.5/setup.py` & `picomc-0.4.6/setup.py`

 * *Files identical despite different names*

