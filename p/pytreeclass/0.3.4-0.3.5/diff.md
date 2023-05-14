# Comparing `tmp/pytreeclass-0.3.4.tar.gz` & `tmp/pytreeclass-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytreeclass-0.3.4.tar", last modified: Fri May 12 18:36:35 2023, max compression
+gzip compressed data, was "pytreeclass-0.3.5.tar", last modified: Sun May 14 01:10:49 2023, max compression
```

## Comparing `pytreeclass-0.3.4.tar` & `pytreeclass-0.3.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:36:35.767387 pytreeclass-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25126 2023-05-12 18:36:35.767387 pytreeclass-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24250 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:36:35.767387 pytreeclass-0.3.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:36:35.767387 pytreeclass-0.3.4/pytreeclass/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/pytreeclass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:36:35.767387 pytreeclass-0.3.4/pytreeclass/_src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/pytreeclass/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9909 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/pytreeclass/_src/code_build.py
--rw-r--r--   0 runner    (1001) docker     (123)    19067 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/pytreeclass/_src/tree_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    28159 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/pytreeclass/_src/tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    28279 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/pytreeclass/_src/tree_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:36:35.767387 pytreeclass-0.3.4/pytreeclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25126 2023-05-12 18:36:35.000000 pytreeclass-0.3.4/pytreeclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-12 18:36:35.000000 pytreeclass-0.3.4/pytreeclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 18:36:35.000000 pytreeclass-0.3.4/pytreeclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 18:36:35.000000 pytreeclass-0.3.4/pytreeclass.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-12 18:36:35.000000 pytreeclass-0.3.4/pytreeclass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-12 18:36:35.000000 pytreeclass-0.3.4/pytreeclass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 18:36:35.767387 pytreeclass-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:36:35.767387 pytreeclass-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17696 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/tests/test_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/tests/test_tree_freeze.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/tests/test_tree_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17411 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/tests/test_tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/tests/test_tree_viz_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/tests/test_treeclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/tests/test_under_jit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:10:49.023305 pytreeclass-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-14 01:10:32.000000 pytreeclass-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25320 2023-05-14 01:10:49.023305 pytreeclass-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24444 2023-05-14 01:10:32.000000 pytreeclass-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:10:49.019305 pytreeclass-0.3.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-14 01:10:32.000000 pytreeclass-0.3.5/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:10:49.019305 pytreeclass-0.3.5/pytreeclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-14 01:10:32.000000 pytreeclass-0.3.5/pytreeclass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:10:49.019305 pytreeclass-0.3.5/pytreeclass/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-14 01:10:32.000000 pytreeclass-0.3.5/pytreeclass/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-05-14 01:10:32.000000 pytreeclass-0.3.5/pytreeclass/_src/code_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19652 2023-05-14 01:10:32.000000 pytreeclass-0.3.5/pytreeclass/_src/tree_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28744 2023-05-14 01:10:32.000000 pytreeclass-0.3.5/pytreeclass/_src/tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28864 2023-05-14 01:10:32.000000 pytreeclass-0.3.5/pytreeclass/_src/tree_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:10:49.019305 pytreeclass-0.3.5/pytreeclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25320 2023-05-14 01:10:48.000000 pytreeclass-0.3.5/pytreeclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-14 01:10:48.000000 pytreeclass-0.3.5/pytreeclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 01:10:48.000000 pytreeclass-0.3.5/pytreeclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 01:10:48.000000 pytreeclass-0.3.5/pytreeclass.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-14 01:10:48.000000 pytreeclass-0.3.5/pytreeclass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-14 01:10:48.000000 pytreeclass-0.3.5/pytreeclass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 01:10:49.023305 pytreeclass-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-14 01:10:32.000000 pytreeclass-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:10:49.019305 pytreeclass-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 01:10:32.000000 pytreeclass-0.3.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17696 2023-05-14 01:10:32.000000 pytreeclass-0.3.5/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-05-14 01:10:32.000000 pytreeclass-0.3.5/tests/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-05-14 01:10:32.000000 pytreeclass-0.3.5/tests/test_tree_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-14 01:10:32.000000 pytreeclass-0.3.5/tests/test_tree_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17411 2023-05-14 01:10:32.000000 pytreeclass-0.3.5/tests/test_tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-14 01:10:32.000000 pytreeclass-0.3.5/tests/test_tree_viz_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-05-14 01:10:32.000000 pytreeclass-0.3.5/tests/test_treeclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-14 01:10:32.000000 pytreeclass-0.3.5/tests/test_under_jit.py
```

### Comparing `pytreeclass-0.3.4/LICENSE` & `pytreeclass-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.4/PKG-INFO` & `pytreeclass-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytreeclass
-Version: 0.3.4
+Version: 0.3.5
 Summary: JAX compatible dataclass.
 Home-page: https://github.com/ASEM000/pytreeclass
 Author: Mahmoud Asem
 Author-email: asem00@kaist.ac.kr
 License: Apache-2.0
 Keywords: python machine-learning pytorch jax
 Classifier: Development Status :: 5 - Production/Stable
@@ -535,43 +535,54 @@
 print(counter.calls) # 10
 ```
 
 </details>
 
 ## ➕ More<a id="more"></a>
 
-<details> <summary>Validate or convert inputs using callbacks</summary>
+<details> <summary>Validate or convert inputs using type hints</summary>
 
-`PyTreeClass` includes `callbacks` in the `field` to apply a sequence of functions on input at setting the attribute stage. The callback is quite useful in several cases, for instance, to ensure a certain input type within a valid range. See example:
+`PyTreeClass` executes functions defined inside `typing.Annotated` on field values before assigning it to the instance.
+The functionality can be quite useful in several cases, for instance, to ensure a certain input type within a valid range. See example:
 
 ```python
 import jax
 import pytreeclass as pytc
-
-def positive_int_callback(value):
-    if not isinstance(value, int):
-        raise TypeError("Value must be an integer")
-    if value <= 0:
-        raise ValueError("Value must be positive")
-    return value
+# python 3.9 and above
+from typing import Annotated
+# python 3.8
+# from typing_extensions import Annotated
+
+class PositiveInt:
+    def __call__(self,value):
+        if not isinstance(value, int):
+            raise TypeError("Value must be an integer")
+        if value <= 0:
+            raise ValueError("Value must be positive")
+        return value
 
 
 class Tree(pytc.TreeClass):
-    in_features:int = pytc.field(callbacks=[positive_int_callback])
-
+    in_features: Annotated[int, PositiveInt()]
 
 tree = Tree(1)
 # no error
 
-tree = Tree(0)
-# ValueError: Error for field=`in_features`:
+try:
+    tree = Tree(0)
+except ValueError as e:
+    print(e)
+# Error for field=`in_features`:
 # Value must be positive
 
-tree = Tree(1.0)
-# TypeError: Error for field=`in_features`:
+try:
+    tree = Tree(1.0)
+except TypeError as e:
+    print(e)
+# Error for field=`in_features`:
 # Value must be an integer
 ```
 
 </details>
 
 <details>  <summary> Add leafwise math operations to PyTreeClass wrapped class</summary>
```

### Comparing `pytreeclass-0.3.4/README.md` & `pytreeclass-0.3.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -512,43 +512,54 @@
 print(counter.calls) # 10
 ```
 
 </details>
 
 ## ➕ More<a id="more"></a>
 
-<details> <summary>Validate or convert inputs using callbacks</summary>
+<details> <summary>Validate or convert inputs using type hints</summary>
 
-`PyTreeClass` includes `callbacks` in the `field` to apply a sequence of functions on input at setting the attribute stage. The callback is quite useful in several cases, for instance, to ensure a certain input type within a valid range. See example:
+`PyTreeClass` executes functions defined inside `typing.Annotated` on field values before assigning it to the instance.
+The functionality can be quite useful in several cases, for instance, to ensure a certain input type within a valid range. See example:
 
 ```python
 import jax
 import pytreeclass as pytc
-
-def positive_int_callback(value):
-    if not isinstance(value, int):
-        raise TypeError("Value must be an integer")
-    if value <= 0:
-        raise ValueError("Value must be positive")
-    return value
+# python 3.9 and above
+from typing import Annotated
+# python 3.8
+# from typing_extensions import Annotated
+
+class PositiveInt:
+    def __call__(self,value):
+        if not isinstance(value, int):
+            raise TypeError("Value must be an integer")
+        if value <= 0:
+            raise ValueError("Value must be positive")
+        return value
 
 
 class Tree(pytc.TreeClass):
-    in_features:int = pytc.field(callbacks=[positive_int_callback])
-
+    in_features: Annotated[int, PositiveInt()]
 
 tree = Tree(1)
 # no error
 
-tree = Tree(0)
-# ValueError: Error for field=`in_features`:
+try:
+    tree = Tree(0)
+except ValueError as e:
+    print(e)
+# Error for field=`in_features`:
 # Value must be positive
 
-tree = Tree(1.0)
-# TypeError: Error for field=`in_features`:
+try:
+    tree = Tree(1.0)
+except TypeError as e:
+    print(e)
+# Error for field=`in_features`:
 # Value must be an integer
 ```
 
 </details>
 
 <details>  <summary> Add leafwise math operations to PyTreeClass wrapped class</summary>
```

### Comparing `pytreeclass-0.3.4/docs/conf.py` & `pytreeclass-0.3.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.4/pytreeclass/__init__.py` & `pytreeclass-0.3.5/pytreeclass/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,8 +46,8 @@
     "tree_map_with_trace",
     "tree_leaves_with_trace",
     "tree_flatten_with_trace",
     "tree_repr_with_trace",
     "Partial",
 )
 
-__version__ = "0.3.4"
+__version__ = "0.3.5"
```

### Comparing `pytreeclass-0.3.4/pytreeclass/_src/code_build.py` & `pytreeclass-0.3.5/pytreeclass/_src/code_build.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,36 @@
+# Copyright 2023 PyTreeClass authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 from __future__ import annotations
 
 import functools as ft
 import sys
 from collections.abc import Callable, MutableMapping, MutableSequence
 from types import FunctionType, MappingProxyType
 from typing import Any, NamedTuple, Sequence
 
+from typing_extensions import Annotated
+
 """Constructor code generation from type annotations."""
 
 PyTree = Any
 EllipsisType = type(Ellipsis)
+AnnotatedType = type(Annotated[int, 1])
 _NOT_SET = type("NOT_SET", (), {"__repr__": lambda _: "NOT_SET"})()
 _MUTABLE_TYPES = (MutableSequence, MutableMapping, set)
 # https://github.com/google/jax/issues/14295
 
 
 class Field(NamedTuple):
     name: str | None = None
@@ -34,50 +51,58 @@
     default: Any = _NOT_SET,
     factory: Callable | None = None,
     init: bool = True,
     repr: bool = True,
     kw_only: bool = False,
     pos_only: bool = False,
     metadata: dict[str, Any] | None = None,  # type: ignore
-    callbacks: Sequence[Any] = (),
     alias: str | None = None,
 ) -> Field:
     """
     Args:
         default: The default value of the field. Mutually exclusive with `factory`.
         factory: A 0-argument function called to initialize field value.
             Mutually exclusive with `default`.
         init: Whether the field is included in the object's __init__ function.
         repr: Whether the field is included in the object's __repr__ function.
         kw_only: Whether the field is keyword-only. Mutually exclusive
             with `pos_only`, effectively placing `/` in the constructor.
         pos_only: Whether the field is positional-only. Mutually exclusive
             with `kw_only`, effectively placing `*` in the constructor.
         metadata: A mapping of user-defined data for the field.
-        callbacks: A sequence of functions to called on `setattr` during
-            initialization to modify the field value.
         alias: An a alias for the field name in the constructor.
 
+    Note:
+        Use functions in `typing.Annotated` metadata to allow for functions
+        to be called on the field value before it is assigned. check the
+        PEP 593, and the example below for more details.
+
     Example:
         >>> import pytreeclass as pytc
-        >>> def instance_cb_factory(klass):
-        ...    def wrapper(x):
-        ...        assert isinstance(x, klass)
+        >>> from typing_extensions import Annotated # if python < 3.9
+
+        >>> class IsInstance:
+        ...    def __init__(self, type_):
+        ...        self.type_ = type_
+        ...    def __call__(self, x):
+        ...        assert isinstance(x, self.type_)
         ...        return x
-        ...    return wrapper
 
-        >>> def positive_check_callback(x):
-        ...    assert x > 0
-        ...    return x
+        >>> class GreaterThan:
+        ...    def __init__(self, value):
+        ...        self.value = value
+        ...    def __call__(self, x):
+        ...        assert x > self.value
+        ...        return x
 
         >>> class Employee(pytc.TreeClass):
         ...    # assert employee `name` is str
-        ...    name: str = pytc.field(callbacks=[instance_cb_factory(str)])
+        ...    name: Annotated[str, IsInstance(str)]
         ...    # use callback compostion to assert employee `age` is int and positive
-        ...    age: int = pytc.field(callbacks=[instance_cb_factory(int), positive_check_callback])
+        ...    age: Annotated[int, IsInstance(int), GreaterThan(0)]
         ...    # use `id` in the constructor for `_id` attribute
         ...    # this is useful for private attributes that are not supposed
         ...    # to be accessed directly and hide it from the repr
         ...    _id: int = pytc.field(alias="id", repr=False)
 
         >>> tree = Employee(name="Asem", age=10, id=1)
         >>> print(tree)  # _id is not shown
@@ -112,40 +137,24 @@
     elif metadata is not None:
         raise TypeError(
             "`metadata` must be a dictionary describing the metadata of "
             "the field or `None` if no metadata is provided, "
             f"got type=`{type(metadata).__name__}` instead."
         )
 
-    if not isinstance(callbacks, Sequence):
-        raise TypeError(
-            f"`callbacks` must be a Sequence of one-argument function(s) "
-            "operating on the field value, and returning a modified value, "
-            f"got type `{type(callbacks).__name__}` instead."
-        )
-
-    for index, callback in enumerate(callbacks):
-        if not isinstance(callback, Callable):  # type: ignore
-            raise TypeError(
-                f"`callback` must be a one-argument function "
-                "operating on the field value, and returning a modified value, "
-                f"got type `{type(callback).__name__}` at {index=} instead."
-            )
-
     return Field(
         name=None,
         type=None,
         default=default,
         factory=factory,
         init=init,
         repr=repr,
         kw_only=kw_only,
         pos_only=pos_only,
         metadata=metadata,  # type: ignore
-        callbacks=callbacks,
         alias=alias,
     )
 
 
 @ft.lru_cache(maxsize=128)
 def _build_field_map(klass: type) -> MappingProxyType[str, Field]:
     field_map = dict()  # type: dict[str, Field]
@@ -158,15 +167,15 @@
 
     # TODO: use inspect to get annotations, once min python version >3.9
     if "__annotations__" not in vars(klass):
         return MappingProxyType(field_map)
 
     for name in (annotation_map := vars(klass)["__annotations__"]):
         value = vars(klass).get(name, _NOT_SET)
-        type = annotation_map[name]
+        hint = annotation_map[name]
 
         if name == "self":
             # while `dataclasses` allows `self` as a field name, its confusing
             # and not recommended. so raise an error
             raise ValueError("Field name cannot be `self`.")
 
         if isinstance(value, Field):
@@ -174,26 +183,33 @@
                 # example case: `x: Any = field(default=[1, 2, 3])`
                 raise TypeError(
                     f"Mutable default value= {value.default} is not allowed"
                     f" for field `{name}` in class `{klass.__name__}`.\n"
                     f" use `field(... ,factory=lambda:{value.default})` instead"
                 )
             # case: `x: Any = field(default=1)`
-            field_map[name] = value._replace(name=name, type=type)
+            field_map[name] = value._replace(name=name, type=hint)
         else:
             if isinstance(value, _MUTABLE_TYPES):
                 # https://github.com/ericvsmith/dataclasses/issues/3
                 # example case: `x: Any = [1, 2, 3]`
                 raise TypeError(
                     f"Mutable value= {(value)} is not allowed"
                     f" for field `{name}` in class `{klass.__name__}`.\n"
                     f" use `field(... ,factory=lambda:{value})` instead"
                 )
             # case: `x: int = 1` or `x: Any`
-            field_map[name] = Field(name=name, type=type, default=value)
+            field_map[name] = Field(name=name, type=hint, default=value)
+
+        if isinstance(hint, AnnotatedType):
+            # case: 'x: Annotated[int, Range(0, 10)]'
+            # follows PEP 593 https://peps.python.org/pep-0593/
+            if callbacks := tuple(x for x in hint.__metadata__ if callable(x)):
+                field_map[name] = field_map[name]._replace(callbacks=callbacks)
+
     return MappingProxyType(field_map)
 
 
 def fields(x: Any) -> Sequence[Field]:
     """Returns a tuple of `Field` objects for the given instance or class.
 
     `Field` objects are generated from the class type hints and contains
```

### Comparing `pytreeclass-0.3.4/pytreeclass/_src/tree_base.py` & `pytreeclass-0.3.5/pytreeclass/_src/tree_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright 2023 PyTreeClass authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 from __future__ import annotations
 
 import abc
 from collections.abc import Callable
 from contextlib import contextmanager
 from typing import Any, NamedTuple, TypeVar
```

### Comparing `pytreeclass-0.3.4/pytreeclass/_src/tree_pprint.py` & `pytreeclass-0.3.5/pytreeclass/_src/tree_pprint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright 2023 PyTreeClass authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 from __future__ import annotations
 
 import dataclasses as dc
 import functools as ft
 import inspect
 import math
 from itertools import chain
```

### Comparing `pytreeclass-0.3.4/pytreeclass/_src/tree_util.py` & `pytreeclass-0.3.5/pytreeclass/_src/tree_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright 2023 PyTreeClass authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 from __future__ import annotations
 
 import dataclasses as dc
 import functools as ft
 import hashlib
 import operator as op
 from math import ceil, floor, trunc
```

### Comparing `pytreeclass-0.3.4/pytreeclass.egg-info/PKG-INFO` & `pytreeclass-0.3.5/pytreeclass.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytreeclass
-Version: 0.3.4
+Version: 0.3.5
 Summary: JAX compatible dataclass.
 Home-page: https://github.com/ASEM000/pytreeclass
 Author: Mahmoud Asem
 Author-email: asem00@kaist.ac.kr
 License: Apache-2.0
 Keywords: python machine-learning pytorch jax
 Classifier: Development Status :: 5 - Production/Stable
@@ -535,43 +535,54 @@
 print(counter.calls) # 10
 ```
 
 </details>
 
 ## ➕ More<a id="more"></a>
 
-<details> <summary>Validate or convert inputs using callbacks</summary>
+<details> <summary>Validate or convert inputs using type hints</summary>
 
-`PyTreeClass` includes `callbacks` in the `field` to apply a sequence of functions on input at setting the attribute stage. The callback is quite useful in several cases, for instance, to ensure a certain input type within a valid range. See example:
+`PyTreeClass` executes functions defined inside `typing.Annotated` on field values before assigning it to the instance.
+The functionality can be quite useful in several cases, for instance, to ensure a certain input type within a valid range. See example:
 
 ```python
 import jax
 import pytreeclass as pytc
-
-def positive_int_callback(value):
-    if not isinstance(value, int):
-        raise TypeError("Value must be an integer")
-    if value <= 0:
-        raise ValueError("Value must be positive")
-    return value
+# python 3.9 and above
+from typing import Annotated
+# python 3.8
+# from typing_extensions import Annotated
+
+class PositiveInt:
+    def __call__(self,value):
+        if not isinstance(value, int):
+            raise TypeError("Value must be an integer")
+        if value <= 0:
+            raise ValueError("Value must be positive")
+        return value
 
 
 class Tree(pytc.TreeClass):
-    in_features:int = pytc.field(callbacks=[positive_int_callback])
-
+    in_features: Annotated[int, PositiveInt()]
 
 tree = Tree(1)
 # no error
 
-tree = Tree(0)
-# ValueError: Error for field=`in_features`:
+try:
+    tree = Tree(0)
+except ValueError as e:
+    print(e)
+# Error for field=`in_features`:
 # Value must be positive
 
-tree = Tree(1.0)
-# TypeError: Error for field=`in_features`:
+try:
+    tree = Tree(1.0)
+except TypeError as e:
+    print(e)
+# Error for field=`in_features`:
 # Value must be an integer
 ```
 
 </details>
 
 <details>  <summary> Add leafwise math operations to PyTreeClass wrapped class</summary>
```

### Comparing `pytreeclass-0.3.4/pytreeclass.egg-info/SOURCES.txt` & `pytreeclass-0.3.5/pytreeclass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.4/setup.py` & `pytreeclass-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.4/tests/test_indexing.py` & `pytreeclass-0.3.5/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.4/tests/test_nn.py` & `pytreeclass-0.3.5/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.4/tests/test_tree_freeze.py` & `pytreeclass-0.3.5/tests/test_tree_freeze.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.4/tests/test_tree_operator.py` & `pytreeclass-0.3.5/tests/test_tree_operator.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.4/tests/test_tree_pprint.py` & `pytreeclass-0.3.5/tests/test_tree_pprint.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.4/tests/test_tree_viz_util.py` & `pytreeclass-0.3.5/tests/test_tree_viz_util.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.4/tests/test_treeclass.py` & `pytreeclass-0.3.5/tests/test_treeclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Any
 
 import jax
 import jax.tree_util as jtu
 import numpy.testing as npt
 import pytest
 from jax import numpy as jnp
+from typing_extensions import Annotated
 
 import pytreeclass as pytc
 
 
 def test_field_mutually_exclusive():
     with pytest.raises(ValueError):
         pytc.field(default=1, factory=lambda: 1)
@@ -365,71 +366,61 @@
             if x < min or x > max:
                 raise AssertionError
             return x
 
         return _range_validator
 
     class Test(pytc.TreeClass):
-        a: int = pytc.field(callbacks=[instance_validator(int)])
+        a: Annotated[int, instance_validator(int)]
 
     with pytest.raises(AssertionError):
         Test(a="a")
 
     assert Test(a=1).a == 1
 
     class Test(pytc.TreeClass):
-        a: int = pytc.field(callbacks=[instance_validator((int, float))])
+        a: Annotated[int, instance_validator((int, float))]
 
     assert Test(a=1).a == 1
     assert Test(a=1.0).a == 1.0
 
     with pytest.raises(AssertionError):
         Test(a="a")
 
     class Test(pytc.TreeClass):
-        a: int = pytc.field(callbacks=[range_validator(0, 10)])
+        a: Annotated[int, range_validator(0, 10)]
 
     with pytest.raises(AssertionError):
         Test(a=-1)
 
     assert Test(a=0).a == 0
 
     with pytest.raises(AssertionError):
         Test(a=11)
 
     class Test(pytc.TreeClass):
-        a: int = pytc.field(callbacks=[range_validator(0, 10), instance_validator(int)])
+        a: Annotated[int, range_validator(0, 10), instance_validator(int)]
 
     with pytest.raises(AssertionError):
         Test(a=-1)
 
     with pytest.raises(AssertionError):
         Test(a=11)
 
     with pytest.raises(TypeError):
 
         class Test(pytc.TreeClass):
-            a: int = pytc.field(callbacks=1)
-
-    with pytest.raises(TypeError):
-
-        class Test(pytc.TreeClass):
-            a: int = pytc.field(callbacks=[1])
-
-    with pytest.raises(TypeError):
-
-        class Test(pytc.TreeClass):
-            a: int = pytc.field(callbacks=[lambda: True])
+            a: Annotated[int, lambda: True]
 
         Test(a=1)
 
 
 def test_treeclass_frozen_field():
     class Test(pytc.TreeClass):
-        a: int = pytc.field(callbacks=[pytc.freeze])
+        a: Annotated[int, pytc.freeze]
 
     t = Test(1)
 
     assert t.a == pytc.freeze(1)
     assert jtu.tree_leaves(t) == []
```

### Comparing `pytreeclass-0.3.4/tests/test_under_jit.py` & `pytreeclass-0.3.5/tests/test_under_jit.py`

 * *Files identical despite different names*

