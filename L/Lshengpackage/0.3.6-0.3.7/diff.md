# Comparing `tmp/Lshengpackage-0.3.6.tar.gz` & `tmp/Lshengpackage-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lshengpackage-0.3.6.tar", last modified: Sun May 14 04:54:19 2023, max compression
+gzip compressed data, was "Lshengpackage-0.3.7.tar", last modified: Sun May 14 07:51:12 2023, max compression
```

## Comparing `Lshengpackage-0.3.6.tar` & `Lshengpackage-0.3.7.tar`

### file list

```diff
@@ -1,46 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 04:54:19.732801 Lshengpackage-0.3.6/
--rw-rw-rw-   0        0        0     1079 2022-05-04 09:06:22.000000 Lshengpackage-0.3.6/LICENSE
--rw-rw-rw-   0        0        0     1077 2022-05-04 09:06:22.000000 Lshengpackage-0.3.6/License.md
-drwxrwxrwx   0        0        0        0 2023-05-14 04:54:19.674792 Lshengpackage-0.3.6/Lshengpackage/
--rw-rw-rw-   0        0        0       49 2023-05-14 01:06:32.000000 Lshengpackage-0.3.6/Lshengpackage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:54:19.703793 Lshengpackage-0.3.6/Lshengpackage/simulate/
--rw-rw-rw-   0        0        0       51 2022-10-10 06:17:48.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:54:19.704795 Lshengpackage-0.3.6/Lshengpackage/simulate/__pycache__/
--rw-rw-rw-   0        0        0      158 2022-10-10 08:40:15.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-05-14 04:54:19.707795 Lshengpackage-0.3.6/Lshengpackage/simulate/adb/
--rw-rw-rw-   0        0        0     2419 2023-05-14 04:20:16.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/adb/Command_adb.py
--rw-rw-rw-   0        0        0       51 2022-10-10 06:18:05.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/adb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:54:19.711792 Lshengpackage-0.3.6/Lshengpackage/simulate/adb/__pycache__/
--rw-rw-rw-   0        0        0     1852 2022-10-10 06:12:01.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/adb/__pycache__/Command_adb.cpython-39.pyc
--rw-rw-rw-   0        0        0      162 2022-10-10 08:45:14.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/adb/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-05-14 04:54:19.716793 Lshengpackage-0.3.6/Lshengpackage/simulate/dm/
--rw-rw-rw-   0        0        0     4677 2022-05-04 09:06:22.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/dm/Pac_dm.py
--rw-rw-rw-   0        0        0      314 2023-05-14 01:06:32.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/dm/Reg.py
--rw-rw-rw-   0        0        0     9334 2022-05-04 09:06:22.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/dm/Win_dm.py
--rw-rw-rw-   0        0        0       49 2022-10-10 06:18:05.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/dm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:54:19.724793 Lshengpackage-0.3.6/Lshengpackage/simulate/dm/__pycache__/
--rw-rw-rw-   0        0        0     4816 2022-10-10 08:45:14.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc
--rw-rw-rw-   0        0        0      565 2022-10-10 08:45:14.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc
--rw-rw-rw-   0        0        0     1262 2022-10-10 08:45:14.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc
--rw-rw-rw-   0        0        0      161 2022-10-10 08:45:14.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/dm/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      286 2022-06-29 01:11:38.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/mock_findFr.py
--rw-rw-rw-   0        0        0     2364 2023-05-14 04:20:16.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/mock_findPic.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:54:19.731792 Lshengpackage-0.3.6/Lshengpackage/tools/
--rw-rw-rw-   0        0        0     1988 2022-05-26 11:29:53.000000 Lshengpackage-0.3.6/Lshengpackage/tools/ChaoJiYing.py
--rw-rw-rw-   0        0        0      759 2023-05-14 04:52:50.000000 Lshengpackage-0.3.6/Lshengpackage/tools/General.py
--rw-rw-rw-   0        0        0      900 2023-05-14 04:31:40.000000 Lshengpackage-0.3.6/Lshengpackage/tools/Loading.py
--rw-rw-rw-   0        0        0     3305 2023-05-14 01:56:09.000000 Lshengpackage-0.3.6/Lshengpackage/tools/OperateFile.py
--rw-rw-rw-   0        0        0     2059 2023-05-14 04:52:50.000000 Lshengpackage-0.3.6/Lshengpackage/tools/SearchFile.py
--rw-rw-rw-   0        0        0       51 2022-10-10 06:17:48.000000 Lshengpackage-0.3.6/Lshengpackage/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:54:19.699828 Lshengpackage-0.3.6/Lshengpackage.egg-info/
--rw-rw-rw-   0        0        0      858 2023-05-14 04:54:19.000000 Lshengpackage-0.3.6/Lshengpackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1246 2023-05-14 04:54:19.000000 Lshengpackage-0.3.6/Lshengpackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 04:54:19.000000 Lshengpackage-0.3.6/Lshengpackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      147 2023-05-14 04:54:19.000000 Lshengpackage-0.3.6/Lshengpackage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-14 04:54:19.000000 Lshengpackage-0.3.6/Lshengpackage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      242 2023-05-14 03:32:07.000000 Lshengpackage-0.3.6/MANIFEST.in
--rw-rw-rw-   0        0        0      858 2023-05-14 04:54:19.732801 Lshengpackage-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     3950 2023-05-14 04:53:00.000000 Lshengpackage-0.3.6/README.md
--rw-rw-rw-   0        0        0      350 2023-05-14 03:44:13.000000 Lshengpackage-0.3.6/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-05-14 04:54:19.738798 Lshengpackage-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0     2056 2023-05-14 03:44:13.000000 Lshengpackage-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 07:51:12.113356 Lshengpackage-0.3.7/
+-rw-rw-rw-   0        0        0     1079 2022-05-04 09:06:22.000000 Lshengpackage-0.3.7/LICENSE
+-rw-rw-rw-   0        0        0     1077 2022-05-04 09:06:22.000000 Lshengpackage-0.3.7/License.md
+drwxrwxrwx   0        0        0        0 2023-05-14 07:51:12.051769 Lshengpackage-0.3.7/Lshengpackage/
+-rw-rw-rw-   0        0        0       49 2023-05-14 01:06:32.000000 Lshengpackage-0.3.7/Lshengpackage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 07:51:12.071298 Lshengpackage-0.3.7/Lshengpackage/simulate/
+-rw-rw-rw-   0        0        0       51 2022-10-10 06:17:48.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 07:51:12.073305 Lshengpackage-0.3.7/Lshengpackage/simulate/__pycache__/
+-rw-rw-rw-   0        0        0      158 2022-10-10 08:40:15.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-05-14 07:51:12.076298 Lshengpackage-0.3.7/Lshengpackage/simulate/adb/
+-rw-rw-rw-   0        0        0     2689 2023-05-14 07:49:17.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/adb/Command_adb.py
+-rw-rw-rw-   0        0        0       51 2022-10-10 06:18:05.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/adb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 07:51:12.078299 Lshengpackage-0.3.7/Lshengpackage/simulate/adb/__pycache__/
+-rw-rw-rw-   0        0        0      162 2022-10-10 08:45:14.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/adb/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-05-14 07:51:12.089827 Lshengpackage-0.3.7/Lshengpackage/simulate/dm/
+-rw-rw-rw-   0        0        0     4677 2022-05-04 09:06:22.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/dm/Pac_dm.py
+-rw-rw-rw-   0        0        0      314 2023-05-14 01:06:32.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/dm/Reg.py
+-rw-rw-rw-   0        0        0     9334 2022-05-04 09:06:22.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/dm/Win_dm.py
+-rw-rw-rw-   0        0        0       49 2022-10-10 06:18:05.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/dm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 07:51:12.099347 Lshengpackage-0.3.7/Lshengpackage/simulate/dm/__pycache__/
+-rw-rw-rw-   0        0        0     4816 2022-10-10 08:45:14.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc
+-rw-rw-rw-   0        0        0      565 2022-10-10 08:45:14.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1262 2022-10-10 08:45:14.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc
+-rw-rw-rw-   0        0        0      161 2022-10-10 08:45:14.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/dm/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      286 2022-06-29 01:11:38.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/mock_findFr.py
+-rw-rw-rw-   0        0        0     2364 2023-05-14 04:20:16.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/mock_findPic.py
+drwxrwxrwx   0        0        0        0 2023-05-14 07:51:12.112354 Lshengpackage-0.3.7/Lshengpackage/tools/
+-rw-rw-rw-   0        0        0     1988 2022-05-26 11:29:53.000000 Lshengpackage-0.3.7/Lshengpackage/tools/ChaoJiYing.py
+-rw-rw-rw-   0        0        0      759 2023-05-14 04:52:50.000000 Lshengpackage-0.3.7/Lshengpackage/tools/General.py
+-rw-rw-rw-   0        0        0      900 2023-05-14 04:31:40.000000 Lshengpackage-0.3.7/Lshengpackage/tools/Loading.py
+-rw-rw-rw-   0        0        0     3305 2023-05-14 01:56:09.000000 Lshengpackage-0.3.7/Lshengpackage/tools/OperateFile.py
+-rw-rw-rw-   0        0        0     2059 2023-05-14 04:52:50.000000 Lshengpackage-0.3.7/Lshengpackage/tools/SearchFile.py
+-rw-rw-rw-   0        0        0       51 2022-10-10 06:17:48.000000 Lshengpackage-0.3.7/Lshengpackage/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 07:51:12.064278 Lshengpackage-0.3.7/Lshengpackage.egg-info/
+-rw-rw-rw-   0        0        0      858 2023-05-14 07:51:11.000000 Lshengpackage-0.3.7/Lshengpackage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1180 2023-05-14 07:51:11.000000 Lshengpackage-0.3.7/Lshengpackage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 07:51:11.000000 Lshengpackage-0.3.7/Lshengpackage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      147 2023-05-14 07:51:11.000000 Lshengpackage-0.3.7/Lshengpackage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-14 07:51:11.000000 Lshengpackage-0.3.7/Lshengpackage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      242 2023-05-14 03:32:07.000000 Lshengpackage-0.3.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      858 2023-05-14 07:51:12.114355 Lshengpackage-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3975 2023-05-14 07:50:08.000000 Lshengpackage-0.3.7/README.md
+-rw-rw-rw-   0        0        0      350 2023-05-14 03:44:13.000000 Lshengpackage-0.3.7/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-05-14 07:51:12.116451 Lshengpackage-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     2056 2023-05-14 07:49:26.000000 Lshengpackage-0.3.7/setup.py
```

### Comparing `Lshengpackage-0.3.6/LICENSE` & `Lshengpackage-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.6/License.md` & `Lshengpackage-0.3.7/License.md`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.6/Lshengpackage/simulate/adb/Command_adb.py` & `Lshengpackage-0.3.7/Lshengpackage/simulate/adb/Command_adb.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,79 +1,93 @@
-# -*coding:utf-8 -*-
-# !/usr/bin/env python
-
-from PIL import ImageFile
-from PIL import Image
-import os
-
-
-class command:
-    def dev(self):
-        # 查看当前链接设备
-        os.system('adb devices')
-
-    def log(self):
-        # 查看日志
-        os.system('adb logcat')
-
-    def kill(self):
-        # 结束adb服务
-        os.system('adb kill-server')
-
-    def star(self):
-        # 开始adb服务
-        os.system('adb start-server')
-
-    def install(self, apk_name):
-        # 安装软件
-        os.system('adb install -r {}.apk'.format(apk_name))
-
-    def uninstall(self, apk_name):
-        # 卸载
-        os.system('adb uninstall {}.apk'.format(apk_name))
-
-    def up(self, file_name, path_phone):
-        # 上传SDCard/../..手机端路径
-        os.system('adb push {} {}'.format(file_name, path_phone))
-
-    def down(self, file_name):
-        # 下载
-        os.system('adb uninstall {}'.format(file_name))
-
-    def scr(self, path_pic_name):
-        # 屏幕截图到手机根目录
-        os.system('adb shell screencap -p /sdcard/{}.png'.format(path_pic_name))
-
-    def video_scr(self, video_name):
-        # 录屏，默认mp4格式
-        os.system('adb shell screenrecord /sdcard/{}.mp4'.format(video_name))
-
-    def cut_scr(self, path_pic_name, path):
-        # 屏幕截图到本地
-        # pic_name:屏幕截图生成地址+名称，默认为手机的根目录,默认的来
-        # path为文件夹目录下
-        self.scr(path_pic_name)
-        os.system("adb pull /sdcard/{} {}{}.png".format(path_pic_name, path, path_pic_name))
-        ImageFile.LOAD_TRUNCATED_IMAGES = True
-
-    def spec_scr(self, pic_name, path, int_x1, int_y1, int_x2, int_y2):
-        """
-        指定截图保存
-        左上角的点到右下角的点
-        """
-        self.cut_scr(pic_name, path)
-        img = Image.open(path + pic_name)
-        # (4)将图片验证码截取
-        code_image = img.crop((int_x1, int_y1, int_x2, int_y2))
-        code_image.save(path + pic_name)  # 原地址重写
-
-    def tap_work(self, x, y):
-        """
-        模拟点击操作
-        """
-        os.system('adb shell input tap {} {}'.format(x, y))
-
-    def swip_work(self, x, y, x2, y2):
-        """
-        模拟滑动操作
-        """
-        os.system('adb shell input swipe {} {} {} {}'.format(x, y, x2, y2))
+# -*coding:utf-8 -*-
+# !/usr/bin/env python
+
+from PIL import ImageFile
+from PIL import Image
+import os
+
+
+class command:
+    def dev(self):
+        # 查看当前链接设备
+        com = os.system('adb devices')
+        return com
+
+    def log(self):
+        # 查看日志
+        com = os.system('adb logcat')
+        return com
+    
+    def kill(self):
+        # 结束adb服务
+        com = os.system('adb kill-server')
+        return com
+
+    def star(self):
+        # 开始adb服务
+        com = os.system('adb start-server')
+        return com
+
+    def install(self, apk_name):
+        # 安装软件
+        com = os.system('adb install -r {}.apk'.format(apk_name))
+        return com
+
+    def uninstall(self, apk_name):
+        # 卸载
+        com = os.system('adb uninstall {}.apk'.format(apk_name))
+        return com
+
+    def up(self, file_name, path_phone):
+        # 上传SDCard/../..手机端路径
+        com = os.system('adb push {} {}'.format(file_name, path_phone))
+        return com
+
+    def down(self, file_name):
+        # 下载
+        com = os.system('adb uninstall {}'.format(file_name))
+        return com
+
+    def scr(self, path_pic_name):
+        # 屏幕截图到手机根目录
+        com = os.system('adb shell screencap -p /sdcard/{}.png'.format(path_pic_name))
+        return com
+
+    def video_scr(self, video_name):
+        # 录屏，默认mp4格式
+        com = os.system('adb shell screenrecord /sdcard/{}.mp4'.format(video_name))
+        return com
+
+    def cut_scr(self, path_pic_name, path):
+        # 屏幕截图到本地
+        # pic_name:屏幕截图生成地址+名称，默认为手机的根目录,默认的来
+        # path为文件夹目录下
+        self.scr(path_pic_name)
+        com = os.system("adb pull /sdcard/{} {}{}.png".format(path_pic_name, path, path_pic_name))
+        ImageFile.LOAD_TRUNCATED_IMAGES = True
+        return com
+
+    def spec_scr(self, pic_name, path, int_x1, int_y1, int_x2, int_y2):
+        """
+        指定截图保存
+        左上角的点到右下角的点
+        """
+        self.cut_scr(pic_name, path)
+        img = Image.open(path + pic_name)
+        # (4)将图片验证码截取
+        code_image = img.crop((int_x1, int_y1, int_x2, int_y2))
+        code_image.save(path + pic_name)  # 原地址重写
+        return True
+
+    def tap_work(self, x, y):
+        """
+        模拟点击操作
+        """
+        com = os.system('adb shell input tap {} {}'.format(x, y))
+        return com
+
+    def swip_work(self, x, y, x2, y2):
+        """
+        模拟滑动操作
+        """
+        com = os.system('adb shell input swipe {} {} {} {}'.format(x, y, x2, y2))
+        return com
```

### Comparing `Lshengpackage-0.3.6/Lshengpackage/simulate/dm/Pac_dm.py` & `Lshengpackage-0.3.7/Lshengpackage/simulate/dm/Pac_dm.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.6/Lshengpackage/simulate/dm/Win_dm.py` & `Lshengpackage-0.3.7/Lshengpackage/simulate/dm/Win_dm.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.6/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc` & `Lshengpackage-0.3.7/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.6/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc` & `Lshengpackage-0.3.7/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.6/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc` & `Lshengpackage-0.3.7/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.6/Lshengpackage/simulate/mock_findPic.py` & `Lshengpackage-0.3.7/Lshengpackage/simulate/mock_findPic.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.6/Lshengpackage/tools/ChaoJiYing.py` & `Lshengpackage-0.3.7/Lshengpackage/tools/ChaoJiYing.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.6/Lshengpackage/tools/General.py` & `Lshengpackage-0.3.7/Lshengpackage/tools/General.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.6/Lshengpackage/tools/Loading.py` & `Lshengpackage-0.3.7/Lshengpackage/tools/Loading.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.6/Lshengpackage/tools/OperateFile.py` & `Lshengpackage-0.3.7/Lshengpackage/tools/OperateFile.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.6/Lshengpackage/tools/SearchFile.py` & `Lshengpackage-0.3.7/Lshengpackage/tools/SearchFile.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.6/Lshengpackage.egg-info/PKG-INFO` & `Lshengpackage-0.3.7/Lshengpackage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lshengpackage
-Version: 0.3.6
+Version: 0.3.7
 Summary: 个人自动化爬虫开源学习
 Home-page: https://lsheng0-0.github.io/
 Download-URL: https://github.com/Lsheng0-0/package
 Author: Lsheng0-0
 Author-email: 1522833718@qq.com
 License: MIT
 Keywords: 游戏,办公,自动化,爬虫
```

### Comparing `Lshengpackage-0.3.6/Lshengpackage.egg-info/SOURCES.txt` & `Lshengpackage-0.3.7/Lshengpackage.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 Lshengpackage.egg-info/top_level.txt
 Lshengpackage/simulate/__init__.py
 Lshengpackage/simulate/mock_findFr.py
 Lshengpackage/simulate/mock_findPic.py
 Lshengpackage/simulate/__pycache__/__init__.cpython-39.pyc
 Lshengpackage/simulate/adb/Command_adb.py
 Lshengpackage/simulate/adb/__init__.py
-Lshengpackage/simulate/adb/__pycache__/Command_adb.cpython-39.pyc
 Lshengpackage/simulate/adb/__pycache__/__init__.cpython-39.pyc
 Lshengpackage/simulate/dm/Pac_dm.py
 Lshengpackage/simulate/dm/Reg.py
 Lshengpackage/simulate/dm/Win_dm.py
 Lshengpackage/simulate/dm/__init__.py
 Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc
 Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc
```

### Comparing `Lshengpackage-0.3.6/PKG-INFO` & `Lshengpackage-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lshengpackage
-Version: 0.3.6
+Version: 0.3.7
 Summary: 个人自动化爬虫开源学习
 Home-page: https://lsheng0-0.github.io/
 Download-URL: https://github.com/Lsheng0-0/package
 Author: Lsheng0-0
 Author-email: 1522833718@qq.com
 License: MIT
 Keywords: 游戏,办公,自动化,爬虫
```

### Comparing `Lshengpackage-0.3.6/README.md` & `Lshengpackage-0.3.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ```cmd
 pip install Lshengpackage
 ```
 
 
 
 > ###关于Command_adb相关模块的调用介绍(更新)
->
+>返回值0,1,2 0为成功
 
 ```python
 # -*- coding: UTF-8 -*-
 from Lshengpackage.simulate.adb.Command_adb import command  # 调用模块
 
 com = command()  # 调用类
 com.star()  # 开始adb进程
```

### Comparing `Lshengpackage-0.3.6/setup.py` & `Lshengpackage-0.3.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='Lshengpackage',  # How you named your package folder (MyLib)
     packages=['Lshengpackage'],  # Chose the same as "name"
-    version='0.3.6',  # Start with a small number and increase it with every change you make
+    version='0.3.7',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='个人自动化爬虫开源学习',  # Give a short description about your library
     # long_description=open('README.md', 'r', encoding='utf-8').read(),
     author='Lsheng0-0',  # Type in your name
     author_email='1522833718@qq.com',  # Type in your E-Mail
     url='https://lsheng0-0.github.io/',  # Provide either the link to your github or to your website
     download_url='https://github.com/Lsheng0-0/package',  # I explain this later on
```

