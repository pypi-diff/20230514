# Comparing `tmp/multibotkit-0.1.8.tar.gz` & `tmp/multibotkit-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multibotkit-0.1.8.tar", last modified: Tue Mar 21 14:05:46 2023, max compression
+gzip compressed data, was "multibotkit-0.1.9.tar", last modified: Tue Apr 11 17:07:03 2023, max compression
```

## Comparing `multibotkit-0.1.8.tar` & `multibotkit-0.1.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:05:46.350743 multibotkit-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-21 14:05:41.000000 multibotkit-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-21 14:05:46.350743 multibotkit-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-21 14:05:41.000000 multibotkit-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:05:46.346743 multibotkit-0.1.8/multibotkit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:05:46.350743 multibotkit-0.1.8/multibotkit/dispatchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/dispatchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/dispatchers/base_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/dispatchers/fb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/dispatchers/telegram.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/dispatchers/viber.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/dispatchers/vk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:05:46.350743 multibotkit-0.1.8/multibotkit/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/helpers/base_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/helpers/fb.py
--rw-r--r--   0 runner    (1001) docker     (123)    39952 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/helpers/telegram.py
--rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/helpers/viber.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/helpers/vk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:05:46.350743 multibotkit-0.1.8/multibotkit/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:05:46.350743 multibotkit-0.1.8/multibotkit/schemas/fb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/schemas/fb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/schemas/fb/incoming.py
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/schemas/fb/outgoing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:05:46.350743 multibotkit-0.1.8/multibotkit/schemas/telegram/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/schemas/telegram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/schemas/telegram/incoming.py
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/schemas/telegram/outgoing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:05:46.350743 multibotkit-0.1.8/multibotkit/schemas/viber/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/schemas/viber/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/schemas/viber/incoming.py
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/schemas/viber/outgoing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:05:46.350743 multibotkit-0.1.8/multibotkit/schemas/vk/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/schemas/vk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2063 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/schemas/vk/incoming.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3918 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/schemas/vk/outgoing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:05:46.350743 multibotkit-0.1.8/multibotkit/states/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/states/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:05:46.350743 multibotkit-0.1.8/multibotkit/states/managers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/states/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/states/managers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/states/managers/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/states/managers/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/states/managers/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-03-21 14:05:41.000000 multibotkit-0.1.8/multibotkit/states/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:05:46.350743 multibotkit-0.1.8/multibotkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-21 14:05:46.000000 multibotkit-0.1.8/multibotkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-03-21 14:05:46.000000 multibotkit-0.1.8/multibotkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 14:05:46.000000 multibotkit-0.1.8/multibotkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-21 14:05:46.000000 multibotkit-0.1.8/multibotkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-21 14:05:46.000000 multibotkit-0.1.8/multibotkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-21 14:05:41.000000 multibotkit-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 14:05:46.350743 multibotkit-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-21 14:05:41.000000 multibotkit-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:07:03.231964 multibotkit-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-11 17:06:59.000000 multibotkit-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-11 17:07:03.231964 multibotkit-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-11 17:06:59.000000 multibotkit-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:07:03.227964 multibotkit-0.1.9/multibotkit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:07:03.227964 multibotkit-0.1.9/multibotkit/dispatchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/dispatchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/dispatchers/base_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/dispatchers/fb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/dispatchers/telegram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/dispatchers/viber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/dispatchers/vk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:07:03.227964 multibotkit-0.1.9/multibotkit/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/helpers/base_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/helpers/fb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42592 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/helpers/telegram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/helpers/viber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/helpers/vk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:07:03.227964 multibotkit-0.1.9/multibotkit/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:07:03.231964 multibotkit-0.1.9/multibotkit/schemas/fb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/schemas/fb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/schemas/fb/incoming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/schemas/fb/outgoing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:07:03.231964 multibotkit-0.1.9/multibotkit/schemas/telegram/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/schemas/telegram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/schemas/telegram/incoming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/schemas/telegram/outgoing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:07:03.231964 multibotkit-0.1.9/multibotkit/schemas/viber/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/schemas/viber/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/schemas/viber/incoming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/schemas/viber/outgoing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:07:03.231964 multibotkit-0.1.9/multibotkit/schemas/vk/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/schemas/vk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2063 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/schemas/vk/incoming.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3918 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/schemas/vk/outgoing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:07:03.231964 multibotkit-0.1.9/multibotkit/states/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/states/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:07:03.231964 multibotkit-0.1.9/multibotkit/states/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/states/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/states/managers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/states/managers/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/states/managers/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/states/managers/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-11 17:06:59.000000 multibotkit-0.1.9/multibotkit/states/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:07:03.227964 multibotkit-0.1.9/multibotkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-11 17:07:03.000000 multibotkit-0.1.9/multibotkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-11 17:07:03.000000 multibotkit-0.1.9/multibotkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:07:03.000000 multibotkit-0.1.9/multibotkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-11 17:07:03.000000 multibotkit-0.1.9/multibotkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 17:07:03.000000 multibotkit-0.1.9/multibotkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-11 17:06:59.000000 multibotkit-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 17:07:03.231964 multibotkit-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-11 17:06:59.000000 multibotkit-0.1.9/setup.py
```

### Comparing `multibotkit-0.1.8/LICENSE` & `multibotkit-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `multibotkit-0.1.8/PKG-INFO` & `multibotkit-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multibotkit
-Version: 0.1.8
+Version: 0.1.9
 Summary: Functional library for developing multiplatform chatbots
 Home-page: https://github.com/Appvelox/multibotkit
 Author: Appvelox LLC
 Author-email: team@appvelox.ru
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `multibotkit-0.1.8/multibotkit/dispatchers/base_dispatcher.py` & `multibotkit-0.1.9/multibotkit/dispatchers/base_dispatcher.py`

 * *Files identical despite different names*

### Comparing `multibotkit-0.1.8/multibotkit/dispatchers/fb.py` & `multibotkit-0.1.9/multibotkit/dispatchers/fb.py`

 * *Files identical despite different names*

### Comparing `multibotkit-0.1.8/multibotkit/dispatchers/telegram.py` & `multibotkit-0.1.9/multibotkit/dispatchers/telegram.py`

 * *Files identical despite different names*

### Comparing `multibotkit-0.1.8/multibotkit/dispatchers/viber.py` & `multibotkit-0.1.9/multibotkit/dispatchers/viber.py`

 * *Files identical despite different names*

### Comparing `multibotkit-0.1.8/multibotkit/dispatchers/vk.py` & `multibotkit-0.1.9/multibotkit/dispatchers/vk.py`

 * *Files identical despite different names*

### Comparing `multibotkit-0.1.8/multibotkit/helpers/base_helper.py` & `multibotkit-0.1.9/multibotkit/helpers/base_helper.py`

 * *Files identical despite different names*

### Comparing `multibotkit-0.1.8/multibotkit/helpers/fb.py` & `multibotkit-0.1.9/multibotkit/helpers/fb.py`

 * *Files identical despite different names*

### Comparing `multibotkit-0.1.8/multibotkit/helpers/telegram.py` & `multibotkit-0.1.9/multibotkit/helpers/telegram.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     InputMediaPhoto,
     Message,
     Photo,
     ReplyKeyboardMarkup,
     SetWebhookParams,
     WebhookInfo,
     MediaGroup, ReplyKeyboardRemove,
+    Sticker
 )
 
 
 class TelegramHelper(BaseHelper):
     """
     Sync and async functions for Telegram Bot API
     """
@@ -1071,7 +1072,81 @@
 
         if len(files.keys()):
             r = await self._perform_async_request(url, data, use_json=False, files=files)
             return r
         
         r = await self._perform_async_request(url, data)
         return r
+
+    async def async_send_sticker(
+            self,
+            chat_id: int,
+            sticker: str,
+            disable_notification: Optional[bool] = None,
+            protect_content: Optional[bool] = None,
+            reply_to_message_id: Optional[int] = None,
+            allow_sending_without_reply: Optional[bool] = None,
+            reply_markup: Optional[Union[InlineKeyboardMarkup, ReplyKeyboardMarkup]] = None
+    ):
+        sticker_obj = Sticker(
+            chat_id=chat_id,
+            sticker=sticker,
+            disable_notification=disable_notification,
+            protect_content=protect_content,
+            reply_to_message_id=reply_to_message_id,
+            allow_sending_without_reply=allow_sending_without_reply,
+            reply_markup=reply_markup
+        )
+
+        url = self.tg_base_url + "sendSticker"
+        data = sticker_obj.dict(exclude_none=True)
+        if "reply_markup" in data.keys():
+            data["reply_markup"] = json.dumps(data["reply_markup"])
+
+        r = await self._perform_async_request(url, data)
+        return r
+
+    def sync_send_sticker(
+            self,
+            chat_id: int,
+            sticker: str,
+            disable_notification: Optional[bool] = None,
+            protect_content: Optional[bool] = None,
+            reply_to_message_id: Optional[int] = None,
+            allow_sending_without_reply: Optional[bool] = None,
+            reply_markup: Optional[Union[InlineKeyboardMarkup, ReplyKeyboardMarkup]] = None
+    ):
+        sticker_obj = Sticker(
+            chat_id=chat_id,
+            sticker=sticker,
+            disable_notification=disable_notification,
+            protect_content=protect_content,
+            reply_to_message_id=reply_to_message_id,
+            allow_sending_without_reply=allow_sending_without_reply,
+            reply_markup=reply_markup
+        )
+
+        url = self.tg_base_url + "sendSticker"
+        data = sticker_obj.dict(exclude_none=True)
+        if "reply_markup" in data.keys():
+            data["reply_markup"] = json.dumps(data["reply_markup"])
+
+        r = self._perform_sync_request(url, data)
+        return r
+
+    def sync_get_sticker_set(
+            self,
+            sticker_set: str,
+    ):
+        url = self.tg_base_url + "getStickerSet"
+        data = {"name": sticker_set}
+        r = self._perform_sync_request(url, data)
+        return r
+
+    async def async_get_sticker_set(
+            self,
+            sticker_set: str,
+    ):
+        url = self.tg_base_url + "getStickerSet"
+        data = {"name": sticker_set}
+        r = await self._perform_async_request(url, data)
+        return r
```

### Comparing `multibotkit-0.1.8/multibotkit/helpers/viber.py` & `multibotkit-0.1.9/multibotkit/helpers/viber.py`

 * *Files identical despite different names*

### Comparing `multibotkit-0.1.8/multibotkit/helpers/vk.py` & `multibotkit-0.1.9/multibotkit/helpers/vk.py`

 * *Files identical despite different names*

### Comparing `multibotkit-0.1.8/multibotkit/schemas/fb/incoming.py` & `multibotkit-0.1.9/multibotkit/schemas/fb/incoming.py`

 * *Files identical despite different names*

### Comparing `multibotkit-0.1.8/multibotkit/schemas/fb/outgoing.py` & `multibotkit-0.1.9/multibotkit/schemas/fb/outgoing.py`

 * *Files identical despite different names*

### Comparing `multibotkit-0.1.8/multibotkit/schemas/telegram/incoming.py` & `multibotkit-0.1.9/multibotkit/schemas/telegram/incoming.py`

 * *Files identical despite different names*

### Comparing `multibotkit-0.1.8/multibotkit/schemas/telegram/outgoing.py` & `multibotkit-0.1.9/multibotkit/schemas/telegram/outgoing.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,7 +214,17 @@
     title: Optional[str] = Field(None, title="Title")
     thumbnail: Optional[str] = Field(None, title="document thumbnail")
     disable_notification: Optional[bool] = Field(None, title="disable notification")
     protect_content: Optional[bool] = Field(None, title="protect content")
     reply_to_message_id: Optional[int] = Field(None, title="reply to message id")
     allow_sending_without_reply: Optional[bool] = Field(None, title="allow sending without reply")
     reply_markup: Optional[Union[InlineKeyboardMarkup, ReplyKeyboardMarkup]] = Field(None, title="reply markup")
+
+
+class Sticker(BaseModel):
+    chat_id: int = Field(..., title="chat id")
+    sticker: str = Field(..., title="document")
+    disable_notification: Optional[bool] = Field(None, title="disable notification")
+    protect_content: Optional[bool] = Field(None, title="protect content")
+    reply_to_message_id: Optional[int] = Field(None, title="reply to message id")
+    allow_sending_without_reply: Optional[bool] = Field(None, title="allow sending without reply")
+    reply_markup: Optional[Union[InlineKeyboardMarkup, ReplyKeyboardMarkup]] = Field(None, title="reply markup")
```

### Comparing `multibotkit-0.1.8/multibotkit/schemas/viber/incoming.py` & `multibotkit-0.1.9/multibotkit/schemas/viber/incoming.py`

 * *Files identical despite different names*

### Comparing `multibotkit-0.1.8/multibotkit/schemas/viber/outgoing.py` & `multibotkit-0.1.9/multibotkit/schemas/viber/outgoing.py`

 * *Files identical despite different names*

### Comparing `multibotkit-0.1.8/multibotkit/schemas/vk/incoming.py` & `multibotkit-0.1.9/multibotkit/schemas/vk/incoming.py`

 * *Files identical despite different names*

### Comparing `multibotkit-0.1.8/multibotkit/schemas/vk/outgoing.py` & `multibotkit-0.1.9/multibotkit/schemas/vk/outgoing.py`

 * *Files identical despite different names*

### Comparing `multibotkit-0.1.8/multibotkit/states/managers/memory.py` & `multibotkit-0.1.9/multibotkit/states/managers/memory.py`

 * *Files identical despite different names*

### Comparing `multibotkit-0.1.8/multibotkit/states/managers/mongo.py` & `multibotkit-0.1.9/multibotkit/states/managers/mongo.py`

 * *Files identical despite different names*

### Comparing `multibotkit-0.1.8/multibotkit/states/managers/redis.py` & `multibotkit-0.1.9/multibotkit/states/managers/redis.py`

 * *Files identical despite different names*

### Comparing `multibotkit-0.1.8/multibotkit/states/state.py` & `multibotkit-0.1.9/multibotkit/states/state.py`

 * *Files identical despite different names*

### Comparing `multibotkit-0.1.8/multibotkit.egg-info/PKG-INFO` & `multibotkit-0.1.9/multibotkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multibotkit
-Version: 0.1.8
+Version: 0.1.9
 Summary: Functional library for developing multiplatform chatbots
 Home-page: https://github.com/Appvelox/multibotkit
 Author: Appvelox LLC
 Author-email: team@appvelox.ru
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `multibotkit-0.1.8/multibotkit.egg-info/SOURCES.txt` & `multibotkit-0.1.9/multibotkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multibotkit-0.1.8/setup.py` & `multibotkit-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="multibotkit",
-    version="0.1.8",
+    version="0.1.9",
     author="Appvelox LLC",
     author_email="team@appvelox.ru",
     description="Functional library for developing multiplatform chatbots",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Appvelox/multibotkit",
     packages=setuptools.find_packages(exclude=["tests*", "examples*"]),
```

