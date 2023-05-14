# Comparing `tmp/get_github_code-0.1.tar.gz` & `tmp/get_github_code-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get_github_code-0.1.tar", max compression
+gzip compressed data, was "get_github_code-0.2.tar", max compression
```

## Comparing `get_github_code-0.1.tar` & `get_github_code-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-05-09 23:19:13.243089 get_github_code-0.1/LICENSE
--rw-r--r--   0        0        0     1836 2023-05-14 16:47:18.200075 get_github_code-0.1/README.md
--rw-r--r--   0        0        0      139 2023-05-14 15:41:54.735614 get_github_code-0.1/get_github_code/__init__.py
--rw-r--r--   0        0        0       86 2023-05-14 15:42:10.623670 get_github_code-0.1/get_github_code/constants/__init__.py
--rw-r--r--   0        0        0       71 2023-05-14 15:42:18.991700 get_github_code-0.1/get_github_code/constants/constants.py
--rw-r--r--   0        0        0       78 2023-05-14 15:42:22.615713 get_github_code-0.1/get_github_code/decode/__init__.py
--rw-r--r--   0        0        0      344 2023-05-13 22:54:57.654359 get_github_code-0.1/get_github_code/decode/decode.py
--rw-r--r--   0        0        0      109 2023-05-14 15:42:28.463733 get_github_code-0.1/get_github_code/exceptions/__init__.py
--rw-r--r--   0        0        0       43 2023-05-13 23:12:57.868721 get_github_code-0.1/get_github_code/exceptions/get_code_error.py
--rw-r--r--   0        0        0      238 2023-05-14 15:42:31.711745 get_github_code-0.1/get_github_code/get_code/__init__.py
--rw-r--r--   0        0        0     2888 2023-05-14 16:05:39.128235 get_github_code-0.1/get_github_code/get_code/get_code.py
--rw-r--r--   0        0        0       70 2023-05-14 15:43:02.731855 get_github_code-0.1/get_github_code/json/__init__.py
--rw-r--r--   0        0        0      244 2023-05-14 00:45:49.709771 get_github_code-0.1/get_github_code/json/json.py
--rw-r--r--   0        0        0       82 2023-05-14 15:43:05.527865 get_github_code-0.1/get_github_code/request/__init__.py
--rw-r--r--   0        0        0     1048 2023-05-14 00:44:44.974768 get_github_code-0.1/get_github_code/request/request.py
--rw-r--r--   0        0        0     1514 2023-05-14 17:38:25.823882 get_github_code-0.1/pyproject.toml
--rw-r--r--   0        0        0     3565 1970-01-01 00:00:00.000000 get_github_code-0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-09 23:19:13.243089 get_github_code-0.2/LICENSE
+-rw-r--r--   0        0        0     2039 2023-05-14 17:59:21.378556 get_github_code-0.2/README.md
+-rw-r--r--   0        0        0      139 2023-05-14 15:41:54.735614 get_github_code-0.2/get_github_code/__init__.py
+-rw-r--r--   0        0        0       86 2023-05-14 15:42:10.623670 get_github_code-0.2/get_github_code/constants/__init__.py
+-rw-r--r--   0        0        0       71 2023-05-14 15:42:18.991700 get_github_code-0.2/get_github_code/constants/constants.py
+-rw-r--r--   0        0        0       78 2023-05-14 15:42:22.615713 get_github_code-0.2/get_github_code/decode/__init__.py
+-rw-r--r--   0        0        0      344 2023-05-13 22:54:57.654359 get_github_code-0.2/get_github_code/decode/decode.py
+-rw-r--r--   0        0        0      109 2023-05-14 15:42:28.463733 get_github_code-0.2/get_github_code/exceptions/__init__.py
+-rw-r--r--   0        0        0       43 2023-05-13 23:12:57.868721 get_github_code-0.2/get_github_code/exceptions/get_code_error.py
+-rw-r--r--   0        0        0      238 2023-05-14 15:42:31.711745 get_github_code-0.2/get_github_code/get_code/__init__.py
+-rw-r--r--   0        0        0     2888 2023-05-14 16:05:39.128235 get_github_code-0.2/get_github_code/get_code/get_code.py
+-rw-r--r--   0        0        0       70 2023-05-14 15:43:02.731855 get_github_code-0.2/get_github_code/json/__init__.py
+-rw-r--r--   0        0        0      244 2023-05-14 00:45:49.709771 get_github_code-0.2/get_github_code/json/json.py
+-rw-r--r--   0        0        0       82 2023-05-14 15:43:05.527865 get_github_code-0.2/get_github_code/request/__init__.py
+-rw-r--r--   0        0        0     1048 2023-05-14 00:44:44.974768 get_github_code-0.2/get_github_code/request/request.py
+-rw-r--r--   0        0        0     1514 2023-05-14 17:58:57.905343 get_github_code-0.2/pyproject.toml
+-rw-r--r--   0        0        0     3768 1970-01-01 00:00:00.000000 get_github_code-0.2/PKG-INFO
```

### Comparing `get_github_code-0.1/LICENSE` & `get_github_code-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `get_github_code-0.1/README.md` & `get_github_code-0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+## Get code from GitHub
+[![pypi](https://img.shields.io/pypi/v/get_github_code)](https://pypi.org/project/get-github-code/)
+[![](https://img.shields.io/pypi/pyversions/get_github_code)](https://pypi.org/project/get-github-code/)
 [![CodeFactor](https://www.codefactor.io/repository/github/vlad2030/get-code-from-github/badge/main)](https://www.codefactor.io/repository/github/vlad2030/get-code-from-github/overview/main)
 
-## Get code from GitHub
 this is a small python library to get code from github repositories
 
 ## How to install
 ```bash
 pip3 install get_github_code
 ```
 
@@ -18,15 +20,15 @@
     user="Vlad2030",
     repo="get-code-from-github",
     branch="main",
     file_path="VERSION",
 )
 
 print(code)
-# 0.1
+# 0.2
 ```
 
 or asynchronous
 
 ```python
 import asyncio
 from get_github_code import async_get_code
@@ -38,15 +40,15 @@
         branch="main",
         file_path="VERSION",
     )
 
     print(code)
 
 asyncio.run(main())
-# 0.1
+# 0.2
 ```
 
 additionally you can through the class by calling property
 
 ```python
 import asyncio
 from get_github_code import GetCode
@@ -55,34 +57,34 @@
     user="Vlad2030",
     repo="get-code-from-github",
     branch="main",
     file_path="VERSION",
 )
 
 print(file.get_code)
-# 0.1
+# 0.2
 
 async def main() -> None:
     file = GetCode(
         user="Vlad2030",
         repo="get-code-from-github",
         branch="main",
         file_path="VERSION",
     )
 
     print(file.async_get_code)
 
 asyncio.run(main())
-# 0.1
+# 0.2
 ```
 
 ## Documentation
 [How to install](https://github.com/Vlad2030/get-code-from-github/blob/main/docs/install.md)
 
 [Classes/GetCode](https://github.com/Vlad2030/get-code-from-github/blob/main/docs/classes/GetCode.md)
 
 [functions/get_code](https://github.com/Vlad2030/get-code-from-github/blob/main/docs/functions/get_code.md)
 
 [functions/async_get_code](https://github.com/Vlad2030/get-code-from-github/blob/main/docs/functions/async_get_code.md)
 
 
-> 2023, version 0.0.1
+> 2023, version 0.2
```

### Comparing `get_github_code-0.1/get_github_code/get_code/get_code.py` & `get_github_code-0.2/get_github_code/get_code/get_code.py`

 * *Files identical despite different names*

### Comparing `get_github_code-0.1/get_github_code/request/request.py` & `get_github_code-0.2/get_github_code/request/request.py`

 * *Files identical despite different names*

### Comparing `get_github_code-0.1/pyproject.toml` & `get_github_code-0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "get_github_code"
 
 
 [tool.poetry]
 name = "get_github_code"
-version = "0.1"
+version = "0.2"
 description = "a small python library to get code from github repositories."
 authors = ["vladdd0 <vlad123123v@gmail.com>"]
 license = "GNU"
 readme = "README.md"
 homepage = "https://github.com/Vlad2030/get-code-from-github"
 repository = "https://github.com/Vlad2030/get-code-from-github"
 documentation = "https://get-code-from-github.readthedocs.io/en/latest/"
```

### Comparing `get_github_code-0.1/PKG-INFO` & `get_github_code-0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: get-github-code
-Version: 0.1
+Version: 0.2
 Summary: a small python library to get code from github repositories.
 Home-page: https://github.com/Vlad2030/get-code-from-github
 License: GNU
 Keywords: urllib3,aiohttp,asyncio,orjson
 Author: vladdd0
 Author-email: vlad123123v@gmail.com
 Requires-Python: >=3.7.0,<4.0.0
@@ -34,17 +34,19 @@
 Requires-Dist: asyncio (>=3.4.3)
 Requires-Dist: orjson (>=3.5.2) ; extra == "orjson" or extra == "all"
 Requires-Dist: urllib3 (>=1.26.5)
 Project-URL: Documentation, https://get-code-from-github.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/Vlad2030/get-code-from-github
 Description-Content-Type: text/markdown
 
+## Get code from GitHub
+[![pypi](https://img.shields.io/pypi/v/get_github_code)](https://pypi.org/project/get-github-code/)
+[![](https://img.shields.io/pypi/pyversions/get_github_code)](https://pypi.org/project/get-github-code/)
 [![CodeFactor](https://www.codefactor.io/repository/github/vlad2030/get-code-from-github/badge/main)](https://www.codefactor.io/repository/github/vlad2030/get-code-from-github/overview/main)
 
-## Get code from GitHub
 this is a small python library to get code from github repositories
 
 ## How to install
 ```bash
 pip3 install get_github_code
 ```
 
@@ -58,15 +60,15 @@
     user="Vlad2030",
     repo="get-code-from-github",
     branch="main",
     file_path="VERSION",
 )
 
 print(code)
-# 0.1
+# 0.2
 ```
 
 or asynchronous
 
 ```python
 import asyncio
 from get_github_code import async_get_code
@@ -78,15 +80,15 @@
         branch="main",
         file_path="VERSION",
     )
 
     print(code)
 
 asyncio.run(main())
-# 0.1
+# 0.2
 ```
 
 additionally you can through the class by calling property
 
 ```python
 import asyncio
 from get_github_code import GetCode
@@ -95,34 +97,34 @@
     user="Vlad2030",
     repo="get-code-from-github",
     branch="main",
     file_path="VERSION",
 )
 
 print(file.get_code)
-# 0.1
+# 0.2
 
 async def main() -> None:
     file = GetCode(
         user="Vlad2030",
         repo="get-code-from-github",
         branch="main",
         file_path="VERSION",
     )
 
     print(file.async_get_code)
 
 asyncio.run(main())
-# 0.1
+# 0.2
 ```
 
 ## Documentation
 [How to install](https://github.com/Vlad2030/get-code-from-github/blob/main/docs/install.md)
 
 [Classes/GetCode](https://github.com/Vlad2030/get-code-from-github/blob/main/docs/classes/GetCode.md)
 
 [functions/get_code](https://github.com/Vlad2030/get-code-from-github/blob/main/docs/functions/get_code.md)
 
 [functions/async_get_code](https://github.com/Vlad2030/get-code-from-github/blob/main/docs/functions/async_get_code.md)
 
 
-> 2023, version 0.0.1
+> 2023, version 0.2
```

