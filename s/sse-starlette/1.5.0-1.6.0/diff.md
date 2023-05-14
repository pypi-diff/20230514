# Comparing `tmp/sse-starlette-1.5.0.tar.gz` & `tmp/sse-starlette-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sse-starlette-1.5.0.tar", last modified: Wed May  3 19:22:57 2023, max compression
+gzip compressed data, was "sse-starlette-1.6.0.tar", last modified: Sun May 14 08:32:32 2023, max compression
```

## Comparing `sse-starlette-1.5.0.tar` & `sse-starlette-1.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-03 19:22:57.411655 sse-starlette-1.5.0/
--rw-r--r--   0 tw         (501) staff       (20)      395 2022-11-20 19:42:25.000000 sse-starlette-1.5.0/AUTHORS
--rw-r--r--   0 tw         (501) staff       (20)     1892 2023-04-18 20:41:56.000000 sse-starlette-1.5.0/CHANGELOG.md
--rw-r--r--   0 tw         (501) staff       (20)     1511 2022-11-20 19:42:25.000000 sse-starlette-1.5.0/LICENSE
--rw-r--r--   0 tw         (501) staff       (20)      103 2022-11-20 19:42:25.000000 sse-starlette-1.5.0/MANIFEST.in
--rw-r--r--   0 tw         (501) staff       (20)     5944 2023-05-03 19:22:57.411723 sse-starlette-1.5.0/PKG-INFO
--rw-r--r--   0 tw         (501) staff       (20)     3801 2023-05-03 19:21:07.000000 sse-starlette-1.5.0/README.md
--rw-r--r--   0 tw         (501) staff       (20)      106 2022-11-20 19:42:25.000000 sse-starlette-1.5.0/pyproject.toml
--rw-r--r--   0 tw         (501) staff       (20)     1800 2023-05-03 19:22:57.412071 sse-starlette-1.5.0/setup.cfg
--rw-r--r--   0 tw         (501) staff       (20)      152 2022-11-20 19:42:25.000000 sse-starlette-1.5.0/setup.py
-drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-03 19:22:57.410791 sse-starlette-1.5.0/sse_starlette/
--rw-r--r--   0 tw         (501) staff       (20)      143 2023-05-03 19:22:35.000000 sse-starlette-1.5.0/sse_starlette/__init__.py
--rw-r--r--   0 tw         (501) staff       (20)        0 2022-11-20 19:42:25.000000 sse-starlette-1.5.0/sse_starlette/py.typed
--rw-r--r--   0 tw         (501) staff       (20)    10632 2023-05-03 19:22:52.000000 sse-starlette-1.5.0/sse_starlette/sse.py
-drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-03 19:22:57.411334 sse-starlette-1.5.0/sse_starlette.egg-info/
--rw-r--r--   0 tw         (501) staff       (20)     5944 2023-05-03 19:22:57.000000 sse-starlette-1.5.0/sse_starlette.egg-info/PKG-INFO
--rw-r--r--   0 tw         (501) staff       (20)      392 2023-05-03 19:22:57.000000 sse-starlette-1.5.0/sse_starlette.egg-info/SOURCES.txt
--rw-r--r--   0 tw         (501) staff       (20)        1 2023-05-03 19:22:57.000000 sse-starlette-1.5.0/sse_starlette.egg-info/dependency_links.txt
--rw-r--r--   0 tw         (501) staff       (20)       10 2023-05-03 19:22:57.000000 sse-starlette-1.5.0/sse_starlette.egg-info/requires.txt
--rw-r--r--   0 tw         (501) staff       (20)       14 2023-05-03 19:22:57.000000 sse-starlette-1.5.0/sse_starlette.egg-info/top_level.txt
-drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-03 19:22:57.411570 sse-starlette-1.5.0/tests/
--rw-r--r--   0 tw         (501) staff       (20)     4859 2023-05-03 19:21:13.000000 sse-starlette-1.5.0/tests/test_event_source_response.py
--rw-r--r--   0 tw         (501) staff       (20)     3028 2023-05-03 17:52:30.000000 sse-starlette-1.5.0/tests/test_sse.py
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-05-14 08:32:32.054255 sse-starlette-1.6.0/
+-rw-r--r--   0 Q187392    (501) staff       (20)      395 2022-12-16 17:29:08.000000 sse-starlette-1.6.0/AUTHORS
+-rw-r--r--   0 Q187392    (501) staff       (20)     1892 2023-03-11 18:12:47.000000 sse-starlette-1.6.0/CHANGELOG.md
+-rw-r--r--   0 Q187392    (501) staff       (20)     1511 2022-12-16 17:29:08.000000 sse-starlette-1.6.0/LICENSE
+-rw-r--r--   0 Q187392    (501) staff       (20)      103 2022-12-16 17:29:08.000000 sse-starlette-1.6.0/MANIFEST.in
+-rw-r--r--   0 Q187392    (501) staff       (20)     6520 2023-05-14 08:32:32.054348 sse-starlette-1.6.0/PKG-INFO
+-rw-r--r--   0 Q187392    (501) staff       (20)     4377 2023-05-14 08:31:06.000000 sse-starlette-1.6.0/README.md
+-rw-r--r--   0 Q187392    (501) staff       (20)      106 2022-12-16 17:29:08.000000 sse-starlette-1.6.0/pyproject.toml
+-rw-r--r--   0 Q187392    (501) staff       (20)     1800 2023-05-14 08:32:32.073549 sse-starlette-1.6.0/setup.cfg
+-rw-r--r--   0 Q187392    (501) staff       (20)      152 2022-12-16 17:29:08.000000 sse-starlette-1.6.0/setup.py
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-05-14 08:32:32.042767 sse-starlette-1.6.0/sse_starlette/
+-rw-r--r--   0 Q187392    (501) staff       (20)      143 2023-05-14 08:31:53.000000 sse-starlette-1.6.0/sse_starlette/__init__.py
+-rw-r--r--   0 Q187392    (501) staff       (20)        0 2022-12-16 17:29:08.000000 sse-starlette-1.6.0/sse_starlette/py.typed
+-rw-r--r--   0 Q187392    (501) staff       (20)    10910 2023-05-14 08:32:12.000000 sse-starlette-1.6.0/sse_starlette/sse.py
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-05-14 08:32:32.052625 sse-starlette-1.6.0/sse_starlette.egg-info/
+-rw-r--r--   0 Q187392    (501) staff       (20)     6520 2023-05-14 08:32:30.000000 sse-starlette-1.6.0/sse_starlette.egg-info/PKG-INFO
+-rw-r--r--   0 Q187392    (501) staff       (20)      392 2023-05-14 08:32:32.000000 sse-starlette-1.6.0/sse_starlette.egg-info/SOURCES.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)        1 2023-05-14 08:32:30.000000 sse-starlette-1.6.0/sse_starlette.egg-info/dependency_links.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)       10 2023-05-14 08:32:30.000000 sse-starlette-1.6.0/sse_starlette.egg-info/requires.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)       14 2023-05-14 08:32:30.000000 sse-starlette-1.6.0/sse_starlette.egg-info/top_level.txt
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-05-14 08:32:32.053874 sse-starlette-1.6.0/tests/
+-rw-r--r--   0 Q187392    (501) staff       (20)     6176 2023-05-14 08:32:12.000000 sse-starlette-1.6.0/tests/test_event_source_response.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     3028 2023-05-02 20:24:28.000000 sse-starlette-1.6.0/tests/test_sse.py
```

### Comparing `sse-starlette-1.5.0/CHANGELOG.md` & `sse-starlette-1.6.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `sse-starlette-1.5.0/LICENSE` & `sse-starlette-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sse-starlette-1.5.0/PKG-INFO` & `sse-starlette-1.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sse-starlette
-Version: 1.5.0
+Version: 1.6.0
 Summary: "SSE plugin for Starlette"
 Home-page: https://github.com/sysid/sse-starlette
 Author: sysid
 Author-email: sysid@gmx.de
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -110,14 +110,23 @@
         generator(), headers={"Cache-Control": "public, max-age=29"}
     )
 ```
 ### Error Handling
 See example: `examples/error_handling.py`
 
 
+### Sending Responses without Async Generators
+Async generators can expose tricky error and cleanup behavior especially when they are interrupted.
+
+[Background: Cleanup in async generators](https://vorpus.org/blog/some-thoughts-on-asynchronous-api-design-in-a-post-asyncawait-world/#cleanup-in-generators-and-async-generators).
+
+Example [`no_async_generators.py`](https://github.com/sysid/sse-starlette/pull/56#issue-1704495339) shows an alternative implementation
+that does not rely on async generators but instead uses memory channels (`examples/no_async_generators.py`).
+
+
 ## Development, Contributing
 1. install pipenv: `pip install pipenv`
 2. install dependencies using pipenv: `pipenv install --dev -e .`
 3. To run tests, either:
    - `pipenv run pytest`
  
 ### Makefile
```

### Comparing `sse-starlette-1.5.0/README.md` & `sse-starlette-1.6.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -91,14 +91,23 @@
         generator(), headers={"Cache-Control": "public, max-age=29"}
     )
 ```
 ### Error Handling
 See example: `examples/error_handling.py`
 
 
+### Sending Responses without Async Generators
+Async generators can expose tricky error and cleanup behavior especially when they are interrupted.
+
+[Background: Cleanup in async generators](https://vorpus.org/blog/some-thoughts-on-asynchronous-api-design-in-a-post-asyncawait-world/#cleanup-in-generators-and-async-generators).
+
+Example [`no_async_generators.py`](https://github.com/sysid/sse-starlette/pull/56#issue-1704495339) shows an alternative implementation
+that does not rely on async generators but instead uses memory channels (`examples/no_async_generators.py`).
+
+
 ## Development, Contributing
 1. install pipenv: `pip install pipenv`
 2. install dependencies using pipenv: `pipenv install --dev -e .`
 3. To run tests, either:
    - `pipenv run pytest`
  
 ### Makefile
```

### Comparing `sse-starlette-1.5.0/setup.cfg` & `sse-starlette-1.6.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sse-starlette
-version = 1.5.0
+version = 1.6.0
 description = "SSE plugin for Starlette"
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 author = sysid
 author_email = sysid@gmx.de
 url = https://github.com/sysid/sse-starlette
 classifiers =
```

### Comparing `sse-starlette-1.5.0/sse_starlette/sse.py` & `sse-starlette-1.6.0/sse_starlette/sse.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,26 +149,30 @@
         status_code: int = 200,
         headers: Optional[Dict] = None,
         media_type: str = "text/event-stream",
         background: Optional[BackgroundTask] = None,
         ping: Optional[int] = None,
         sep: Optional[str] = None,
         ping_message_factory: Optional[Callable[[], ServerSentEvent]] = None,
+        data_sender_callable: Optional[
+            Callable[[], Coroutine[None, None, None]]
+        ] = None,
     ) -> None:
         self.sep = sep
         self.ping_message_factory = ping_message_factory
         if isinstance(content, AsyncIterable):
             self.body_iterator = (
                 content
             )  # type: AsyncIterable[Union[Any,dict,ServerSentEvent]]
         else:
             self.body_iterator = iterate_in_threadpool(content)  # type: ignore
         self.status_code = status_code
         self.media_type = self.media_type if media_type is None else media_type
         self.background = background  # type: ignore  # follows https://github.com/encode/starlette/blob/master/starlette/responses.py
+        self.data_sender_callable = data_sender_callable
 
         _headers = {}
         if headers is not None:  # pragma: no cover
             _headers.update(headers)
 
         # mandatory for servers-sent events headers
         # allow cache control header to be set by user to support fan out proxies
@@ -235,14 +239,18 @@
                 await func()
                 # noinspection PyAsyncCall
                 task_group.cancel_scope.cancel()
 
             task_group.start_soon(wrap, partial(self.stream_response, safe_send))
             task_group.start_soon(wrap, partial(self._ping, safe_send))
             task_group.start_soon(wrap, self.listen_for_exit_signal)
+
+            if self.data_sender_callable:
+                task_group.start_soon(self.data_sender_callable)
+
             await wrap(partial(self.listen_for_disconnect, receive))
 
         if self.background is not None:  # pragma: no cover, tested in StreamResponse
             await self.background()
 
     def enable_compression(self, force: bool = False) -> None:
         raise NotImplementedError
```

### Comparing `sse-starlette-1.5.0/sse_starlette.egg-info/PKG-INFO` & `sse-starlette-1.6.0/sse_starlette.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sse-starlette
-Version: 1.5.0
+Version: 1.6.0
 Summary: "SSE plugin for Starlette"
 Home-page: https://github.com/sysid/sse-starlette
 Author: sysid
 Author-email: sysid@gmx.de
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -110,14 +110,23 @@
         generator(), headers={"Cache-Control": "public, max-age=29"}
     )
 ```
 ### Error Handling
 See example: `examples/error_handling.py`
 
 
+### Sending Responses without Async Generators
+Async generators can expose tricky error and cleanup behavior especially when they are interrupted.
+
+[Background: Cleanup in async generators](https://vorpus.org/blog/some-thoughts-on-asynchronous-api-design-in-a-post-asyncawait-world/#cleanup-in-generators-and-async-generators).
+
+Example [`no_async_generators.py`](https://github.com/sysid/sse-starlette/pull/56#issue-1704495339) shows an alternative implementation
+that does not rely on async generators but instead uses memory channels (`examples/no_async_generators.py`).
+
+
 ## Development, Contributing
 1. install pipenv: `pip install pipenv`
 2. install dependencies using pipenv: `pipenv install --dev -e .`
 3. To run tests, either:
    - `pipenv run pytest`
  
 ### Makefile
```

### Comparing `sse-starlette-1.5.0/tests/test_event_source_response.py` & `sse-starlette-1.6.0/tests/test_event_source_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import asyncio
 import logging
+import math
+from functools import partial
 
 import anyio
 import anyio.lowlevel
 import pytest
 from httpx import AsyncClient
 from sse_starlette import EventSourceResponse
 from starlette.testclient import TestClient
@@ -56,14 +58,48 @@
         await response(scope, receive, send)
 
     client = TestClient(app)
     response = client.get("/")
     assert response.content.decode().count("ping") == 2
     assert expected in response.content
     print(response.content)
+
+
+@pytest.mark.parametrize(
+    "input,expected",
+    [
+        ("integer", b"data: 1\r\n\r\n"),
+        ("dict1", b"data: 1\r\n\r\n"),
+        ("dict2", b"event: message\r\ndata: 1\r\n\r\n"),
+    ],
+)
+def test_sync_memory_channel_event_source_response(input, expected):
+    async def app(scope, receive, send):
+        send_chan, recv_chan = anyio.create_memory_object_stream(math.inf)
+
+        async def numbers(inner_send_chan, minimum, maximum):
+            async with send_chan:
+                for i in range(minimum, maximum + 1):
+                    await anyio.sleep(0.1)
+
+                    if input == "integer":
+                        await inner_send_chan.send(i)
+                    elif input == "dict1":
+                        await inner_send_chan.send(dict(data=i))
+                    elif input == "dict2":
+                        await inner_send_chan.send(dict(data=i, event="message"))
+
+        response = EventSourceResponse(recv_chan, data_sender_callable=partial(numbers, send_chan, 1, 5), ping=0.2)  # type: ignore
+        await response(scope, receive, send)
+
+    client = TestClient(app)
+    response = client.get("/")
+    assert response.content.decode().count("ping") == 2
+    assert expected in response.content
+    print(response.content)
 
 
 @pytest.mark.anyio
 async def test_endless():
     async def app(scope, receive, send):
         async def event_publisher():
             i = 0
```

### Comparing `sse-starlette-1.5.0/tests/test_sse.py` & `sse-starlette-1.6.0/tests/test_sse.py`

 * *Files identical despite different names*

