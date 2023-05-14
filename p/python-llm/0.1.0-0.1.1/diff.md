# Comparing `tmp/python-llm-0.1.0.tar.gz` & `tmp/python-llm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-llm-0.1.0.tar", last modified: Sat May 13 13:43:48 2023, max compression
+gzip compressed data, was "python-llm-0.1.1.tar", last modified: Sun May 14 15:46:59 2023, max compression
```

## Comparing `python-llm-0.1.0.tar` & `python-llm-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-13 13:43:48.045773 python-llm-0.1.0/
--rw-r--r--   0 danielgross   (501) staff       (20)     1069 2023-03-30 14:06:17.000000 python-llm-0.1.0/LICENSE
--rw-r--r--   0 danielgross   (501) staff       (20)      183 2023-05-13 13:43:48.045645 python-llm-0.1.0/PKG-INFO
--rw-r--r--   0 danielgross   (501) staff       (20)     1216 2023-05-13 13:41:51.000000 python-llm-0.1.0/README.md
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-13 13:43:48.044599 python-llm-0.1.0/llm/
--rw-r--r--   0 danielgross   (501) staff       (20)       56 2023-03-30 14:41:48.000000 python-llm-0.1.0/llm/__init__.py
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-13 13:43:48.044931 python-llm-0.1.0/llm/api/
--rw-r--r--   0 danielgross   (501) staff       (20)        0 2023-03-29 19:17:50.000000 python-llm-0.1.0/llm/api/__init__.py
--rw-r--r--   0 danielgross   (501) staff       (20)     1792 2023-05-13 13:35:08.000000 python-llm-0.1.0/llm/api/claude.py
--rw-r--r--   0 danielgross   (501) staff       (20)      980 2023-03-30 14:01:26.000000 python-llm-0.1.0/llm/api/openaiapi.py
--rw-r--r--   0 danielgross   (501) staff       (20)     1829 2023-05-13 13:36:58.000000 python-llm-0.1.0/llm/main.py
--rw-r--r--   0 danielgross   (501) staff       (20)     1781 2023-05-13 13:24:32.000000 python-llm-0.1.0/llm/util.py
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-13 13:43:48.045490 python-llm-0.1.0/python_llm.egg-info/
--rw-r--r--   0 danielgross   (501) staff       (20)      183 2023-05-13 13:43:48.000000 python-llm-0.1.0/python_llm.egg-info/PKG-INFO
--rw-r--r--   0 danielgross   (501) staff       (20)      294 2023-05-13 13:43:48.000000 python-llm-0.1.0/python_llm.egg-info/SOURCES.txt
--rw-r--r--   0 danielgross   (501) staff       (20)        1 2023-05-13 13:43:48.000000 python-llm-0.1.0/python_llm.egg-info/dependency_links.txt
--rw-r--r--   0 danielgross   (501) staff       (20)       17 2023-05-13 13:43:48.000000 python-llm-0.1.0/python_llm.egg-info/requires.txt
--rw-r--r--   0 danielgross   (501) staff       (20)        4 2023-05-13 13:43:48.000000 python-llm-0.1.0/python_llm.egg-info/top_level.txt
--rw-r--r--   0 danielgross   (501) staff       (20)       38 2023-05-13 13:43:48.045807 python-llm-0.1.0/setup.cfg
--rw-r--r--   0 danielgross   (501) staff       (20)      445 2023-05-13 13:43:03.000000 python-llm-0.1.0/setup.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 15:46:59.031965 python-llm-0.1.1/
+-rw-r--r--   0 danielgross   (501) staff       (20)     1069 2023-03-30 14:06:17.000000 python-llm-0.1.1/LICENSE
+-rw-r--r--   0 danielgross   (501) staff       (20)      183 2023-05-14 15:46:59.031861 python-llm-0.1.1/PKG-INFO
+-rw-r--r--   0 danielgross   (501) staff       (20)     1197 2023-05-14 15:44:12.000000 python-llm-0.1.1/README.md
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 15:46:59.030581 python-llm-0.1.1/llm/
+-rw-r--r--   0 danielgross   (501) staff       (20)       69 2023-05-13 13:51:59.000000 python-llm-0.1.1/llm/__init__.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 15:46:59.030874 python-llm-0.1.1/llm/api/
+-rw-r--r--   0 danielgross   (501) staff       (20)        0 2023-03-29 19:17:50.000000 python-llm-0.1.1/llm/api/__init__.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     2376 2023-05-14 14:49:00.000000 python-llm-0.1.1/llm/api/claude.py
+-rw-r--r--   0 danielgross   (501) staff       (20)      980 2023-03-30 14:01:26.000000 python-llm-0.1.1/llm/api/openaiapi.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     2384 2023-05-14 14:49:01.000000 python-llm-0.1.1/llm/main.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     1781 2023-05-13 13:24:32.000000 python-llm-0.1.1/llm/util.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 15:46:59.031414 python-llm-0.1.1/python_llm.egg-info/
+-rw-r--r--   0 danielgross   (501) staff       (20)      183 2023-05-14 15:46:59.000000 python-llm-0.1.1/python_llm.egg-info/PKG-INFO
+-rw-r--r--   0 danielgross   (501) staff       (20)      336 2023-05-14 15:46:59.000000 python-llm-0.1.1/python_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)        1 2023-05-14 15:46:59.000000 python-llm-0.1.1/python_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)      146 2023-05-14 15:46:59.000000 python-llm-0.1.1/python_llm.egg-info/requires.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)        4 2023-05-14 15:46:59.000000 python-llm-0.1.1/python_llm.egg-info/top_level.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)       38 2023-05-14 15:46:59.032000 python-llm-0.1.1/setup.cfg
+-rw-r--r--   0 danielgross   (501) staff       (20)      445 2023-05-14 15:46:30.000000 python-llm-0.1.1/setup.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 15:46:59.031692 python-llm-0.1.1/tests/
+-rw-r--r--   0 danielgross   (501) staff       (20)     2465 2023-05-14 15:05:09.000000 python-llm-0.1.1/tests/test_claude.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     1811 2023-05-14 15:01:48.000000 python-llm-0.1.1/tests/test_openai.py
```

### Comparing `python-llm-0.1.0/LICENSE` & `python-llm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.0/README.md` & `python-llm-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,12 @@
 # python-llm: A LLM API for Humans
 
-This is a Python wrapper for the Language Learning Models (LLM) APIs, designed to make it easy to use different language models. It supports models from OpenAI and Anthropic, with a simple and intuitive interface.
+Like python-requests but for LLMs. It supports models from OpenAI and Anthropic, with more coming soon.
 
-## Features
-
-- **Text Completion**: Complete text prompts using different language models.
-- **Chat**: Simulate a conversation with a language model.
-- **Text Embedding**: Transform text into a high-dimensional vector (not yet implemented).
-
-## Installation
-
-To install `python-llm`, use pip: ```pip install python-llm```.
+![Tests](https://github.com/danielgross/python-llm/actions/workflows/tests.yml/badge.svg)
 
 ## Usage
 
 ```python
 import llm
 
 # Completion
@@ -26,14 +18,24 @@
 
 # Embedding 
 llm.embed(open("harrypotter.txt").read())
 
 # Engines are in the provider:model format, as in openai:gpt-4, or anthropic:claude-instant-v1.
 ```
 
+## Installation
+
+To install `python-llm`, use pip: ```pip install python-llm```.
+
+## Features
+
+- **Text Completion**: Complete text prompts using different language models.
+- **Chat**: Simulate a conversation with a language model.
+- **Text Embedding**: Transform text into a high-dimensional vector (not yet implemented).
+
 ## Configuration
 You can configure the API keys for the various services using the set_api_key method:
 ```python
 llm.set_api_key(openai="sk-...", natdev="...")
 # or
 llm.set_api_key("path/to/api_keys.json")
 ```
```

### Comparing `python-llm-0.1.0/llm/api/claude.py` & `python-llm-0.1.1/llm/api/claude.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,34 @@
 import anthropic
 from llm.util import api_keys
 
 
 BASE_URL = "https://api.anthropic.com"
 
 
+def client():
+    return anthropic.Client(api_keys["anthropic"])
+
+
+def format_chat_messages(messages):
+    prompt = []
+    for message in messages:
+        if message["role"] == "user":
+            prompt.append(f"{anthropic.HUMAN_PROMPT} {message['content']}")
+        elif message["role"] == "assistant":
+            prompt.append(f"{anthropic.AI_PROMPT} {message['content']}")
+        else:
+            raise ValueError(f"Unknown role {message['role']}")
+    if messages[-1]["role"] != "user":
+        raise ValueError("Last message must be from the user.")
+    # Add a final AI prompt
+    prompt.append(anthropic.AI_PROMPT)
+    return "".join(prompt)
+
+
 def complete(prompt, engine="claude-v1", max_tokens_to_sample=10, **kwargs):
     headers = {
         "x-api-key": api_keys.get("anthropic"),
         "Content-Type": "application/json",
     }
 
     data = {
@@ -33,30 +53,32 @@
 
 
 def chat(messages, engine="claude-v1", system=None, max_tokens_to_sample=30, **kwargs):
     if system is not None:
         raise NotImplementedError(
             "System messages are not yet implemented for Claude.")
 
-    c = anthropic.Client(api_keys["anthropic"])
-    prompt = []
-    for message in messages:
-        if message["role"] == "user":
-            prompt.append(f"{anthropic.HUMAN_PROMPT} {message['content']}")
-        elif message["role"] == "assistant":
-            prompt.append(f"{anthropic.AI_PROMPT} {message['content']}")
-        else:
-            raise ValueError(f"Unknown role {message['role']}")
-    if messages[-1]["role"] != "user":
-        raise ValueError("Last message must be from the user.")
-    # Add a final AI prompt
-    prompt.append(anthropic.AI_PROMPT)
-    print(prompt)
-    prompt = "".join(prompt)
+    c = client()
+    prompt = format_chat_messages(messages)
     resp = c.completion(
         prompt=prompt,
         stop_sequences=[anthropic.HUMAN_PROMPT],
         model=engine,
         max_tokens_to_sample=max_tokens_to_sample,
         **kwargs
     )
     return resp["completion"]
+
+
+async def stream_chat(messages, engine="claude-v1", system=None, max_tokens_to_sample=30, **kwargs):
+    c = client()
+    prompt = format_chat_messages(messages)
+    response = await c.acompletion_stream(
+        prompt=prompt,
+        stop_sequences=[anthropic.HUMAN_PROMPT],
+        max_tokens_to_sample=max_tokens_to_sample,
+        model=engine,
+        stream=True,
+    )
+    async for data in response:
+        # return a generator of responses
+        yield data["completion"]
```

### Comparing `python-llm-0.1.0/llm/api/openaiapi.py` & `python-llm-0.1.1/llm/api/openaiapi.py`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.0/llm/main.py` & `python-llm-0.1.1/llm/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,24 +22,39 @@
     elif args.service == "anthropic":
         return claude.complete(prompt, args.engine, **args.kwargs)
     else:
         raise ValueError(f"Engine {engine} is not supported.")
 
 
 # Can also pass in system="Behave like a bunny rabbit" for system message.
-def chat(messages, engine="text-davinci-003", **kwargs):
+def chat(messages, engine="openai:text-davinci-003", **kwargs):
     """Chat with the LLM API."""
     args = parse_args(engine, **kwargs)
     messages = structure_chat(messages)
     if args.service == "openai":
-        return openaiapi.chat(messages, args.engine, **args.kwargs)
+        result = openaiapi.chat(messages, args.engine, **args.kwargs)
     elif args.service == "anthropic":
-        return claude.chat(messages, args.engine, **args.kwargs)
+        result = claude.chat(messages, args.engine, **args.kwargs)
     else:
         raise ValueError(f"Engine {engine} is not supported.")
+    return result.strip()
+
+
+async def stream_chat(messages, engine="text-davinci-003", **kwargs):
+    """Chat with the LLM API."""
+    args = parse_args(engine, **kwargs)
+    messages = structure_chat(messages)
+    if args.service == "openai":
+        NotImplementedError("Not implemented yet.")
+    elif args.service == "anthropic":
+        result = claude.stream_chat(messages, args.engine, **args.kwargs)
+    else:
+        raise ValueError(f"Engine {engine} is not supported.")
+    async for message in result:
+        yield message.strip()
 
 
 def embed(text, engine="text-davinci-003", **kwargs):
     """Embed text using the LLM API."""
     raise NotImplementedError("Embedding is not yet implemented.")
```

### Comparing `python-llm-0.1.0/llm/util.py` & `python-llm-0.1.1/llm/util.py`

 * *Files identical despite different names*

