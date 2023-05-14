# Comparing `tmp/embedbase-1.1.4.tar.gz` & `tmp/embedbase-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase-1.1.4.tar", max compression
+gzip compressed data, was "embedbase-1.1.5.tar", max compression
```

## Comparing `embedbase-1.1.4.tar` & `embedbase-1.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1069 2023-05-03 14:41:13.518171 embedbase-1.1.4/LICENSE
--rw-r--r--   0        0        0     6149 2023-05-03 14:41:13.518171 embedbase-1.1.4/README.md
--rw-r--r--   0        0        0      121 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/__init__.py
--rw-r--r--   0        0        0     1658 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/__main__.py
--rw-r--r--   0        0        0      976 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/api.py
--rw-r--r--   0        0        0    16357 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/app.py
--rw-r--r--   0        0        0       88 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/database/__init__.py
--rw-r--r--   0        0        0     3505 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/database/base.py
--rw-r--r--   0        0        0     5939 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/database/memory_db.py
--rw-r--r--   0        0        0     9702 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/database/postgres_db.py
--rw-r--r--   0        0        0     6620 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/database/supabase_db.py
--rw-r--r--   0        0        0       77 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/embedding/__init__.py
--rw-r--r--   0        0        0      858 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/embedding/base.py
--rw-r--r--   0        0        0     1237 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/embedding/cohere.py
--rw-r--r--   0        0        0     2059 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/embedding/openai.py
--rw-r--r--   0        0        0     1551 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/firebase_auth.py
--rw-r--r--   0        0        0      690 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/logging_utils.py
--rw-r--r--   0        0        0      802 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/models.py
--rw-r--r--   0        0        0     1285 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/settings.py
--rw-r--r--   0        0        0     3208 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/strings.py
--rw-r--r--   0        0        0      301 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/supabase_auth.py
--rw-r--r--   0        0        0     3867 2023-05-03 14:41:13.590168 embedbase-1.1.4/embedbase/utils.py
--rw-r--r--   0        0        0     3669 2023-05-03 14:41:13.594168 embedbase-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     7587 1970-01-01 00:00:00.000000 embedbase-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-14 08:01:24.202878 embedbase-1.1.5/LICENSE
+-rw-r--r--   0        0        0     4905 2023-05-14 08:01:24.202878 embedbase-1.1.5/README.md
+-rw-r--r--   0        0        0      121 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/__init__.py
+-rw-r--r--   0        0        0     1646 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/__main__.py
+-rw-r--r--   0        0        0      976 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/api.py
+-rw-r--r--   0        0        0    16416 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/app.py
+-rw-r--r--   0        0        0       88 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/database/__init__.py
+-rw-r--r--   0        0        0     3505 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/database/base.py
+-rw-r--r--   0        0        0     5939 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/database/memory_db.py
+-rw-r--r--   0        0        0     9702 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/database/postgres_db.py
+-rw-r--r--   0        0        0     6620 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/database/supabase_db.py
+-rw-r--r--   0        0        0       77 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/embedding/__init__.py
+-rw-r--r--   0        0        0      858 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/embedding/base.py
+-rw-r--r--   0        0        0     1237 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/embedding/cohere.py
+-rw-r--r--   0        0        0     2059 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/embedding/openai.py
+-rw-r--r--   0        0        0     1551 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/firebase_auth.py
+-rw-r--r--   0        0        0      690 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/logging_utils.py
+-rw-r--r--   0        0        0      802 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/models.py
+-rw-r--r--   0        0        0     1285 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/settings.py
+-rw-r--r--   0        0        0     3208 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/strings.py
+-rw-r--r--   0        0        0      301 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/supabase_auth.py
+-rw-r--r--   0        0        0     3867 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/utils.py
+-rw-r--r--   0        0        0     3669 2023-05-14 08:01:24.270878 embedbase-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     6343 1970-01-01 00:00:00.000000 embedbase-1.1.5/PKG-INFO
```

### Comparing `embedbase-1.1.4/LICENSE` & `embedbase-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.4/README.md` & `embedbase-1.1.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,102 +1,83 @@
+Metadata-Version: 2.1
+Name: embedbase
+Version: 1.1.5
+Summary: API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings.
+Home-page: https://github.com/different-ai/embedbase
+License: MIT
+Keywords: embeddings,machine learning,artificial intelligence
+Author: Different AI
+Author-email: louis@embedbase.xyz
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Dist: fastapi (>=0.95.1,<0.96.0)
+Requires-Dist: openai (>=0.27.0,<0.28.0)
+Requires-Dist: pandas (>=1.3.4,<2.0.0)
+Requires-Dist: pydantic_yaml[pyyaml] (>=0.4.0,<0.5.0)
+Requires-Dist: tenacity (>=8.0.1,<9.0.0)
+Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
+Requires-Dist: uvicorn[standard] (>=0.15.0,<0.16.0)
+Project-URL: Repository, https://github.com/different-ai/embedbase
+Description-Content-Type: text/markdown
+
 <br />
 
 
 <p align="center">
 <img width="150" alt="embedbasevector" src="https://user-images.githubusercontent.com/11430621/223136025-14572cac-f2aa-455c-936b-a48cb35a0c57.png">
   <h1 align="center">Embedbase</h1>
 
 
-<h3 align="center">Seamless data connections to LLMs</h3>
+<h3 align="center">Seamless data integration for LLMs</h3>
 
   <p align="center">
     <br />
     <a href="https://discord.gg/pMNeuGrDky"><img alt="Discord" src="https://img.shields.io/discord/1066022656845025310?color=black&style=for-the-badge"></a>
     <a href="https://badge.fury.io/py/embedbase"><img alt="PyPI" src="https://img.shields.io/pypi/v/embedbase?color=black&style=for-the-badge"></a>
     <br />
-    <a href="https://render.com/deploy?repo=https://github.com/different-ai/embedbase-render">
-      <img src="https://render.com/images/deploy-to-render-button.svg" alt="Deploy to Render">
-    </a>
-    <br />
-    <a href="https://replit.com/@benjaminshafii/Embedbase-Quickstart-JS?v=1">
-      <img src="https://replit.com/badge?caption=Try%20with%20Replit" alt="Try with Replit Badge">
-    </a>
-    <br />
     <a target="_blank" href="https://colab.research.google.com/github/different-ai/embedbase/blob/main/notebooks/Embedbase_Getting_started.ipynb">
       <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
     </a>
-    <p align="center">Open-source API & SDK to sync your data and easily hook them up to LLMs</p>
+    <p align="center">Open-source API & SDK to integrate your data and easily hook them up to LLMs</p>
     <p align="center">Used by <a href="https://github.com/louis030195/obsidian-ava">AVA</a> and serving 100k request a day</p>
     <div align="center">
-      <a href="https://app.embedbase.xyz/signup">Try Embedbase Cloud now</a>
+      <a href="https://app.embedbase.xyz/signup">Try the Hosted Version</a>
       ·
       <a href="https://github.com/different-ai/embedbase/issues/new?assignees=&labels=enhancement">Request Feature</a>
       ·
       <a href="https://github.com/different-ai/embedbase/issues/new?assignees=&labels=bug">Report Bug</a>
     </div>
     <br />
   </p>
 </p>
 
 Check out the [docs](https://docs.embedbase.xyz) for more info.
 
+## What is it
 
-## Table of Contents
-
-- [Getting started](#getting-started)
-- [Javascript SDK](#sdk)
-- [Docs and support](#docs-and-support)
-- [Contributing](#contributing)
-
-## The 3 ways to use Embedbase
-
-- [Embedbase Cloud](#managed-instance): **Build embeddings-powered apps in minutes** | `npm i embedbase-js` | ⏱️ 3min
-- [Embedbase.py](#getting-started): **Choose your own db, embeddings models, and get started with a simple** | `pip install embedbase` | ⏱️ 5 min
-- [Embedbase self-hosted](https://docs.embedbase.xyz/tutorials/self-host-on-render): **Get Embedbase Cloud on your infra** | `docker-compose up` | ⏱️ 15 min
-
-
-## What are people building
-
-- [Recommendation Engines: AVA uses Embedbase to help their users find related notes](https://github.com/louis030195/obsidian-ava)
-- [Chat with your data: Solpilot uses Embedbase to put smart contract integration on autopilot](https://solpilot.xyz/chat)
-- [Talk to your docs: ChatGPT-powered search for markdown documentation](https://github.com/different-ai/chat-gpt-powered-nextra)
-
-## Getting started
-
-Let's install Python dependencies:
-
-```bash
-pip install embedbase sentence-transformers
-```
-
-Run a local-first instance of Embedbase:
-
-```bash
-embedbase run
-```
-
-![pika-1681921124330-1x](https://user-images.githubusercontent.com/25003283/233138132-cf42ec0f-3821-495f-8e29-2067e643d6db.png)
-
-🔥 Embedbase now runs! [Look here to see how to use the sdk](#sdk)
-
-ℹ️ Look at the code you just ran [here](./embedbase/__main__.py), feel free to modify it to your needs.
-
-### Managed Instance
-
-The fastest way to get started with Embedbase is signing up for free to [Embedbase Cloud](https://app.embedbase.xyz/).
-
-![Dashboard Screenshot](https://user-images.githubusercontent.com/11430621/227351386-f540fac0-c5fa-485a-bcc9-f23368fe3f63.png)
-
-
-## How to use 
-### SDK
+Embedbase is a dead-simple API to help you use [VectorDBs](https://learn.microsoft.com/en-us/semantic-kernel/concepts-ai/vectordb) and [Embeddings Models](https://en.wikipedia.org/wiki/Sentence_embedding#:~:text=Sentence%20embedding%20is%20the%20collective,to%20vectors%20of%20real%20numbers.) without needing to host them!
+You can use embedbase to customize LLM (like ChatGPT!) and automatically feed them the right information.
 
+## Installation
 `npm i embedbase-js`
 
 ```js
+// this examples shows how you can use embedbase to automatically add context in a ChatGPT prompt
 import { createClient } from 'embedbase-js'
 
 const question = 'What can I do with Embedbase API?'
 
 const embedbase = createClient(
   'https://api.embedbase.xyz',
   'api-key')
@@ -117,70 +98,70 @@
   `Write a response to question: ${question} 
   based on the follwing context ${context.toString()}`
 )
 // answer:
 // You can use the Embedbase API to store unstructured data and then use the data to connect it to LLMs
 ```
 
+## Table of Contents
 
+- [Getting started](#getting-started)
+- [Javascript SDK](#sdk)
+- [Docs and support](#docs-and-support)
+- [Integrations](#our-integrations)
+- [Contributing](#contributing)
 
-### Inserting data
 
-```ts
-const URL = 'http://localhost:8000'
-const VAULT_ID = 'people'
-// if using the hosted version
-const API_KEY = '<https://app.embedbase.xyz/signup>'
-fetch(`${URL}/v1/${VAULT_ID}`, {
-    method: 'POST',
-    headers: {
-      'Content-Type': 'application/json',
-      // if using the hosted version, uncomment
-      // 'Authorization': `Bearer ${API_KEY}`
-    },
-    body: JSON.stringify({
-      documents: [{
-        data: 'Elon is sipping a tea on Mars',
-      }],
-    }),
-  });
-```
+## What are people building
 
-### Searching
+- [Recommendation Engines: AVA uses Embedbase to help their users find related notes](https://github.com/louis030195/obsidian-ava)
+- [Chat with your data: Solpilot uses Embedbase to put smart contract integration on autopilot](https://app.solpilot.xyz/chat)
+- [Talk to your docs: ChatGPT-powered search for markdown documentation](https://github.com/different-ai/chat-gpt-powered-nextra)
+
+
+
+The fastest way to get started with Embedbase is signing up for free to [Embedbase Cloud](https://app.embedbase.xyz/).
+
+![Dashboard Screenshot](https://user-images.githubusercontent.com/11430621/227351386-f540fac0-c5fa-485a-bcc9-f23368fe3f63.png)
+
+
+
+## Supported Integrations
+
+### Connections
+- [x] Any data with the sdk or api
+- [x] PDF
+- [ ] Github
+
+### Vector DBs
+- [x] Supabase
+- [x] Postgres
+- [x] Qdrant
+- [ ] Weaviate
+- [ ] Redix
+
+### Embedding Models
+- [x] OpenAI Embeddings
+- [x] sentence-transformers
+- [ ] T5
 
-```ts
-fetch(`${URL}/v1/${VAULT_ID}/search`, {
-    method: 'POST',
-    headers: {
-      'Content-Type': 'application/json',
-      // 'Authorization': `Bearer ${API_KEY}`
-    },
-    body: JSON.stringify({
-      query: 'Something about a red planet',
-    }),
-  });
-```
 
-Result:
 
-```json
-{
-  "query": "Something about a red planet",
-  "similarities": [
-    {
-      "score": 0.828773,
-      "id": "ABCU75FEBE",
-      "data": "Elon is sipping a tea on Mars",
-    }
-  ]
-}
-```
 
 ## Docs and support
 
 Check out our [tutorials](https://docs.embedbase.xyz) for step-by-step guides, how-to's, and best practices, our documentation is powered by GPT-4, so you can ask question directly. 
 
 Ask a question in our [Discord community](https://discord.gg/pMNeuGrDky) to get support.
 
 ## Contributing
 
 Please read [CONTRIBUTING.md](./CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
+
+## Self-hosting
+
+> Note: this render configuration works well for experimentation. 
+
+<a href="https://render.com/deploy?repo=https://github.com/different-ai/embedbase-render">
+      <img src="https://render.com/images/deploy-to-render-button.svg" alt="Deploy to Render">
+</a>
+
```

### Comparing `embedbase-1.1.4/embedbase/__main__.py` & `embedbase-1.1.5/embedbase/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,12 +43,12 @@
 
 
 app = get_app().use_db(MemoryDatabase()).use_embedder(LocalEmbedder()).run()
 
 
 # pylint: disable=missing-function-docstring
 def run_app():
-    uvicorn.run("embedbase:app", host="0.0.0.0")
+    uvicorn.run(app, host="0.0.0.0")
 
 
 if __name__ == "__main__":
     run_app()
```

### Comparing `embedbase-1.1.4/embedbase/api.py` & `embedbase-1.1.5/embedbase/api.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.4/embedbase/app.py` & `embedbase-1.1.5/embedbase/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
 import os
-from typing import Awaitable, Callable, Optional, Tuple, Union
+from typing import Awaitable, Callable, Optional, Tuple, Union, Any
 from fastapi import FastAPI, Request, status
 from fastapi.middleware import Middleware
 from starlette.types import Scope
 from embedbase.database.base import VectorDatabase
 from embedbase.embedding.base import Embedder
 from embedbase.logging_utils import get_logger
 from embedbase.models import (
@@ -62,30 +62,30 @@
         self.embedder = embedder
         return self
 
     def use_middleware(
         self,
         plugin: Union[
             Middleware,
-            Callable[[Scope], Awaitable[Tuple[str, str]]],
+            Callable[[Scope, Any, VectorDatabase, Embedder], Awaitable[Tuple[str, str]]],
         ],
         **kwargs,
     ) -> "Embedbase":
         """
         Use the chosen middleware.
         """
         if asyncio.iscoroutinefunction(plugin):
             self.logger.info(f"Enabling Middleware {plugin}")
 
             @self.fastapi_app.middleware("http")
             async def middleware(request: Request, call_next):
-                return await plugin(request, call_next)
+                return await plugin(request, call_next, self.db, self.embedder)
 
         elif "CORSMiddleware" in str(plugin):
-            self.logger.info(f"Enabling CORSMiddleware")
+            self.logger.info("Enabling CORSMiddleware")
             self.fastapi_app.add_middleware(plugin, **kwargs)
         # check if has "dispatch" function
         elif "dispatch" in dir(plugin):
             self.logger.info(f"Enabling Middleware {plugin}")
             self.fastapi_app.add_middleware(plugin)
         else:
             warnings.warn(f"Plugin {plugin} is not supported")
```

### Comparing `embedbase-1.1.4/embedbase/database/base.py` & `embedbase-1.1.5/embedbase/database/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.4/embedbase/database/memory_db.py` & `embedbase-1.1.5/embedbase/database/memory_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.4/embedbase/database/postgres_db.py` & `embedbase-1.1.5/embedbase/database/postgres_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.4/embedbase/database/supabase_db.py` & `embedbase-1.1.5/embedbase/database/supabase_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.4/embedbase/embedding/base.py` & `embedbase-1.1.5/embedbase/embedding/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.4/embedbase/embedding/cohere.py` & `embedbase-1.1.5/embedbase/embedding/cohere.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.4/embedbase/embedding/openai.py` & `embedbase-1.1.5/embedbase/embedding/openai.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.4/embedbase/firebase_auth.py` & `embedbase-1.1.5/embedbase/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.4/embedbase/logging_utils.py` & `embedbase-1.1.5/embedbase/logging_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.4/embedbase/models.py` & `embedbase-1.1.5/embedbase/models.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.4/embedbase/settings.py` & `embedbase-1.1.5/embedbase/settings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.4/embedbase/strings.py` & `embedbase-1.1.5/embedbase/strings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.4/embedbase/utils.py` & `embedbase-1.1.5/embedbase/utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.4/pyproject.toml` & `embedbase-1.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "embedbase"
-version = "1.1.4"
+version = "1.1.5"
 description = "API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings."
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase"
 homepage = "https://github.com/different-ai/embedbase"
 keywords = ["embeddings", "machine learning", "artificial intelligence"]
```

