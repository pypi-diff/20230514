# Comparing `tmp/fp_browser_sdk-0.9.1.tar.gz` & `tmp/fp_browser_sdk-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fp_browser_sdk-0.9.1.tar", last modified: Tue May  9 07:30:21 2023, max compression
+gzip compressed data, was "dist/fp_browser_sdk-0.9.2.tar", last modified: Sun May 14 03:38:48 2023, max compression
```

## Comparing `fp_browser_sdk-0.9.1.tar` & `fp_browser_sdk-0.9.2.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-09 07:30:21.000000 fp_browser_sdk-0.9.1/
--rw-r--r--   0 leeyang    (501) staff       (20)      264 2023-05-09 07:30:21.000000 fp_browser_sdk-0.9.1/PKG-INFO
--rw-r--r--   0 leeyang    (501) staff       (20)     8453 2023-02-12 04:55:25.000000 fp_browser_sdk-0.9.1/README.md
-drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-09 07:30:21.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/
--rw-r--r--   0 leeyang    (501) staff       (20)    15571 2022-12-15 04:40:42.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/__init__.py
-drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-09 07:30:21.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/data/
--rw-r--r--   0 leeyang    (501) staff       (20)        0 2022-08-05 08:21:32.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/data/__init__.py
--rw-r--r--   0 leeyang    (501) staff       (20)   183083 2022-08-16 02:45:13.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/data/motion.py
-drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-09 07:30:21.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/
--rw-r--r--   0 leeyang    (501) staff       (20)        0 2022-08-05 08:21:32.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/__init__.py
--rw-r--r--   0 leeyang    (501) staff       (20)     6386 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/basic.py
--rw-r--r--   0 leeyang    (501) staff       (20)     3212 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/battery.py
--rw-r--r--   0 leeyang    (501) staff       (20)    17258 2023-04-07 07:59:18.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/browser_enum.py
--rw-r--r--   0 leeyang    (501) staff       (20)     3357 2023-03-13 13:15:24.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/client_hints.py
--rw-r--r--   0 leeyang    (501) staff       (20)     5336 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/device_motion.py
--rw-r--r--   0 leeyang    (501) staff       (20)     2059 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/device_orientation.py
--rw-r--r--   0 leeyang    (501) staff       (20)     7142 2023-01-15 06:50:48.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/document.py
--rw-r--r--   0 leeyang    (501) staff       (20)      451 2022-08-07 03:58:52.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/exception.py
--rw-r--r--   0 leeyang    (501) staff       (20)     3291 2023-04-10 11:49:02.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/fingerprint_offset.py
--rw-r--r--   0 leeyang    (501) staff       (20)     1851 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/geo.py
--rw-r--r--   0 leeyang    (501) staff       (20)     1328 2023-05-09 07:29:43.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/gl.py
--rw-r--r--   0 leeyang    (501) staff       (20)     3266 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/header.py
--rw-r--r--   0 leeyang    (501) staff       (20)      465 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/inject_js.py
--rw-r--r--   0 leeyang    (501) staff       (20)     2223 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/media.py
--rw-r--r--   0 leeyang    (501) staff       (20)     2539 2022-08-05 07:15:01.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/module.py
--rw-r--r--   0 leeyang    (501) staff       (20)     6966 2023-05-08 07:08:22.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/navigator.py
--rw-r--r--   0 leeyang    (501) staff       (20)     3917 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/network.py
--rw-r--r--   0 leeyang    (501) staff       (20)     9140 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/performance.py
-drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-09 07:30:21.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/
--rw-r--r--   0 leeyang    (501) staff       (20)      294 2022-09-18 13:15:09.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/__init__.py
--rw-r--r--   0 leeyang    (501) staff       (20)    13786 2022-12-17 12:48:42.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/permission_type.py
--rw-r--r--   0 leeyang    (501) staff       (20)    12917 2022-09-18 13:09:11.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/permission_type_102.py
--rw-r--r--   0 leeyang    (501) staff       (20)    12683 2022-12-17 12:48:42.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/permission_type_107.py
--rw-r--r--   0 leeyang    (501) staff       (20)     9857 2022-09-18 13:09:11.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/permission_type_88.py
--rw-r--r--   0 leeyang    (501) staff       (20)    10280 2022-09-18 13:09:11.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/permission_type_90.py
--rw-r--r--   0 leeyang    (501) staff       (20)    11710 2022-09-18 13:09:11.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/permission_type_93.py
--rw-r--r--   0 leeyang    (501) staff       (20)     1049 2022-12-17 12:48:42.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/util.py
--rw-r--r--   0 leeyang    (501) staff       (20)     2087 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/plugin.py
--rw-r--r--   0 leeyang    (501) staff       (20)     3923 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/screen.py
--rw-r--r--   0 leeyang    (501) staff       (20)     2343 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/speech_synthesis_voice.py
--rw-r--r--   0 leeyang    (501) staff       (20)     1678 2023-02-12 04:54:23.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/ext/webrtc.py
--rw-r--r--   0 leeyang    (501) staff       (20)      471 2022-11-11 04:36:45.000000 fp_browser_sdk-0.9.1/fp_browser_sdk/fp_browser_settings.py
-drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-09 07:30:21.000000 fp_browser_sdk-0.9.1/fp_browser_sdk.egg-info/
--rw-r--r--   0 leeyang    (501) staff       (20)      264 2023-05-09 07:30:21.000000 fp_browser_sdk-0.9.1/fp_browser_sdk.egg-info/PKG-INFO
--rw-r--r--   0 leeyang    (501) staff       (20)     1473 2023-05-09 07:30:21.000000 fp_browser_sdk-0.9.1/fp_browser_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 leeyang    (501) staff       (20)        1 2023-05-09 07:30:21.000000 fp_browser_sdk-0.9.1/fp_browser_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 leeyang    (501) staff       (20)       15 2023-05-09 07:30:21.000000 fp_browser_sdk-0.9.1/fp_browser_sdk.egg-info/top_level.txt
--rw-r--r--   0 leeyang    (501) staff       (20)       38 2023-05-09 07:30:21.000000 fp_browser_sdk-0.9.1/setup.cfg
--rw-r--r--   0 leeyang    (501) staff       (20)      387 2023-05-09 07:30:11.000000 fp_browser_sdk-0.9.1/setup.py
+drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-14 03:38:48.000000 fp_browser_sdk-0.9.2/
+-rw-r--r--   0 leeyang    (501) staff       (20)      264 2023-05-14 03:38:48.000000 fp_browser_sdk-0.9.2/PKG-INFO
+-rw-r--r--   0 leeyang    (501) staff       (20)     8453 2023-02-12 04:55:25.000000 fp_browser_sdk-0.9.2/README.md
+drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-14 03:38:48.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/
+-rw-r--r--   0 leeyang    (501) staff       (20)    15571 2022-12-15 04:40:42.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/__init__.py
+drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-14 03:38:48.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/data/
+-rw-r--r--   0 leeyang    (501) staff       (20)        0 2022-08-05 08:21:32.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/data/__init__.py
+-rw-r--r--   0 leeyang    (501) staff       (20)   183083 2022-08-16 02:45:13.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/data/motion.py
+drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-14 03:38:48.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/
+-rw-r--r--   0 leeyang    (501) staff       (20)        0 2022-08-05 08:21:32.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/__init__.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     6741 2023-05-14 02:37:31.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/basic.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     1341 2023-05-14 03:34:14.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/basic_match.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     3212 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/battery.py
+-rw-r--r--   0 leeyang    (501) staff       (20)    17258 2023-04-07 07:59:18.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/browser_enum.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     3357 2023-03-13 13:15:24.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/client_hints.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     5336 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/device_motion.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     2059 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/device_orientation.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     7142 2023-01-15 06:50:48.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/document.py
+-rw-r--r--   0 leeyang    (501) staff       (20)      451 2022-08-07 03:58:52.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/exception.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     3291 2023-04-10 11:49:02.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/fingerprint_offset.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     1851 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/geo.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     1328 2023-05-09 07:29:43.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/gl.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     3266 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/header.py
+-rw-r--r--   0 leeyang    (501) staff       (20)      465 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/inject_js.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     2223 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/media.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     2539 2022-08-05 07:15:01.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/module.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     6966 2023-05-08 07:08:22.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/navigator.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     3917 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/network.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     9140 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/performance.py
+drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-14 03:38:48.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/permission_types/
+-rw-r--r--   0 leeyang    (501) staff       (20)      294 2022-09-18 13:15:09.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/permission_types/__init__.py
+-rw-r--r--   0 leeyang    (501) staff       (20)    13786 2022-12-17 12:48:42.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/permission_types/permission_type.py
+-rw-r--r--   0 leeyang    (501) staff       (20)    12917 2022-09-18 13:09:11.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/permission_types/permission_type_102.py
+-rw-r--r--   0 leeyang    (501) staff       (20)    12683 2022-12-17 12:48:42.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/permission_types/permission_type_107.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     9857 2022-09-18 13:09:11.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/permission_types/permission_type_88.py
+-rw-r--r--   0 leeyang    (501) staff       (20)    10280 2022-09-18 13:09:11.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/permission_types/permission_type_90.py
+-rw-r--r--   0 leeyang    (501) staff       (20)    11710 2022-09-18 13:09:11.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/permission_types/permission_type_93.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     1049 2022-12-17 12:48:42.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/permission_types/util.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     2087 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/plugin.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     3923 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/screen.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     2343 2022-11-10 12:59:52.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/speech_synthesis_voice.py
+-rw-r--r--   0 leeyang    (501) staff       (20)     1678 2023-02-12 04:54:23.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/ext/webrtc.py
+-rw-r--r--   0 leeyang    (501) staff       (20)      471 2022-11-11 04:36:45.000000 fp_browser_sdk-0.9.2/fp_browser_sdk/fp_browser_settings.py
+drwxr-xr-x   0 leeyang    (501) staff       (20)        0 2023-05-14 03:38:48.000000 fp_browser_sdk-0.9.2/fp_browser_sdk.egg-info/
+-rw-r--r--   0 leeyang    (501) staff       (20)      264 2023-05-14 03:38:47.000000 fp_browser_sdk-0.9.2/fp_browser_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 leeyang    (501) staff       (20)     1507 2023-05-14 03:38:48.000000 fp_browser_sdk-0.9.2/fp_browser_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 leeyang    (501) staff       (20)        1 2023-05-14 03:38:47.000000 fp_browser_sdk-0.9.2/fp_browser_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 leeyang    (501) staff       (20)       15 2023-05-14 03:38:47.000000 fp_browser_sdk-0.9.2/fp_browser_sdk.egg-info/top_level.txt
+-rw-r--r--   0 leeyang    (501) staff       (20)       38 2023-05-14 03:38:48.000000 fp_browser_sdk-0.9.2/setup.cfg
+-rw-r--r--   0 leeyang    (501) staff       (20)      387 2023-05-14 03:38:47.000000 fp_browser_sdk-0.9.2/setup.py
```

### Comparing `fp_browser_sdk-0.9.1/README.md` & `fp_browser_sdk-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk/__init__.py` & `fp_browser_sdk-0.9.2/fp_browser_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk/data/motion.py` & `fp_browser_sdk-0.9.2/fp_browser_sdk/data/motion.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/basic.py` & `fp_browser_sdk-0.9.2/fp_browser_sdk/ext/basic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List
 import time
 from .module import Module
 from .browser_enum import TLSVersion
 from .inject_js import InjectJS
 from .media import Media
+from .basic_match import BasicMatch
 
 
 class Basic(Module):
     def __init__(self):
         super(Basic, self).__init__()
         self._global_disable_settings = False
         self._disable_window_status = False
@@ -27,14 +28,15 @@
         self._memory_info_total_js = None
         self._memory_info_used_js = None
         self._memory_info_limit_js = None
         self._disable_alert = False
         self._disable_window_open = False
         self._confirm = None
         self._media_list = []
+        self._match_json = []
         pass
 
     def _to_dict(self):
         """
         解析成 dict
         """
         result = {
@@ -60,14 +62,17 @@
             "memoryinfo.limit-js": self._memory_info_limit_js,
             "frame.disable-alert": self._bool_to_int(self._disable_alert),
             "frame.disable-window-open": self._bool_to_int(self._disable_window_open),
             "frame.confirm": self._bool_to_int(self._confirm),
             "media.list-json": [item.to_dict() for item in self._media_list],
         }
 
+        if len(self._match_json) > 0:
+            result['basic.match-json'] = [item.to_dict() for item in self._match_json]
+
         return result
 
     def set_disable_window(self, value: bool):
         """
         是否禁用 window 的 chrome 属性
         """
         self._disable_window_status = value
@@ -215,7 +220,14 @@
 
     def append_media(self, value: Media):
         """
         硬件设备信息
         """
         self._media_list.append(value)
         return self
+
+    def append_match_list(self, value: BasicMatch):
+        """
+        添加匹配对象
+        """
+        self._match_json.append(value)
+        return self
```

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/battery.py` & `fp_browser_sdk-0.9.2/fp_browser_sdk/ext/battery.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/browser_enum.py` & `fp_browser_sdk-0.9.2/fp_browser_sdk/ext/browser_enum.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/client_hints.py` & `fp_browser_sdk-0.9.2/fp_browser_sdk/ext/client_hints.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/device_motion.py` & `fp_browser_sdk-0.9.2/fp_browser_sdk/ext/device_motion.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/device_orientation.py` & `fp_browser_sdk-0.9.2/fp_browser_sdk/ext/device_orientation.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/document.py` & `fp_browser_sdk-0.9.2/fp_browser_sdk/ext/document.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/fingerprint_offset.py` & `fp_browser_sdk-0.9.2/fp_browser_sdk/ext/fingerprint_offset.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/geo.py` & `fp_browser_sdk-0.9.2/fp_browser_sdk/ext/geo.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/gl.py` & `fp_browser_sdk-0.9.2/fp_browser_sdk/ext/gl.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/header.py` & `fp_browser_sdk-0.9.2/fp_browser_sdk/ext/header.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/media.py` & `fp_browser_sdk-0.9.2/fp_browser_sdk/ext/media.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/module.py` & `fp_browser_sdk-0.9.2/fp_browser_sdk/ext/module.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/navigator.py` & `fp_browser_sdk-0.9.2/fp_browser_sdk/ext/navigator.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/network.py` & `fp_browser_sdk-0.9.2/fp_browser_sdk/ext/network.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/performance.py` & `fp_browser_sdk-0.9.2/fp_browser_sdk/ext/performance.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/permission_type.py` & `fp_browser_sdk-0.9.2/fp_browser_sdk/ext/permission_types/permission_type.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/permission_type_102.py` & `fp_browser_sdk-0.9.2/fp_browser_sdk/ext/permission_types/permission_type_102.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/permission_type_107.py` & `fp_browser_sdk-0.9.2/fp_browser_sdk/ext/permission_types/permission_type_107.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/permission_type_88.py` & `fp_browser_sdk-0.9.2/fp_browser_sdk/ext/permission_types/permission_type_88.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/permission_type_90.py` & `fp_browser_sdk-0.9.2/fp_browser_sdk/ext/permission_types/permission_type_90.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/permission_type_93.py` & `fp_browser_sdk-0.9.2/fp_browser_sdk/ext/permission_types/permission_type_93.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/permission_types/util.py` & `fp_browser_sdk-0.9.2/fp_browser_sdk/ext/permission_types/util.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/plugin.py` & `fp_browser_sdk-0.9.2/fp_browser_sdk/ext/plugin.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/screen.py` & `fp_browser_sdk-0.9.2/fp_browser_sdk/ext/screen.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/speech_synthesis_voice.py` & `fp_browser_sdk-0.9.2/fp_browser_sdk/ext/speech_synthesis_voice.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk/ext/webrtc.py` & `fp_browser_sdk-0.9.2/fp_browser_sdk/ext/webrtc.py`

 * *Files identical despite different names*

### Comparing `fp_browser_sdk-0.9.1/fp_browser_sdk.egg-info/SOURCES.txt` & `fp_browser_sdk-0.9.2/fp_browser_sdk.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 fp_browser_sdk.egg-info/SOURCES.txt
 fp_browser_sdk.egg-info/dependency_links.txt
 fp_browser_sdk.egg-info/top_level.txt
 fp_browser_sdk/data/__init__.py
 fp_browser_sdk/data/motion.py
 fp_browser_sdk/ext/__init__.py
 fp_browser_sdk/ext/basic.py
+fp_browser_sdk/ext/basic_match.py
 fp_browser_sdk/ext/battery.py
 fp_browser_sdk/ext/browser_enum.py
 fp_browser_sdk/ext/client_hints.py
 fp_browser_sdk/ext/device_motion.py
 fp_browser_sdk/ext/device_orientation.py
 fp_browser_sdk/ext/document.py
 fp_browser_sdk/ext/exception.py
```

