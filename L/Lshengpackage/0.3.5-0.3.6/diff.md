# Comparing `tmp/Lshengpackage-0.3.5.tar.gz` & `tmp/Lshengpackage-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lshengpackage-0.3.5.tar", last modified: Wed Dec  7 09:41:56 2022, max compression
+gzip compressed data, was "Lshengpackage-0.3.6.tar", last modified: Sun May 14 04:54:19 2023, max compression
```

## Comparing `Lshengpackage-0.3.5.tar` & `Lshengpackage-0.3.6.tar`

### file list

```diff
@@ -1,56 +1,46 @@
-drwxrwxrwx   0        0        0        0 2022-12-07 09:41:56.273427 Lshengpackage-0.3.5/
--rw-rw-rw-   0        0        0     1079 2022-05-04 09:06:22.000000 Lshengpackage-0.3.5/LICENSE
--rw-rw-rw-   0        0        0     1077 2022-05-04 09:06:22.000000 Lshengpackage-0.3.5/License.md
-drwxrwxrwx   0        0        0        0 2022-12-07 09:41:56.219572 Lshengpackage-0.3.5/Lshengpackage/
--rw-rw-rw-   0        0        0     1988 2022-05-26 11:29:53.000000 Lshengpackage-0.3.5/Lshengpackage/Chaojiying.py
--rw-rw-rw-   0        0        0      429 2022-10-09 08:20:49.000000 Lshengpackage-0.3.5/Lshengpackage/Delay.py
--rw-rw-rw-   0        0        0      278 2022-10-20 09:11:16.000000 Lshengpackage-0.3.5/Lshengpackage/Entry.py
--rw-rw-rw-   0        0        0      809 2022-10-20 09:13:41.000000 Lshengpackage-0.3.5/Lshengpackage/Load.py
--rw-rw-rw-   0        0        0      605 2022-10-10 08:54:27.000000 Lshengpackage-0.3.5/Lshengpackage/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-07 09:41:56.234531 Lshengpackage-0.3.5/Lshengpackage/file/
--rw-rw-rw-   0        0        0     1105 2022-10-20 03:32:50.000000 Lshengpackage-0.3.5/Lshengpackage/file/Temp.py
--rw-rw-rw-   0        0        0       51 2022-10-10 06:17:48.000000 Lshengpackage-0.3.5/Lshengpackage/file/__init__.py
--rw-rw-rw-   0        0        0     2228 2022-12-07 09:33:53.000000 Lshengpackage-0.3.5/Lshengpackage/file/deal_file.py
--rw-rw-rw-   0        0        0     2058 2022-10-21 09:26:24.000000 Lshengpackage-0.3.5/Lshengpackage/file/search_file.py
-drwxrwxrwx   0        0        0        0 2022-12-07 09:41:56.236526 Lshengpackage-0.3.5/Lshengpackage/simulate/
--rw-rw-rw-   0        0        0       51 2022-10-10 06:17:48.000000 Lshengpackage-0.3.5/Lshengpackage/simulate/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-07 09:41:56.237523 Lshengpackage-0.3.5/Lshengpackage/simulate/__pycache__/
--rw-rw-rw-   0        0        0      158 2022-10-10 08:40:15.000000 Lshengpackage-0.3.5/Lshengpackage/simulate/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2022-12-07 09:41:56.242509 Lshengpackage-0.3.5/Lshengpackage/simulate/adb/
--rw-rw-rw-   0        0        0     1194 2022-05-04 09:06:22.000000 Lshengpackage-0.3.5/Lshengpackage/simulate/adb/Command_adb.py
--rw-rw-rw-   0        0        0     3572 2022-10-11 06:37:43.000000 Lshengpackage-0.3.5/Lshengpackage/simulate/adb/Pac_adb.py
--rw-rw-rw-   0        0        0       51 2022-10-10 06:18:05.000000 Lshengpackage-0.3.5/Lshengpackage/simulate/adb/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-07 09:41:56.247504 Lshengpackage-0.3.5/Lshengpackage/simulate/adb/__pycache__/
--rw-rw-rw-   0        0        0     1852 2022-10-10 06:12:01.000000 Lshengpackage-0.3.5/Lshengpackage/simulate/adb/__pycache__/Command_adb.cpython-39.pyc
--rw-rw-rw-   0        0        0     2932 2022-10-19 05:14:30.000000 Lshengpackage-0.3.5/Lshengpackage/simulate/adb/__pycache__/Pac_adb.cpython-39.pyc
--rw-rw-rw-   0        0        0      162 2022-10-10 08:45:14.000000 Lshengpackage-0.3.5/Lshengpackage/simulate/adb/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2022-12-07 09:41:56.253480 Lshengpackage-0.3.5/Lshengpackage/simulate/dm/
--rw-rw-rw-   0        0        0     4677 2022-05-04 09:06:22.000000 Lshengpackage-0.3.5/Lshengpackage/simulate/dm/Pac_dm.py
--rw-rw-rw-   0        0        0      247 2022-05-26 13:33:04.000000 Lshengpackage-0.3.5/Lshengpackage/simulate/dm/Reg.py
--rw-rw-rw-   0        0        0     9334 2022-05-04 09:06:22.000000 Lshengpackage-0.3.5/Lshengpackage/simulate/dm/Win_dm.py
--rw-rw-rw-   0        0        0       49 2022-10-10 06:18:05.000000 Lshengpackage-0.3.5/Lshengpackage/simulate/dm/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-07 09:41:56.262456 Lshengpackage-0.3.5/Lshengpackage/simulate/dm/__pycache__/
--rw-rw-rw-   0        0        0     4816 2022-10-10 08:45:14.000000 Lshengpackage-0.3.5/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc
--rw-rw-rw-   0        0        0      565 2022-10-10 08:45:14.000000 Lshengpackage-0.3.5/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc
--rw-rw-rw-   0        0        0     1262 2022-10-10 08:45:14.000000 Lshengpackage-0.3.5/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc
--rw-rw-rw-   0        0        0      161 2022-10-10 08:45:14.000000 Lshengpackage-0.3.5/Lshengpackage/simulate/dm/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2022-12-07 09:41:56.267443 Lshengpackage-0.3.5/Lshengpackage/simulate/pc/
--rw-rw-rw-   0        0        0       49 2022-10-10 06:18:05.000000 Lshengpackage-0.3.5/Lshengpackage/simulate/pc/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-07 09:41:56.271434 Lshengpackage-0.3.5/Lshengpackage/simulate/pc/__pycache__/
--rw-rw-rw-   0        0        0      161 2022-10-10 08:40:15.000000 Lshengpackage-0.3.5/Lshengpackage/simulate/pc/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     1315 2022-10-19 01:23:17.000000 Lshengpackage-0.3.5/Lshengpackage/simulate/pc/__pycache__/find_pic.cpython-39.pyc
--rw-rw-rw-   0        0        0      425 2022-10-10 08:45:14.000000 Lshengpackage-0.3.5/Lshengpackage/simulate/pc/__pycache__/find_word.cpython-39.pyc
--rw-rw-rw-   0        0        0     1708 2022-10-18 02:05:31.000000 Lshengpackage-0.3.5/Lshengpackage/simulate/pc/find_pic.py
--rw-rw-rw-   0        0        0      286 2022-06-29 01:11:38.000000 Lshengpackage-0.3.5/Lshengpackage/simulate/pc/find_word.py
-drwxrwxrwx   0        0        0        0 2022-12-07 09:41:56.227550 Lshengpackage-0.3.5/Lshengpackage.egg-info/
--rw-rw-rw-   0        0        0      866 2022-12-07 09:41:56.000000 Lshengpackage-0.3.5/Lshengpackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1594 2022-12-07 09:41:56.000000 Lshengpackage-0.3.5/Lshengpackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-07 09:41:56.000000 Lshengpackage-0.3.5/Lshengpackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2022-12-07 09:41:56.000000 Lshengpackage-0.3.5/Lshengpackage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-12-07 09:41:56.000000 Lshengpackage-0.3.5/Lshengpackage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      288 2022-10-21 09:24:59.000000 Lshengpackage-0.3.5/MANIFEST.in
--rw-rw-rw-   0        0        0      866 2022-12-07 09:41:56.273427 Lshengpackage-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     2460 2022-10-10 08:54:18.000000 Lshengpackage-0.3.5/README.md
--rw-rw-rw-   0        0        0        2 2022-10-10 07:50:18.000000 Lshengpackage-0.3.5/requirements.txt
--rw-rw-rw-   0        0        0       86 2022-12-07 09:41:56.275421 Lshengpackage-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1978 2022-12-07 09:40:02.000000 Lshengpackage-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 04:54:19.732801 Lshengpackage-0.3.6/
+-rw-rw-rw-   0        0        0     1079 2022-05-04 09:06:22.000000 Lshengpackage-0.3.6/LICENSE
+-rw-rw-rw-   0        0        0     1077 2022-05-04 09:06:22.000000 Lshengpackage-0.3.6/License.md
+drwxrwxrwx   0        0        0        0 2023-05-14 04:54:19.674792 Lshengpackage-0.3.6/Lshengpackage/
+-rw-rw-rw-   0        0        0       49 2023-05-14 01:06:32.000000 Lshengpackage-0.3.6/Lshengpackage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 04:54:19.703793 Lshengpackage-0.3.6/Lshengpackage/simulate/
+-rw-rw-rw-   0        0        0       51 2022-10-10 06:17:48.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 04:54:19.704795 Lshengpackage-0.3.6/Lshengpackage/simulate/__pycache__/
+-rw-rw-rw-   0        0        0      158 2022-10-10 08:40:15.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-05-14 04:54:19.707795 Lshengpackage-0.3.6/Lshengpackage/simulate/adb/
+-rw-rw-rw-   0        0        0     2419 2023-05-14 04:20:16.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/adb/Command_adb.py
+-rw-rw-rw-   0        0        0       51 2022-10-10 06:18:05.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/adb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 04:54:19.711792 Lshengpackage-0.3.6/Lshengpackage/simulate/adb/__pycache__/
+-rw-rw-rw-   0        0        0     1852 2022-10-10 06:12:01.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/adb/__pycache__/Command_adb.cpython-39.pyc
+-rw-rw-rw-   0        0        0      162 2022-10-10 08:45:14.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/adb/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-05-14 04:54:19.716793 Lshengpackage-0.3.6/Lshengpackage/simulate/dm/
+-rw-rw-rw-   0        0        0     4677 2022-05-04 09:06:22.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/dm/Pac_dm.py
+-rw-rw-rw-   0        0        0      314 2023-05-14 01:06:32.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/dm/Reg.py
+-rw-rw-rw-   0        0        0     9334 2022-05-04 09:06:22.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/dm/Win_dm.py
+-rw-rw-rw-   0        0        0       49 2022-10-10 06:18:05.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/dm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 04:54:19.724793 Lshengpackage-0.3.6/Lshengpackage/simulate/dm/__pycache__/
+-rw-rw-rw-   0        0        0     4816 2022-10-10 08:45:14.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc
+-rw-rw-rw-   0        0        0      565 2022-10-10 08:45:14.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1262 2022-10-10 08:45:14.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc
+-rw-rw-rw-   0        0        0      161 2022-10-10 08:45:14.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/dm/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      286 2022-06-29 01:11:38.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/mock_findFr.py
+-rw-rw-rw-   0        0        0     2364 2023-05-14 04:20:16.000000 Lshengpackage-0.3.6/Lshengpackage/simulate/mock_findPic.py
+drwxrwxrwx   0        0        0        0 2023-05-14 04:54:19.731792 Lshengpackage-0.3.6/Lshengpackage/tools/
+-rw-rw-rw-   0        0        0     1988 2022-05-26 11:29:53.000000 Lshengpackage-0.3.6/Lshengpackage/tools/ChaoJiYing.py
+-rw-rw-rw-   0        0        0      759 2023-05-14 04:52:50.000000 Lshengpackage-0.3.6/Lshengpackage/tools/General.py
+-rw-rw-rw-   0        0        0      900 2023-05-14 04:31:40.000000 Lshengpackage-0.3.6/Lshengpackage/tools/Loading.py
+-rw-rw-rw-   0        0        0     3305 2023-05-14 01:56:09.000000 Lshengpackage-0.3.6/Lshengpackage/tools/OperateFile.py
+-rw-rw-rw-   0        0        0     2059 2023-05-14 04:52:50.000000 Lshengpackage-0.3.6/Lshengpackage/tools/SearchFile.py
+-rw-rw-rw-   0        0        0       51 2022-10-10 06:17:48.000000 Lshengpackage-0.3.6/Lshengpackage/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 04:54:19.699828 Lshengpackage-0.3.6/Lshengpackage.egg-info/
+-rw-rw-rw-   0        0        0      858 2023-05-14 04:54:19.000000 Lshengpackage-0.3.6/Lshengpackage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1246 2023-05-14 04:54:19.000000 Lshengpackage-0.3.6/Lshengpackage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 04:54:19.000000 Lshengpackage-0.3.6/Lshengpackage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      147 2023-05-14 04:54:19.000000 Lshengpackage-0.3.6/Lshengpackage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-14 04:54:19.000000 Lshengpackage-0.3.6/Lshengpackage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      242 2023-05-14 03:32:07.000000 Lshengpackage-0.3.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      858 2023-05-14 04:54:19.732801 Lshengpackage-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3950 2023-05-14 04:53:00.000000 Lshengpackage-0.3.6/README.md
+-rw-rw-rw-   0        0        0      350 2023-05-14 03:44:13.000000 Lshengpackage-0.3.6/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-05-14 04:54:19.738798 Lshengpackage-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     2056 2023-05-14 03:44:13.000000 Lshengpackage-0.3.6/setup.py
```

### Comparing `Lshengpackage-0.3.5/LICENSE` & `Lshengpackage-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.5/License.md` & `Lshengpackage-0.3.6/License.md`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.5/Lshengpackage/Chaojiying.py` & `Lshengpackage-0.3.6/Lshengpackage/tools/ChaoJiYing.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.5/Lshengpackage/file/search_file.py` & `Lshengpackage-0.3.6/Lshengpackage/tools/SearchFile.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         data = [data_]
         scr = pd.DataFrame(data=data)
         scr.to_csv('path_.csv', index=False, header=False)
         return road
 
 
 # 首次找出路径并保存到存档，会需要点时间
-def find_file_path(paths, filename):
+def searchfile_path(paths, filename):
     if os.path.exists('path_.csv'):
         path = search_in_csv(filename)
         if path:
             return path
         else:
             _find_file = _find_file_path(paths, filename)
             if _find_file:
```

### Comparing `Lshengpackage-0.3.5/Lshengpackage/simulate/adb/__pycache__/Command_adb.cpython-39.pyc` & `Lshengpackage-0.3.6/Lshengpackage/simulate/adb/__pycache__/Command_adb.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.5/Lshengpackage/simulate/dm/Pac_dm.py` & `Lshengpackage-0.3.6/Lshengpackage/simulate/dm/Pac_dm.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.5/Lshengpackage/simulate/dm/Win_dm.py` & `Lshengpackage-0.3.6/Lshengpackage/simulate/dm/Win_dm.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.5/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc` & `Lshengpackage-0.3.6/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.5/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc` & `Lshengpackage-0.3.6/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.5/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc` & `Lshengpackage-0.3.6/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.5/Lshengpackage.egg-info/PKG-INFO` & `Lshengpackage-0.3.6/Lshengpackage.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: Lshengpackage
-Version: 0.3.5
+Version: 0.3.6
 Summary: 个人自动化爬虫开源学习
-Home-page: https://github.com/Lsheng0-0/package
+Home-page: https://lsheng0-0.github.io/
 Download-URL: https://github.com/Lsheng0-0/package
 Author: Lsheng0-0
 Author-email: 1522833718@qq.com
 License: MIT
 Keywords: 游戏,办公,自动化,爬虫
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `Lshengpackage-0.3.5/PKG-INFO` & `Lshengpackage-0.3.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: Lshengpackage
-Version: 0.3.5
+Version: 0.3.6
 Summary: 个人自动化爬虫开源学习
-Home-page: https://github.com/Lsheng0-0/package
+Home-page: https://lsheng0-0.github.io/
 Download-URL: https://github.com/Lsheng0-0/package
 Author: Lsheng0-0
 Author-email: 1522833718@qq.com
 License: MIT
 Keywords: 游戏,办公,自动化,爬虫
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `Lshengpackage-0.3.5/README.md` & `Lshengpackage-0.3.6/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 个人博客：https://lsheng0-0.github.io
 
 作者：凉笙
 
 声名：个人学习开源，仅供学习参考，非商业用途。
 
-自行下载食用：
+> 自行下载食用：
 
-```python
+```cmd
 pip install Lshengpackage
 ```
 
 
 
-> ###关于Command_adb相关模块的调用介绍
+> ###关于Command_adb相关模块的调用介绍(更新)
 >
 
 ```python
 # -*- coding: UTF-8 -*-
 from Lshengpackage.simulate.adb.Command_adb import command  # 调用模块
 
 com = command()  # 调用类
@@ -28,48 +28,68 @@
 com.log()  # 查看日志
 com.up('file_name', 'path_phone')  # file_name:上传文件的名称，需要带文件后缀，path_phone：手机文件路径/sdcard/..
 com.down('file_name')  # 下载：file_name;为文件名称，需要带文件后缀
 com.scr('pic_name')  # 屏幕截图保存到手机根目录/sdcard/..，保存图片的名称.默认png格式
 com.install('apk_name')  # 安装程序：无需后缀，默认apk文件安装
 com.uninstall('apk_name')  # 卸载程序：无需后缀，默认apk文件卸载
 com.video_scr('video_name')  # 屏幕录制：保存视频到手机根目录/sdcard/..,名称,默认mp4格式
+com.cut_scr('path_pic_name', 'path') #屏幕截图到本地 path_pic_name:截图手机路径 path：本地程序图片路径
+com.spec_scr('path_pic_name', 'path', 'int_x1', 'int_y1', 'int_x2', 'int_y2') # 屏幕指定范围截图到本地 path_pic_name:截图手机路径 path：本地程序图片路径
+#int_x1, int_y1, int_x2, int_y2 分别是左上角和右下角的点左边,转文字用
+com.tap_work('x', 'y') #模拟手动点击 x，y为坐标
+com.swip_work('x', 'y', 'x2', 'y2') # 模拟手动滑动，x, y, x2, y2为第一个点到第二个点
 ```
 > ###关于超级鹰验证码识别的调用-Python
 >[注册超级鹰账号](http://www.chaojiying.com/user/reg/)
 
 用户中心 ->软件ID ->生成软件ID
 
 调用方法：
 
 ```python
-from Lshengpackage.Chaojiying import Verification
+from Lshengpackage.tools.ChaoJiYing import Verification
 
 # 处理验证码
 
 verify = Verification()  # 调用超级鹰模块
 verify_code = verify.verification_code('超级鹰登录用户名', '超级鹰登录密码', '软件ID号', img)
 # 外部请求超级鹰，img为验证码路劲图片文件
 print(verify_code['pic_str'])
 # 打印验证码
 ```
 
-> ###新增pc找图定位模块 v3.0
+> ###找图定位、转文字模块 v3.0-3.6(更新)
 
 ```python
-from Lshengpackage.simulate.pc import find_word,find_pic
+from Lshengpackage.simulate.mock_findFr import  fr
 
+word = fr(img='')  #图片识字
+print(word)
 
-find_word.fr(img='')  #图片识字
-find_pic.screen_shot() #屏幕截图(默认为根目录pic文件夹下)
-find_pic.find_image(target='')  #当前页面找图,找到匹配对象位置中心点（参数对应需要寻找的图片路径名称)
+from Lshengpackage.simulate.mock_findPic import screen_shot,find_image
+screen_shot('截图的路径','截图的名') #pc桌面截图保存图片到指定位置
+find_image('获取图片文件夹', '目标图片文件夹', '目标名称.png',)  #当前页面找图,找到匹配对象位置中心点（参数对应需要寻找的图片路径名称)
 #成功返回中心点坐标，否则为空值
-from Lshengpackage.Load import load,load_click
+from Lshengpackage.tools.Loading import load,load_click
 
 #页面刷新等待，直到找到目标并点击
 # 设置自动防故障功能（将鼠标移动到左上角将停止程序）
-load(img='')  
+load('获取图片文件夹', '目标图片文件夹', '目标名称.png')  
 #直到找到目标返回坐标值
-load_click(img='')  
-#找到目标返回坐标值,并点击
+load_click('获取图片文件夹', '目标图片文件夹', '目标名称.png')  
+#找到目标坐标点击,成功范围True，失败返回False 鼠标移至（0,0）退出程序
+```
+> ###其他的一些工具模块 v3.6(更新)
+>
+```python
+
+from Lshengpackage.tools.General import  Delay,Enter_Ch
+
+Delay.delay() #随机等待时间
+
+Enter_Ch.insert('需要输入的文字内容') #模拟输入中文文字
 
+from Lshengpackage.tools.SearchFile import searchfile_path,search_it
+search_it('文件路径', '文件名') #检索遍历根目录下的所有文件，找到指定文件为止
+searchfile_path('文件路径', '文件名') #找到指定文件后进行缓存，下次可直接提去（可用于未指定路径文件，自搜索）
 
 ```
```

### Comparing `Lshengpackage-0.3.5/setup.py` & `Lshengpackage-0.3.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from distutils.core import setup
 
 setup(
     name='Lshengpackage',  # How you named your package folder (MyLib)
     packages=['Lshengpackage'],  # Chose the same as "name"
-    version='0.3.5',  # Start with a small number and increase it with every change you make
+    version='0.3.6',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='个人自动化爬虫开源学习',  # Give a short description about your library
     # long_description=open('README.md', 'r', encoding='utf-8').read(),
     author='Lsheng0-0',  # Type in your name
     author_email='1522833718@qq.com',  # Type in your E-Mail
-    url='https://github.com/Lsheng0-0/package',  # Provide either the link to your github or to your website
+    url='https://lsheng0-0.github.io/',  # Provide either the link to your github or to your website
     download_url='https://github.com/Lsheng0-0/package',  # I explain this later on
     include_package_data=True,
     install_requires=[  # I get to this in a second
-        'numpy',
-        'aircv',
-        'Pillow',
-        'opencv-python',
-        'pywin32',
-        'requests',
-        'pyautogui',
-        'pytesseract',
+        'openpyxl~=3.0.9',
+        'pandas~=1.4.3',
+        'PyAutoGUI~=0.9.53',
+        'pyperclip~=1.8.2',
+        'opencv-python~=4.5.1.48',
+        'Pillow~=9.1.1',
+        'aircv~=1.4.6',
+        'numpy~=1.22.4',
+        'requests~=2.27.1'
     ],
     keywords=['游戏', '办公', '自动化', '爬虫'],  # Keywords that define your package best
     classifiers=[
         'Development Status :: 3 - Alpha',
         # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Intended Audience :: Developers',  # Define that your audience are developers
         'Topic :: Software Development :: Build Tools',
```

