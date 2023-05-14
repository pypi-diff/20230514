# Comparing `tmp/v4xyz-0.0.4.tar.gz` & `tmp/v4xyz-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "v4xyz-0.0.4.tar", last modified: Sat May 13 12:03:00 2023, max compression
+gzip compressed data, was "v4xyz-0.0.5.tar", last modified: Sun May 14 09:51:52 2023, max compression
```

## Comparing `v4xyz-0.0.4.tar` & `v4xyz-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-13 12:03:00.441102 v4xyz-0.0.4/
--rw-r--r--   0 john      (1000) john      (1000)    11540 2023-05-13 11:27:28.000000 v4xyz-0.0.4/LICENSE
--rw-r--r--   0 john      (1000) john      (1000)     3037 2023-05-13 12:03:00.441102 v4xyz-0.0.4/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)     1793 2023-05-13 11:37:16.000000 v4xyz-0.0.4/README.md
--rw-r--r--   0 john      (1000) john      (1000)       38 2023-05-13 12:03:00.441102 v4xyz-0.0.4/setup.cfg
--rw-r--r--   0 john      (1000) john      (1000)     1370 2023-05-13 12:02:34.000000 v4xyz-0.0.4/setup.py
--rw-r--r--   0 john      (1000) john      (1000)     4952 2023-05-13 11:19:45.000000 v4xyz-0.0.4/v4.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-13 12:03:00.441102 v4xyz-0.0.4/v4xyz.egg-info/
--rw-r--r--   0 john      (1000) john      (1000)     3037 2023-05-13 12:03:00.000000 v4xyz-0.0.4/v4xyz.egg-info/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)      208 2023-05-13 12:03:00.000000 v4xyz-0.0.4/v4xyz.egg-info/SOURCES.txt
--rw-r--r--   0 john      (1000) john      (1000)        1 2023-05-13 12:03:00.000000 v4xyz-0.0.4/v4xyz.egg-info/dependency_links.txt
--rw-r--r--   0 john      (1000) john      (1000)       32 2023-05-13 12:03:00.000000 v4xyz-0.0.4/v4xyz.egg-info/entry_points.txt
--rw-r--r--   0 john      (1000) john      (1000)       50 2023-05-13 12:03:00.000000 v4xyz-0.0.4/v4xyz.egg-info/requires.txt
--rw-r--r--   0 john      (1000) john      (1000)        3 2023-05-13 12:03:00.000000 v4xyz-0.0.4/v4xyz.egg-info/top_level.txt
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-14 09:51:51.991528 v4xyz-0.0.5/
+-rw-r--r--   0 john      (1000) john      (1000)    11540 2023-05-13 11:27:28.000000 v4xyz-0.0.5/LICENSE
+-rw-r--r--   0 john      (1000) john      (1000)     3128 2023-05-14 09:51:51.991528 v4xyz-0.0.5/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)     1863 2023-05-14 09:49:41.000000 v4xyz-0.0.5/README.md
+-rw-r--r--   0 john      (1000) john      (1000)       74 2023-05-14 09:51:51.991528 v4xyz-0.0.5/setup.cfg
+-rw-r--r--   0 john      (1000) john      (1000)     1429 2023-05-14 09:51:41.000000 v4xyz-0.0.5/setup.py
+-rw-r--r--   0 john      (1000) john      (1000)     5242 2023-05-13 14:11:35.000000 v4xyz-0.0.5/v4.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-14 09:51:51.991528 v4xyz-0.0.5/v4xyz.egg-info/
+-rw-r--r--   0 john      (1000) john      (1000)     3128 2023-05-14 09:51:51.000000 v4xyz-0.0.5/v4xyz.egg-info/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)      218 2023-05-14 09:51:51.000000 v4xyz-0.0.5/v4xyz.egg-info/SOURCES.txt
+-rw-r--r--   0 john      (1000) john      (1000)        1 2023-05-14 09:51:51.000000 v4xyz-0.0.5/v4xyz.egg-info/dependency_links.txt
+-rw-r--r--   0 john      (1000) john      (1000)       32 2023-05-14 09:51:51.000000 v4xyz-0.0.5/v4xyz.egg-info/entry_points.txt
+-rw-r--r--   0 john      (1000) john      (1000)       50 2023-05-14 09:51:51.000000 v4xyz-0.0.5/v4xyz.egg-info/requires.txt
+-rw-r--r--   0 john      (1000) john      (1000)        3 2023-05-14 09:51:51.000000 v4xyz-0.0.5/v4xyz.egg-info/top_level.txt
```

### Comparing `v4xyz-0.0.4/LICENSE` & `v4xyz-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `v4xyz-0.0.4/PKG-INFO` & `v4xyz-0.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 Metadata-Version: 2.1
 Name: v4xyz
-Version: 0.0.4
+Version: 0.0.5
 Summary: A command line tool to chat with GPT4 and render markdown response.
 Home-page: https://github.com/imhuwq/v4xyz
 Author: imhuwq
 Author-email: imhuwq@gmail.com
 License: UNKNOWN
 Description: # v4xyz
         
         ---
         <div align="center">
         <p align="center">
         
         <!-- prettier-ignore -->
         
-        **A command line tool to chat with GPT4 and render markdown response.**
+        ## v4xyz, way for doing kinds of things.
         
-        ---
         ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/v4xyz?style=social)
         ![PyPI](https://img.shields.io/pypi/v/v4xyz?style=social)
         ![PyPI - Downloads](https://img.shields.io/pypi/dm/v4xyz?style=social)
         ![PyPI - License](https://img.shields.io/pypi/l/v4xyz?style=social)
         
+        **A cli tool that ask GPT4 for programming solutions and get answers directly in terminal.**
+        
         ```
          ______   __    _              _             __    __            _      __             
         /_  __/  / /   (_)  ___       (_)  ___      / /_  / /  ___      | | /| / / ___ _  __ __
          / /    / _ \ / /  (_-<      / /  (_-<     / __/ / _ \/ -_)     | |/ |/ / / _ `/ / // /
         /_/    /_//_//_/  /___/     /_/  /___/     \__/ /_//_/\__/      |__/|__/  \_,_/  \_, / 
                                                                                         /___/  
         ```
         
+        ---
+        
         </p>
         </div>
         
         ## 1. Installation
         
         ### 1.1 Installing from pypi
         
@@ -64,17 +67,17 @@
           "openai_secret": "",
           "http_proxy": "",
           "https_proxy": ""
         }
         ```
         
         The `openai_secret` must be set to your OpenAI key.   
-        The `http_proxy` and `https_proxy` are optional if the OpenAI API is accessible from your region.
+        The `http_proxy` and `https_proxy` are optional if the OpenAI API is directly accessible from your region.
         
-        ## 3. Chat with GPT4 in Terminal
+        ## 3. Ask GPT4 in Terminal
         
         ```shell
         v4 'How to config a reverse proxy with Nginx?'
         v4 'send a HTTP GET request using telnet'
         v4 'any thing here'
         ```
```

### Comparing `v4xyz-0.0.4/README.md` & `v4xyz-0.0.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,30 +2,33 @@
 
 ---
 <div align="center">
 <p align="center">
 
 <!-- prettier-ignore -->
 
-**A command line tool to chat with GPT4 and render markdown response.**
+## v4xyz, way for doing kinds of things.
 
----
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/v4xyz?style=social)
 ![PyPI](https://img.shields.io/pypi/v/v4xyz?style=social)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/v4xyz?style=social)
 ![PyPI - License](https://img.shields.io/pypi/l/v4xyz?style=social)
 
+**A cli tool that ask GPT4 for programming solutions and get answers directly in terminal.**
+
 ```
  ______   __    _              _             __    __            _      __             
 /_  __/  / /   (_)  ___       (_)  ___      / /_  / /  ___      | | /| / / ___ _  __ __
  / /    / _ \ / /  (_-<      / /  (_-<     / __/ / _ \/ -_)     | |/ |/ / / _ `/ / // /
 /_/    /_//_//_/  /___/     /_/  /___/     \__/ /_//_/\__/      |__/|__/  \_,_/  \_, / 
                                                                                 /___/  
 ```
 
+---
+
 </p>
 </div>
 
 ## 1. Installation
 
 ### 1.1 Installing from pypi
 
@@ -56,16 +59,16 @@
   "openai_secret": "",
   "http_proxy": "",
   "https_proxy": ""
 }
 ```
 
 The `openai_secret` must be set to your OpenAI key.   
-The `http_proxy` and `https_proxy` are optional if the OpenAI API is accessible from your region.
+The `http_proxy` and `https_proxy` are optional if the OpenAI API is directly accessible from your region.
 
-## 3. Chat with GPT4 in Terminal
+## 3. Ask GPT4 in Terminal
 
 ```shell
 v4 'How to config a reverse proxy with Nginx?'
 v4 'send a HTTP GET request using telnet'
 v4 'any thing here'
 ```
```

### Comparing `v4xyz-0.0.4/setup.py` & `v4xyz-0.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from setuptools import setup
 
-version = "0.0.4"
+version = "0.0.5"
 description = "A command line tool to chat with GPT4 and render markdown response."
 with open("README.md") as fp:
     long_description = fp.read()
 url = "https://github.com/imhuwq/v4xyz"
 author = "imhuwq"
 author_email = "imhuwq@gmail.com"
+with open("LICENSE") as fp:
+    license_text = fp.read()
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Topic :: Communications :: Chat",
     "Topic :: Terminals",
     "Operating System :: POSIX :: Linux",
```

### Comparing `v4xyz-0.0.4/v4.py` & `v4xyz-0.0.5/v4.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,26 +37,30 @@
     click.edit(filename=CONFIG_PATH)
 
 
 def load_config():
     global OPENAI_SECRET
 
     if not os.path.exists(CONFIG_PATH):
-        click.echo("config file not found, try `v4 -e` first to generate a config file.")
+        click.echo("config file not found, try `v4 -e` first to set your config file.")
         exit(1)
 
     with open(CONFIG_PATH) as fp:
         config = json.load(fp)
 
     if config["http_proxy"]:
         os.environ["http_proxy"] = config["http_proxy"]
     if config["https_proxy"]:
         os.environ["https_proxy"] = config["https_proxy"]
 
     OPENAI_SECRET = config["openai_secret"]
+    if not OPENAI_SECRET:
+        click.echo("openai_secret is not set in config file, try `v4 -e` to edit your config file")
+        exit(1)
+
     openai.api_key = OPENAI_SECRET
 
 
 def count_token(content: str):
     return len(content) // 4
 
 
@@ -139,21 +143,24 @@
     print("")
     print("-" * 10)
     print(f"[bold yellow]Received: {count_token(answer)} tokens[/]")
 
 
 @click.command(cls=Cmd)
 @click.option("-e", "--edit", is_flag=True, help="Edit the config file")
-@click.argument("inputs", nargs=1, required=True)
+@click.argument("inputs", nargs=1, required=False)  # required must be False, otherwise we cant get into edit mode
 def v4(edit, inputs):
     if edit is True:
         return edit_config()
-    else:
-        load_config()
 
+    if inputs is None:
+        click.echo(v4.get_help(click.Context(v4)))
+        exit(1)
+
+    load_config()
     inputs = inputs.strip()
     if not inputs:
         return
 
     inputs = inputs.capitalize()
     return ask_gpt4(inputs)
```

### Comparing `v4xyz-0.0.4/v4xyz.egg-info/PKG-INFO` & `v4xyz-0.0.5/v4xyz.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 Metadata-Version: 2.1
 Name: v4xyz
-Version: 0.0.4
+Version: 0.0.5
 Summary: A command line tool to chat with GPT4 and render markdown response.
 Home-page: https://github.com/imhuwq/v4xyz
 Author: imhuwq
 Author-email: imhuwq@gmail.com
 License: UNKNOWN
 Description: # v4xyz
         
         ---
         <div align="center">
         <p align="center">
         
         <!-- prettier-ignore -->
         
-        **A command line tool to chat with GPT4 and render markdown response.**
+        ## v4xyz, way for doing kinds of things.
         
-        ---
         ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/v4xyz?style=social)
         ![PyPI](https://img.shields.io/pypi/v/v4xyz?style=social)
         ![PyPI - Downloads](https://img.shields.io/pypi/dm/v4xyz?style=social)
         ![PyPI - License](https://img.shields.io/pypi/l/v4xyz?style=social)
         
+        **A cli tool that ask GPT4 for programming solutions and get answers directly in terminal.**
+        
         ```
          ______   __    _              _             __    __            _      __             
         /_  __/  / /   (_)  ___       (_)  ___      / /_  / /  ___      | | /| / / ___ _  __ __
          / /    / _ \ / /  (_-<      / /  (_-<     / __/ / _ \/ -_)     | |/ |/ / / _ `/ / // /
         /_/    /_//_//_/  /___/     /_/  /___/     \__/ /_//_/\__/      |__/|__/  \_,_/  \_, / 
                                                                                         /___/  
         ```
         
+        ---
+        
         </p>
         </div>
         
         ## 1. Installation
         
         ### 1.1 Installing from pypi
         
@@ -64,17 +67,17 @@
           "openai_secret": "",
           "http_proxy": "",
           "https_proxy": ""
         }
         ```
         
         The `openai_secret` must be set to your OpenAI key.   
-        The `http_proxy` and `https_proxy` are optional if the OpenAI API is accessible from your region.
+        The `http_proxy` and `https_proxy` are optional if the OpenAI API is directly accessible from your region.
         
-        ## 3. Chat with GPT4 in Terminal
+        ## 3. Ask GPT4 in Terminal
         
         ```shell
         v4 'How to config a reverse proxy with Nginx?'
         v4 'send a HTTP GET request using telnet'
         v4 'any thing here'
         ```
```

