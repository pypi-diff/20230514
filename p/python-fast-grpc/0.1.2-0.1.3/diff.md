# Comparing `tmp/python_fast_grpc-0.1.2.tar.gz` & `tmp/python_fast_grpc-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_fast_grpc-0.1.2.tar", max compression
+gzip compressed data, was "python_fast_grpc-0.1.3.tar", max compression
```

## Comparing `python_fast_grpc-0.1.2.tar` & `python_fast_grpc-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-05-07 10:06:20.785302 python_fast_grpc-0.1.2/LICENSE
--rw-r--r--   0        0        0      939 2023-05-08 16:51:46.015329 python_fast_grpc-0.1.2/README.md
--rw-r--r--   0        0        0     6148 2023-05-08 16:48:47.382250 python_fast_grpc-0.1.2/fast_grpc/.DS_Store
--rw-r--r--   0        0        0      127 2023-05-07 10:04:32.688620 python_fast_grpc-0.1.2/fast_grpc/__init__.py
--rw-r--r--   0        0        0     3639 2023-05-08 16:11:07.098108 python_fast_grpc-0.1.2/fast_grpc/app.py
--rw-r--r--   0        0        0      242 2023-05-07 08:52:13.078197 python_fast_grpc-0.1.2/fast_grpc/base.py
--rw-r--r--   0        0        0      981 2023-05-07 08:52:17.786157 python_fast_grpc-0.1.2/fast_grpc/exceptions.py
--rw-r--r--   0        0        0      570 2023-05-07 08:53:00.804651 python_fast_grpc-0.1.2/fast_grpc/middleware/__init__.py
--rw-r--r--   0        0        0     1657 2023-05-07 10:04:32.670718 python_fast_grpc-0.1.2/fast_grpc/middleware/base.py
--rw-r--r--   0        0        0       24 2023-05-07 08:53:11.397718 python_fast_grpc-0.1.2/fast_grpc/middleware/exception.py
--rw-r--r--   0        0        0     6819 2023-05-08 17:00:54.741345 python_fast_grpc-0.1.2/fast_grpc/proto.py
--rw-r--r--   0        0        0     5022 2023-05-08 16:25:53.094255 python_fast_grpc-0.1.2/fast_grpc/service.py
--rw-r--r--   0        0        0      139 2023-04-22 16:02:22.806235 python_fast_grpc-0.1.2/fast_grpc/signals.py
--rw-r--r--   0        0        0     3313 2023-05-08 16:08:10.646222 python_fast_grpc-0.1.2/fast_grpc/types.py
--rw-r--r--   0        0        0     2103 2023-05-08 16:13:38.796925 python_fast_grpc-0.1.2/fast_grpc/utils.py
--rw-r--r--   0        0        0     1339 2023-05-08 17:07:10.252190 python_fast_grpc-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1707 1970-01-01 00:00:00.000000 python_fast_grpc-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-07 10:06:20.785302 python_fast_grpc-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1038 2023-05-14 15:32:32.269858 python_fast_grpc-0.1.3/README.md
+-rw-r--r--   0        0        0     6148 2023-05-08 16:48:47.382250 python_fast_grpc-0.1.3/fast_grpc/.DS_Store
+-rw-r--r--   0        0        0      192 2023-05-14 15:12:18.407743 python_fast_grpc-0.1.3/fast_grpc/__init__.py
+-rw-r--r--   0        0        0     3778 2023-05-14 08:37:15.553003 python_fast_grpc-0.1.3/fast_grpc/app.py
+-rw-r--r--   0        0        0      242 2023-05-07 08:52:13.078197 python_fast_grpc-0.1.3/fast_grpc/base.py
+-rw-r--r--   0        0        0      191 2023-05-13 17:31:04.941670 python_fast_grpc-0.1.3/fast_grpc/context.py
+-rw-r--r--   0        0        0      981 2023-05-07 08:52:17.786157 python_fast_grpc-0.1.3/fast_grpc/exceptions.py
+-rw-r--r--   0        0        0      570 2023-05-07 08:53:00.804651 python_fast_grpc-0.1.3/fast_grpc/middleware/__init__.py
+-rw-r--r--   0        0        0     1663 2023-05-13 18:27:09.361631 python_fast_grpc-0.1.3/fast_grpc/middleware/base.py
+-rw-r--r--   0        0        0       24 2023-05-07 08:53:11.397718 python_fast_grpc-0.1.3/fast_grpc/middleware/exception.py
+-rw-r--r--   0        0        0     6819 2023-05-08 17:00:54.741345 python_fast_grpc-0.1.3/fast_grpc/proto.py
+-rw-r--r--   0        0        0     6628 2023-05-14 08:20:08.768008 python_fast_grpc-0.1.3/fast_grpc/service.py
+-rw-r--r--   0        0        0      139 2023-04-22 16:02:22.806235 python_fast_grpc-0.1.3/fast_grpc/signals.py
+-rw-r--r--   0        0        0     3240 2023-05-13 16:44:23.185300 python_fast_grpc-0.1.3/fast_grpc/types.py
+-rw-r--r--   0        0        0     2103 2023-05-08 16:13:38.796925 python_fast_grpc-0.1.3/fast_grpc/utils.py
+-rw-r--r--   0        0        0     1339 2023-05-14 15:48:25.742155 python_fast_grpc-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1806 1970-01-01 00:00:00.000000 python_fast_grpc-0.1.3/PKG-INFO
```

### Comparing `python_fast_grpc-0.1.2/LICENSE` & `python_fast_grpc-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_fast_grpc-0.1.2/README.md` & `python_fast_grpc-0.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 # fast-grpc
-fast to code grpc in Python 3.7+
+Fast to Code gRPC in Python 3.7+
 
 # Installation
 Require Python 3.7+
 ```shell
 pip install python-fast-grpc
 ```
 
 # Quick start
 1. Run a gRPC application
 ```python
-from fast_grpc import BaseSchema, FastGRPC
+from fast_grpc import BaseSchema, FastGRPC, ServicerContext, method
 
-rpc = FastGRPC("Greeter")
+app = FastGRPC()
 
 class HelloRequest(BaseSchema):
     name: str
 
 class HelloReply(BaseSchema):
     message: str
 
-@rpc.add_method("SayHello", request_model=HelloRequest, response_model=HelloReply)
-async def say_hello(request: HelloRequest) -> HelloReply:
-    return HelloReply(message=f"Hello {request.name}")
+class Greeter:
+    @method("SayHello", request_model=HelloRequest, response_model=HelloReply)
+    async def say_hello(self, request: HelloRequest, context: ServicerContext) -> HelloReply:
+        return HelloReply(message=f"Greeter SayHello {request.name}")
 
+app.add_service(Greeter)
 # this step will generate .proto file and python gRPC code, then start a grpc server
-rpc.run()
+app.run()
 ```
-2. run client invoke
+2. Client invoke
 ```python
 import grpc
 import greeter_pb2 as pb2
 import greeter_pb2_grpc as pb2_grpc
 
 channel = grpc.insecure_channel("127.0.0.1:50051")
 stub = pb2_grpc.GreeterStub(channel)
```

### Comparing `python_fast_grpc-0.1.2/fast_grpc/.DS_Store` & `python_fast_grpc-0.1.3/fast_grpc/.DS_Store`

 * *Files identical despite different names*

### Comparing `python_fast_grpc-0.1.2/fast_grpc/app.py` & `python_fast_grpc-0.1.3/fast_grpc/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,41 +7,42 @@
 from grpc.aio._typing import ChannelArgumentType  # noqa
 from logzero import logger
 from pydantic import BaseModel
 
 from fast_grpc.middleware import Middleware
 from fast_grpc.middleware.base import BaseRPCMiddleware
 from fast_grpc.service import Service
-from fast_grpc.types import App
 
 
 class FastGRPC(object):
     def __init__(
         self,
-        default_service_name: str = "FastGRPC",
+        default_service_name: Optional[str] = None,
         middleware: Optional[Sequence[Middleware]] = None,
     ):
-        self.default_service_name = default_service_name
-        self.service = Service(service_name=self.default_service_name)
-
+        self.services = []
+        if default_service_name:
+            self.default_service = Service(type(default_service_name, (object,), {}))
+            self.services.append(self.default_service)
+        else:
+            self.default_service = None
         self.rpc_startup_funcs: List[Callable[..., Any]] = []
         self.rpc_shutdown_funcs: List[Callable[..., Any]] = []
         self.user_middleware: List[Middleware] = [] if middleware is None else list(middleware)
-        self.middleware_stack: App = self.build_middleware_stack()
 
     def setup(self) -> None:
         # build proto
-        self.service.gen_and_compile_proto()
+        for service in self.services:
+            service.gen_and_compile_proto()
 
     def on_startup(self, func: Callable[..., None]):
         self.rpc_startup_funcs.append(func)
 
     def add_middleware(self, middleware_class: type, **options: Any) -> None:
         self.user_middleware.insert(0, Middleware(middleware_class, **options))
-        self.middleware_stack = self.build_middleware_stack()
 
     def run(
         self,
         host: str = "127.0.0.1",
         port: int = 50051,
         options: Optional[ChannelArgumentType] = None,
         maximum_concurrent_rpcs: Optional[int] = None,
@@ -64,40 +65,42 @@
         self,
         host: str = "127.0.0.1",
         port: int = 50051,
         options: Optional[ChannelArgumentType] = None,
         maximum_concurrent_rpcs: Optional[int] = None,
         compression: Optional[grpc.Compression] = None,
     ) -> None:
+        def build_middleware_stack(app):
+            middleware = [Middleware(BaseRPCMiddleware)]
+            for cls, options in middleware:
+                app = cls(app=app, **options)
+            return app
+
         self.setup()
         for handler in self.rpc_startup_funcs:
             if inspect.iscoroutinefunction(handler):
                 await handler()
             else:
                 handler()
         server = grpc.aio.server(
             options=options,
             maximum_concurrent_rpcs=maximum_concurrent_rpcs,
             compression=compression,
         )
-        self.service.bind_server(server, self)
+        for service in self.services:
+            service.bind_server(server, build_middleware_stack(service))
         logger.info(f"Running grpc on {host}:{port}")
         server.add_insecure_port(f"{host}:{port}")
         await server.start()
         await server.wait_for_termination()
 
     def add_method(self, name, *, request_model: Type[BaseModel], response_model: Type[BaseModel]) -> Callable:
         def decorator(func: Callable) -> Callable:
-            self.service.add_rpc_method(name, func, request_model=request_model, response_model=response_model)
+            if self.default_service is None:
+                raise ValueError("Need set default_service_name")
+            self.default_service.add_rpc_method(name, func, request_model=request_model, response_model=response_model)
             return func
 
         return decorator
 
-    def build_middleware_stack(self):
-        middleware = [Middleware(BaseRPCMiddleware)]
-        app = self.service
-        for cls, options in middleware:
-            app = cls(app=app, **options)
-        return app
-
-    async def __call__(self, request, context, handler):
-        return await self.middleware_stack(request, context, handler)
+    def add_service(self, servicer):
+        self.services.append(Service(servicer))
```

### Comparing `python_fast_grpc-0.1.2/fast_grpc/exceptions.py` & `python_fast_grpc-0.1.3/fast_grpc/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_fast_grpc-0.1.2/fast_grpc/middleware/__init__.py` & `python_fast_grpc-0.1.3/fast_grpc/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `python_fast_grpc-0.1.2/fast_grpc/middleware/base.py` & `python_fast_grpc-0.1.3/fast_grpc/middleware/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 # -*- coding: utf-8 -*-
 import asyncio
 import time
 from typing import Callable, Optional
 
 import grpc
 from google.protobuf.text_format import MessageToString
-from grpc import ServicerContext
 from logzero import logger
 
-from fast_grpc.types import App, Message
+from fast_grpc.types import App, Message, ServicerContext
 from fast_grpc.utils import await_sync_function
 
 
 class BaseRPCMiddleware:
     def __init__(self, app: App, handler: Optional[Callable] = None):
         self.app = app
         self.handler = handler
 
-    async def __call__(self, request: Message, context: ServicerContext, method):
+    async def __call__(self, request: Message, context: ServicerContext):
         try:
             start_time = time.time()
-            response = await self.app(request, context, method)
+            response = await self.app(request, context)
             message = MessageToString(request, as_one_line=True)
             end_time = time.time()
             elapsed_time = end_time - start_time
             logger.info(
-                f"GRPC invoke {method.service.service_name}.{method.name}({message}) [OK] {elapsed_time:.3f} seconds"
+                f"GRPC invoke {context.method.servicer.__name__}.{context.method.name}({message}) [OK] {elapsed_time:.3f} seconds"
             )
             return response
         except Exception as exc:
             if self.handler:
                 if asyncio.iscoroutinefunction(self.handler):
                     response = await self.handler(request, context, exc)
                 else:
                     response = await await_sync_function(self.handler)(request, context, exc)
                 return response
             else:
                 message = MessageToString(request, as_one_line=True)
                 logger.exception(
-                    f"GRPC invoke {method.service.service_name}.{method.name}({message}) [Err] -> {repr(exc)}"
+                    f"GRPC invoke {context.method.servicer.__name__}.{context.method.name}({message}) [Err] -> {repr(exc)}"
                 )
-                await context.abort(grpc.StatusCode.UNKNOWN, repr(exc))
+                await context.rpc_context.abort(grpc.StatusCode.UNKNOWN, repr(exc))
```

### Comparing `python_fast_grpc-0.1.2/fast_grpc/proto.py` & `python_fast_grpc-0.1.3/fast_grpc/proto.py`

 * *Files identical despite different names*

### Comparing `python_fast_grpc-0.1.2/fast_grpc/service.py` & `python_fast_grpc-0.1.3/fast_grpc/service.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
+import functools
 import inspect
 import os
 from concurrent.futures import ThreadPoolExecutor
 from importlib import import_module
-from typing import Any, Callable, List, Optional
+from typing import Any, Callable, Optional, Type
 
 from google.protobuf.json_format import MessageToDict, Parse, ParseDict
 
 from fast_grpc.proto import ProtoBuilder, protoc_compile
 from fast_grpc.types import Message, ServicerContext
 from fast_grpc.utils import (
     await_sync_function,
@@ -25,129 +26,171 @@
     return Parse(data, message, ignore_unknown_fields=True)
 
 
 def dict_to_message(data, message):
     return ParseDict(data, message, ignore_unknown_fields=True)
 
 
+def is_entrypoint(method):
+    return hasattr(method, "servicer")
+
+
 class ServiceMetaclass(type):
     def __new__(mcs, name, bases, attrs):
         new_class = type.__new__(mcs, name, bases, attrs)
         for key, value in attrs.items():
             setattr(new_class, key, value)
 
         return new_class
 
 
 class Service:
-    def __init__(self, service_name: str, package_name: str = "", proto_path="."):
-        self.service_name = service_name
-        self.methods: List[Method] = []
+    def __init__(self, servicer: Type, package_name: str = "", proto_path="."):
+        self.service_name = servicer.__name__
         self.proto_path = proto_path
         self.thread_pool: Optional[ThreadPoolExecutor] = None
+        self.servicer_class = servicer
 
         if is_camel_case(self.service_name):
-            self.proto_name = camel_to_snake(self.service_name).lower()
+            self.proto_file_name = camel_to_snake(self.service_name).lower()
         elif is_snake_case(self.service_name):
-            self.proto_name = self.service_name.lower()
+            self.proto_file_name = self.service_name.lower()
         else:
-            self.proto_name = self.service_name.lower()
+            self.proto_file_name = self.service_name.lower()
 
         if package_name:
             self.package_name = package_name
         else:
-            self.package_name = self.proto_name
+            self.package_name = self.proto_file_name
 
         self._proto_file = None
         self._pb2 = None
         self._pb2_grpc = None
 
     @property
     def proto_file(self):
         if self._proto_file is None:
             if not os.path.exists(self.proto_path):
                 os.makedirs(self.proto_path)
-            self._proto_file = os.path.join(self.proto_path, f"{self.proto_name}.proto")
+            self._proto_file = os.path.join(self.proto_path, f"{self.proto_file_name}.proto")
         return self._proto_file
 
     @property
     def pb2(self):
         if self._pb2 is None:
             self._pb2 = import_module(f"{self.package_name}_pb2")
         return self._pb2
 
     @property
     def pb2_grpc(self):
         if self._pb2_grpc is None:
             self._pb2_grpc = import_module(f"{self.package_name}_pb2_grpc")
         return self._pb2_grpc
 
+    @property
+    def methods(self):
+        return [attr for _, attr in inspect.getmembers(self.servicer_class) if is_entrypoint(attr)]
+
     def gen_and_compile_proto(self):
         builder = ProtoBuilder(self)
         proto = builder.create()
         with open(self.proto_file, "w") as f:
             f.write(proto)
         protoc_compile(self.proto_file)
 
     def bind_server(self, server, app):
         """
         demo_pb2_grpc.add_GreeterServicer_to_server(Greeter(), server)
         """
-        getattr(self.pb2_grpc, f"add_{self.service_name}Servicer_to_server")(self.to_grpc_service(app), server)
+        getattr(self.pb2_grpc, f"add_{self.service_name}Servicer_to_server")(self.to_grpc_service(app)(), server)
         # self.thread_pool
 
     def to_grpc_service(self, app):
-        def decorator(method: Method):
+        def decorator(_method: Method):
             async def handle(_self, request, context):
-                return await app(request, context, method)
+                return await app(request, ServicerContext(context, _method))
 
             return handle
 
         service_interface = getattr(self.pb2_grpc, f"{self.service_name}Servicer")
-        attrs_dict = {method.name: decorator(method) for method in self.methods}
-        return type(f"{self.service_name}", (service_interface,), attrs_dict)()
+        # attrs_dict = {_method.name: decorator(_method) for _method in self.methods}
+        for _method in self.methods:
+            setattr(self.servicer_class, _method.name, decorator(_method))
+        cls = type(f"{self.service_name}", (self.servicer_class, service_interface), {})
+        return cls
 
     def add_rpc_method(
         self,
         name: str,
         endpoint: Callable[..., Any],
         *,
         request_model: Any,
         response_model: Any,
     ):
-        self.methods.append(
-            Method(
-                name=name, endpoint=endpoint, request_model=request_model, response_model=response_model, service=self
-            )
-        )
+        rpc_method = Method(name=name, endpoint=endpoint, request_model=request_model, response_model=response_model)
+        setattr(self.servicer_class, name, rpc_method)
 
-    async def __call__(self, request: Message, context: ServicerContext, invoke_method: "Method") -> Message:
-        py_request = invoke_method.request_model.parse_obj(message_to_dict(request))
-        response = await invoke_method(py_request, context)
-        return json_to_message(response.json(), getattr(self.pb2, invoke_method.response_model.__name__)())
+    async def __call__(self, request: Message, context: ServicerContext) -> Message:
+        py_request = context.method.request_model.parse_obj(message_to_dict(request))
+        response = await context.method(py_request, context)
+        return json_to_message(response.json(), getattr(self.pb2, context.method.response_model.__name__)())
 
 
 class Method:
-    def __init__(
-        self,
-        name: str,
-        endpoint: Callable[..., Any],
-        *,
-        request_model: Any,
-        response_model: Any,
-        service: Service,
-    ):
+    def __init__(self, name: str, endpoint: Callable[..., Any], *, request_model: Any, response_model: Any):
         self.name = name
         self.endpoint = endpoint
         self.request_model = request_model
         self.response_model = response_model
-        self.service = service
+        self._servicer = None
+
+    @property
+    def servicer(self):
+        return self._servicer
+
+    def __get__(self, instance, cls):
+        if self.servicer is None:
+            self._servicer = cls
+        if instance is None:
+            return self
+        else:
+            return functools.partial(self, instance)
+
+    def __set__(self, instance, value):
+        raise ValueError("Not allowed to modify Servicer Method.")
 
     async def __call__(self, request, context):
+        parameters = inspect.signature(self.endpoint).parameters
+        if "self" in parameters:
+            if len(parameters) == 2:
+                args = (None, request)
+            elif len(parameters) == 3:
+                args = (None, request, context)
+            else:
+                raise ValueError("rpc method need request and context two param")
+        else:
+            if len(parameters) == 1:
+                args = (request,)
+            elif len(parameters) == 2:
+                args = (request, context)
+            else:
+                raise ValueError("rpc method need request and context two param")
         if inspect.isasyncgenfunction(self.endpoint):
             raise NotImplementedError(f"{self.endpoint} is an async generator function, which is not supported.")
         elif inspect.iscoroutinefunction(self.endpoint):
-            response = await self.endpoint(request)
+            response = await self.endpoint(*args)
             return response
         else:
-            response = await await_sync_function(self.endpoint)(request)
+            response = await await_sync_function(self.endpoint)(*args)
             return response
+
+
+def method(name: str, request_model: Any, response_model: Any):
+    def decorator(endpoint):
+        return Method(
+            name=name,
+            endpoint=endpoint,
+            request_model=request_model,
+            response_model=response_model,
+        )
+
+    return decorator
```

### Comparing `python_fast_grpc-0.1.2/fast_grpc/types.py` & `python_fast_grpc-0.1.3/fast_grpc/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # -*- coding: utf-8 -*-
 from enum import IntEnum as _IntEnum
 from typing import TYPE_CHECKING, Awaitable, Callable, Generic, Optional, TypeVar
 
 from google.protobuf.message import Message
-from grpc.aio import ServicerContext
 from logzero import logger
 from pydantic import ConstrainedInt
 from pydantic.generics import GenericModel
 
 from fast_grpc.base import BaseSchema
+from fast_grpc.context import ServicerContext
 
-Handler = Callable[[BaseSchema, ServicerContext], Awaitable[BaseSchema]]
-App = Callable[[Message, ServicerContext, Handler], Awaitable[Message]]
+App = Callable[[Message, ServicerContext], Awaitable[Message]]
 
 if TYPE_CHECKING:
     Uint32 = int
     Uint64 = int
     Int32 = int
     Int64 = int
     Double = float
```

### Comparing `python_fast_grpc-0.1.2/fast_grpc/utils.py` & `python_fast_grpc-0.1.3/fast_grpc/utils.py`

 * *Files identical despite different names*

### Comparing `python_fast_grpc-0.1.2/pyproject.toml` & `python_fast_grpc-0.1.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-fast-grpc"
-version = "0.1.2"
+version = "0.1.3"
 description = "fast to code grpc in python"
 authors = ["taogeYT <li_yatao@outlook.com>"]
 readme = "README.md"
 packages = [{include = "fast_grpc"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `python_fast_grpc-0.1.2/PKG-INFO` & `python_fast_grpc-0.1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-fast-grpc
-Version: 0.1.2
+Version: 0.1.3
 Summary: fast to code grpc in python
 Author: taogeYT
 Author-email: li_yatao@outlook.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -16,43 +16,45 @@
 Requires-Dist: grpcio-tools (>=1.53.0,<2.0.0)
 Requires-Dist: logzero (>=1.7.0,<2.0.0)
 Requires-Dist: protobuf (>=4.22.0,<5.0.0)
 Requires-Dist: pydantic (>=1.10.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # fast-grpc
-fast to code grpc in Python 3.7+
+Fast to Code gRPC in Python 3.7+
 
 # Installation
 Require Python 3.7+
 ```shell
 pip install python-fast-grpc
 ```
 
 # Quick start
 1. Run a gRPC application
 ```python
-from fast_grpc import BaseSchema, FastGRPC
+from fast_grpc import BaseSchema, FastGRPC, ServicerContext, method
 
-rpc = FastGRPC("Greeter")
+app = FastGRPC()
 
 class HelloRequest(BaseSchema):
     name: str
 
 class HelloReply(BaseSchema):
     message: str
 
-@rpc.add_method("SayHello", request_model=HelloRequest, response_model=HelloReply)
-async def say_hello(request: HelloRequest) -> HelloReply:
-    return HelloReply(message=f"Hello {request.name}")
+class Greeter:
+    @method("SayHello", request_model=HelloRequest, response_model=HelloReply)
+    async def say_hello(self, request: HelloRequest, context: ServicerContext) -> HelloReply:
+        return HelloReply(message=f"Greeter SayHello {request.name}")
 
+app.add_service(Greeter)
 # this step will generate .proto file and python gRPC code, then start a grpc server
-rpc.run()
+app.run()
 ```
-2. run client invoke
+2. Client invoke
 ```python
 import grpc
 import greeter_pb2 as pb2
 import greeter_pb2_grpc as pb2_grpc
 
 channel = grpc.insecure_channel("127.0.0.1:50051")
 stub = pb2_grpc.GreeterStub(channel)
```

