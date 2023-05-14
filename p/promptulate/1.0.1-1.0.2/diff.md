# Comparing `tmp/promptulate-1.0.1.tar.gz` & `tmp/promptulate-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptulate-1.0.1.tar", last modified: Sat May 13 17:13:28 2023, max compression
+gzip compressed data, was "promptulate-1.0.2.tar", last modified: Sun May 14 03:18:49 2023, max compression
```

## Comparing `promptulate-1.0.1.tar` & `promptulate-1.0.2.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 17:13:28.627344 promptulate-1.0.1/
--rw-rw-rw-   0        0        0    11558 2023-05-13 17:09:36.000000 promptulate-1.0.1/LICENSE
--rw-rw-rw-   0        0        0    15599 2023-05-13 17:13:28.625372 promptulate-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    14665 2023-05-13 17:09:36.000000 promptulate-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-13 17:13:28.538782 promptulate-1.0.1/promptulate/
--rw-rw-rw-   0        0        0     1199 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 17:13:28.554780 promptulate-1.0.1/promptulate/command/
--rw-rw-rw-   0        0        0      127 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/command/__init__.py
--rw-rw-rw-   0        0        0     1673 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/command/chat.py
--rw-rw-rw-   0        0        0     2655 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/config.py
-drwxrwxrwx   0        0        0        0 2023-05-13 17:13:28.562727 promptulate-1.0.1/promptulate/frameworks/
--rw-rw-rw-   0        0        0      866 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/frameworks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 17:13:28.566667 promptulate-1.0.1/promptulate/frameworks/base/
--rw-rw-rw-   0        0        0      878 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/frameworks/base/__init__.py
--rw-rw-rw-   0        0        0     3367 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/frameworks/base/conversation.py
--rw-rw-rw-   0        0        0     1776 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/frameworks/prompt.py
-drwxrwxrwx   0        0        0        0 2023-05-13 17:13:28.569667 promptulate-1.0.1/promptulate/frameworks/react/
--rw-rw-rw-   0        0        0      769 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/frameworks/react/__init__.py
--rw-rw-rw-   0        0        0     1074 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/frameworks/schema.py
-drwxrwxrwx   0        0        0        0 2023-05-13 17:13:28.571674 promptulate-1.0.1/promptulate/frameworks/self_ask/
--rw-rw-rw-   0        0        0      769 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/frameworks/self_ask/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 17:13:28.578667 promptulate-1.0.1/promptulate/llms/
--rw-rw-rw-   0        0        0      848 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/llms/__init__.py
--rw-rw-rw-   0        0        0     1504 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/llms/base.py
--rw-rw-rw-   0        0        0     3828 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/llms/openai.py
-drwxrwxrwx   0        0        0        0 2023-05-13 17:13:28.588729 promptulate-1.0.1/promptulate/memory/
--rw-rw-rw-   0        0        0      963 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/memory/__init__.py
--rw-rw-rw-   0        0        0     1721 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/memory/base.py
--rw-rw-rw-   0        0        0     1773 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/memory/buffer.py
--rw-rw-rw-   0        0        0     1894 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/memory/local_cache.py
-drwxrwxrwx   0        0        0        0 2023-05-13 17:13:28.596725 promptulate-1.0.1/promptulate/preset_roles/
--rw-rw-rw-   0        0        0      925 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/preset_roles/__init__.py
--rw-rw-rw-   0        0        0     3264 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/preset_roles/prompt.py
--rw-rw-rw-   0        0        0     5331 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/preset_roles/roles.py
-drwxrwxrwx   0        0        0        0 2023-05-13 17:13:28.601721 promptulate-1.0.1/promptulate/provider/
--rw-rw-rw-   0        0        0     1059 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/provider/__init__.py
--rw-rw-rw-   0        0        0     5477 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/provider/mixins.py
--rw-rw-rw-   0        0        0     5982 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/schema.py
--rw-rw-rw-   0        0        0      881 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/tips.py
-drwxrwxrwx   0        0        0        0 2023-05-13 17:13:28.607719 promptulate-1.0.1/promptulate/tools/
--rw-rw-rw-   0        0        0      773 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/tools/__init__.py
--rw-rw-rw-   0        0        0      769 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/tools/duckduckgo.py
-drwxrwxrwx   0        0        0        0 2023-05-13 17:13:28.622726 promptulate-1.0.1/promptulate/utils/
--rw-rw-rw-   0        0        0     1304 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/utils/__init__.py
--rw-rw-rw-   0        0        0     2145 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/utils/_utils.py
--rw-rw-rw-   0        0        0     1962 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/utils/logger.py
--rw-rw-rw-   0        0        0     1626 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/utils/proxy.py
--rw-rw-rw-   0        0        0      656 2023-05-13 17:09:36.000000 promptulate-1.0.1/promptulate/utils/singleton.py
-drwxrwxrwx   0        0        0        0 2023-05-13 17:13:28.550789 promptulate-1.0.1/promptulate.egg-info/
--rw-rw-rw-   0        0        0    15599 2023-05-13 17:13:28.000000 promptulate-1.0.1/promptulate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1200 2023-05-13 17:13:28.000000 promptulate-1.0.1/promptulate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 17:13:28.000000 promptulate-1.0.1/promptulate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-05-13 17:13:28.000000 promptulate-1.0.1/promptulate.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       12 2023-05-13 17:13:28.000000 promptulate-1.0.1/promptulate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-13 17:13:28.627344 promptulate-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1976 2023-05-13 17:09:36.000000 promptulate-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 03:18:49.383516 promptulate-1.0.2/
+-rw-rw-rw-   0        0        0    11558 2023-05-13 17:09:36.000000 promptulate-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0    15599 2023-05-14 03:18:49.382516 promptulate-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    14665 2023-05-13 17:09:36.000000 promptulate-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 03:18:49.289442 promptulate-1.0.2/promptulate/
+-rw-rw-rw-   0        0        0     1199 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 03:18:49.310420 promptulate-1.0.2/promptulate/command/
+-rw-rw-rw-   0        0        0      127 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/command/__init__.py
+-rw-rw-rw-   0        0        0     1673 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/command/chat.py
+-rw-rw-rw-   0        0        0     2655 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/config.py
+drwxrwxrwx   0        0        0        0 2023-05-14 03:18:49.317354 promptulate-1.0.2/promptulate/frameworks/
+-rw-rw-rw-   0        0        0      866 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/frameworks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 03:18:49.323350 promptulate-1.0.2/promptulate/frameworks/base/
+-rw-rw-rw-   0        0        0      878 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/frameworks/base/__init__.py
+-rw-rw-rw-   0        0        0     3367 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/frameworks/base/conversation.py
+-rw-rw-rw-   0        0        0     1776 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/frameworks/prompt.py
+drwxrwxrwx   0        0        0        0 2023-05-14 03:18:49.326357 promptulate-1.0.2/promptulate/frameworks/react/
+-rw-rw-rw-   0        0        0      769 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/frameworks/react/__init__.py
+-rw-rw-rw-   0        0        0     1074 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/frameworks/schema.py
+drwxrwxrwx   0        0        0        0 2023-05-14 03:18:49.328355 promptulate-1.0.2/promptulate/frameworks/self_ask/
+-rw-rw-rw-   0        0        0      769 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/frameworks/self_ask/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 03:18:49.336380 promptulate-1.0.2/promptulate/llms/
+-rw-rw-rw-   0        0        0      848 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/llms/__init__.py
+-rw-rw-rw-   0        0        0     1504 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/llms/base.py
+-rw-rw-rw-   0        0        0     3828 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/llms/openai.py
+drwxrwxrwx   0        0        0        0 2023-05-14 03:18:49.347376 promptulate-1.0.2/promptulate/memory/
+-rw-rw-rw-   0        0        0      963 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/memory/__init__.py
+-rw-rw-rw-   0        0        0     1721 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/memory/base.py
+-rw-rw-rw-   0        0        0     1773 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/memory/buffer.py
+-rw-rw-rw-   0        0        0     1894 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/memory/local_cache.py
+drwxrwxrwx   0        0        0        0 2023-05-14 03:18:49.355409 promptulate-1.0.2/promptulate/preset_roles/
+-rw-rw-rw-   0        0        0      925 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/preset_roles/__init__.py
+-rw-rw-rw-   0        0        0     3264 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/preset_roles/prompt.py
+-rw-rw-rw-   0        0        0     5331 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/preset_roles/roles.py
+drwxrwxrwx   0        0        0        0 2023-05-14 03:18:49.361407 promptulate-1.0.2/promptulate/provider/
+-rw-rw-rw-   0        0        0     1059 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/provider/__init__.py
+-rw-rw-rw-   0        0        0     5477 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/provider/mixins.py
+-rw-rw-rw-   0        0        0     5982 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/schema.py
+-rw-rw-rw-   0        0        0      881 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/tips.py
+drwxrwxrwx   0        0        0        0 2023-05-14 03:18:49.365411 promptulate-1.0.2/promptulate/tools/
+-rw-rw-rw-   0        0        0      773 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/tools/__init__.py
+-rw-rw-rw-   0        0        0      769 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/tools/duckduckgo.py
+drwxrwxrwx   0        0        0        0 2023-05-14 03:18:49.379407 promptulate-1.0.2/promptulate/utils/
+-rw-rw-rw-   0        0        0     1304 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/utils/__init__.py
+-rw-rw-rw-   0        0        0     2145 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/utils/_utils.py
+-rw-rw-rw-   0        0        0     1962 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/utils/logger.py
+-rw-rw-rw-   0        0        0     1626 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/utils/proxy.py
+-rw-rw-rw-   0        0        0      656 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/utils/singleton.py
+drwxrwxrwx   0        0        0        0 2023-05-14 03:18:49.305426 promptulate-1.0.2/promptulate.egg-info/
+-rw-rw-rw-   0        0        0    15599 2023-05-14 03:18:49.000000 promptulate-1.0.2/promptulate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1234 2023-05-14 03:18:49.000000 promptulate-1.0.2/promptulate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 03:18:49.000000 promptulate-1.0.2/promptulate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-05-14 03:18:49.000000 promptulate-1.0.2/promptulate.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-05-14 03:18:49.000000 promptulate-1.0.2/promptulate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-14 03:18:49.000000 promptulate-1.0.2/promptulate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 03:18:49.383516 promptulate-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2041 2023-05-14 03:17:30.000000 promptulate-1.0.2/setup.py
```

### Comparing `promptulate-1.0.1/LICENSE` & `promptulate-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/PKG-INFO` & `promptulate-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptulate
-Version: 1.0.1
+Version: 1.0.2
 Summary: A powerful LLM Prompt Layer frameworks
 Home-page: https://github.com/Undertone0809/promptulate
 Author: Zeeland
 Author-email: zeeland@foxmail.com
 License: Apache 2.0
 Keywords: promptulate,prompt-me,prompt,chatgpt,gpt,chatbot,llm
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `promptulate-1.0.1/README.md` & `promptulate-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/__init__.py` & `promptulate-1.0.2/promptulate/__init__.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/command/chat.py` & `promptulate-1.0.2/promptulate/command/chat.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/config.py` & `promptulate-1.0.2/promptulate/config.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/frameworks/__init__.py` & `promptulate-1.0.2/promptulate/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/frameworks/base/__init__.py` & `promptulate-1.0.2/promptulate/frameworks/base/__init__.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/frameworks/base/conversation.py` & `promptulate-1.0.2/promptulate/frameworks/base/conversation.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/frameworks/prompt.py` & `promptulate-1.0.2/promptulate/frameworks/prompt.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/frameworks/react/__init__.py` & `promptulate-1.0.2/promptulate/frameworks/react/__init__.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/frameworks/schema.py` & `promptulate-1.0.2/promptulate/frameworks/schema.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/frameworks/self_ask/__init__.py` & `promptulate-1.0.2/promptulate/frameworks/self_ask/__init__.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/llms/__init__.py` & `promptulate-1.0.2/promptulate/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/llms/base.py` & `promptulate-1.0.2/promptulate/llms/base.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/llms/openai.py` & `promptulate-1.0.2/promptulate/llms/openai.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/memory/__init__.py` & `promptulate-1.0.2/promptulate/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/memory/base.py` & `promptulate-1.0.2/promptulate/memory/base.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/memory/buffer.py` & `promptulate-1.0.2/promptulate/memory/buffer.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/memory/local_cache.py` & `promptulate-1.0.2/promptulate/memory/local_cache.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/preset_roles/__init__.py` & `promptulate-1.0.2/promptulate/preset_roles/__init__.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/preset_roles/prompt.py` & `promptulate-1.0.2/promptulate/preset_roles/prompt.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/preset_roles/roles.py` & `promptulate-1.0.2/promptulate/preset_roles/roles.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/provider/__init__.py` & `promptulate-1.0.2/promptulate/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/provider/mixins.py` & `promptulate-1.0.2/promptulate/provider/mixins.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/schema.py` & `promptulate-1.0.2/promptulate/schema.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/tips.py` & `promptulate-1.0.2/promptulate/tips.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/tools/__init__.py` & `promptulate-1.0.2/promptulate/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/tools/duckduckgo.py` & `promptulate-1.0.2/promptulate/tools/duckduckgo.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/utils/__init__.py` & `promptulate-1.0.2/promptulate/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/utils/_utils.py` & `promptulate-1.0.2/promptulate/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/utils/logger.py` & `promptulate-1.0.2/promptulate/utils/logger.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/utils/proxy.py` & `promptulate-1.0.2/promptulate/utils/proxy.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate/utils/singleton.py` & `promptulate-1.0.2/promptulate/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.0.1/promptulate.egg-info/PKG-INFO` & `promptulate-1.0.2/promptulate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptulate
-Version: 1.0.1
+Version: 1.0.2
 Summary: A powerful LLM Prompt Layer frameworks
 Home-page: https://github.com/Undertone0809/promptulate
 Author: Zeeland
 Author-email: zeeland@foxmail.com
 License: Apache 2.0
 Keywords: promptulate,prompt-me,prompt,chatgpt,gpt,chatbot,llm
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `promptulate-1.0.1/promptulate.egg-info/SOURCES.txt` & `promptulate-1.0.2/promptulate.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 promptulate/config.py
 promptulate/schema.py
 promptulate/tips.py
 promptulate.egg-info/PKG-INFO
 promptulate.egg-info/SOURCES.txt
 promptulate.egg-info/dependency_links.txt
 promptulate.egg-info/entry_points.txt
+promptulate.egg-info/requires.txt
 promptulate.egg-info/top_level.txt
 promptulate/command/__init__.py
 promptulate/command/chat.py
 promptulate/frameworks/__init__.py
 promptulate/frameworks/prompt.py
 promptulate/frameworks/schema.py
 promptulate/frameworks/base/__init__.py
```

### Comparing `promptulate-1.0.1/setup.py` & `promptulate-1.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,22 +16,23 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="promptulate",
-    version="1.0.1",
+    version="1.0.2",
     author="Zeeland",
     author_email="zeeland@foxmail.com",
     description="A powerful LLM Prompt Layer frameworks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Undertone0809/promptulate",
     packages=setuptools.find_packages(),
+    install_requires=['cushy-storage', 'pydantic', 'requests'],
     license="Apache 2.0",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

