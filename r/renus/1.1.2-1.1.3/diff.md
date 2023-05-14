# Comparing `tmp/renus-1.1.2.tar.gz` & `tmp/renus-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renus-1.1.2.tar", last modified: Wed May  3 09:44:01 2023, max compression
+gzip compressed data, was "renus-1.1.3.tar", last modified: Sun May 14 05:42:37 2023, max compression
```

## Comparing `renus-1.1.2.tar` & `renus-1.1.3.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 09:44:01.442286 renus-1.1.2/
--rw-rw-rw-   0        0        0     1539 2022-12-08 07:04:23.000000 renus-1.1.2/LICENSE
--rw-rw-rw-   0        0        0       37 2023-04-20 05:31:47.000000 renus-1.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      220 2023-05-03 09:44:01.442286 renus-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0        7 2022-12-05 06:16:54.000000 renus-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 09:44:00.871275 renus-1.1.2/renus/
--rw-rw-rw-   0        0        0        0 2023-04-20 05:37:22.000000 renus-1.1.2/renus/__init__.py
--rw-rw-rw-   0        0        0     7705 2022-12-08 08:01:10.000000 renus-1.1.2/renus/app.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:44:00.936277 renus-1.1.2/renus/commands/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.2/renus/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:44:00.983274 renus-1.1.2/renus/commands/app/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.2/renus/commands/app/__init__.py
--rw-rw-rw-   0        0        0     1786 2023-05-03 04:46:26.000000 renus-1.1.2/renus/commands/app/controller.temp
--rw-rw-rw-   0        0        0     1008 2023-05-03 09:35:45.000000 renus-1.1.2/renus/commands/app/model.temp
--rw-rw-rw-   0        0        0      518 2023-03-14 08:51:15.000000 renus-1.1.2/renus/commands/app/route.temp
--rw-rw-rw-   0        0        0     4144 2022-10-15 05:56:43.000000 renus-1.1.2/renus/commands/app/run.py
--rw-rw-rw-   0        0        0      211 2022-10-09 08:00:32.000000 renus-1.1.2/renus/commands/app/vue.temp
-drwxrwxrwx   0        0        0        0 2023-05-03 09:44:01.008397 renus-1.1.2/renus/commands/backup/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.2/renus/commands/backup/__init__.py
--rw-rw-rw-   0        0        0     1522 2023-04-01 10:04:36.000000 renus-1.1.2/renus/commands/backup/run.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:44:01.017381 renus-1.1.2/renus/commands/copy/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.2/renus/commands/copy/__init__.py
--rw-rw-rw-   0        0        0     1768 2023-04-01 10:04:36.000000 renus-1.1.2/renus/commands/copy/run.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:44:01.025397 renus-1.1.2/renus/commands/default/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.2/renus/commands/default/__init__.py
--rw-rw-rw-   0        0        0     1380 2023-04-30 01:41:46.000000 renus-1.1.2/renus/commands/default/run.py
--rw-rw-rw-   0        0        0     1416 2023-04-15 07:24:18.000000 renus-1.1.2/renus/commands/help.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:44:01.082191 renus-1.1.2/renus/commands/install/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.2/renus/commands/install/__init__.py
--rw-rw-rw-   0        0        0     4079 2023-03-12 17:31:41.000000 renus-1.1.2/renus/commands/install/build.py
--rw-rw-rw-   0        0        0     3946 2023-03-12 07:22:04.000000 renus-1.1.2/renus/commands/install/run.py
--rw-rw-rw-   0        0        0     1025 2023-03-02 07:29:31.000000 renus-1.1.2/renus/commands/install/service.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:44:01.090174 renus-1.1.2/renus/commands/permission/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.2/renus/commands/permission/__init__.py
--rw-rw-rw-   0        0        0      763 2023-04-30 01:38:29.000000 renus-1.1.2/renus/commands/permission/run.py
--rw-rw-rw-   0        0        0      372 2022-08-01 09:27:06.000000 renus-1.1.2/renus/commands/run.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:44:01.393490 renus-1.1.2/renus/core/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.2/renus/core/__init__.py
--rw-rw-rw-   0        0        0     5695 2022-09-25 10:11:54.000000 renus-1.1.2/renus/core/cache.py
--rw-rw-rw-   0        0        0     1442 2022-08-01 09:27:06.000000 renus-1.1.2/renus/core/concurrency.py
--rw-rw-rw-   0        0        0      442 2022-08-01 09:27:06.000000 renus-1.1.2/renus/core/config.py
--rw-rw-rw-   0        0        0     2158 2023-05-03 09:30:03.000000 renus-1.1.2/renus/core/cprint.py
--rw-rw-rw-   0        0        0     2098 2023-04-15 09:01:12.000000 renus-1.1.2/renus/core/crypt.py
--rw-rw-rw-   0        0        0     4968 2022-08-01 09:27:06.000000 renus-1.1.2/renus/core/datastructures.py
--rw-rw-rw-   0        0        0     1894 2022-11-21 07:22:01.000000 renus-1.1.2/renus/core/exception.py
--rw-rw-rw-   0        0        0     8588 2022-09-25 10:17:27.000000 renus-1.1.2/renus/core/formparsers.py
--rw-rw-rw-   0        0        0     3918 2022-08-10 04:50:38.000000 renus-1.1.2/renus/core/injection.py
--rw-rw-rw-   0        0        0      647 2022-08-01 09:27:06.000000 renus-1.1.2/renus/core/log.py
--rw-rw-rw-   0        0        0      427 2022-08-01 09:27:06.000000 renus-1.1.2/renus/core/middleware.py
--rw-rw-rw-   0        0        0    14800 2023-04-20 18:01:14.000000 renus-1.1.2/renus/core/model.py
--rw-rw-rw-   0        0        0     6580 2023-03-12 15:37:00.000000 renus-1.1.2/renus/core/request.py
--rw-rw-rw-   0        0        0    15219 2023-02-08 08:59:43.000000 renus-1.1.2/renus/core/response.py
--rw-rw-rw-   0        0        0     7911 2023-01-22 09:11:31.000000 renus-1.1.2/renus/core/routing.py
--rw-rw-rw-   0        0        0     7256 2022-09-03 10:48:49.000000 renus-1.1.2/renus/core/schedule.py
--rw-rw-rw-   0        0        0     1448 2023-01-22 09:14:04.000000 renus-1.1.2/renus/core/serialize.py
--rw-rw-rw-   0        0        0     2933 2022-08-01 09:27:06.000000 renus-1.1.2/renus/core/status.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:44:01.431285 renus-1.1.2/renus/core/validation/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.2/renus/core/validation/__init__.py
--rw-rw-rw-   0        0        0     8773 2022-10-23 08:35:28.000000 renus-1.1.2/renus/core/validation/rules.py
--rw-rw-rw-   0        0        0     3235 2022-08-31 08:30:44.000000 renus-1.1.2/renus/core/validation/validate.py
--rw-rw-rw-   0        0        0     5857 2022-08-01 09:27:06.000000 renus-1.1.2/renus/core/websockets.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:44:01.441302 renus-1.1.2/renus/util/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.2/renus/util/__init__.py
--rw-rw-rw-   0        0        0     2348 2023-01-22 09:11:31.000000 renus-1.1.2/renus/util/helper.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:44:00.890276 renus-1.1.2/renus.egg-info/
--rw-rw-rw-   0        0        0      220 2023-05-03 09:44:00.000000 renus-1.1.2/renus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1426 2023-05-03 09:44:00.000000 renus-1.1.2/renus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 09:44:00.000000 renus-1.1.2/renus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-03 09:44:00.000000 renus-1.1.2/renus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 09:44:01.443285 renus-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      334 2023-05-03 09:20:03.000000 renus-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 05:42:37.525927 renus-1.1.3/
+-rw-rw-rw-   0        0        0     1539 2022-12-08 07:04:23.000000 renus-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0       37 2023-04-20 05:31:47.000000 renus-1.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      220 2023-05-14 05:42:37.523925 renus-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2022-12-05 06:16:54.000000 renus-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 05:42:37.351939 renus-1.1.3/renus/
+-rw-rw-rw-   0        0        0        0 2023-04-20 05:37:22.000000 renus-1.1.3/renus/__init__.py
+-rw-rw-rw-   0        0        0     7705 2022-12-08 08:01:10.000000 renus-1.1.3/renus/app.py
+drwxrwxrwx   0        0        0        0 2023-05-14 05:42:37.392960 renus-1.1.3/renus/commands/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.3/renus/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 05:42:37.410923 renus-1.1.3/renus/commands/app/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.3/renus/commands/app/__init__.py
+-rw-rw-rw-   0        0        0     1786 2023-05-03 04:46:26.000000 renus-1.1.3/renus/commands/app/controller.temp
+-rw-rw-rw-   0        0        0     1008 2023-05-03 09:35:45.000000 renus-1.1.3/renus/commands/app/model.temp
+-rw-rw-rw-   0        0        0      518 2023-03-14 08:51:15.000000 renus-1.1.3/renus/commands/app/route.temp
+-rw-rw-rw-   0        0        0     4144 2022-10-15 05:56:43.000000 renus-1.1.3/renus/commands/app/run.py
+-rw-rw-rw-   0        0        0      211 2022-10-09 08:00:32.000000 renus-1.1.3/renus/commands/app/vue.temp
+drwxrwxrwx   0        0        0        0 2023-05-14 05:42:37.416923 renus-1.1.3/renus/commands/backup/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.3/renus/commands/backup/__init__.py
+-rw-rw-rw-   0        0        0     1522 2023-04-01 10:04:36.000000 renus-1.1.3/renus/commands/backup/run.py
+drwxrwxrwx   0        0        0        0 2023-05-14 05:42:37.422959 renus-1.1.3/renus/commands/copy/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.3/renus/commands/copy/__init__.py
+-rw-rw-rw-   0        0        0     1768 2023-04-01 10:04:36.000000 renus-1.1.3/renus/commands/copy/run.py
+drwxrwxrwx   0        0        0        0 2023-05-14 05:42:37.428959 renus-1.1.3/renus/commands/default/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.3/renus/commands/default/__init__.py
+-rw-rw-rw-   0        0        0     1380 2023-04-30 01:41:46.000000 renus-1.1.3/renus/commands/default/run.py
+-rw-rw-rw-   0        0        0     1416 2023-04-15 07:24:18.000000 renus-1.1.3/renus/commands/help.py
+drwxrwxrwx   0        0        0        0 2023-05-14 05:42:37.439920 renus-1.1.3/renus/commands/install/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.3/renus/commands/install/__init__.py
+-rw-rw-rw-   0        0        0     4079 2023-03-12 17:31:41.000000 renus-1.1.3/renus/commands/install/build.py
+-rw-rw-rw-   0        0        0     3946 2023-03-12 07:22:04.000000 renus-1.1.3/renus/commands/install/run.py
+-rw-rw-rw-   0        0        0     1025 2023-03-02 07:29:31.000000 renus-1.1.3/renus/commands/install/service.py
+drwxrwxrwx   0        0        0        0 2023-05-14 05:42:37.444925 renus-1.1.3/renus/commands/permission/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.3/renus/commands/permission/__init__.py
+-rw-rw-rw-   0        0        0      763 2023-04-30 01:38:29.000000 renus-1.1.3/renus/commands/permission/run.py
+-rw-rw-rw-   0        0        0      372 2022-08-01 09:27:06.000000 renus-1.1.3/renus/commands/run.py
+drwxrwxrwx   0        0        0        0 2023-05-14 05:42:37.506927 renus-1.1.3/renus/core/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.3/renus/core/__init__.py
+-rw-rw-rw-   0        0        0     5695 2022-09-25 10:11:54.000000 renus-1.1.3/renus/core/cache.py
+-rw-rw-rw-   0        0        0     1442 2022-08-01 09:27:06.000000 renus-1.1.3/renus/core/concurrency.py
+-rw-rw-rw-   0        0        0      442 2022-08-01 09:27:06.000000 renus-1.1.3/renus/core/config.py
+-rw-rw-rw-   0        0        0     2368 2023-05-03 09:54:55.000000 renus-1.1.3/renus/core/cprint.py
+-rw-rw-rw-   0        0        0     2098 2023-04-15 09:01:12.000000 renus-1.1.3/renus/core/crypt.py
+-rw-rw-rw-   0        0        0     4968 2022-08-01 09:27:06.000000 renus-1.1.3/renus/core/datastructures.py
+-rw-rw-rw-   0        0        0     1894 2022-11-21 07:22:01.000000 renus-1.1.3/renus/core/exception.py
+-rw-rw-rw-   0        0        0     8588 2022-09-25 10:17:27.000000 renus-1.1.3/renus/core/formparsers.py
+-rw-rw-rw-   0        0        0     3918 2022-08-10 04:50:38.000000 renus-1.1.3/renus/core/injection.py
+-rw-rw-rw-   0        0        0      647 2022-08-01 09:27:06.000000 renus-1.1.3/renus/core/log.py
+-rw-rw-rw-   0        0        0      427 2022-08-01 09:27:06.000000 renus-1.1.3/renus/core/middleware.py
+-rw-rw-rw-   0        0        0    14800 2023-04-20 18:01:14.000000 renus-1.1.3/renus/core/model.py
+-rw-rw-rw-   0        0        0     6580 2023-03-12 15:37:00.000000 renus-1.1.3/renus/core/request.py
+-rw-rw-rw-   0        0        0    15219 2023-02-08 08:59:43.000000 renus-1.1.3/renus/core/response.py
+-rw-rw-rw-   0        0        0     7911 2023-01-22 09:11:31.000000 renus-1.1.3/renus/core/routing.py
+-rw-rw-rw-   0        0        0     7256 2022-09-03 10:48:49.000000 renus-1.1.3/renus/core/schedule.py
+-rw-rw-rw-   0        0        0     1448 2023-01-22 09:14:04.000000 renus-1.1.3/renus/core/serialize.py
+-rw-rw-rw-   0        0        0     2933 2022-08-01 09:27:06.000000 renus-1.1.3/renus/core/status.py
+drwxrwxrwx   0        0        0        0 2023-05-14 05:42:37.515932 renus-1.1.3/renus/core/validation/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.3/renus/core/validation/__init__.py
+-rw-rw-rw-   0        0        0     8909 2023-05-14 05:18:01.000000 renus-1.1.3/renus/core/validation/rules.py
+-rw-rw-rw-   0        0        0     3552 2023-05-14 05:22:21.000000 renus-1.1.3/renus/core/validation/validate.py
+-rw-rw-rw-   0        0        0     5857 2022-08-01 09:27:06.000000 renus-1.1.3/renus/core/websockets.py
+drwxrwxrwx   0        0        0        0 2023-05-14 05:42:37.520931 renus-1.1.3/renus/util/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.3/renus/util/__init__.py
+-rw-rw-rw-   0        0        0     2348 2023-01-22 09:11:31.000000 renus-1.1.3/renus/util/helper.py
+drwxrwxrwx   0        0        0        0 2023-05-14 05:42:37.382927 renus-1.1.3/renus.egg-info/
+-rw-rw-rw-   0        0        0      220 2023-05-14 05:42:37.000000 renus-1.1.3/renus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1426 2023-05-14 05:42:37.000000 renus-1.1.3/renus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 05:42:37.000000 renus-1.1.3/renus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-14 05:42:37.000000 renus-1.1.3/renus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 05:42:37.526935 renus-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      334 2023-05-14 05:39:59.000000 renus-1.1.3/setup.py
```

### Comparing `renus-1.1.2/LICENSE` & `renus-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/app.py` & `renus-1.1.3/renus/app.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/commands/app/controller.temp` & `renus-1.1.3/renus/commands/app/controller.temp`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/commands/app/model.temp` & `renus-1.1.3/renus/commands/app/model.temp`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/commands/app/route.temp` & `renus-1.1.3/renus/commands/app/route.temp`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/commands/app/run.py` & `renus-1.1.3/renus/commands/app/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/commands/backup/run.py` & `renus-1.1.3/renus/commands/backup/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/commands/copy/run.py` & `renus-1.1.3/renus/commands/copy/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/commands/default/run.py` & `renus-1.1.3/renus/commands/default/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/commands/help.py` & `renus-1.1.3/renus/commands/help.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/commands/install/build.py` & `renus-1.1.3/renus/commands/install/build.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/commands/install/run.py` & `renus-1.1.3/renus/commands/install/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/commands/install/service.py` & `renus-1.1.3/renus/commands/install/service.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/commands/permission/run.py` & `renus-1.1.3/renus/commands/permission/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/core/cache.py` & `renus-1.1.3/renus/core/cache.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/core/concurrency.py` & `renus-1.1.3/renus/core/concurrency.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/core/cprint.py` & `renus-1.1.3/renus/core/cprint.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from renus.core.config import Config
 
 app = Config('app')
 
 
 class Cprint:
 
-    def __init__(self) -> None:
-        self.debug = app.get('debug', False)
+    def __init__(self, debug: bool = None) -> None:
+        """
+        @param debug: by default read debug mode from Config file
+        """
+        self._debug = app.get('debug', False) if debug is None else debug
 
     def print(self, txt):
-        if self.debug:
+        """
+        print txt if debug mode is True
+        """
+        if self._debug:
             print(txt)
 
     @staticmethod
     def bold(txt):
         return f'\033[1m{txt}\033[0m'
 
     @staticmethod
```

### Comparing `renus-1.1.2/renus/core/crypt.py` & `renus-1.1.3/renus/core/crypt.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/core/datastructures.py` & `renus-1.1.3/renus/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/core/exception.py` & `renus-1.1.3/renus/core/exception.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/core/formparsers.py` & `renus-1.1.3/renus/core/formparsers.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/core/injection.py` & `renus-1.1.3/renus/core/injection.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/core/log.py` & `renus-1.1.3/renus/core/log.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/core/model.py` & `renus-1.1.3/renus/core/model.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/core/request.py` & `renus-1.1.3/renus/core/request.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/core/response.py` & `renus-1.1.3/renus/core/response.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/core/routing.py` & `renus-1.1.3/renus/core/routing.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/core/schedule.py` & `renus-1.1.3/renus/core/schedule.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/core/serialize.py` & `renus-1.1.3/renus/core/serialize.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/core/status.py` & `renus-1.1.3/renus/core/status.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/core/validation/rules.py` & `renus-1.1.3/renus/core/validation/rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,21 @@
         self.d = data
 
     def __call__(self, input):
         if input is None:
             return self.d
         return True
 
+class Convert:
+    def __init__(self, func):
+        self.f = func
+
+    def __call__(self, input):
+        return self.f(input)
+
 
 def Required(input) -> any:
     if input is not None:
         return True
     return 'required_error'
```

### Comparing `renus-1.1.2/renus/core/validation/validate.py` & `renus-1.1.3/renus/core/validation/validate.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,28 +49,37 @@
 
     def has_default(self, rules):
         for item in rules:
             if isinstance(item, vr.Default):
                 return item
         return False
 
+    def has_convert(self, rules):
+        for item in rules:
+            if isinstance(item, vr.Convert):
+                return item
+        return False
+
     def has_required(self, rules):
         for item in rules:
             if type(item) == type(vr.Required):
                 return True
         return False
 
     def rules(self, rules_data: dict, msg: str = 'invalid_data') -> dictAttribute:
         res = {}
         for field in rules_data:
             keys=field.split('.')
             val = keys_exists(self._form, keys)
             default = self.has_default(rules_data[field])
+            convert = self.has_convert(rules_data[field])
             if val is None and default is not False:
                 val = default(val)
+            if convert:
+                val=convert(val)
 
             check = self.__check(val, rules_data[field])
             if check == True:
                 set_key(res,keys,val)
             else:
                 self._error = True
                 self._msg[field] = check
@@ -81,15 +90,15 @@
 
         return dictAttribute(res)
 
     def __check(self, input, rules):
         error = False
         msg = []
         for rule in rules:
-            if rule != '$or' and not isinstance(rule, vr.Default):
+            if rule != '$or' and not isinstance(rule, vr.Default) and not isinstance(rule, vr.Convert):
                 test = rule(input)
                 if test != True:
                     error = True
                     msg.append(test)
             elif rule == '$or':
                 test = False
                 for item in rules['$or']:
```

### Comparing `renus-1.1.2/renus/core/websockets.py` & `renus-1.1.3/renus/core/websockets.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus/util/helper.py` & `renus-1.1.3/renus/util/helper.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.2/renus.egg-info/SOURCES.txt` & `renus-1.1.3/renus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

