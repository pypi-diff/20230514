# Comparing `tmp/enochecker3-0.8.0.tar.gz` & `tmp/enochecker3-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enochecker3-0.8.0.tar", last modified: Sun May 14 17:23:58 2023, max compression
+gzip compressed data, was "enochecker3-0.8.1.tar", last modified: Sun May 14 20:20:29 2023, max compression
```

## Comparing `enochecker3-0.8.0.tar` & `enochecker3-0.8.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:23:58.686290 enochecker3-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-14 17:23:45.000000 enochecker3-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-14 17:23:45.000000 enochecker3-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-14 17:23:58.686290 enochecker3-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-14 17:23:45.000000 enochecker3-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:23:58.686290 enochecker3-0.8.0/enochecker3/
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-14 17:23:45.000000 enochecker3-0.8.0/enochecker3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-14 17:23:45.000000 enochecker3-0.8.0/enochecker3/chaindb.py
--rw-r--r--   0 runner    (1001) docker     (123)    21915 2023-05-14 17:23:45.000000 enochecker3-0.8.0/enochecker3/enochecker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-14 17:23:45.000000 enochecker3-0.8.0/enochecker3/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:23:45.000000 enochecker3-0.8.0/enochecker3/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-14 17:23:45.000000 enochecker3-0.8.0/enochecker3/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-14 17:23:45.000000 enochecker3-0.8.0/enochecker3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:23:58.686290 enochecker3-0.8.0/enochecker3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-14 17:23:58.000000 enochecker3-0.8.0/enochecker3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-14 17:23:58.000000 enochecker3-0.8.0/enochecker3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 17:23:58.000000 enochecker3-0.8.0/enochecker3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 17:23:58.000000 enochecker3-0.8.0/enochecker3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-14 17:23:58.000000 enochecker3-0.8.0/enochecker3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-14 17:23:58.000000 enochecker3-0.8.0/enochecker3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-14 17:23:45.000000 enochecker3-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 17:23:58.686290 enochecker3-0.8.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1569 2023-05-14 17:23:45.000000 enochecker3-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:23:58.686290 enochecker3-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:23:45.000000 enochecker3-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-14 17:23:45.000000 enochecker3-0.8.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-14 17:23:45.000000 enochecker3-0.8.0/tests/test_chaindb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-14 17:23:45.000000 enochecker3-0.8.0/tests/test_dependency_injection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-14 17:23:45.000000 enochecker3-0.8.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-14 17:23:45.000000 enochecker3-0.8.0/tests/test_variant_ids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:20:29.287109 enochecker3-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-14 20:20:10.000000 enochecker3-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-14 20:20:10.000000 enochecker3-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-14 20:20:29.287109 enochecker3-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-14 20:20:10.000000 enochecker3-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:20:29.287109 enochecker3-0.8.1/enochecker3/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-14 20:20:10.000000 enochecker3-0.8.1/enochecker3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-14 20:20:10.000000 enochecker3-0.8.1/enochecker3/chaindb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21840 2023-05-14 20:20:10.000000 enochecker3-0.8.1/enochecker3/enochecker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-14 20:20:10.000000 enochecker3-0.8.1/enochecker3/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 20:20:10.000000 enochecker3-0.8.1/enochecker3/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-14 20:20:10.000000 enochecker3-0.8.1/enochecker3/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-14 20:20:10.000000 enochecker3-0.8.1/enochecker3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:20:29.287109 enochecker3-0.8.1/enochecker3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-14 20:20:29.000000 enochecker3-0.8.1/enochecker3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-14 20:20:29.000000 enochecker3-0.8.1/enochecker3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 20:20:29.000000 enochecker3-0.8.1/enochecker3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 20:20:29.000000 enochecker3-0.8.1/enochecker3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-14 20:20:29.000000 enochecker3-0.8.1/enochecker3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-14 20:20:29.000000 enochecker3-0.8.1/enochecker3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-14 20:20:10.000000 enochecker3-0.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 20:20:29.287109 enochecker3-0.8.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1569 2023-05-14 20:20:10.000000 enochecker3-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:20:29.287109 enochecker3-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 20:20:10.000000 enochecker3-0.8.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-14 20:20:10.000000 enochecker3-0.8.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-14 20:20:10.000000 enochecker3-0.8.1/tests/test_chaindb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-14 20:20:10.000000 enochecker3-0.8.1/tests/test_dependency_injection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-14 20:20:10.000000 enochecker3-0.8.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-14 20:20:10.000000 enochecker3-0.8.1/tests/test_variant_ids.py
```

### Comparing `enochecker3-0.8.0/LICENSE` & `enochecker3-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `enochecker3-0.8.0/PKG-INFO` & `enochecker3-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enochecker3
-Version: 0.8.0
+Version: 0.8.1
 Summary: FastAPI based library for building async python checkers for the EnoEngine A/D CTF Framework
 Home-page: https://github.com/ENOWARS/enochecker3
 Author: ldruschk
 Author-email: ldruschk@posteo.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `enochecker3-0.8.0/README.md` & `enochecker3-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `enochecker3-0.8.0/enochecker3/__init__.py` & `enochecker3-0.8.1/enochecker3/__init__.py`

 * *Files identical despite different names*

### Comparing `enochecker3-0.8.0/enochecker3/chaindb.py` & `enochecker3-0.8.1/enochecker3/chaindb.py`

 * *Files identical despite different names*

### Comparing `enochecker3-0.8.0/enochecker3/enochecker.py` & `enochecker3-0.8.1/enochecker3/enochecker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import contextlib
 import logging
 import os
 import sys
 import traceback
-from contextlib import AsyncExitStack, asynccontextmanager
+from contextlib import AsyncExitStack
 from inspect import Parameter, isawaitable, signature
 from types import TracebackType
 from typing import (
     Any,
     AsyncContextManager,
     AsyncIterator,
     Callable,
@@ -97,16 +97,16 @@
         exc_value: Optional[BaseException],
         traceback: Optional[TracebackType],
     ) -> Optional[bool]:
         return await self._exit_stack.__aexit__(exc_type, exc_value, traceback)
 
     async def get(self, t: type, name: str = "") -> Any:
         injector = self.checker.resolve_injector(name, t)
-        args = await self._exit_stack.enter_async_context(
-            self.checker._inject_dependencies(self.task, injector, None)
+        args = await self.checker._inject_dependencies(
+            self.task, injector, self._exit_stack
         )
         res = injector(*args)
         if isawaitable(res):
             res = await res
 
         if not hasattr(res, "__enter__") and not hasattr(res, "__aenter__"):
             return res
@@ -239,21 +239,21 @@
             if generic_key not in self._dependency_injections:
                 raise ValueError(
                     f"No registered dependency for name {key[0]} and/or type {key[1]}"
                 )
             return self._dependency_injections[generic_key]
         return self._dependency_injections[key]
 
-    @asynccontextmanager
     async def _inject_dependencies(
         self,
         task: BaseCheckerTaskMessage,
         f: Callable[..., Any],
+        stack: AsyncExitStack,
         dependencies: Optional[Set[Callable[..., Any]]] = None,
-    ) -> AsyncIterator[Any]:
+    ) -> List[Any]:
         dependencies = dependencies or set()
 
         sig = signature(f)
         task_message_type = METHOD_TO_TASK_MESSAGE_MAPPING[task.method]
 
         args: List[Union[AsyncContextManager[Any], Any]] = []
         for v in sig.parameters.values():
@@ -267,44 +267,45 @@
             else:
                 injector = self.resolve_injector(v.name, v.annotation)
                 if injector in dependencies:
                     raise CircularDependencyException(
                         f"Detected circular dependency in {f} with injected type {v.annotation}"
                     )
                 else:
-                    async with self._inject_dependencies(
-                        task, injector, dependencies.union([injector])
-                    ) as args_:
-                        arg = injector(*args_)
-                        if isawaitable(arg):
-                            arg = await arg
-                        args.append(arg)
-
-        async with AsyncExitStack() as stack:
-            # new_args contains the return values of __(a)enter__, which would be the "x" in "(async) with ... as x:"
-            new_args = []
-            for arg in args:
-                if not hasattr(arg, "__enter__") and not hasattr(arg, "__aenter__"):
-                    new_args.append(arg)
-                    continue
-                new_args.append(await stack.enter_async_context(arg))
-            yield new_args
+                    args_ = await self._inject_dependencies(
+                        task, injector, stack, dependencies.union([injector])
+                    )
+                    arg = injector(*args_)
+                    if isawaitable(arg):
+                        arg = await arg
+                    args.append(arg)
+
+        # new_args contains the return values of __(a)enter__, which would be the "x" in "(async) with ... as x:"
+        new_args = []
+        for arg in args:
+            if not hasattr(arg, "__enter__") and not hasattr(arg, "__aenter__"):
+                new_args.append(arg)
+                continue
+            new_args.append(await stack.enter_async_context(arg))
+        return new_args
 
     async def _call_method_raw(self, task: BaseCheckerTaskMessage) -> Optional[str]:
         variant_id = task.variant_id
         method = task.method
         try:
             f = self._method_variants[method][variant_id]
         except KeyError:
             raise AttributeError(
                 f"Variant_id {variant_id} not defined for method {method}"
             )
 
-        async with self._inject_dependencies(task, f) as args:
-            return await f(*args)
+        async with AsyncExitStack() as stack:
+            args = await self._inject_dependencies(task, f, stack)
+            res = await f(*args)
+        return res
 
     async def _call_method(self, task: BaseCheckerTaskMessage) -> Optional[str]:
         try:
             return await asyncio.wait_for(
                 self._call_method_raw(task),
                 timeout=(task.timeout / 1000) - TIMEOUT_BUFFER,
             )
```

### Comparing `enochecker3-0.8.0/enochecker3/logging.py` & `enochecker3-0.8.1/enochecker3/logging.py`

 * *Files identical despite different names*

### Comparing `enochecker3-0.8.0/enochecker3/types.py` & `enochecker3-0.8.1/enochecker3/types.py`

 * *Files identical despite different names*

### Comparing `enochecker3-0.8.0/enochecker3/utils.py` & `enochecker3-0.8.1/enochecker3/utils.py`

 * *Files identical despite different names*

### Comparing `enochecker3-0.8.0/enochecker3.egg-info/PKG-INFO` & `enochecker3-0.8.1/enochecker3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enochecker3
-Version: 0.8.0
+Version: 0.8.1
 Summary: FastAPI based library for building async python checkers for the EnoEngine A/D CTF Framework
 Home-page: https://github.com/ENOWARS/enochecker3
 Author: ldruschk
 Author-email: ldruschk@posteo.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `enochecker3-0.8.0/enochecker3.egg-info/SOURCES.txt` & `enochecker3-0.8.1/enochecker3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enochecker3-0.8.0/setup.py` & `enochecker3-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="enochecker3",
-    version="0.8.0",
+    version="0.8.1",
     author="ldruschk",
     author_email="ldruschk@posteo.de",
     description="FastAPI based library for building async python checkers for the EnoEngine A/D CTF Framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ENOWARS/enochecker3",
     packages=setuptools.find_packages(),
```

### Comparing `enochecker3-0.8.0/tests/conftest.py` & `enochecker3-0.8.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `enochecker3-0.8.0/tests/test_chaindb.py` & `enochecker3-0.8.1/tests/test_chaindb.py`

 * *Files identical despite different names*

### Comparing `enochecker3-0.8.0/tests/test_dependency_injection.py` & `enochecker3-0.8.1/tests/test_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `enochecker3-0.8.0/tests/test_utils.py` & `enochecker3-0.8.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `enochecker3-0.8.0/tests/test_variant_ids.py` & `enochecker3-0.8.1/tests/test_variant_ids.py`

 * *Files identical despite different names*

