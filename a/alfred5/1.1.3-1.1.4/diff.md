# Comparing `tmp/alfred5-1.1.3.tar.gz` & `tmp/alfred5-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfred5-1.1.3.tar", last modified: Fri Apr 14 09:48:46 2023, max compression
+gzip compressed data, was "alfred5-1.1.4.tar", last modified: Sun May 14 20:05:56 2023, max compression
```

## Comparing `alfred5-1.1.3.tar` & `alfred5-1.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:48:46.542957 alfred5-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-14 09:48:35.000000 alfred5-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-14 09:48:35.000000 alfred5-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-04-14 09:48:46.542957 alfred5-1.1.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:48:46.538957 alfred5-1.1.3/alfred5/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-14 09:48:35.000000 alfred5-1.1.3/alfred5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11588 2023-04-14 09:48:35.000000 alfred5-1.1.3/alfred5/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-14 09:48:35.000000 alfred5-1.1.3/alfred5/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:48:46.542957 alfred5-1.1.3/alfred5/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    14257 2023-04-14 09:48:35.000000 alfred5-1.1.3/alfred5/icons/download.png
--rw-r--r--   0 runner    (1001) docker     (123)    35477 2023-04-14 09:48:35.000000 alfred5-1.1.3/alfred5/icons/error.png
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-14 09:48:35.000000 alfred5-1.1.3/alfred5/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:48:46.542957 alfred5-1.1.3/alfred5.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-04-14 09:48:46.000000 alfred5-1.1.3/alfred5.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-14 09:48:46.000000 alfred5-1.1.3/alfred5.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:48:46.000000 alfred5-1.1.3/alfred5.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:48:46.000000 alfred5-1.1.3/alfred5.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-14 09:48:46.000000 alfred5-1.1.3/alfred5.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-14 09:48:46.000000 alfred5-1.1.3/alfred5.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:48:46.542957 alfred5-1.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-04-14 09:48:35.000000 alfred5-1.1.3/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 09:48:46.542957 alfred5-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-14 09:48:35.000000 alfred5-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:48:46.542957 alfred5-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:48:35.000000 alfred5-1.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-14 09:48:35.000000 alfred5-1.1.3/tests/test_snippets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:05:56.983430 alfred5-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-05-14 20:05:48.000000 alfred5-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-14 20:05:48.000000 alfred5-1.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-05-14 20:05:56.983430 alfred5-1.1.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:05:56.979430 alfred5-1.1.4/alfred5/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-14 20:05:48.000000 alfred5-1.1.4/alfred5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-05-14 20:05:48.000000 alfred5-1.1.4/alfred5/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-14 20:05:48.000000 alfred5-1.1.4/alfred5/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:05:56.979430 alfred5-1.1.4/alfred5/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    14257 2023-05-14 20:05:48.000000 alfred5-1.1.4/alfred5/icons/download.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35477 2023-05-14 20:05:48.000000 alfred5-1.1.4/alfred5/icons/error.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-14 20:05:48.000000 alfred5-1.1.4/alfred5/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:05:56.979430 alfred5-1.1.4/alfred5.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-05-14 20:05:56.000000 alfred5-1.1.4/alfred5.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-14 20:05:56.000000 alfred5-1.1.4/alfred5.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 20:05:56.000000 alfred5-1.1.4/alfred5.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 20:05:56.000000 alfred5-1.1.4/alfred5.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-14 20:05:56.000000 alfred5-1.1.4/alfred5.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-14 20:05:56.000000 alfred5-1.1.4/alfred5.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:05:56.979430 alfred5-1.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-05-14 20:05:48.000000 alfred5-1.1.4/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 20:05:56.983430 alfred5-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-14 20:05:48.000000 alfred5-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:05:56.983430 alfred5-1.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 20:05:48.000000 alfred5-1.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-14 20:05:48.000000 alfred5-1.1.4/tests/test_snippets.py
```

### Comparing `alfred5-1.1.3/LICENSE` & `alfred5-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alfred5-1.1.3/PKG-INFO` & `alfred5-1.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfred5
-Version: 1.1.3
+Version: 1.1.4
 Summary: Simple python wrapper for alfred5 workflow / snippets
 Home-page: https://github.com/yedhrab/alfred5
 Author: Yunus Emre Ak
 Author-email: yemreak.com@gmail.com
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/yedhrab/alfred5/
 Project-URL: Changelog, https://github.com/yedhrab/alfred5/releases
@@ -32,20 +32,40 @@
 ```bash
 pip install alfred5
 ```
 - Projects dir structure
     - Put your codes and `requirements.txt` to `src` folders
     - Install `alfred5` via 
         ```bash
-        pip install alfred5 --target=src/lib
+        pip install alfred5 --target=src/libs
         ```
+    - Add the top of the `main.py`
+        ```python
+            import sys
+
+            sys.path.insert(0, "src/libs")
+        ```
+        - ![main](https://i.imgur.com/O6rYLQA.png)
     - If u want to use different `--target` for ex `.` use `WorkflowClient.run(packagedir=".")`
     - Sample of default structure: 
         - ![structure](https://i.imgur.com/doLWDR4.png)
     - **If u install all of requirements, dont need to create `requirements.txt` file in `src`**
+    - _If you use `vscode`, add the code that below to `.vscode/settings.json` to debug your file_
+        - ![vscode](https://i.imgur.com/QeseMTr.png)
+        ```json
+        {
+            "python.analysis.extraPaths": [
+                "./src/libs"
+            ],
+            "python.analysis.exclude": [
+                "./src/libs"
+            ]
+        }
+
+        ```
 - Via `SnippetsClient` API create custom snippets programmaically
 - Via `WorkflowClient` API create custom alfred workflow
     - Craete `requirements.txt` file for your python project to let `alfred5` installs them if needed 🙃
     - To install `from requirements.txt` do all import packages inside `main`
             - Use `global` keyword to access imported packages globally
         - `client.query` is the query string
         - `client.page_count` is the page count for pagination results
@@ -60,14 +80,17 @@
 ## ⭐️ Example Project
 
 ![alt](https://i.imgur.com/tUJjVUJ.png)
 
 ```python
 from re import sub
 from urllib.parse import quote_plus
+import sys
+
+sys.path.insert(0, "src/libs")
 
 from alfred5 import WorkflowClient
 
 
 async def main(client: WorkflowClient):
     # To auto install requirements all import operation must be in here
     global get
```

### Comparing `alfred5-1.1.3/alfred5/client.py` & `alfred5-1.1.4/alfred5/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -255,14 +255,15 @@
     def add_result(
         self,
         title: str,
         subtitle: str = "",
         icon_path: str | Path | None = None,
         arg: str = "",
         http_downloader: Callable[[str], str] | None = None,
+        index: int | None = None,
     ) -> None:
         """Create and add alfred result
 
         - title: result title
         - subtitle: result subtitle
         - icon_path: result icon path
         - arg: argument to pass to alfred
@@ -270,15 +271,22 @@
         """
         icon = None
         if icon_path:
             if http_downloader and "http" in str(icon_path):
                 self.log(f"downloading icon from {icon_path}")
                 icon_path = http_downloader(str(icon_path))
             icon = Result.Icon(str(icon_path))
-        self.results.append(Result(title=title, subtitle=subtitle, icon=icon, arg=arg))
+        if index is not None:
+            self.results.insert(
+                index, Result(title=title, subtitle=subtitle, icon=icon, arg=arg)
+            )
+        else:
+            self.results.append(
+                Result(title=title, subtitle=subtitle, icon=icon, arg=arg)
+            )
 
     def error_response(
         self,
         title: str,
         subtitle: str,
         icon_path: str | Path | None = None,
         arg: str = "",
```

### Comparing `alfred5-1.1.3/alfred5/icons/download.png` & `alfred5-1.1.4/alfred5/icons/download.png`

 * *Files identical despite different names*

### Comparing `alfred5-1.1.3/alfred5/icons/error.png` & `alfred5-1.1.4/alfred5/icons/error.png`

 * *Files identical despite different names*

### Comparing `alfred5-1.1.3/alfred5/models.py` & `alfred5-1.1.4/alfred5/models.py`

 * *Files identical despite different names*

### Comparing `alfred5-1.1.3/alfred5.egg-info/PKG-INFO` & `alfred5-1.1.4/alfred5.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfred5
-Version: 1.1.3
+Version: 1.1.4
 Summary: Simple python wrapper for alfred5 workflow / snippets
 Home-page: https://github.com/yedhrab/alfred5
 Author: Yunus Emre Ak
 Author-email: yemreak.com@gmail.com
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/yedhrab/alfred5/
 Project-URL: Changelog, https://github.com/yedhrab/alfred5/releases
@@ -32,20 +32,40 @@
 ```bash
 pip install alfred5
 ```
 - Projects dir structure
     - Put your codes and `requirements.txt` to `src` folders
     - Install `alfred5` via 
         ```bash
-        pip install alfred5 --target=src/lib
+        pip install alfred5 --target=src/libs
         ```
+    - Add the top of the `main.py`
+        ```python
+            import sys
+
+            sys.path.insert(0, "src/libs")
+        ```
+        - ![main](https://i.imgur.com/O6rYLQA.png)
     - If u want to use different `--target` for ex `.` use `WorkflowClient.run(packagedir=".")`
     - Sample of default structure: 
         - ![structure](https://i.imgur.com/doLWDR4.png)
     - **If u install all of requirements, dont need to create `requirements.txt` file in `src`**
+    - _If you use `vscode`, add the code that below to `.vscode/settings.json` to debug your file_
+        - ![vscode](https://i.imgur.com/QeseMTr.png)
+        ```json
+        {
+            "python.analysis.extraPaths": [
+                "./src/libs"
+            ],
+            "python.analysis.exclude": [
+                "./src/libs"
+            ]
+        }
+
+        ```
 - Via `SnippetsClient` API create custom snippets programmaically
 - Via `WorkflowClient` API create custom alfred workflow
     - Craete `requirements.txt` file for your python project to let `alfred5` installs them if needed 🙃
     - To install `from requirements.txt` do all import packages inside `main`
             - Use `global` keyword to access imported packages globally
         - `client.query` is the query string
         - `client.page_count` is the page count for pagination results
@@ -60,14 +80,17 @@
 ## ⭐️ Example Project
 
 ![alt](https://i.imgur.com/tUJjVUJ.png)
 
 ```python
 from re import sub
 from urllib.parse import quote_plus
+import sys
+
+sys.path.insert(0, "src/libs")
 
 from alfred5 import WorkflowClient
 
 
 async def main(client: WorkflowClient):
     # To auto install requirements all import operation must be in here
     global get
```

### Comparing `alfred5-1.1.3/docs/README.md` & `alfred5-1.1.4/docs/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -7,20 +7,40 @@
 ```bash
 pip install alfred5
 ```
 - Projects dir structure
     - Put your codes and `requirements.txt` to `src` folders
     - Install `alfred5` via 
         ```bash
-        pip install alfred5 --target=src/lib
+        pip install alfred5 --target=src/libs
         ```
+    - Add the top of the `main.py`
+        ```python
+            import sys
+
+            sys.path.insert(0, "src/libs")
+        ```
+        - ![main](https://i.imgur.com/O6rYLQA.png)
     - If u want to use different `--target` for ex `.` use `WorkflowClient.run(packagedir=".")`
     - Sample of default structure: 
         - ![structure](https://i.imgur.com/doLWDR4.png)
     - **If u install all of requirements, dont need to create `requirements.txt` file in `src`**
+    - _If you use `vscode`, add the code that below to `.vscode/settings.json` to debug your file_
+        - ![vscode](https://i.imgur.com/QeseMTr.png)
+        ```json
+        {
+            "python.analysis.extraPaths": [
+                "./src/libs"
+            ],
+            "python.analysis.exclude": [
+                "./src/libs"
+            ]
+        }
+
+        ```
 - Via `SnippetsClient` API create custom snippets programmaically
 - Via `WorkflowClient` API create custom alfred workflow
     - Craete `requirements.txt` file for your python project to let `alfred5` installs them if needed 🙃
     - To install `from requirements.txt` do all import packages inside `main`
             - Use `global` keyword to access imported packages globally
         - `client.query` is the query string
         - `client.page_count` is the page count for pagination results
@@ -35,14 +55,17 @@
 ## ⭐️ Example Project
 
 ![alt](https://i.imgur.com/tUJjVUJ.png)
 
 ```python
 from re import sub
 from urllib.parse import quote_plus
+import sys
+
+sys.path.insert(0, "src/libs")
 
 from alfred5 import WorkflowClient
 
 
 async def main(client: WorkflowClient):
     # To auto install requirements all import operation must be in here
     global get
```

### Comparing `alfred5-1.1.3/setup.py` & `alfred5-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 
 from glob import glob
 from os.path import basename, splitext
 from setuptools import find_packages, setup
 from pathlib import Path
 
-VERSION = "1.1.3"
+VERSION = "1.1.4"
 DESCRIPTION = "Simple python wrapper for alfred5 workflow / snippets"
 README_PATH = "docs/README.md"
 USERNAME = "yedhrab"
 REPOSITORY = "alfred5"
 KEYWORDS = [
     "alfred",
     "alfred5",
```

