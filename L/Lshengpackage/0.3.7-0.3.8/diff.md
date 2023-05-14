# Comparing `tmp/Lshengpackage-0.3.7.tar.gz` & `tmp/Lshengpackage-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lshengpackage-0.3.7.tar", last modified: Sun May 14 07:51:12 2023, max compression
+gzip compressed data, was "Lshengpackage-0.3.8.tar", last modified: Sun May 14 08:46:08 2023, max compression
```

## Comparing `Lshengpackage-0.3.7.tar` & `Lshengpackage-0.3.8.tar`

### file list

```diff
@@ -1,45 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 07:51:12.113356 Lshengpackage-0.3.7/
--rw-rw-rw-   0        0        0     1079 2022-05-04 09:06:22.000000 Lshengpackage-0.3.7/LICENSE
--rw-rw-rw-   0        0        0     1077 2022-05-04 09:06:22.000000 Lshengpackage-0.3.7/License.md
-drwxrwxrwx   0        0        0        0 2023-05-14 07:51:12.051769 Lshengpackage-0.3.7/Lshengpackage/
--rw-rw-rw-   0        0        0       49 2023-05-14 01:06:32.000000 Lshengpackage-0.3.7/Lshengpackage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 07:51:12.071298 Lshengpackage-0.3.7/Lshengpackage/simulate/
--rw-rw-rw-   0        0        0       51 2022-10-10 06:17:48.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 07:51:12.073305 Lshengpackage-0.3.7/Lshengpackage/simulate/__pycache__/
--rw-rw-rw-   0        0        0      158 2022-10-10 08:40:15.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-05-14 07:51:12.076298 Lshengpackage-0.3.7/Lshengpackage/simulate/adb/
--rw-rw-rw-   0        0        0     2689 2023-05-14 07:49:17.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/adb/Command_adb.py
--rw-rw-rw-   0        0        0       51 2022-10-10 06:18:05.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/adb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 07:51:12.078299 Lshengpackage-0.3.7/Lshengpackage/simulate/adb/__pycache__/
--rw-rw-rw-   0        0        0      162 2022-10-10 08:45:14.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/adb/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-05-14 07:51:12.089827 Lshengpackage-0.3.7/Lshengpackage/simulate/dm/
--rw-rw-rw-   0        0        0     4677 2022-05-04 09:06:22.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/dm/Pac_dm.py
--rw-rw-rw-   0        0        0      314 2023-05-14 01:06:32.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/dm/Reg.py
--rw-rw-rw-   0        0        0     9334 2022-05-04 09:06:22.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/dm/Win_dm.py
--rw-rw-rw-   0        0        0       49 2022-10-10 06:18:05.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/dm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 07:51:12.099347 Lshengpackage-0.3.7/Lshengpackage/simulate/dm/__pycache__/
--rw-rw-rw-   0        0        0     4816 2022-10-10 08:45:14.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc
--rw-rw-rw-   0        0        0      565 2022-10-10 08:45:14.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc
--rw-rw-rw-   0        0        0     1262 2022-10-10 08:45:14.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc
--rw-rw-rw-   0        0        0      161 2022-10-10 08:45:14.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/dm/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      286 2022-06-29 01:11:38.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/mock_findFr.py
--rw-rw-rw-   0        0        0     2364 2023-05-14 04:20:16.000000 Lshengpackage-0.3.7/Lshengpackage/simulate/mock_findPic.py
-drwxrwxrwx   0        0        0        0 2023-05-14 07:51:12.112354 Lshengpackage-0.3.7/Lshengpackage/tools/
--rw-rw-rw-   0        0        0     1988 2022-05-26 11:29:53.000000 Lshengpackage-0.3.7/Lshengpackage/tools/ChaoJiYing.py
--rw-rw-rw-   0        0        0      759 2023-05-14 04:52:50.000000 Lshengpackage-0.3.7/Lshengpackage/tools/General.py
--rw-rw-rw-   0        0        0      900 2023-05-14 04:31:40.000000 Lshengpackage-0.3.7/Lshengpackage/tools/Loading.py
--rw-rw-rw-   0        0        0     3305 2023-05-14 01:56:09.000000 Lshengpackage-0.3.7/Lshengpackage/tools/OperateFile.py
--rw-rw-rw-   0        0        0     2059 2023-05-14 04:52:50.000000 Lshengpackage-0.3.7/Lshengpackage/tools/SearchFile.py
--rw-rw-rw-   0        0        0       51 2022-10-10 06:17:48.000000 Lshengpackage-0.3.7/Lshengpackage/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 07:51:12.064278 Lshengpackage-0.3.7/Lshengpackage.egg-info/
--rw-rw-rw-   0        0        0      858 2023-05-14 07:51:11.000000 Lshengpackage-0.3.7/Lshengpackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1180 2023-05-14 07:51:11.000000 Lshengpackage-0.3.7/Lshengpackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 07:51:11.000000 Lshengpackage-0.3.7/Lshengpackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      147 2023-05-14 07:51:11.000000 Lshengpackage-0.3.7/Lshengpackage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-14 07:51:11.000000 Lshengpackage-0.3.7/Lshengpackage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      242 2023-05-14 03:32:07.000000 Lshengpackage-0.3.7/MANIFEST.in
--rw-rw-rw-   0        0        0      858 2023-05-14 07:51:12.114355 Lshengpackage-0.3.7/PKG-INFO
--rw-rw-rw-   0        0        0     3975 2023-05-14 07:50:08.000000 Lshengpackage-0.3.7/README.md
--rw-rw-rw-   0        0        0      350 2023-05-14 03:44:13.000000 Lshengpackage-0.3.7/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-05-14 07:51:12.116451 Lshengpackage-0.3.7/setup.cfg
--rw-rw-rw-   0        0        0     2056 2023-05-14 07:49:26.000000 Lshengpackage-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 08:46:08.227055 Lshengpackage-0.3.8/
+-rw-rw-rw-   0        0        0     1079 2022-05-04 09:06:22.000000 Lshengpackage-0.3.8/LICENSE
+-rw-rw-rw-   0        0        0     1077 2022-05-04 09:06:22.000000 Lshengpackage-0.3.8/License.md
+drwxrwxrwx   0        0        0        0 2023-05-14 08:46:08.191886 Lshengpackage-0.3.8/Lshengpackage/
+-rw-rw-rw-   0        0        0       49 2023-05-14 01:06:32.000000 Lshengpackage-0.3.8/Lshengpackage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 08:46:08.201396 Lshengpackage-0.3.8/Lshengpackage/simulate/
+-rw-rw-rw-   0        0        0       51 2022-10-10 06:17:48.000000 Lshengpackage-0.3.8/Lshengpackage/simulate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 08:46:08.203396 Lshengpackage-0.3.8/Lshengpackage/simulate/adb/
+-rw-rw-rw-   0        0        0     2689 2023-05-14 07:49:17.000000 Lshengpackage-0.3.8/Lshengpackage/simulate/adb/Command_adb.py
+-rw-rw-rw-   0        0        0       51 2022-10-10 06:18:05.000000 Lshengpackage-0.3.8/Lshengpackage/simulate/adb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 08:46:08.204901 Lshengpackage-0.3.8/Lshengpackage/simulate/adb/__pycache__/
+-rw-rw-rw-   0        0        0      162 2022-10-10 08:45:14.000000 Lshengpackage-0.3.8/Lshengpackage/simulate/adb/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-05-14 08:46:08.210918 Lshengpackage-0.3.8/Lshengpackage/simulate/dm/
+-rw-rw-rw-   0        0        0     4677 2022-05-04 09:06:22.000000 Lshengpackage-0.3.8/Lshengpackage/simulate/dm/Pac_dm.py
+-rw-rw-rw-   0        0        0      314 2023-05-14 01:06:32.000000 Lshengpackage-0.3.8/Lshengpackage/simulate/dm/Reg.py
+-rw-rw-rw-   0        0        0     9334 2022-05-04 09:06:22.000000 Lshengpackage-0.3.8/Lshengpackage/simulate/dm/Win_dm.py
+-rw-rw-rw-   0        0        0       49 2022-10-10 06:18:05.000000 Lshengpackage-0.3.8/Lshengpackage/simulate/dm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 08:46:08.217048 Lshengpackage-0.3.8/Lshengpackage/simulate/dm/__pycache__/
+-rw-rw-rw-   0        0        0     4816 2022-10-10 08:45:14.000000 Lshengpackage-0.3.8/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc
+-rw-rw-rw-   0        0        0      565 2022-10-10 08:45:14.000000 Lshengpackage-0.3.8/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1262 2022-10-10 08:45:14.000000 Lshengpackage-0.3.8/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc
+-rw-rw-rw-   0        0        0      161 2022-10-10 08:45:14.000000 Lshengpackage-0.3.8/Lshengpackage/simulate/dm/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      286 2022-06-29 01:11:38.000000 Lshengpackage-0.3.8/Lshengpackage/simulate/mock_findFr.py
+-rw-rw-rw-   0        0        0     2364 2023-05-14 04:20:16.000000 Lshengpackage-0.3.8/Lshengpackage/simulate/mock_findPic.py
+drwxrwxrwx   0        0        0        0 2023-05-14 08:46:08.225052 Lshengpackage-0.3.8/Lshengpackage/tools/
+-rw-rw-rw-   0        0        0     1988 2022-05-26 11:29:53.000000 Lshengpackage-0.3.8/Lshengpackage/tools/ChaoJiYing.py
+-rw-rw-rw-   0        0        0      759 2023-05-14 04:52:50.000000 Lshengpackage-0.3.8/Lshengpackage/tools/General.py
+-rw-rw-rw-   0        0        0      900 2023-05-14 04:31:40.000000 Lshengpackage-0.3.8/Lshengpackage/tools/Loading.py
+-rw-rw-rw-   0        0        0     3305 2023-05-14 01:56:09.000000 Lshengpackage-0.3.8/Lshengpackage/tools/OperateFile.py
+-rw-rw-rw-   0        0        0     2059 2023-05-14 04:52:50.000000 Lshengpackage-0.3.8/Lshengpackage/tools/SearchFile.py
+-rw-rw-rw-   0        0        0       51 2022-10-10 06:17:48.000000 Lshengpackage-0.3.8/Lshengpackage/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 08:46:08.197885 Lshengpackage-0.3.8/Lshengpackage.egg-info/
+-rw-rw-rw-   0        0        0      858 2023-05-14 08:46:08.000000 Lshengpackage-0.3.8/Lshengpackage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1121 2023-05-14 08:46:08.000000 Lshengpackage-0.3.8/Lshengpackage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 08:46:08.000000 Lshengpackage-0.3.8/Lshengpackage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      147 2023-05-14 08:46:08.000000 Lshengpackage-0.3.8/Lshengpackage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-14 08:46:08.000000 Lshengpackage-0.3.8/Lshengpackage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      242 2023-05-14 03:32:07.000000 Lshengpackage-0.3.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      858 2023-05-14 08:46:08.227055 Lshengpackage-0.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3975 2023-05-14 07:50:08.000000 Lshengpackage-0.3.8/README.md
+-rw-rw-rw-   0        0        0      350 2023-05-14 03:44:13.000000 Lshengpackage-0.3.8/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-05-14 08:46:08.228053 Lshengpackage-0.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     2056 2023-05-14 08:46:01.000000 Lshengpackage-0.3.8/setup.py
```

### Comparing `Lshengpackage-0.3.7/LICENSE` & `Lshengpackage-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.7/License.md` & `Lshengpackage-0.3.8/License.md`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.7/Lshengpackage/simulate/adb/Command_adb.py` & `Lshengpackage-0.3.8/Lshengpackage/simulate/adb/Command_adb.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.7/Lshengpackage/simulate/dm/Pac_dm.py` & `Lshengpackage-0.3.8/Lshengpackage/simulate/dm/Pac_dm.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.7/Lshengpackage/simulate/dm/Win_dm.py` & `Lshengpackage-0.3.8/Lshengpackage/simulate/dm/Win_dm.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.7/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc` & `Lshengpackage-0.3.8/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.7/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc` & `Lshengpackage-0.3.8/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.7/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc` & `Lshengpackage-0.3.8/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.7/Lshengpackage/simulate/mock_findPic.py` & `Lshengpackage-0.3.8/Lshengpackage/simulate/mock_findPic.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.7/Lshengpackage/tools/ChaoJiYing.py` & `Lshengpackage-0.3.8/Lshengpackage/tools/ChaoJiYing.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.7/Lshengpackage/tools/General.py` & `Lshengpackage-0.3.8/Lshengpackage/tools/General.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.7/Lshengpackage/tools/Loading.py` & `Lshengpackage-0.3.8/Lshengpackage/tools/Loading.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.7/Lshengpackage/tools/OperateFile.py` & `Lshengpackage-0.3.8/Lshengpackage/tools/OperateFile.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.7/Lshengpackage/tools/SearchFile.py` & `Lshengpackage-0.3.8/Lshengpackage/tools/SearchFile.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.7/Lshengpackage.egg-info/PKG-INFO` & `Lshengpackage-0.3.8/Lshengpackage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lshengpackage
-Version: 0.3.7
+Version: 0.3.8
 Summary: 个人自动化爬虫开源学习
 Home-page: https://lsheng0-0.github.io/
 Download-URL: https://github.com/Lsheng0-0/package
 Author: Lsheng0-0
 Author-email: 1522833718@qq.com
 License: MIT
 Keywords: 游戏,办公,自动化,爬虫
```

### Comparing `Lshengpackage-0.3.7/Lshengpackage.egg-info/SOURCES.txt` & `Lshengpackage-0.3.8/Lshengpackage.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 Lshengpackage.egg-info/SOURCES.txt
 Lshengpackage.egg-info/dependency_links.txt
 Lshengpackage.egg-info/requires.txt
 Lshengpackage.egg-info/top_level.txt
 Lshengpackage/simulate/__init__.py
 Lshengpackage/simulate/mock_findFr.py
 Lshengpackage/simulate/mock_findPic.py
-Lshengpackage/simulate/__pycache__/__init__.cpython-39.pyc
 Lshengpackage/simulate/adb/Command_adb.py
 Lshengpackage/simulate/adb/__init__.py
 Lshengpackage/simulate/adb/__pycache__/__init__.cpython-39.pyc
 Lshengpackage/simulate/dm/Pac_dm.py
 Lshengpackage/simulate/dm/Reg.py
 Lshengpackage/simulate/dm/Win_dm.py
 Lshengpackage/simulate/dm/__init__.py
```

### Comparing `Lshengpackage-0.3.7/PKG-INFO` & `Lshengpackage-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lshengpackage
-Version: 0.3.7
+Version: 0.3.8
 Summary: 个人自动化爬虫开源学习
 Home-page: https://lsheng0-0.github.io/
 Download-URL: https://github.com/Lsheng0-0/package
 Author: Lsheng0-0
 Author-email: 1522833718@qq.com
 License: MIT
 Keywords: 游戏,办公,自动化,爬虫
```

### Comparing `Lshengpackage-0.3.7/README.md` & `Lshengpackage-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.7/setup.py` & `Lshengpackage-0.3.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='Lshengpackage',  # How you named your package folder (MyLib)
     packages=['Lshengpackage'],  # Chose the same as "name"
-    version='0.3.7',  # Start with a small number and increase it with every change you make
+    version='0.3.8',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='个人自动化爬虫开源学习',  # Give a short description about your library
     # long_description=open('README.md', 'r', encoding='utf-8').read(),
     author='Lsheng0-0',  # Type in your name
     author_email='1522833718@qq.com',  # Type in your E-Mail
     url='https://lsheng0-0.github.io/',  # Provide either the link to your github or to your website
     download_url='https://github.com/Lsheng0-0/package',  # I explain this later on
```

