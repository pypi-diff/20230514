# Comparing `tmp/worktoy-0.25.tar.gz` & `tmp/worktoy-0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "worktoy-0.25.tar", last modified: Sat May 13 03:51:54 2023, max compression
+gzip compressed data, was "worktoy-0.28.tar", last modified: Sun May 14 09:41:35 2023, max compression
```

## Comparing `worktoy-0.25.tar` & `worktoy-0.28.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 03:51:54.305395 worktoy-0.25/
--rw-rw-rw-   0        0        0     1096 2023-05-12 03:07:56.000000 worktoy-0.25/LICENSE
--rw-rw-rw-   0        0        0     7155 2023-05-13 03:51:54.305395 worktoy-0.25/PKG-INFO
--rw-rw-rw-   0        0        0     6650 2023-05-12 18:41:19.000000 worktoy-0.25/README.md
--rw-rw-rw-   0        0        0      595 2023-05-13 03:09:55.000000 worktoy-0.25/pyproject.toml
--rw-rw-rw-   0        0        0      585 2023-05-13 03:51:54.306396 worktoy-0.25/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-13 03:51:54.279425 worktoy-0.25/src/
-drwxrwxrwx   0        0        0        0 2023-05-13 03:51:54.290341 worktoy-0.25/src/worktoy/
--rw-rw-rw-   0        0        0      414 2023-05-12 18:45:18.000000 worktoy-0.25/src/worktoy/__init__.py
--rw-rw-rw-   0        0        0      901 2023-05-12 19:25:01.000000 worktoy-0.25/src/worktoy/_anywayuwantit.py
--rw-rw-rw-   0        0        0     3279 2023-05-12 20:26:22.000000 worktoy-0.25/src/worktoy/_callmemaybe.py
--rw-rw-rw-   0        0        0      438 2023-05-12 06:13:52.000000 worktoy-0.25/src/worktoy/_maybe.py
--rw-rw-rw-   0        0        0      497 2023-05-12 06:17:00.000000 worktoy-0.25/src/worktoy/_maybeType.py
--rw-rw-rw-   0        0        0      775 2023-05-12 10:47:24.000000 worktoy-0.25/src/worktoy/_maybeTypes.py
--rw-rw-rw-   0        0        0     3304 2023-05-12 09:36:50.000000 worktoy-0.25/src/worktoy/_searchKeys.py
--rw-rw-rw-   0        0        0     2421 2023-05-12 11:53:37.000000 worktoy-0.25/src/worktoy/_stringlist.py
-drwxrwxrwx   0        0        0        0 2023-05-13 03:51:54.297124 worktoy-0.25/src/worktoy/mockdata/
--rw-rw-rw-   0        0        0      234 2023-05-12 16:56:26.000000 worktoy-0.25/src/worktoy/mockdata/__init__.py
--rw-rw-rw-   0        0        0     3575 2023-05-12 17:55:55.000000 worktoy-0.25/src/worktoy/mockdata/_intfactory.py
--rw-rw-rw-   0        0        0      920 2023-05-12 10:47:13.000000 worktoy-0.25/src/worktoy/mockdata/_strfactory.py
-drwxrwxrwx   0        0        0        0 2023-05-13 03:51:54.295143 worktoy-0.25/src/worktoy.egg-info/
--rw-rw-rw-   0        0        0     7155 2023-05-13 03:51:54.000000 worktoy-0.25/src/worktoy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      699 2023-05-13 03:51:54.000000 worktoy-0.25/src/worktoy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 03:51:54.000000 worktoy-0.25/src/worktoy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-13 03:51:54.000000 worktoy-0.25/src/worktoy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-13 03:51:54.303907 worktoy-0.25/tests/
--rw-rw-rw-   0        0        0     5886 2023-05-12 09:45:06.000000 worktoy-0.25/tests/testSearchKeys.py
--rw-rw-rw-   0        0        0     3145 2023-05-12 20:23:16.000000 worktoy-0.25/tests/test__callmemaybe.py
--rw-rw-rw-   0        0        0     1163 2023-05-12 19:23:01.000000 worktoy-0.25/tests/test__intfactory.py
--rw-rw-rw-   0        0        0      750 2023-05-12 07:23:58.000000 worktoy-0.25/tests/test__maybe.py
--rw-rw-rw-   0        0        0     1141 2023-05-12 08:31:06.000000 worktoy-0.25/tests/test__maybeType.py
--rw-rw-rw-   0        0        0     1722 2023-05-12 09:48:15.000000 worktoy-0.25/tests/test__maybeTypes.py
--rw-rw-rw-   0        0        0     1553 2023-05-12 10:42:03.000000 worktoy-0.25/tests/test__strfactory.py
--rw-rw-rw-   0        0        0     1881 2023-05-12 12:13:26.000000 worktoy-0.25/tests/test__stringlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:41:35.142263 worktoy-0.28/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-14 09:41:23.000000 worktoy-0.28/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-05-14 09:41:35.142263 worktoy-0.28/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-05-14 09:41:23.000000 worktoy-0.28/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-14 09:41:23.000000 worktoy-0.28/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-14 09:41:35.142263 worktoy-0.28/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:41:35.138263 worktoy-0.28/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:41:35.138263 worktoy-0.28/src/worktoy/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-14 09:41:23.000000 worktoy-0.28/src/worktoy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-14 09:41:23.000000 worktoy-0.28/src/worktoy/_anywayuwantit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-14 09:41:23.000000 worktoy-0.28/src/worktoy/_callmemaybe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-14 09:41:23.000000 worktoy-0.28/src/worktoy/_maybe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-14 09:41:23.000000 worktoy-0.28/src/worktoy/_maybeType.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-14 09:41:23.000000 worktoy-0.28/src/worktoy/_maybeTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-14 09:41:23.000000 worktoy-0.28/src/worktoy/_searchKeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-14 09:41:23.000000 worktoy-0.28/src/worktoy/_stringlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:41:35.142263 worktoy-0.28/src/worktoy/mockdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-14 09:41:23.000000 worktoy-0.28/src/worktoy/mockdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-14 09:41:23.000000 worktoy-0.28/src/worktoy/mockdata/_intfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-14 09:41:23.000000 worktoy-0.28/src/worktoy/mockdata/_strfactory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:41:35.138263 worktoy-0.28/src/worktoy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-05-14 09:41:35.000000 worktoy-0.28/src/worktoy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-14 09:41:35.000000 worktoy-0.28/src/worktoy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 09:41:35.000000 worktoy-0.28/src/worktoy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-14 09:41:35.000000 worktoy-0.28/src/worktoy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:41:35.142263 worktoy-0.28/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-14 09:41:23.000000 worktoy-0.28/tests/test__callmemaybe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-14 09:41:23.000000 worktoy-0.28/tests/test__intfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-14 09:41:23.000000 worktoy-0.28/tests/test__maybe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-14 09:41:23.000000 worktoy-0.28/tests/test__maybeType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-14 09:41:23.000000 worktoy-0.28/tests/test__maybeTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-14 09:41:23.000000 worktoy-0.28/tests/test__searchKeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-14 09:41:23.000000 worktoy-0.28/tests/test__strfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-14 09:41:23.000000 worktoy-0.28/tests/test__stringlist.py
```

### Comparing `worktoy-0.25/LICENSE` & `worktoy-0.28/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Asger Jon Vistisen
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Asger Jon Vistisen
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `worktoy-0.25/PKG-INFO` & `worktoy-0.28/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,195 +1,195 @@
-Metadata-Version: 2.1
-Name: worktoy
-Version: 0.25
-Summary: Collection of Utilities
-Author-email: Asger Jon Vistisen <asgerjon2@gmail.com>
-Project-URL: Homepage, https://github.com/AsgerJon/WorkToy
-Project-URL: Bug Tracker, https://github.com/AsgerJon/WorkToy
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# WorkToy
-
-Collection of General Utilities
-
-## The None-aware 'maybe'
-
-In a programming language which shall rename nameless as well as typeless,
-the following syntax is available:
-
-    const func = (arg = null) => {
-        let val1 = arg || 1.0;
-        let val2 = arg ?? 1.0;
-        return [val1, val2]; }
-
-In the above code, the default argument is set to null (in this context
-null is treated the same as None in Python). The `??` operator is the
-null-coalescence operator, which is nearly the same as the `or` operator.  
-Consider the return value obtained from calling `func()`:
-
-    func()
-    >>> (2)  [1, 1]
-
-This makes sense, but what happens when we call the function on a falsy
-value other than null, such as 0:
-
-    func(0)
-    >>> (3)  [1, 0]
-
-The first value in the return value comes from using the pipes (the
-logical or operator), is not aware of the difference between null and
-other falsy values. The null-coalescence operator is able to tell the
-difference. The WorkToy module brings this to python along with several
-derived utility functions:
-
-### `maybe`
-
-In the below python code, we implement the same function using the maybe
-function from WorkToy:
-
-    def func(arg: Any = None) -> Any:
-        """Function using the maybe from the WorkToy module"""
-        val1 = arg or 1.0
-        val2 = maybe(arg, 1.0)
-        return [val1, val2]
-
-The implementation of maybe simply follows a common pattern:
-
-    def maybe(*args) -> Any:
-        """Implementation of maybe returns the first argument given that 
-        is different from None. If no such argument is found None is 
-        returned."""
-        for arg in args:
-            if arg is not None: 
-                return arg
-        return None
-
-Unlike the `??` operator, the `maybe` operator handles an arbitrary
-number of arguments.
-
-### `maybeType`
-
-The first of the derived functions finds the first argument of a
-particular type:
-
-    def maybeType(type_: type, *args) -> type_:
-        """Returns the first argument of given type"""
-
-### `maybeTypes`
-
-Adding an 's' returns every argument of given type. Further, it supports
-keyword arguments `pad: int` and `padChar: Any`. If `pad` is given it
-defines the length of the returned list padded with `padChar` or `None`
-by default. Setting `pad` will either pad or crop as necessary.
-
-### `searchKeys`
-
-A common way to handle optional keyword arguments is something like:
-
-    def func(*args, **kwargs) -> Any:
-        """Common function accepting arbitrary positional and keyword 
-        arguments."""
-        val = kwargs.get('key', defaultValue)
-        ...
-
-In the above code, the `get` function is used to look for a given key in
-the collection of keyword arguments along with a (optional) default value.
-Instead, `searchKeys` allows for multiple keys in order of priority:
-
-    def func(*args, **kwargs) -> Any:
-        """Common function accepting arbitrary positional and keyword 
-        arguments."""
-        dV = defaultValue
-        val = searchKeys('k1', 'k2', 'k3', **kwargs)
-        ...
-
-In addition, WorkToy provides the following syntactic pork-scratchings
-for the keto-aware programmer:
-
-    def func(*args, **kwargs) -> Any:
-        """Common function accepting arbitrary positional and keyword 
-        arguments."""
-        dV = defaultValue
-        val = searchKeys('k1', 'k2', 'k3') @ int >> (kwargs, dV)
-        ...
-
-The matrix multiplication operator `@` sets a type requirement and the
-right-shift operator `>>` invokes the search. The default value is then
-given as the second positional argument in the tuple. Please note that
-absense of `**`. This causes `kwargs` to be treated as a dictionary
-entirely contained at the first positional argument. If invoked without a
-default value, the parentheses may be omitted.
-
-### `CallMeMaybe`
-
-This abstract baseclass registers any callable object as an instance.
-This makes it stronger than the built-in `callable` and even the
-`Callable` from the `typing` package. If a custom class implements the
-`__call__` method, instances of this class may still not be recognized as
-callable by the mentioned methods.
-
-    class FilteredClass:
-        """A class requiring a callable filter before invoking some other 
-        function"""
-
-        def __init__(self, *args, **kwargs) -> None:
-            filterKwarg = searchKeys('filter') @ CallMeMaybe >> kwargs
-            filterArg = maybeType(CallMeMaybe, *args)
-            filterDefault = lambda *arg, **kwargs: (arg, kwargs)
-            self._filter = maybe(filterKwarg, filterArg, filterDefault)
-            self._func = someFunction
-        
-        def __call__(self, *args, **kwargs) -> Any:
-            """Invokes some underlying function subject to the filter"""
-            return self._func(self._filter(*args, **kwargs))
-
-Additionally, decorate functions with `CallMeMaybe` to explicitly flag
-functions as being instances of `CallMeMaybe`. As expected, instances of
-subclasses of `CallMeMaybe` are regarded as instances.
-
-## String Tools
-
-WorkToy also brings a number of convenient string related functions:
-
-### `stringList`
-
-Consider the following code:
-
-`numbers = ['one', 'two', 'three', 'four']`
-The above involve repeated use of `'`. On the Danish keyboard layout, the
-`'` key is located as indicated `jklæø'`, meaning that the right pinky
-finger must leap over two other keys. Instead, use `stringList`:
-
-    numbers = stringList('one, two, three, four', )
-    >>> ['one', 'two', 'three', 'four']
-
-### `monoSpace`
-
-Consider the following code:
-
-    msg = """Hello there! I am writing a long string right here in python 
-    that stretches in length beyond the allowable line length. Thankfully,
-    we have the triple quotation mark syntax for indication of longer 
-    strings."""
-
-The above code takes things literally meaning that new lines are inserted.
-Thus, in between 'python' at the end of the first line and 'that' at the
-beginning of the second line, a `'\n'` has been inserted. Instead, use
-`monoSpace`:
-
-    msgLine = monoSpace(msg)  # msg as defined above
-
-Now `msgLine` contains now new lines and no repeated spaces. To
-explicitly set a line break in the string, insert `'<br>'` in the text.
-Set a different string to denote a line break, give that string as the
-second argument.
-
-    rawLines = """This is the first line. <br>   Here is the second line. 
-    Don't worry about the extra spaces surrounding the tag, they are 
-    removed. """
-    
-    twoLines = monoSpace(rawLines)
+Metadata-Version: 2.1
+Name: worktoy
+Version: 0.28
+Summary: Collection of Utilities
+Author-email: Asger Jon Vistisen <asgerjon2@gmail.com>
+Project-URL: Homepage, https://github.com/AsgerJon/WorkToy
+Project-URL: Bug Tracker, https://github.com/AsgerJon/WorkToy
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# WorkToy
+
+Collection of General Utilities
+
+## The None-aware 'maybe'
+
+In a programming language which shall rename nameless as well as typeless,
+the following syntax is available:
+
+    const func = (arg = null) => {
+        let val1 = arg || 1.0;
+        let val2 = arg ?? 1.0;
+        return [val1, val2]; }
+
+In the above code, the default argument is set to null (in this context
+null is treated the same as None in Python). The `??` operator is the
+null-coalescence operator, which is nearly the same as the `or` operator.  
+Consider the return value obtained from calling `func()`:
+
+    func()
+    >>> (2)  [1, 1]
+
+This makes sense, but what happens when we call the function on a falsy
+value other than null, such as 0:
+
+    func(0)
+    >>> (3)  [1, 0]
+
+The first value in the return value comes from using the pipes (the
+logical or operator), is not aware of the difference between null and
+other falsy values. The null-coalescence operator is able to tell the
+difference. The WorkToy module brings this to python along with several
+derived utility functions:
+
+### `maybe`
+
+In the below python code, we implement the same function using the maybe
+function from WorkToy:
+
+    def func(arg: Any = None) -> Any:
+        """Function using the maybe from the WorkToy module"""
+        val1 = arg or 1.0
+        val2 = maybe(arg, 1.0)
+        return [val1, val2]
+
+The implementation of maybe simply follows a common pattern:
+
+    def maybe(*args) -> Any:
+        """Implementation of maybe returns the first argument given that 
+        is different from None. If no such argument is found None is 
+        returned."""
+        for arg in args:
+            if arg is not None: 
+                return arg
+        return None
+
+Unlike the `??` operator, the `maybe` operator handles an arbitrary
+number of arguments.
+
+### `maybeType`
+
+The first of the derived functions finds the first argument of a
+particular type:
+
+    def maybeType(type_: type, *args) -> type_:
+        """Returns the first argument of given type"""
+
+### `maybeTypes`
+
+Adding an 's' returns every argument of given type. Further, it supports
+keyword arguments `pad: int` and `padChar: Any`. If `pad` is given it
+defines the length of the returned list padded with `padChar` or `None`
+by default. Setting `pad` will either pad or crop as necessary.
+
+### `searchKeys`
+
+A common way to handle optional keyword arguments is something like:
+
+    def func(*args, **kwargs) -> Any:
+        """Common function accepting arbitrary positional and keyword 
+        arguments."""
+        val = kwargs.get('key', defaultValue)
+        ...
+
+In the above code, the `get` function is used to look for a given key in
+the collection of keyword arguments along with a (optional) default value.
+Instead, `searchKeys` allows for multiple keys in order of priority:
+
+    def func(*args, **kwargs) -> Any:
+        """Common function accepting arbitrary positional and keyword 
+        arguments."""
+        dV = defaultValue
+        val = searchKeys('k1', 'k2', 'k3', **kwargs)
+        ...
+
+In addition, WorkToy provides the following syntactic pork-scratchings
+for the keto-aware programmer:
+
+    def func(*args, **kwargs) -> Any:
+        """Common function accepting arbitrary positional and keyword 
+        arguments."""
+        dV = defaultValue
+        val = searchKeys('k1', 'k2', 'k3') @ int >> (kwargs, dV)
+        ...
+
+The matrix multiplication operator `@` sets a type requirement and the
+right-shift operator `>>` invokes the search. The default value is then
+given as the second positional argument in the tuple. Please note that
+absense of `**`. This causes `kwargs` to be treated as a dictionary
+entirely contained at the first positional argument. If invoked without a
+default value, the parentheses may be omitted.
+
+### `CallMeMaybe`
+
+This abstract baseclass registers any callable object as an instance.
+This makes it stronger than the built-in `callable` and even the
+`Callable` from the `typing` package. If a custom class implements the
+`__call__` method, instances of this class may still not be recognized as
+callable by the mentioned methods.
+
+    class FilteredClass:
+        """A class requiring a callable filter before invoking some other 
+        function"""
+
+        def __init__(self, *args, **kwargs) -> None:
+            filterKwarg = searchKeys('filter') @ CallMeMaybe >> kwargs
+            filterArg = maybeType(CallMeMaybe, *args)
+            filterDefault = lambda *arg, **kwargs: (arg, kwargs)
+            self._filter = maybe(filterKwarg, filterArg, filterDefault)
+            self._func = someFunction
+        
+        def __call__(self, *args, **kwargs) -> Any:
+            """Invokes some underlying function subject to the filter"""
+            return self._func(self._filter(*args, **kwargs))
+
+Additionally, decorate functions with `CallMeMaybe` to explicitly flag
+functions as being instances of `CallMeMaybe`. As expected, instances of
+subclasses of `CallMeMaybe` are regarded as instances.
+
+## String Tools
+
+WorkToy also brings a number of convenient string related functions:
+
+### `stringList`
+
+Consider the following code:
+
+`numbers = ['one', 'two', 'three', 'four']`
+The above involve repeated use of `'`. On the Danish keyboard layout, the
+`'` key is located as indicated `jklæø'`, meaning that the right pinky
+finger must leap over two other keys. Instead, use `stringList`:
+
+    numbers = stringList('one, two, three, four', )
+    >>> ['one', 'two', 'three', 'four']
+
+### `monoSpace`
+
+Consider the following code:
+
+    msg = """Hello there! I am writing a long string right here in python 
+    that stretches in length beyond the allowable line length. Thankfully,
+    we have the triple quotation mark syntax for indication of longer 
+    strings."""
+
+The above code takes things literally meaning that new lines are inserted.
+Thus, in between 'python' at the end of the first line and 'that' at the
+beginning of the second line, a `'\n'` has been inserted. Instead, use
+`monoSpace`:
+
+    msgLine = monoSpace(msg)  # msg as defined above
+
+Now `msgLine` contains now new lines and no repeated spaces. To
+explicitly set a line break in the string, insert `'<br>'` in the text.
+Set a different string to denote a line break, give that string as the
+second argument.
+
+    rawLines = """This is the first line. <br>   Here is the second line. 
+    Don't worry about the extra spaces surrounding the tag, they are 
+    removed. """
+    
+    twoLines = monoSpace(rawLines)
```

### Comparing `worktoy-0.25/README.md` & `worktoy-0.28/README.md`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,181 +1,181 @@
-# WorkToy
-
-Collection of General Utilities
-
-## The None-aware 'maybe'
-
-In a programming language which shall rename nameless as well as typeless,
-the following syntax is available:
-
-    const func = (arg = null) => {
-        let val1 = arg || 1.0;
-        let val2 = arg ?? 1.0;
-        return [val1, val2]; }
-
-In the above code, the default argument is set to null (in this context
-null is treated the same as None in Python). The `??` operator is the
-null-coalescence operator, which is nearly the same as the `or` operator.  
-Consider the return value obtained from calling `func()`:
-
-    func()
-    >>> (2)  [1, 1]
-
-This makes sense, but what happens when we call the function on a falsy
-value other than null, such as 0:
-
-    func(0)
-    >>> (3)  [1, 0]
-
-The first value in the return value comes from using the pipes (the
-logical or operator), is not aware of the difference between null and
-other falsy values. The null-coalescence operator is able to tell the
-difference. The WorkToy module brings this to python along with several
-derived utility functions:
-
-### `maybe`
-
-In the below python code, we implement the same function using the maybe
-function from WorkToy:
-
-    def func(arg: Any = None) -> Any:
-        """Function using the maybe from the WorkToy module"""
-        val1 = arg or 1.0
-        val2 = maybe(arg, 1.0)
-        return [val1, val2]
-
-The implementation of maybe simply follows a common pattern:
-
-    def maybe(*args) -> Any:
-        """Implementation of maybe returns the first argument given that 
-        is different from None. If no such argument is found None is 
-        returned."""
-        for arg in args:
-            if arg is not None: 
-                return arg
-        return None
-
-Unlike the `??` operator, the `maybe` operator handles an arbitrary
-number of arguments.
-
-### `maybeType`
-
-The first of the derived functions finds the first argument of a
-particular type:
-
-    def maybeType(type_: type, *args) -> type_:
-        """Returns the first argument of given type"""
-
-### `maybeTypes`
-
-Adding an 's' returns every argument of given type. Further, it supports
-keyword arguments `pad: int` and `padChar: Any`. If `pad` is given it
-defines the length of the returned list padded with `padChar` or `None`
-by default. Setting `pad` will either pad or crop as necessary.
-
-### `searchKeys`
-
-A common way to handle optional keyword arguments is something like:
-
-    def func(*args, **kwargs) -> Any:
-        """Common function accepting arbitrary positional and keyword 
-        arguments."""
-        val = kwargs.get('key', defaultValue)
-        ...
-
-In the above code, the `get` function is used to look for a given key in
-the collection of keyword arguments along with a (optional) default value.
-Instead, `searchKeys` allows for multiple keys in order of priority:
-
-    def func(*args, **kwargs) -> Any:
-        """Common function accepting arbitrary positional and keyword 
-        arguments."""
-        dV = defaultValue
-        val = searchKeys('k1', 'k2', 'k3', **kwargs)
-        ...
-
-In addition, WorkToy provides the following syntactic pork-scratchings
-for the keto-aware programmer:
-
-    def func(*args, **kwargs) -> Any:
-        """Common function accepting arbitrary positional and keyword 
-        arguments."""
-        dV = defaultValue
-        val = searchKeys('k1', 'k2', 'k3') @ int >> (kwargs, dV)
-        ...
-
-The matrix multiplication operator `@` sets a type requirement and the
-right-shift operator `>>` invokes the search. The default value is then
-given as the second positional argument in the tuple. Please note that
-absense of `**`. This causes `kwargs` to be treated as a dictionary
-entirely contained at the first positional argument. If invoked without a
-default value, the parentheses may be omitted.
-
-### `CallMeMaybe`
-
-This abstract baseclass registers any callable object as an instance.
-This makes it stronger than the built-in `callable` and even the
-`Callable` from the `typing` package. If a custom class implements the
-`__call__` method, instances of this class may still not be recognized as
-callable by the mentioned methods.
-
-    class FilteredClass:
-        """A class requiring a callable filter before invoking some other 
-        function"""
-
-        def __init__(self, *args, **kwargs) -> None:
-            filterKwarg = searchKeys('filter') @ CallMeMaybe >> kwargs
-            filterArg = maybeType(CallMeMaybe, *args)
-            filterDefault = lambda *arg, **kwargs: (arg, kwargs)
-            self._filter = maybe(filterKwarg, filterArg, filterDefault)
-            self._func = someFunction
-        
-        def __call__(self, *args, **kwargs) -> Any:
-            """Invokes some underlying function subject to the filter"""
-            return self._func(self._filter(*args, **kwargs))
-
-Additionally, decorate functions with `CallMeMaybe` to explicitly flag
-functions as being instances of `CallMeMaybe`. As expected, instances of
-subclasses of `CallMeMaybe` are regarded as instances.
-
-## String Tools
-
-WorkToy also brings a number of convenient string related functions:
-
-### `stringList`
-
-Consider the following code:
-
-`numbers = ['one', 'two', 'three', 'four']`
-The above involve repeated use of `'`. On the Danish keyboard layout, the
-`'` key is located as indicated `jklæø'`, meaning that the right pinky
-finger must leap over two other keys. Instead, use `stringList`:
-
-    numbers = stringList('one, two, three, four', )
-    >>> ['one', 'two', 'three', 'four']
-
-### `monoSpace`
-
-Consider the following code:
-
-    msg = """Hello there! I am writing a long string right here in python 
-    that stretches in length beyond the allowable line length. Thankfully,
-    we have the triple quotation mark syntax for indication of longer 
-    strings."""
-
-The above code takes things literally meaning that new lines are inserted.
-Thus, in between 'python' at the end of the first line and 'that' at the
-beginning of the second line, a `'\n'` has been inserted. Instead, use
-`monoSpace`:
-
-    msgLine = monoSpace(msg)  # msg as defined above
-
-Now `msgLine` contains now new lines and no repeated spaces. To
-explicitly set a line break in the string, insert `'<br>'` in the text.
-Set a different string to denote a line break, give that string as the
-second argument.
-
-    rawLines = """This is the first line. <br>   Here is the second line. 
-    Don't worry about the extra spaces surrounding the tag, they are 
-    removed. """
-    
-    twoLines = monoSpace(rawLines)
+# WorkToy
+
+Collection of General Utilities
+
+## The None-aware 'maybe'
+
+In a programming language which shall rename nameless as well as typeless,
+the following syntax is available:
+
+    const func = (arg = null) => {
+        let val1 = arg || 1.0;
+        let val2 = arg ?? 1.0;
+        return [val1, val2]; }
+
+In the above code, the default argument is set to null (in this context
+null is treated the same as None in Python). The `??` operator is the
+null-coalescence operator, which is nearly the same as the `or` operator.  
+Consider the return value obtained from calling `func()`:
+
+    func()
+    >>> (2)  [1, 1]
+
+This makes sense, but what happens when we call the function on a falsy
+value other than null, such as 0:
+
+    func(0)
+    >>> (3)  [1, 0]
+
+The first value in the return value comes from using the pipes (the
+logical or operator), is not aware of the difference between null and
+other falsy values. The null-coalescence operator is able to tell the
+difference. The WorkToy module brings this to python along with several
+derived utility functions:
+
+### `maybe`
+
+In the below python code, we implement the same function using the maybe
+function from WorkToy:
+
+    def func(arg: Any = None) -> Any:
+        """Function using the maybe from the WorkToy module"""
+        val1 = arg or 1.0
+        val2 = maybe(arg, 1.0)
+        return [val1, val2]
+
+The implementation of maybe simply follows a common pattern:
+
+    def maybe(*args) -> Any:
+        """Implementation of maybe returns the first argument given that 
+        is different from None. If no such argument is found None is 
+        returned."""
+        for arg in args:
+            if arg is not None: 
+                return arg
+        return None
+
+Unlike the `??` operator, the `maybe` operator handles an arbitrary
+number of arguments.
+
+### `maybeType`
+
+The first of the derived functions finds the first argument of a
+particular type:
+
+    def maybeType(type_: type, *args) -> type_:
+        """Returns the first argument of given type"""
+
+### `maybeTypes`
+
+Adding an 's' returns every argument of given type. Further, it supports
+keyword arguments `pad: int` and `padChar: Any`. If `pad` is given it
+defines the length of the returned list padded with `padChar` or `None`
+by default. Setting `pad` will either pad or crop as necessary.
+
+### `searchKeys`
+
+A common way to handle optional keyword arguments is something like:
+
+    def func(*args, **kwargs) -> Any:
+        """Common function accepting arbitrary positional and keyword 
+        arguments."""
+        val = kwargs.get('key', defaultValue)
+        ...
+
+In the above code, the `get` function is used to look for a given key in
+the collection of keyword arguments along with a (optional) default value.
+Instead, `searchKeys` allows for multiple keys in order of priority:
+
+    def func(*args, **kwargs) -> Any:
+        """Common function accepting arbitrary positional and keyword 
+        arguments."""
+        dV = defaultValue
+        val = searchKeys('k1', 'k2', 'k3', **kwargs)
+        ...
+
+In addition, WorkToy provides the following syntactic pork-scratchings
+for the keto-aware programmer:
+
+    def func(*args, **kwargs) -> Any:
+        """Common function accepting arbitrary positional and keyword 
+        arguments."""
+        dV = defaultValue
+        val = searchKeys('k1', 'k2', 'k3') @ int >> (kwargs, dV)
+        ...
+
+The matrix multiplication operator `@` sets a type requirement and the
+right-shift operator `>>` invokes the search. The default value is then
+given as the second positional argument in the tuple. Please note that
+absense of `**`. This causes `kwargs` to be treated as a dictionary
+entirely contained at the first positional argument. If invoked without a
+default value, the parentheses may be omitted.
+
+### `CallMeMaybe`
+
+This abstract baseclass registers any callable object as an instance.
+This makes it stronger than the built-in `callable` and even the
+`Callable` from the `typing` package. If a custom class implements the
+`__call__` method, instances of this class may still not be recognized as
+callable by the mentioned methods.
+
+    class FilteredClass:
+        """A class requiring a callable filter before invoking some other 
+        function"""
+
+        def __init__(self, *args, **kwargs) -> None:
+            filterKwarg = searchKeys('filter') @ CallMeMaybe >> kwargs
+            filterArg = maybeType(CallMeMaybe, *args)
+            filterDefault = lambda *arg, **kwargs: (arg, kwargs)
+            self._filter = maybe(filterKwarg, filterArg, filterDefault)
+            self._func = someFunction
+        
+        def __call__(self, *args, **kwargs) -> Any:
+            """Invokes some underlying function subject to the filter"""
+            return self._func(self._filter(*args, **kwargs))
+
+Additionally, decorate functions with `CallMeMaybe` to explicitly flag
+functions as being instances of `CallMeMaybe`. As expected, instances of
+subclasses of `CallMeMaybe` are regarded as instances.
+
+## String Tools
+
+WorkToy also brings a number of convenient string related functions:
+
+### `stringList`
+
+Consider the following code:
+
+`numbers = ['one', 'two', 'three', 'four']`
+The above involve repeated use of `'`. On the Danish keyboard layout, the
+`'` key is located as indicated `jklæø'`, meaning that the right pinky
+finger must leap over two other keys. Instead, use `stringList`:
+
+    numbers = stringList('one, two, three, four', )
+    >>> ['one', 'two', 'three', 'four']
+
+### `monoSpace`
+
+Consider the following code:
+
+    msg = """Hello there! I am writing a long string right here in python 
+    that stretches in length beyond the allowable line length. Thankfully,
+    we have the triple quotation mark syntax for indication of longer 
+    strings."""
+
+The above code takes things literally meaning that new lines are inserted.
+Thus, in between 'python' at the end of the first line and 'that' at the
+beginning of the second line, a `'\n'` has been inserted. Instead, use
+`monoSpace`:
+
+    msgLine = monoSpace(msg)  # msg as defined above
+
+Now `msgLine` contains now new lines and no repeated spaces. To
+explicitly set a line break in the string, insert `'<br>'` in the text.
+Set a different string to denote a line break, give that string as the
+second argument.
+
+    rawLines = """This is the first line. <br>   Here is the second line. 
+    Don't worry about the extra spaces surrounding the tag, they are 
+    removed. """
+    
+    twoLines = monoSpace(rawLines)
```

### Comparing `worktoy-0.25/setup.cfg` & `worktoy-0.28/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-00000000: 5b4d 4554 4144 4154 415d 0d0a 6e61 6d65  [METADATA]..name
-00000010: 203d 2057 6f72 6b54 6f79 0d0a 7665 7273   = WorkToy..vers
-00000020: 696f 6e20 3d20 302e 3235 0d0a 6175 7468  ion = 0.25..auth
-00000030: 6f72 203d 2041 7367 6572 204a 6f6e 2056  or = Asger Jon V
-00000040: 6973 7469 7365 6e0d 0a61 7574 686f 725f  istisen..author_
-00000050: 656d 6169 6c20 3d20 6173 6765 726a 6f6e  email = asgerjon
-00000060: 3240 676d 6169 6c2e 636f 6d0d 0a64 6573  2@gmail.com..des
-00000070: 6372 6970 7469 6f6e 203d 2041 2043 6f6c  cription = A Col
-00000080: 6c65 6374 696f 6e20 6f66 2055 7469 6c69  lection of Utili
-00000090: 7469 6573 0d0a 6c6f 6e67 5f64 6573 6372  ties..long_descr
-000000a0: 6970 7469 6f6e 203d 2066 696c 653a 5245  iption = file:RE
-000000b0: 4144 4d45 2e6d 642c 4c49 4345 4e53 450d  ADME.md,LICENSE.
-000000c0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
-000000d0: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
-000000e0: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
-000000f0: 7572 6c20 3d20 0d0a 7072 6f6a 6563 745f  url = ..project_
-00000100: 7572 6c73 203d 200d 0a63 6c61 7373 6966  urls = ..classif
-00000110: 6965 7273 203d 200d 0a09 5072 6f67 7261  iers = ...Progra
-00000120: 6d6d 696e 6720 4c61 6e67 7561 6765 3a3a  mming Language::
-00000130: 5079 7468 6f6e 3a3a 330d 0a09 4c49 4345  Python::3...LICE
-00000140: 4e53 453a 3a0d 0a09 4f70 6572 6174 696e  NSE::...Operatin
-00000150: 6720 5379 7374 656d 3a3a 4f53 2049 6e64  g System::OS Ind
-00000160: 6570 656e 6465 6e74 0d0a 6b65 7977 6f72  ependent..keywor
-00000170: 6473 203d 200d 0a09 7574 696c 6974 6965  ds = ...utilitie
-00000180: 730d 0a09 636f 6e76 656e 6965 6e63 650d  s...convenience.
-00000190: 0a09 4173 6765 7220 4a6f 6e20 5669 7374  ..Asger Jon Vist
-000001a0: 6973 656e 0d0a 0d0a 5b4f 5054 494f 4e53  isen....[OPTIONS
-000001b0: 5d0d 0a70 6163 6b61 6765 5f64 6972 203d  ]..package_dir =
-000001c0: 200d 0a09 3d73 7263 0d0a 7061 636b 6167   ...=src..packag
-000001d0: 6573 203d 2066 696e 643a 0d0a 7079 7468  es = find:..pyth
-000001e0: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
-000001f0: 332e 380d 0a0d 0a5b 6f70 7469 6f6e 732e  3.8....[options.
-00000200: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
-00000210: 7768 6572 6520 3d20 7372 630d 0a0d 0a5b  where = src....[
-00000220: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
-00000230: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
-00000240: 6520 3d20 300d 0a0d 0a                   e = 0....
+00000000: 5b4d 4554 4144 4154 415d 0a6e 616d 6520  [METADATA].name 
+00000010: 3d20 576f 726b 546f 790a 7665 7273 696f  = WorkToy.versio
+00000020: 6e20 3d20 302e 3238 0a61 7574 686f 7220  n = 0.28.author 
+00000030: 3d20 4173 6765 7220 4a6f 6e20 5669 7374  = Asger Jon Vist
+00000040: 6973 656e 0a61 7574 686f 725f 656d 6169  isen.author_emai
+00000050: 6c20 3d20 6173 6765 726a 6f6e 3240 676d  l = asgerjon2@gm
+00000060: 6169 6c2e 636f 6d0a 6465 7363 7269 7074  ail.com.descript
+00000070: 696f 6e20 3d20 4120 436f 6c6c 6563 7469  ion = A Collecti
+00000080: 6f6e 206f 6620 5574 696c 6974 6965 730a  on of Utilities.
+00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+000000a0: 203d 2066 696c 653a 5245 4144 4d45 2e6d   = file:README.m
+000000b0: 642c 4c49 4345 4e53 450a 6c6f 6e67 5f64  d,LICENSE.long_d
+000000c0: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
+000000d0: 6e74 5f74 7970 6520 3d20 7465 7874 2f6d  nt_type = text/m
+000000e0: 6172 6b64 6f77 6e0a 7572 6c20 3d20 0a70  arkdown.url = .p
+000000f0: 726f 6a65 6374 5f75 726c 7320 3d20 0a63  roject_urls = .c
+00000100: 6c61 7373 6966 6965 7273 203d 200a 0950  lassifiers = ..P
+00000110: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000120: 6167 653a 3a50 7974 686f 6e3a 3a33 0a09  age::Python::3..
+00000130: 4c49 4345 4e53 453a 3a0a 094f 7065 7261  LICENSE::..Opera
+00000140: 7469 6e67 2053 7973 7465 6d3a 3a4f 5320  ting System::OS 
+00000150: 496e 6465 7065 6e64 656e 740a 6b65 7977  Independent.keyw
+00000160: 6f72 6473 203d 200a 0975 7469 6c69 7469  ords = ..utiliti
+00000170: 6573 0a09 636f 6e76 656e 6965 6e63 650a  es..convenience.
+00000180: 0941 7367 6572 204a 6f6e 2056 6973 7469  .Asger Jon Visti
+00000190: 7365 6e0a 0a5b 4f50 5449 4f4e 535d 0a70  sen..[OPTIONS].p
+000001a0: 6163 6b61 6765 5f64 6972 203d 200a 093d  ackage_dir = ..=
+000001b0: 7372 630a 7061 636b 6167 6573 203d 2066  src.packages = f
+000001c0: 696e 643a 0a70 7974 686f 6e5f 7265 7175  ind:.python_requ
+000001d0: 6972 6573 203d 203e 3d33 2e38 0a0a 5b6f  ires = >=3.8..[o
+000001e0: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
+000001f0: 6669 6e64 5d0a 7768 6572 6520 3d20 7372  find].where = sr
+00000200: 630a 0a5b 6567 675f 696e 666f 5d0a 7461  c..[egg_info].ta
+00000210: 675f 6275 696c 6420 3d20 0a74 6167 5f64  g_build = .tag_d
+00000220: 6174 6520 3d20 300a 0a                   ate = 0..
```

### Comparing `worktoy-0.25/src/worktoy/_anywayuwantit.py` & `worktoy-0.28/src/worktoy/_anywayuwantit.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-"""AnywayUWantIt provides a simplified abstract metaclass"""
-#  MIT License
-#  Copyright (c) 2023 Asger Jon Vistisen
-from __future__ import annotations
-
-from _py_abc import ABCMeta
-from abc import ABCMeta as ABCMetaLOL
-from typing import Any
-
-_modules = [ABCMetaLOL]
-
-
-class AnywayUWantIt(ABCMeta):
-  """AnywayUWantIt provides a simplified abstract metaclass"""
-
-  def __new__(mcls, *args, **kwargs) -> ABCMeta:
-    cls = super().__new__(mcls, *args, **kwargs)
-    return cls
-
-  def __instancecheck__(cls, instance: Any) -> bool:
-    """On the subclass, implement a function named 'recognizeInstance' to
-    explicitly define if an instance is to be regarded as an instance of
-    it."""
-    recognizeInstance = getattr(cls, 'recognizeInstance', None)
-    if recognizeInstance is None:
-      return super().__instancecheck__(instance)
-    return recognizeInstance(instance)
+"""AnywayUWantIt provides a simplified abstract metaclass"""
+#  MIT License
+#  Copyright (c) 2023 Asger Jon Vistisen
+from __future__ import annotations
+
+from _py_abc import ABCMeta
+from abc import ABCMeta as ABCMetaLOL
+from typing import Any
+
+_modules = [ABCMetaLOL]
+
+
+class AnywayUWantIt(ABCMeta):
+  """AnywayUWantIt provides a simplified abstract metaclass"""
+
+  def __new__(mcls, *args, **kwargs) -> ABCMeta:
+    cls = super().__new__(mcls, *args, **kwargs)
+    return cls
+
+  def __instancecheck__(cls, instance: Any = None) -> bool:
+    """On the subclass, implement a function named 'recognizeInstance' to
+    explicitly define if an instance is to be regarded as an instance of
+    it."""
+    if instance == cls:
+      return True
+    if instance is None:
+      return True
+    recognizeInstance = getattr(cls, 'recognizeInstance', None)
+    if recognizeInstance is None:
+      return super().__instancecheck__(instance)
+    return recognizeInstance(instance)
```

### Comparing `worktoy-0.25/src/worktoy/_callmemaybe.py` & `worktoy-0.28/src/worktoy/_callmemaybe.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,91 +1,92 @@
-"""This abstract metaclass registers any callable object as an instance."""
-#  MIT License
-#  Copyright (c) 2023 Asger Jon Vistisen
-from __future__ import annotations
-
-from typing import Any, NoReturn
-
-from worktoy import AnywayUWantIt, searchKeys, maybeType, maybe
-
-
-class CallMeMaybe(metaclass=AnywayUWantIt):
-  """This abstract metaclass registers any callable object as an instance."""
-
-  _explicits = []
-  _callables = []
-  _unCallables = []
-
-  @classmethod
-  def registerUnCallable(cls, other: type) -> NoReturn:
-    """Registers other type as being explicitly not callable"""
-    cls._unCallables.append(other)
-
-  @classmethod
-  def registerCallable(cls, other: type) -> NoReturn:
-    """Registers other type as being explicitly callable"""
-    cls._callables.append(other)
-
-  def __init__(self, *args, **kwargs) -> None:
-    callableKwarg = searchKeys('callable', 'callMeMaybe') @ bool >> kwargs
-    callableArg = maybeType(str, *args)
-    if callableArg is not None:
-      if callableArg == 'callable':
-        callableArg = True
-      elif callableArg in ['Not-callable', 'not callable']:
-        callableArg = False
-    callableDefault = True
-    self._callableFlag = maybe(callableKwarg, callableArg, callableDefault)
-
-  def __call__(self, func: Any) -> Any:
-    """Use as a function decorator. By default the decorated function are
-    regarded as callable. Change this by setting keyword argument
-    'callable' to False so that a decorated function will not be regarded
-    as a callable. """
-    if isinstance(func, type):
-      if maybe(self._callableFlag, True):
-        CallMeMaybe.registerCallable(func)
-        return func
-      CallMeMaybe.registerUnCallable(func)
-      return func
-    setattr(func, '__isCallable__', maybe(self._callableFlag, True))
-    return func
-
-  def recognizeInstance(self, instance: Any) -> bool:
-    """Recognizing anything callable as an instance"""
-    callableFlag = getattr(instance, '__isCallable__', None)
-    if callableFlag is not None:
-      if not callableFlag:
-        return False
-    if isinstance(instance, (int, float, str, complex)):
-      return False
-    if isinstance(instance, (tuple, dict, list, set)):
-      return False
-    for callableType in self._callables:
-      if isinstance(instance, callableType):
-        return True
-    for callableType in self._unCallables:
-      if isinstance(instance, callableType):
-        return False
-    if instance is None:
-      return False
-    classId = getattr(instance, '__class__', None)
-    instanceName = getattr(instance, '__name__', None)
-    if instanceName is None:
-      e = """Unable to recognize instance name"""
-      raise ValueError(e)
-    if classId is None:
-      e = """Unable to recognize class of instance"""
-      raise ValueError(e)
-    className = getattr(classId, '__name__', None)
-    if className is None:
-      e = """Unable to recognize name of instance class"""
-      raise ValueError(e)
-    if className == 'builtin_function_or_method':
-      return True
-    if className == 'function':
-      return True
-    callFunc = getattr(instance, '__call__', None)
-    if callFunc is None:
-      return False
-    if callFunc is not None:
-      return True
+"""This abstract metaclass registers any callable object as an instance."""
+#  MIT License
+#  Copyright (c) 2023 Asger Jon Vistisen
+from __future__ import annotations
+
+from typing import Any, NoReturn
+
+from worktoy import AnywayUWantIt, searchKeys, maybeType, maybe
+
+
+class CallMeMaybe(metaclass=AnywayUWantIt):
+  """This abstract metaclass registers any callable object as an instance."""
+
+  _explicits = []
+  _callables = []
+  _unCallables = []
+
+  @staticmethod
+  def recognizeInstance(instance: Any = None) -> bool:
+    """Recognizing anything callable as an instance"""
+    callableFlag = getattr(instance, '__isCallable__', None)
+    if callableFlag is not None:
+      if not callableFlag:
+        return False
+    if isinstance(instance, (int, float, str, complex)):
+      return False
+    if isinstance(instance, (tuple, dict, list, set)):
+      return False
+    for callableType in CallMeMaybe._callables:
+      if isinstance(instance, callableType):
+        return True
+    for callableType in CallMeMaybe._unCallables:
+      if isinstance(instance, callableType):
+        return False
+    if instance is None:
+      return False
+    classId = getattr(instance, '__class__', None)
+    instanceName = getattr(instance, '__name__', None)
+    if instanceName is None:
+      e = """Unable to recognize instance name"""
+      raise ValueError(e)
+    if classId is None:
+      e = """Unable to recognize class of instance"""
+      raise ValueError(e)
+    className = getattr(classId, '__name__', None)
+    if className is None:
+      e = """Unable to recognize name of instance class"""
+      raise ValueError(e)
+    if className == 'builtin_function_or_method':
+      return True
+    if className == 'function':
+      return True
+    callFunc = getattr(instance, '__call__', None)
+    if callFunc is None:
+      return False
+    if callFunc is not None:
+      return True
+
+  @classmethod
+  def registerUnCallable(cls, other: type) -> NoReturn:
+    """Registers other type as being explicitly not callable"""
+    cls._unCallables.append(other)
+
+  @classmethod
+  def registerCallable(cls, other: type) -> NoReturn:
+    """Registers other type as being explicitly callable"""
+    cls._callables.append(other)
+
+  def __init__(self, *args, **kwargs) -> None:
+    callableKwarg = searchKeys('callable', 'callMeMaybe') @ bool >> kwargs
+    callableArg = maybeType(str, *args)
+    if callableArg is not None:
+      if callableArg == 'callable':
+        callableArg = True
+      elif callableArg in ['Not-callable', 'not callable']:
+        callableArg = False
+    callableDefault = True
+    self._callableFlag = maybe(callableKwarg, callableArg, callableDefault)
+
+  def __call__(self, func: Any) -> Any:
+    """Use as a function decorator. By default, the decorated function are
+    regarded as callable. Change this by setting keyword argument
+    'callable' to False so that a decorated function will not be regarded
+    as a callable. """
+    if isinstance(func, type):
+      if maybe(self._callableFlag, True):
+        CallMeMaybe.registerCallable(func)
+        return func
+      CallMeMaybe.registerUnCallable(func)
+      return func
+    setattr(func, '__isCallable__', maybe(self._callableFlag, True))
+    return func
```

### Comparing `worktoy-0.25/src/worktoy/_searchKeys.py` & `worktoy-0.28/src/worktoy/_searchKeys.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-"""The searchKeys function provides a flexible way of extracting values
-from keyword arguments."""
-#  MIT License
-#  Copyright (c) 2023 Asger Jon Vistisen
-from __future__ import annotations
-
-from typing import Any, NoReturn
-
-
-class _SearchKeys:
-  """The searchKeys function provides a flexible way of extracting values
-  from keyword arguments.
-  #  MIT License
-  #  Copyright (c) 2023 Asger Jon Vistisen"""
-
-  @classmethod
-  def searchKeys(cls, *keys: str) -> _SearchKeys:
-    """Creates a new instance on the given keys"""
-    out = cls()
-    out._setKeys(*keys)
-    return out
-
-  def __init__(self, ) -> None:
-    self._keys = []
-    self._types = []
-    self._defVal = None
-
-  def _clearKeys(self) -> NoReturn:
-    """Deleter-function for the instance keys"""
-    while self._keys:
-      self._keys.pop()
-
-  def _setKeys(self, *keys: str) -> NoReturn:
-    """Setter-function for the instance keys"""
-    self._clearKeys()
-    for key in keys:
-      if isinstance(key, str):
-        self._keys.append(key)
-
-  def _clearTypes(self) -> NoReturn:
-    """Clears the type list"""
-    while self._types:
-      self._types.pop()
-
-  def _setType(self, *type_: type) -> NoReturn:
-    """Setter-function for type """
-    self._clearTypes()
-    for arg in type_:
-      if isinstance(arg, type):
-        self._types.append(arg)
-
-  def _resetDefaultValue(self) -> NoReturn:
-    """Deleter-function for default value"""
-    self._defVal = None
-
-  def _setDefaultValue(self, dV: Any) -> NoReturn:
-    """Setter-function for the default value"""
-    self._defVal = dV
-
-  def _getDefaultValue(self) -> Any:
-    """Getter-function for the default value"""
-    return self._defVal
-
-  def _validateByType(self, arg: Any) -> Any:
-    """Returns the argument if it matches instance type. If instance type
-    is None, any argument is returned."""
-    if arg is None:
-      return None
-    if not self._types:
-      return arg
-    for type_ in self._types:
-      if isinstance(arg, type_):
-        return arg
-    return None
-
-  def _invoke(self, **kwargs) -> Any:
-    """Invokes the function"""
-    for key in self._keys:
-      val = self._validateByType(kwargs.get(key, None))
-      if val is not None:
-        return val
-      val = self._validateByType(kwargs.get(key.lower(), None))
-      if val is not None:
-        return val
-    return self._getDefaultValue()
-
-  def __matmul__(self, other: tuple[type, ...] | type) -> _SearchKeys:
-    """Sets the types for this instance"""
-    if isinstance(other, type):
-      self._setType(other)
-      return self
-    self._setType(*other)
-    return self
-
-  def __rshift__(self, other: tuple[dict, Any] | dict) -> Any:
-    """Evaluates the keyword arguments given. If a tuple is given,
-    the first member of it are assumed to be the keyword argument
-    dictionary and the second member is the default value. If a dict is
-    given, no default value can be given, and the dict is processed
-    directly."""
-    self._resetDefaultValue()
-    if isinstance(other, tuple):
-      kwargs = other[0]
-      if len(other) > 1:
-        self._setDefaultValue(other[1])
-      return self._invoke(**kwargs)
-    return self._invoke(**other)
-
-
-searchKeys = _SearchKeys.searchKeys
+"""The searchKeys function provides a flexible way of extracting values
+from keyword arguments."""
+#  MIT License
+#  Copyright (c) 2023 Asger Jon Vistisen
+from __future__ import annotations
+
+from typing import Any, NoReturn
+
+
+class _SearchKeys:
+  """The searchKeys function provides a flexible way of extracting values
+  from keyword arguments.
+  #  MIT License
+  #  Copyright (c) 2023 Asger Jon Vistisen"""
+
+  @classmethod
+  def searchKeys(cls, *keys: str) -> _SearchKeys:
+    """Creates a new instance on the given keys"""
+    out = cls()
+    out._setKeys(*keys)
+    return out
+
+  def __init__(self, ) -> None:
+    self._keys = []
+    self._types = []
+    self._defVal = None
+
+  def _clearKeys(self) -> NoReturn:
+    """Deleter-function for the instance keys"""
+    while self._keys:
+      self._keys.pop()
+
+  def _setKeys(self, *keys: str) -> NoReturn:
+    """Setter-function for the instance keys"""
+    self._clearKeys()
+    for key in keys:
+      if isinstance(key, str):
+        self._keys.append(key)
+
+  def _clearTypes(self) -> NoReturn:
+    """Clears the type list"""
+    while self._types:
+      self._types.pop()
+
+  def _setType(self, *type_: type) -> NoReturn:
+    """Setter-function for type """
+    self._clearTypes()
+    for arg in type_:
+      if isinstance(arg, type):
+        self._types.append(arg)
+
+  def _resetDefaultValue(self) -> NoReturn:
+    """Deleter-function for default value"""
+    self._defVal = None
+
+  def _setDefaultValue(self, dV: Any) -> NoReturn:
+    """Setter-function for the default value"""
+    self._defVal = dV
+
+  def _getDefaultValue(self) -> Any:
+    """Getter-function for the default value"""
+    return self._defVal
+
+  def _validateByType(self, arg: Any) -> Any:
+    """Returns the argument if it matches instance type. If instance type
+    is None, any argument is returned."""
+    if arg is None:
+      return None
+    if not self._types:
+      return arg
+    for type_ in self._types:
+      if isinstance(arg, type_):
+        return arg
+    return None
+
+  def _invoke(self, **kwargs) -> Any:
+    """Invokes the function"""
+    for key in self._keys:
+      val = self._validateByType(kwargs.get(key, None))
+      if val is not None:
+        return val
+      val = self._validateByType(kwargs.get(key.lower(), None))
+      if val is not None:
+        return val
+    return self._getDefaultValue()
+
+  def __matmul__(self, other: tuple[type, ...] | type) -> _SearchKeys:
+    """Sets the types for this instance"""
+    if isinstance(other, type):
+      self._setType(other)
+      return self
+    self._setType(*other)
+    return self
+
+  def __rshift__(self, other: tuple[dict, Any] | dict) -> Any:
+    """Evaluates the keyword arguments given. If a tuple is given,
+    the first member of it are assumed to be the keyword argument
+    dictionary and the second member is the default value. If a dict is
+    given, no default value can be given, and the dict is processed
+    directly."""
+    self._resetDefaultValue()
+    if isinstance(other, tuple):
+      kwargs = other[0]
+      if len(other) > 1:
+        self._setDefaultValue(other[1])
+      return self._invoke(**kwargs)
+    return self._invoke(**other)
+
+
+searchKeys = _SearchKeys.searchKeys
```

### Comparing `worktoy-0.25/src/worktoy/_stringlist.py` & `worktoy-0.28/src/worktoy/_stringlist.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-"""The stringList function provides an easier way to write lists of
-strings. Instead of wrapping each item in ticks, write on long string with
-consistent separators, and stringList will convert it to a list of
-strings.
-Instead of: numbers = ['one', 'two', 'three', 'four']
-Use stringList: numbers = stringList('one, two, three, four')"""
-#  MIT License
-#  Copyright (c) 2023 Asger Jon Vistisen
-from __future__ import annotations
-
-from worktoy import searchKeys, maybeTypes, maybe
-from worktoy.mockdata import strFactory
-
-
-def stringList(*args, **kwargs) -> list[str]:
-  """The stringList function provides an easier way to write lists of
-  strings. Instead of wrapping each item in ticks, write on long string with
-  consistent separators, and stringList will convert it to a list of
-  strings.
-  Instead of: numbers = ['one', 'two', 'three', 'four']
-  Use stringList: numbers = stringList('one, two, three, four')
-  Please note that all white space around each separator will be removed.
-  Meaning that ', ' and ',' will produce the same outcome when used as
-  separators on the same text.
-  #  MIT License
-  #  Copyright (c) 2023 Asger Jon Vistisen"""
-
-  strArgs = maybeTypes(str, *args, padLen=3, padChar=None)
-  sourceKwarg = searchKeys('source', 'src', 'txt') @ str >> kwargs
-  separatorKwarg = searchKeys('separator', 'splitHere') @ str >> kwargs
-  ignoreKwarg = searchKeys('ignoreChar', 'ignore') @ str >> kwargs
-  sourceArg, separatorArg, ignoreArg = strArgs
-  sourceDefault, separatorDefault, ignoreDefault = None, ', ', '@'
-  source = maybe(sourceKwarg, sourceArg, sourceDefault)
-  separator = maybe(separatorKwarg, separatorArg, separatorDefault, )
-  # separator = separator.replace(' ', '')
-  ignore = maybe(ignoreKwarg, ignoreArg, ignoreDefault)
-  if source is None:
-    msg = 'stringList received no string!'
-    raise ValueError(msg)
-  # if ignore == 'LOL':
-  #   print(ignore)
-  ignoreSeparator = '%s%s' % (ignore, separator)
-  tempIgnore = '___%s___' % (strFactory(16))
-  source = source.replace(ignoreSeparator, tempIgnore)
-  # preSpace = ' %s' % separator
-  # postSpace = '%s ' % separator
-  # while preSpace in source:
-  #   source = source.replace(preSpace, separator)
-  # while postSpace in source:
-  #   source = source.replace(postSpace, separator)
-  out = source.split(separator)
-  return [word.replace(tempIgnore, separator) for word in out]
+"""The stringList function provides an easier way to write lists of
+strings. Instead of wrapping each item in ticks, write on long string with
+consistent separators, and stringList will convert it to a list of
+strings.
+Instead of: numbers = ['one', 'two', 'three', 'four']
+Use stringList: numbers = stringList('one, two, three, four')"""
+#  MIT License
+#  Copyright (c) 2023 Asger Jon Vistisen
+from __future__ import annotations
+
+from worktoy import searchKeys, maybeTypes, maybe
+from worktoy.mockdata import strFactory
+
+
+def stringList(*args, **kwargs) -> list[str]:
+  """The stringList function provides an easier way to write lists of
+  strings. Instead of wrapping each item in ticks, write on long string with
+  consistent separators, and stringList will convert it to a list of
+  strings.
+  Instead of: numbers = ['one', 'two', 'three', 'four']
+  Use stringList: numbers = stringList('one, two, three, four')
+  Please note that all white space around each separator will be removed.
+  Meaning that ', ' and ',' will produce the same outcome when used as
+  separators on the same text.
+  #  MIT License
+  #  Copyright (c) 2023 Asger Jon Vistisen"""
+
+  strArgs = maybeTypes(str, *args, padLen=3, padChar=None)
+  sourceKwarg = searchKeys('source', 'src', 'txt') @ str >> kwargs
+  separatorKwarg = searchKeys('separator', 'splitHere') @ str >> kwargs
+  ignoreKwarg = searchKeys('ignoreChar', 'ignore') @ str >> kwargs
+  sourceArg, separatorArg, ignoreArg = strArgs
+  sourceDefault, separatorDefault, ignoreDefault = None, ', ', '@'
+  source = maybe(sourceKwarg, sourceArg, sourceDefault)
+  separator = maybe(separatorKwarg, separatorArg, separatorDefault, )
+  # separator = separator.replace(' ', '')
+  ignore = maybe(ignoreKwarg, ignoreArg, ignoreDefault)
+  if source is None:
+    msg = 'stringList received no string!'
+    raise ValueError(msg)
+  # if ignore == 'LOL':
+  #   print(ignore)
+  ignoreSeparator = '%s%s' % (ignore, separator)
+  tempIgnore = '___%s___' % (strFactory(16))
+  source = source.replace(ignoreSeparator, tempIgnore)
+  # preSpace = ' %s' % separator
+  # postSpace = '%s ' % separator
+  # while preSpace in source:
+  #   source = source.replace(preSpace, separator)
+  # while postSpace in source:
+  #   source = source.replace(postSpace, separator)
+  out = source.split(separator)
+  return [word.replace(tempIgnore, separator) for word in out]
```

### Comparing `worktoy-0.25/src/worktoy/mockdata/_intfactory.py` & `worktoy-0.28/src/worktoy/mockdata/_intfactory.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-"""The intFactory generates random integers"""
-#  MIT License
-#  Copyright (c) 2023 Asger Jon Vistisen
-from __future__ import annotations
-
-from random import randint
-from typing import NoReturn
-
-from worktoy import maybeTypes, maybe
-
-
-class _IntFactory:
-  """The intFactory generates random integers
-  #  MIT License
-  #  Copyright (c) 2023 Asger Jon Vistisen"""
-
-  _singleTon = None
-  _numbers = []
-
-  @classmethod
-  def intFactory(cls, *args, **kwargs) -> _IntFactory:
-    """Integer factory function"""
-    if _IntFactory._singleTon is None:
-      _IntFactory._singleTon = cls(*args, **kwargs)
-      return _IntFactory.intFactory()
-    lower, upper = _IntFactory._parseLimits(*args, **kwargs)
-    _IntFactory._singleTon.setUpper(upper)
-    _IntFactory._singleTon.setLower(lower)
-    return _IntFactory._singleTon
-
-  @staticmethod
-  def _parseLimits(*args, **kwargs) -> tuple[int, int]:
-    """Parses the arguments to upper and lower limits"""
-    intArgs = maybeTypes(int, *args, padLen=2, padChar=None)
-    lowerKwarg = kwargs.get('lower', **kwargs)
-    upperKwarg = kwargs.get('upper', **kwargs)
-    lowerArg, upperArg = intArgs
-    lowerDefault, upperDefault = 0, 2 ** 16 - 1
-    _lower = maybe(lowerKwarg, lowerArg, lowerDefault)
-    _upper = maybe(upperKwarg, upperArg, upperDefault)
-    return (_lower, _upper)
-
-  @staticmethod
-  def gcd(a: int, b: int) -> int:
-    """Greatest common divisor"""
-    if max([a, b]) % min([a, b]):
-      return _IntFactory.gcd(min([a, b]), max([a, b]) % min(a, b))
-    else:
-      return min([a, b])
-
-  def __init__(self, *args, **kwargs) -> None:
-    self._lower, self._upper = self._parseLimits(*args, **kwargs)
-
-  def _getUpper(self) -> int:
-    """Getter-function for upper limit"""
-    return self._upper
-
-  def setUpper(self, upper: int) -> NoReturn:
-    """Setter-function for upper limit"""
-    self._upper = upper
-
-  def _getLower(self) -> int:
-    """Getter-function for lower limit"""
-    return self._lower
-
-  def setLower(self, lower: int) -> NoReturn:
-    """Setter-function for lower limit"""
-    self._lower = lower
-
-  def coPrimeTest(self, n: int = None) -> float:
-    """Collects n unique instances. """
-    n = maybe(n, 16)
-    while len(self._numbers) < n:
-      self.getNumber()
-    coPrime = 0
-    notCoPrime = 0
-    count = 0
-    for innerNumber in sorted(self._numbers):
-      for outerNumber in sorted(self._numbers):
-        if innerNumber < outerNumber:
-          count += 1
-          if self.gcd(innerNumber, outerNumber) == 1:
-            coPrime += 1
-          else:
-            notCoPrime += 1
-    return coPrime / max([count, 0])
-
-  def getNumber(self) -> int:
-    """Getter-function for number"""
-    number = randint(self._getLower(), self._getUpper())
-    self._numbers.append(number)
-    return number
-
-  def __rshift__(self, other: tuple | list) -> int:
-    """Returns a single new number in the given range"""
-    intArgs = maybeTypes(int, *other, padLen=2, padChar=None)
-    a, b = intArgs
-    a = maybe(a, self._getLower())
-    b = maybe(b, self._getUpper())
-    return randint(a, b)
-
-  def __len__(self, ) -> int:
-    """The length of the instance is taken to mean the length of the list
-    of numbers so far obtained."""
-    return len(self._numbers)
-
-  def __call__(self, *args, **kwargs) -> list[int]:
-    """Calling the instance returns a sample of sampleSize given as a
-    positional argument or at the keyword argument sampleSize."""
-
-
-_intFactory = _IntFactory.intFactory
+"""The intFactory generates random integers"""
+#  MIT License
+#  Copyright (c) 2023 Asger Jon Vistisen
+from __future__ import annotations
+
+from random import randint
+from typing import NoReturn
+
+from worktoy import maybeTypes, maybe
+
+
+class _IntFactory:
+  """The intFactory generates random integers
+  #  MIT License
+  #  Copyright (c) 2023 Asger Jon Vistisen"""
+
+  _singleTon = None
+  _numbers = []
+
+  @classmethod
+  def intFactory(cls, *args, **kwargs) -> _IntFactory:
+    """Integer factory function"""
+    if _IntFactory._singleTon is None:
+      _IntFactory._singleTon = cls(*args, **kwargs)
+      return _IntFactory.intFactory()
+    lower, upper = _IntFactory._parseLimits(*args, **kwargs)
+    _IntFactory._singleTon.setUpper(upper)
+    _IntFactory._singleTon.setLower(lower)
+    return _IntFactory._singleTon
+
+  @staticmethod
+  def _parseLimits(*args, **kwargs) -> tuple[int, int]:
+    """Parses the arguments to upper and lower limits"""
+    intArgs = maybeTypes(int, *args, padLen=2, padChar=None)
+    lowerKwarg = kwargs.get('lower', **kwargs)
+    upperKwarg = kwargs.get('upper', **kwargs)
+    lowerArg, upperArg = intArgs
+    lowerDefault, upperDefault = 0, 2 ** 16 - 1
+    _lower = maybe(lowerKwarg, lowerArg, lowerDefault)
+    _upper = maybe(upperKwarg, upperArg, upperDefault)
+    return (_lower, _upper)
+
+  @staticmethod
+  def gcd(a: int, b: int) -> int:
+    """Greatest common divisor"""
+    if max([a, b]) % min([a, b]):
+      return _IntFactory.gcd(min([a, b]), max([a, b]) % min(a, b))
+    else:
+      return min([a, b])
+
+  def __init__(self, *args, **kwargs) -> None:
+    self._lower, self._upper = self._parseLimits(*args, **kwargs)
+
+  def _getUpper(self) -> int:
+    """Getter-function for upper limit"""
+    return self._upper
+
+  def setUpper(self, upper: int) -> NoReturn:
+    """Setter-function for upper limit"""
+    self._upper = upper
+
+  def _getLower(self) -> int:
+    """Getter-function for lower limit"""
+    return self._lower
+
+  def setLower(self, lower: int) -> NoReturn:
+    """Setter-function for lower limit"""
+    self._lower = lower
+
+  def coPrimeTest(self, n: int = None) -> float:
+    """Collects n unique instances. """
+    n = maybe(n, 16)
+    while len(self._numbers) < n:
+      self.getNumber()
+    coPrime = 0
+    notCoPrime = 0
+    count = 0
+    for innerNumber in sorted(self._numbers):
+      for outerNumber in sorted(self._numbers):
+        if innerNumber < outerNumber:
+          count += 1
+          if self.gcd(innerNumber, outerNumber) == 1:
+            coPrime += 1
+          else:
+            notCoPrime += 1
+    return coPrime / max([count, 0])
+
+  def getNumber(self) -> int:
+    """Getter-function for number"""
+    number = randint(self._getLower(), self._getUpper())
+    self._numbers.append(number)
+    return number
+
+  def __rshift__(self, other: tuple | list) -> int:
+    """Returns a single new number in the given range"""
+    intArgs = maybeTypes(int, *other, padLen=2, padChar=None)
+    a, b = intArgs
+    a = maybe(a, self._getLower())
+    b = maybe(b, self._getUpper())
+    return randint(a, b)
+
+  def __len__(self, ) -> int:
+    """The length of the instance is taken to mean the length of the list
+    of numbers so far obtained."""
+    return len(self._numbers)
+
+  def __call__(self, *args, **kwargs) -> list[int]:
+    """Calling the instance returns a sample of sampleSize given as a
+    positional argument or at the keyword argument sampleSize."""
+
+
+_intFactory = _IntFactory.intFactory
```

### Comparing `worktoy-0.25/src/worktoy/mockdata/_strfactory.py` & `worktoy-0.28/src/worktoy/mockdata/_strfactory.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-"""The strFactory function creates random strings of arbitrary length"""
-#  MIT License
-#  Copyright (c) 2023 Asger Jon Vistisen
-from __future__ import annotations
-
-from random import choice
-import string
-
-from worktoy import maybe
-
-
-def strFactory(n: int = None, *skipChars, ) -> str:
-  """The strFactory function creates random strings of arbitrary length.
-  #  MIT License
-  #  Copyright (c) 2023 Asger Jon Vistisen"""
-  n = maybe(n, 16)
-  if not n:
-    return ''
-  if n < 0:
-    msg = 'Expected non-negative integer for length of str, but received:'
-    raise ValueError('%s %d!' % (msg, n))
-  rawBase = string.ascii_letters + string.digits
-  ignoreChars = []
-  for word in skipChars:
-    for char in word:
-      ignoreChars.append(char)
-  base = [char for char in rawBase if char not in ignoreChars]
-  out = []
-  while len(out) < n:
-    out.append(choice(base))
-  return ''.join(out)
+"""The strFactory function creates random strings of arbitrary length"""
+#  MIT License
+#  Copyright (c) 2023 Asger Jon Vistisen
+from __future__ import annotations
+
+from random import choice
+import string
+
+from worktoy import maybe
+
+
+def strFactory(n: int = None, *skipChars, ) -> str:
+  """The strFactory function creates random strings of arbitrary length.
+  #  MIT License
+  #  Copyright (c) 2023 Asger Jon Vistisen"""
+  n = maybe(n, 16)
+  if not n:
+    return ''
+  if n < 0:
+    msg = 'Expected non-negative integer for length of str, but received:'
+    raise ValueError('%s %d!' % (msg, n))
+  rawBase = string.ascii_letters + string.digits
+  ignoreChars = []
+  for word in skipChars:
+    for char in word:
+      ignoreChars.append(char)
+  base = [char for char in rawBase if char not in ignoreChars]
+  out = []
+  while len(out) < n:
+    out.append(choice(base))
+  return ''.join(out)
```

### Comparing `worktoy-0.25/src/worktoy.egg-info/PKG-INFO` & `worktoy-0.28/src/worktoy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,195 +1,195 @@
-Metadata-Version: 2.1
-Name: worktoy
-Version: 0.25
-Summary: Collection of Utilities
-Author-email: Asger Jon Vistisen <asgerjon2@gmail.com>
-Project-URL: Homepage, https://github.com/AsgerJon/WorkToy
-Project-URL: Bug Tracker, https://github.com/AsgerJon/WorkToy
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# WorkToy
-
-Collection of General Utilities
-
-## The None-aware 'maybe'
-
-In a programming language which shall rename nameless as well as typeless,
-the following syntax is available:
-
-    const func = (arg = null) => {
-        let val1 = arg || 1.0;
-        let val2 = arg ?? 1.0;
-        return [val1, val2]; }
-
-In the above code, the default argument is set to null (in this context
-null is treated the same as None in Python). The `??` operator is the
-null-coalescence operator, which is nearly the same as the `or` operator.  
-Consider the return value obtained from calling `func()`:
-
-    func()
-    >>> (2)  [1, 1]
-
-This makes sense, but what happens when we call the function on a falsy
-value other than null, such as 0:
-
-    func(0)
-    >>> (3)  [1, 0]
-
-The first value in the return value comes from using the pipes (the
-logical or operator), is not aware of the difference between null and
-other falsy values. The null-coalescence operator is able to tell the
-difference. The WorkToy module brings this to python along with several
-derived utility functions:
-
-### `maybe`
-
-In the below python code, we implement the same function using the maybe
-function from WorkToy:
-
-    def func(arg: Any = None) -> Any:
-        """Function using the maybe from the WorkToy module"""
-        val1 = arg or 1.0
-        val2 = maybe(arg, 1.0)
-        return [val1, val2]
-
-The implementation of maybe simply follows a common pattern:
-
-    def maybe(*args) -> Any:
-        """Implementation of maybe returns the first argument given that 
-        is different from None. If no such argument is found None is 
-        returned."""
-        for arg in args:
-            if arg is not None: 
-                return arg
-        return None
-
-Unlike the `??` operator, the `maybe` operator handles an arbitrary
-number of arguments.
-
-### `maybeType`
-
-The first of the derived functions finds the first argument of a
-particular type:
-
-    def maybeType(type_: type, *args) -> type_:
-        """Returns the first argument of given type"""
-
-### `maybeTypes`
-
-Adding an 's' returns every argument of given type. Further, it supports
-keyword arguments `pad: int` and `padChar: Any`. If `pad` is given it
-defines the length of the returned list padded with `padChar` or `None`
-by default. Setting `pad` will either pad or crop as necessary.
-
-### `searchKeys`
-
-A common way to handle optional keyword arguments is something like:
-
-    def func(*args, **kwargs) -> Any:
-        """Common function accepting arbitrary positional and keyword 
-        arguments."""
-        val = kwargs.get('key', defaultValue)
-        ...
-
-In the above code, the `get` function is used to look for a given key in
-the collection of keyword arguments along with a (optional) default value.
-Instead, `searchKeys` allows for multiple keys in order of priority:
-
-    def func(*args, **kwargs) -> Any:
-        """Common function accepting arbitrary positional and keyword 
-        arguments."""
-        dV = defaultValue
-        val = searchKeys('k1', 'k2', 'k3', **kwargs)
-        ...
-
-In addition, WorkToy provides the following syntactic pork-scratchings
-for the keto-aware programmer:
-
-    def func(*args, **kwargs) -> Any:
-        """Common function accepting arbitrary positional and keyword 
-        arguments."""
-        dV = defaultValue
-        val = searchKeys('k1', 'k2', 'k3') @ int >> (kwargs, dV)
-        ...
-
-The matrix multiplication operator `@` sets a type requirement and the
-right-shift operator `>>` invokes the search. The default value is then
-given as the second positional argument in the tuple. Please note that
-absense of `**`. This causes `kwargs` to be treated as a dictionary
-entirely contained at the first positional argument. If invoked without a
-default value, the parentheses may be omitted.
-
-### `CallMeMaybe`
-
-This abstract baseclass registers any callable object as an instance.
-This makes it stronger than the built-in `callable` and even the
-`Callable` from the `typing` package. If a custom class implements the
-`__call__` method, instances of this class may still not be recognized as
-callable by the mentioned methods.
-
-    class FilteredClass:
-        """A class requiring a callable filter before invoking some other 
-        function"""
-
-        def __init__(self, *args, **kwargs) -> None:
-            filterKwarg = searchKeys('filter') @ CallMeMaybe >> kwargs
-            filterArg = maybeType(CallMeMaybe, *args)
-            filterDefault = lambda *arg, **kwargs: (arg, kwargs)
-            self._filter = maybe(filterKwarg, filterArg, filterDefault)
-            self._func = someFunction
-        
-        def __call__(self, *args, **kwargs) -> Any:
-            """Invokes some underlying function subject to the filter"""
-            return self._func(self._filter(*args, **kwargs))
-
-Additionally, decorate functions with `CallMeMaybe` to explicitly flag
-functions as being instances of `CallMeMaybe`. As expected, instances of
-subclasses of `CallMeMaybe` are regarded as instances.
-
-## String Tools
-
-WorkToy also brings a number of convenient string related functions:
-
-### `stringList`
-
-Consider the following code:
-
-`numbers = ['one', 'two', 'three', 'four']`
-The above involve repeated use of `'`. On the Danish keyboard layout, the
-`'` key is located as indicated `jklæø'`, meaning that the right pinky
-finger must leap over two other keys. Instead, use `stringList`:
-
-    numbers = stringList('one, two, three, four', )
-    >>> ['one', 'two', 'three', 'four']
-
-### `monoSpace`
-
-Consider the following code:
-
-    msg = """Hello there! I am writing a long string right here in python 
-    that stretches in length beyond the allowable line length. Thankfully,
-    we have the triple quotation mark syntax for indication of longer 
-    strings."""
-
-The above code takes things literally meaning that new lines are inserted.
-Thus, in between 'python' at the end of the first line and 'that' at the
-beginning of the second line, a `'\n'` has been inserted. Instead, use
-`monoSpace`:
-
-    msgLine = monoSpace(msg)  # msg as defined above
-
-Now `msgLine` contains now new lines and no repeated spaces. To
-explicitly set a line break in the string, insert `'<br>'` in the text.
-Set a different string to denote a line break, give that string as the
-second argument.
-
-    rawLines = """This is the first line. <br>   Here is the second line. 
-    Don't worry about the extra spaces surrounding the tag, they are 
-    removed. """
-    
-    twoLines = monoSpace(rawLines)
+Metadata-Version: 2.1
+Name: worktoy
+Version: 0.28
+Summary: Collection of Utilities
+Author-email: Asger Jon Vistisen <asgerjon2@gmail.com>
+Project-URL: Homepage, https://github.com/AsgerJon/WorkToy
+Project-URL: Bug Tracker, https://github.com/AsgerJon/WorkToy
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# WorkToy
+
+Collection of General Utilities
+
+## The None-aware 'maybe'
+
+In a programming language which shall rename nameless as well as typeless,
+the following syntax is available:
+
+    const func = (arg = null) => {
+        let val1 = arg || 1.0;
+        let val2 = arg ?? 1.0;
+        return [val1, val2]; }
+
+In the above code, the default argument is set to null (in this context
+null is treated the same as None in Python). The `??` operator is the
+null-coalescence operator, which is nearly the same as the `or` operator.  
+Consider the return value obtained from calling `func()`:
+
+    func()
+    >>> (2)  [1, 1]
+
+This makes sense, but what happens when we call the function on a falsy
+value other than null, such as 0:
+
+    func(0)
+    >>> (3)  [1, 0]
+
+The first value in the return value comes from using the pipes (the
+logical or operator), is not aware of the difference between null and
+other falsy values. The null-coalescence operator is able to tell the
+difference. The WorkToy module brings this to python along with several
+derived utility functions:
+
+### `maybe`
+
+In the below python code, we implement the same function using the maybe
+function from WorkToy:
+
+    def func(arg: Any = None) -> Any:
+        """Function using the maybe from the WorkToy module"""
+        val1 = arg or 1.0
+        val2 = maybe(arg, 1.0)
+        return [val1, val2]
+
+The implementation of maybe simply follows a common pattern:
+
+    def maybe(*args) -> Any:
+        """Implementation of maybe returns the first argument given that 
+        is different from None. If no such argument is found None is 
+        returned."""
+        for arg in args:
+            if arg is not None: 
+                return arg
+        return None
+
+Unlike the `??` operator, the `maybe` operator handles an arbitrary
+number of arguments.
+
+### `maybeType`
+
+The first of the derived functions finds the first argument of a
+particular type:
+
+    def maybeType(type_: type, *args) -> type_:
+        """Returns the first argument of given type"""
+
+### `maybeTypes`
+
+Adding an 's' returns every argument of given type. Further, it supports
+keyword arguments `pad: int` and `padChar: Any`. If `pad` is given it
+defines the length of the returned list padded with `padChar` or `None`
+by default. Setting `pad` will either pad or crop as necessary.
+
+### `searchKeys`
+
+A common way to handle optional keyword arguments is something like:
+
+    def func(*args, **kwargs) -> Any:
+        """Common function accepting arbitrary positional and keyword 
+        arguments."""
+        val = kwargs.get('key', defaultValue)
+        ...
+
+In the above code, the `get` function is used to look for a given key in
+the collection of keyword arguments along with a (optional) default value.
+Instead, `searchKeys` allows for multiple keys in order of priority:
+
+    def func(*args, **kwargs) -> Any:
+        """Common function accepting arbitrary positional and keyword 
+        arguments."""
+        dV = defaultValue
+        val = searchKeys('k1', 'k2', 'k3', **kwargs)
+        ...
+
+In addition, WorkToy provides the following syntactic pork-scratchings
+for the keto-aware programmer:
+
+    def func(*args, **kwargs) -> Any:
+        """Common function accepting arbitrary positional and keyword 
+        arguments."""
+        dV = defaultValue
+        val = searchKeys('k1', 'k2', 'k3') @ int >> (kwargs, dV)
+        ...
+
+The matrix multiplication operator `@` sets a type requirement and the
+right-shift operator `>>` invokes the search. The default value is then
+given as the second positional argument in the tuple. Please note that
+absense of `**`. This causes `kwargs` to be treated as a dictionary
+entirely contained at the first positional argument. If invoked without a
+default value, the parentheses may be omitted.
+
+### `CallMeMaybe`
+
+This abstract baseclass registers any callable object as an instance.
+This makes it stronger than the built-in `callable` and even the
+`Callable` from the `typing` package. If a custom class implements the
+`__call__` method, instances of this class may still not be recognized as
+callable by the mentioned methods.
+
+    class FilteredClass:
+        """A class requiring a callable filter before invoking some other 
+        function"""
+
+        def __init__(self, *args, **kwargs) -> None:
+            filterKwarg = searchKeys('filter') @ CallMeMaybe >> kwargs
+            filterArg = maybeType(CallMeMaybe, *args)
+            filterDefault = lambda *arg, **kwargs: (arg, kwargs)
+            self._filter = maybe(filterKwarg, filterArg, filterDefault)
+            self._func = someFunction
+        
+        def __call__(self, *args, **kwargs) -> Any:
+            """Invokes some underlying function subject to the filter"""
+            return self._func(self._filter(*args, **kwargs))
+
+Additionally, decorate functions with `CallMeMaybe` to explicitly flag
+functions as being instances of `CallMeMaybe`. As expected, instances of
+subclasses of `CallMeMaybe` are regarded as instances.
+
+## String Tools
+
+WorkToy also brings a number of convenient string related functions:
+
+### `stringList`
+
+Consider the following code:
+
+`numbers = ['one', 'two', 'three', 'four']`
+The above involve repeated use of `'`. On the Danish keyboard layout, the
+`'` key is located as indicated `jklæø'`, meaning that the right pinky
+finger must leap over two other keys. Instead, use `stringList`:
+
+    numbers = stringList('one, two, three, four', )
+    >>> ['one', 'two', 'three', 'four']
+
+### `monoSpace`
+
+Consider the following code:
+
+    msg = """Hello there! I am writing a long string right here in python 
+    that stretches in length beyond the allowable line length. Thankfully,
+    we have the triple quotation mark syntax for indication of longer 
+    strings."""
+
+The above code takes things literally meaning that new lines are inserted.
+Thus, in between 'python' at the end of the first line and 'that' at the
+beginning of the second line, a `'\n'` has been inserted. Instead, use
+`monoSpace`:
+
+    msgLine = monoSpace(msg)  # msg as defined above
+
+Now `msgLine` contains now new lines and no repeated spaces. To
+explicitly set a line break in the string, insert `'<br>'` in the text.
+Set a different string to denote a line break, give that string as the
+second argument.
+
+    rawLines = """This is the first line. <br>   Here is the second line. 
+    Don't worry about the extra spaces surrounding the tag, they are 
+    removed. """
+    
+    twoLines = monoSpace(rawLines)
```

### Comparing `worktoy-0.25/src/worktoy.egg-info/SOURCES.txt` & `worktoy-0.28/src/worktoy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 src/worktoy.egg-info/PKG-INFO
 src/worktoy.egg-info/SOURCES.txt
 src/worktoy.egg-info/dependency_links.txt
 src/worktoy.egg-info/top_level.txt
 src/worktoy/mockdata/__init__.py
 src/worktoy/mockdata/_intfactory.py
 src/worktoy/mockdata/_strfactory.py
-tests/testSearchKeys.py
 tests/test__callmemaybe.py
 tests/test__intfactory.py
 tests/test__maybe.py
 tests/test__maybeType.py
 tests/test__maybeTypes.py
+tests/test__searchKeys.py
 tests/test__strfactory.py
 tests/test__stringlist.py
```

### Comparing `worktoy-0.25/tests/testSearchKeys.py` & `worktoy-0.28/tests/test__searchKeys.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,176 +1,187 @@
-"""Testing the searchKeys"""
-#  MIT License
-#  Copyright (c) 2023 Asger Jon Vistisen
-from __future__ import annotations
-
-from random import randint, sample, choice, random
-import string
-from typing import NoReturn, Callable, Any
-from unittest import TestCase
-
-from worktoy import searchKeys
-
-
-class TestSearchKeys(TestCase):
-  """Testing the searchKeys
-  #  MIT License
-  #  Copyright (c) 2023 Asger Jon Vistisen"""
-
-  @staticmethod
-  def newTuple(n: int = None) -> tuple:
-    """Creates single new tuple"""
-    n = randint(0, 8) if n is None else n
-    out = ()
-    while n:
-      out = (out,)
-      n -= 1
-    return out
-
-  @staticmethod
-  def newFloat(a: float = None, b: float = None) -> float:
-    """Creates single new float"""
-    if a is None:
-      a, b = 0., 1.
-    if b is None:
-      b = 0.
-    a, b = float(min([a, b])), float(max([a, b]))
-    return random() * (b - a) + a
-
-  @staticmethod
-  def newInt(a: int = None, b: int = None) -> int:
-    """Creates single new integer"""
-    if a is None:
-      a, b = 0, 255
-    if b is None:
-      b = 0
-    a, b = min([a, b]), max([a, b])
-    return randint(a, b)
-
-  @staticmethod
-  def newKey() -> str:
-    """Creates a single new key"""
-    base = [char for char in string.ascii_letters + string.digits]
-    n = randint(4, 6)
-    return ''.join(sample(base, n))
-
-  @staticmethod
-  def getKeys(n: int = None) -> list[str]:
-    """Getter-function for random collection of goodKeys"""
-    n = 16 if n is None else n
-    out = []
-    while len(out) < n:
-      key = TestSearchKeys.newKey()
-      if key not in out:
-        out.append(key)
-    return out
-
-  @staticmethod
-  def getType(**kwargs) -> (Callable, type) | list[(Callable, type)]:
-    """Returns a random type"""
-    full = kwargs.get('full', False)
-    which = kwargs.get('index', None)
-    types = [
-      (str, TestSearchKeys.newKey),
-      (int, TestSearchKeys.newInt),
-      (float, TestSearchKeys.newFloat),
-      (tuple, TestSearchKeys.newTuple),
-    ]
-    if full:
-      return types
-    if which is not None:
-      if isinstance(which, int):
-        return types[which % len(types)]
-    return choice(types)
-
-  @staticmethod
-  def getRandomValues(n: int = None) -> tuple[list[type], list[Any]]:
-    """Getter-function for random values for use with dictionaries"""
-    n = 16 if n is None else n
-    types = []
-    values = []
-    while len(types) + len(values) < 2 * n:
-      t, f = TestSearchKeys.getType()
-      types.append(t)
-      values.append(f())
-    return (types, values)
-
-  def setUp(self) -> NoReturn:
-    """Setting up the tests"""
-    n = 16
-    self.goodKeys = self.getKeys(n)
-    self.badKeys = self.getKeys(n)
-    self.types, self.values = TestSearchKeys.getRandomValues(n)
-    self.typeDicts = {}
-    self.valueDicts = {}
-    for (key, (type_, val)) in zip(self.goodKeys,
-                                   zip(self.types, self.values)):
-      self.typeDicts |= {key: type_}
-      self.valueDicts |= {key: val}
-    self.defVal = {
-      tuple: self.newTuple(3),
-      int  : 69420,
-      float: .1337,
-      str  : 'lol',
-    }
-
-  def testSimpleKeys(self) -> NoReturn:
-    """Testing good keys. The simplest case"""
-    allKeys = self.goodKeys + self.badKeys
-    allKeys = [*allKeys, *[key.lower() for key in allKeys]]
-    for key in allKeys:
-      if key in self.goodKeys:
-        trueVal = self.valueDicts.get(key, None)
-        if trueVal is not None:
-          searchVal = searchKeys(key) >> self.valueDicts
-          self.assertEqual(trueVal, searchVal, )
-      if key in self.badKeys:
-        defSearch = searchKeys(key) >> (self.valueDicts, 'lol')
-        self.assertEqual(defSearch, 'lol')
-
-  def testTypeKeys(self) -> NoReturn:
-    """Testing good keys, but bad types"""
-    intVal = searchKeys(*self.goodKeys) @ int >> self.valueDicts
-    self.assertIsInstance(intVal, int)
-    tupleVal = searchKeys(*self.goodKeys) @ tuple >> self.valueDicts
-    self.assertIsInstance(tupleVal, tuple)
-    floatVal = searchKeys(*self.goodKeys) @ float >> self.valueDicts
-    self.assertIsInstance(floatVal, float)
-    strVal = searchKeys(*self.goodKeys) @ str >> self.valueDicts
-    self.assertIsInstance(strVal, str)
-
-  def testSingleTypeMultiKey(self) -> NoReturn:
-    """Testing good keys, but bad combinations of types"""
-    for k1 in self.goodKeys:
-      for k2 in [key for key in self.goodKeys if key != k1]:
-        for (type_, defVal) in self.defVal.items():
-          t1, t2 = [self.typeDicts.get(k, None) for k in [k1, k2]]
-          typeVal = searchKeys(k1, k2) @ type_ >> (self.valueDicts, defVal)
-          v1, v2 = [searchKeys(k) >> self.valueDicts for k in [k1, k2]]
-          if t1 is type_:
-            self.assertEqual(typeVal, v1)
-          elif t2 is type_:
-            self.assertEqual(typeVal, v2)
-          else:
-            self.assertEqual(typeVal, defVal)
-
-  def testMultiTypeMultiKey(self) -> NoReturn:
-    """Testing multiple keys and multiple types"""
-    for k1 in self.goodKeys:
-      keyType1 = self.typeDicts.get(k1, None)
-      keyVal1 = self.valueDicts.get(k1, None)
-      self.assertIsNotNone(keyType1)
-      self.assertIsNotNone(keyVal1)
-      for k2 in self.goodKeys:
-        keyType2 = self.typeDicts.get(k2, None)
-        keyVal2 = self.valueDicts.get(k2, None)
-        self.assertIsNotNone(keyType2)
-        self.assertIsNotNone(keyVal2)
-        for (t1, dV1) in self.defVal.items():
-          for (t2, dV2) in self.defVal.items():
-            val = searchKeys(k1, k2) @ (t1, t2) >> (self.valueDicts, dV1)
-            if keyType1 in (t1, t2):
-              self.assertEqual(keyVal1, val)
-            elif keyType2 in (t1, t2):
-              self.assertEqual(keyVal2, val)
-            else:
-              self.assertEqual(val, dV1)
+"""Testing the searchKeys"""
+#  MIT License
+#  Copyright (c) 2023 Asger Jon Vistisen
+from __future__ import annotations
+
+from random import randint, sample, choice, random
+import string
+from typing import NoReturn, Callable, Any
+from unittest import TestCase
+
+from worktoy import searchKeys, CallMeMaybe
+
+
+def _someFunc() -> NoReturn:
+  """Hi there, I'm a function!"""
+  return None
+
+
+class TestSearchKeys(TestCase):
+  """Testing the searchKeys
+  #  MIT License
+  #  Copyright (c) 2023 Asger Jon Vistisen"""
+
+  @staticmethod
+  def newTuple(n: int = None) -> tuple:
+    """Creates single new tuple"""
+    n = randint(0, 8) if n is None else n
+    out = ()
+    while n:
+      out = (out,)
+      n -= 1
+    return out
+
+  @staticmethod
+  def newFloat(a: float = None, b: float = None) -> float:
+    """Creates single new float"""
+    if a is None:
+      a, b = 0., 1.
+    if b is None:
+      b = 0.
+    a, b = float(min([a, b])), float(max([a, b]))
+    return random() * (b - a) + a
+
+  @staticmethod
+  def newInt(a: int = None, b: int = None) -> int:
+    """Creates single new integer"""
+    if a is None:
+      a, b = 0, 255
+    if b is None:
+      b = 0
+    a, b = min([a, b]), max([a, b])
+    return randint(a, b)
+
+  @staticmethod
+  def newKey() -> str:
+    """Creates a single new key"""
+    base = [char for char in string.ascii_letters + string.digits]
+    n = randint(4, 6)
+    return ''.join(sample(base, n))
+
+  @staticmethod
+  def getKeys(n: int = None) -> list[str]:
+    """Getter-function for random collection of goodKeys"""
+    n = 16 if n is None else n
+    out = []
+    while len(out) < n:
+      key = TestSearchKeys.newKey()
+      if key not in out:
+        out.append(key)
+    return out
+
+  @staticmethod
+  def getType(**kwargs) -> (Callable, type) | list[(Callable, type)]:
+    """Returns a random type"""
+    full = kwargs.get('full', False)
+    which = kwargs.get('index', None)
+    types = [
+      (str, TestSearchKeys.newKey),
+      (int, TestSearchKeys.newInt),
+      (float, TestSearchKeys.newFloat),
+      (tuple, TestSearchKeys.newTuple),
+    ]
+    if full:
+      return types
+    if which is not None:
+      if isinstance(which, int):
+        return types[which % len(types)]
+    return choice(types)
+
+  @staticmethod
+  def getRandomValues(n: int = None) -> tuple[list[type], list[Any]]:
+    """Getter-function for random values for use with dictionaries"""
+    n = 16 if n is None else n
+    types = []
+    values = []
+    while len(types) + len(values) < 2 * n:
+      t, f = TestSearchKeys.getType()
+      types.append(t)
+      values.append(f())
+    return (types, values)
+
+  def setUp(self) -> NoReturn:
+    """Setting up the tests"""
+    n = 16
+    self.goodKeys = self.getKeys(n)
+    self.badKeys = self.getKeys(n)
+    self.types, self.values = TestSearchKeys.getRandomValues(n)
+    self.typeDicts = {}
+    self.valueDicts = {}
+    for (key, (type_, val)) in zip(self.goodKeys,
+                                   zip(self.types, self.values)):
+      self.typeDicts |= {key: type_}
+      self.valueDicts |= {key: val}
+    self.defVal = {
+      tuple: self.newTuple(3),
+      int  : 69420,
+      float: .1337,
+      str  : 'lol',
+    }
+
+  def testCallMeMaybe(self) -> NoReturn:
+    """Testing if searchKeys can handle searching for callables"""
+    testKwarg = {'here': _someFunc, 'lol': 77777, 'blabla': 777777777}
+    res = searchKeys('here', 'there') @ CallMeMaybe >> testKwarg
+    self.assertEqual(res, _someFunc)
+
+  def testSimpleKeys(self) -> NoReturn:
+    """Testing good keys. The simplest case"""
+    allKeys = self.goodKeys + self.badKeys
+    allKeys = [*allKeys, *[key.lower() for key in allKeys]]
+    for key in allKeys:
+      if key in self.goodKeys:
+        trueVal = self.valueDicts.get(key, None)
+        if trueVal is not None:
+          searchVal = searchKeys(key) >> self.valueDicts
+          self.assertEqual(trueVal, searchVal, )
+      if key in self.badKeys:
+        defSearch = searchKeys(key) >> (self.valueDicts, 'lol')
+        self.assertEqual(defSearch, 'lol')
+
+  def testTypeKeys(self) -> NoReturn:
+    """Testing good keys, but bad types"""
+    intVal = searchKeys(*self.goodKeys) @ int >> self.valueDicts
+    self.assertIsInstance(intVal, int)
+    tupleVal = searchKeys(*self.goodKeys) @ tuple >> self.valueDicts
+    self.assertIsInstance(tupleVal, tuple)
+    floatVal = searchKeys(*self.goodKeys) @ float >> self.valueDicts
+    self.assertIsInstance(floatVal, float)
+    strVal = searchKeys(*self.goodKeys) @ str >> self.valueDicts
+    self.assertIsInstance(strVal, str)
+
+  def testSingleTypeMultiKey(self) -> NoReturn:
+    """Testing good keys, but bad combinations of types"""
+    for k1 in self.goodKeys:
+      for k2 in [key for key in self.goodKeys if key != k1]:
+        for (type_, defVal) in self.defVal.items():
+          t1, t2 = [self.typeDicts.get(k, None) for k in [k1, k2]]
+          typeVal = searchKeys(k1, k2) @ type_ >> (self.valueDicts, defVal)
+          v1, v2 = [searchKeys(k) >> self.valueDicts for k in [k1, k2]]
+          if t1 is type_:
+            self.assertEqual(typeVal, v1)
+          elif t2 is type_:
+            self.assertEqual(typeVal, v2)
+          else:
+            self.assertEqual(typeVal, defVal)
+
+  def testMultiTypeMultiKey(self) -> NoReturn:
+    """Testing multiple keys and multiple types"""
+    for k1 in self.goodKeys:
+      keyType1 = self.typeDicts.get(k1, None)
+      keyVal1 = self.valueDicts.get(k1, None)
+      self.assertIsNotNone(keyType1)
+      self.assertIsNotNone(keyVal1)
+      for k2 in self.goodKeys:
+        keyType2 = self.typeDicts.get(k2, None)
+        keyVal2 = self.valueDicts.get(k2, None)
+        self.assertIsNotNone(keyType2)
+        self.assertIsNotNone(keyVal2)
+        for (t1, dV1) in self.defVal.items():
+          for (t2, dV2) in self.defVal.items():
+            val = searchKeys(k1, k2) @ (t1, t2) >> (self.valueDicts, dV1)
+            if keyType1 in (t1, t2):
+              self.assertEqual(keyVal1, val)
+            elif keyType2 in (t1, t2):
+              self.assertEqual(keyVal2, val)
+            else:
+              self.assertEqual(val, dV1)
```

### Comparing `worktoy-0.25/tests/test__callmemaybe.py` & `worktoy-0.28/tests/test__callmemaybe.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-"""Testing CallMeMaybe"""
-#  MIT License
-#  Copyright (c) 2023 Asger Jon Vistisen
-from __future__ import annotations
-
-from math import sin
-from typing import NoReturn
-from unittest import TestCase
-
-from worktoy import CallMeMaybe
-
-
-def func() -> NoReturn:
-  """General function"""
-
-
-class WishInWell:
-  """Parent-class for sample class"""
-
-  def __init__(self, *__, **_) -> None:
-    self._name = None
-
-  def _getName(self) -> str:
-    """Getter-function for name"""
-    return self._name
-
-  def _setName(self, name: str) -> NoReturn:
-    """Setter-function for name"""
-    self._name = name
-    setattr(self, '__name__', name)
-
-  def _delName(self, *_) -> NoReturn:
-    """Illegal deleter-function"""
-    raise TypeError('Read only error!')
-
-  name = property(_getName, _setName, _delName)
-
-  def __str__(self) -> str:
-    """String representation"""
-    return self.name
-
-  def __repr__(self) -> str:
-    """Code representation"""
-    return '%s()' % getattr(self, '__name__', 'nameLess')
-
-
-class HereIsMyNumber(WishInWell):
-  """This is a callable class"""
-
-  def __init__(self, *args, **kwargs) -> None:
-    WishInWell.__init__(self, *args, **kwargs)
-    WishInWell._setName(self, 'I\'m callable!')
-
-  def __call__(self, *args, **kwargs) -> NoReturn:
-    """Implementation of the call"""
-    print(self)
-
-
-class ThisIsCrazy(WishInWell):
-  """Not callable!"""
-
-  def __init__(self, *args, **kwargs) -> None:
-    WishInWell.__init__(self, *args, **kwargs)
-    WishInWell._setName(self, 'I\'m not callable!')
-
-
-@CallMeMaybe(callable=False)
-def inCognitoFunction() -> NoReturn:
-  """Callable function explicitly marked as unCallable"""
-
-
-@CallMeMaybe(callable=False)
-class InCognitoClass:
-  """Class implementing __call__, but explicitly set to not being
-  recognized by CallMeMaybe"""
-
-  def __call__(self, *args, **kwargs) -> NoReturn:
-    """f... da police!"""
-    return 'f... da police!'
-
-
-class TestCallMeMaybe(TestCase):
-  """Testing CallMeMaybe
-  #  MIT License
-  #  Copyright (c) 2023 Asger Jon Vistisen"""
-
-  def setUp(self) -> NoReturn:
-    """Sets up the tests"""
-    self.callMeMaybe = CallMeMaybe()
-    self.callable = HereIsMyNumber()
-    self.notCallable = ThisIsCrazy()
-    self.inCognitoClassInstance = InCognitoClass()
-    self.inCognitoFunction = inCognitoFunction
-
-  def testCallables(self) -> NoReturn:
-    """Testing the type name of print"""
-    callables = [print, func, sin, self.callable, ]
-    for item in callables:
-      self.assertTrue(self.callMeMaybe.recognizeInstance(item))
-
-  def testUnCallables(self) -> NoReturn:
-    """Testing objects that are not callable"""
-    for item in [7, 0.7, 1 + 1j, (((),), ()), [7, 7], ]:
-      self.assertFalse(self.callMeMaybe.recognizeInstance(item),
-                       getattr(item, '__name__', str(item)))
-
-    for item in [self.notCallable,
-                 self.inCognitoClassInstance,
-                 self.inCognitoFunction]:
-      self.assertFalse(self.callMeMaybe.recognizeInstance(item),
-                       getattr(item, '__name__', '%s' % item))
+"""Testing CallMeMaybe"""
+#  MIT License
+#  Copyright (c) 2023 Asger Jon Vistisen
+from __future__ import annotations
+
+from math import sin
+from typing import NoReturn
+from unittest import TestCase
+
+from worktoy import CallMeMaybe
+
+
+def func() -> NoReturn:
+  """General function"""
+
+
+class WishInWell:
+  """Parent-class for sample class"""
+
+  def __init__(self, *__, **_) -> None:
+    self._name = None
+
+  def _getName(self) -> str:
+    """Getter-function for name"""
+    return self._name
+
+  def _setName(self, name: str) -> NoReturn:
+    """Setter-function for name"""
+    self._name = name
+    setattr(self, '__name__', name)
+
+  def _delName(self, *_) -> NoReturn:
+    """Illegal deleter-function"""
+    raise TypeError('Read only error!')
+
+  name = property(_getName, _setName, _delName)
+
+  def __str__(self) -> str:
+    """String representation"""
+    return self.name
+
+  def __repr__(self) -> str:
+    """Code representation"""
+    return '%s()' % getattr(self, '__name__', 'nameLess')
+
+
+class HereIsMyNumber(WishInWell):
+  """This is a callable class"""
+
+  def __init__(self, *args, **kwargs) -> None:
+    WishInWell.__init__(self, *args, **kwargs)
+    WishInWell._setName(self, 'I\'m callable!')
+
+  def __call__(self, *args, **kwargs) -> NoReturn:
+    """Implementation of the call"""
+    print(self)
+
+
+class ThisIsCrazy(WishInWell):
+  """Not callable!"""
+
+  def __init__(self, *args, **kwargs) -> None:
+    WishInWell.__init__(self, *args, **kwargs)
+    WishInWell._setName(self, 'I\'m not callable!')
+
+
+@CallMeMaybe(callable=False)
+def inCognitoFunction() -> NoReturn:
+  """Callable function explicitly marked as unCallable"""
+
+
+@CallMeMaybe(callable=False)
+class InCognitoClass:
+  """Class implementing __call__, but explicitly set to not being
+  recognized by CallMeMaybe"""
+
+  def __call__(self, *args, **kwargs) -> NoReturn:
+    """f... da police!"""
+    return 'f... da police!'
+
+
+class TestCallMeMaybe(TestCase):
+  """Testing CallMeMaybe
+  #  MIT License
+  #  Copyright (c) 2023 Asger Jon Vistisen"""
+
+  def setUp(self) -> NoReturn:
+    """Sets up the tests"""
+    self.callMeMaybe = CallMeMaybe()
+    self.callable = HereIsMyNumber()
+    self.notCallable = ThisIsCrazy()
+    self.inCognitoClassInstance = InCognitoClass()
+    self.inCognitoFunction = inCognitoFunction
+
+  def testCallables(self) -> NoReturn:
+    """Testing the type name of print"""
+    callables = [print, func, sin, self.callable, ]
+    for item in callables:
+      self.assertTrue(self.callMeMaybe.recognizeInstance(item))
+
+  def testUnCallables(self) -> NoReturn:
+    """Testing objects that are not callable"""
+    for item in [7, 0.7, 1 + 1j, (((),), ()), [7, 7], ]:
+      self.assertFalse(self.callMeMaybe.recognizeInstance(item),
+                       getattr(item, '__name__', str(item)))
+
+    for item in [self.notCallable,
+                 self.inCognitoClassInstance,
+                 self.inCognitoFunction]:
+      self.assertFalse(self.callMeMaybe.recognizeInstance(item),
+                       getattr(item, '__name__', '%s' % item))
```

### Comparing `worktoy-0.25/tests/test__intfactory.py` & `worktoy-0.28/tests/test__intfactory.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-"""Testing the integer factory"""
-#  MIT License
-#  Copyright (c) 2023 Asger Jon Vistisen
-from __future__ import annotations
-
-from cmath import pi
-from typing import NoReturn
-from unittest import TestCase
-
-from worktoy.mockdata import intFactory
-
-
-class TestIntFactory(TestCase):
-  """Testing the integer factory"""
-
-  def setUp(self, ) -> NoReturn:
-    """Sets up the tests"""
-    self.factory = intFactory()
-
-  def testBasic(self) -> int:
-    """Tests for basic functionality"""
-    val = self.factory >> (2 ** 31, 2 ** 32 - 1)
-    self.assertLess(val, 2 ** 32 - 1)
-    self.assertGreaterEqual(val, 2 ** 31)
-
-  def testCoPrime(self) -> NoReturn:
-    """This test ensures that the integers returned are in fact randomly
-    distributed.
-    The probability that two stochastic variables of unbounded scale
-    and uniform distribution across the positive integers are co-prime,
-    that is, having greatest common divisor equal to 1, is equal to:
-      6 / pi**2.
-    This value is the value of the Riemann Zeta-function evaluated at 2"""
-    p = self.factory.coPrimeTest(100)
-    self.assertLess((p - 6 / pi / pi) ** 2, 0.05)
+"""Testing the integer factory"""
+#  MIT License
+#  Copyright (c) 2023 Asger Jon Vistisen
+from __future__ import annotations
+
+from cmath import pi
+from typing import NoReturn
+from unittest import TestCase
+
+from worktoy.mockdata import intFactory
+
+
+class TestIntFactory(TestCase):
+  """Testing the integer factory"""
+
+  def setUp(self, ) -> NoReturn:
+    """Sets up the tests"""
+    self.factory = intFactory()
+
+  def testBasic(self) -> int:
+    """Tests for basic functionality"""
+    val = self.factory >> (2 ** 31, 2 ** 32 - 1)
+    self.assertLess(val, 2 ** 32 - 1)
+    self.assertGreaterEqual(val, 2 ** 31)
+
+  def testCoPrime(self) -> NoReturn:
+    """This test ensures that the integers returned are in fact randomly
+    distributed.
+    The probability that two stochastic variables of unbounded scale
+    and uniform distribution across the positive integers are co-prime,
+    that is, having greatest common divisor equal to 1, is equal to:
+      6 / pi**2.
+    This value is the value of the Riemann Zeta-function evaluated at 2"""
+    p = self.factory.coPrimeTest(100)
+    self.assertLess((p - 6 / pi / pi) ** 2, 0.05)
```

### Comparing `worktoy-0.25/tests/test__maybe.py` & `worktoy-0.28/tests/test__maybe.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-"""Testing the maybe function"""
-#  MIT License
-#  Copyright (c) 2023 Asger Jon Vistisen
-from __future__ import annotations
-
-from typing import NoReturn
-import unittest
-
-from worktoy import maybe
-
-
-class TestMaybe(unittest.TestCase):
-  def testMaybeReturnsNoneIfAllArgsAreNone(self) -> NoReturn:
-    """Test that the maybe function returns None if all input arguments
-    are None."""
-
-    self.assertIsNone(maybe(None, None, None))
-
-  def testMaybeReturnsFirstArgNotNone(self) -> NoReturn:
-    """Test that the maybe function returns the first non-None argument."""
-
-    self.assertEqual(maybe(None, "foo", "bar"), "foo")
-    self.assertEqual(maybe(None, None, "baz", None), "baz")
-    self.assertEqual(maybe(0, 1, None), 0)
+"""Testing the maybe function"""
+#  MIT License
+#  Copyright (c) 2023 Asger Jon Vistisen
+from __future__ import annotations
+
+from typing import NoReturn
+import unittest
+
+from worktoy import maybe
+
+
+class TestMaybe(unittest.TestCase):
+  def testMaybeReturnsNoneIfAllArgsAreNone(self) -> NoReturn:
+    """Test that the maybe function returns None if all input arguments
+    are None."""
+
+    self.assertIsNone(maybe(None, None, None))
+
+  def testMaybeReturnsFirstArgNotNone(self) -> NoReturn:
+    """Test that the maybe function returns the first non-None argument."""
+
+    self.assertEqual(maybe(None, "foo", "bar"), "foo")
+    self.assertEqual(maybe(None, None, "baz", None), "baz")
+    self.assertEqual(maybe(0, 1, None), 0)
```

### Comparing `worktoy-0.25/tests/test__maybeType.py` & `worktoy-0.28/tests/test__maybeType.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-"""Testing the maybeType"""
-#  MIT License
-#  Copyright (c) 2023 Asger Jon Vistisen
-from __future__ import annotations
-
-from typing import NoReturn
-import unittest
-
-from worktoy import maybeType
-
-
-class TestMaybeType(unittest.TestCase):
-  """A class that defines the testcases to check the implementation of
-  `maybeType`."""
-
-  def test_maybeType_correct_type(self) -> NoReturn:
-    """Test that the function returns the first argument of the specified
-    type when it exists."""
-    self.assertEqual(maybeType(int, 1, '2', None, 3), 1)
-    self.assertEqual(maybeType(str, None, 2, 'hello', {}, []), 'hello')
-
-  def test_maybeType_incorrect_type(self) -> NoReturn:
-    """Test that the function returns None when no argument of the
-    specified type is found."""
-    self.assertEqual(maybeType(float, 1, 2.0, '', None), 2.0)
-    self.assertIsNone(maybeType(list, 1, '2', None, {}))
-    self.assertIsNone(maybeType(complex, 1, 2.0, '', None))
-
-  def test_maybeType_empty_args(self) -> NoReturn:
-    """Test that the function returns None when no arguments are given."""
-    self.assertIsNone(maybeType(str))
+"""Testing the maybeType"""
+#  MIT License
+#  Copyright (c) 2023 Asger Jon Vistisen
+from __future__ import annotations
+
+from typing import NoReturn
+import unittest
+
+from worktoy import maybeType
+
+
+class TestMaybeType(unittest.TestCase):
+  """A class that defines the testcases to check the implementation of
+  `maybeType`."""
+
+  def test_maybeType_correct_type(self) -> NoReturn:
+    """Test that the function returns the first argument of the specified
+    type when it exists."""
+    self.assertEqual(maybeType(int, 1, '2', None, 3), 1)
+    self.assertEqual(maybeType(str, None, 2, 'hello', {}, []), 'hello')
+
+  def test_maybeType_incorrect_type(self) -> NoReturn:
+    """Test that the function returns None when no argument of the
+    specified type is found."""
+    self.assertEqual(maybeType(float, 1, 2.0, '', None), 2.0)
+    self.assertIsNone(maybeType(list, 1, '2', None, {}))
+    self.assertIsNone(maybeType(complex, 1, 2.0, '', None))
+
+  def test_maybeType_empty_args(self) -> NoReturn:
+    """Test that the function returns None when no arguments are given."""
+    self.assertIsNone(maybeType(str))
```

### Comparing `worktoy-0.25/tests/test__maybeTypes.py` & `worktoy-0.28/tests/test__maybeTypes.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-#  MIT License
-#  Copyright (c) 2023 Asger Jon Vistisen
-from __future__ import annotations
-
-import unittest
-
-from worktoy import maybeTypes
-
-
-class TestMaybeTypes(unittest.TestCase):
-  """A class that defines the testcases to check the implementation of
-  `maybeTypes`."""
-
-  def testMaybeTypesCorrectType(self):
-    """Test that the function correctly returns a list of all arguments of
-    the specified type."""
-    self.assertEqual(maybeTypes(int, 1, '2', None, 3), [1, 3])
-    self.assertEqual(maybeTypes(str, None, 2, 'hello', {}, []), ['hello'])
-
-  def testMaybeTypesEmptyArgs(self):
-    """Test that the function returns an empty list when no arguments are
-    given."""
-    self.assertEqual(maybeTypes(int), [])
-
-  def testMaybeTypesPadLenNone(self):
-    """Test that the function returns the full list when padLen is None."""
-    self.assertEqual(maybeTypes(int, 1, 2, 3), [1, 2, 3])
-
-  def testMaybeTypesPadLenCorrectLength(self):
-    """Test that the function returns a list of correct length when padLen
-    is specified."""
-    self.assertEqual(maybeTypes(int, 1, '2', None, 3, padLen=3),
-                     [1, 3, None])
-
-  def testMaybeTypesPadLenShorterList(self):
-    """Test that the function returns the full list when padLen is less
-    than the number of elements in the list."""
-    self.assertEqual(maybeTypes(int, 1, 2, 3, 4, padLen=3), [1, 2, 3])
-
-  def testMaybeTypesPadChar(self):
-    """Test that the function pads the list correctly with the specified
-    padding character when padLen is greater than the number of elements
-    in the list."""
-    self.assertEqual(maybeTypes(int, 1, 2, padLen=4, padChar=0),
-                     [1, 2, 0, 0])
+#  MIT License
+#  Copyright (c) 2023 Asger Jon Vistisen
+from __future__ import annotations
+
+import unittest
+
+from worktoy import maybeTypes
+
+
+class TestMaybeTypes(unittest.TestCase):
+  """A class that defines the testcases to check the implementation of
+  `maybeTypes`."""
+
+  def testMaybeTypesCorrectType(self):
+    """Test that the function correctly returns a list of all arguments of
+    the specified type."""
+    self.assertEqual(maybeTypes(int, 1, '2', None, 3), [1, 3])
+    self.assertEqual(maybeTypes(str, None, 2, 'hello', {}, []), ['hello'])
+
+  def testMaybeTypesEmptyArgs(self):
+    """Test that the function returns an empty list when no arguments are
+    given."""
+    self.assertEqual(maybeTypes(int), [])
+
+  def testMaybeTypesPadLenNone(self):
+    """Test that the function returns the full list when padLen is None."""
+    self.assertEqual(maybeTypes(int, 1, 2, 3), [1, 2, 3])
+
+  def testMaybeTypesPadLenCorrectLength(self):
+    """Test that the function returns a list of correct length when padLen
+    is specified."""
+    self.assertEqual(maybeTypes(int, 1, '2', None, 3, padLen=3),
+                     [1, 3, None])
+
+  def testMaybeTypesPadLenShorterList(self):
+    """Test that the function returns the full list when padLen is less
+    than the number of elements in the list."""
+    self.assertEqual(maybeTypes(int, 1, 2, 3, 4, padLen=3), [1, 2, 3])
+
+  def testMaybeTypesPadChar(self):
+    """Test that the function pads the list correctly with the specified
+    padding character when padLen is greater than the number of elements
+    in the list."""
+    self.assertEqual(maybeTypes(int, 1, 2, padLen=4, padChar=0),
+                     [1, 2, 0, 0])
```

### Comparing `worktoy-0.25/tests/test__strfactory.py` & `worktoy-0.28/tests/test__strfactory.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-"""Testing the strFactory function"""
-#  MIT License
-#  Copyright (c) 2023 Asger Jon Vistisen
-from __future__ import annotations
-
-import string
-from typing import NoReturn
-from unittest import TestCase
-
-from worktoy.mockdata import strFactory
-
-
-class TestStrFactory(TestCase):
-  """Testing the strFactory function
-  #  MIT License
-  #  Copyright (c) 2023 Asger Jon Vistisen"""
-
-  @staticmethod
-  def getAllChars() -> list[str]:
-    """Getter-function for all chars"""
-    return [char for char in string.ascii_letters + string.digits]
-
-  @staticmethod
-  def getAllExcept(*char: str) -> list[str]:
-    """Getter-function for a list all characters except those given."""
-    allChars = TestStrFactory.getAllChars()
-    return [c for c in allChars if c not in [cc for cc in char]]
-
-  def testStrFactory(self, ) -> NoReturn:
-    """Testing the length of words"""
-    for i in range(24):
-      if not i:
-        self.assertFalse(strFactory(i))
-      else:
-        self.assertEqual(len(strFactory(i)), i)
-
-  def testException(self) -> NoReturn:
-    """Testing the exception raised by passing strFactory a negative
-    number"""
-    self.assertRaises(ValueError)
-
-  def testIgnoreChars(self) -> NoReturn:
-    """Testing that strFactory correctly ignores given characters. """
-    allChars = TestStrFactory.getAllChars()
-    for char in allChars:
-      ignoreChars = self.getAllExcept(char)
-      testSample = strFactory(8, ignoreChars)
-      for testChar in testSample:
-        self.assertEqual(char, testChar)
+"""Testing the strFactory function"""
+#  MIT License
+#  Copyright (c) 2023 Asger Jon Vistisen
+from __future__ import annotations
+
+import string
+from typing import NoReturn
+from unittest import TestCase
+
+from worktoy.mockdata import strFactory
+
+
+class TestStrFactory(TestCase):
+  """Testing the strFactory function
+  #  MIT License
+  #  Copyright (c) 2023 Asger Jon Vistisen"""
+
+  @staticmethod
+  def getAllChars() -> list[str]:
+    """Getter-function for all chars"""
+    return [char for char in string.ascii_letters + string.digits]
+
+  @staticmethod
+  def getAllExcept(*char: str) -> list[str]:
+    """Getter-function for a list all characters except those given."""
+    allChars = TestStrFactory.getAllChars()
+    return [c for c in allChars if c not in [cc for cc in char]]
+
+  def testStrFactory(self, ) -> NoReturn:
+    """Testing the length of words"""
+    for i in range(24):
+      if not i:
+        self.assertFalse(strFactory(i))
+      else:
+        self.assertEqual(len(strFactory(i)), i)
+
+  def testException(self) -> NoReturn:
+    """Testing the exception raised by passing strFactory a negative
+    number"""
+    self.assertRaises(ValueError)
+
+  def testIgnoreChars(self) -> NoReturn:
+    """Testing that strFactory correctly ignores given characters. """
+    allChars = TestStrFactory.getAllChars()
+    for char in allChars:
+      ignoreChars = self.getAllExcept(char)
+      testSample = strFactory(8, ignoreChars)
+      for testChar in testSample:
+        self.assertEqual(char, testChar)
```

### Comparing `worktoy-0.25/tests/test__stringlist.py` & `worktoy-0.28/tests/test__stringlist.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-"""Testing stringList function """
-#  MIT License
-#  Copyright (c) 2023 Asger Jon Vistisen
-from __future__ import annotations
-
-from typing import NoReturn
-from unittest import TestCase
-
-from loremify import lorem
-
-from worktoy import stringList
-
-
-class TestStringList(TestCase):
-  """Testing stringList function
-  #  MIT License
-  #  Copyright (c) 2023 Asger Jon Vistisen"""
-
-  def testBasics(self) -> NoReturn:
-    """Testing the basic functionalities"""
-    base = stringList('one, two, three, four')
-    self.assertEqual(base, ['one', 'two', 'three', 'four'])
-
-  def testIgnore(self) -> NoReturn:
-    """Testing the use of the ignore flags"""
-    base = stringList('one, two@, three, four')
-    self.assertEqual(base, ['one', 'two, three', 'four'])
-
-  def testIgnoreLorem(self) -> NoReturn:
-    """Testing the number of commas compared to length of resulting list."""
-    base = lorem()
-    baseList = stringList(base, )
-    self.assertEqual(base.count(','), len(baseList) - 1)
-
-  def testIgnoreSingle(self, ) -> NoReturn:
-    """Testing one character separator and ignores"""
-    base = stringList('One | Two | Three @| Seven Halves | Four', '|', '@')
-    self.assertEqual(base, ['One ', ' Two ', ' Three | Seven Halves ',
-                            ' Four', ])
-
-  def testIgnoreSingleIgnoreMultiSplit(self, ) -> NoReturn:
-    """Testing single character ignore flag with multi character separator"""
-    base = stringList('One | Two | Three@ | Seven Halves | Four', ' | ', '@')
-    self.assertEqual(base, ['One', 'Two', 'Three | Seven Halves', 'Four', ])
-
-  def testIgnoreMultiIgnoreSingleSplit(self, ) -> NoReturn:
-    """Testing multi character ignore flag with single character
-    separator."""
-    base = stringList('A<>1<>B<>2@<>C<>3', '<>', '@')
-    res = ['A', '1', 'B', '2<>C', '3']
-    self.assertEqual(base, res)
+"""Testing stringList function """
+#  MIT License
+#  Copyright (c) 2023 Asger Jon Vistisen
+from __future__ import annotations
+
+from typing import NoReturn
+from unittest import TestCase
+
+from loremify import lorem
+
+from worktoy import stringList
+
+
+class TestStringList(TestCase):
+  """Testing stringList function
+  #  MIT License
+  #  Copyright (c) 2023 Asger Jon Vistisen"""
+
+  def testBasics(self) -> NoReturn:
+    """Testing the basic functionalities"""
+    base = stringList('one, two, three, four')
+    self.assertEqual(base, ['one', 'two', 'three', 'four'])
+
+  def testIgnore(self) -> NoReturn:
+    """Testing the use of the ignore flags"""
+    base = stringList('one, two@, three, four')
+    self.assertEqual(base, ['one', 'two, three', 'four'])
+
+  def testIgnoreLorem(self) -> NoReturn:
+    """Testing the number of commas compared to length of resulting list."""
+    base = lorem()
+    baseList = stringList(base, )
+    self.assertEqual(base.count(','), len(baseList) - 1)
+
+  def testIgnoreSingle(self, ) -> NoReturn:
+    """Testing one character separator and ignores"""
+    base = stringList('One | Two | Three @| Seven Halves | Four', '|', '@')
+    self.assertEqual(base, ['One ', ' Two ', ' Three | Seven Halves ',
+                            ' Four', ])
+
+  def testIgnoreSingleIgnoreMultiSplit(self, ) -> NoReturn:
+    """Testing single character ignore flag with multi character separator"""
+    base = stringList('One | Two | Three@ | Seven Halves | Four', ' | ', '@')
+    self.assertEqual(base, ['One', 'Two', 'Three | Seven Halves', 'Four', ])
+
+  def testIgnoreMultiIgnoreSingleSplit(self, ) -> NoReturn:
+    """Testing multi character ignore flag with single character
+    separator."""
+    base = stringList('A<>1<>B<>2@<>C<>3', '<>', '@')
+    res = ['A', '1', 'B', '2<>C', '3']
+    self.assertEqual(base, res)
```

