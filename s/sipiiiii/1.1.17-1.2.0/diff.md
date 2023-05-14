# Comparing `tmp/sipiiiii-1.1.17.tar.gz` & `tmp/sipiiiii-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sipiiiii-1.1.17.tar", last modified: Sun May 14 14:26:41 2023, max compression
+gzip compressed data, was "sipiiiii-1.2.0.tar", last modified: Sun May 14 14:30:01 2023, max compression
```

## Comparing `sipiiiii-1.1.17.tar` & `sipiiiii-1.2.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-14 14:26:41.218494 sipiiiii-1.1.17/
--rw-r--r--   0 j0hn       (501) staff       (20)       18 2023-05-03 12:00:50.000000 sipiiiii-1.1.17/MANIFEST.in
--rw-r--r--   0 j0hn       (501) staff       (20)     3789 2023-05-14 14:26:41.217826 sipiiiii-1.1.17/PKG-INFO
--rw-r--r--   0 j0hn       (501) staff       (20)     3271 2023-05-11 16:47:37.000000 sipiiiii-1.1.17/README.md
--rw-r--r--   0 j0hn       (501) staff       (20)      635 2023-05-14 14:25:01.000000 sipiiiii-1.1.17/pyproject.toml
--rw-r--r--   0 j0hn       (501) staff       (20)       38 2023-05-14 14:26:41.218751 sipiiiii-1.1.17/setup.cfg
--rw-r--r--   0 j0hn       (501) staff       (20)     3402 2023-05-14 14:25:01.000000 sipiiiii-1.1.17/setup.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-14 14:26:41.192188 sipiiiii-1.1.17/sipiiiii/
--rw-r--r--   0 j0hn       (501) staff       (20)       22 2023-03-28 16:40:14.000000 sipiiiii-1.1.17/sipiiiii/__init__.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-14 14:26:41.200971 sipiiiii-1.1.17/sipiiiii/app/
--rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-28 03:21:50.000000 sipiiiii-1.1.17/sipiiiii/app/__init__.py
--rw-r--r--   0 j0hn       (501) staff       (20)    13002 2023-05-11 17:42:48.000000 sipiiiii-1.1.17/sipiiiii/app/core.py
--rw-r--r--   0 j0hn       (501) staff       (20)    22242 2023-05-14 14:25:12.000000 sipiiiii-1.1.17/sipiiiii/app/new_app.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-14 14:26:41.206311 sipiiiii-1.1.17/sipiiiii/app/utils/
--rw-r--r--   0 j0hn       (501) staff       (20)     7845 2023-05-03 09:19:05.000000 sipiiiii-1.1.17/sipiiiii/app/utils/HttpSDK.py
--rw-r--r--   0 j0hn       (501) staff       (20)     1712 2023-05-14 14:11:29.000000 sipiiiii-1.1.17/sipiiiii/app/utils/Tools.py
--rw-r--r--   0 j0hn       (501) staff       (20)      735 2023-03-30 02:41:50.000000 sipiiiii-1.1.17/sipiiiii/app/utils/ZipFileTool.py
--rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-30 02:41:28.000000 sipiiiii-1.1.17/sipiiiii/app/utils/__init__.py
--rw-r--r--   0 j0hn       (501) staff       (20)      151 2023-05-04 12:35:33.000000 sipiiiii-1.1.17/sipiiiii/app/utils/config.py
--rw-r--r--   0 j0hn       (501) staff       (20)     1325 2023-01-05 06:18:13.000000 sipiiiii-1.1.17/sipiiiii/app/utils/formatConversion.py
--rw-r--r--   0 j0hn       (501) staff       (20)       18 2023-05-14 14:25:01.000000 sipiiiii-1.1.17/sipiiiii/app/version.py
--rw-r--r--   0 j0hn       (501) staff       (20)     8341 2023-05-11 17:10:16.000000 sipiiiii-1.1.17/sipiiiii/main.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-14 14:26:41.197155 sipiiiii-1.1.17/sipiiiii.egg-info/
--rw-r--r--   0 j0hn       (501) staff       (20)     3789 2023-05-14 14:26:40.000000 sipiiiii-1.1.17/sipiiiii.egg-info/PKG-INFO
--rw-r--r--   0 j0hn       (501) staff       (20)      821 2023-05-14 14:26:41.000000 sipiiiii-1.1.17/sipiiiii.egg-info/SOURCES.txt
--rw-r--r--   0 j0hn       (501) staff       (20)        1 2023-05-14 14:26:41.000000 sipiiiii-1.1.17/sipiiiii.egg-info/dependency_links.txt
--rw-r--r--   0 j0hn       (501) staff       (20)       48 2023-05-14 14:26:41.000000 sipiiiii-1.1.17/sipiiiii.egg-info/entry_points.txt
--rw-r--r--   0 j0hn       (501) staff       (20)      104 2023-05-14 14:26:41.000000 sipiiiii-1.1.17/sipiiiii.egg-info/requires.txt
--rw-r--r--   0 j0hn       (501) staff       (20)        9 2023-05-14 14:26:41.000000 sipiiiii-1.1.17/sipiiiii.egg-info/top_level.txt
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-14 14:26:41.216943 sipiiiii-1.1.17/template/
--rw-r--r--   0 j0hn       (501) staff       (20)      366 2023-04-18 15:46:14.000000 sipiiiii-1.1.17/template/python_fastapi.j2
--rw-r--r--   0 j0hn       (501) staff       (20)      371 2023-05-04 06:44:54.000000 sipiiiii-1.1.17/template/python_flask.j2
--rw-r--r--   0 j0hn       (501) staff       (20)     1505 2023-05-01 16:17:11.000000 sipiiiii-1.1.17/template/python_openai.j2
--rw-r--r--   0 j0hn       (501) staff       (20)      238 2023-05-04 06:44:09.000000 sipiiiii-1.1.17/template/python_streamlit.j2
--rw-r--r--   0 j0hn       (501) staff       (20)      762 2023-05-01 16:06:57.000000 sipiiiii-1.1.17/template/template_fastapi.yaml
--rw-r--r--   0 j0hn       (501) staff       (20)      762 2023-05-04 06:17:59.000000 sipiiiii-1.1.17/template/template_flask.yaml
--rw-r--r--   0 j0hn       (501) staff       (20)      795 2023-05-03 13:15:30.000000 sipiiiii-1.1.17/template/template_openai.yaml
--rw-r--r--   0 j0hn       (501) staff       (20)       85 2023-05-14 14:25:01.000000 sipiiiii-1.1.17/template/template_other.yaml
--rw-r--r--   0 j0hn       (501) staff       (20)       89 2023-05-14 14:25:01.000000 sipiiiii-1.1.17/template/template_streamlit.yaml
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-14 14:30:01.816847 sipiiiii-1.2.0/
+-rw-r--r--   0 j0hn       (501) staff       (20)       18 2023-05-03 12:00:50.000000 sipiiiii-1.2.0/MANIFEST.in
+-rw-r--r--   0 j0hn       (501) staff       (20)     3788 2023-05-14 14:30:01.816282 sipiiiii-1.2.0/PKG-INFO
+-rw-r--r--   0 j0hn       (501) staff       (20)     3271 2023-05-11 16:47:37.000000 sipiiiii-1.2.0/README.md
+-rw-r--r--   0 j0hn       (501) staff       (20)      634 2023-05-14 14:29:18.000000 sipiiiii-1.2.0/pyproject.toml
+-rw-r--r--   0 j0hn       (501) staff       (20)       38 2023-05-14 14:30:01.816984 sipiiiii-1.2.0/setup.cfg
+-rw-r--r--   0 j0hn       (501) staff       (20)     3401 2023-05-14 14:29:18.000000 sipiiiii-1.2.0/setup.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-14 14:30:01.783860 sipiiiii-1.2.0/sipiiiii/
+-rw-r--r--   0 j0hn       (501) staff       (20)       22 2023-03-28 16:40:14.000000 sipiiiii-1.2.0/sipiiiii/__init__.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-14 14:30:01.794846 sipiiiii-1.2.0/sipiiiii/app/
+-rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-28 03:21:50.000000 sipiiiii-1.2.0/sipiiiii/app/__init__.py
+-rw-r--r--   0 j0hn       (501) staff       (20)    13002 2023-05-11 17:42:48.000000 sipiiiii-1.2.0/sipiiiii/app/core.py
+-rw-r--r--   0 j0hn       (501) staff       (20)    22242 2023-05-14 14:25:12.000000 sipiiiii-1.2.0/sipiiiii/app/new_app.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-14 14:30:01.804817 sipiiiii-1.2.0/sipiiiii/app/utils/
+-rw-r--r--   0 j0hn       (501) staff       (20)     7845 2023-05-03 09:19:05.000000 sipiiiii-1.2.0/sipiiiii/app/utils/HttpSDK.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     1712 2023-05-14 14:11:29.000000 sipiiiii-1.2.0/sipiiiii/app/utils/Tools.py
+-rw-r--r--   0 j0hn       (501) staff       (20)      735 2023-03-30 02:41:50.000000 sipiiiii-1.2.0/sipiiiii/app/utils/ZipFileTool.py
+-rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-30 02:41:28.000000 sipiiiii-1.2.0/sipiiiii/app/utils/__init__.py
+-rw-r--r--   0 j0hn       (501) staff       (20)      151 2023-05-04 12:35:33.000000 sipiiiii-1.2.0/sipiiiii/app/utils/config.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     1325 2023-01-05 06:18:13.000000 sipiiiii-1.2.0/sipiiiii/app/utils/formatConversion.py
+-rw-r--r--   0 j0hn       (501) staff       (20)       17 2023-05-14 14:29:18.000000 sipiiiii-1.2.0/sipiiiii/app/version.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     8341 2023-05-11 17:10:16.000000 sipiiiii-1.2.0/sipiiiii/main.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-14 14:30:01.789755 sipiiiii-1.2.0/sipiiiii.egg-info/
+-rw-r--r--   0 j0hn       (501) staff       (20)     3788 2023-05-14 14:30:01.000000 sipiiiii-1.2.0/sipiiiii.egg-info/PKG-INFO
+-rw-r--r--   0 j0hn       (501) staff       (20)      821 2023-05-14 14:30:01.000000 sipiiiii-1.2.0/sipiiiii.egg-info/SOURCES.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)        1 2023-05-14 14:30:01.000000 sipiiiii-1.2.0/sipiiiii.egg-info/dependency_links.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)       48 2023-05-14 14:30:01.000000 sipiiiii-1.2.0/sipiiiii.egg-info/entry_points.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)      104 2023-05-14 14:30:01.000000 sipiiiii-1.2.0/sipiiiii.egg-info/requires.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)        9 2023-05-14 14:30:01.000000 sipiiiii-1.2.0/sipiiiii.egg-info/top_level.txt
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-14 14:30:01.814658 sipiiiii-1.2.0/template/
+-rw-r--r--   0 j0hn       (501) staff       (20)      366 2023-04-18 15:46:14.000000 sipiiiii-1.2.0/template/python_fastapi.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)      371 2023-05-04 06:44:54.000000 sipiiiii-1.2.0/template/python_flask.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)     1505 2023-05-01 16:17:11.000000 sipiiiii-1.2.0/template/python_openai.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)      238 2023-05-04 06:44:09.000000 sipiiiii-1.2.0/template/python_streamlit.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)      762 2023-05-01 16:06:57.000000 sipiiiii-1.2.0/template/template_fastapi.yaml
+-rw-r--r--   0 j0hn       (501) staff       (20)      762 2023-05-04 06:17:59.000000 sipiiiii-1.2.0/template/template_flask.yaml
+-rw-r--r--   0 j0hn       (501) staff       (20)      795 2023-05-03 13:15:30.000000 sipiiiii-1.2.0/template/template_openai.yaml
+-rw-r--r--   0 j0hn       (501) staff       (20)       84 2023-05-14 14:29:18.000000 sipiiiii-1.2.0/template/template_other.yaml
+-rw-r--r--   0 j0hn       (501) staff       (20)       88 2023-05-14 14:29:18.000000 sipiiiii-1.2.0/template/template_streamlit.yaml
```

### Comparing `sipiiiii-1.1.17/PKG-INFO` & `sipiiiii-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipiiiii
-Version: 1.1.17
+Version: 1.2.0
 Summary: sipiiiii定位为简单易用的云应用托管平台
 Home-page: http://www.depl.run/
 Author: sipiiiii@admin
 Author-email: DeplRun <sipiiiii@example.com>
 Project-URL: Homepage, http://www.depl.run/
 Project-URL: Bug Tracker, http://www.depl.run/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sipiiiii-1.1.17/README.md` & `sipiiiii-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.1.17/pyproject.toml` & `sipiiiii-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sipiiiii"
-version = "1.1.17"
+version = "1.2.0"
 authors = [
   { name="DeplRun", email="sipiiiii@example.com" },
 ]
 description = "sipiiiii定位为简单易用的云应用托管平台"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `sipiiiii-1.1.17/setup.py` & `sipiiiii-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     print(msg)
     sys.exit(1)
 
 setuptools.setup(
     # 包的分发名称，使用字母、数字、_、-
     name="sipiiiii",
     # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
-    version="1.1.17",
+    version="1.2.0",
     # 作者名
     author="sipiiiii@admin",
     # 作者邮箱
     author_email="j0hn.wahahaha@gmail.com",
     # 包的简介描述
     description="depl sipiiiii, App Development Framework",
     # 包的详细介绍(一般通过加载README.md)
```

### Comparing `sipiiiii-1.1.17/sipiiiii/app/core.py` & `sipiiiii-1.2.0/sipiiiii/app/core.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.1.17/sipiiiii/app/new_app.py` & `sipiiiii-1.2.0/sipiiiii/app/new_app.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.1.17/sipiiiii/app/utils/HttpSDK.py` & `sipiiiii-1.2.0/sipiiiii/app/utils/HttpSDK.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.1.17/sipiiiii/app/utils/Tools.py` & `sipiiiii-1.2.0/sipiiiii/app/utils/Tools.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.1.17/sipiiiii/app/utils/ZipFileTool.py` & `sipiiiii-1.2.0/sipiiiii/app/utils/ZipFileTool.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.1.17/sipiiiii/app/utils/formatConversion.py` & `sipiiiii-1.2.0/sipiiiii/app/utils/formatConversion.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.1.17/sipiiiii/main.py` & `sipiiiii-1.2.0/sipiiiii/main.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.1.17/sipiiiii.egg-info/PKG-INFO` & `sipiiiii-1.2.0/sipiiiii.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipiiiii
-Version: 1.1.17
+Version: 1.2.0
 Summary: sipiiiii定位为简单易用的云应用托管平台
 Home-page: http://www.depl.run/
 Author: sipiiiii@admin
 Author-email: DeplRun <sipiiiii@example.com>
 Project-URL: Homepage, http://www.depl.run/
 Project-URL: Bug Tracker, http://www.depl.run/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sipiiiii-1.1.17/sipiiiii.egg-info/SOURCES.txt` & `sipiiiii-1.2.0/sipiiiii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.1.17/template/python_openai.j2` & `sipiiiii-1.2.0/template/python_openai.j2`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.1.17/template/template_fastapi.yaml` & `sipiiiii-1.2.0/template/template_fastapi.yaml`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.1.17/template/template_flask.yaml` & `sipiiiii-1.2.0/template/template_flask.yaml`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.1.17/template/template_openai.yaml` & `sipiiiii-1.2.0/template/template_openai.yaml`

 * *Files identical despite different names*

