# Comparing `tmp/enochecker3-0.7.1.tar.gz` & `tmp/enochecker3-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enochecker3-0.7.1.tar", last modified: Sun Oct 23 12:45:09 2022, max compression
+gzip compressed data, was "enochecker3-0.8.0.tar", last modified: Sun May 14 17:23:58 2023, max compression
```

## Comparing `enochecker3-0.7.1.tar` & `enochecker3-0.8.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 12:45:09.092661 enochecker3-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-10-23 12:45:00.000000 enochecker3-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-10-23 12:45:00.000000 enochecker3-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2762 2022-10-23 12:45:09.092661 enochecker3-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2123 2022-10-23 12:45:00.000000 enochecker3-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 12:45:09.088661 enochecker3-0.7.1/enochecker3/
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-10-23 12:45:00.000000 enochecker3-0.7.1/enochecker3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      978 2022-10-23 12:45:00.000000 enochecker3-0.7.1/enochecker3/chaindb.py
--rw-r--r--   0 runner    (1001) docker     (121)    21031 2022-10-23 12:45:00.000000 enochecker3-0.7.1/enochecker3/enochecker.py
--rw-r--r--   0 runner    (1001) docker     (121)     3310 2022-10-23 12:45:00.000000 enochecker3-0.7.1/enochecker3/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-23 12:45:00.000000 enochecker3-0.7.1/enochecker3/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     3588 2022-10-23 12:45:00.000000 enochecker3-0.7.1/enochecker3/types.py
--rw-r--r--   0 runner    (1001) docker     (121)      978 2022-10-23 12:45:00.000000 enochecker3-0.7.1/enochecker3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 12:45:09.092661 enochecker3-0.7.1/enochecker3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2762 2022-10-23 12:45:09.000000 enochecker3-0.7.1/enochecker3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-10-23 12:45:09.000000 enochecker3-0.7.1/enochecker3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-23 12:45:09.000000 enochecker3-0.7.1/enochecker3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-23 12:45:08.000000 enochecker3-0.7.1/enochecker3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-10-23 12:45:09.000000 enochecker3-0.7.1/enochecker3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-10-23 12:45:09.000000 enochecker3-0.7.1/enochecker3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-10-23 12:45:00.000000 enochecker3-0.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-23 12:45:09.092661 enochecker3-0.7.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1519 2022-10-23 12:45:00.000000 enochecker3-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 12:45:09.092661 enochecker3-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-23 12:45:00.000000 enochecker3-0.7.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      685 2022-10-23 12:45:00.000000 enochecker3-0.7.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-10-23 12:45:00.000000 enochecker3-0.7.1/tests/test_chaindb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1724 2022-10-23 12:45:00.000000 enochecker3-0.7.1/tests/test_dependency_injection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1488 2022-10-23 12:45:00.000000 enochecker3-0.7.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1790 2022-10-23 12:45:00.000000 enochecker3-0.7.1/tests/test_variant_ids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:23:58.686290 enochecker3-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-14 17:23:45.000000 enochecker3-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-14 17:23:45.000000 enochecker3-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-14 17:23:58.686290 enochecker3-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-14 17:23:45.000000 enochecker3-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:23:58.686290 enochecker3-0.8.0/enochecker3/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-14 17:23:45.000000 enochecker3-0.8.0/enochecker3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-14 17:23:45.000000 enochecker3-0.8.0/enochecker3/chaindb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21915 2023-05-14 17:23:45.000000 enochecker3-0.8.0/enochecker3/enochecker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-14 17:23:45.000000 enochecker3-0.8.0/enochecker3/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:23:45.000000 enochecker3-0.8.0/enochecker3/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-14 17:23:45.000000 enochecker3-0.8.0/enochecker3/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-14 17:23:45.000000 enochecker3-0.8.0/enochecker3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:23:58.686290 enochecker3-0.8.0/enochecker3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-14 17:23:58.000000 enochecker3-0.8.0/enochecker3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-14 17:23:58.000000 enochecker3-0.8.0/enochecker3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 17:23:58.000000 enochecker3-0.8.0/enochecker3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 17:23:58.000000 enochecker3-0.8.0/enochecker3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-14 17:23:58.000000 enochecker3-0.8.0/enochecker3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-14 17:23:58.000000 enochecker3-0.8.0/enochecker3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-14 17:23:45.000000 enochecker3-0.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 17:23:58.686290 enochecker3-0.8.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1569 2023-05-14 17:23:45.000000 enochecker3-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:23:58.686290 enochecker3-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:23:45.000000 enochecker3-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-14 17:23:45.000000 enochecker3-0.8.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-14 17:23:45.000000 enochecker3-0.8.0/tests/test_chaindb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-14 17:23:45.000000 enochecker3-0.8.0/tests/test_dependency_injection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-14 17:23:45.000000 enochecker3-0.8.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-14 17:23:45.000000 enochecker3-0.8.0/tests/test_variant_ids.py
```

### Comparing `enochecker3-0.7.1/LICENSE` & `enochecker3-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `enochecker3-0.7.1/PKG-INFO` & `enochecker3-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: enochecker3
-Version: 0.7.1
+Version: 0.8.0
 Summary: FastAPI based library for building async python checkers for the EnoEngine A/D CTF Framework
 Home-page: https://github.com/ENOWARS/enochecker3
 Author: ldruschk
 Author-email: ldruschk@posteo.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # enochecker3
 
 A FastAPI based checker library for writing async checkers in python. It is called enochecker3 even though enochecker2 never existed, because it is intended to be the reference implementation for version 3 of the enochecker API specification which is yet to come.
@@ -38,15 +39,15 @@
     Enochecker,
     GetflagCheckerTaskMessage,
     MumbleException,
     PutflagCheckerTaskMessage,
 )
 from enochecker3.utils import FlagSearcher, assert_equals, assert_in
 
-checker = Enochecker("ExampleChecker", 1337)
+checker = Enochecker("ExampleService", 1337)
 
 
 @checker.putflag(0)
 async def putflag_test(
     task: PutflagCheckerTaskMessage,
     client: AsyncClient,
     db: ChainDB,
```

### Comparing `enochecker3-0.7.1/README.md` & `enochecker3-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     Enochecker,
     GetflagCheckerTaskMessage,
     MumbleException,
     PutflagCheckerTaskMessage,
 )
 from enochecker3.utils import FlagSearcher, assert_equals, assert_in
 
-checker = Enochecker("ExampleChecker", 1337)
+checker = Enochecker("ExampleService", 1337)
 
 
 @checker.putflag(0)
 async def putflag_test(
     task: PutflagCheckerTaskMessage,
     client: AsyncClient,
     db: ChainDB,
```

### Comparing `enochecker3-0.7.1/enochecker3/__init__.py` & `enochecker3-0.8.0/enochecker3/__init__.py`

 * *Files identical despite different names*

### Comparing `enochecker3-0.7.1/enochecker3/chaindb.py` & `enochecker3-0.8.0/enochecker3/chaindb.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         val = await self.collection.find_one(
             {
                 "task_chain_id": self.task_chain_id,
                 "key": key,
             }
         )
         if val is None:
-            raise KeyError(f"key {key} not found")
+            raise KeyError(f"Key {key} not found")
         return val["value"]
 
     async def set(self, key: str, val: Any) -> None:
         await self.collection.replace_one(
             {
                 "task_chain_id": self.task_chain_id,
                 "key": key,
```

### Comparing `enochecker3-0.7.1/enochecker3/enochecker.py` & `enochecker3-0.8.0/enochecker3/enochecker.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,19 +95,16 @@
         self,
         exc_type: Optional[Type[BaseException]],
         exc_value: Optional[BaseException],
         traceback: Optional[TracebackType],
     ) -> Optional[bool]:
         return await self._exit_stack.__aexit__(exc_type, exc_value, traceback)
 
-    async def get(self, t: type) -> Any:
-        if t not in self.checker._dependency_injections:
-            raise ValueError(f"No registered dependency for type {t}")
-
-        injector = self.checker._dependency_injections[t]
+    async def get(self, t: type, name: str = "") -> Any:
+        injector = self.checker.resolve_injector(name, t)
         args = await self._exit_stack.enter_async_context(
             self.checker._inject_dependencies(self.task, injector, None)
         )
         res = injector(*args)
         if isawaitable(res):
             res = await res
 
@@ -119,15 +116,15 @@
 class Enochecker:
     def __init__(self, service_name: str, service_port: int):
         self.service_name: str = service_name
         self.service_port: int = service_port
 
         self.checker_name: str = service_name + "Checker"
 
-        self._dependency_injections: Dict[type, Callable[..., Any]] = {}
+        self._dependency_injections: Dict[Tuple[str, type], Callable[..., Any]] = {}
         self._logger: logging.Logger = logging.getLogger(__name__)
 
         handler = logging.StreamHandler(sys.stdout)
         if os.getenv("LOG_FORMAT") == "DEBUG":
             handler.setFormatter(DebugFormatter("%(message)s"))
         else:
             handler.setFormatter(ELKFormatter("%(message)s"))
@@ -162,15 +159,15 @@
         mongo_host = os.getenv("MONGO_HOST", "127.0.0.1")
         mongo_port = os.getenv("MONGO_PORT", 27017)
         mongo_user = os.getenv("MONGO_USER", None)
         mongo_password = os.getenv("MONGO_PASSWORD", None)
 
         if (mongo_user and not mongo_password) or (not mongo_user and mongo_password):
             raise ValueError(
-                "cannot set only MONGO_USER or MONGO_PASSWORD, must set none or both"
+                "Cannot set only MONGO_USER or MONGO_PASSWORD, must set none or both"
             )
 
         if mongo_user:
             connection_string = (
                 f"mongodb://{mongo_user}:{mongo_password}@{mongo_host}:{mongo_port}"
             )
         else:
@@ -204,15 +201,15 @@
             if variant_id < 0:
                 raise InvalidVariantIdsException(
                     f"variant_id {variant_id} must not be negative"
                 )
 
             if variant_id in self._method_variants[method]:
                 raise InvalidVariantIdsException(
-                    f"variant_id {variant_id} already defined for method {method}"
+                    f"Variant_id {variant_id} already defined for method {method}"
                 )
 
         def wrapper(f: Callable[..., Any]) -> None:
             for variant_id in variant_ids:
                 self._method_variants[method][variant_id] = f
 
         return wrapper
@@ -231,20 +228,31 @@
 
     def havoc(self, *variant_ids: int) -> Callable[[Callable[..., Any]], None]:
         return self._define_method(CheckerMethod.HAVOC, *variant_ids)
 
     def exploit(self, *variant_ids: int) -> Callable[[Callable[..., Any]], None]:
         return self._define_method(CheckerMethod.EXPLOIT, *variant_ids)
 
+    def resolve_injector(self, name: str, t: type) -> Callable[..., Any]:
+        key: Tuple[str, type] = (name.split("_", 1)[0], t)
+        if key not in self._dependency_injections:
+            generic_key: Tuple[str, type] = ("", t)
+            if generic_key not in self._dependency_injections:
+                raise ValueError(
+                    f"No registered dependency for name {key[0]} and/or type {key[1]}"
+                )
+            return self._dependency_injections[generic_key]
+        return self._dependency_injections[key]
+
     @asynccontextmanager
     async def _inject_dependencies(
         self,
         task: BaseCheckerTaskMessage,
         f: Callable[..., Any],
-        dependencies: Optional[Set[type]] = None,
+        dependencies: Optional[Set[Callable[..., Any]]] = None,
     ) -> AsyncIterator[Any]:
         dependencies = dependencies or set()
 
         sig = signature(f)
         task_message_type = METHOD_TO_TASK_MESSAGE_MAPPING[task.method]
 
         args: List[Union[AsyncContextManager[Any], Any]] = []
@@ -252,27 +260,28 @@
             try:
                 subclass = issubclass(task_message_type, v.annotation)
             except TypeError:
                 # subscripted generics, e.g. AsyncSocket = Tuple[..., ...], cannot be used in issubclass
                 subclass = False
             if subclass:
                 args.append(task)
-            elif v.annotation in dependencies:
-                raise CircularDependencyException(
-                    f"detected circular dependency in {f} with injected type {v.annotation}"
-                )
             else:
-                injector = self._dependency_injections[v.annotation]
-                async with self._inject_dependencies(
-                    task, injector, dependencies.union([v.annotation])
-                ) as args_:
-                    arg = injector(*args_)
-                    if isawaitable(arg):
-                        arg = await arg
-                    args.append(arg)
+                injector = self.resolve_injector(v.name, v.annotation)
+                if injector in dependencies:
+                    raise CircularDependencyException(
+                        f"Detected circular dependency in {f} with injected type {v.annotation}"
+                    )
+                else:
+                    async with self._inject_dependencies(
+                        task, injector, dependencies.union([injector])
+                    ) as args_:
+                        arg = injector(*args_)
+                        if isawaitable(arg):
+                            arg = await arg
+                        args.append(arg)
 
         async with AsyncExitStack() as stack:
             # new_args contains the return values of __(a)enter__, which would be the "x" in "(async) with ... as x:"
             new_args = []
             for arg in args:
                 if not hasattr(arg, "__enter__") and not hasattr(arg, "__aenter__"):
                     new_args.append(arg)
@@ -283,41 +292,53 @@
     async def _call_method_raw(self, task: BaseCheckerTaskMessage) -> Optional[str]:
         variant_id = task.variant_id
         method = task.method
         try:
             f = self._method_variants[method][variant_id]
         except KeyError:
             raise AttributeError(
-                f"variant_id {variant_id} not defined for method {method}"
+                f"Variant_id {variant_id} not defined for method {method}"
             )
 
         async with self._inject_dependencies(task, f) as args:
             return await f(*args)
 
     async def _call_method(self, task: BaseCheckerTaskMessage) -> Optional[str]:
         try:
             return await asyncio.wait_for(
                 self._call_method_raw(task),
                 timeout=(task.timeout / 1000) - TIMEOUT_BUFFER,
             )
+        except (MumbleException, OfflineException, InternalErrorException):
+            raise
         except asyncio.IncompleteReadError:
             trace = traceback.format_exc()
             logger = self._get_logger_adapter(task)
             logger.error(f"Service connection closed abruptly\n{trace}")
             raise MumbleException("Service connection closed abruptly")
         except asyncio.TimeoutError:
             trace = traceback.format_exc()
             logger = self._get_logger_adapter(task)
             logger.error(f"Service is responding too slow\n{trace}")
             raise MumbleException("Service is responding too slow")
-        except (httpx.ConnectTimeout, httpx.ConnectError, httpx.RemoteProtocolError):
+        except (
+            httpx.ConnectTimeout,
+            httpx.ConnectError,
+            httpx.ReadTimeout,
+            httpx.RemoteProtocolError,
+        ):
             trace = traceback.format_exc()
             logger = self._get_logger_adapter(task)
             logger.info(f"HTTP connection to service failed\n{trace}")
             raise OfflineException("HTTP connection to service failed")
+        except Exception as e:
+            trace = traceback.format_exc()
+            logger = self._get_logger_adapter(task)
+            logger.info(f"Checker internal error\n{trace}")
+            raise InternalErrorException("Checker internal error", e)
 
     async def _call_putflag(
         self, task: PutflagCheckerTaskMessage
     ) -> CheckerResultMessage:
         attack_info: Optional[str] = await self._call_method(task)
         return CheckerResultMessage(
             result=CheckerTaskResult.OK, attack_info=attack_info
@@ -355,24 +376,33 @@
             )
         return CheckerResultMessage(result=CheckerTaskResult.OK, flag=flag)
 
     ########################
     # Dependency Injection #
     ########################
 
-    def register_dependency(self, f: Callable[..., Any]) -> None:
-        sig = signature(f)
-        if sig.return_annotation == Parameter.empty:
-            raise AttributeError(f"missing return annotation for {f.__name__}")
-        if sig.return_annotation in self._dependency_injections:
-            raise ValueError(
-                f"already registered a dependency with return type {sig.return_annotation}"
-            )
+    def register_named_dependency(self, name: str = "") -> Callable[..., Any]:
+        def decorator(f: Callable[..., Any]) -> Callable[..., Any]:
+            sig = signature(f)
+            key: Tuple[str, type] = (name.split("_", 1)[0], sig.return_annotation)
+            if sig.return_annotation == Parameter.empty:
+                raise AttributeError(f"missing return annotation for {f.__name__}")
+            if key in self._dependency_injections:
+                raise ValueError(
+                    f"already registered a dependency with name {key[0]} and type {key[1]}"
+                )
+
+            self._dependency_injections[key] = f
+
+            return f
 
-        self._dependency_injections[sig.return_annotation] = f
+        return decorator
+
+    def register_dependency(self, f: Callable[..., Any]) -> Callable[..., Any]:
+        return self.register_named_dependency("")(f)
 
     def _get_http_client(self, task: BaseCheckerTaskMessage) -> httpx.AsyncClient:
         return httpx.AsyncClient(
             base_url=f"http://{task.address}:{self.service_port}", verify=False
         )
 
     def _get_chaindb(self, task: BaseCheckerTaskMessage) -> ChainDB:
@@ -429,22 +459,22 @@
     #########################
 
     def _validate_variant_ids(self) -> Tuple[int, int, int, int]:
         putflag_keys = self._method_variants[CheckerMethod.PUTFLAG].keys()
         getflag_keys = self._method_variants[CheckerMethod.GETFLAG].keys()
         if putflag_keys != getflag_keys:
             raise InvalidVariantIdsException(
-                "mismatch between putflag and getflag variants"
+                "Mismatch between putflag and getflag variants"
             )
 
         putnoise_keys = self._method_variants[CheckerMethod.PUTNOISE].keys()
         getnoise_keys = self._method_variants[CheckerMethod.GETNOISE].keys()
         if putnoise_keys != getnoise_keys:
             raise InvalidVariantIdsException(
-                "mismatch between putnoise and getnoise variants"
+                "Mismatch between putnoise and getnoise variants"
             )
 
         for method in self._method_variants.keys():
             self._ensure_sequential_variant_ids(method)
 
         return (
             len(self._method_variants[CheckerMethod.PUTFLAG]),
@@ -541,26 +571,18 @@
                 trace = traceback.format_exc()
                 logger.info(f"Encountered offline exception:\n{trace}")
                 return CheckerResultMessage(
                     result=CheckerTaskResult.OFFLINE, message=e.message
                 )
             except InternalErrorException as e:
                 trace = traceback.format_exc()
-                logger.info(f"Encountered explicit internal error exception:\n{trace}")
+                logger.info(f"Encountered internal error exception:\n{trace}")
                 return CheckerResultMessage(
                     result=CheckerTaskResult.INTERNAL_ERROR, message=e.message
                 )
-            except Exception as e:
-                traceback.print_exc()
-                trace = traceback.format_exc()
-                logger.critical(f"Encountered internal exception:\n{trace}")
-                return CheckerResultMessage(
-                    result=CheckerTaskResult.INTERNAL_ERROR,
-                    message=f"Unhandled exception of type {type(e)}",
-                )
 
         app.on_event("startup")(self._init)
 
         return app
 
     def run(self, port: Optional[int] = None) -> None:
         uvicorn.run(self.app, host="127.0.0.1", port=port or 8000)
```

### Comparing `enochecker3-0.7.1/enochecker3/logging.py` & `enochecker3-0.8.0/enochecker3/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,19 @@
             record, "checker_task", None
         )
 
         timestamp: str = datetime.datetime.utcnow().strftime("%H:%M:%S.%f")[:-3]
         method: str = getattr(checker_task, "method", None) or "<method>"
         levelname: str = getattr(record, "levelname", None) or "<level>"
         task_id: str = getattr(checker_task, "task_id", None) or "<taskid>"
-        prefix: str = "{} {} {} {} : ".format(timestamp, levelname, method, task_id)
+        info_line: str = "{} {} {} {}".format(timestamp, levelname, method, task_id)
 
-        log_lines: List[str] = []
-        for line in record.msg.strip().split("\n"):
-            log_lines.append(prefix + line)
+        log_lines: List[str] = [info_line]
+        for i, line in enumerate(record.msg.strip().split("\n")):
+            log_lines.append("    | " + line)
 
         return "\n".join(log_lines)
 
 
 class ELKFormatter(logging.Formatter):
     def format(self, record: logging.LogRecord) -> str:
         if type(record.args) is tuple and len(record.args) > 0:
```

### Comparing `enochecker3-0.7.1/enochecker3/types.py` & `enochecker3-0.8.0/enochecker3/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -139,15 +139,17 @@
 
 
 class OfflineException(BaseException):
     pass
 
 
 class InternalErrorException(BaseException):
-    pass
+    def __init__(self, message: Optional[str], inner: Optional[Exception] = None):
+        super().__init__(message)
+        self.inner: Optional[Exception] = inner
 
 
 class EnoLogMessage(BaseModel):
     tool: str
     type: str
     severity: str
     severity_level: int
```

### Comparing `enochecker3-0.7.1/enochecker3.egg-info/PKG-INFO` & `enochecker3-0.8.0/enochecker3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: enochecker3
-Version: 0.7.1
+Version: 0.8.0
 Summary: FastAPI based library for building async python checkers for the EnoEngine A/D CTF Framework
 Home-page: https://github.com/ENOWARS/enochecker3
 Author: ldruschk
 Author-email: ldruschk@posteo.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # enochecker3
 
 A FastAPI based checker library for writing async checkers in python. It is called enochecker3 even though enochecker2 never existed, because it is intended to be the reference implementation for version 3 of the enochecker API specification which is yet to come.
@@ -38,15 +39,15 @@
     Enochecker,
     GetflagCheckerTaskMessage,
     MumbleException,
     PutflagCheckerTaskMessage,
 )
 from enochecker3.utils import FlagSearcher, assert_equals, assert_in
 
-checker = Enochecker("ExampleChecker", 1337)
+checker = Enochecker("ExampleService", 1337)
 
 
 @checker.putflag(0)
 async def putflag_test(
     task: PutflagCheckerTaskMessage,
     client: AsyncClient,
     db: ChainDB,
```

### Comparing `enochecker3-0.7.1/enochecker3.egg-info/SOURCES.txt` & `enochecker3-0.8.0/enochecker3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enochecker3-0.7.1/setup.py` & `enochecker3-0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="enochecker3",
-    version="0.7.1",
+    version="0.8.0",
     author="ldruschk",
     author_email="ldruschk@posteo.de",
     description="FastAPI based library for building async python checkers for the EnoEngine A/D CTF Framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ENOWARS/enochecker3",
     packages=setuptools.find_packages(),
@@ -31,11 +31,12 @@
         "License :: OSI Approved :: MIT License",
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     zip_safe=False,  # This might be needed for requirements.txt
     python_requires=">=3.7",
 )
```

### Comparing `enochecker3-0.7.1/tests/conftest.py` & `enochecker3-0.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `enochecker3-0.7.1/tests/test_chaindb.py` & `enochecker3-0.8.0/tests/test_chaindb.py`

 * *Files identical despite different names*

### Comparing `enochecker3-0.7.1/tests/test_dependency_injection.py` & `enochecker3-0.8.0/tests/test_dependency_injection.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from enochecker3 import Enochecker, HavocCheckerTaskMessage
+from enochecker3 import Enochecker, HavocCheckerTaskMessage, InternalErrorException
 from enochecker3.enochecker import CircularDependencyException
 
 
 @pytest.fixture
 def havoc_task() -> HavocCheckerTaskMessage:
     return HavocCheckerTaskMessage(
         task_id=0,
@@ -29,14 +29,31 @@
     async def havoc(param: str):
         assert param == "123"
 
     await checker._call_havoc(havoc_task)
 
 
 @pytest.mark.asyncio
+async def test_unnamed(checker: Enochecker, havoc_task: HavocCheckerTaskMessage):
+    @checker.register_dependency
+    def inject_string() -> str:
+        return "123"
+
+    @checker.register_named_dependency("special")
+    def inject_special_string() -> str:
+        return "456"
+
+    @checker.havoc(0)
+    async def havoc(a: str, b: str, special: str):
+        assert a == "123" and b == "123" and special == "456"
+
+    await checker._call_havoc(havoc_task)
+
+
+@pytest.mark.asyncio
 async def test_recursive_dependency(
     checker: Enochecker, havoc_task: HavocCheckerTaskMessage
 ):
     @checker.register_dependency
     def inject_string(x: int) -> str:
         return f"int: {x}"
 
@@ -63,9 +80,10 @@
     def inject_integer(x: str) -> int:
         return len(x)
 
     @checker.havoc(0)
     async def havoc(param: str):
         pass
 
-    with pytest.raises(CircularDependencyException):
+    with pytest.raises(InternalErrorException) as exc_info:
         await checker._call_havoc(havoc_task)
+    assert type(exc_info.value.inner) == CircularDependencyException
```

### Comparing `enochecker3-0.7.1/tests/test_utils.py` & `enochecker3-0.8.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `enochecker3-0.7.1/tests/test_variant_ids.py` & `enochecker3-0.8.0/tests/test_variant_ids.py`

 * *Files identical despite different names*

