# Comparing `tmp/realtouch-0.1.2.tar.gz` & `tmp/realtouch-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "realtouch-0.1.2.tar", last modified: Sat May 13 02:52:01 2023, max compression
+gzip compressed data, was "realtouch-0.1.3.tar", last modified: Sun May 14 09:14:50 2023, max compression
```

## Comparing `realtouch-0.1.2.tar` & `realtouch-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 k          (501) staff       (20)        0 2023-05-13 02:52:01.077028 realtouch-0.1.2/
--rw-r--r--   0 k          (501) staff       (20)    35148 2023-05-12 00:09:36.000000 realtouch-0.1.2/LICENSE
--rw-r--r--   0 k          (501) staff       (20)      539 2023-05-13 02:52:01.076574 realtouch-0.1.2/PKG-INFO
-drwxr-xr-x   0 k          (501) staff       (20)        0 2023-05-13 02:52:01.069774 realtouch-0.1.2/realtouch/
-drwxr-xr-x   0 k          (501) staff       (20)        0 2023-05-13 02:52:01.072533 realtouch-0.1.2/realtouch/src/
-drwxr-xr-x   0 k          (501) staff       (20)        0 2023-05-13 02:52:01.075765 realtouch-0.1.2/realtouch/src/realtouch.egg-info/
--rw-r--r--   0 k          (501) staff       (20)      539 2023-05-13 02:52:00.000000 realtouch-0.1.2/realtouch/src/realtouch.egg-info/PKG-INFO
--rw-r--r--   0 k          (501) staff       (20)      277 2023-05-13 02:52:01.000000 realtouch-0.1.2/realtouch/src/realtouch.egg-info/SOURCES.txt
--rw-r--r--   0 k          (501) staff       (20)        1 2023-05-13 02:52:00.000000 realtouch-0.1.2/realtouch/src/realtouch.egg-info/dependency_links.txt
--rw-r--r--   0 k          (501) staff       (20)       16 2023-05-13 02:52:00.000000 realtouch-0.1.2/realtouch/src/realtouch.egg-info/requires.txt
--rw-r--r--   0 k          (501) staff       (20)       10 2023-05-13 02:52:00.000000 realtouch-0.1.2/realtouch/src/realtouch.egg-info/top_level.txt
--rw-r--r--   0 k          (501) staff       (20)    18488 2023-05-13 01:54:08.000000 realtouch-0.1.2/realtouch/src/realtouch.py
--rw-r--r--   0 k          (501) staff       (20)       38 2023-05-13 02:52:01.077193 realtouch-0.1.2/setup.cfg
--rw-r--r--   0 k          (501) staff       (20)      852 2023-05-13 02:51:32.000000 realtouch-0.1.2/setup.py
+drwxr-xr-x   0 k          (501) staff       (20)        0 2023-05-14 09:14:50.849645 realtouch-0.1.3/
+-rw-r--r--   0 k          (501) staff       (20)    35148 2023-05-12 00:09:36.000000 realtouch-0.1.3/LICENSE
+-rw-r--r--   0 k          (501) staff       (20)      539 2023-05-14 09:14:50.849402 realtouch-0.1.3/PKG-INFO
+drwxr-xr-x   0 k          (501) staff       (20)        0 2023-05-14 09:14:50.845266 realtouch-0.1.3/realtouch/
+drwxr-xr-x   0 k          (501) staff       (20)        0 2023-05-14 09:14:50.847258 realtouch-0.1.3/realtouch/src/
+drwxr-xr-x   0 k          (501) staff       (20)        0 2023-05-14 09:14:50.848975 realtouch-0.1.3/realtouch/src/realtouch.egg-info/
+-rw-r--r--   0 k          (501) staff       (20)      539 2023-05-14 09:14:50.000000 realtouch-0.1.3/realtouch/src/realtouch.egg-info/PKG-INFO
+-rw-r--r--   0 k          (501) staff       (20)      277 2023-05-14 09:14:50.000000 realtouch-0.1.3/realtouch/src/realtouch.egg-info/SOURCES.txt
+-rw-r--r--   0 k          (501) staff       (20)        1 2023-05-14 09:14:50.000000 realtouch-0.1.3/realtouch/src/realtouch.egg-info/dependency_links.txt
+-rw-r--r--   0 k          (501) staff       (20)       16 2023-05-14 09:14:50.000000 realtouch-0.1.3/realtouch/src/realtouch.egg-info/requires.txt
+-rw-r--r--   0 k          (501) staff       (20)       10 2023-05-14 09:14:50.000000 realtouch-0.1.3/realtouch/src/realtouch.egg-info/top_level.txt
+-rw-r--r--   0 k          (501) staff       (20)    18556 2023-05-14 09:14:04.000000 realtouch-0.1.3/realtouch/src/realtouch.py
+-rw-r--r--   0 k          (501) staff       (20)       38 2023-05-14 09:14:50.849728 realtouch-0.1.3/setup.cfg
+-rw-r--r--   0 k          (501) staff       (20)      852 2023-05-14 09:14:31.000000 realtouch-0.1.3/setup.py
```

### Comparing `realtouch-0.1.2/LICENSE` & `realtouch-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `realtouch-0.1.2/PKG-INFO` & `realtouch-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: realtouch
-Version: 0.1.2
+Version: 0.1.3
 Summary: realTouch Robot SDK
 Home-page: https://realtouch.dev
 Author: realTouch Dev
 Author-email: contact@realtouch.dev
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `realtouch-0.1.2/realtouch/src/realtouch.egg-info/PKG-INFO` & `realtouch-0.1.3/realtouch/src/realtouch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: realtouch
-Version: 0.1.2
+Version: 0.1.3
 Summary: realTouch Robot SDK
 Home-page: https://realtouch.dev
 Author: realTouch Dev
 Author-email: contact@realtouch.dev
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `realtouch-0.1.2/realtouch/src/realtouch.py` & `realtouch-0.1.3/realtouch/src/realtouch.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     def phone(self, position: int) -> 'Phone':
         return self._phones.get(position)
 
     @property
     def phones(self) -> dict[int, 'Phone']:
         return self._phones
 
-    def call_func(self, position, path, **kwargs):
+    def call_func(self, position, path, **kwargs) -> Union[dict, bytes, str]:
         phone = self.phone(position)
         if phone:
             headers = {
                 'PhonePosition': str(phone.position)
             }
         else:
             headers = {}
@@ -217,22 +217,25 @@
         """
         读取最近短信. MIUI可以读取验证码短信 但是需要给agent授权
         :return:
         """
         key = 'screen/read_sms'
         return self.phone.robot.call_func(self.phone.position, key)
 
-    def phone_info(self, update=False):
+    def phone_info(self):
         """
         手机信息
-        :param update:
         :return:
         """
-        key = 'screen/phone_info'
-        return self.phone.robot.call_func(self.phone.position, key, update=update)
+        key = 'self/to-json'
+        return self.phone.robot.call_func(self.phone.position, key)
+
+    def copy_clipboard(self):
+        info = self.phone_info()
+        return info['clipboard']
 
     def get_phone_text(self, local_only=False):
         """
         获取手机屏幕上的文字
         格式: [[[start_x, start_y, end_x, end_y], 文字, 可信度]]
         :param local_only: 是否使用缓存
         :return:
@@ -534,15 +537,15 @@
         """
         return self.robot.call_func(self.position, 'self/take_picture')
 
     @staticmethod
     def location_serialize(location: Union[
         ImgLocation, list[ImgLocation],
         ImgArea, list[ImgArea]] = ImgLocation.FULL):
-        if not isinstance(location, list) or not isinstance(location, tuple):
+        if not isinstance(location, list) and not isinstance(location, tuple):
             location = [location]
         result = []
         for loc in location:
             if isinstance(loc, ImgLocation):
                 result.append(loc.name)
             else:
                 result.append(asdict(location))
```

### Comparing `realtouch-0.1.2/setup.py` & `realtouch-0.1.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="realtouch",
-    version="0.1.2",
+    version="0.1.3",
     author="realTouch Dev",
     author_email="contact@realtouch.dev",
     description="realTouch Robot SDK",
     long_description="realTouch Robot SDK",
     long_description_content_type="text/markdown",
     url="https://realtouch.dev",
     packages=find_packages(),
```

