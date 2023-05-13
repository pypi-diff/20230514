# Comparing `tmp/aihandler-1.9.8.tar.gz` & `tmp/aihandler-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aihandler-1.9.8.tar", last modified: Fri Apr 28 12:51:06 2023, max compression
+gzip compressed data, was "aihandler-1.9.9.tar", last modified: Fri Apr 28 12:53:21 2023, max compression
```

## Comparing `aihandler-1.9.8.tar` & `aihandler-1.9.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:51:06.171291 aihandler-1.9.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 12:50:52.000000 aihandler-1.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-28 12:51:06.171291 aihandler-1.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-28 12:50:52.000000 aihandler-1.9.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 12:51:06.171291 aihandler-1.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-28 12:50:52.000000 aihandler-1.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:51:06.167291 aihandler-1.9.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:51:06.167291 aihandler-1.9.8/src/aihandler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/controlnet_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/llmrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/offline_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/pyqt_offline_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/qtvar.py
--rw-r--r--   0 runner    (1001) docker     (123)    54948 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/settings_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/socket_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:51:06.171291 aihandler-1.9.8/src/aihandler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-28 12:51:06.000000 aihandler-1.9.8/src/aihandler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-28 12:51:06.000000 aihandler-1.9.8/src/aihandler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 12:51:06.000000 aihandler-1.9.8/src/aihandler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-28 12:51:06.000000 aihandler-1.9.8/src/aihandler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 12:51:06.000000 aihandler-1.9.8/src/aihandler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:53:21.540511 aihandler-1.9.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 12:53:05.000000 aihandler-1.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-28 12:53:21.540511 aihandler-1.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-28 12:53:05.000000 aihandler-1.9.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 12:53:21.540511 aihandler-1.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-28 12:53:05.000000 aihandler-1.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:53:21.536511 aihandler-1.9.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:53:21.540511 aihandler-1.9.9/src/aihandler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:53:05.000000 aihandler-1.9.9/src/aihandler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-28 12:53:05.000000 aihandler-1.9.9/src/aihandler/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-28 12:53:05.000000 aihandler-1.9.9/src/aihandler/controlnet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-28 12:53:05.000000 aihandler-1.9.9/src/aihandler/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-28 12:53:05.000000 aihandler-1.9.9/src/aihandler/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-04-28 12:53:05.000000 aihandler-1.9.9/src/aihandler/llmrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-28 12:53:05.000000 aihandler-1.9.9/src/aihandler/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-04-28 12:53:05.000000 aihandler-1.9.9/src/aihandler/offline_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-04-28 12:53:05.000000 aihandler-1.9.9/src/aihandler/pyqt_offline_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-28 12:53:05.000000 aihandler-1.9.9/src/aihandler/qtvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54948 2023-04-28 12:53:05.000000 aihandler-1.9.9/src/aihandler/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-04-28 12:53:05.000000 aihandler-1.9.9/src/aihandler/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-28 12:53:05.000000 aihandler-1.9.9/src/aihandler/settings_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-28 12:53:05.000000 aihandler-1.9.9/src/aihandler/socket_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-04-28 12:53:05.000000 aihandler-1.9.9/src/aihandler/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:53:21.540511 aihandler-1.9.9/src/aihandler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-28 12:53:21.000000 aihandler-1.9.9/src/aihandler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-28 12:53:21.000000 aihandler-1.9.9/src/aihandler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 12:53:21.000000 aihandler-1.9.9/src/aihandler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-28 12:53:21.000000 aihandler-1.9.9/src/aihandler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 12:53:21.000000 aihandler-1.9.9/src/aihandler.egg-info/top_level.txt
```

### Comparing `aihandler-1.9.8/LICENSE` & `aihandler-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.8/PKG-INFO` & `aihandler-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aihandler
-Version: 1.9.8
+Version: 1.9.9
 Summary: AI Handler: An engine which wraps certain huggingface models
 Home-page: https://github.com/Capsize-Games/aihandler
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
```

### Comparing `aihandler-1.9.8/README.md` & `aihandler-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.8/setup.py` & `aihandler-1.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,25 +37,25 @@
     "tqdm==4.65.0",
     "charset-normalizer==3.1.0",
     "opencv-python==4.7.0.72",
     "setuptools==65.5.1",
     "sympy==1.11.1",
     "typing_extensions==4.5.0",
     "urllib3==1.26.15",
-    "diffusers==0.16.0",
+    "diffusers==0.16.1",
     "transformers==4.28.1",
     "compel==1.1.3",
     "sympy==1.11.1",
     "regex",
 ]
 
 
 setup(
     name="aihandler",
-    version="1.9.8",
+    version="1.9.9",
     author="Capsize LLC",
     description="AI Handler: An engine which wraps certain huggingface models",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="ai, chatbot, chat, ai",
     license="AGPL-3.0",
     author_email="contact@capsize.gg",
```

### Comparing `aihandler-1.9.8/src/aihandler/base_runner.py` & `aihandler-1.9.9/src/aihandler/base_runner.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.8/src/aihandler/controlnet_utils.py` & `aihandler-1.9.9/src/aihandler/controlnet_utils.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.8/src/aihandler/database.py` & `aihandler-1.9.9/src/aihandler/database.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.8/src/aihandler/llmrunner.py` & `aihandler-1.9.9/src/aihandler/llmrunner.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.8/src/aihandler/logger.py` & `aihandler-1.9.9/src/aihandler/logger.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.8/src/aihandler/offline_client.py` & `aihandler-1.9.9/src/aihandler/offline_client.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.8/src/aihandler/pyqt_offline_client.py` & `aihandler-1.9.9/src/aihandler/pyqt_offline_client.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.8/src/aihandler/qtvar.py` & `aihandler-1.9.9/src/aihandler/qtvar.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.8/src/aihandler/runner.py` & `aihandler-1.9.9/src/aihandler/runner.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.8/src/aihandler/settings.py` & `aihandler-1.9.9/src/aihandler/settings.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.8/src/aihandler/settings_manager.py` & `aihandler-1.9.9/src/aihandler/settings_manager.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.8/src/aihandler/socket_server.py` & `aihandler-1.9.9/src/aihandler/socket_server.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.8/src/aihandler/util.py` & `aihandler-1.9.9/src/aihandler/util.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.8/src/aihandler.egg-info/PKG-INFO` & `aihandler-1.9.9/src/aihandler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aihandler
-Version: 1.9.8
+Version: 1.9.9
 Summary: AI Handler: An engine which wraps certain huggingface models
 Home-page: https://github.com/Capsize-Games/aihandler
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
```

### Comparing `aihandler-1.9.8/src/aihandler.egg-info/SOURCES.txt` & `aihandler-1.9.9/src/aihandler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.8/src/aihandler.egg-info/requires.txt` & `aihandler-1.9.9/src/aihandler.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,12 +25,12 @@
 tqdm==4.65.0
 charset-normalizer==3.1.0
 opencv-python==4.7.0.72
 setuptools==65.5.1
 sympy==1.11.1
 typing_extensions==4.5.0
 urllib3==1.26.15
-diffusers==0.16.0
+diffusers==0.16.1
 transformers==4.28.1
 compel==1.1.3
 sympy==1.11.1
 regex
```

