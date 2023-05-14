# Comparing `tmp/wraps-0.4.0.tar.gz` & `tmp/wraps-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wraps-0.4.0.tar", max compression
+gzip compressed data, was "wraps-0.5.0.tar", max compression
```

## Comparing `wraps-0.4.0.tar` & `wraps-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0     1092 2023-04-24 21:34:43.395506 wraps-0.4.0/LICENSE
--rw-r--r--   0        0        0     6490 2023-04-24 21:34:43.395506 wraps-0.4.0/README.md
--rw-r--r--   0        0        0     3331 2023-04-24 21:34:43.399508 wraps-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2526 2023-04-24 21:34:43.399508 wraps-0.4.0/wraps/__init__.py
--rw-r--r--   0        0        0     2852 2023-04-24 21:34:43.399508 wraps-0.4.0/wraps/early.py
--rw-r--r--   0        0        0    15275 2023-04-24 21:34:43.399508 wraps-0.4.0/wraps/either.py
--rw-r--r--   0        0        0     1187 2023-04-24 21:34:43.399508 wraps-0.4.0/wraps/errors.py
--rw-r--r--   0        0        0     3952 2023-04-24 21:34:43.399508 wraps-0.4.0/wraps/future.py
--rw-r--r--   0        0        0     1134 2023-04-24 21:34:43.399508 wraps-0.4.0/wraps/future_either.py
--rw-r--r--   0        0        0     9285 2023-04-24 21:34:43.399508 wraps-0.4.0/wraps/future_option.py
--rw-r--r--   0        0        0    14054 2023-04-24 21:34:43.399508 wraps-0.4.0/wraps/future_result.py
--rw-r--r--   0        0        0    40999 2023-04-24 21:34:43.399508 wraps-0.4.0/wraps/option.py
--rw-r--r--   0        0        0        0 2023-04-24 21:34:43.399508 wraps-0.4.0/wraps/py.typed
--rw-r--r--   0        0        0     1809 2023-04-24 21:34:43.399508 wraps-0.4.0/wraps/reawaitable.py
--rw-r--r--   0        0        0    53456 2023-04-24 21:34:43.399508 wraps-0.4.0/wraps/result.py
--rw-r--r--   0        0        0      604 2023-04-24 21:34:43.399508 wraps-0.4.0/wraps/utils.py
--rw-r--r--   0        0        0     9436 2023-04-24 21:34:43.399508 wraps-0.4.0/wraps/wraps.py
--rw-r--r--   0        0        0     7742 1970-01-01 00:00:00.000000 wraps-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-14 13:50:08.282964 wraps-0.5.0/LICENSE
+-rw-r--r--   0        0        0     6517 2023-05-14 13:50:08.282964 wraps-0.5.0/README.md
+-rw-r--r--   0        0        0     3332 2023-05-14 13:50:08.286964 wraps-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2566 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/__init__.py
+-rw-r--r--   0        0        0     2852 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/early.py
+-rw-r--r--   0        0        0    15275 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/either.py
+-rw-r--r--   0        0        0     1226 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/errors.py
+-rw-r--r--   0        0        0     4377 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/future.py
+-rw-r--r--   0        0        0     1360 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/future_either.py
+-rw-r--r--   0        0        0    12014 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/future_option.py
+-rw-r--r--   0        0        0    15807 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/future_result.py
+-rw-r--r--   0        0        0      340 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/markers.py
+-rw-r--r--   0        0        0    41149 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/option.py
+-rw-r--r--   0        0        0        0 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/py.typed
+-rw-r--r--   0        0        0     1809 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/reawaitable.py
+-rw-r--r--   0        0        0    53507 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/result.py
+-rw-r--r--   0        0        0      853 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/typing.py
+-rw-r--r--   0        0        0      604 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/utils.py
+-rw-r--r--   0        0        0     9422 2023-05-14 13:50:08.286964 wraps-0.5.0/wraps/wraps.py
+-rw-r--r--   0        0        0     7769 1970-01-01 00:00:00.000000 wraps-0.5.0/PKG-INFO
```

### Comparing `wraps-0.4.0/LICENSE` & `wraps-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wraps-0.4.0/README.md` & `wraps-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 $ poetry add wraps
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-wraps = "^0.4.0"
+wraps = "^0.5.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.wraps]
 git = "https://github.com/nekitdev/wraps.git"
@@ -100,15 +100,15 @@
 
 def divide(numerator: float, denominator: float) -> Result[float, DivideError]:
     return Ok(numerator / denominator) if denominator else Error(DivideError.DIVISION_BY_ZERO)
 ```
 
 ### Early Return
 
-Early return functionality (`?` operator in Rust) is implemented via `early` methods
+Early return functionality (like the *question-mark* (`?`) operator in Rust) is implemented via `early` methods
 (for both [`Option`][wraps.option.Option] and [`Result`][wraps.result.Result] types)
 combined with the [`@early_option`][wraps.early.early_option] and
 [`@early_result`][wraps.early.early_result] decorators respectively.
 
 ```python
 from wraps import Option, early_option, wrap_option
```

### Comparing `wraps-0.4.0/pyproject.toml` & `wraps-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wraps"
-version = "0.4.0"
+version = "0.5.0"
 description = "Meaningful and safe wrapping types."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/wraps"
@@ -30,16 +30,16 @@
 include = "wraps"
 
 [tool.poetry.dependencies]
 python = ">= 3.7"
 
 attrs = ">= 23.1.0"
 
-funcs = ">= 0.5.0"
-async-extensions = ">= 1.2.2"
+funcs = ">= 0.5.1"
+async-extensions = ">= 1.2.3"
 typing-extensions = ">= 4.5.0"
 
 [tool.poetry.group.format]
 optional = true
 
 [tool.poetry.group.format.dependencies]
 black = "23.3.0"
@@ -53,38 +53,38 @@
 version = "5.12.0"
 python = ">= 3.8"
 
 [tool.poetry.group.check]
 optional = true
 
 [tool.poetry.group.check.dependencies]
-mypy = "1.2.0"
+mypy = "1.3.0"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "7.3.1"
 pytest-cov = "4.0.0"
 anyio = "3.6.2"
 trio = "0.22.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-mkdocs = "1.4.2"
-mkdocs-material = "9.1.8"
+mkdocs = "1.4.3"
+mkdocs-material = "9.1.12"
 
 [tool.poetry.group.docs.dependencies.mkdocstrings]
 version = "0.21.2"
 extras = ["python"]
 
 [tool.poetry.group.dev.dependencies]
-changelogging = "1.1.0"
+changelogging = "1.2.0"
 
 [tool.black]
 line_length = 100
 
 [tool.flake8]
 max_line_length = 100
 ignore = [
@@ -141,15 +141,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "wraps"
-version = "0.4.0"
+version = "0.5.0"
 url = "https://github.com/nekitdev/wraps"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `wraps-0.4.0/wraps/__init__.py` & `wraps-0.5.0/wraps/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 __description__ = "Meaningful and safe wrapping types."
 __url__ = "https://github.com/nekitdev/wraps"
 
 __title__ = "wraps"
 __author__ = "nekitdev"
 __license__ = "MIT"
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
 from wraps.early import early_option, early_option_await, early_result, early_result_await
 from wraps.either import Either, Left, Right, is_left, is_right
 from wraps.errors import Panic, panic
 from wraps.future import Future
 from wraps.future_option import FutureOption
 from wraps.future_result import FutureResult
@@ -40,14 +40,15 @@
     WrapResultAwait,
     wrap_future,
     wrap_future_either,
     wrap_future_option,
     wrap_future_result,
     wrap_option,
     wrap_option_await,
+    wrap_optional,
     wrap_result,
     wrap_result_await,
 )
 
 __all__ = (
     # option
     "Option",
@@ -87,14 +88,15 @@
     # wraps
     "WrapOption",
     "WrapOptionAwait",
     "WrapResult",
     "WrapResultAwait",
     "wrap_option",
     "wrap_option_await",
+    "wrap_optional",
     "wrap_result",
     "wrap_result_await",
     "wrap_future",
     "wrap_future_option",
     "wrap_future_result",
     "wrap_future_either",
 )
```

### Comparing `wraps-0.4.0/wraps/early.py` & `wraps-0.5.0/wraps/early.py`

 * *Files identical despite different names*

### Comparing `wraps-0.4.0/wraps/either.py` & `wraps-0.5.0/wraps/either.py`

 * *Files identical despite different names*

### Comparing `wraps-0.4.0/wraps/errors.py` & `wraps-0.5.0/wraps/errors.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Panics and early return errors."""
+
 from typing import Generic, TypeVar
 
 from funcs.typing import AnyError
 from typing_extensions import Never
 
 __all__ = ("Panic", "panic", "EarlyOption", "EarlyResult")
```

### Comparing `wraps-0.4.0/wraps/future.py` & `wraps-0.5.0/wraps/future.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,95 +1,116 @@
+"""Asynchronous computation using futures."""
+
 from __future__ import annotations
 
 from typing import AsyncIterator, Awaitable, Generator, TypeVar
 
-from attrs import define, field
+from attrs import field, frozen
 from funcs.typing import AsyncUnary, Unary
 
 from wraps.reawaitable import ReAwaitable
 from wraps.utils import async_identity, identity
 
 __all__ = ("Future",)
 
 T = TypeVar("T", covariant=True)
 U = TypeVar("U")
 
+
 # NOTE: functions here are suffixed with `future` to avoid name clashes with derived types
 
 
-@define()
+def reawaitable_converter(awaitable: Awaitable[T]) -> ReAwaitable[T]:
+    return ReAwaitable(awaitable)
+
+
+@frozen()
 class Future(Awaitable[T]):
-    reawaitable: ReAwaitable[T] = field(repr=False)
+    """Represents future computations."""
+
+    reawaitable: ReAwaitable[T] = field(repr=False, converter=reawaitable_converter)
 
     @property
     def awaitable(self) -> Awaitable[T]:
         return self.reawaitable.awaitable
 
     def __await__(self) -> Generator[None, None, T]:
         return self.awaitable.__await__()
 
     @classmethod
-    def from_awaitable(cls, awaitable: Awaitable[U]) -> Future[U]:
+    def create(cls, awaitable: Awaitable[U]) -> Future[U]:
         """Creates a [`Future[U]`][wraps.future.Future] from an [`Awaitable[U]`][typing.Awaitable].
 
         Arguments:
             awaitable: The awaitable to wrap.
 
         Returns:
             The future wrapping the given awaitable.
         """
-        return cls(ReAwaitable(awaitable))  # type: ignore
+        return cls(awaitable)  # type: ignore
 
     def map_future(self, function: Unary[T, U]) -> Future[U]:
         """Maps a [`Future[T]`][wraps.future.Future] to a [`Future[U]`][wraps.future.Future]
-        by applying the `function` to the result.
+        by applying the `function` to its result.
 
         Arguments:
             function: The function to apply.
 
         Returns:
             The mapped future.
         """
-        return self.from_awaitable(self.actual_map_future(function))
+        return self.create(self.actual_map_future(function))
 
     def map_future_await(self, function: AsyncUnary[T, U]) -> Future[U]:
         """Maps a [`Future[T]`][wraps.future.Future] to a [`Future[U]`][wraps.future.Future]
-        by applying the asynchronous `function` to the result.
+        by applying the asynchronous `function` to its result.
 
         Arguments:
             function: The asynchronous function to apply.
 
         Returns:
             The mapped future.
         """
-        return self.from_awaitable(self.actual_map_future_await(function))
+        return self.create(self.actual_map_future_await(function))
 
     async def actual_map_future(self, function: Unary[T, U]) -> U:
         return function(await self.awaitable)
 
     async def actual_map_future_await(self, function: AsyncUnary[T, U]) -> U:
         return await function(await self.awaitable)
 
-    def then_future(self, function: Unary[T, Future[U]]) -> Future[U]:
-        """Chains computation by applying the `function` to the result, returning
+    def then(self, function: Unary[T, Future[U]]) -> Future[U]:
+        """Chains computation by applying the `function` to the result, returning the resulting
         [`Future[U]`][wraps.future.Future].
 
         Arguments:
-            function: The function returning future to apply.
+            function: The future-returning function to apply.
 
         Returns:
             The resulting future.
         """
-        return self.from_awaitable(self.actual_then_future(function))
+        return self.create(self.actual_then(function))
 
-    async def actual_then_future(self, function: Unary[T, Future[U]]) -> U:
+    async def actual_then(self, function: Unary[T, Future[U]]) -> U:
         return await function(await self.awaitable).awaitable
 
     def flatten_future(self: Future[Future[T]]) -> Future[T]:
-        return self.then_future(identity)
+        """Flattens a [`Future[Future[T]]`][wraps.future.Future]
+        to a [`Future[T]`][wraps.future.Future].
+
+        This is identical to:
+
+        ```python
+        future.then(identity)
+        ```
+
+        Returns:
+            The flattened future.
+        """
+        return self.then(identity)
 
     def __aiter__(self) -> AsyncIterator[T]:
         return self.async_iter()
 
     async def async_iter(self) -> AsyncIterator[T]:
         """Creates an asynchronous iterator over the result of this
         [`Future[T]`][wraps.future.Future].
@@ -107,15 +128,15 @@
 
         ```python
         async def async_identity(value: T) -> T:
             return value
 
         value = 42
 
-        future = Future.from_awaitable(async_identity(value))
+        future = Future.create(async_identity(value))
         ```
 
         Example:
             ```python
             value = 42
 
             assert await Future.from_value(value) is value
@@ -123,8 +144,8 @@
 
         Arguments:
             value: The value to wrap.
 
         Returns:
             The future wrapping the given value.
         """
-        return cls.from_awaitable(async_identity(value))
+        return cls.create(async_identity(value))
```

### Comparing `wraps-0.4.0/wraps/future_either.py` & `wraps-0.5.0/wraps/future_either.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+"""Future either values."""
+
 from __future__ import annotations
 
 from typing import Awaitable, TypeVar, final
 
-from attrs import frozen
+from attrs import field, frozen
 from typing_extensions import Never
 
 from wraps.either import Either, Left, Right
 from wraps.future import Future
 from wraps.reawaitable import ReAwaitable
 
 __all__ = ("FutureEither",)
@@ -14,24 +16,28 @@
 L = TypeVar("L", covariant=True)
 R = TypeVar("R", covariant=True)
 
 M = TypeVar("M")
 S = TypeVar("S")
 
 
+def reawaitable_converter(awaitable: Awaitable[Either[L, R]]) -> ReAwaitable[Either[L, R]]:
+    return ReAwaitable(awaitable)
+
+
 @final
 @frozen()
 class FutureEither(Future[Either[L, R]]):
     """[`Future[Either[L, R]]`][wraps.future.Future], adapted to leverage future functionality."""
 
+    reawaitable: ReAwaitable[Either[L, R]] = field(repr=False, converter=reawaitable_converter)
+
     @classmethod
-    def from_awaitable(  # type: ignore
-        cls, awaitable: Awaitable[Either[M, S]]
-    ) -> FutureEither[M, S]:
-        return cls(ReAwaitable(awaitable))  # type: ignore
+    def create(cls, awaitable: Awaitable[Either[M, S]]) -> FutureEither[M, S]:  # type: ignore
+        return cls(awaitable)  # type: ignore
 
     @classmethod
     def from_either(cls, either: Either[M, S]) -> FutureEither[M, S]:
         return cls.from_value(either)  # type: ignore
 
     @classmethod
     def from_left(cls, left: M) -> FutureEither[M, Never]:
```

### Comparing `wraps-0.4.0/wraps/future_result.py` & `wraps-0.5.0/wraps/future_result.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,173 +1,233 @@
+"""Future error handling."""
+
 from __future__ import annotations
 
 from typing import Awaitable, TypeVar, final
 
-from attrs import frozen
-from funcs.typing import AsyncInspect, AsyncNullary, AsyncUnary, Inspect, Nullary, Unary
+from attrs import field, frozen
+from funcs.typing import (
+    AnyError,
+    AsyncInspect,
+    AsyncNullary,
+    AsyncPredicate,
+    AsyncUnary,
+    Inspect,
+    Nullary,
+    Predicate,
+    Unary,
+)
 from typing_extensions import Never
 
+from wraps.either import Either
 from wraps.future import Future
 from wraps.option import Option
 from wraps.reawaitable import ReAwaitable
-from wraps.result import Error, Ok, Result, is_error, is_ok
+from wraps.result import Error, Ok, Result
 from wraps.utils import identity
 
 __all__ = ("FutureResult",)
 
 T = TypeVar("T", covariant=True)
 U = TypeVar("U")
 
 E = TypeVar("E", covariant=True)
 F = TypeVar("F")
 
-
 V = TypeVar("V")
 
 
+def reawaitable_converter(awaitable: Awaitable[Result[T, E]]) -> ReAwaitable[Result[T, E]]:
+    return ReAwaitable(awaitable)
+
+
 @final
 @frozen()
 class FutureResult(Future[Result[T, E]]):
     """[`Future[Result[T, E]]`][wraps.future.Future], adapted to leverage future functionality."""
 
+    reawaitable: ReAwaitable[Result[T, E]] = field(repr=False, converter=reawaitable_converter)
+
     @classmethod
-    def from_awaitable(cls, awaitable: Awaitable[Result[U, F]]) -> FutureResult[U, F]:  # type: ignore
-        return cls(ReAwaitable(awaitable))  # type: ignore
+    def create(cls, awaitable: Awaitable[Result[U, F]]) -> FutureResult[U, F]:  # type: ignore
+        return cls(awaitable)  # type: ignore
 
     @classmethod
     def from_result(cls, result: Result[U, F]) -> FutureResult[U, F]:
         return cls.from_value(result)  # type: ignore
 
     @classmethod
     def from_ok(cls, value: U) -> FutureResult[U, Never]:
         return cls.from_result(Ok(value))
 
     @classmethod
     def from_error(cls, value: F) -> FutureResult[Never, F]:
         return cls.from_result(Error(value))
 
+    def is_ok(self) -> Future[bool]:
+        return super().create(self.actual_is_ok())
+
+    def is_ok_and(self, predicate: Predicate[T]) -> Future[bool]:
+        return super().create(self.actual_is_ok_and(predicate))
+
+    def is_ok_and_await(self, predicate: AsyncPredicate[T]) -> Future[bool]:
+        return super().create(self.actual_is_ok_and_await(predicate))
+
+    async def actual_is_ok(self) -> bool:
+        return (await self.awaitable).is_ok()
+
+    async def actual_is_ok_and(self, predicate: Predicate[T]) -> bool:
+        return (await self.awaitable).is_ok_and(predicate)
+
+    async def actual_is_ok_and_await(self, predicate: AsyncPredicate[T]) -> bool:
+        return await (await self.awaitable).is_ok_and_await(predicate)
+
+    def is_error(self) -> Future[bool]:
+        return super().create(self.actual_is_error())
+
+    def is_error_and(self, predicate: Predicate[E]) -> Future[bool]:
+        return super().create(self.actual_is_error_and(predicate))
+
+    def is_error_and_await(self, predicate: AsyncPredicate[E]) -> Future[bool]:
+        return super().create(self.actual_is_error_and_await(predicate))
+
+    async def actual_is_error(self) -> bool:
+        return (await self.awaitable).is_error()
+
+    async def actual_is_error_and(self, predicate: Predicate[E]) -> bool:
+        return (await self.awaitable).is_error_and(predicate)
+
+    async def actual_is_error_and_await(self, predicate: AsyncPredicate[E]) -> bool:
+        return await (await self.awaitable).is_error_and_await(predicate)
+
     def expect(self, message: str) -> Future[T]:
-        return super().from_awaitable(self.actual_expect(message))
+        return super().create(self.actual_expect(message))
 
     def expect_error(self, message: str) -> Future[E]:
-        return super().from_awaitable(self.actual_expect_error(message))
+        return super().create(self.actual_expect_error(message))
 
     async def actual_expect(self, message: str) -> T:
         return (await self.awaitable).expect(message)
 
     async def actual_expect_error(self, message: str) -> E:
         return (await self.awaitable).expect_error(message)
 
     def unwrap(self) -> Future[T]:
-        return super().from_awaitable(self.actual_unwrap())
+        return super().create(self.actual_unwrap())
 
     def unwrap_or(self, default: T) -> Future[T]:  # type: ignore
-        return super().from_awaitable(self.actual_unwrap_or(default))
+        return super().create(self.actual_unwrap_or(default))
 
     def unwrap_or_else(self, default: Nullary[T]) -> Future[T]:
-        return super().from_awaitable(self.actual_unwrap_or_else(default))
+        return super().create(self.actual_unwrap_or_else(default))
 
     def unwrap_or_else_await(self, default: AsyncNullary[T]) -> Future[T]:
-        return super().from_awaitable(self.actual_unwrap_or_else_await(default))
+        return super().create(self.actual_unwrap_or_else_await(default))
 
     async def actual_unwrap(self) -> T:
         return (await self.awaitable).unwrap()
 
     async def actual_unwrap_or(self, default: T) -> T:  # type: ignore
         return (await self.awaitable).unwrap_or(default)
 
     async def actual_unwrap_or_else(self, default: Nullary[T]) -> T:
         return (await self.awaitable).unwrap_or_else(default)
 
     async def actual_unwrap_or_else_await(self, default: AsyncNullary[T]) -> T:
         return await (await self.awaitable).unwrap_or_else_await(default)
 
     def unwrap_error(self) -> Future[E]:
-        return super().from_awaitable(self.actual_unwrap_error())
+        return super().create(self.actual_unwrap_error())
 
     def unwrap_error_or(self, default: E) -> Future[E]:  # type: ignore
-        return super().from_awaitable(self.actual_unwrap_error_or(default))
+        return super().create(self.actual_unwrap_error_or(default))
 
     def unwrap_error_or_else(self, default: Nullary[E]) -> Future[E]:
-        return super().from_awaitable(self.actual_unwrap_error_or_else(default))
+        return super().create(self.actual_unwrap_error_or_else(default))
 
     def unwrap_error_or_else_await(self, default: AsyncNullary[E]) -> Future[E]:
-        return super().from_awaitable(self.actual_unwrap_error_or_else_await(default))
+        return super().create(self.actual_unwrap_error_or_else_await(default))
 
     async def actual_unwrap_error(self) -> E:
         return (await self.awaitable).unwrap_error()
 
     async def actual_unwrap_error_or(self, default: E) -> E:  # type: ignore
         return (await self.awaitable).unwrap_error_or(default)
 
     async def actual_unwrap_error_or_else(self, default: Nullary[E]) -> E:
         return (await self.awaitable).unwrap_error_or_else(default)
 
     async def actual_unwrap_error_or_else_await(self, default: AsyncNullary[E]) -> E:
         return await (await self.awaitable).unwrap_error_or_else_await(default)
 
+    def raising(self: FutureResult[T, AnyError]) -> Future[T]:
+        return super().create(self.actual_raising())
+
+    async def actual_raising(self: FutureResult[T, AnyError]) -> T:
+        return (await self.awaitable).raising()
+
     def ok(self) -> FutureOption[T]:
-        return FutureOption.from_awaitable(self.actual_ok())
+        return FutureOption(self.actual_ok())
 
     def error(self) -> FutureOption[E]:
-        return FutureOption.from_awaitable(self.actual_error())
+        return FutureOption(self.actual_error())
 
     async def actual_ok(self) -> Option[T]:
         return (await self.awaitable).ok()
 
     async def actual_error(self) -> Option[E]:
         return (await self.awaitable).error()
 
     def inspect(self, function: Inspect[T]) -> FutureResult[T, E]:
-        return self.from_awaitable(self.actual_inspect(function))
+        return self.create(self.actual_inspect(function))
 
     def inspect_error(self, function: Inspect[E]) -> FutureResult[T, E]:
-        return self.from_awaitable(self.actual_inspect_error(function))
+        return self.create(self.actual_inspect_error(function))
 
     def inspect_await(self, function: AsyncInspect[T]) -> FutureResult[T, E]:
-        return self.from_awaitable(self.actual_inspect_await(function))
+        return self.create(self.actual_inspect_await(function))
 
     def inspect_error_await(self, function: AsyncInspect[E]) -> FutureResult[T, E]:
-        return self.from_awaitable(self.actual_inspect_error_await(function))
+        return self.create(self.actual_inspect_error_await(function))
 
     async def actual_inspect(self, function: Inspect[T]) -> Result[T, E]:
         return (await self.awaitable).inspect(function)
 
     async def actual_inspect_error(self, function: Inspect[E]) -> Result[T, E]:
         return (await self.awaitable).inspect_error(function)
 
     async def actual_inspect_await(self, function: AsyncInspect[T]) -> Result[T, E]:
         return await (await self.awaitable).inspect_await(function)
 
     async def actual_inspect_error_await(self, function: AsyncInspect[E]) -> Result[T, E]:
         return await (await self.awaitable).inspect_error_await(function)
 
     def map(self, function: Unary[T, U]) -> FutureResult[U, E]:
-        return self.from_awaitable(self.actual_map(function))
+        return self.create(self.actual_map(function))
 
     def map_or(self, default: U, function: Unary[T, U]) -> Future[U]:
-        return super().from_awaitable(self.actual_map_or(default, function))
+        return super().create(self.actual_map_or(default, function))
 
     def map_or_else(self, default: Nullary[U], function: Unary[T, U]) -> Future[U]:
-        return super().from_awaitable(self.actual_map_or_else(default, function))
+        return super().create(self.actual_map_or_else(default, function))
 
     def map_or_else_await(self, default: AsyncNullary[U], function: Unary[T, U]) -> Future[U]:
-        return super().from_awaitable(self.actual_map_or_else_await(default, function))
+        return super().create(self.actual_map_or_else_await(default, function))
 
     def map_error(self, function: Unary[E, F]) -> FutureResult[T, F]:
-        return self.from_awaitable(self.actual_map_error(function))
+        return self.create(self.actual_map_error(function))
 
     def map_error_or(self, default: F, function: Unary[E, F]) -> Future[F]:
-        return super().from_awaitable(self.actual_map_error_or(default, function))
+        return super().create(self.actual_map_error_or(default, function))
 
     def map_error_or_else(self, default: Nullary[F], function: Unary[E, F]) -> Future[F]:
-        return super().from_awaitable(self.actual_map_error_or_else(default, function))
+        return super().create(self.actual_map_error_or_else(default, function))
 
     def map_error_or_else_await(self, default: AsyncNullary[F], function: Unary[E, F]) -> Future[F]:
-        return super().from_awaitable(self.actual_map_error_or_else_await(default, function))
+        return super().create(self.actual_map_error_or_else_await(default, function))
 
     async def actual_map(self, function: Unary[T, U]) -> Result[U, E]:
         return (await self.awaitable).map(function)
 
     async def actual_map_or(self, default: U, function: Unary[T, U]) -> U:
         return (await self.awaitable).map_or(default, function)
 
@@ -188,40 +248,40 @@
 
     async def actual_map_error_or_else_await(
         self, default: AsyncNullary[F], function: Unary[E, F]
     ) -> F:
         return await (await self.awaitable).map_error_or_else_await(default, function)
 
     def map_await(self, function: AsyncUnary[T, U]) -> FutureResult[U, E]:
-        return self.from_awaitable(self.actual_map_await(function))
+        return self.create(self.actual_map_await(function))
 
     def map_await_or(self, default: U, function: AsyncUnary[T, U]) -> Future[U]:
-        return super().from_awaitable(self.actual_map_await_or(default, function))
+        return super().create(self.actual_map_await_or(default, function))
 
     def map_await_or_else(self, default: Nullary[U], function: AsyncUnary[T, U]) -> Future[U]:
-        return super().from_awaitable(self.actual_map_await_or_else(default, function))
+        return super().create(self.actual_map_await_or_else(default, function))
 
     def map_await_or_else_await(
         self, default: AsyncNullary[U], function: AsyncUnary[T, U]
     ) -> Future[U]:
-        return super().from_awaitable(self.actual_map_await_or_else_await(default, function))
+        return super().create(self.actual_map_await_or_else_await(default, function))
 
     def map_error_await(self, function: AsyncUnary[E, F]) -> FutureResult[T, F]:
-        return self.from_awaitable(self.actual_map_error_await(function))
+        return self.create(self.actual_map_error_await(function))
 
     def map_error_await_or(self, default: F, function: AsyncUnary[E, F]) -> Future[F]:
-        return super().from_awaitable(self.actual_map_error_await_or(default, function))
+        return super().create(self.actual_map_error_await_or(default, function))
 
     def map_error_await_or_else(self, default: Nullary[F], function: AsyncUnary[E, F]) -> Future[F]:
-        return super().from_awaitable(self.actual_map_error_await_or_else(default, function))
+        return super().create(self.actual_map_error_await_or_else(default, function))
 
     def map_error_await_or_else_await(
         self, default: AsyncNullary[F], function: AsyncUnary[E, F]
     ) -> Future[F]:
-        return super().from_awaitable(self.actual_map_error_await_or_else_await(default, function))
+        return super().create(self.actual_map_error_await_or_else_await(default, function))
 
     async def actual_map_await(self, function: AsyncUnary[T, U]) -> Result[U, E]:
         return await (await self.awaitable).map_await(function)
 
     async def actual_map_await_or(self, default: U, function: AsyncUnary[T, U]) -> U:
         return await (await self.awaitable).map_await_or(default, function)
 
@@ -246,75 +306,78 @@
 
     async def actual_map_error_await_or_else_await(
         self, default: AsyncNullary[F], function: AsyncUnary[E, F]
     ) -> F:
         return await (await self.awaitable).map_error_await_or_else_await(default, function)
 
     def and_then(self, function: Unary[T, Result[U, E]]) -> FutureResult[U, E]:
-        return self.from_awaitable(self.actual_and_then(function))
+        return self.create(self.actual_and_then(function))
 
     def and_then_await(self, function: AsyncUnary[T, Result[U, E]]) -> FutureResult[U, E]:
-        return self.from_awaitable(self.actual_and_then_await(function))
+        return self.create(self.actual_and_then_await(function))
 
     def or_else(self, function: Unary[E, Result[T, F]]) -> FutureResult[T, F]:
-        return self.from_awaitable(self.actual_or_else(function))
+        return self.create(self.actual_or_else(function))
 
     def or_else_await(self, function: AsyncUnary[E, Result[T, F]]) -> FutureResult[T, F]:
-        return self.from_awaitable(self.actual_or_else_await(function))
+        return self.create(self.actual_or_else_await(function))
 
     async def actual_and_then(self, function: Unary[T, Result[U, E]]) -> Result[U, E]:
         return (await self.awaitable).and_then(function)
 
     async def actual_and_then_await(self, function: AsyncUnary[T, Result[U, E]]) -> Result[U, E]:
         return await (await self.awaitable).and_then_await(function)
 
     async def actual_or_else(self, function: Unary[E, Result[T, F]]) -> Result[T, F]:
         return (await self.awaitable).or_else(function)
 
     async def actual_or_else_await(self, function: AsyncUnary[E, Result[T, F]]) -> Result[T, F]:
         return await (await self.awaitable).or_else_await(function)
 
-    def and_then_future(self, function: Unary[T, FutureResult[U, E]]) -> FutureResult[U, E]:
-        return self.from_awaitable(self.actual_and_then_future(function))
-
-    def or_else_future(self, function: Unary[E, FutureResult[T, F]]) -> FutureResult[T, F]:
-        return self.from_awaitable(self.actual_or_else_future(function))
-
-    async def actual_and_then_future(self, function: Unary[T, FutureResult[U, E]]) -> Result[U, E]:
-        result = await self.awaitable
-
-        if is_ok(result):
-            return await function(result.unwrap())
-
-        return result  # type: ignore  # guaranteed `Error[E]`
+    def try_flatten(self: FutureResult[FutureResult[T, E], E]) -> FutureResult[T, E]:
+        return self.and_then_await(identity)
 
-    async def actual_or_else_future(self, function: Unary[E, FutureResult[T, F]]) -> Result[T, F]:
-        result = await self.awaitable
+    def try_flatten_error(self: FutureResult[T, FutureResult[T, E]]) -> FutureResult[T, E]:
+        return self.or_else_await(identity)
 
-        if is_error(result):
-            return await function(result.unwrap_error())
+    def contains(self, value: U) -> Future[bool]:
+        return super().create(self.actual_contains(value))
 
-        return result  # type: ignore  # guaranteed `Ok[T]`
+    async def actual_contains(self, value: U) -> bool:
+        return (await self.awaitable).contains(value)
 
-    def try_flatten(self: FutureResult[FutureResult[T, E], E]) -> FutureResult[T, E]:
-        return self.and_then_future(identity)
+    def contains_error(self, error: F) -> Future[bool]:
+        return super().create(self.actual_contains_error(error))
 
-    def try_flatten_error(self: FutureResult[T, FutureResult[T, E]]) -> FutureResult[T, E]:
-        return self.or_else_future(identity)
+    async def actual_contains_error(self, error: F) -> bool:
+        return (await self.awaitable).contains_error(error)
 
     def flip(self) -> FutureResult[E, T]:
-        return self.from_awaitable(self.actual_flip())
+        return self.create(self.actual_flip())
 
     async def actual_flip(self) -> Result[E, T]:
         return (await self.awaitable).flip()
 
     def into_ok_or_error(self: FutureResult[T, T]) -> Future[T]:
-        return super().from_awaitable(self.actual_into_ok_or_error())
+        return super().create(self.actual_into_ok_or_error())
 
     async def actual_into_ok_or_error(self: FutureResult[T, T]) -> T:
         return (await self.awaitable).into_ok_or_error()
 
+    def into_either(self) -> FutureEither[T, E]:
+        return FutureEither(self.actual_into_either())
+
+    async def actual_into_either(self) -> Either[T, E]:
+        return (await self.awaitable).into_either()
+
+    def early(self) -> Future[T]:
+        return super().create(self.actual_early())
+
+    async def actual_early(self) -> T:
+        return (await self.awaitable).early()
+
     def into_future(self) -> Future[Result[T, E]]:
-        return super().from_awaitable(self.awaitable)
+        return super().create(self.awaitable)
 
 
+from wraps.future_either import FutureEither
 from wraps.future_option import FutureOption
```

### Comparing `wraps-0.4.0/wraps/option.py` & `wraps-0.5.0/wraps/option.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,24 +40,35 @@
     case Some(result):
         print(result)
 
     case Null():
         print(DIVISION_BY_ZERO)
 ```
 
-Her, we know that [`Null`][wraps.option.Null] represents only one case,
+Here, we know that [`Null`][wraps.option.Null] represents only one case,
 that is, attempts to divide by zero. However, when we need to represent multiple errors
 from one function, we might want to use [`Result[T, E]`][wraps.result.Result] instead,
 as described in the [`result`][wraps.result] section.
 """
 
 from __future__ import annotations
 
 from abc import abstractmethod as required
-from typing import AsyncIterator, Iterator, Optional, Tuple, TypeVar, Union, final, overload
+from typing import (
+    AsyncIterable,
+    AsyncIterator,
+    Iterable,
+    Iterator,
+    Optional,
+    Tuple,
+    TypeVar,
+    Union,
+    final,
+    overload,
+)
 
 from attrs import frozen
 from funcs.typing import (
     AsyncBinary,
     AsyncInspect,
     AsyncNullary,
     AsyncPredicate,
@@ -78,15 +89,15 @@
 T = TypeVar("T", covariant=True)
 U = TypeVar("U")
 V = TypeVar("V")
 
 E = TypeVar("E")
 
 
-class OptionProtocol(Protocol[T]):  # type: ignore[misc]
+class OptionProtocol(AsyncIterable[T], Iterable[T], Protocol[T]):  # type: ignore[misc]
     def __iter__(self) -> Iterator[T]:
         return self.iter()
 
     def __aiter__(self) -> AsyncIterator[T]:
         return self.async_iter()
 
     @required
@@ -1049,15 +1060,14 @@
             assert null.unzip() == (Null(), Null())
 
         Returns:
             The resulting tuple of two options.
         """
         ...
 
-    # @required
     # def transpose(self: OptionProtocol[ResultProtocol[T, E]]) -> Result[Option[T], E]:
     #     """Transposes an option of a result into result of an option.
     #     This function maps [`Option[Result[T, E]]`][wraps.option.Option] into
     #     [`Result[Option[T], E]]`][wraps.result.Result] in the following way:
 
     #     - [`Null()`][wraps.option.Null] is mapped to [`Ok(Null())`][wraps.result.Ok];
     #     - [`Some(Ok(value))`][wraps.option.Some] is mapped to
@@ -1072,15 +1082,15 @@
 
     #         assert option.transpose() == result
     #         ```
 
     #     Returns:
     #         The transposed result.
     #     """
-    #     ...
+    #     return transpose_option(self)  # type: ignore
 
     def flatten(self: OptionProtocol[OptionProtocol[U]]) -> Option[U]:
         """Flattens an [`Option[Option[T]]`][wraps.option.Option]
         to [`Option[T]`][wraps.option.Option].
 
         Example:
             ```python
@@ -1123,15 +1133,15 @@
         Returns:
             Whether the contained value is equal to `value`.
         """
         ...
 
     @required
     def early(self) -> T:
-        """Functionally similar to `?` operator in Rust.
+        """Functionally similar to the *question-mark* (`?`) operator in Rust.
 
         See [`early`][wraps.early] for more information.
         """
         ...
 
 
 UNWRAP_ON_NULL = "called `unwrap` on null"
```

### Comparing `wraps-0.4.0/wraps/reawaitable.py` & `wraps-0.5.0/wraps/reawaitable.py`

 * *Files identical despite different names*

### Comparing `wraps-0.4.0/wraps/result.py` & `wraps-0.5.0/wraps/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         print(error)
 ```
 """
 
 from __future__ import annotations
 
 from abc import abstractmethod as required
-from typing import AsyncIterator, Iterator, TypeVar, Union, final
+from typing import AsyncIterable, AsyncIterator, Iterable, Iterator, TypeVar, Union, final
 
 from attrs import frozen
 from funcs.typing import (
     AnyError,
     AsyncInspect,
     AsyncNullary,
     AsyncPredicate,
@@ -59,30 +59,30 @@
     Predicate,
     Unary,
 )
 from typing_extensions import Literal, Never, ParamSpec, Protocol, TypeGuard
 
 from wraps.errors import EarlyResult, panic
 from wraps.option import Null, Option, Some
-from wraps.utils import async_empty, async_once, empty, once
+from wraps.utils import async_empty, async_once, empty, identity, once
 
 __all__ = ("Result", "Ok", "Error", "is_ok", "is_error")
 
 P = ParamSpec("P")
 
 T = TypeVar("T", covariant=True)
 U = TypeVar("U")
 
 E = TypeVar("E", covariant=True)
 F = TypeVar("F")
 
 V = TypeVar("V")
 
 
-class ResultProtocol(Protocol[T, E]):  # type: ignore[misc]
+class ResultProtocol(AsyncIterable[T], Iterable[T], Protocol[T, E]):  # type: ignore[misc]
     def __iter__(self) -> Iterator[T]:
         return self.iter()
 
     def __aiter__(self) -> AsyncIterator[T]:
         return self.async_iter()
 
     @required
@@ -134,15 +134,15 @@
     @required
     async def is_ok_and_await(self, predicate: AsyncPredicate[T]) -> bool:
         """Checks if the result is [`Ok[T]`][wraps.result.Ok] and the value
         inside of it matches the asynchronous `predicate`.
 
         Example:
             ```python
-            def is_positive(value: int) -> bool:
+            async def is_positive(value: int) -> bool:
                 return value > 0
 
             ok = Ok(13)
             assert await ok.is_ok_and_await(is_positive)
 
             zero = Ok(0)
             assert not await zero.is_ok_and_await(is_positive)
@@ -400,14 +400,15 @@
         or [`unwrap_error_or_else`][wraps.result.ResultProtocol.unwrap_error_or_else].
 
         Example:
             ```python
             >>> error = Error(13)
             >>> error.unwrap_error()
             13
+
             >>> ok = Ok(42)
             >>> ok.unwrap_error()
             Traceback (most recent call last):
               ...
             wraps.errors.Panic: called `unwrap_error` on ok
             ```
 
@@ -472,15 +473,15 @@
             async def default() -> int:
                 return 0
 
             error = Error(13)
             assert await error.unwrap_error_or_else_await(default)
 
             ok = Ok(5)
-            assert not ok.unwrap_error_or_else_await(default)
+            assert not await ok.unwrap_error_or_else_await(default)
             ```
 
         Arguments:
             default: The asynchronous default-computing function to use.
 
         Returns:
             The contained error value or the `await default()` one.
@@ -493,14 +494,15 @@
         contained [`Error[AnyError]`][wraps.result.Error] value.
 
         Example:
             ```python
             >>> ok = Ok(13)
             >>> ok.raising()
             13
+
             >>> error = Error(ValueError("error..."))
             >>> error.raising()
             Traceback (most recent call last):
               ...
             ValueError: error...
             ```
 
@@ -511,15 +513,15 @@
             The contained value.
         """
         ...
 
     @required
     def ok(self) -> Option[T]:
         """Converts a [`Result[T, E]`][wraps.result.Result]
-        to an [`Option[T]`][wraps.option.Option].
+        into an [`Option[T]`][wraps.option.Option].
 
         Converts `self` into an [`Option[T]`][wraps.option.Option], discarding errors, if any.
 
         Example:
             ```python
             ok = Ok(42)
 
@@ -534,15 +536,15 @@
             The converted option.
         """
         ...
 
     @required
     def error(self) -> Option[E]:
         """Converts a [`Result[T, E]`][wraps.result.Result]
-        to an [`Option[E]`][wraps.option.Option].
+        into an [`Option[E]`][wraps.option.Option].
 
         Converts `self` into an [`Option[E]`][wraps.option.Option],
         discarding success values, if any.
 
         Example:
             ```python
             error = Error(13)
@@ -1281,15 +1283,15 @@
         Returns:
             The bound result.
         """
         ...
 
     def try_flatten(self: ResultProtocol[ResultProtocol[T, E], E]) -> Result[T, E]:
         """Flattens a [`Result[Result[T, E], E]`][wraps.result.Result]
-        to a [`Result[T, E]`][wraps.result.Result].
+        into a [`Result[T, E]`][wraps.result.Result].
 
         This is equivalent to [`result.and_then(identity)`][wraps.result.ResultProtocol.and_then].
 
         Example:
             ```python
             ok = Ok(42)
             ok_nested = Ok(ok)
@@ -1305,15 +1307,15 @@
         Returns:
             The flattened result.
         """
         return self.and_then(identity)  # type: ignore
 
     def try_flatten_error(self: ResultProtocol[T, ResultProtocol[T, E]]) -> Result[T, E]:
         """Flattens a [`Result[T, Result[T, E]]`][wraps.result.Result]
-        to a [`Result[T, E]`][wraps.result.Result].
+        into a [`Result[T, E]`][wraps.result.Result].
 
         This is equivalent to [`result.or_else(identity)`][wraps.result.ResultProtocol.or_else].
 
         Example:
             ```python
             ok = Ok(42)
             ok_nested = Error(ok)
@@ -1327,38 +1329,36 @@
             ```
 
         Returns:
             The flattened result.
         """
         return self.or_else(identity)  # type: ignore
 
-    # @required
     # def transpose(self: ResultProtocol[OptionProtocol[T], E]) -> Option[Result[T, E]]:
-    #     """Transposes a result of an option into option of a result.
+    #     """Transposes a result of an option into an option of a result.
     #     This function maps [`Result[Option[T], E]`][wraps.result.Result] into
     #     [`Option[Result[T, E]]`][wraps.option.Option] in the following way:
 
     #     - [`Ok(Null())`][wraps.result.Ok] is mapped to [`Null()`][wraps.option.Null];
     #     - [`Ok(Some(value))`][wraps.result.Ok] is mapped to
     #       [`Some(Ok(value))`][wraps.option.Some];
     #     - [`Error(error)`][wraps.result.Error] is mapped to
     #       [`Some(Error(error))`][wraps.option.Some].
 
     #     Example:
     #         ```python
     #         result = Ok(Some(64))
-    #         option = Some(Ok(64))
-
+    #         option = Some(Ok(64)
     #         assert result.transpose() == option
     #         ```
 
     #     Returns:
     #         The transposed option.
     #     """
-    #     ...
+    #     return transpose_result(self)  # type: ignore
 
     @required
     def contains(self, value: U) -> bool:
         """Checks if the contained value is equal to the `value`.
 
         Example:
             ```python
@@ -1405,15 +1405,15 @@
             Whether the contained error value is equal to the `error`.
         """
         ...
 
     @required
     def flip(self) -> Result[E, T]:
         """Converts a [`Result[T, E]`][wraps.result.Result]
-        to a [`Result[E, T]`][wraps.result.Result].
+        into a [`Result[E, T]`][wraps.result.Result].
 
         [`Ok(value)`][wraps.result.Ok] and [`Error(error)`][wraps.result.Error] get swapped to
         [`Error(value)`][wraps.result.Error] and [`Ok(error)`][wraps.result.Ok] respectively.
 
         Example:
             ```python
             value = 42
@@ -1427,36 +1427,38 @@
         Returns:
             The flipped result.
         """
         ...
 
     @required
     def into_ok_or_error(self: ResultProtocol[V, V]) -> V:
-        """Returns the [`Ok[V]`][wraps.result.Ok] value if `self` is [`Ok[V]`][wraps.result.Ok], and
-        the [`Error[V]`][wraps.result.Error] value if `self` is an [`Error[V]`][wraps.result.Error].
-
-        In other words, this function returns the value of a [`Result[V, V]`][wraps.result.Result],
-        regardless of whether or not that result is
-        [`Ok[V]`][wraps.result.Ok] or [`Error[V]`][wraps.result.Error].
+        """Returns the value contained within [`Result[V, V]`][wraps.result.Result], regardless
+        of whether or not that result is [`Ok[V]`][wraps.result.Ok]
+        or [`Error[V]`][wraps.result.Error].
 
         Example:
             ```python
             result: Result[int, int] = Ok(69)
 
-            print(result.into_ok_or_error())  # 69
+            print(result.into_ok_or_error())  # 69; inferred `int`
+
+            result = Error(42)
+
+            print(result.into_ok_or_error())  # 42; inferred `int`
             ```
 
         Returns:
             The contained value, regardless of whether or not it is an error one.
         """
         ...
 
     @required
     def into_either(self) -> Either[T, E]:
-        """Maps a [`Result[T, E]`][wraps.result.Result] to an [`Either[T, E]`][wraps.either.Either].
+        """Converts a [`Result[T, E]`][wraps.result.Result]
+        into an [`Either[T, E]`][wraps.either.Either].
 
         [`Ok(value)`][wraps.result.Ok] is mapped to [`Left(value)`][wraps.either.Left]
         and [`Error(error)`][wraps.result.Error] is mapped to [`Right(error)`][wraps.either.Right].
 
         Example:
             ```python
             value = 42
@@ -1475,15 +1477,15 @@
         Returns:
             The mapped either.
         """
         ...
 
     @required
     def early(self) -> T:
-        """Functionally similar to `?` operator in Rust.
+        """Functionally similar to the *question-mark* (`?`) operator in Rust.
 
         See [`early`][wraps.early] for more information.
         """
         ...
 
 
 UNWRAP_ON_ERROR = "called `unwrap` on error"
```

### Comparing `wraps-0.4.0/wraps/utils.py` & `wraps-0.5.0/wraps/utils.py`

 * *Files identical despite different names*

### Comparing `wraps-0.4.0/wraps/wraps.py` & `wraps-0.5.0/wraps/wraps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Highly composable wrapping decorators."""
+
 from __future__ import annotations
 
 from typing import Callable, Generic, Optional, Type, TypeVar, final
 
 from attrs import frozen
 from funcs.decorators import wraps
 from funcs.typing import AnyError, AsyncCallable, NormalError
@@ -270,15 +272,15 @@
 
     Returns:
         The wrapping function.
     """
 
     @wraps(function)
     def wrap(*args: P.args, **kwargs: P.kwargs) -> Future[T]:
-        return Future.from_awaitable(function(*args, **kwargs))
+        return Future(function(*args, **kwargs))
 
     return wrap
 
 
 def wrap_future_option(function: AsyncCallable[P, Option[T]]) -> Callable[P, FutureOption[T]]:
     """Wraps an asynchronous `function` returning [`Option[T]`][wraps.option.Option] into a function
     returning [`FutureOption[T]`][wraps.future_option.FutureOption].
@@ -288,15 +290,15 @@
 
     Returns:
         The wrapping function.
     """
 
     @wraps(function)
     def wrap(*args: P.args, **kwargs: P.kwargs) -> FutureOption[T]:
-        return FutureOption.from_awaitable(function(*args, **kwargs))
+        return FutureOption(function(*args, **kwargs))
 
     return wrap
 
 
 def wrap_future_result(function: AsyncCallable[P, Result[T, E]]) -> Callable[P, FutureResult[T, E]]:
     """Wraps an asynchronous `function` returning [`Result[T, E]`][wraps.result.Result]
     into a function returning [`FutureResult[T, E]`][wraps.future_result.FutureResult].
@@ -306,15 +308,15 @@
 
     Returns:
         The wrapping function.
     """
 
     @wraps(function)
     def wrap(*args: P.args, **kwargs: P.kwargs) -> FutureResult[T, E]:
-        return FutureResult.from_awaitable(function(*args, **kwargs))
+        return FutureResult(function(*args, **kwargs))
 
     return wrap
 
 
 def wrap_future_either(function: AsyncCallable[P, Either[L, R]]) -> Callable[P, FutureEither[L, R]]:
     """Wraps an asynchronous `function` returning [`Either[L, R]`][wraps.either.Either]
     into a function returning [`FutureEither[L, R]`][wraps.future_either.FutureEither].
@@ -324,10 +326,10 @@
 
     Returns:
         The wrapping function.
     """
 
     @wraps(function)
     def wrap(*args: P.args, **kwargs: P.kwargs) -> FutureEither[L, R]:
-        return FutureEither.from_awaitable(function(*args, **kwargs))
+        return FutureEither(function(*args, **kwargs))
 
     return wrap
```

### Comparing `wraps-0.4.0/PKG-INFO` & `wraps-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wraps
-Version: 0.4.0
+Version: 0.5.0
 Summary: Meaningful and safe wrapping types.
 Home-page: https://github.com/nekitdev/wraps
 License: MIT
 Keywords: python,future,either,option,result
 Author: nekitdev
 Requires-Python: >=3.7
 Classifier: Development Status :: 4 - Beta
@@ -15,17 +15,17 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Dist: async-extensions (>=1.2.2)
+Requires-Dist: async-extensions (>=1.2.3)
 Requires-Dist: attrs (>=23.1.0)
-Requires-Dist: funcs (>=0.5.0)
+Requires-Dist: funcs (>=0.5.1)
 Requires-Dist: typing-extensions (>=4.5.0)
 Project-URL: Documentation, https://nekitdev.github.io/wraps
 Project-URL: Discord, https://nekit.dev/discord
 Project-URL: Funding, https://patreon.com/nekitdev
 Project-URL: Issues, https://github.com/nekitdev/wraps/issues
 Project-URL: Repository, https://github.com/nekitdev/wraps
 Description-Content-Type: text/markdown
@@ -72,15 +72,15 @@
 $ poetry add wraps
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-wraps = "^0.4.0"
+wraps = "^0.5.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.wraps]
 git = "https://github.com/nekitdev/wraps.git"
@@ -132,15 +132,15 @@
 
 def divide(numerator: float, denominator: float) -> Result[float, DivideError]:
     return Ok(numerator / denominator) if denominator else Error(DivideError.DIVISION_BY_ZERO)
 ```
 
 ### Early Return
 
-Early return functionality (`?` operator in Rust) is implemented via `early` methods
+Early return functionality (like the *question-mark* (`?`) operator in Rust) is implemented via `early` methods
 (for both [`Option`][wraps.option.Option] and [`Result`][wraps.result.Result] types)
 combined with the [`@early_option`][wraps.early.early_option] and
 [`@early_result`][wraps.early.early_result] decorators respectively.
 
 ```python
 from wraps import Option, early_option, wrap_option
```

