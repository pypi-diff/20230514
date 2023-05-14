# Comparing `tmp/meiga-1.8.3.tar.gz` & `tmp/meiga-1.9.0.tar.gz`

## Comparing `meiga-1.8.3.tar` & `meiga-1.9.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/VERSION
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/__init__.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/alias.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/deprecation.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/error.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/handlers.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/misc.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/no_given_value.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/on_failure_exception.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/public_api.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/py.typed
--rw-r--r--   0        0        0     7432 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/result.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/assertions/__init__.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/assertions/assert_failure.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/assertions/assert_success.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/decorators/__init__.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/decorators/early_return.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/decorators/to_result.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/decorators/unexpected_decoration_order_error.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 meiga-1.8.3/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 meiga-1.8.3/LICENSE
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 meiga-1.8.3/README.md
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 meiga-1.8.3/pyproject.toml
--rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 meiga-1.8.3/PKG-INFO
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/VERSION
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/__init__.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/alias.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/deprecation.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/error.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/handlers.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/misc.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/no_given_value.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/on_failure_exception.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/public_api.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/py.typed
+-rw-r--r--   0        0        0    10392 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/result.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/assertions/__init__.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/assertions/assert_failure.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/assertions/assert_success.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/decorators/__init__.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/decorators/early_return.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/decorators/to_result.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 meiga-1.9.0/meiga/decorators/unexpected_decoration_order_error.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 meiga-1.9.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 meiga-1.9.0/LICENSE
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 meiga-1.9.0/README.md
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 meiga-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 meiga-1.9.0/PKG-INFO
```

### Comparing `meiga-1.8.3/meiga/alias.py` & `meiga-1.9.0/meiga/alias.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,13 +14,12 @@
 class Failure(Generic[TF], Result[Any, TF]):
     __match_args__ = ("_value_failure",)
 
     def __init__(self, error: TF = cast(TF, Error())) -> None:
         super().__init__(failure=error)
 
 
-isSuccess: Result = Success()
-isFailure: Result = Failure()
-NotImplementedMethodError: Result = isFailure
-
 BoolResult = Result[bool, Error]
 AnyResult = Result[Any, Error]
+isSuccess: AnyResult = Success()
+isFailure: AnyResult = Failure()
+NotImplementedMethodError: AnyResult = isFailure
```

### Comparing `meiga-1.8.3/meiga/deprecation.py` & `meiga-1.9.0/meiga/deprecation.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-from typing import Dict, Union
+from __future__ import annotations
+
+from typing import Any
 
 from meiga.handlers import OnFailureHandler, OnSuccessHandler
 
 
 def get_on_success_handler_from_deprecated_args(
-    kwargs: Dict,
-) -> Union[OnSuccessHandler, None]:
+    kwargs: dict[Any, Any]
+) -> OnSuccessHandler | None:
     on_success = kwargs.get("on_success")
     if on_success:
         return OnSuccessHandler(func=on_success, args=kwargs.get("success_args"))
     return None
 
 
 def get_on_failure_handler_from_deprecated_args(
-    kwargs: Dict,
-) -> Union[OnFailureHandler, None]:
+    kwargs: dict[Any, Any],
+) -> OnFailureHandler | None:
     on_failure = kwargs.get("on_failure")
     if on_failure:
         return OnFailureHandler(func=on_failure, args=kwargs.get("failure_args"))
     return None
```

### Comparing `meiga-1.8.3/meiga/handlers.py` & `meiga-1.9.0/meiga/handlers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,25 @@
-from typing import Callable, Iterable, Optional
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Any, Callable, Iterable
 
 from meiga.misc import get_args_list
 
+if TYPE_CHECKING:  # pragma: no cover
+    from meiga.result import TF, TS, Result
+
 
 class Handler:
-    def __init__(self, func: Callable[..., None], args: Optional[Iterable] = None):
+    def __init__(
+        self, func: Callable[..., None], args: Iterable[Any] | None = None
+    ) -> None:
         self.func = func
         self.args = args
 
-    def execute(self, result) -> None:
+    def execute(self, result: Result[TS, TF]) -> None:
         if self.args is not None:
             failure_args = get_args_list(self.args)
             if result.__id__ in failure_args:
                 index_meiga_result = failure_args.index(result.__id__)
                 failure_args[index_meiga_result] = result
             self.func(*tuple(failure_args))
         else:
```

### Comparing `meiga-1.8.3/meiga/public_api.py` & `meiga-1.9.0/meiga/public_api.py`

 * *Files identical despite different names*

### Comparing `meiga-1.8.3/meiga/assertions/assert_failure.py` & `meiga-1.9.0/meiga/assertions/assert_failure.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import TYPE_CHECKING, Any, Optional, Type
+from typing import TYPE_CHECKING, Any, Type, Union
 
 if TYPE_CHECKING:  # pragma: no cover
-    from meiga.result import Result
+    from meiga.result import TF, TS, Result
 
 
 def assert_failure(
-    result: "Result",
-    value_is_instance_of: Optional[Type] = None,
-    value_is_equal_to: Optional[Any] = None,
+    result: "Result[TS, TF]",
+    value_is_instance_of: Union[Type[Any], None] = None,
+    value_is_equal_to: Union[Any, None] = None,
 ) -> None:
     assert (
         result.is_failure
     ), f"result is not failure as expected. Given failure value is {result.value}"
     if value_is_instance_of:
         assert isinstance(result.value, value_is_instance_of), (
             f"Value is not instance of {value_is_instance_of}. "
```

### Comparing `meiga-1.8.3/meiga/assertions/assert_success.py` & `meiga-1.9.0/meiga/assertions/assert_success.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import TYPE_CHECKING, Any, Optional, Type
+from typing import TYPE_CHECKING, Any, Type, Union
 
 if TYPE_CHECKING:  # pragma: no cover
-    from meiga.result import Result
+    from meiga.result import TF, TS, Result
 
 
 def assert_success(
-    result: "Result",
-    value_is_instance_of: Optional[Type] = None,
-    value_is_equal_to: Optional[Any] = None,
+    result: "Result[TS, TF]",
+    value_is_instance_of: Union[Type[Any], None] = None,
+    value_is_equal_to: Union[Any, None] = None,
 ) -> None:
     assert (
         result.is_success
     ), f"result is not success as expected. Given failure value is {result.value}"
     if value_is_instance_of:
         assert isinstance(result.value, value_is_instance_of), (
             f"Value is not instance of {value_is_instance_of}. "
```

### Comparing `meiga-1.8.3/meiga/decorators/early_return.py` & `meiga-1.9.0/meiga/decorators/to_result.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,33 @@
 import sys
 from functools import wraps
-from typing import Callable, TypeVar, cast
+from typing import Any, Callable, TypeVar, cast
 
 if sys.version_info < (3, 10):  # pragma: no cover
     from typing_extensions import ParamSpec
 else:
     from typing import ParamSpec
 
 from meiga.alias import Failure
 from meiga.decorators.unexpected_decoration_order_error import (
     UnexpectedDecorationOrderError,
 )
-from meiga.error import Error
-from meiga.on_failure_exception import OnFailureException
 from meiga.result import Result
 
 P = ParamSpec("P")
-R = TypeVar("R", bound=Result)
+R = TypeVar("R", bound=Result[Any, Any])
 
 
-def early_return(func: Callable[P, R]) -> Callable[P, R]:
+def to_result(func: Callable[P, R]) -> Callable[P, R]:
     @wraps(func)
-    def _early_return(*args: P.args, **kwargs: P.kwargs) -> R:
+    def _to_result(*args: P.args, **kwargs: P.kwargs) -> R:
         try:
             if isinstance(func, staticmethod):
                 return Failure(UnexpectedDecorationOrderError())
             elif isinstance(func, classmethod):
                 return Failure(UnexpectedDecorationOrderError())
             else:
                 return func(*args, **kwargs)
-        except OnFailureException as exc:
-            return cast(R, exc.result)
-        except Error as error:
-            return cast(R, Failure(error))
+        except Exception as exc:
+            return cast(R, Failure(exc))
 
-    return _early_return
-
-
-meiga = early_return  # To keep compatibility (Now this is deprecated)
+    return _to_result
```

### Comparing `meiga-1.8.3/.gitignore` & `meiga-1.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `meiga-1.8.3/LICENSE` & `meiga-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meiga-1.8.3/README.md` & `meiga-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `meiga-1.8.3/pyproject.toml` & `meiga-1.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `meiga-1.8.3/PKG-INFO` & `meiga-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meiga
-Version: 1.8.3
+Version: 1.9.0
 Summary: A simple, typed and monad-based Result type for Python
 Project-URL: Documentation, https://alice-biometrics.github.io/meiga/
 Project-URL: Homepage, https://github.com/alice-biometrics/meiga
 Author-email: Alice Biometrics <support@alicebiometrics.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: Monad,Result,Typed,Typing,result-type
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: meiga Version: 1.8.3 Summary: A simple, typed and
+Metadata-Version: 2.1 Name: meiga Version: 1.9.0 Summary: A simple, typed and
 monad-based Result type for Python Project-URL: Documentation, https://alice-
 biometrics.github.io/meiga/ Project-URL: Homepage, https://github.com/alice-
 biometrics/meiga Author-email: Alice Biometrics
 alicebiometrics.com> License-Expression: MIT License-File: LICENSE Keywords:
 Monad,Result,Typed,Typing,result-type Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: System Administrators Classifier: License :: OSI Approved
```

