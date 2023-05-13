# Comparing `tmp/plugnplai-0.0.5.tar.gz` & `tmp/plugnplai-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugnplai-0.0.5.tar", max compression
+gzip compressed data, was "plugnplai-0.0.6.tar", max compression
```

## Comparing `plugnplai-0.0.5.tar` & `plugnplai-0.0.6.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-04-25 18:31:47.487043 plugnplai-0.0.5/LICENSE
--rw-r--r--   0        0        0     1935 2023-05-04 06:13:47.475045 plugnplai-0.0.5/README.md
--rw-r--r--   0        0        0      466 2023-04-25 18:31:47.503043 plugnplai-0.0.5/plugnplai/__init__.py
--rw-r--r--   0        0        0     4889 2023-04-25 18:31:47.504043 plugnplai-0.0.5/plugnplai/call_api.py
--rw-r--r--   0        0        0     5599 2023-05-04 06:15:01.990050 plugnplai-0.0.5/plugnplai/load.py
--rw-r--r--   0        0        0     5755 2023-04-25 18:31:47.510043 plugnplai-0.0.5/plugnplai/plugin.py
--rw-r--r--   0        0        0      400 2023-05-04 06:17:03.779060 plugnplai-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2512 1970-01-01 00:00:00.000000 plugnplai-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-06 15:09:14.157127 plugnplai-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1943 2023-05-06 15:09:53.922130 plugnplai-0.0.6/README.md
+-rw-r--r--   0        0        0      536 2023-05-07 01:14:27.562759 plugnplai-0.0.6/plugnplai/__init__.py
+-rw-r--r--   0        0        0     4889 2023-05-06 15:09:14.167127 plugnplai-0.0.6/plugnplai/call_api.py
+-rw-r--r--   0        0        0     2533 2023-05-07 01:49:00.904915 plugnplai-0.0.6/plugnplai/embeddings.py
+-rw-r--r--   0        0        0     5590 2023-05-07 01:01:39.922701 plugnplai-0.0.6/plugnplai/load.py
+-rw-r--r--   0        0        0     5753 2023-05-07 01:01:39.923701 plugnplai-0.0.6/plugnplai/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-07 01:02:14.288703 plugnplai-0.0.6/plugnplai/prompt.py
+-rw-r--r--   0        0        0      483 2023-05-07 01:56:01.656947 plugnplai-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2690 1970-01-01 00:00:00.000000 plugnplai-0.0.6/PKG-INFO
```

### Comparing `plugnplai-0.0.5/LICENSE` & `plugnplai-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `plugnplai-0.0.5/README.md` & `plugnplai-0.0.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -38,18 +38,18 @@
 urls = plugnplai.get_plugins(filter = 'ChatGPT')
 
 #  Get working plugins - only tested plugins (in progress)
 urls = plugnplai.get_plugins(filter = 'working')
 
 
 # Get the Manifest and the OpenAPI specification from the plugin URL 
-manifest, openapi_spec = spec_from_url(plugins[0])
+manifest, openapi_spec = plugnplai.spec_from_url(urls[0])
 ```
 
 ## Contributing
 
 Plug and Plai is an open source library, and we welcome contributions from the entire community. If you're interested in contributing to the project, please feel free to fork, submit pull requests, report issues, or suggest new features.
 
 ## Links
 
-- Plugins directory: [https://plugplai.com/](https://plugplai.com/)
-- API reference: [https://plugnplai.github.io/](https://plugnplai.github.io/)
+- Plugins directory: [https://plugnplai.com/](https://plugnplai.com/)
+- API reference: [https://plugnplai.github.io/](https://plugnplai.github.io/)
```

### Comparing `plugnplai-0.0.5/plugnplai/call_api.py` & `plugnplai-0.0.6/plugnplai/call_api.py`

 * *Files identical despite different names*

### Comparing `plugnplai-0.0.5/plugnplai/load.py` & `plugnplai-0.0.6/plugnplai/load.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 import os
 
 import jsonref
 import requests
 import yaml
 
 
-def get_plugins(
-    filter: str = None, provider: str = "plugnplai"
-):
+def get_plugins(filter: str = None, provider: str = "plugnplai"):
     if provider == "plugnplai":
         base_url = "https://www.plugnplai.com/_functions/getUrls"
         # Construct the endpoint URL based on the filter argument
         if filter in ["working", "ChatGPT"]:
             url = f'{base_url.strip("/")}/{filter}'
         else:
             url = base_url
@@ -25,20 +23,21 @@
         else:
             # Handle unsuccessful responses
             return f"An error occurred: {response.status_code} {response.reason}"
     elif provider == "pluginso":
         url = "https://plugin.so/api/plugins/list"
         response = requests.get(url)
         if response.status_code == 200:
-                # Parse the JSON response and return the result
+            # Parse the JSON response and return the result
             return [f"https://{entry['domain']}" for entry in response.json()]
         else:
             # Handle unsuccessful responses
             return f"An error occurred: {response.status_code} {response.reason}"
 
+
 # given a plugin url, get the ai-plugin.json manifest, in "/.well-known/ai-plugin.json"
 def get_plugin_manifest(url: str):
     urlJson = os.path.join(url, ".well-known/ai-plugin.json")
     response = requests.get(urlJson).json()
     return response
```

### Comparing `plugnplai-0.0.5/plugnplai/plugin.py` & `plugnplai-0.0.6/plugnplai/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,14 @@
 
     #     method_schema = f"\noperationId {info['operationId']} = ({parametersStr}) => any"
 
     #     prompt_description += method_schema
 
 
 class Plugin(BaseModel):
-
     name: str
     url: str
     description_for_model: str
     plugin_json: PluginJson
     prompt: str
     api_spec: dict
 
@@ -161,15 +160,14 @@
         prefix_prompt += "\n\n// Plugin " + str(n) + ":\n\n"
         prefix_prompt += plugin.prompt
         n += 1
     return prefix_prompt
 
 
 class InstallPlugins(BaseModel):
-
     Plugins: list
     Prompt: str
 
     @classmethod
     def from_urls_list(cls, urls: list) -> list:
         """Load the plugins from list."""
```

### Comparing `plugnplai-0.0.5/PKG-INFO` & `plugnplai-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: plugnplai
-Version: 0.0.5
+Version: 0.0.6
 Summary: Connect plugins to AI
 License: MIT
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0)
 Requires-Dist: jsonref (>=1.1.0,<2.0.0)
+Requires-Dist: langchain (>=0.0.160,<0.0.161)
+Requires-Dist: openai (>=0.27.6,<0.28.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
 Description-Content-Type: text/markdown
 
 # 🎸 Plug and Plai
 
 Plug and Plai is an open source library aiming to simplify the integration of AI plugins into open-source language models (LLMs). 
 
 It provides utility functions to get a list of active plugins from [plugnplai.com](https://plugnplai.com/) directory, get plugin manifests, and extract OpenAPI specifications and load plugins.
@@ -55,19 +59,18 @@
 urls = plugnplai.get_plugins(filter = 'ChatGPT')
 
 #  Get working plugins - only tested plugins (in progress)
 urls = plugnplai.get_plugins(filter = 'working')
 
 
 # Get the Manifest and the OpenAPI specification from the plugin URL 
-manifest, openapi_spec = spec_from_url(plugins[0])
+manifest, openapi_spec = plugnplai.spec_from_url(urls[0])
 ```
 
 ## Contributing
 
 Plug and Plai is an open source library, and we welcome contributions from the entire community. If you're interested in contributing to the project, please feel free to fork, submit pull requests, report issues, or suggest new features.
 
 ## Links
 
-- Plugins directory: [https://plugplai.com/](https://plugplai.com/)
+- Plugins directory: [https://plugnplai.com/](https://plugnplai.com/)
 - API reference: [https://plugnplai.github.io/](https://plugnplai.github.io/)
-
```

