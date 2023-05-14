# Comparing `tmp/Qpro-0.9.8.tar.gz` & `tmp/Qpro-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Qpro-0.9.8.tar", last modified: Fri May  6 23:56:26 2022, max compression
+gzip compressed data, was "Qpro-0.9.9.tar", last modified: Sat May 21 09:02:51 2022, max compression
```

## Comparing `Qpro-0.9.8.tar` & `Qpro-0.9.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-05-06 23:56:26.122923 Qpro-0.9.8/
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     1067 2019-09-13 15:12:28.000000 Qpro-0.9.8/LICENSE
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      864 2022-05-06 23:56:26.122994 Qpro-0.9.8/PKG-INFO
-drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-05-06 23:56:26.120875 Qpro-0.9.8/Qpro.egg-info/
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      864 2022-05-06 23:56:26.000000 Qpro-0.9.8/Qpro.egg-info/PKG-INFO
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      452 2022-05-06 23:56:26.000000 Qpro-0.9.8/Qpro.egg-info/SOURCES.txt
--rw-r--r--   0 lianhaocheng   (501) staff       (20)        1 2022-05-06 23:56:26.000000 Qpro-0.9.8/Qpro.egg-info/dependency_links.txt
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      147 2022-05-06 23:56:26.000000 Qpro-0.9.8/Qpro.egg-info/entry_points.txt
--rw-r--r--   0 lianhaocheng   (501) staff       (20)       38 2022-05-06 23:56:26.000000 Qpro-0.9.8/Qpro.egg-info/requires.txt
--rw-r--r--   0 lianhaocheng   (501) staff       (20)       13 2022-05-06 23:56:26.000000 Qpro-0.9.8/Qpro.egg-info/top_level.txt
--rw-r--r--   0 lianhaocheng   (501) staff       (20)        1 2019-09-13 15:52:47.000000 Qpro-0.9.8/Qpro.egg-info/zip-safe
-drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-05-06 23:56:26.122749 Qpro-0.9.8/QuickProject/
--rw-r--r--   0 lianhaocheng   (501) staff       (20)    10507 2022-05-03 08:45:03.000000 Qpro-0.9.8/QuickProject/Commander.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)    30935 2022-05-06 23:53:31.000000 Qpro-0.9.8/QuickProject/Qpro.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     9670 2022-04-25 16:35:30.000000 Qpro-0.9.8/QuickProject/QproFigTable.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      564 2022-04-25 16:17:48.000000 Qpro-0.9.8/QuickProject/QproZshComp.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     3396 2022-04-27 12:51:00.000000 Qpro-0.9.8/QuickProject/__config__.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     9995 2022-05-06 01:43:39.000000 Qpro-0.9.8/QuickProject/__init__.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     3862 2021-06-17 15:57:48.000000 Qpro-0.9.8/QuickProject/detector.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     5750 2022-04-13 01:23:47.000000 Qpro-0.9.8/QuickProject/qrun.py
--rwxr-xr-x   0 lianhaocheng   (501) staff       (20)     7909 2021-10-24 10:06:19.000000 Qpro-0.9.8/QuickProject/tmpm.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      421 2022-01-29 11:54:42.000000 Qpro-0.9.8/README.md
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      140 2022-05-06 23:56:26.123215 Qpro-0.9.8/setup.cfg
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     1078 2022-05-06 23:53:43.000000 Qpro-0.9.8/setup.py
+drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-05-21 09:02:51.900154 Qpro-0.9.9/
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     1067 2019-09-13 15:12:28.000000 Qpro-0.9.9/LICENSE
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      864 2022-05-21 09:02:51.900217 Qpro-0.9.9/PKG-INFO
+drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-05-21 09:02:51.897778 Qpro-0.9.9/Qpro.egg-info/
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      864 2022-05-21 09:02:51.000000 Qpro-0.9.9/Qpro.egg-info/PKG-INFO
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      452 2022-05-21 09:02:51.000000 Qpro-0.9.9/Qpro.egg-info/SOURCES.txt
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)        1 2022-05-21 09:02:51.000000 Qpro-0.9.9/Qpro.egg-info/dependency_links.txt
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      146 2022-05-21 09:02:51.000000 Qpro-0.9.9/Qpro.egg-info/entry_points.txt
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)       38 2022-05-21 09:02:51.000000 Qpro-0.9.9/Qpro.egg-info/requires.txt
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)       13 2022-05-21 09:02:51.000000 Qpro-0.9.9/Qpro.egg-info/top_level.txt
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)        1 2019-09-13 15:52:47.000000 Qpro-0.9.9/Qpro.egg-info/zip-safe
+drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-05-21 09:02:51.899970 Qpro-0.9.9/QuickProject/
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)    10507 2022-05-03 08:45:03.000000 Qpro-0.9.9/QuickProject/Commander.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)    31177 2022-05-21 08:10:12.000000 Qpro-0.9.9/QuickProject/Qpro.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     9670 2022-04-25 16:35:30.000000 Qpro-0.9.9/QuickProject/QproFigTable.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      564 2022-04-25 16:17:48.000000 Qpro-0.9.9/QuickProject/QproZshComp.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     3396 2022-04-27 12:51:00.000000 Qpro-0.9.9/QuickProject/__config__.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     9995 2022-05-06 01:43:39.000000 Qpro-0.9.9/QuickProject/__init__.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     3862 2021-06-17 15:57:48.000000 Qpro-0.9.9/QuickProject/detector.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     5750 2022-04-13 01:23:47.000000 Qpro-0.9.9/QuickProject/qrun.py
+-rwxr-xr-x   0 lianhaocheng   (501) staff       (20)     7909 2021-10-24 10:06:19.000000 Qpro-0.9.9/QuickProject/tmpm.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      421 2022-01-29 11:54:42.000000 Qpro-0.9.9/README.md
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      140 2022-05-21 09:02:51.900420 Qpro-0.9.9/setup.cfg
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     1078 2022-05-21 09:02:23.000000 Qpro-0.9.9/setup.py
```

### Comparing `Qpro-0.9.8/LICENSE` & `Qpro-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Qpro-0.9.8/PKG-INFO` & `Qpro-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Qpro
-Version: 0.9.8
+Version: 0.9.9
 Summary: Small but powerful command line IDE.
 Home-page: https://github.com/Rhythmicc/QuickProject
 Author: RhythmLian
 License: MIT
 Keywords: script for CLionProjects
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Qpro-0.9.8/Qpro.egg-info/PKG-INFO` & `Qpro-0.9.9/Qpro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Qpro
-Version: 0.9.8
+Version: 0.9.9
 Summary: Small but powerful command line IDE.
 Home-page: https://github.com/Rhythmicc/QuickProject
 Author: RhythmLian
 License: MIT
 Keywords: script for CLionProjects
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Qpro-0.9.8/QuickProject/Commander.py` & `Qpro-0.9.9/QuickProject/Commander.py`

 * *Files identical despite different names*

### Comparing `Qpro-0.9.8/QuickProject/Qpro.py` & `Qpro-0.9.9/QuickProject/Qpro.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,15 +371,15 @@
 
 
 def delete_all():
     server_targets = get_server_targets()
     st = 0
     for server_target in server_targets:
         _st = SshProtocol.command(server_target['user'], server_target['host'], server_target['path'], server_target['port'], 'rm -rf .')
-        st |= _st
+        st |= 1 if _st else 0
         QproDefaultConsole.print(QproErrorString, f'{server_target}: delete all failed with error: {st}')
     if not st:
         remove(os.getcwd())
 
 
 def delete():
     try:
@@ -399,16 +399,17 @@
                     (f"{path} 不在当前 Qpro 项目中!" if os.path.exists(path) else f'该路径不存在: {path}')
                 )
         server_targets = get_server_targets()
         st = 0
         for server_target in server_targets:
             _st = SshProtocol.command(server_target['user'], server_target['host'], server_target['path'],
                                       server_target['port'], f'rm -rf {sub_path}')
-            st |= _st
-            QproDefaultConsole.print(QproErrorString, f'{server_target}: delete {sub_path} failed with error: {st}')
+            st |= 1 if _st else 0
+            if _st:
+                QproDefaultConsole.print(QproErrorString, f'{server_target}: delete {sub_path} failed with error: {_st}')
         if not st or _ask({
             'type': 'confirm',
             'name': 'confirm',
             'message': f'{path} is not in this Qpro project! Do you want to delete it?' if user_lang != 'zh' else f'{path} 不在当前 Qpro 项目中! 是否删除?',
         }):
             remove(sub_path)
 
@@ -483,14 +484,16 @@
         os.mkdir(os.path.join(QproGlobalDir, 'bin'))
     if not os.path.exists(os.path.join(QproGlobalDir, 'fig')):
         os.mkdir(os.path.join(QproGlobalDir, 'fig'))
     return QproGlobalDir
 
 
 def register_global_command():
+    if not os.path.exists(configure_name):
+        return QproDefaultConsole.print(QproErrorString, f'{configure_name} is not exists!' if user_lang != 'zh' else f'{configure_name} 不存在!')
     if is_win:
         return QproDefaultConsole.print(QproWarnString, 'Not Support Windows!' if user_lang != 'zh' else '不支持 Windows!')
     QproGlobalDir = __get_Qpro_fig_Dir()
     if not QproGlobalDir:
         return
     import json
```

### Comparing `Qpro-0.9.8/QuickProject/QproFigTable.py` & `Qpro-0.9.9/QuickProject/QproFigTable.py`

 * *Files identical despite different names*

### Comparing `Qpro-0.9.8/QuickProject/QproZshComp.py` & `Qpro-0.9.9/QuickProject/QproZshComp.py`

 * *Files identical despite different names*

### Comparing `Qpro-0.9.8/QuickProject/__config__.py` & `Qpro-0.9.9/QuickProject/__config__.py`

 * *Files identical despite different names*

### Comparing `Qpro-0.9.8/QuickProject/__init__.py` & `Qpro-0.9.9/QuickProject/__init__.py`

 * *Files identical despite different names*

### Comparing `Qpro-0.9.8/QuickProject/detector.py` & `Qpro-0.9.9/QuickProject/detector.py`

 * *Files identical despite different names*

### Comparing `Qpro-0.9.8/QuickProject/qrun.py` & `Qpro-0.9.9/QuickProject/qrun.py`

 * *Files identical despite different names*

### Comparing `Qpro-0.9.8/QuickProject/tmpm.py` & `Qpro-0.9.9/QuickProject/tmpm.py`

 * *Files identical despite different names*

### Comparing `Qpro-0.9.8/setup.py` & `Qpro-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
-VERSION = '0.9.8'
+VERSION = '0.9.9'
 
 setup(
     name='Qpro',
     version=VERSION,
     description='Small but powerful command line IDE.',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

