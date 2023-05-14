# Comparing `tmp/sipiiiii-1.0.2.tar.gz` & `tmp/sipiiiii-1.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sipiiiii-1.0.2.tar", last modified: Fri May  5 16:46:19 2023, max compression
+gzip compressed data, was "sipiiiii-1.1.17.tar", last modified: Sun May 14 14:26:41 2023, max compression
```

## Comparing `sipiiiii-1.0.2.tar` & `sipiiiii-1.1.17.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 16:46:19.728312 sipiiiii-1.0.2/
--rw-r--r--   0 j0hn       (501) staff       (20)       18 2023-05-03 12:00:50.000000 sipiiiii-1.0.2/MANIFEST.in
--rw-r--r--   0 j0hn       (501) staff       (20)     3700 2023-05-05 16:46:19.727863 sipiiiii-1.0.2/PKG-INFO
--rw-r--r--   0 j0hn       (501) staff       (20)     3183 2023-05-05 10:00:41.000000 sipiiiii-1.0.2/README.md
--rw-r--r--   0 j0hn       (501) staff       (20)      634 2023-05-05 16:45:08.000000 sipiiiii-1.0.2/pyproject.toml
--rw-r--r--   0 j0hn       (501) staff       (20)       38 2023-05-05 16:46:19.728543 sipiiiii-1.0.2/setup.cfg
--rw-r--r--   0 j0hn       (501) staff       (20)     3401 2023-05-05 16:45:08.000000 sipiiiii-1.0.2/setup.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 16:46:19.691638 sipiiiii-1.0.2/sipiiiii/
--rw-r--r--   0 j0hn       (501) staff       (20)       22 2023-03-28 16:40:14.000000 sipiiiii-1.0.2/sipiiiii/__init__.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 16:46:19.714001 sipiiiii-1.0.2/sipiiiii/app/
--rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-28 03:21:50.000000 sipiiiii-1.0.2/sipiiiii/app/__init__.py
--rw-r--r--   0 j0hn       (501) staff       (20)    12474 2023-05-04 14:34:32.000000 sipiiiii-1.0.2/sipiiiii/app/core.py
--rw-r--r--   0 j0hn       (501) staff       (20)    21490 2023-05-05 16:45:08.000000 sipiiiii-1.0.2/sipiiiii/app/new_app.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 16:46:19.719809 sipiiiii-1.0.2/sipiiiii/app/utils/
--rw-r--r--   0 j0hn       (501) staff       (20)     7845 2023-05-03 09:19:05.000000 sipiiiii-1.0.2/sipiiiii/app/utils/HttpSDK.py
--rw-r--r--   0 j0hn       (501) staff       (20)     1565 2023-05-04 03:09:45.000000 sipiiiii-1.0.2/sipiiiii/app/utils/Tools.py
--rw-r--r--   0 j0hn       (501) staff       (20)      735 2023-03-30 02:41:50.000000 sipiiiii-1.0.2/sipiiiii/app/utils/ZipFileTool.py
--rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-30 02:41:28.000000 sipiiiii-1.0.2/sipiiiii/app/utils/__init__.py
--rw-r--r--   0 j0hn       (501) staff       (20)      151 2023-05-04 12:35:33.000000 sipiiiii-1.0.2/sipiiiii/app/utils/config.py
--rw-r--r--   0 j0hn       (501) staff       (20)     1325 2023-01-05 06:18:13.000000 sipiiiii-1.0.2/sipiiiii/app/utils/formatConversion.py
--rw-r--r--   0 j0hn       (501) staff       (20)       17 2023-05-05 16:45:08.000000 sipiiiii-1.0.2/sipiiiii/app/version.py
--rw-r--r--   0 j0hn       (501) staff       (20)     8056 2023-05-05 10:00:55.000000 sipiiiii-1.0.2/sipiiiii/main.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 16:46:19.707875 sipiiiii-1.0.2/sipiiiii.egg-info/
--rw-r--r--   0 j0hn       (501) staff       (20)     3700 2023-05-05 16:46:19.000000 sipiiiii-1.0.2/sipiiiii.egg-info/PKG-INFO
--rw-r--r--   0 j0hn       (501) staff       (20)      792 2023-05-05 16:46:19.000000 sipiiiii-1.0.2/sipiiiii.egg-info/SOURCES.txt
--rw-r--r--   0 j0hn       (501) staff       (20)        1 2023-05-05 16:46:19.000000 sipiiiii-1.0.2/sipiiiii.egg-info/dependency_links.txt
--rw-r--r--   0 j0hn       (501) staff       (20)       48 2023-05-05 16:46:19.000000 sipiiiii-1.0.2/sipiiiii.egg-info/entry_points.txt
--rw-r--r--   0 j0hn       (501) staff       (20)      104 2023-05-05 16:46:19.000000 sipiiiii-1.0.2/sipiiiii.egg-info/requires.txt
--rw-r--r--   0 j0hn       (501) staff       (20)        9 2023-05-05 16:46:19.000000 sipiiiii-1.0.2/sipiiiii.egg-info/top_level.txt
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 16:46:19.726994 sipiiiii-1.0.2/template/
--rw-r--r--   0 j0hn       (501) staff       (20)      366 2023-04-18 15:46:14.000000 sipiiiii-1.0.2/template/python_fastapi.j2
--rw-r--r--   0 j0hn       (501) staff       (20)      371 2023-05-04 06:44:54.000000 sipiiiii-1.0.2/template/python_flask.j2
--rw-r--r--   0 j0hn       (501) staff       (20)     1505 2023-05-01 16:17:11.000000 sipiiiii-1.0.2/template/python_openai.j2
--rw-r--r--   0 j0hn       (501) staff       (20)      238 2023-05-04 06:44:09.000000 sipiiiii-1.0.2/template/python_streamlit.j2
--rw-r--r--   0 j0hn       (501) staff       (20)      762 2023-05-01 16:06:57.000000 sipiiiii-1.0.2/template/template_fastapi.yaml
--rw-r--r--   0 j0hn       (501) staff       (20)      762 2023-05-04 06:17:59.000000 sipiiiii-1.0.2/template/template_flask.yaml
--rw-r--r--   0 j0hn       (501) staff       (20)      795 2023-05-03 13:15:30.000000 sipiiiii-1.0.2/template/template_openai.yaml
--rw-r--r--   0 j0hn       (501) staff       (20)       88 2023-05-05 16:45:08.000000 sipiiiii-1.0.2/template/template_streamlit.yaml
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-14 14:26:41.218494 sipiiiii-1.1.17/
+-rw-r--r--   0 j0hn       (501) staff       (20)       18 2023-05-03 12:00:50.000000 sipiiiii-1.1.17/MANIFEST.in
+-rw-r--r--   0 j0hn       (501) staff       (20)     3789 2023-05-14 14:26:41.217826 sipiiiii-1.1.17/PKG-INFO
+-rw-r--r--   0 j0hn       (501) staff       (20)     3271 2023-05-11 16:47:37.000000 sipiiiii-1.1.17/README.md
+-rw-r--r--   0 j0hn       (501) staff       (20)      635 2023-05-14 14:25:01.000000 sipiiiii-1.1.17/pyproject.toml
+-rw-r--r--   0 j0hn       (501) staff       (20)       38 2023-05-14 14:26:41.218751 sipiiiii-1.1.17/setup.cfg
+-rw-r--r--   0 j0hn       (501) staff       (20)     3402 2023-05-14 14:25:01.000000 sipiiiii-1.1.17/setup.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-14 14:26:41.192188 sipiiiii-1.1.17/sipiiiii/
+-rw-r--r--   0 j0hn       (501) staff       (20)       22 2023-03-28 16:40:14.000000 sipiiiii-1.1.17/sipiiiii/__init__.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-14 14:26:41.200971 sipiiiii-1.1.17/sipiiiii/app/
+-rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-28 03:21:50.000000 sipiiiii-1.1.17/sipiiiii/app/__init__.py
+-rw-r--r--   0 j0hn       (501) staff       (20)    13002 2023-05-11 17:42:48.000000 sipiiiii-1.1.17/sipiiiii/app/core.py
+-rw-r--r--   0 j0hn       (501) staff       (20)    22242 2023-05-14 14:25:12.000000 sipiiiii-1.1.17/sipiiiii/app/new_app.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-14 14:26:41.206311 sipiiiii-1.1.17/sipiiiii/app/utils/
+-rw-r--r--   0 j0hn       (501) staff       (20)     7845 2023-05-03 09:19:05.000000 sipiiiii-1.1.17/sipiiiii/app/utils/HttpSDK.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     1712 2023-05-14 14:11:29.000000 sipiiiii-1.1.17/sipiiiii/app/utils/Tools.py
+-rw-r--r--   0 j0hn       (501) staff       (20)      735 2023-03-30 02:41:50.000000 sipiiiii-1.1.17/sipiiiii/app/utils/ZipFileTool.py
+-rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-30 02:41:28.000000 sipiiiii-1.1.17/sipiiiii/app/utils/__init__.py
+-rw-r--r--   0 j0hn       (501) staff       (20)      151 2023-05-04 12:35:33.000000 sipiiiii-1.1.17/sipiiiii/app/utils/config.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     1325 2023-01-05 06:18:13.000000 sipiiiii-1.1.17/sipiiiii/app/utils/formatConversion.py
+-rw-r--r--   0 j0hn       (501) staff       (20)       18 2023-05-14 14:25:01.000000 sipiiiii-1.1.17/sipiiiii/app/version.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     8341 2023-05-11 17:10:16.000000 sipiiiii-1.1.17/sipiiiii/main.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-14 14:26:41.197155 sipiiiii-1.1.17/sipiiiii.egg-info/
+-rw-r--r--   0 j0hn       (501) staff       (20)     3789 2023-05-14 14:26:40.000000 sipiiiii-1.1.17/sipiiiii.egg-info/PKG-INFO
+-rw-r--r--   0 j0hn       (501) staff       (20)      821 2023-05-14 14:26:41.000000 sipiiiii-1.1.17/sipiiiii.egg-info/SOURCES.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)        1 2023-05-14 14:26:41.000000 sipiiiii-1.1.17/sipiiiii.egg-info/dependency_links.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)       48 2023-05-14 14:26:41.000000 sipiiiii-1.1.17/sipiiiii.egg-info/entry_points.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)      104 2023-05-14 14:26:41.000000 sipiiiii-1.1.17/sipiiiii.egg-info/requires.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)        9 2023-05-14 14:26:41.000000 sipiiiii-1.1.17/sipiiiii.egg-info/top_level.txt
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-14 14:26:41.216943 sipiiiii-1.1.17/template/
+-rw-r--r--   0 j0hn       (501) staff       (20)      366 2023-04-18 15:46:14.000000 sipiiiii-1.1.17/template/python_fastapi.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)      371 2023-05-04 06:44:54.000000 sipiiiii-1.1.17/template/python_flask.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)     1505 2023-05-01 16:17:11.000000 sipiiiii-1.1.17/template/python_openai.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)      238 2023-05-04 06:44:09.000000 sipiiiii-1.1.17/template/python_streamlit.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)      762 2023-05-01 16:06:57.000000 sipiiiii-1.1.17/template/template_fastapi.yaml
+-rw-r--r--   0 j0hn       (501) staff       (20)      762 2023-05-04 06:17:59.000000 sipiiiii-1.1.17/template/template_flask.yaml
+-rw-r--r--   0 j0hn       (501) staff       (20)      795 2023-05-03 13:15:30.000000 sipiiiii-1.1.17/template/template_openai.yaml
+-rw-r--r--   0 j0hn       (501) staff       (20)       85 2023-05-14 14:25:01.000000 sipiiiii-1.1.17/template/template_other.yaml
+-rw-r--r--   0 j0hn       (501) staff       (20)       89 2023-05-14 14:25:01.000000 sipiiiii-1.1.17/template/template_streamlit.yaml
```

### Comparing `sipiiiii-1.0.2/PKG-INFO` & `sipiiiii-1.1.17/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: sipiiiii
-Version: 1.0.2
-Summary: sipiiiii定位为简单易用的云应用托管平台
-Home-page: http://www.depl.run/
-Author: sipiiiii@admin
-Author-email: DeplRun <sipiiiii@example.com>
-Project-URL: Homepage, http://www.depl.run/
-Project-URL: Bug Tracker, http://www.depl.run/
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
 sipiiiii是一款面向小微企业和个人开发者的应用托管平台。其主要目的是满足chatgpt插件系统的托管需求。
 ## 产品定位
 sipiiiii定位为简单易用的云应用托管平台:
 - 小微企业:可以便捷部署业务应用,降低 IT 成本
 - 个人开发者:可以快速部署个人开发的应用,实现想法
 - chatgpt插件开发者:专为chatgpt插件系统提供托管服务,降低开发难度
 ## 产品优势
@@ -61,45 +46,51 @@
 ### 运行应用(非部署)
 在应用目录下直接运行:
  
 sipiiiii -d 或 --dev
 ### 本地化部署应用
 消耗5积分,同一个应用只扣一次:
 
-sipiiiii -LD <app name> 或 --localdepl <app name>
-sipiiiii -LD <test.yaml> 或 --localdepl <test.yaml>
+sipiiiii -LD 或 --localdepl
+根据当前目录名获取应用名
+
 ### 部署应用
 消耗20积分,同一个应用只扣一次:
 
 sipiiiii -D 或 --deployed 
+根据当前目录名获取应用名
+
 ## 应用生成
 根据 yaml 模版和选项创建一个应用框架,目前有三种方式创建应用
 1. 根据自己提供的yaml文件创建应用
 2. 使用aiapi的模版创建应用
 3. 使用向导模式创建应用
  
 sipiiiii -n <test.yaml> 或 --new <test.yaml>
+如果没有 <test.yaml> 参数则根据模板或者向导创建应用
+
 ## 应用管理
 ### 列出应用列表
 
 sipiiiii -l 或 --list
 ### 查看应用详情
 
 sipiiiii -i <app name> 或 --info <app name> 
-sipiiiii -i <test.yaml> 或 --info <test.yaml>
+如果没有 <app name> 参数则根据当前目录名获取应用名
+
 ### 停止应用(非本地部署)
 
 sipiiiii -s <app name> 或 --stop <app name>
-sipiiiii -s <test.yaml> 或 --stop <test.yaml> 
+如果没有 <app name> 参数则根据当前目录名获取应用名
+
 ### 重启应用(非本地部署)
 
 sipiiiii -r <app name> 或 --restart <app name>  
-sipiiiii -r <test.yaml> 或 --restart <test.yaml>
- 
+如果没有 <app name> 参数则根据当前目录名获取应用名
+
 ## 示例
 
-sipiiiii -n test.yaml  
-sipiiiii -LD test.yaml
-sipiiiii -LD your-app-name
+sipiiiii -L
+sipiiiii -n 
 sipiiiii -D
-sipiiiii -L  
-sipiiiii -i your-app-name
+sipiiiii -l
+sipiiiii -i your-app-name
```

### Comparing `sipiiiii-1.0.2/pyproject.toml` & `sipiiiii-1.1.17/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sipiiiii"
-version = "1.0.2"
+version = "1.1.17"
 authors = [
   { name="DeplRun", email="sipiiiii@example.com" },
 ]
 description = "sipiiiii定位为简单易用的云应用托管平台"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `sipiiiii-1.0.2/setup.py` & `sipiiiii-1.1.17/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     print(msg)
     sys.exit(1)
 
 setuptools.setup(
     # 包的分发名称，使用字母、数字、_、-
     name="sipiiiii",
     # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
-    version="1.0.2",
+    version="1.1.17",
     # 作者名
     author="sipiiiii@admin",
     # 作者邮箱
     author_email="j0hn.wahahaha@gmail.com",
     # 包的简介描述
     description="depl sipiiiii, App Development Framework",
     # 包的详细介绍(一般通过加载README.md)
```

### Comparing `sipiiiii-1.0.2/sipiiiii/app/core.py` & `sipiiiii-1.1.17/sipiiiii/app/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import json
 import sys
 
 from shutil import rmtree
 from pathlib import Path
 from jinja2 import Environment, FileSystemLoader
 from .utils.config import fix
-from .utils.Tools import get_current_path, read_app_yaml
+from .utils.Tools import get_current_path, read_app_yaml, is_encomm_char
 
 
 class ExecAppClass(object):
-    def __init__(self,file_path):
+    def __init__(self, file_path):
         self.file_path = file_path
 
     def run_python_app(self):
         cmd_line = input("请输出python解析器[python,python3或pypy](默认python):")
         if cmd_line is None or cmd_line == "":
             cmd_line = "python"
         # sys.path.append(self.cwd)
@@ -80,26 +80,58 @@
             requirements.append('flask')
         if app_type == "openai":
             requirements.append('quart')
             requirements.append('quart_cors')
         if app_type == "streamlit":
             requirements.append('streamlit')
 
-        status, requirements_file_path = create_requirements(
-            self.app_name, requirements)
+        status, requirements_file_path = create_requirements(requirements)
         if not status:
             return False, requirements_file_path
 
+    def creaye_other_file(self, code_type):
+        if code_type == "python":
+            requirements_file = os.path.join(os.getcwd(), "requirements.txt")
+            if not os.path.exists(requirements_file):
+                self.__create_python_requirements("other")
+
+        self.app_yaml = ""
+        for path in os.listdir(os.getcwd()):
+            if os.path.isfile(path):
+                if path.find(".yaml") > -1:
+                    openapi_file_path = os.path.join(os.getcwd(), path)
+                    with open(openapi_file_path, "r", encoding="utf-8") as f:
+                        openapi_yaml = f.read()
+                    self.app_yaml = yaml.safe_load(openapi_yaml)
+                    break
+
+        if self.app_yaml == "":
+            status, _, self.app_yaml, _ = yaml_app_info(None, "other")
+            status, openapi_file_path = create_app_yaml(self.app_yaml)
+            if not status:
+                return False, openapi_file_path
+        try:
+            _ = self.app_yaml['info']['title']
+        except Exception as e:
+            return False, f"yaml 解析错误: {str(e)}"
+
+        self.app_yaml['info']['title'] = self.app_name
+        self.app_yaml['info']['description'] = self.app_name
+
+        with open(openapi_file_path, "w", encoding="utf-8") as f:
+            yaml.dump(self.app_yaml, stream=f, allow_unicode=True)
+
+        return True, ""
+
     def create_streamlit_app(self, code_type):
         self.__create_app_path()
         if code_type == "python":
             self.__create_python_requirements("streamlit")
 
-        status, openapi_file_path = create_app_yaml(
-            self.app_name, self.app_yaml, "streamlit")
+        status, openapi_file_path = create_app_yaml(self.app_yaml)
         if not status:
             return False, openapi_file_path
 
         code = f"""
 import streamlit as st
 
 def main():
@@ -125,16 +157,15 @@
 
     def create_flask_app(self, code_type):
         self.__create_app_path()
 
         if code_type == "python":
             self.__create_python_requirements("flask")
 
-        status, openapi_file_path = create_app_yaml(
-            self.app_name, self.app_yaml, "flask")
+        status, openapi_file_path = create_app_yaml(self.app_yaml)
         if not status:
             return False, openapi_file_path
 
         ststus, msg = self.__create_code(code_type, "flask")
         if not ststus:
             return False, msg
 
@@ -142,16 +173,15 @@
 
     def create_fastapi_app(self, code_type):
         self.__create_app_path()
 
         if code_type == "python":
             self.__create_python_requirements("fastapi")
 
-        status, openapi_file_path = create_app_yaml(
-            self.app_name, self.app_yaml, "fastapi")
+        status, openapi_file_path = create_app_yaml(self.app_yaml)
         if not status:
             return False, openapi_file_path
 
         ststus, msg = self.__create_code(code_type, "fastapi")
         if not ststus:
             return False, msg
 
@@ -192,16 +222,15 @@
             return False, str(e)
 
         self.__create_app_path()
 
         if code_type == "python":
             self.__create_python_requirements("openai")
 
-        status, openapi_file_path = create_app_yaml(
-            self.app_name, self.app_yaml, "openai")
+        status, openapi_file_path = create_app_yaml(self.app_yaml)
         if not status:
             return False, openapi_file_path
 
         status, plugin_json_file_path = create_app_config(
             self.app_name, ai_plugin_json, "openai")
         if not status:
             return False, plugin_json_file_path
@@ -209,43 +238,22 @@
         ststus, msg = self.__create_code(code_type, "openai")
         if not ststus:
             return False, msg
 
         return True, f"创建openai框架代码成功, 项目目录: ./{self.app_name}"
 
 
-def get_app_name(app_name, is_yaml=False):
+def get_app_name(app_name):
     if app_name is None:
-        while True:
-            app_yaml_file = ""
-            try:
-                app_yaml_file = input("请输入APP yaml文件:")
-            except KeyboardInterrupt:
-                print("\r\n")
-                sys.exit(1)
-
-            if app_yaml_file == "":
-                continue
-            status, app_name, openapi_yaml, aiapi_dir = yaml_app_info(
-                app_yaml_file, None)
-            if not status:
-                return False, app_name, openapi_yaml, aiapi_dir
+        app_name = os.getcwd().lower()
+        app_name = os.path.basename(app_name)
+    if not is_encomm_char(app_name):
+        return False, "应用名(当前目录)只能是纯英文"
 
-            return True, app_name, openapi_yaml, aiapi_dir
-
-    elif app_name.find(".yaml") > -1:
-        status, app_name, openapi_yaml, aiapi_dir = yaml_app_info(
-            app_name, None)
-        if not status:
-            return False, app_name, openapi_yaml, aiapi_dir
-        return True, app_name, openapi_yaml, aiapi_dir
-    else:
-        if is_yaml:
-            return False, app_name, "", ""
-        return True, app_name, "", ""
+    return True, app_name
 
 
 def get_app_code_type(file_path):
     _fix = ""
     try:
         _fix = os.path.splitext(file_path)[-1].split(".")[-1]
     except Exception as e:
@@ -278,27 +286,28 @@
     if app_name == "":
         return False, "yaml中没有找到 yaml[info][title]", None, None
 
     app_name = app_name.replace(" ", "")
     return True, app_name, openapi_yaml, aiapi_dir
 
 
-def create_requirements(directory_path, requirements):
+def create_requirements(requirements):
     if type(requirements) != list:
         return False, "requirements 错误!"
 
+    directory_path = os.getcwd()
     if not os.path.exists(directory_path):
         return False, f"{directory_path} 没有找到."
 
     requirements_file_path = os.path.join(directory_path, "requirements.txt")
     requirements_data = ""
     if len(requirements) > 0:
         requirements_data = "\n".join(requirements)
 
-    with open(requirements_file_path, "w") as f:
+    with open(requirements_file_path, "w", encoding="utf8") as f:
         f.write(requirements_data)
 
     return True, requirements_file_path
 
 
 def create_app_config(directory_path, plugin_json, app_type):
     if type(plugin_json) != dict:
@@ -317,15 +326,16 @@
     # plugin_json_data = "\n".join(plugin_json_file_path)
     with open(plugin_json_file_path, encoding="utf-8", mode="w") as f:
         json.dump(plugin_json, f, indent=2)
 
     return True, plugin_json_file_path
 
 
-def create_app_yaml(directory_path, openapi_yaml, app_type):
+def create_app_yaml(openapi_yaml):
+    directory_path = os.getcwd()
     if not os.path.exists(directory_path):
         return False, f"{directory_path} 目录不存在"
 
     # openapi_yaml_file_path = os.path.join(directory_path, f"{app_type}.yaml")
     # if app_type is None:
     openapi_yaml_file_path = os.path.join(directory_path, "aiapi.yaml")
     # openapi.yaml
```

### Comparing `sipiiiii-1.0.2/sipiiiii/app/new_app.py` & `sipiiiii-1.1.17/sipiiiii/app/new_app.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,21 +8,25 @@
 from requests_toolbelt.multipart.encoder import MultipartEncoder
 from pathlib import Path
 
 from .core import CreateAppTypeClass, yaml_app_info, ExecAppClass, get_app_code_type, get_app_name
 
 from .utils.ZipFileTool import zip_folder
 from .utils.HttpSDK import https_get, https_post, https_file
-from .utils.Tools import get_outside_ip, is_encomm_char, write_new_yaml
+from .utils.Tools import get_outside_ip, is_encomm_char, write_new_yaml, move_file
 from .utils.config import app_all_types, server_host, fix
 
 
 def process_update_outside_ip(domain, _token):
     while True:
-        time.sleep(60 * 30)
+        try:
+            time.sleep(60 * 30)
+        except KeyboardInterrupt:
+            break
+
         outside_ip = get_outside_ip()
         headers = {
             "Content-type": "application/json",
             "authorization": _token
         }
         url = f"{server_host}/system/openapi/modify/domain/bind/ip"
         data = {
@@ -84,38 +88,43 @@
             with open(f"{os.getcwd()}{os.sep}aiapi.yaml", "w", encoding="utf-8") as f:
                 f.write(yaml_data)
 
             status, msg, app_name, app_type = create_app(
                 f"{os.getcwd()}{os.sep}aiapi.yaml")
             if status:
                 write_new_yaml(
-                    f"{os.getcwd()}{os.sep}{app_name}{os.sep}aiapi.yaml", app_type)
+                    f"{os.getcwd()}{os.sep}aiapi.yaml", app_type)
 
-            os.remove(f"{os.getcwd()}{os.sep}aiapi.yaml")
+            # os.remove(f"{os.getcwd()}{os.sep}aiapi.yaml")
             break
 
         elif is_wizard_create == "n":
             status, msg, app_name, _ = create_app(None)
             break
         else:
             continue
 
+    move_file(f"{os.getcwd()}{os.sep}requirements.txt",
+              f"{os.getcwd()}{os.sep}{app_name}{os.sep}requirements.txt")
+
+    move_file(f"{os.getcwd()}{os.sep}aiapi.yaml",
+              f"{os.getcwd()}{os.sep}{app_name}{os.sep}aiapi.yaml")
     return status, msg, app_name
 
 
 # 创建yaml模版
 def create_yaml(app_name, app_version, app_desc):
     status, _token = get_token()
     if not status:
         return False, _token
 
     while True:
-        route_num = input("请输入有多少个接口(默认1个接口):")
+        route_num = input("请输入有多少个接口(默认无接口):")
         if route_num == "":
-            route_num = 1
+            route_num = 0
 
         try:
             route_num = int(route_num)
             break
         except Exception as _:
             print("接口数量必须为数字")
 
@@ -227,35 +236,30 @@
 
     method_of_catc = getattr(eac, f"run_{code_type}_app")
     status, msg = method_of_catc()
 
     return status, msg
 
 
-def localdepl(yaml_file_name):
+def localdepl(app_name):
     status, _token = get_token()
     if not status:
         return False, _token
 
-    status, app_name, app_yaml, _ = get_app_name(yaml_file_name, True)
+    status, app_name = get_app_name(app_name)
     if not status:
         return False, f"获取应用名错误: {app_name}"
 
     app_cn_name = input("请输入应用别名:")
     if app_cn_name == "":
         app_cn_name = app_name
 
-    print(f"本地部署: {app_name} 项目\r\n")
+    # description = input("请输入应用说明:")
 
-    description = ""
-    try:
-        description = app_yaml.get(
-            'info', {}).get('description', "")
-    except Exception as e:
-        return False, str(e)
+    print(f"本地部署: {app_name} 项目\r\n")
 
     outside_ip = get_outside_ip()
     if outside_ip == "":
         return False, "无法访问互联网"
 
     print(f"本机外网IP: {outside_ip}")
     status, _token = get_token()
@@ -288,25 +292,27 @@
         "authorization": _token
     }
     data = {
         "app_name": app_name,
         "app_dock": "app",
         "app_cn_name": app_cn_name,
         "ip": outside_ip,
-        "description": description,
+        "description": f"本地部署的{app_name}",
         "app_language": app_language
     }
 
     response = https_post(url, json_data=data, headers=headers)
     if response.code != 200:
         return False, "内部服务器错误，请稍后再试"
 
     if not response.success:
         return False, response.msg
 
+    print(f"域名: {response.data['domain']}")
+    time.sleep(3)
     p = multiprocessing.Process(
         target=process_update_outside_ip, args=(response.data['domain'], _token), daemon=True)
     p.start()
 
     status, code_type = get_app_code_type(file_path)
     if not status:
         return False, code_type
@@ -320,15 +326,15 @@
 
 
 def stop_app(app_name=None):
     status, _token = get_token()
     if not status:
         return False, _token
 
-    status, app_name, _, _ = get_app_name(app_name)
+    status, app_name = get_app_name(app_name)
     if not status:
         return False, f"获取应用名错误: {app_name}"
 
     data = {"app_name": app_name}
 
     headers = {
         "Content-type": "application/json",
@@ -344,15 +350,16 @@
 
 def deployed():
     status, _token = get_token()
     if not status:
         return False, _token
     print("""
     *** 必须在项目目录下进行操作
-    *** 暴露的端口必须为8000
+    *** 如果是对外服务暴露的端口必须为8000
+    *** 之前部署过的项目再部署则是更新, 域名不会改变
     """)
     headers = {
         "Content-type": "application/json",
         "authorization": _token
     }
 
     url = f"{server_host}/system/openapi/users/check/token"
@@ -361,14 +368,18 @@
 
     if not response.success:
         return False, "用户令牌无效，请登录使用 sipiiiiii -L 登录."
 
     if not response.data["exist"]:
         return False, "用户令牌无效或超时，请登录使用 sipiiiiii -L 登录."
 
+    status, app_name = get_app_name(None)
+    if not status:
+        return False, f"获取应用名错误: {app_name}"
+
     app_cn_name = input("请输入APP别名:")
     # input("please input APP docking party(chatgpt, other):")
     app_dock = "other"
     run_main = input("请输入APP运行文件:")
 
     if app_cn_name == "" or run_main == "":
         return False, "APP别名 或者 APP运行文件的不能为空."
@@ -387,29 +398,33 @@
         return False, "错误: 不存在项目路径, 请到项目路径下运行, 或者使用sipiiiii -n 创建项目"
 
     if run_main_fix[-1] not in list(fix.values()):
         return False, f"APP运行文件不在允许的列表范围内: {list(fix.keys())}"
 
     app_language = [k for k, v in fix.items() if v == run_main_fix[-1]][0]
 
+    catc = CreateAppTypeClass(app_name, "", "")
+    status, msg = catc.creaye_other_file(app_language)
+
+    if not status:
+        return False, msg
+
     zip_file_path = zip_folder(cwd)
     if zip_file_path is None:
         return False, "应用程序打包失败。请检查应用程序目录中是否存在异常文件或文件夹"
 
+    print(f"远程部署: {app_name} 项目\r\n")
     filename = os.path.basename(cwd)
-    print(f"远程部署: {filename} 项目\r\n")
-    # filename = ""#os.path.basename(zip_file_path)
     files = MultipartEncoder(fields={
-        'file': (f"{filename}.zip", open(zip_file_path, 'rb'), 'application/octet-stream'),
+        'file': (f"{app_name}.zip", open(zip_file_path, 'rb'), 'application/octet-stream'),
     })
 
     url = f"{server_host}/system/openapi/app/upload"
     response = https_file(url, files=files, headers=headers)
-    # response = requests.post(url, data=files, headers=headers, timeout=300)
-    # print(response)
+
     if response['code'] != 200:
         return False, "内部服务器错误，请稍后再试"
 
     if not response['success']:
         return False, response['msg']
 
     url = f"{server_host}/system/openapi/app/deployment"
@@ -438,16 +453,16 @@
     # if not status:
     #     return False, "部署成功，状态获取失败"
 
     # bar = ProgPercent(50, monitor=True)
     print("正在远程部署...\r\n")
     i = 0
     while True:
-        if i >= 60 * 5:
-            return False, "\r\n获取状态超时, 请用 sipiiiii -l查看应用列表"
+        if i >= 60 * 1:
+            break
         i += 1
         time.sleep(1)
         status, info_json, _ = get_app_info(filename.lower())
         if not status:
             continue
 
         if info_json['ServerStatus'] == "close" or info_json['ServerStatus'] == "exited":
@@ -455,14 +470,15 @@
             return True, f"\r\n应用程序部署出错，日志: \r\n{info_json['Log']}"
 
         if info_json['ServerStatus'] == "created" or info_json['ServerStatus'] == "running":
             # bar.update(50)
             return True, f"\r\n部署成功, \r\n域名: {info_json['Domain']}"
 
     # return True, response.data
+    return False, "\r\n应用部署失败, 请检查应用是否可正常运行或者检查包是否正确"
 
 
 def login(email, password):
     url = f"{server_host}/system/openapi/users/login"
     headers = {
         "Content-type": "application/json"
     }
@@ -518,15 +534,15 @@
         return False, _token
 
     url = f"{server_host}/system/openapi/app/restart"
     headers = {
         "Content-type": "application/json",
         "authorization": _token
     }
-    status, app_name, _, _ = get_app_name(app_name)
+    status, app_name = get_app_name(app_name)
     if not status:
         return False, f"获取应用名错误: {app_name}"
 
     response = https_post(
         url, json_data={"app_name": app_name}, headers=headers)
     if response.code != 200:
         return False, "服务器内部错误, 请稍后再试"
@@ -543,15 +559,15 @@
         return False, {}, _token
 
     url = f"{server_host}/system/openapi/app/status"
     headers = {
         "Content-type": "application/json",
         "authorization": _token
     }
-    status, app_name, _, _ = get_app_name(app_name)
+    status, app_name = get_app_name(app_name)
     if not status:
         return False, {}, f"获取应用名错误: {app_name}"
     app_name = app_name.lower()
     data = {"app_name": app_name}
 
     response = https_post(url, json_data=data, headers=headers)
     if response.code != 200:
@@ -599,15 +615,23 @@
         table.add_row((app['AppName'], app['AppCnName'], app['Domain'],
                       app['ServerStatus'], app['CreateTime']))
 
     return True, table
 
 
 def get_cli_server_version():
-    return "1.0.2"
+    headers = {
+        "Content-type": "application/json",
+    }
+    url = f"{server_host}/system/openapi/users/get/client"
+    response = https_get(url, headers=headers)
+    if response.code != 200:
+        return False, "服务器内部错误, 请稍后再试"
+
+    return response.msg
 
 
 def update_template():
     pass
 
 
 def activate_account():
```

### Comparing `sipiiiii-1.0.2/sipiiiii/app/utils/HttpSDK.py` & `sipiiiii-1.1.17/sipiiiii/app/utils/HttpSDK.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.0.2/sipiiiii/app/utils/Tools.py` & `sipiiiii-1.1.17/sipiiiii/app/utils/Tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import requests
 import yaml
 import os
+import shutil
 from pathlib import Path
 
 
 def get_outside_ip():
     ip = ""
     try:
         ip = requests.get("http://ifconfig.me/ip", timeout=5).text.strip()
@@ -52,7 +53,15 @@
     with open(yaml_file, "r", encoding="utf-8") as f:
         openapi_yaml = f.read()
     openapi_yaml = yaml.safe_load(openapi_yaml)
     openapi_yaml['openapi'] = "3.0.1"
     del openapi_yaml['swagger']
     with open(f"{os.getcwd()}{os.sep}aiapi.yaml", "w", encoding="utf") as f:
         yaml.dump(openapi_yaml, stream=f, allow_unicode=True)
+
+
+def move_file(src_file, dst_file):
+    try:
+        shutil.move(src_file, dst_file)
+    except FileNotFoundError:
+        pass
+
```

### Comparing `sipiiiii-1.0.2/sipiiiii/app/utils/ZipFileTool.py` & `sipiiiii-1.1.17/sipiiiii/app/utils/ZipFileTool.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.0.2/sipiiiii/app/utils/formatConversion.py` & `sipiiiii-1.1.17/sipiiiii/app/utils/formatConversion.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.0.2/sipiiiii/main.py` & `sipiiiii-1.1.17/sipiiiii/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import argparse
 import getpass
 import sys
 from .app.version import version
 from .app.new_app import *
 
+last_version = get_cli_server_version()
+
 
 def echo_help():
     # 显示一个帮助信息
     _log = f'''
   _____ _____ _____ _____ _____ _____ _____ _____ 
  / ____|_   _|  __ \_   _|_   _|_   _|_   _|_   _|
 | (___   | | | |__) || |   | |   | |   | |   | |  
  \___ \  | | |  ___/ | |   | |   | |   | |   | |  
  ____) |_| |_| |    _| |_ _| |_ _| |_ _| |_ _| |_ 
 |_____/|_____|_|   |_____|_____|_____|_____|_____|
 
 /* 专业应用托管服务平台 */
 
-本地客户端版本: {version}, 最新客户端版本: {get_cli_server_version()}:
+本地客户端版本: {version}, 最新客户端版本: {last_version}:
 
 用法: sipiiiii [选项]
 
   显示帮助信息:
     sipiiiii -h 或 --help
 
   账号管理:
@@ -39,47 +41,49 @@
 
   应用部署:
     运行应用(非部署)，在应用目录下直接运行:
       sipiiiii -d 或 --dev
 
     本地化部署应用，不需要上传代码到我们的部署服务器，在本地部署一个应用，并且我们提供一个二级域名解析到你的外网IP
     每部署一个本地应用将消耗5积分, 一个应用名只扣除一次积分:
-      sipiiiii -LD <app name> 或 --localdepl <app name>
-      sipiiiii -LD <test.yaml> 或 --localdepl <test.yaml>
+      sipiiiii -LD 或 --localdepl
+      根据当前目录名获取应用名
 
     部署你的应用，将在我们的部署服务器中运行，并且我们提供一个二级域名解析
     每部署一个远程应用将消耗20积分, 一个应用名只扣除一次积分:
       sipiiiii -D 或 --deployed
+      根据当前目录名获取应用名
 
   应用生成:
     根据 yaml 模版和选项创建一个应用框架
     有三种方式创建应用
     1) 根据自己提供的yaml文件创建应用
     2) 使用aiapi的模版创建应用
     3) 使用向导模式创建应用
       sipiiiii -n <test.yaml> 或 --new <test.yaml>
+      如果没有 <test.yaml> 参数则根据模板或者向导创建应用
 
   应用管理:
     列出你的应用列表:
       sipiiiii -l 或 --list
 
     查看你的应用详情:
       sipiiiii -i <app name> 或 --info <app name>
-      sipiiiii -i <test.yaml> 或 --info <test.yaml>
+      如果没有 <app name> 参数则根据当前目录名获取应用名
 
     停止你正在运行的应用(非本地部署):
       sipiiiii -s <app name> 或 --stop <app name>
-      sipiiiii -s <test.yaml> 或 --stop <test.yaml>
+      如果没有 <app name> 参数则根据当前目录名获取应用名
 
     重启你的应用(非本地部署):
       sipiiiii -r <app name> 或 --restart <app name>
-      sipiiiii -r <test.yaml> 或 --restart <test.yaml>
+      如果没有 <app name> 参数则根据当前目录名获取应用名
       
   示例:
-    使用注册邮箱和密码进行登录
+    使用注册的邮箱和密码进行登录
     sipiiiii -L 
     创建一个新的应用, 创建后编写相关的业务代码
     sipiiiii -n 
     进入到应用目录后, 进行部署
     sipiiiii -D
     查看应用详情信息 
     sipiiiii -i 应用名
@@ -116,16 +120,17 @@
                         required=False, nargs='?', const='default_value')
     parser.add_argument('-LD', '--localdepl', help='本地部署应用',
                         required=False, nargs='?', const='default_value')
     args = vars(parser.parse_args())
 
     if args is None:
         print(echo_help())
-        if version != get_cli_server_version():
-            print("pip install sipiiiii")
+        if version != last_version:
+            print(
+                f"最新版本,{last_version}, 请使用: pip install sipiiiii -U 更新")
         sys.exit(1)
 
     if args['deployed']:
         # execute deployed code here
         _, msg = deployed()
         print(msg)
 
@@ -228,13 +233,14 @@
 
         print(msg)
 
     elif args['help']:
         print(echo_help())
     else:
         print(echo_help())
-        if version != get_cli_server_version():
-            print("\r\npip install sipiiiii -U")
+        if version != last_version:
+            print(
+                f"最新版本,{last_version}, 请使用: pip install sipiiiii -U 更新")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `sipiiiii-1.0.2/sipiiiii.egg-info/PKG-INFO` & `sipiiiii-1.1.17/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipiiiii
-Version: 1.0.2
+Version: 1.1.17
 Summary: sipiiiii定位为简单易用的云应用托管平台
 Home-page: http://www.depl.run/
 Author: sipiiiii@admin
 Author-email: DeplRun <sipiiiii@example.com>
 Project-URL: Homepage, http://www.depl.run/
 Project-URL: Bug Tracker, http://www.depl.run/
 Classifier: Programming Language :: Python :: 3
@@ -61,45 +61,51 @@
 ### 运行应用(非部署)
 在应用目录下直接运行:
  
 sipiiiii -d 或 --dev
 ### 本地化部署应用
 消耗5积分,同一个应用只扣一次:
 
-sipiiiii -LD <app name> 或 --localdepl <app name>
-sipiiiii -LD <test.yaml> 或 --localdepl <test.yaml>
+sipiiiii -LD 或 --localdepl
+根据当前目录名获取应用名
+
 ### 部署应用
 消耗20积分,同一个应用只扣一次:
 
 sipiiiii -D 或 --deployed 
+根据当前目录名获取应用名
+
 ## 应用生成
 根据 yaml 模版和选项创建一个应用框架,目前有三种方式创建应用
 1. 根据自己提供的yaml文件创建应用
 2. 使用aiapi的模版创建应用
 3. 使用向导模式创建应用
  
 sipiiiii -n <test.yaml> 或 --new <test.yaml>
+如果没有 <test.yaml> 参数则根据模板或者向导创建应用
+
 ## 应用管理
 ### 列出应用列表
 
 sipiiiii -l 或 --list
 ### 查看应用详情
 
 sipiiiii -i <app name> 或 --info <app name> 
-sipiiiii -i <test.yaml> 或 --info <test.yaml>
+如果没有 <app name> 参数则根据当前目录名获取应用名
+
 ### 停止应用(非本地部署)
 
 sipiiiii -s <app name> 或 --stop <app name>
-sipiiiii -s <test.yaml> 或 --stop <test.yaml> 
+如果没有 <app name> 参数则根据当前目录名获取应用名
+
 ### 重启应用(非本地部署)
 
 sipiiiii -r <app name> 或 --restart <app name>  
-sipiiiii -r <test.yaml> 或 --restart <test.yaml>
- 
+如果没有 <app name> 参数则根据当前目录名获取应用名
+
 ## 示例
 
-sipiiiii -n test.yaml  
-sipiiiii -LD test.yaml
-sipiiiii -LD your-app-name
+sipiiiii -L
+sipiiiii -n 
 sipiiiii -D
-sipiiiii -L  
+sipiiiii -l
 sipiiiii -i your-app-name
```

### Comparing `sipiiiii-1.0.2/sipiiiii.egg-info/SOURCES.txt` & `sipiiiii-1.1.17/sipiiiii.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 template/python_fastapi.j2
 template/python_flask.j2
 template/python_openai.j2
 template/python_streamlit.j2
 template/template_fastapi.yaml
 template/template_flask.yaml
 template/template_openai.yaml
+template/template_other.yaml
 template/template_streamlit.yaml
```

### Comparing `sipiiiii-1.0.2/template/python_openai.j2` & `sipiiiii-1.1.17/template/python_openai.j2`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.0.2/template/template_fastapi.yaml` & `sipiiiii-1.1.17/template/template_fastapi.yaml`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.0.2/template/template_flask.yaml` & `sipiiiii-1.1.17/template/template_flask.yaml`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.0.2/template/template_openai.yaml` & `sipiiiii-1.1.17/template/template_openai.yaml`

 * *Files identical despite different names*

