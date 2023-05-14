# Comparing `tmp/pipe21-1.8.0.tar.gz` & `tmp/pipe21-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipe21-1.8.0.tar", last modified: Sun Mar 12 10:56:23 2023, max compression
+gzip compressed data, was "pipe21-1.9.0.tar", last modified: Sat May 13 04:38:53 2023, max compression
```

## Comparing `pipe21-1.8.0.tar` & `pipe21-1.9.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 10:56:23.598630 pipe21-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-03-12 10:56:23.598630 pipe21-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-03-12 10:56:06.000000 pipe21-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 10:56:23.598630 pipe21-1.8.0/pipe21.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-03-12 10:56:23.000000 pipe21-1.8.0/pipe21.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-12 10:56:23.000000 pipe21-1.8.0/pipe21.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-12 10:56:23.000000 pipe21-1.8.0/pipe21.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-12 10:56:23.000000 pipe21-1.8.0/pipe21.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-12 10:56:23.000000 pipe21-1.8.0/pipe21.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-12 10:56:23.000000 pipe21-1.8.0/pipe21.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-03-12 10:56:06.000000 pipe21-1.8.0/pipe21.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-03-12 10:56:06.000000 pipe21-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-12 10:56:23.598630 pipe21-1.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 04:38:53.817582 pipe21-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-05-13 04:38:53.817582 pipe21-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-05-13 04:38:39.000000 pipe21-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 04:38:53.817582 pipe21-1.9.0/pipe21.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-05-13 04:38:53.000000 pipe21-1.9.0/pipe21.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-13 04:38:53.000000 pipe21-1.9.0/pipe21.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 04:38:53.000000 pipe21-1.9.0/pipe21.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-13 04:38:53.000000 pipe21-1.9.0/pipe21.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-13 04:38:53.000000 pipe21-1.9.0/pipe21.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-13 04:38:39.000000 pipe21-1.9.0/pipe21.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-05-13 04:38:39.000000 pipe21-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 04:38:53.817582 pipe21-1.9.0/setup.cfg
```

### Comparing `pipe21-1.8.0/PKG-INFO` & `pipe21-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipe21
-Version: 1.8.0
+Version: 1.9.0
 Summary: simple functional pipes
 Author-email: Alexander Rodionov <tandav@tandav.me>
 Project-URL: source, https://github.com/tandav/pipe21
 Project-URL: docs, https://tandav.github.io/pipe21/
 Project-URL: issues, https://github.com/tandav/pipe21/issues
 Project-URL: release notes, https://github.com/tandav/pipe21/releases
 Requires-Python: >=3.8
@@ -130,7 +130,8 @@
 )
 ```
 
 ---
 
 - [all available methods reference](reference.md)
 - [review of similar tools / alternatives](similar-tools.md)
+- written in pure python (70 LOC), no dependencies
```

### Comparing `pipe21-1.8.0/README.md` & `pipe21-1.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -117,7 +117,8 @@
 )
 ```
 
 ---
 
 - [all available methods reference](reference.md)
 - [review of similar tools / alternatives](similar-tools.md)
+- written in pure python (70 LOC), no dependencies
```

### Comparing `pipe21-1.8.0/pipe21.egg-info/PKG-INFO` & `pipe21-1.9.0/pipe21.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipe21
-Version: 1.8.0
+Version: 1.9.0
 Summary: simple functional pipes
 Author-email: Alexander Rodionov <tandav@tandav.me>
 Project-URL: source, https://github.com/tandav/pipe21
 Project-URL: docs, https://tandav.github.io/pipe21/
 Project-URL: issues, https://github.com/tandav/pipe21/issues
 Project-URL: release notes, https://github.com/tandav/pipe21/releases
 Requires-Python: >=3.8
@@ -130,7 +130,8 @@
 )
 ```
 
 ---
 
 - [all available methods reference](reference.md)
 - [review of similar tools / alternatives](similar-tools.md)
+- written in pure python (70 LOC), no dependencies
```

### Comparing `pipe21-1.8.0/pipe21.py` & `pipe21-1.9.0/pipe21.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 import functools
 import itertools
 import re
 
-__version__ = '1.8.0'
+__version__ = '1.9.0'
 
 
 class B:
     def __init__(self, f=None, *args, **kw):
-        self.f = f; self.args = args; self.kw = kw
-class Pipe  (B): __ror__ = lambda self, x: self.f(x)
-class Map   (B): __ror__ = lambda self, x: map   (self.f, x)
-class Filter(B): __ror__ = lambda self, x: filter(self.f, x)
+        self.f = f
+        self.args = args
+        self.kw = kw
 
 
-class Reduce       (B): __ror__ = lambda self, x: functools.reduce(self.f, x, *self.args)
+class Pipe         (B): __ror__ = lambda self, x: self.f(x)
+class Map          (B): __ror__ = lambda self, it: map(self.f, it)
+class Filter       (B): __ror__ = lambda self, it: filter(self.f, it)
+class Reduce       (B): __ror__ = lambda self, it: functools.reduce(self.f, it, *self.args)
 class MapValues    (B): __ror__ = lambda self, it: it | Map(lambda kv: (kv[0], self.f(kv[1])))
 class MapKeys      (B): __ror__ = lambda self, it: it | Map(lambda kv: (self.f(kv[0]), kv[1]))
 class FilterFalse  (B): __ror__ = lambda self, it: it | Filter(lambda x: not self.f(x))
 class FilterKeys   (B): __ror__ = lambda self, it: it | Filter(lambda x: (self.f or bool)(x[0]))
 class FilterValues (B): __ror__ = lambda self, it: it | Filter(lambda x: (self.f or bool)(x[1]))
 class FlatMap      (B): __ror__ = lambda self, it: it | Map(self.f) | Pipe(itertools.chain.from_iterable)
 class FlatMapValues(B): __ror__ = lambda self, it: it | FlatMap(lambda kv: ((kv[0], x) for x in self.f(kv[1])))
 class KeyBy        (B): __ror__ = lambda self, it: it | Map(lambda x: (self.f(x), x))
 class ValueBy      (B): __ror__ = lambda self, it: it | Map(lambda x: (x, self.f(x)))
 class Append       (B): __ror__ = lambda self, it: it | Map(lambda x: (*x, self.f(x)))
 class Keys         (B): __ror__ = lambda self, it: it | Map(lambda x: x[0])
 class Values       (B): __ror__ = lambda self, it: it | Map(lambda x: x[1])
-class Grep         (B): __ror__ = lambda self, it: it | Filter(lambda x:     re.search(self.f, x))
+class Grep         (B): __ror__ = lambda self, it: it | Filter(lambda x: re.search(self.f, x))
 class GrepV        (B): __ror__ = lambda self, it: it | Filter(lambda x: not re.search(self.f, x))
 class Count        (B): __ror__ = lambda self, it: sum(1 for _ in it)
 class Slice        (B): __ror__ = lambda self, it: itertools.islice(it, self.f, *self.args)
 class Take         (B): __ror__ = lambda self, it: it | Slice(self.f) | Pipe(tuple)
 class Chunked      (B): __ror__ = lambda self, it: iter(functools.partial(lambda n, i: i | Take(n), self.f, iter(it)), ())
-class GroupBy      (B): __ror__ = lambda self, it: itertools.groupby(it, key=self.f)
+class Sorted       (B): __ror__ = lambda self, it: sorted(it, **self.kw)
+class GroupBy      (B): __ror__ = lambda self, it: itertools.groupby(it | Sorted(key=self.f), key=self.f)
 class PipeArgs     (B): __ror__ = lambda self, x: self.f(*x)
 class StarMap      (B): __ror__ = lambda self, x: x | Map(lambda y: y | PipeArgs(self.f))
 class IsUnique     (B): __ror__ = lambda self, seq: len(seq) == len(set(seq if self.f is None else map(self.f, seq)))
-class Sorted       (B): __ror__ = lambda self, it: sorted(it, **self.kw)
 class MapApply     (B): __ror__ = lambda self, it: it | Map(lambda x: x | Apply(self.f))
 class ReduceByKey  (B): __ror__ = lambda self, it: it | Sorted(lambda kv: kv[0]) | GroupBy(lambda kv: kv[0]) | MapValues(lambda kv: kv | Values() | Reduce(self.f)) | Pipe(list)
 
 
 class Unique(B):
     def __ror__(self, it):
         key = self.f or (lambda x: x)
```

### Comparing `pipe21-1.8.0/pyproject.toml` & `pipe21-1.9.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pipe21"
-version = "1.8.0"
+version = "1.9.0"
 authors = [
     {name = "Alexander Rodionov", email = "tandav@tandav.me"},
 ]
 description = "simple functional pipes"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = []
@@ -25,29 +25,24 @@
 
 [project.urls]
 source = "https://github.com/tandav/pipe21"
 docs = "https://tandav.github.io/pipe21/"
 issues = "https://github.com/tandav/pipe21/issues"
 "release notes" = "https://github.com/tandav/pipe21/releases"
 
-
-[project.scripts]
-chans-cli = "chans.__main__:main"
-chans-server = "chans.server:main"
-
 # ==============================================================================
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 # ==============================================================================
 
 [tool.bumpver]
-current_version = "v1.8.0"
+current_version = "v1.9.0"
 version_pattern = "vMAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
@@ -88,56 +83,71 @@
 [[tool.mypy.overrides]]
 module = ["tests.*"]
 disallow_untyped_defs = false
 
 # ==============================================================================
 
 [tool.ruff]
-extend-select = [
-    "W",
-    "C",
-    "I",
-    "SIM",
-    "TCH",
-    "C4",
-    "S",
-    "BLE",
-    "B",
-    "T10",
-    "INP",
-    "PIE",
-    "PL",
-    "RUF",
-]
+select = ["ALL"]
 ignore = [
     "E501",  # line too long
-    "E731",
-    "E701",
-    "E702",
+    "E731", # lambda assignment
+    "E701", # multiple statements
+    "E702", # multiple statements
     "F403", # star imports
     "F405", # star imports
-    "B008",
-    "PLR0913",
-    "TCH003",
+    "B008", # function-call-in-default-argument
+    "PLR0913", # too-many-arguments
+    "TCH003", # typing-only-standard-library-import
+    "ANN", # type annotations
+    "D", #docstrings
+    "Q", # quotes
+    "ARG005", # Unused lambda argument
+    "PTH123", # `open()` should be replaced by `Path.open()`
 ]
 
 [tool.ruff.per-file-ignores]
 "examples/*" = ["INP001"]
 "tests/*" = ["S101"]
 
 [tool.ruff.isort]
 force-single-line = true
 
 # ==============================================================================
 
+[tool.pylint.MASTER]
+load-plugins=[
+    "pylint_per_file_ignores",
+]
+
 [tool.pylint.messages-control]
 disable = [
-    "C0321","C3001","C0116","C0301","C0103","C0115","C0114",
-    "W1514",
-    "W0401",  # wildcard import
-    "W0614",
-    "W1113",
-    "R0903",
-    "E0401",
+    "invalid-name",
+    "missing-function-docstring",
+    "missing-class-docstring",
+    "missing-module-docstring",
+    "unnecessary-lambda-assignment",
+    "multiple-statements",
+    "line-too-long",
+    "unspecified-encoding",
+    "wildcard-import",
+    "unused-wildcard-import",
+    "keyword-arg-before-vararg",
+    "too-few-public-methods",
 ]
 
+[tool.pylint-per-file-ignores]
+"/tests/" = "import-error"
+
+# ==============================================================================
+
+[tool.autopep8]
+ignore="E501,E701"
+recursive = true
+aggressive = 3
+
+# ==============================================================================
+
+[tool.pytest.ini_options]
+asyncio_mode = "strict"
+
 # ==============================================================================
```

