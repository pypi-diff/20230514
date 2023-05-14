# Comparing `tmp/fastapi_async_langchain-0.5.4.tar.gz` & `tmp/fastapi_async_langchain-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_async_langchain-0.5.4.tar", max compression
+gzip compressed data, was "fastapi_async_langchain-0.5.5.tar", max compression
```

## Comparing `fastapi_async_langchain-0.5.4.tar` & `fastapi_async_langchain-0.5.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1073 2023-05-13 11:31:36.433893 fastapi_async_langchain-0.5.4/LICENSE
--rw-r--r--   0        0        0     2938 2023-05-13 11:31:36.433893 fastapi_async_langchain-0.5.4/README.md
--rw-r--r--   0        0        0        0 2023-05-13 11:31:36.621895 fastapi_async_langchain-0.5.4/fastapi_async_langchain/__init__.py
--rw-r--r--   0        0        0     2326 2023-05-13 11:31:36.621895 fastapi_async_langchain-0.5.4/fastapi_async_langchain/callbacks/__init__.py
--rw-r--r--   0        0        0      956 2023-05-13 11:31:36.621895 fastapi_async_langchain-0.5.4/fastapi_async_langchain/callbacks/base.py
--rw-r--r--   0        0        0     1389 2023-05-13 11:31:36.621895 fastapi_async_langchain-0.5.4/fastapi_async_langchain/callbacks/llm.py
--rw-r--r--   0        0        0     2704 2023-05-13 11:31:36.621895 fastapi_async_langchain-0.5.4/fastapi_async_langchain/callbacks/qa_with_sources.py
--rw-r--r--   0        0        0     2882 2023-05-13 11:31:36.621895 fastapi_async_langchain-0.5.4/fastapi_async_langchain/callbacks/retrieval_qa.py
--rw-r--r--   0        0        0     1332 2023-05-13 11:31:36.621895 fastapi_async_langchain-0.5.4/fastapi_async_langchain/register.py
--rw-r--r--   0        0        0       74 2023-05-13 11:31:36.621895 fastapi_async_langchain-0.5.4/fastapi_async_langchain/responses/__init__.py
--rw-r--r--   0        0        0     2787 2023-05-13 11:31:36.621895 fastapi_async_langchain-0.5.4/fastapi_async_langchain/responses/streaming.py
--rw-r--r--   0        0        0      536 2023-05-13 11:31:36.621895 fastapi_async_langchain-0.5.4/fastapi_async_langchain/schemas.py
--rw-r--r--   0        0        0       69 2023-05-13 11:31:36.621895 fastapi_async_langchain-0.5.4/fastapi_async_langchain/testing/__init__.py
--rw-r--r--   0        0        0     3212 2023-05-13 11:31:36.621895 fastapi_async_langchain-0.5.4/fastapi_async_langchain/testing/gradio.py
--rw-r--r--   0        0        0      391 2023-05-13 11:31:36.621895 fastapi_async_langchain-0.5.4/fastapi_async_langchain/testing/settings.py
--rw-r--r--   0        0        0       73 2023-05-13 11:31:36.621895 fastapi_async_langchain-0.5.4/fastapi_async_langchain/websockets/__init__.py
--rw-r--r--   0        0        0     3661 2023-05-13 11:31:36.621895 fastapi_async_langchain-0.5.4/fastapi_async_langchain/websockets/base.py
--rw-r--r--   0        0        0      766 2023-05-13 11:31:36.621895 fastapi_async_langchain-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     3778 1970-01-01 00:00:00.000000 fastapi_async_langchain-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-14 15:24:02.709795 fastapi_async_langchain-0.5.5/LICENSE
+-rw-r--r--   0        0        0     3102 2023-05-14 15:24:02.709795 fastapi_async_langchain-0.5.5/README.md
+-rw-r--r--   0        0        0      304 2023-05-14 15:24:02.893800 fastapi_async_langchain-0.5.5/fastapi_async_langchain/__init__.py
+-rw-r--r--   0        0        0     2326 2023-05-14 15:24:02.893800 fastapi_async_langchain-0.5.5/fastapi_async_langchain/callbacks/__init__.py
+-rw-r--r--   0        0        0      956 2023-05-14 15:24:02.893800 fastapi_async_langchain-0.5.5/fastapi_async_langchain/callbacks/base.py
+-rw-r--r--   0        0        0     1389 2023-05-14 15:24:02.893800 fastapi_async_langchain-0.5.5/fastapi_async_langchain/callbacks/llm.py
+-rw-r--r--   0        0        0     2704 2023-05-14 15:24:02.893800 fastapi_async_langchain-0.5.5/fastapi_async_langchain/callbacks/qa_with_sources.py
+-rw-r--r--   0        0        0     2882 2023-05-14 15:24:02.893800 fastapi_async_langchain-0.5.5/fastapi_async_langchain/callbacks/retrieval_qa.py
+-rw-r--r--   0        0        0     1332 2023-05-14 15:24:02.893800 fastapi_async_langchain-0.5.5/fastapi_async_langchain/register.py
+-rw-r--r--   0        0        0       74 2023-05-14 15:24:02.893800 fastapi_async_langchain-0.5.5/fastapi_async_langchain/responses/__init__.py
+-rw-r--r--   0        0        0     2787 2023-05-14 15:24:02.893800 fastapi_async_langchain-0.5.5/fastapi_async_langchain/responses/streaming.py
+-rw-r--r--   0        0        0      536 2023-05-14 15:24:02.893800 fastapi_async_langchain-0.5.5/fastapi_async_langchain/schemas.py
+-rw-r--r--   0        0        0       69 2023-05-14 15:24:02.893800 fastapi_async_langchain-0.5.5/fastapi_async_langchain/testing/__init__.py
+-rw-r--r--   0        0        0     3212 2023-05-14 15:24:02.893800 fastapi_async_langchain-0.5.5/fastapi_async_langchain/testing/gradio.py
+-rw-r--r--   0        0        0      391 2023-05-14 15:24:02.893800 fastapi_async_langchain-0.5.5/fastapi_async_langchain/testing/settings.py
+-rw-r--r--   0        0        0       73 2023-05-14 15:24:02.893800 fastapi_async_langchain-0.5.5/fastapi_async_langchain/websockets/__init__.py
+-rw-r--r--   0        0        0     3661 2023-05-14 15:24:02.893800 fastapi_async_langchain-0.5.5/fastapi_async_langchain/websockets/base.py
+-rw-r--r--   0        0        0      766 2023-05-14 15:24:02.893800 fastapi_async_langchain-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     3942 1970-01-01 00:00:00.000000 fastapi_async_langchain-0.5.5/PKG-INFO
```

### Comparing `fastapi_async_langchain-0.5.4/LICENSE` & `fastapi_async_langchain-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.5.4/README.md` & `fastapi_async_langchain-0.5.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # fastapi-async-langchain
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/ajndkr/fastapi-async-langchain/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/fastapi-async-langchain.svg)](https://pypi.org/project/fastapi-async-langchain/)
 
+> ⚠️ DISCLAIMER: `fastapi-async-langchain` has been deprecated in favor of `lanarky`. You can find the PyPI project [here](https://pypi.org/project/lanarky/).
+
 Ship production-ready [LangChain](https://github.com/hwchase17/langchain) projects with
 [FastAPI](https://github.com/tiangolo/fastapi).
 
 ## 🚀 Features
 
 - supports token streaming over HTTP and Websocket
 - supports multiple langchain `Chain` types
```

### Comparing `fastapi_async_langchain-0.5.4/fastapi_async_langchain/callbacks/__init__.py` & `fastapi_async_langchain-0.5.5/fastapi_async_langchain/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.5.4/fastapi_async_langchain/callbacks/base.py` & `fastapi_async_langchain-0.5.5/fastapi_async_langchain/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.5.4/fastapi_async_langchain/callbacks/llm.py` & `fastapi_async_langchain-0.5.5/fastapi_async_langchain/callbacks/llm.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.5.4/fastapi_async_langchain/callbacks/qa_with_sources.py` & `fastapi_async_langchain-0.5.5/fastapi_async_langchain/callbacks/qa_with_sources.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.5.4/fastapi_async_langchain/callbacks/retrieval_qa.py` & `fastapi_async_langchain-0.5.5/fastapi_async_langchain/callbacks/retrieval_qa.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.5.4/fastapi_async_langchain/register.py` & `fastapi_async_langchain-0.5.5/fastapi_async_langchain/register.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.5.4/fastapi_async_langchain/responses/streaming.py` & `fastapi_async_langchain-0.5.5/fastapi_async_langchain/responses/streaming.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.5.4/fastapi_async_langchain/schemas.py` & `fastapi_async_langchain-0.5.5/fastapi_async_langchain/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.5.4/fastapi_async_langchain/testing/gradio.py` & `fastapi_async_langchain-0.5.5/fastapi_async_langchain/testing/gradio.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.5.4/fastapi_async_langchain/websockets/base.py` & `fastapi_async_langchain-0.5.5/fastapi_async_langchain/websockets/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.5.4/pyproject.toml` & `fastapi_async_langchain-0.5.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-async-langchain"
-version = "0.5.4"
+version = "0.5.5"
 description = "Ship production-ready LangChain projects with FastAPI"
 authors = ["Ajinkya Indulkar <26824103+ajndkr@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/ajndkr/fastapi-async-langchain"
 repository = "https://github.com/ajndkr/fastapi-async-langchain"
 license = "MIT"
 packages = [{include = "fastapi_async_langchain"}]
```

### Comparing `fastapi_async_langchain-0.5.4/PKG-INFO` & `fastapi_async_langchain-0.5.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-async-langchain
-Version: 0.5.4
+Version: 0.5.5
 Summary: Ship production-ready LangChain projects with FastAPI
 Home-page: https://github.com/ajndkr/fastapi-async-langchain
 License: MIT
 Author: Ajinkya Indulkar
 Author-email: 26824103+ajndkr@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -20,14 +20,16 @@
 Description-Content-Type: text/markdown
 
 # fastapi-async-langchain
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/ajndkr/fastapi-async-langchain/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/fastapi-async-langchain.svg)](https://pypi.org/project/fastapi-async-langchain/)
 
+> ⚠️ DISCLAIMER: `fastapi-async-langchain` has been deprecated in favor of `lanarky`. You can find the PyPI project [here](https://pypi.org/project/lanarky/).
+
 Ship production-ready [LangChain](https://github.com/hwchase17/langchain) projects with
 [FastAPI](https://github.com/tiangolo/fastapi).
 
 ## 🚀 Features
 
 - supports token streaming over HTTP and Websocket
 - supports multiple langchain `Chain` types
```

