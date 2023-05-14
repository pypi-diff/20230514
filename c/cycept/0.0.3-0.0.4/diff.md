# Comparing `tmp/cycept-0.0.3.tar.gz` & `tmp/cycept-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycept-0.0.3.tar", last modified: Sun Apr 16 18:27:27 2023, max compression
+gzip compressed data, was "cycept-0.0.4.tar", last modified: Wed Apr 19 12:37:35 2023, max compression
```

## Comparing `cycept-0.0.3.tar` & `cycept-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-04-16 18:27:27.419529 cycept-0.0.3/
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     1068 2023-04-01 21:39:01.000000 cycept-0.0.3/LICENSE
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     6196 2023-04-16 18:27:27.419529 cycept-0.0.3/PKG-INFO
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     4840 2023-04-16 18:25:44.000000 cycept-0.0.3/README.md
-drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-04-16 18:27:27.419529 cycept-0.0.3/cycept/
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)       84 2023-04-15 21:05:00.000000 cycept-0.0.3/cycept/__init__.py
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)    26554 2023-04-16 00:23:56.000000 cycept-0.0.3/cycept/call.py
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     4767 2023-04-16 17:37:25.000000 cycept-0.0.3/cycept/compile.py
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)    22931 2023-04-15 18:33:58.000000 cycept-0.0.3/cycept/core.py
-drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-04-16 18:27:27.419529 cycept-0.0.3/cycept/tests/
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)      998 2023-04-16 12:40:48.000000 cycept-0.0.3/cycept/tests/__init__.py
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)    11614 2023-04-15 22:47:01.000000 cycept-0.0.3/cycept/tests/test_cycept.py
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)    14083 2023-04-16 17:40:47.000000 cycept-0.0.3/cycept/tests/test_perf.py
-drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-04-16 18:27:27.419529 cycept-0.0.3/cycept.egg-info/
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     6196 2023-04-16 18:27:27.000000 cycept-0.0.3/cycept.egg-info/PKG-INFO
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)      327 2023-04-16 18:27:27.000000 cycept-0.0.3/cycept.egg-info/SOURCES.txt
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)        1 2023-04-16 18:27:27.000000 cycept-0.0.3/cycept.egg-info/dependency_links.txt
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)      185 2023-04-16 18:27:27.000000 cycept-0.0.3/cycept.egg-info/requires.txt
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)        7 2023-04-16 18:27:27.000000 cycept-0.0.3/cycept.egg-info/top_level.txt
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     1712 2023-04-16 18:26:29.000000 cycept-0.0.3/pyproject.toml
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)       38 2023-04-16 18:27:27.419529 cycept-0.0.3/setup.cfg
+drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-04-19 12:37:35.878347 cycept-0.0.4/
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     1068 2023-04-01 21:39:01.000000 cycept-0.0.4/LICENSE
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     6797 2023-04-19 12:37:35.878347 cycept-0.0.4/PKG-INFO
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     5401 2023-04-17 23:04:54.000000 cycept-0.0.4/README.md
+drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-04-19 12:37:35.878347 cycept-0.0.4/cycept/
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     2875 2023-04-18 11:56:30.000000 cycept-0.0.4/cycept/__init__.py
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)    29550 2023-04-18 20:38:42.000000 cycept-0.0.4/cycept/call.py
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     4600 2023-04-18 10:45:45.000000 cycept-0.0.4/cycept/compile.py
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)    23082 2023-04-18 10:03:41.000000 cycept-0.0.4/cycept/core.py
+drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-04-19 12:37:35.878347 cycept-0.0.4/cycept/tests/
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     1080 2023-04-18 10:01:25.000000 cycept-0.0.4/cycept/tests/__init__.py
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)    11614 2023-04-15 22:47:01.000000 cycept-0.0.4/cycept/tests/test_cycept.py
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)    16391 2023-04-19 12:34:46.000000 cycept-0.0.4/cycept/tests/test_perf.py
+drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-04-19 12:37:35.878347 cycept-0.0.4/cycept.egg-info/
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     6797 2023-04-19 12:37:35.000000 cycept-0.0.4/cycept.egg-info/PKG-INFO
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)      327 2023-04-19 12:37:35.000000 cycept-0.0.4/cycept.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)        1 2023-04-19 12:37:35.000000 cycept-0.0.4/cycept.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)      185 2023-04-19 12:37:35.000000 cycept-0.0.4/cycept.egg-info/requires.txt
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)        7 2023-04-19 12:37:35.000000 cycept-0.0.4/cycept.egg-info/top_level.txt
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     1747 2023-04-19 11:33:08.000000 cycept-0.0.4/pyproject.toml
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)       38 2023-04-19 12:37:35.878347 cycept-0.0.4/setup.cfg
```

### Comparing `cycept-0.0.3/LICENSE` & `cycept-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cycept-0.0.3/PKG-INFO` & `cycept-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycept
-Version: 0.0.3
+Version: 0.0.4
 Summary: Effortless just-in-time compilation of Python functions, powered by Cython
 Author-email: Jeppe Dakin <jeppe_dakin@hotmail.com>
 Project-URL: Download, https://pypi.python.org/pypi/cycept
 Project-URL: Changelog, https://github.com/jmd-dk/cycept/blob/main/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/jmd-dk/cycept/issues
 Project-URL: Source code, https://github.com/jmd-dk/cycept
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: C
+Classifier: Programming Language :: C++
 Classifier: Programming Language :: Cython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -48,14 +49,26 @@
 * On **macOS** you may install [Clang](https://clang.llvm.org/)
   (available through [Xcode](https://developer.apple.com/xcode/)).
 * On **Windows** you may install
   [MSVC](https://en.wikipedia.org/wiki/Microsoft_Visual_C%2B%2B)
   (available through
   [Microsoft C++ Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/)).
 
+If you are using [Anaconda](https://www.anaconda.com/) on Linux or macOS,
+you may also obtain a C compiler through
+`conda install -c conda-forge c-compiler`.
+
+Once installed you can check whether Cycept functions correctly using
+```bash
+python -c "import cycept; cycept.check()"
+```
+If it does not work due to missing `Python.h` and you are running Linux,
+make sure to install the Python development headers (Debian-like distros:
+`sudo apt install python3-dev` if you are using the system Python).
+
 
 ## Quick demo
 ```python
 """Comparison of Python function JITs
 
 Below we implement the sample function sum((a - b)**2) where a and b
 are both 2D NumPy arrays. The following strategies are implemented and
@@ -63,108 +76,109 @@
 * Pure Python (baseline)
 * NumPy
 * Cycept JIT
 * Cython JIT
 * Numba JIT
 """
 
-from time import time
+from time import perf_counter
 import numpy as np
 
-a = np.random.random((2_000, 3_000))
-b = np.random.random((2_000, 3_000))
+m, n = 2_000, 3_000
+a = np.random.random((m, n))
+b = np.random.random((m, n))
 
 # Pure Python
 def func(a, b):
     x = 0
     for i in range(a.shape[0]):
         for j in range(a.shape[1]):
             x += (a[i, j] - b[i, j])**2
     return x
-tic = time()
+tic = perf_counter()
 result = func(a, b)
-toc = time()
+toc = perf_counter()
 t_ref = toc - tic
-print(f'Pure python: {result:<18} in {t_ref:.3e} s')
+print(f'Python: {result:<18} in {t_ref:.3e} s')
 
 # NumPy
 def func_numpy(a, b):
-    return np.sum((a - b)**2)
-tic = time()
+    return ((a - b)**2).sum()
+tic = perf_counter()
 result = func_numpy(a, b)
-toc = time()
+toc = perf_counter()
 t = toc - tic
 print(f'NumPy:       {result:<18} in {t:.3e} s ({int(t_ref/t)}x)')
 
 # Cycept
 import cycept
 @cycept.jit
 def func_cycept(a, b):
     x = 0
     for i in range(a.shape[0]):
         for j in range(a.shape[1]):
             x += (a[i, j] - b[i, j])**2
     return x
 func_cycept(a[:1, :1], b[:1, :1])  # to compile
-tic = time()
+tic = perf_counter()
 result = func_cycept(a, b)
-toc = time()
+toc = perf_counter()
 t = toc - tic
 print(f'Cycept:      {result:<18} in {t:.3e} s ({int(t_ref/t)}x)')
 
 # Cython
 import cython
 @cython.compile
 def func_cython(a, b):
     x = 0
     for i in range(a.shape[0]):
         for j in range(a.shape[1]):
             x += (a[i, j] - b[i, j])**2
     return x
 func_cython(a[:1, :1], b[:1, :1])  # to compile
-tic = time()
+tic = perf_counter()
 result = func_cython(a, b)
-toc = time()
+toc = perf_counter()
 t = toc - tic
 print(f'Cython:      {result:<18} in {t:.3e} s ({int(t_ref/t)}x)')
 
 # Numba
 import numba
-@numba.jit
+@numba.njit
 def func_numba(a, b):
     x = 0
     for i in range(a.shape[0]):
         for j in range(a.shape[1]):
             x += (a[i, j] - b[i, j])**2
     return x
 func_numba(a[:1, :1], b[:1, :1])  # to compile
-tic = time()
+tic = perf_counter()
 result = func_numba(a, b)
-toc = time()
+toc = perf_counter()
 t = toc - tic
 print(f'Numba:       {result:<18} in {t:.3e} s ({int(t_ref/t)}x)')
 ```
 
 Running the above results in something similar to
 ```
-Pure python: 1000265.9355757801 in 2.316e+00 s
-NumPy:       1000265.9355757139 in 2.967e-02 s (78x)
-Cycept:      1000265.9355757138 in 6.429e-03 s (360x)
-Cython:      1000265.9355757801 in 7.103e-02 s (32x)
-Numba:       1000265.9355757801 in 7.376e-03 s (314x)
+Python: 1000265.9355757801 in 2.316e+00 s
+NumPy:  1000265.9355757139 in 2.967e-02 s (78x)
+Cycept: 1000265.9355757138 in 6.429e-03 s (360x)
+Cython: 1000265.9355757801 in 7.103e-02 s (32x)
+Numba:  1000265.9355757801 in 7.376e-03 s (314x)
 ```
 For scientific codebases in the wild, code of the NumPy style is the
 most widespread. However, writing out the loops while adding a JIT can
 often lead to dramatic performance improvements, even when compared
 to NumPy. A further benefit of this is a reduced memory footprint,
 as no temporary arrays are created behind the scenes by the computation.
 
 See the help info on `cycept.jit` for optional arguments:
 ```bash
-python -c 'import cycept; help(cycept.jit)'
+python -c "import cycept; help(cycept.jit)"
 ```
 
 
 ## Tests
 The code contains a unit test suite which may be run as
 ```bash
 python -c "import cycept; cycept.test('cycept')"
@@ -185,11 +199,11 @@
 'Cycept' is an amalgamation of '[Cython](https://cython.org/)' and
 '[CO*N*CEPT](https://github.com/jmd-dk/concept)', the latter of which is a
 cosmological simulation code that makes heavy use of code transformation,
 both custom and through Cython. As the author of both projects, Cycept is my
 attempt to extract some of the code transformation ideas buried within
 CO*N*CEPT, making them available within an easy-to-use library.
 Though no code is shared between the projects, in many respects Cycept
-can be considered a spiritual descendant of CO*N*CEPT.
+can be considered a spiritual successor to CO*N*CEPT.
 Furthermore, 'Cy*cept*' has a nice in*cept*ion ring to it,
 which seems fitting for a piece of code that generates code.
```

### Comparing `cycept-0.0.3/README.md` & `cycept-0.0.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -18,14 +18,26 @@
 * On **macOS** you may install [Clang](https://clang.llvm.org/)
   (available through [Xcode](https://developer.apple.com/xcode/)).
 * On **Windows** you may install
   [MSVC](https://en.wikipedia.org/wiki/Microsoft_Visual_C%2B%2B)
   (available through
   [Microsoft C++ Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/)).
 
+If you are using [Anaconda](https://www.anaconda.com/) on Linux or macOS,
+you may also obtain a C compiler through
+`conda install -c conda-forge c-compiler`.
+
+Once installed you can check whether Cycept functions correctly using
+```bash
+python -c "import cycept; cycept.check()"
+```
+If it does not work due to missing `Python.h` and you are running Linux,
+make sure to install the Python development headers (Debian-like distros:
+`sudo apt install python3-dev` if you are using the system Python).
+
 
 ## Quick demo
 ```python
 """Comparison of Python function JITs
 
 Below we implement the sample function sum((a - b)**2) where a and b
 are both 2D NumPy arrays. The following strategies are implemented and
@@ -33,108 +45,109 @@
 * Pure Python (baseline)
 * NumPy
 * Cycept JIT
 * Cython JIT
 * Numba JIT
 """
 
-from time import time
+from time import perf_counter
 import numpy as np
 
-a = np.random.random((2_000, 3_000))
-b = np.random.random((2_000, 3_000))
+m, n = 2_000, 3_000
+a = np.random.random((m, n))
+b = np.random.random((m, n))
 
 # Pure Python
 def func(a, b):
     x = 0
     for i in range(a.shape[0]):
         for j in range(a.shape[1]):
             x += (a[i, j] - b[i, j])**2
     return x
-tic = time()
+tic = perf_counter()
 result = func(a, b)
-toc = time()
+toc = perf_counter()
 t_ref = toc - tic
-print(f'Pure python: {result:<18} in {t_ref:.3e} s')
+print(f'Python: {result:<18} in {t_ref:.3e} s')
 
 # NumPy
 def func_numpy(a, b):
-    return np.sum((a - b)**2)
-tic = time()
+    return ((a - b)**2).sum()
+tic = perf_counter()
 result = func_numpy(a, b)
-toc = time()
+toc = perf_counter()
 t = toc - tic
 print(f'NumPy:       {result:<18} in {t:.3e} s ({int(t_ref/t)}x)')
 
 # Cycept
 import cycept
 @cycept.jit
 def func_cycept(a, b):
     x = 0
     for i in range(a.shape[0]):
         for j in range(a.shape[1]):
             x += (a[i, j] - b[i, j])**2
     return x
 func_cycept(a[:1, :1], b[:1, :1])  # to compile
-tic = time()
+tic = perf_counter()
 result = func_cycept(a, b)
-toc = time()
+toc = perf_counter()
 t = toc - tic
 print(f'Cycept:      {result:<18} in {t:.3e} s ({int(t_ref/t)}x)')
 
 # Cython
 import cython
 @cython.compile
 def func_cython(a, b):
     x = 0
     for i in range(a.shape[0]):
         for j in range(a.shape[1]):
             x += (a[i, j] - b[i, j])**2
     return x
 func_cython(a[:1, :1], b[:1, :1])  # to compile
-tic = time()
+tic = perf_counter()
 result = func_cython(a, b)
-toc = time()
+toc = perf_counter()
 t = toc - tic
 print(f'Cython:      {result:<18} in {t:.3e} s ({int(t_ref/t)}x)')
 
 # Numba
 import numba
-@numba.jit
+@numba.njit
 def func_numba(a, b):
     x = 0
     for i in range(a.shape[0]):
         for j in range(a.shape[1]):
             x += (a[i, j] - b[i, j])**2
     return x
 func_numba(a[:1, :1], b[:1, :1])  # to compile
-tic = time()
+tic = perf_counter()
 result = func_numba(a, b)
-toc = time()
+toc = perf_counter()
 t = toc - tic
 print(f'Numba:       {result:<18} in {t:.3e} s ({int(t_ref/t)}x)')
 ```
 
 Running the above results in something similar to
 ```
-Pure python: 1000265.9355757801 in 2.316e+00 s
-NumPy:       1000265.9355757139 in 2.967e-02 s (78x)
-Cycept:      1000265.9355757138 in 6.429e-03 s (360x)
-Cython:      1000265.9355757801 in 7.103e-02 s (32x)
-Numba:       1000265.9355757801 in 7.376e-03 s (314x)
+Python: 1000265.9355757801 in 2.316e+00 s
+NumPy:  1000265.9355757139 in 2.967e-02 s (78x)
+Cycept: 1000265.9355757138 in 6.429e-03 s (360x)
+Cython: 1000265.9355757801 in 7.103e-02 s (32x)
+Numba:  1000265.9355757801 in 7.376e-03 s (314x)
 ```
 For scientific codebases in the wild, code of the NumPy style is the
 most widespread. However, writing out the loops while adding a JIT can
 often lead to dramatic performance improvements, even when compared
 to NumPy. A further benefit of this is a reduced memory footprint,
 as no temporary arrays are created behind the scenes by the computation.
 
 See the help info on `cycept.jit` for optional arguments:
 ```bash
-python -c 'import cycept; help(cycept.jit)'
+python -c "import cycept; help(cycept.jit)"
 ```
 
 
 ## Tests
 The code contains a unit test suite which may be run as
 ```bash
 python -c "import cycept; cycept.test('cycept')"
@@ -155,11 +168,11 @@
 'Cycept' is an amalgamation of '[Cython](https://cython.org/)' and
 '[CO*N*CEPT](https://github.com/jmd-dk/concept)', the latter of which is a
 cosmological simulation code that makes heavy use of code transformation,
 both custom and through Cython. As the author of both projects, Cycept is my
 attempt to extract some of the code transformation ideas buried within
 CO*N*CEPT, making them available within an easy-to-use library.
 Though no code is shared between the projects, in many respects Cycept
-can be considered a spiritual descendant of CO*N*CEPT.
+can be considered a spiritual successor to CO*N*CEPT.
 Furthermore, 'Cy*cept*' has a nice in*cept*ion ring to it,
 which seems fitting for a piece of code that generates code.
```

### Comparing `cycept-0.0.3/cycept/call.py` & `cycept-0.0.4/cycept/call.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,17 +25,18 @@
         source_ext: str
         html: str
 
     class Time(typing.NamedTuple):
         compile: float
         total: float
 
-    def __init__(self, func, args, kwargs):
+    def __init__(self, func, wrapper, args, kwargs):
         # Function and call arguments
         self.func = func
+        self.wrapper = wrapper
         self.args = args
         self.kwargs = kwargs
         # Properties to be lazily constructed
         self._func_name = None
         self._signature = None
         self._arguments = None
         self._arguments_types = None
@@ -97,15 +98,15 @@
         return self._arguments_types
 
     # Hash of the function call
     @property
     def hash(self):
         if self._hash is not None:
             return self._hash
-        self._hash = abs(hash((self.func, self.arguments_types)))
+        self._hash = abs(hash((self.func, self.wrapper, self.arguments_types)))
         return self._hash
 
     # Source code of the function
     @property
     def source(self):
         if self._source is not None:
             return self._source
@@ -340,63 +341,94 @@
         }
         names.discard('return')
         if not names:
             # No local arrays found
             return
         # Wrap local arrays
         class ArrayWrapper(ast.NodeTransformer):
+            class ArrayAttribute(typing.NamedTuple):
+                name: str
+                is_scalar: bool = False
+                is_sequence: bool = False
+            array_attributes = {
+                'shape': ArrayAttribute('shape', is_sequence=True),
+                'strides': ArrayAttribute('strides', is_sequence=True),
+                'ndim': ArrayAttribute('ndim', is_scalar=True),
+                'size': ArrayAttribute('size', is_scalar=True),
+                'itemsize': ArrayAttribute('itemsize', is_scalar=True),
+                'nbytes': ArrayAttribute('nbytes', is_scalar=True),
+            }
             def __init__(self, call, names, array_args, wrapper_func, tmp_name):
                 self.call = call
                 self.names = names
                 self.array_args = array_args
                 self.wrapper_func = wrapper_func
                 self.tmp_name = tmp_name
-                self.shape_attrs = set()
+                self.sequence_attrs = set()
                 self.wrapped_any = False
                 self.tmp_any = False
             def wrap(self):
-                self.shape_attrs.clear()
+                self.sequence_attrs.clear()
                 self.wrapped_any = False
                 self.tmp_any = False
                 return self.visit(self.call.ast)
             def wrap_node(self, node, kind=0):
-                def is_scalar(node):
-                    if isinstance(node, ast.Name):
-                        tp = self.call.types[node.id]
-                        if tp.startswith('cython.') and '[' not in tp:
-                            return True
-                    elif isinstance(node, ast.Constant):
-                        if isinstance(node.value, int):
-                            return True
-                    return False
                 nodes_subscript = []
                 while isinstance(node, ast.Subscript):
                     nodes_subscript.append(node)
                     node = node.value
                 if not isinstance(node, ast.Name) or node.id not in self.names:
                     return
                 if nodes_subscript:
                     # Memoryview/array indexing arr[x0][x1, x2][...].
                     # If we can prove that all x are scalars
                     # we use the memoryview as is.
                     for node_subscript in nodes_subscript:
                         if isinstance(node_subscript.slice, ast.Tuple):
-                            if not all(is_scalar(el) for el in node_subscript.slice.elts):
+                            if not all(self.is_scalar(el) for el in node_subscript.slice.elts):
                                 break
-                        elif not is_scalar(node_subscript.slice):
+                        elif not self.is_scalar(node_subscript.slice):
                             break
                     else:
                         return
                 # Wrap node
                 self.wrapped_any = True
                 if kind == 0:
                     node.id = f'{self.wrapper_func}({node.id})'
                 elif kind == 1:
                     self.tmp_any = True
                     node.id = f'{self.tmp_name} = {self.wrapper_func}({node.id}); {self.tmp_name}'
+            def is_scalar(self, node):
+                if isinstance(node, ast.Name):
+                    tp = self.call.types[node.id]
+                    return tp.startswith('cython.') and '[' not in tp
+                elif isinstance(node, ast.Constant):
+                    return isinstance(node.value, int)
+                elif isinstance(node, ast.UnaryOp):
+                    return self.is_scalar(node.operand)
+                elif isinstance(node, ast.BinOp):
+                    return self.is_scalar(node.left) and self.is_scalar(node.right)
+                elif isinstance(node, ast.Subscript):
+                    if isinstance(node.value, ast.Name):
+                        return node.value.id in self.names and self.is_scalar(node.slice)
+                    elif isinstance(node.value, ast.Attribute):
+                        return (
+                            node.value.value.id in self.names
+                            and (array_attribute := self.array_attributes.get(node.value.attr)) is not None
+                            and array_attribute.is_sequence
+                            and self.is_scalar(node.slice)
+                        )
+                elif isinstance(node, ast.Attribute):
+                    return (
+                        isinstance(node.value, ast.Name)
+                        and node.value.id in self.names
+                        and (array_attribute := self.array_attributes.get(node.attr)) is not None
+                        and array_attribute.is_scalar
+                    )
+                return False
             def visit_UnaryOp(self, node):
                 node = self.generic_visit(node)
                 self.wrap_node(node.operand)
                 return node
             def visit_BinOp(self, node):
                 node = self.generic_visit(node)
                 self.wrap_node(node.left)
@@ -417,34 +449,51 @@
             def visit_Call(self, node):
                 node = self.generic_visit(node)
                 if not self.array_args:
                     return node
                 for arg in node.args:
                     self.wrap_node(arg)
                 return node
-            # NumPy arrays and Cython memory views generally share the same
-            # attributes. One exception is 'shape', which for memoryviews
-            # is meant to be used as memoryview.shape[i]. If the 'shape'
-            # attribute is to be used without immediately indexing into it,
-            # use a NumPy array instead of a memoryview.
+            # Cython memoryviews and NumPy arrays share a subset of
+            # their attributes, as specified by array_attributes.
+            # Below, the visit_Attribute() method will check if an attribute
+            # lookup is a recognized memoryview attribute, in which case the
+            # lookup will not be wrapped. Otherwise it will. However, for the
+            # sequence attributes, e.g. 'shape', the value of the Cython
+            # memoryview attribute and the NumPy array attribute are not
+            # equivalent (they have different lengths in general). What is
+            # equivalent is the result of subsequent indexing into these
+            # sequences, e.g. .shape[i], with i an integer (scalar).
+            # The visit_Subscript() method below will find such subscript
+            # nodes and flag them, so that the visit_Attribute() method will
+            # know not to wrap these. Sequence attribute lookups that are not
+            # immediately indexed will not be flagged
+            # and will thus be wrapped.
             def visit_Subscript(self, node):
                 value = node.value
                 if (
                     isinstance(value, ast.Attribute)
                     and isinstance(value.value, ast.Name)
                     and value.value.id in self.names
-                    and value.attr == 'shape'
+                    and (array_attribute := self.array_attributes.get(value.attr)) is not None
+                    and array_attribute.is_sequence
+                    and self.is_scalar(node.slice)
                 ):
                     # Record usage of memoryview.shape[i]
-                    self.shape_attrs.add(value)
+                    self.sequence_attrs.add(value)
                 node = self.generic_visit(node)
                 return node
             def visit_Attribute(self, node):
                 node = self.generic_visit(node)
-                if node not in self.shape_attrs:
+                if (array_attribute := self.array_attributes.get(node.attr)) is None:
+                    # Not a memoryview attribute lookup
+                    self.wrap_node(node.value)
+                elif array_attribute.is_sequence and node not in self.sequence_attrs:
+                    # Memoryview attribute lookup of sequence
+                    # that is not immediately indexed by a scalar.
                     self.wrap_node(node.value)
                 return node
         wrapper_func = '_cycept_asarray_'
         tmp_name = '_cycept_tmp_'
         array_wrapper = ArrayWrapper(self, names, array_args, wrapper_func, tmp_name)
         self._source = ast.unparse(array_wrapper.wrap())
         self._ast = None  # invalidate AST (cannot use the above as expressions are used as names)
@@ -553,25 +602,26 @@
     def compile(self, optimizations, c_lang, html, silent):
         # Cythonize and compile extension module within temporary directory.
         # The compiled module is then imported (through hacking of sys.path)
         # before it is removed from disk.
         @contextlib.contextmanager
         def hack_sys_path():
             sys.path.append(dir_name)
-            yield
-            sys.path.remove(dir_name)
+            try:
+                yield
+            except Exception:
+                raise
+            finally:
+                sys.path.remove(dir_name)
         module_name = f'_cycept_module_{self.hash}'
         namespace = {}
         source_c = None
         html_annotation = None
-        tempfile_kwargs = {}
-        if sys.version_info >= (3, 10):
-            tempfile_kwargs |= {'ignore_cleanup_errors': True}
         with (
-            tempfile.TemporaryDirectory(**tempfile_kwargs) as dir_name,
+            tempfile.TemporaryDirectory(ignore_cleanup_errors=True) as dir_name,
             hack_sys_path(),
         ):
             # Write Cython source to file
             module_path = pathlib.Path(dir_name) / module_name
             module_path.with_suffix('.pyx').write_text(self.source, 'utf-8')
             # Call Cython. We do so within a subprocess in order
             # to capture stdout an stderr when running silently.
```

### Comparing `cycept-0.0.3/cycept/compile.py` & `cycept-0.0.4/cycept/compile.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,41 +6,34 @@
 import warnings
 
 import Cython.Build
 import Cython.Distutils
 import setuptools
 
 
-# Implement contextlib.chdir if missing
-if sys.version_info < (3, 11):
-    @contextlib.contextmanager
-    def _chdir(path):
-        old_cwd = os.getcwd()
-        os.chdir(path)
-        yield
-        os.chdir(old_cwd)
-    contextlib.chdir = _chdir
-
-
 # Method for handling Cythonization and C compilation
 def compile(module_path, optimizations, c_lang, html):
     module_path = pathlib.Path(module_path)
     optimization_options = OptimizationOptions(optimizations)
     macros = get_macros()
     # Context manager to redirect all logging to stdout
     @contextlib.contextmanager
     def print_logging():
         root = logging.getLogger()
         level = root.level
         root.setLevel(logging.DEBUG)
         handler = logging.StreamHandler(sys.stdout)
         handler.setLevel(logging.DEBUG)
         root.addHandler(handler)
-        yield
-        root.removeHandler(handler)
+        try:
+            yield
+        except Exception:
+            raise
+        finally:
+            root.removeHandler(handler)
     # Cythonize and compile extension module
     with (
         contextlib.chdir(module_path.parent),
         print_logging(),
     ):
         print(f'Changed working directory to {os.getcwd()}')
         extension_kwargs = {}
```

### Comparing `cycept-0.0.3/cycept/core.py` & `cycept-0.0.4/cycept/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,15 +268,15 @@
     floating=None,
     floating_complex=None,
 ):
     if not compile:
         return func, None
     # Fetch function call object, implementing dynamic evaluation
     # of various attributes.
-    call = fetch_function_call(func, args, kwargs)
+    call = fetch_function_call(func, wrapper, args, kwargs)
     # If the call has already been transpiled and cached,
     # return immediately.
     if call.compiled is not None:
         return call.compiled.func, None
     # The function call object was not found in cache
     tic = time.perf_counter()
     # Populate global mappings of Cython types in accordance
@@ -315,30 +315,31 @@
         print(f'Total jitting time: {call.time.total:#.4g} s')
     # Return the result only
     return None, result
 
 
 # Function used to fetch FunctionCall instance from the global
 # cache or instantiating a new one if not found in the cache.
-def fetch_function_call(func, args=None, kwargs=None):
+def fetch_function_call(func, wrapper=None, args=None, kwargs=None):
     if isinstance(func, int):
         # Called with function call hash
         return cache[func]
     # Fast lookup if called with the same objects as last time
     ids = (
         id(func),
+        id(wrapper),
         *(id(arg) for arg in args),
         *kwargs.keys(),
         *(id(kwarg) for kwarg in kwargs.values()),
     )
     loot = cache.get('last')
     if loot is not None and loot[1] == ids:
         return loot[0]
     # We need to instantiate a fresh instance to obtain the hash
-    call = FunctionCall(func, args, kwargs)
+    call = FunctionCall(func, wrapper, args, kwargs)
     call_cached = cache.get(call.hash)
     if call_cached is not None:
         # Found in cache. Disregard the freshly created instance.
         return call_cached
     # Not found in cache. Cache and return the freshly created instance.
     cache[call.hash] = call
     cache['last'] = call, ids  # special additional store
@@ -512,20 +513,24 @@
     def hack_module_dict():
         call.module_dict[cycept_module_refname] = sys.modules['cycept.core']
         nonlocals_ori = {}
         for name, val in call.nonlocals.items():
             if name in call.module_dict:
                 nonlocals_ori[name] = call.module_dict[name]
             call.module_dict[name] = val
-        yield
-        call.module_dict.pop(cycept_module_refname)
-        for name in call.nonlocals:
-            call.module_dict.pop(name)
-        for name, val in nonlocals_ori.items():
-            call.module_dict[name] = val
+        try:
+            yield
+        except Exception:
+            raise
+        finally:
+            call.module_dict.pop(cycept_module_refname)
+            for name in call.nonlocals:
+                call.module_dict.pop(name)
+            for name, val in nonlocals_ori.items():
+                call.module_dict[name] = val
     with hack_module_dict():
         # Define modified function within definition module
         exec(source, call.module_dict)
         # Call modified function with passed arguments
         return_val = call.module_dict[func_name_tmp](*call.args, **call.kwargs)
     # Remove modified function from definition module
     call.module_dict.pop(func_name_tmp)
```

### Comparing `cycept-0.0.3/cycept/tests/__init__.py` & `cycept-0.0.4/cycept/tests/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,13 +19,17 @@
     # We prevent pytest from writing to __pycache__ by hacking on
     # sys.dont_write_bytecode. We do this as such files are not cleanly
     # removed by 'pip uninstall cycept'.
     @contextlib.contextmanager
     def hack_sys_dont_write_bytecode():
         backup = sys.dont_write_bytecode
         sys.dont_write_bytecode = True
-        yield
-        sys.dont_write_bytecode = backup
+        try:
+            yield
+        except Exception:
+            raise
+        finally:
+            sys.dont_write_bytecode = backup
     with hack_sys_dont_write_bytecode():
         import pytest
         pytest.main(['-p', 'no:cacheprovider', '--pyargs', *testfiles])
```

### Comparing `cycept-0.0.3/cycept/tests/test_cycept.py` & `cycept-0.0.4/cycept/tests/test_cycept.py`

 * *Files identical despite different names*

### Comparing `cycept-0.0.3/cycept/tests/test_perf.py` & `cycept-0.0.4/cycept/tests/test_perf.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,70 @@
 import contextlib
 import dataclasses
 import datetime
 import functools
 import inspect
 import os
+import tempfile
 import time
 import warnings
 
 import numpy as np
 
 
-# Number of times to repeat the measurement
+# Number of times to repeat each performance measurement
 repeats = 5
 
-# Rough minimum and maximum number of seconds to spend
-# on each pure Python performance measurement.
-t_perf = (0.1, 10)
-
-# Minimum number of loop iterations deemed appropriate
-calls_appropriate = 100
-
-# Minimum number of loop iterations allowed
-calls_min = 1
+# Rough number of seconds to spend on each performance measurement
+t_perf = 0.2
 
 # JITs known by this module
 names = {
-    'python': 'pure Python',
+    'python': 'Python',
     'numpy': 'NumPy',
     'cycept': 'Cycept',
     'cython': 'Cython',
     'numba': 'Numba',
 }
 class Jit:
-    def __init__(self, *decorators, suppress_compiler_warnings=False):
+    def __init__(self, *decorators, silent_compiler_warnings=False):
         self.decorators = decorators
-        self.suppress_compiler_warnings = suppress_compiler_warnings
+        self.silent_compiler_warnings = silent_compiler_warnings
 @dataclasses.dataclass
 class Findings:
     python: float = np.inf
     numpy: float = np.inf
     cycept: float = np.inf
     cython: float = np.inf
     numba: float = np.inf
 
 
 # Function returning the JITs available on the system
 @functools.cache
-def get_jits():
+def get_jits(silent=True):
     jits = {}
     # Cycept
     try:
         import cycept
     except Exception:
         pass
     else:
-        jits['cycept'] = Jit(cycept.jit)
+        jits['cycept'] = Jit(functools.partial(cycept.jit, silent=silent))
     # Cython
     try:
         import cython
     except Exception:
         pass
     else:
-        jits['cython'] = Jit(cython.compile, suppress_compiler_warnings=True)
+        jits['cython'] = Jit(cython.compile, silent_compiler_warnings=silent)
+        # Set CYTHON_CACHE_DIR to a new temporary directory,
+        # ensuring that Cython does not reuse previously compiled modules.
+        var = 'CYTHON_CACHE_DIR'
+        if var not in os.environ:
+            os.environ[var] = tempfile.mkdtemp()
     # Numba (nopython mode, then fallback to object mode)
     try:
         import numba
     except Exception:
         pass
     else:
         jits['numba'] = Jit(
@@ -81,60 +80,74 @@
         )
     print('JITs:', ', '.join(names[name] for name in jits))
     return jits
 
 
 # Function for running all performance tests without using pytest.
 # (timings will be shown this way).
-def bench(show_func=False):
+def bench(silent=True, show_func=False):
     @contextlib.contextmanager
     def set_globals():
-        global test_asserts, print_source
+        global test_asserts, print_source, silent_jitting
         test_asserts_backup = test_asserts
         print_source_backup = print_source
+        silent_jitting_backup = silent_jitting
         # Disable test asserts when not testing with pytest
         test_asserts = False
         # If show_func, enable printing of the tested source code
-        if show_func:
-            print_source = True
-        yield
-        test_asserts = test_asserts_backup
-        print_source = print_source_backup
+        print_source = show_func
+        # If silent, disable messages during jitting
+        silent_jitting = silent
+        try:
+            yield
+        except Exception:
+            raise
+        finally:
+            test_asserts = test_asserts_backup
+            print_source = print_source_backup
     # Discover and run test functions within this module
     with set_globals():
         for var, val in globals().copy().items():
             if not var.startswith('test_') and not var.endswith('_test'):
                 continue
             if callable(val):
                 val()
 test_asserts = True
 print_source = False
+silent_jitting = True
 
 
 # Main function for performing the performance measurements
 def perf(func, *args, **kwargs):
     func_numpy = None
     if isinstance(func, tuple):
         func, func_numpy = func
 
+    def measure(name, func):
+        calls = determine_calls(func)
+        t_best = np.inf
+        for _ in range(repeats):
+            result, t = run(func, calls)
+            t_best = min(t_best, t)
+        setattr(results, name, result)
+        setattr(timings, name, t_best/calls)
+        return calls
+
+    def determine_calls(func):
+        result, t = run(func)
+        calls = max(int(float(f'{t_perf/t:.0e}')), 1)
+        return calls
+
     def run(func, calls=1):
         tic = time.perf_counter()
         for _ in range(calls):
             result = func(*args, **kwargs)
         toc = time.perf_counter()
         return result, toc - tic
 
-    def measure(name, func, calls=1):
-        t_best = np.inf
-        for _ in range(repeats):
-            result, t = run(func, calls)
-            t_best = min(t_best, t)
-        setattr(results, name, result)
-        setattr(timings, name, t_best)
-
     def print_timings(name, calls):
         def check_equal():
             result = getattr(results, name)
             result_python = results.python
             same_types = (
                 isinstance(result, (int, np.integer))
                 and isinstance(result_python, (int, np.integer))
@@ -160,35 +173,38 @@
             speedup = timings.python/t
             if speedup >= 10:
                 return f'{speedup:.0f}'
             elif speedup >= 1:
                 return f'{speedup:.1f}'
             return f'{speedup:.2f}'
         maxlen = max(map(len, names.values()))
-        s0 = f'* {{:<{maxlen + 1}}}'.format(names[name] + ':')
+        s0 = f'⚡ {{:<{maxlen + 1}}}'.format(names[name] + ':')
         t = getattr(timings, name)
         if t == np.inf:
-            print(f'{s0} Fails to compile')
+            print(f'{s0} Fails to compile'.replace('⚡', '❌'))
             return
         if name != 'python':
             is_equal = check_equal()
             if not is_equal:
-                print(f'{s0} Disagrees with pure Python')
+                print(f'{s0} Disagrees with pure Python'.replace('⚡', '❓'))
             if test_asserts and name == 'cycept':
                 assert is_equal
             if not is_equal:
                 return
-        s1 = s2 = ''
-        if calls > 1:
-            s1 = 's'
+        s1 = 's' if calls > 1 else ' '
+        s2 = ''
         if name != 'python':
             speedup = get_speedup()
             s2 = f' ({speedup}x)'
-        t_pretty = stringify_time(t)
-        print(f'{s0} {calls} loop{s1}, best of {repeats}: {t_pretty:<7} per loop{s2}')
+        calls_pretty = pretty_int(calls)
+        t_pretty = pretty_time(t)
+        print(
+            f'{s0} {calls_pretty} loop{s1}, best of {repeats}: '
+            f'{t_pretty} per loop{s2}'
+        )
 
     def print_heading():
         def dedent(text, indentation='auto'):
             lines = text.split('\n')
             if indentation == 'auto':
                 indentation = ' ' * (len(lines[0]) - len(lines[0].lstrip()))
             lines = [
@@ -208,102 +224,121 @@
         doc = dedent(globals()[caller_name].__doc__, ' ' * 4)
         print('\n'.join(f'# {line}' for line in doc.split('\n')))
         source = get_source(func)
         print(source)
         if func_numpy is not None:
             source_numpy = get_source(func_numpy)
             print(source_numpy)
-    jits = get_jits()
+    jits = get_jits(silent_jitting)
     print_heading()
     timings = Findings()
     results = Findings()
     # Pure Python
-    result, t = run(func)
-    calls = int(float(f'{t_perf[0]/(repeats*t):.0e}'))
-    if calls < calls_appropriate:
-        calls = int(float(f'{t_perf[1]/(repeats*t):.0e}'))
-        calls = min(calls, calls_appropriate)
-    calls = max(calls, calls_min)
-    measure('python', func, calls)
+    calls = measure('python', func)
     print_timings('python', calls)
     # NumPy
     if func_numpy is not None:
-        measure('numpy', func_numpy, calls)
+        calls = measure('numpy', func_numpy)
         print_timings('numpy', calls)
     # Jits
     for name, jit in jits.items():
         for jit_decorator in jit.decorators:
             func_jitted = jit_decorator(func)
             try:
-                with silence(jit.suppress_compiler_warnings):
-                    run(func_jitted)  # to compile
+                with silence(silent_jitting, jit.silent_compiler_warnings):
+                    run(func_jitted)
             except Exception:
                 if name == 'cycept':
                     raise
             else:
-                measure(name, func_jitted, calls)
+                calls = measure(name, func_jitted)
                 break
         print_timings(name, calls)
     return timings
 
 
 # Context manager for silencing stdout and stderr, Python and compiler warnings
 @contextlib.contextmanager
-def silence(silence_compiler_warnings=False):
+def silence(silent=True, silent_compiler_warnings=False):
 
     @contextlib.contextmanager
     def hack_cflags():
         suppress_warnings = {
-            'gcc': '-w',
-            'clang': '-Wno-everything',
+            'gcc': {
+                'CFLAGS': '-w',
+            },
+            'clang': {
+                'CFLAGS': '-Wno-everything',
+            },
         }
-        if not silence_compiler_warnings:
+        if not silent_compiler_warnings:
             yield
             return
-        cflags = ''
-        cflags_backup = None
-        if 'CFLAGS' in os.environ:
-            cflags = os.environ['CFLAGS']
-            cflags_backup = cflags
-        os.environ['CFLAGS'] = ' '.join([cflags, *suppress_warnings.values()])
-        yield
-        if cflags_backup:
-            os.environ['CFLAGS'] = cflags_backuo
-        else:
-            os.environ.pop('CFLAGS')
+        backups = {}
+        for env in suppress_warnings.values():
+            for var in env:
+                backups[var] = os.environ.get(var)
+        for env in suppress_warnings.values():
+            for var, val in env.items():
+                os.environ[var] = os.environ.get(var, '') + f' {val}'
+        try:
+            yield
+        except Exception:
+            raise
+        finally:
+            for var, val in backups.items():
+                if val is None:
+                    os.environ.pop(var)
+                else:
+                    os.environ[var] = val
 
+    if not silent:
+        yield
+        return
     with (
         (devnull := open(os.devnull, 'w')),
         contextlib.redirect_stdout(devnull),
         contextlib.redirect_stderr(devnull),
         warnings.catch_warnings(),
         hack_cflags(),
     ):
         warnings.simplefilter("ignore")
         yield
 
+# Function for converting int of one significant digit to pretty str
+def pretty_int(n):
+    superscripts = '⁰¹²³⁴⁵⁶⁷⁸⁹'
+    if n < 10_000:
+        pretty_i =  str(n)
+    else:
+        factor, _, exponent = f'{n:.0e}'.partition('e')
+        pretty_i = f'{factor}×10{superscripts[int(exponent)]}'
+    return f'{pretty_i:>5}'
 
 # Function for converting time interval in seconds to pretty str
-def stringify_time(t):
+def pretty_time(t):
     if t <= 0:
         return 'no time at all'
     if t == np.inf:
         return '∞'
     units = {
         'ns': 1e-9,
         'μs': 1e-6,
         'ms': 1e-3,
         's': 1,
     }
     for unit, ratio in units.items():
         factor = 59.95 if unit == 's' else 999.5
         if t < factor*ratio:
             num = f'{t/ratio:#.3g}'.rstrip('.')
-            return f'{num} {unit}'
-    return str(datetime.timedelta(seconds=int(round(t)))).removeprefix('0:')
+            t_pretty = f'{num} {unit}'
+            break
+    else:
+        t_pretty = str(datetime.timedelta(seconds=int(round(t)))).removeprefix('0:')
+    return f'{t_pretty:>7}'
 
 
 # Test functions below
 
 def test_prime():
     """Computes the n'th prime number.
     This tests the performance of integer operations.
@@ -316,15 +351,15 @@
             for j in range(2, i):
                 if i % j == 0:
                     break
             else:
                 count += 1
                 if count == n:
                     return i
-    n = 1_000
+    n = 500
     timings = perf(f, n)
     if test_asserts:
         assert timings.cycept < timings.python / 4
 
 
 def test_wallis():
     """Computes π using the Wallis product.
@@ -332,30 +367,30 @@
     """
     def f(n):
         π = 2
         for i in range(1, n):
             π *= 4 * i ** 2 / (4 * i ** 2 - 1)
         return π
     def f_numpy(n):
-        a = 4 * np.arange(1, n) ** 2
+        a = 4 * np.arange(1, n, dtype=np.int64) ** 2
         return 2 * np.prod(a / (a - 1))
-    n = 100_000
+    n = 2_000_000
     timings = perf((f, f_numpy), n)
     if test_asserts:
         assert timings.cycept < timings.python / 50
 
 
 def test_fibonacci():
     """Computes the n'th Fibonacci number using recursion.
     This tests the performance of recursive function calls.
     """
     def f(n):
-        if n < 3:
-            return 1
-        return f(n - 1) + f(n - 2)
+        if n < 2:
+            return n
+        return f(n - 2) + f(n - 1)
     n = 30
     timings = perf(f, n)
     if test_asserts:
         assert timings.cycept < timings.python / 25
 
 
 def test_mostcommon():
@@ -374,27 +409,28 @@
                 counter[obj] = 0
             counter[obj] += 1
         n = max(counter.values())
         for obj, count in counter.items():
             if count == n:
                 return obj
     n = 100
-    objs =  1 * n * list(np.arange(n))
-    objs += 2 * n * list(np.linspace(0, 1, n))
+    objs =  1 * n * list(np.arange(n, dtype=np.int64))
+    objs += 2 * n * list(np.linspace(0, 1, n, dtype=np.float64))
     objs += 3 * n * [None, 'hello', True, (0, 1, 2), 'hello']
     timings = perf(f, objs)
     if test_asserts:
         assert timings.cycept < timings.python
 
 
 def test_life():
     """Evolves a glider in Conway's Game of Life.
     This tests the performance of pure Python operations and closures.
     """
     def f(n):
+        glider = {(0, 2), (1, 0), (1, 2), (2, 1), (2, 2)}
         def evolve(state):
             get_neighbors = lambda x, y: {
                 (x + dx, y + dy)
                 for dx in range(-1, 2)
                 for dy in range(-1, 2)
                 if not dx == dy == 0
             }
@@ -404,18 +440,19 @@
             state_new = set()
             for x, y in squares:
                 neighbors = get_neighbors(x, y)
                 count = len(neighbors & state)
                 if count == 3 or (count == 2 and (x, y) in state):
                     state_new.add((x, y))
             return state_new
-        state = {(0, 2), (1, 0), (1, 2), (2, 1), (2, 2)}
+        state = glider.copy()
         for _ in range(4 * n):
             state = evolve(state)
-    n = 100
+        return state
+    n = 30
     timings = perf(f, n)
     if test_asserts:
         assert timings.cycept < timings.python
 
 
 def test_array():
     """Computes the value sum((a - b)**2) with a and b being arrays.
@@ -425,40 +462,71 @@
         x = 0
         for i in range(a.shape[0]):
             for j in range(a.shape[1]):
                 x += (a[i, j] - b[i, j]) ** 2
         return x
     def f_numpy(a, b):
         return ((a - b)**2).sum()
-    n = 1_000
+    n = 800
     a = np.linspace(0, 1, n ** 2, dtype=np.float64).reshape((n, n))
     b = np.linspace(1, 0, n ** 2, dtype=np.float64).reshape((n, n))
     timings = perf((f, f_numpy), a, b)
     if test_asserts:
         assert timings.cycept < timings.python / 50
 
 
 def test_matmul():
     """Computes the matrix multiplication a @ b.
     This tests the performance of array indexing.
-    Note that the NumPy implementation is by far the fastest
-    (expected as its implementation is much more sophisticated).
+    Here NumPy is expected to be the fastest due to its
+    much more sophisticated implementation.
     """
     def f(a, b):
-        c = np.empty((a.shape[0], b.shape[1]), dtype=a.dtype)
-        for i in range(a.shape[0]):
-            for j in range(b.shape[1]):
+        m, n = a.shape
+        p, q = b.shape
+        b = b.transpose().copy()
+        c = np.empty((m, q), dtype=a.dtype)
+        for i in range(m):
+            for j in range(q):
                 val = 0
-                for k in range(a.shape[1]):
-                    val += a[i, k] * b[k, j]
+                for k in range(n):
+                    val += a[i, k] * b[j, k]
                 c[i, j] = val
         return c
     def f_numpy(a, b):
         return a @ b
-    m, n = 100, 50
-    p, q = n, 200
+    m, n = 150, 350
+    p, q = n, 250
     a = np.linspace(0, 1, m * n, dtype=np.float64).reshape((m, n))
     b = np.linspace(0, 1, p * q, dtype=np.float64).reshape((p, q))
     timings = perf((f, f_numpy), a, b)
     if test_asserts:
-        assert timings.cycept < timings.python / 500
+        assert timings.cycept < timings.python / 200
+
+
+def test_mandelbrot():
+    """Computes an image of the Mandelbrot set.
+    This tests the performance of complex numbers and iteration.
+    """
+    def f(x_min, x_max, y_min, y_max, n_max, image):
+        for i in range(image.shape[0]):
+            for j in range(image.shape[1]):
+                x = x_min + i*(x_max - x_min)/(image.shape[0] - 1)
+                y = y_min + j*(y_max - y_min)/(image.shape[1] - 1)
+                c = x + y*1j
+                z = 0j
+                for n in range(n_max):
+                    z = z * z + c
+                    if abs(z) >= 2:
+                        break
+                image[i, j] = n
+        return image
+    x_min, x_max = -2, 0.5
+    y_min, y_max = -1.2, 1.2
+    n_max = 30
+    width = 300
+    height = int(width*(y_max - y_min)/(x_max - x_min))
+    image = np.empty((width, height), dtype=np.uint8)
+    timings = perf(f, x_min, x_max, y_min, y_max, n_max, image)
+    if test_asserts:
+        assert timings.cycept < timings.python / 30
```

### Comparing `cycept-0.0.3/cycept.egg-info/PKG-INFO` & `cycept-0.0.4/cycept.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycept
-Version: 0.0.3
+Version: 0.0.4
 Summary: Effortless just-in-time compilation of Python functions, powered by Cython
 Author-email: Jeppe Dakin <jeppe_dakin@hotmail.com>
 Project-URL: Download, https://pypi.python.org/pypi/cycept
 Project-URL: Changelog, https://github.com/jmd-dk/cycept/blob/main/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/jmd-dk/cycept/issues
 Project-URL: Source code, https://github.com/jmd-dk/cycept
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: C
+Classifier: Programming Language :: C++
 Classifier: Programming Language :: Cython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -48,14 +49,26 @@
 * On **macOS** you may install [Clang](https://clang.llvm.org/)
   (available through [Xcode](https://developer.apple.com/xcode/)).
 * On **Windows** you may install
   [MSVC](https://en.wikipedia.org/wiki/Microsoft_Visual_C%2B%2B)
   (available through
   [Microsoft C++ Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/)).
 
+If you are using [Anaconda](https://www.anaconda.com/) on Linux or macOS,
+you may also obtain a C compiler through
+`conda install -c conda-forge c-compiler`.
+
+Once installed you can check whether Cycept functions correctly using
+```bash
+python -c "import cycept; cycept.check()"
+```
+If it does not work due to missing `Python.h` and you are running Linux,
+make sure to install the Python development headers (Debian-like distros:
+`sudo apt install python3-dev` if you are using the system Python).
+
 
 ## Quick demo
 ```python
 """Comparison of Python function JITs
 
 Below we implement the sample function sum((a - b)**2) where a and b
 are both 2D NumPy arrays. The following strategies are implemented and
@@ -63,108 +76,109 @@
 * Pure Python (baseline)
 * NumPy
 * Cycept JIT
 * Cython JIT
 * Numba JIT
 """
 
-from time import time
+from time import perf_counter
 import numpy as np
 
-a = np.random.random((2_000, 3_000))
-b = np.random.random((2_000, 3_000))
+m, n = 2_000, 3_000
+a = np.random.random((m, n))
+b = np.random.random((m, n))
 
 # Pure Python
 def func(a, b):
     x = 0
     for i in range(a.shape[0]):
         for j in range(a.shape[1]):
             x += (a[i, j] - b[i, j])**2
     return x
-tic = time()
+tic = perf_counter()
 result = func(a, b)
-toc = time()
+toc = perf_counter()
 t_ref = toc - tic
-print(f'Pure python: {result:<18} in {t_ref:.3e} s')
+print(f'Python: {result:<18} in {t_ref:.3e} s')
 
 # NumPy
 def func_numpy(a, b):
-    return np.sum((a - b)**2)
-tic = time()
+    return ((a - b)**2).sum()
+tic = perf_counter()
 result = func_numpy(a, b)
-toc = time()
+toc = perf_counter()
 t = toc - tic
 print(f'NumPy:       {result:<18} in {t:.3e} s ({int(t_ref/t)}x)')
 
 # Cycept
 import cycept
 @cycept.jit
 def func_cycept(a, b):
     x = 0
     for i in range(a.shape[0]):
         for j in range(a.shape[1]):
             x += (a[i, j] - b[i, j])**2
     return x
 func_cycept(a[:1, :1], b[:1, :1])  # to compile
-tic = time()
+tic = perf_counter()
 result = func_cycept(a, b)
-toc = time()
+toc = perf_counter()
 t = toc - tic
 print(f'Cycept:      {result:<18} in {t:.3e} s ({int(t_ref/t)}x)')
 
 # Cython
 import cython
 @cython.compile
 def func_cython(a, b):
     x = 0
     for i in range(a.shape[0]):
         for j in range(a.shape[1]):
             x += (a[i, j] - b[i, j])**2
     return x
 func_cython(a[:1, :1], b[:1, :1])  # to compile
-tic = time()
+tic = perf_counter()
 result = func_cython(a, b)
-toc = time()
+toc = perf_counter()
 t = toc - tic
 print(f'Cython:      {result:<18} in {t:.3e} s ({int(t_ref/t)}x)')
 
 # Numba
 import numba
-@numba.jit
+@numba.njit
 def func_numba(a, b):
     x = 0
     for i in range(a.shape[0]):
         for j in range(a.shape[1]):
             x += (a[i, j] - b[i, j])**2
     return x
 func_numba(a[:1, :1], b[:1, :1])  # to compile
-tic = time()
+tic = perf_counter()
 result = func_numba(a, b)
-toc = time()
+toc = perf_counter()
 t = toc - tic
 print(f'Numba:       {result:<18} in {t:.3e} s ({int(t_ref/t)}x)')
 ```
 
 Running the above results in something similar to
 ```
-Pure python: 1000265.9355757801 in 2.316e+00 s
-NumPy:       1000265.9355757139 in 2.967e-02 s (78x)
-Cycept:      1000265.9355757138 in 6.429e-03 s (360x)
-Cython:      1000265.9355757801 in 7.103e-02 s (32x)
-Numba:       1000265.9355757801 in 7.376e-03 s (314x)
+Python: 1000265.9355757801 in 2.316e+00 s
+NumPy:  1000265.9355757139 in 2.967e-02 s (78x)
+Cycept: 1000265.9355757138 in 6.429e-03 s (360x)
+Cython: 1000265.9355757801 in 7.103e-02 s (32x)
+Numba:  1000265.9355757801 in 7.376e-03 s (314x)
 ```
 For scientific codebases in the wild, code of the NumPy style is the
 most widespread. However, writing out the loops while adding a JIT can
 often lead to dramatic performance improvements, even when compared
 to NumPy. A further benefit of this is a reduced memory footprint,
 as no temporary arrays are created behind the scenes by the computation.
 
 See the help info on `cycept.jit` for optional arguments:
 ```bash
-python -c 'import cycept; help(cycept.jit)'
+python -c "import cycept; help(cycept.jit)"
 ```
 
 
 ## Tests
 The code contains a unit test suite which may be run as
 ```bash
 python -c "import cycept; cycept.test('cycept')"
@@ -185,11 +199,11 @@
 'Cycept' is an amalgamation of '[Cython](https://cython.org/)' and
 '[CO*N*CEPT](https://github.com/jmd-dk/concept)', the latter of which is a
 cosmological simulation code that makes heavy use of code transformation,
 both custom and through Cython. As the author of both projects, Cycept is my
 attempt to extract some of the code transformation ideas buried within
 CO*N*CEPT, making them available within an easy-to-use library.
 Though no code is shared between the projects, in many respects Cycept
-can be considered a spiritual descendant of CO*N*CEPT.
+can be considered a spiritual successor to CO*N*CEPT.
 Furthermore, 'Cy*cept*' has a nice in*cept*ion ring to it,
 which seems fitting for a piece of code that generates code.
```

### Comparing `cycept-0.0.3/pyproject.toml` & `cycept-0.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools >= 65.6.0, < 68",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cycept"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     {name="Jeppe Dakin", email="jeppe_dakin@hotmail.com"},
 ]
 description = "Effortless just-in-time compilation of Python functions, powered by Cython"
 readme = "README.md"
 requires-python = ">= 3.9"
 dependencies = [
@@ -26,14 +26,15 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: C",
+    "Programming Language :: C++",
     "Programming Language :: Cython",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development :: Code Generators",
     "Topic :: Software Development :: Compilers",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
```

