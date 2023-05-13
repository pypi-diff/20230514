# Comparing `tmp/spacs-0.0.8.tar.gz` & `tmp/spacs-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacs-0.0.8.tar", max compression
+gzip compressed data, was "spacs-0.0.9.tar", max compression
```

## Comparing `spacs-0.0.8.tar` & `spacs-0.0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1093 2023-04-26 20:46:06.053000 spacs-0.0.8/LICENSE
--rw-r--r--   0        0        0      506 2023-05-07 14:12:28.762774 spacs-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4046 2023-05-07 15:59:37.368789 spacs-0.0.8/README.md
--rw-r--r--   0        0        0      217 2023-05-07 14:37:52.722081 spacs-0.0.8/spacs/__init__.py
--rw-r--r--   0        0        0     8417 2023-05-07 14:37:34.446392 spacs-0.0.8/spacs/client.py
--rw-r--r--   0        0        0       55 2023-05-04 13:54:47.377396 spacs-0.0.8/spacs/conf.py
--rw-r--r--   0        0        0     4707 1970-01-01 00:00:00.000000 spacs-0.0.8/setup.py
--rw-r--r--   0        0        0     4388 1970-01-01 00:00:00.000000 spacs-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-04-26 20:46:06.053000 spacs-0.0.9/LICENSE
+-rw-r--r--   0        0        0      506 2023-05-13 22:26:21.834850 spacs-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4023 2023-05-13 22:23:33.564057 spacs-0.0.9/README.md
+-rw-r--r--   0        0        0      217 2023-05-07 14:37:52.722081 spacs-0.0.9/spacs/__init__.py
+-rw-r--r--   0        0        0     9341 2023-05-13 21:56:08.141454 spacs-0.0.9/spacs/client.py
+-rw-r--r--   0        0        0       55 2023-05-04 13:54:47.377396 spacs-0.0.9/spacs/conf.py
+-rw-r--r--   0        0        0     4684 1970-01-01 00:00:00.000000 spacs-0.0.9/setup.py
+-rw-r--r--   0        0        0     4372 1970-01-01 00:00:00.000000 spacs-0.0.9/PKG-INFO
```

### Comparing `spacs-0.0.8/LICENSE` & `spacs-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spacs-0.0.8/README.md` & `spacs-0.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -33,17 +33,15 @@
 async def example():
     client = SpacsClient(base_url="https://httpbin.org")
     request = SpacsRequest(path="/get", params={"foo": "bar"})
     result = await client.get(request)
     print(result)
     await client.close()
 
-
-loop = asyncio.new_event_loop()
-loop.run_until_complete(example())
+asyncio.new_event_loop().run_until_complete(example())
 ```
 
 ### Sending Pydantic objects via request body
 ```python
 import asyncio
 from spacs import SpacsClient, SpacsRequest
 from pydantic import BaseModel
@@ -56,17 +54,15 @@
     client = SpacsClient(base_url="https://httpbin.org")
     person = Person(name="James", age=25)
     request = SpacsRequest(path="/post", body=person)
     response = await client.post(request)
     print(response)
     await client.close()
 
-
-loop = asyncio.new_event_loop()
-loop.run_until_complete(example())
+asyncio.new_event_loop().run_until_complete(example())
 ```
 
 #### Tip: Response Model
 For all examples here, if the API declares that response bodies will *only* contain json data representing a Pydantic object, the payload can be deserialized into an object by specifying a Pydantic class in the request. For example, using our above `Person` model:
 ```python
 request = SpacsRequest(path="/post", body=person, response_model=Person)
 response = await client.post(request)
@@ -84,37 +80,34 @@
     request = SpacsRequest(path="/status/404")
     try:
         await client.get(request)
     except SpacsRequestError as error:
         print({"code": error.status, "reason": error.reason})
     await client.close()
 
-
-loop = asyncio.new_event_loop()
-loop.run_until_complete(example())
+asyncio.new_event_loop().run_until_complete(example())
 ```
 
 ### Injecting Error Handler
 ```python
 import asyncio
 from spacs import SpacsClient, SpacsRequest, SpacsRequestError
 
 async def error_handler(error: SpacsRequestError) -> None:
     print(f"It blew up: {error.reason}")
+    await error.client.close()
 
 async def example():
     client = SpacsClient(base_url="https://httpbin.org", error_handler=error_handler)
     request = SpacsRequest(path="/status/504")
     response = await client.get(request)
-    await client.close()
+    assert not client.is_open
     assert response is None
 
-
-loop = asyncio.new_event_loop()
-loop.run_until_complete(example())
+asyncio.new_event_loop().run_until_complete(example())
 ```
 
 ### Closing sessions
 In the above examples, a `client.close()` call is made. This is to ensure that the underlying AIOHTTP session
 is properly cleaned up, and is a step that should always be performed on application teardown. Alternatively, the following can be used to close all open sessions without having to
 directly reference a client instance:
 ```python
```

### Comparing `spacs-0.0.8/spacs/client.py` & `spacs-0.0.9/spacs/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,48 +31,57 @@
     content_type: ContentType = ContentType.JSON
     response_model: ResponseModel = None
 
 
 class SpacsRequestError(Exception):
     status: int
     reason: str
+    client: "SpacsClient"
+    request: SpacsRequest
 
-    def __init__(self, status: int, reason: str):
+    def __init__(
+        self, status: int, reason: str, client: "SpacsClient", request: SpacsRequest
+    ):
         self.status = status
         self.reason = reason
+        self.client = client
+        self.request = request
 
     def __repr__(self) -> str:
         return f"SpacsRequestError(status={self.status}, reason={self.reason}"
 
 
 class SpacsClient:
     base_url: str | None
     path_prefix: str
     error_handler: Callable[[SpacsRequestError], Awaitable[None]] | None
+    close_on_error: bool | list[int]
 
     _sessions: ClassVar[list[Self]] = []
     _session: aiohttp.ClientSession | None = None
 
     def __init__(
         self,
         *,
         base_url: str | None = None,
         path_prefix: str = "",
         error_handler: Callable[[SpacsRequestError], Awaitable[None]] | None = None,
+        close_on_error: bool | list[int] = False,
     ) -> None:
         """
 
         Keyword Args:
             base_url (str | None): Base url to be used for all requests
             path_prefix (str): Path partial to be prepended to paths for all requests
         """
         self._sessions.append(self)
         self.base_url = base_url
         self.path_prefix = path_prefix.strip("/")
         self.error_handler = error_handler
+        self.close_on_error = close_on_error
 
     def __del__(self) -> None:
         self._sessions.remove(self)
 
     @property
     def session(self) -> aiohttp.ClientSession:
         if not self.is_open:
@@ -106,58 +115,27 @@
         self,
         action: Callable[..., Awaitable[ClientResponse]],
         request: SpacsRequest,
     ) -> SpacsResponse:
         """Generic function for issuing requests"""
         request = self._prepare_request(request)
 
-        start_time = datetime.datetime.now(tz=datetime.timezone.utc)
         base_log_info = {
             "method": action.__name__,
             "base_url": self.base_url,
             "path": request.path,
         }
 
         try:
-            response = await action(
-                request.path,
-                params=request.params,
-                data=request.body,
-                headers=request.headers,
-            )
-            end_time = datetime.datetime.now(tz=datetime.timezone.utc)
-            logger.debug(
-                {
-                    "msg": "Request completed",
-                    **base_log_info,
-                    "status": response.status,
-                    "duration": str(end_time - start_time),
-                }
-            )
-            if response.ok:
-                return await self._handle_ok_response(response, request.response_model)
-            else:
-                raise SpacsRequestError(
-                    status=response.status,
-                    reason=response.reason,
-                )
+            return await self._make_request(request, action, base_log_info)
         except ClientConnectorError as error:
             logger.error("Failed to connect to server.")
             raise error
         except Exception as error:
-            logger.error(
-                {
-                    "msg": "Request error",
-                    **base_log_info,
-                    "error": repr(error),
-                }
-            )
-            if self.error_handler is not None and isinstance(error, SpacsRequestError):
-                return await self.error_handler(error)
-            raise error
+            return await self._handle_request_failure(error, base_log_info)
 
     def _prepare_request(self, request: SpacsRequest) -> SpacsRequest:
         # Copy content to not modify inputs to `SpacsClient` actions
         result = request.copy(deep=True)
 
         if result.headers is None:
             result.headers = {}
@@ -178,14 +156,69 @@
     def _build_path(self, path: str) -> str:
         prepend_slash = "/" if self.base_url else ""
         result = f"{prepend_slash}{path.strip('/')}"
         if self.path_prefix:
             result = f"{prepend_slash}{self.path_prefix}{result}"
         return result
 
+    async def _make_request(
+        self,
+        request: SpacsRequest,
+        action: Callable[..., Awaitable[ClientResponse]],
+        base_log_info: dict,
+    ) -> str | JsonContent | ModelContent:
+        start_time = datetime.datetime.now(tz=datetime.timezone.utc)
+        response = await action(
+            request.path,
+            params=request.params,
+            data=request.body,
+            headers=request.headers,
+        )
+        duration = datetime.datetime.now(tz=datetime.timezone.utc) - start_time
+        logger.debug(
+            {
+                "msg": "Request completed",
+                **base_log_info,
+                "status": response.status,
+                "duration": str(duration),
+            }
+        )
+        if response.ok:
+            return await self._handle_ok_response(response, request.response_model)
+        raise SpacsRequestError(
+            status=response.status,
+            reason=response.reason,
+            client=self,
+            request=request,
+        )
+
+    async def _handle_request_failure(
+        self, error: Exception, base_log_info: dict
+    ) -> None:
+        logger.error(
+            {
+                "msg": "Request error",
+                **base_log_info,
+                "error": repr(error),
+            }
+        )
+
+        if not isinstance(error, SpacsRequestError):
+            raise error
+
+        if self.close_on_error is True or (
+            isinstance(self.close_on_error, list)
+            and error.status in self.close_on_error
+        ):
+            await self.close()
+
+        if self.error_handler is not None:
+            return await self.error_handler(error)
+        raise error
+
     @classmethod
     async def close_all(cls) -> None:
         for session in cls._sessions:
             if not session.is_open:
                 continue
             await session.close()
```

### Comparing `spacs-0.0.8/setup.py` & `spacs-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.8.4,<4.0.0', 'pydantic>=1.10.7,<2.0.0']
 
 setup_kwargs = {
     'name': 'spacs',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Simple Pydantic AIOHTTP Client Sessions',
-    'long_description': '# SPACS: Simple Pydantic AIOHTTP Client Sessions\n\nA package to assist in managing and using long-lived AIOHTTP client sessions with simplicity. Built to handle Pydantic objects.\n\n## Features\n\n- Handles request params and bodies as either Pydantic objects or native Python dictionaries, converting items to JSON-safe format.\n- Abstracts away internals of managing the request/response objects, instead either returning parsed response content on success, or raising a specialized error object.\n- Automatically manages persistent connections to be shared over extended lifespan across application, cleaning up all open connections on teardown.\n- Utilizes modern Python type hinting.\n\n## Installation\n\nUsing poetry (preferred):\n\n```bash\npoetry add spacs\n```\n\nUsing pip:\n\n```bash\npip install spacs\n```\n\n## Basic Usage\nSPACS currently supports the HTTP methods GET, POST, PUT, and DELETE. All methods take the same, singular `SpacsRequest` argument. The following are some common patterns to be utilized when working with SPACS.\n### Request With Params\n```python\nimport asyncio\nfrom spacs import SpacsClient, SpacsRequest\n\nasync def example():\n    client = SpacsClient(base_url="https://httpbin.org")\n    request = SpacsRequest(path="/get", params={"foo": "bar"})\n    result = await client.get(request)\n    print(result)\n    await client.close()\n\n\nloop = asyncio.new_event_loop()\nloop.run_until_complete(example())\n```\n\n### Sending Pydantic objects via request body\n```python\nimport asyncio\nfrom spacs import SpacsClient, SpacsRequest\nfrom pydantic import BaseModel\n\nclass Person(BaseModel):\n    name: str\n    age: int\n\nasync def example():\n    client = SpacsClient(base_url="https://httpbin.org")\n    person = Person(name="James", age=25)\n    request = SpacsRequest(path="/post", body=person)\n    response = await client.post(request)\n    print(response)\n    await client.close()\n\n\nloop = asyncio.new_event_loop()\nloop.run_until_complete(example())\n```\n\n#### Tip: Response Model\nFor all examples here, if the API declares that response bodies will *only* contain json data representing a Pydantic object, the payload can be deserialized into an object by specifying a Pydantic class in the request. For example, using our above `Person` model:\n```python\nrequest = SpacsRequest(path="/post", body=person, response_model=Person)\nresponse = await client.post(request)\nassert isinstance(response, Person)\n```\n\n## Handling Errors\n### Manual Error Handling\n```python\nimport asyncio\nfrom spacs import SpacsClient, SpacsRequest, SpacsRequestError\n\nasync def example():\n    client = SpacsClient(base_url="https://httpbin.org")\n    request = SpacsRequest(path="/status/404")\n    try:\n        await client.get(request)\n    except SpacsRequestError as error:\n        print({"code": error.status, "reason": error.reason})\n    await client.close()\n\n\nloop = asyncio.new_event_loop()\nloop.run_until_complete(example())\n```\n\n### Injecting Error Handler\n```python\nimport asyncio\nfrom spacs import SpacsClient, SpacsRequest, SpacsRequestError\n\nasync def error_handler(error: SpacsRequestError) -> None:\n    print(f"It blew up: {error.reason}")\n\nasync def example():\n    client = SpacsClient(base_url="https://httpbin.org", error_handler=error_handler)\n    request = SpacsRequest(path="/status/504")\n    response = await client.get(request)\n    await client.close()\n    assert response is None\n\n\nloop = asyncio.new_event_loop()\nloop.run_until_complete(example())\n```\n\n### Closing sessions\nIn the above examples, a `client.close()` call is made. This is to ensure that the underlying AIOHTTP session\nis properly cleaned up, and is a step that should always be performed on application teardown. Alternatively, the following can be used to close all open sessions without having to\ndirectly reference a client instance:\n```python\nawait SpacsClient.close_all()\n```\n> SPACS is not affiliated with httpbin.org.\n\n## Building\n\n```\npoetry build\n```\n',
+    'long_description': '# SPACS: Simple Pydantic AIOHTTP Client Sessions\n\nA package to assist in managing and using long-lived AIOHTTP client sessions with simplicity. Built to handle Pydantic objects.\n\n## Features\n\n- Handles request params and bodies as either Pydantic objects or native Python dictionaries, converting items to JSON-safe format.\n- Abstracts away internals of managing the request/response objects, instead either returning parsed response content on success, or raising a specialized error object.\n- Automatically manages persistent connections to be shared over extended lifespan across application, cleaning up all open connections on teardown.\n- Utilizes modern Python type hinting.\n\n## Installation\n\nUsing poetry (preferred):\n\n```bash\npoetry add spacs\n```\n\nUsing pip:\n\n```bash\npip install spacs\n```\n\n## Basic Usage\nSPACS currently supports the HTTP methods GET, POST, PUT, and DELETE. All methods take the same, singular `SpacsRequest` argument. The following are some common patterns to be utilized when working with SPACS.\n### Request With Params\n```python\nimport asyncio\nfrom spacs import SpacsClient, SpacsRequest\n\nasync def example():\n    client = SpacsClient(base_url="https://httpbin.org")\n    request = SpacsRequest(path="/get", params={"foo": "bar"})\n    result = await client.get(request)\n    print(result)\n    await client.close()\n\nasyncio.new_event_loop().run_until_complete(example())\n```\n\n### Sending Pydantic objects via request body\n```python\nimport asyncio\nfrom spacs import SpacsClient, SpacsRequest\nfrom pydantic import BaseModel\n\nclass Person(BaseModel):\n    name: str\n    age: int\n\nasync def example():\n    client = SpacsClient(base_url="https://httpbin.org")\n    person = Person(name="James", age=25)\n    request = SpacsRequest(path="/post", body=person)\n    response = await client.post(request)\n    print(response)\n    await client.close()\n\nasyncio.new_event_loop().run_until_complete(example())\n```\n\n#### Tip: Response Model\nFor all examples here, if the API declares that response bodies will *only* contain json data representing a Pydantic object, the payload can be deserialized into an object by specifying a Pydantic class in the request. For example, using our above `Person` model:\n```python\nrequest = SpacsRequest(path="/post", body=person, response_model=Person)\nresponse = await client.post(request)\nassert isinstance(response, Person)\n```\n\n## Handling Errors\n### Manual Error Handling\n```python\nimport asyncio\nfrom spacs import SpacsClient, SpacsRequest, SpacsRequestError\n\nasync def example():\n    client = SpacsClient(base_url="https://httpbin.org")\n    request = SpacsRequest(path="/status/404")\n    try:\n        await client.get(request)\n    except SpacsRequestError as error:\n        print({"code": error.status, "reason": error.reason})\n    await client.close()\n\nasyncio.new_event_loop().run_until_complete(example())\n```\n\n### Injecting Error Handler\n```python\nimport asyncio\nfrom spacs import SpacsClient, SpacsRequest, SpacsRequestError\n\nasync def error_handler(error: SpacsRequestError) -> None:\n    print(f"It blew up: {error.reason}")\n    await error.client.close()\n\nasync def example():\n    client = SpacsClient(base_url="https://httpbin.org", error_handler=error_handler)\n    request = SpacsRequest(path="/status/504")\n    response = await client.get(request)\n    assert not client.is_open\n    assert response is None\n\nasyncio.new_event_loop().run_until_complete(example())\n```\n\n### Closing sessions\nIn the above examples, a `client.close()` call is made. This is to ensure that the underlying AIOHTTP session\nis properly cleaned up, and is a step that should always be performed on application teardown. Alternatively, the following can be used to close all open sessions without having to\ndirectly reference a client instance:\n```python\nawait SpacsClient.close_all()\n```\n> SPACS is not affiliated with httpbin.org.\n\n## Building\n\n```\npoetry build\n```\n',
     'author': 'rlebel12',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/rlebel12/spacs',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `spacs-0.0.8/PKG-INFO` & `spacs-0.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacs
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple Pydantic AIOHTTP Client Sessions
 Home-page: https://github.com/rlebel12/spacs
 Author: rlebel12
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
@@ -47,17 +47,15 @@
 async def example():
     client = SpacsClient(base_url="https://httpbin.org")
     request = SpacsRequest(path="/get", params={"foo": "bar"})
     result = await client.get(request)
     print(result)
     await client.close()
 
-
-loop = asyncio.new_event_loop()
-loop.run_until_complete(example())
+asyncio.new_event_loop().run_until_complete(example())
 ```
 
 ### Sending Pydantic objects via request body
 ```python
 import asyncio
 from spacs import SpacsClient, SpacsRequest
 from pydantic import BaseModel
@@ -70,17 +68,15 @@
     client = SpacsClient(base_url="https://httpbin.org")
     person = Person(name="James", age=25)
     request = SpacsRequest(path="/post", body=person)
     response = await client.post(request)
     print(response)
     await client.close()
 
-
-loop = asyncio.new_event_loop()
-loop.run_until_complete(example())
+asyncio.new_event_loop().run_until_complete(example())
 ```
 
 #### Tip: Response Model
 For all examples here, if the API declares that response bodies will *only* contain json data representing a Pydantic object, the payload can be deserialized into an object by specifying a Pydantic class in the request. For example, using our above `Person` model:
 ```python
 request = SpacsRequest(path="/post", body=person, response_model=Person)
 response = await client.post(request)
@@ -98,37 +94,34 @@
     request = SpacsRequest(path="/status/404")
     try:
         await client.get(request)
     except SpacsRequestError as error:
         print({"code": error.status, "reason": error.reason})
     await client.close()
 
-
-loop = asyncio.new_event_loop()
-loop.run_until_complete(example())
+asyncio.new_event_loop().run_until_complete(example())
 ```
 
 ### Injecting Error Handler
 ```python
 import asyncio
 from spacs import SpacsClient, SpacsRequest, SpacsRequestError
 
 async def error_handler(error: SpacsRequestError) -> None:
     print(f"It blew up: {error.reason}")
+    await error.client.close()
 
 async def example():
     client = SpacsClient(base_url="https://httpbin.org", error_handler=error_handler)
     request = SpacsRequest(path="/status/504")
     response = await client.get(request)
-    await client.close()
+    assert not client.is_open
     assert response is None
 
-
-loop = asyncio.new_event_loop()
-loop.run_until_complete(example())
+asyncio.new_event_loop().run_until_complete(example())
 ```
 
 ### Closing sessions
 In the above examples, a `client.close()` call is made. This is to ensure that the underlying AIOHTTP session
 is properly cleaned up, and is a step that should always be performed on application teardown. Alternatively, the following can be used to close all open sessions without having to
 directly reference a client instance:
 ```python
```

