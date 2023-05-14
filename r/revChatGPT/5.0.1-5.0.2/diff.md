# Comparing `tmp/revChatGPT-5.0.1.tar.gz` & `tmp/revChatGPT-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-5.0.1.tar", last modified: Mon May  1 08:35:05 2023, max compression
+gzip compressed data, was "revChatGPT-5.0.2.tar", last modified: Sun May 14 02:10:01 2023, max compression
```

## Comparing `revChatGPT-5.0.1.tar` & `revChatGPT-5.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:35:05.526491 revChatGPT-5.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-01 08:34:36.000000 revChatGPT-5.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-05-01 08:35:05.526491 revChatGPT-5.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-05-01 08:35:05.000000 revChatGPT-5.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-01 08:35:05.530491 revChatGPT-5.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-01 08:34:36.000000 revChatGPT-5.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:35:05.526491 revChatGPT-5.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:35:05.526491 revChatGPT-5.0.1/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    49253 2023-05-01 08:34:36.000000 revChatGPT-5.0.1/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-05-01 08:34:36.000000 revChatGPT-5.0.1/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-01 08:34:36.000000 revChatGPT-5.0.1/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-01 08:34:36.000000 revChatGPT-5.0.1/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:35:05.526491 revChatGPT-5.0.1/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-01 08:34:36.000000 revChatGPT-5.0.1/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-05-01 08:34:36.000000 revChatGPT-5.0.1/src/revChatGPT/recipient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-01 08:34:36.000000 revChatGPT-5.0.1/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-01 08:34:36.000000 revChatGPT-5.0.1/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:35:05.526491 revChatGPT-5.0.1/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-05-01 08:35:05.000000 revChatGPT-5.0.1/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-01 08:35:05.000000 revChatGPT-5.0.1/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 08:35:05.000000 revChatGPT-5.0.1/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-01 08:35:05.000000 revChatGPT-5.0.1/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-01 08:35:05.000000 revChatGPT-5.0.1/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:35:05.526491 revChatGPT-5.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-01 08:34:36.000000 revChatGPT-5.0.1/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:10:01.781939 revChatGPT-5.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-14 02:09:27.000000 revChatGPT-5.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-05-14 02:10:01.781939 revChatGPT-5.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-05-14 02:10:01.000000 revChatGPT-5.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-14 02:10:01.781939 revChatGPT-5.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-14 02:09:27.000000 revChatGPT-5.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:10:01.777938 revChatGPT-5.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:10:01.777938 revChatGPT-5.0.2/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    48990 2023-05-14 02:09:27.000000 revChatGPT-5.0.2/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-05-14 02:09:27.000000 revChatGPT-5.0.2/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-14 02:09:27.000000 revChatGPT-5.0.2/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-14 02:09:27.000000 revChatGPT-5.0.2/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:10:01.781939 revChatGPT-5.0.2/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-14 02:09:27.000000 revChatGPT-5.0.2/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-05-14 02:09:27.000000 revChatGPT-5.0.2/src/revChatGPT/recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-14 02:09:27.000000 revChatGPT-5.0.2/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-14 02:09:27.000000 revChatGPT-5.0.2/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:10:01.781939 revChatGPT-5.0.2/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-05-14 02:10:01.000000 revChatGPT-5.0.2/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-14 02:10:01.000000 revChatGPT-5.0.2/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 02:10:01.000000 revChatGPT-5.0.2/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-14 02:10:01.000000 revChatGPT-5.0.2/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-14 02:10:01.000000 revChatGPT-5.0.2/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:10:01.781939 revChatGPT-5.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-14 02:09:27.000000 revChatGPT-5.0.2/tests/test_recipient.py
```

### Comparing `revChatGPT-5.0.1/LICENSE` & `revChatGPT-5.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.1/PKG-INFO` & `revChatGPT-5.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 5.0.1
+Version: 5.0.2
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -55,15 +55,15 @@
 
 <details>
 
   <summary>
 
 # V1 Standard ChatGPT
 
-Uses a proxy to get around cloudflare. It's open source: https://github.com/acheong08/ChatGPT-Proxy-V4. I currently host the default proxy. As always, no data collected other than by Cloudflare and OpenAI.
+Due to recent tightening of OpenAI's security, the default endpoint has been swapped over to one provided by @pengzhile. It is not open source and privacy is not guarenteed. Use it at your own risk. I am working on an open source implementation with the latest changes but that could take a while.
 
 </summary>
 
 ## Rate limits
 - Proxy server: 5 requests / 10 seconds
 - OpenAI: 50 requests / hour for each account
```

### Comparing `revChatGPT-5.0.1/README.md` & `revChatGPT-5.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 <details>
 
   <summary>
 
 # V1 Standard ChatGPT
 
-Uses a proxy to get around cloudflare. It's open source: https://github.com/acheong08/ChatGPT-Proxy-V4. I currently host the default proxy. As always, no data collected other than by Cloudflare and OpenAI.
+Due to recent tightening of OpenAI's security, the default endpoint has been swapped over to one provided by @pengzhile. It is not open source and privacy is not guarenteed. Use it at your own risk. I am working on an open source implementation with the latest changes but that could take a while.
 
 </summary>
 
 ## Rate limits
 - Proxy server: 5 requests / 10 seconds
 - OpenAI: 50 requests / hour for each account
```

### Comparing `revChatGPT-5.0.1/setup.py` & `revChatGPT-5.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="5.0.1",
+    version="5.0.2",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-5.0.1/src/revChatGPT/V1.py` & `revChatGPT-5.0.2/src/revChatGPT/V1.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             return out
 
         return wrapper
 
     return decorator
 
 
-BASE_URL = environ.get("CHATGPT_BASE_URL") or "https://bypass.churchless.tech/"
+BASE_URL = environ.get("CHATGPT_BASE_URL") or "https://ai.fakeopen.com/api/"
 
 bcolors = t.Colors()
 
 
 class Chatbot:
     """
     Chatbot class for ChatGPT
@@ -210,23 +210,15 @@
         """
         self.session.headers.clear()
         self.session.headers.update(
             {
                 "Accept": "text/event-stream",
                 "Authorization": f"Bearer {access_token}",
                 "Content-Type": "application/json",
-                "X-Openai-Assistant-App-Id": "",
-                "Connection": "close",
-                "Accept-Language": "en-US,en;q=0.9",
-                "Referer": "https://chat.openai.com/chat",
-            },
-        )
-        self.session.cookies.update(
-            {
-                "library": "revChatGPT",
+                "User-Agent": "OpenAI-API-Client/0.1.0",
             },
         )
 
         self.config["access_token"] = access_token
 
         email = self.config.get("email", None)
         if email is not None:
```

### Comparing `revChatGPT-5.0.1/src/revChatGPT/V3.py` & `revChatGPT-5.0.2/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.1/src/revChatGPT/__init__.py` & `revChatGPT-5.0.2/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.1/src/revChatGPT/__main__.py` & `revChatGPT-5.0.2/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.1/src/revChatGPT/config/enable_internet.json` & `revChatGPT-5.0.2/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.1/src/revChatGPT/recipient.py` & `revChatGPT-5.0.2/src/revChatGPT/recipient.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.1/src/revChatGPT/typings.py` & `revChatGPT-5.0.2/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.1/src/revChatGPT/utils.py` & `revChatGPT-5.0.2/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.0.1/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-5.0.2/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 5.0.1
+Version: 5.0.2
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -55,15 +55,15 @@
 
 <details>
 
   <summary>
 
 # V1 Standard ChatGPT
 
-Uses a proxy to get around cloudflare. It's open source: https://github.com/acheong08/ChatGPT-Proxy-V4. I currently host the default proxy. As always, no data collected other than by Cloudflare and OpenAI.
+Due to recent tightening of OpenAI's security, the default endpoint has been swapped over to one provided by @pengzhile. It is not open source and privacy is not guarenteed. Use it at your own risk. I am working on an open source implementation with the latest changes but that could take a while.
 
 </summary>
 
 ## Rate limits
 - Proxy server: 5 requests / 10 seconds
 - OpenAI: 50 requests / hour for each account
```

### Comparing `revChatGPT-5.0.1/tests/test_recipient.py` & `revChatGPT-5.0.2/tests/test_recipient.py`

 * *Files identical despite different names*

