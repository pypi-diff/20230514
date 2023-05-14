# Comparing `tmp/hypofuzz-23.4.1.tar.gz` & `tmp/hypofuzz-23.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypofuzz-23.4.1.tar", last modified: Wed Apr 26 00:18:40 2023, max compression
+gzip compressed data, was "hypofuzz-23.5.1.tar", last modified: Sun May 14 01:44:54 2023, max compression
```

## Comparing `hypofuzz-23.4.1.tar` & `hypofuzz-23.5.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:18:40.243405 hypofuzz-23.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-26 00:18:40.243405 hypofuzz-23.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 00:18:40.243405 hypofuzz-23.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:18:40.239405 hypofuzz-23.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:18:40.239405 hypofuzz-23.4.1/src/hypofuzz/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/src/hypofuzz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/src/hypofuzz/corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/src/hypofuzz/cov.py
--rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/src/hypofuzz/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/src/hypofuzz/debugger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/src/hypofuzz/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17170 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/src/hypofuzz/hy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/src/hypofuzz/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/src/hypofuzz/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:18:40.243405 hypofuzz-23.4.1/src/hypofuzz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-26 00:18:40.000000 hypofuzz-23.4.1/src/hypofuzz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-26 00:18:40.000000 hypofuzz-23.4.1/src/hypofuzz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 00:18:40.000000 hypofuzz-23.4.1/src/hypofuzz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-26 00:18:40.000000 hypofuzz-23.4.1/src/hypofuzz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 00:18:40.000000 hypofuzz-23.4.1/src/hypofuzz.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-26 00:18:40.000000 hypofuzz-23.4.1/src/hypofuzz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 00:18:40.000000 hypofuzz-23.4.1/src/hypofuzz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:18:40.243405 hypofuzz-23.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/tests/test_corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/tests/test_coverage_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/tests/test_fuzz_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:44:54.544266 hypofuzz-23.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-14 01:44:54.544266 hypofuzz-23.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 01:44:54.544266 hypofuzz-23.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:44:54.540266 hypofuzz-23.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:44:54.544266 hypofuzz-23.5.1/src/hypofuzz/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/src/hypofuzz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/src/hypofuzz/corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/src/hypofuzz/cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/src/hypofuzz/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/src/hypofuzz/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/src/hypofuzz/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17271 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/src/hypofuzz/hy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/src/hypofuzz/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/src/hypofuzz/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:44:54.544266 hypofuzz-23.5.1/src/hypofuzz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-14 01:44:54.000000 hypofuzz-23.5.1/src/hypofuzz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-14 01:44:54.000000 hypofuzz-23.5.1/src/hypofuzz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 01:44:54.000000 hypofuzz-23.5.1/src/hypofuzz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-14 01:44:54.000000 hypofuzz-23.5.1/src/hypofuzz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 01:44:54.000000 hypofuzz-23.5.1/src/hypofuzz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-14 01:44:54.000000 hypofuzz-23.5.1/src/hypofuzz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-14 01:44:54.000000 hypofuzz-23.5.1/src/hypofuzz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:44:54.544266 hypofuzz-23.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/tests/test_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/tests/test_coverage_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/tests/test_fuzz_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-14 01:44:44.000000 hypofuzz-23.5.1/tests/test_version.py
```

### Comparing `hypofuzz-23.4.1/LICENSE` & `hypofuzz-23.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.4.1/PKG-INFO` & `hypofuzz-23.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypofuzz
-Version: 23.4.1
+Version: 23.5.1
 Summary: Adaptive fuzzing for property-based tests
 Home-page: https://hypofuzz.com/
 Author: Zac Hatfield-Dodds
 Author-email: zac@hypofuzz.com
 License: AGPL-3.0
 Project-URL: Documentation, https://hypofuzz.com/docs/
 Project-URL: Changelog, https://hypofuzz.com/docs/changelog.html
```

### Comparing `hypofuzz-23.4.1/README.md` & `hypofuzz-23.5.1/README.md`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.4.1/setup.py` & `hypofuzz-23.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     },
     license="AGPL-3.0",
     description="Adaptive fuzzing for property-based tests",
     zip_safe=False,
     install_requires=[
         "coverage >= 5.2.1",
         "dash >= 2.0.0",
-        "hypothesis[cli] >= 6.50.1",
+        "hypothesis[cli] >= 6.75.2",
         "pandas >= 1.0.0",
         "psutil >= 3.0.0",
         "pytest >= 6.0.1",
         "requests >= 2.24.0",
     ],
     extras_require={
         "pytrace": [
```

### Comparing `hypofuzz-23.4.1/src/hypofuzz/corpus.py` & `hypofuzz-23.5.1/src/hypofuzz/corpus.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.4.1/src/hypofuzz/cov.py` & `hypofuzz-23.5.1/src/hypofuzz/cov.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.4.1/src/hypofuzz/dashboard.py` & `hypofuzz-23.5.1/src/hypofuzz/dashboard.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.4.1/src/hypofuzz/debugger.py` & `hypofuzz-23.5.1/src/hypofuzz/debugger.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.4.1/src/hypofuzz/entrypoint.py` & `hypofuzz-23.5.1/src/hypofuzz/entrypoint.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.4.1/src/hypofuzz/hy.py` & `hypofuzz-23.5.1/src/hypofuzz/hy.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,19 @@
 from hypothesis.internal.reflection import function_digest, get_signature
 from hypothesis.reporting import with_reporter
 from sortedcontainers import SortedKeyList
 
 from .corpus import BlackBoxMutator, CrossOverMutator, EngineStub, HowGenerated, Pool
 from .cov import CustomCollectionContext
 
+record_pytrace: Optional[Callable[..., Any]]
 try:
     from .debugger import record_pytrace
 except ImportError:
-    record_pytrace = None  # type: ignore
+    record_pytrace = None
 
 Report = Dict[str, Union[int, float, str, list, Dict[str, int]]]
 
 UNDELIVERED_REPORTS: List[Report] = []
 
 
 @contextlib.contextmanager
@@ -78,15 +79,15 @@
     """
 
     @classmethod
     def from_hypothesis_test(
         cls,
         wrapped_test: Any,
         *,
-        nodeid: str = None,
+        nodeid: Optional[str] = None,
         extra_kw: Optional[Dict[str, object]] = None,
     ) -> "FuzzProcess":
         """Return a FuzzProcess for an @given-decorated test function."""
         _, _, _, search_strategy = process_arguments_to_given(
             wrapped_test,
             arguments=(),
             kwargs=extra_kw or {},
@@ -104,15 +105,15 @@
 
     def __init__(
         self,
         test_fn: Callable,
         strategy: st.SearchStrategy,
         *,
         random_seed: int = 0,
-        nodeid: str = None,
+        nodeid: Optional[str] = None,
         database_key: bytes,
         hypothesis_database: ExampleDatabase,
     ) -> None:
         """Construct a FuzzProcess from specific arguments."""
         # The actual fuzzer implementation
         self.random = Random(random_seed)
         self.__test_fn = test_fn
@@ -201,14 +202,15 @@
             # Shrink to our minimal failing example, since we'll stop after this.
             self.shrinking = True
             shrinker = Shrinker(
                 EngineStub(self._run_test_on, self.random),
                 result,
                 predicate=lambda d: d.status is Status.INTERESTING,
                 allow_transition=None,
+                explain=True,
             )
             self.stop_shrinking_at = self.elapsed_time + 300
             with contextlib.suppress(HitShrinkTimeoutError):
                 shrinker.shrink()
             self.shrinking = False
             if record_pytrace:
                 # Replay minimal example under our time-travelling debug tracer
@@ -230,15 +232,15 @@
         #     self.pool.distill(self._run_test_on, self.random)
 
     def _run_test_on(
         self,
         buffer: bytes,
         *,
         source: HowGenerated = HowGenerated.shrinking,
-        collector: contextlib.AbstractContextManager = None,
+        collector: Optional[contextlib.AbstractContextManager] = None,
     ) -> ConjectureData:
         """Run the test_fn on a given buffer of bytes, in a way a Shrinker can handle.
 
         In normal operation, it's called via run_one (above), but we might also
         delegate to the shrinker to find minimal covering examples.
         """
         start = time.perf_counter()
@@ -356,15 +358,15 @@
 
     @property
     def has_found_failure(self) -> bool:
         """If we've already found a failing example we might reprioritize."""
         return bool(self.pool.interesting_examples)
 
 
-def fuzz_several(*targets_: FuzzProcess, random_seed: int = None) -> NoReturn:
+def fuzz_several(*targets_: FuzzProcess, random_seed: Optional[int] = None) -> NoReturn:
     """Take N fuzz targets and run them all."""
     # TODO: this isn't actually multi-process yet, and that's bad.
     rand = Random(random_seed)
     targets = SortedKeyList(targets_, lambda t: t.since_new_cov)
 
     # Loop forever: at each timestep, we choose a target using an epsilon-greedy
     # strategy for simplicity (TODO: improve this later) and run it once.
```

### Comparing `hypofuzz-23.4.1/src/hypofuzz/interface.py` & `hypofuzz-23.5.1/src/hypofuzz/interface.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-"""CLI and Python API for the fuzzer."""
-import io
-import sys
-from contextlib import redirect_stdout, suppress
-from functools import partial
-from typing import TYPE_CHECKING, Iterable, List, NoReturn, Tuple
-
-import pytest
-import requests
-
-if TYPE_CHECKING:
-    # We have to defer imports to within functions here, because this module
-    # is a Hypothesis entry point and is thus imported earlier than the others.
-    from .hy import FuzzProcess
-
-
-class _ItemsCollector:
-    """A pytest plugin which grabs all the fuzzable tests at the end of collection."""
-
-    def __init__(self) -> None:
-        self.fuzz_targets: List["FuzzProcess"] = []
-
-    def pytest_collection_finish(self, session: pytest.Session) -> None:
-        from .hy import FuzzProcess
-
-        for item in session.items:
-            # If the test takes a fixture, we skip it - the fuzzer doesn't have
-            # pytest scopes, so we just can't support them.  TODO: note skips.
-            if item._request._fixturemanager.getfixtureinfo(
-                node=item, func=item.function, cls=None
-            ).name2fixturedefs:
-                continue
-            # For parametrized tests, we have to pass the parametrized args into
-            # wrapped_test.hypothesis.get_strategy() to avoid trivial TypeErrors
-            # from missing required arguments.
-            extra_kw = item.callspec.params if hasattr(item, "callspec") else {}
-            # Wrap it up in a FuzzTarget and we're done!
-            fuzz = FuzzProcess.from_hypothesis_test(
-                item.obj, nodeid=item.nodeid, extra_kw=extra_kw
-            )
-            self.fuzz_targets.append(fuzz)
-
-
-def _get_hypothesis_tests_with_pytest(args: Iterable[str]) -> List["FuzzProcess"]:
-    """Find the hypothesis-only test functions run by pytest.
-
-    This basically uses `pytest --collect-only -m hypothesis $args`.
-    """
-    collector = _ItemsCollector()
-    out = io.StringIO()
-    with redirect_stdout(out):
-        ret = pytest.main(
-            args=[
-                "--collect-only",
-                "-m=hypothesis",
-                "--pythonwarnings=ignore::pytest.PytestAssertRewriteWarning",
-                *args,
-            ],
-            plugins=[collector],
-        )
-    if ret:
-        print(out.getvalue())  # noqa
-        print(f"Exiting because pytest returned exit code {ret}")  # noqa
-        sys.exit(ret)
-    return collector.fuzz_targets
-
-
-def _post(port: int, data: dict) -> None:
-    with suppress(Exception):
-        requests.post(f"http://localhost:{port}/", json=data)
-
-
-def _fuzz_several(
-    pytest_args: Tuple[str, ...], nodeids: List[str], port: int = None
-) -> NoReturn:
-    """Collect and fuzz tests.
-
-    Designed to be used inside a multiprocessing.Process started with the spawn()
-    method - requires picklable arguments but works on Windows too.
-    """
-    # Import within the function to break an import cycle when used as an entry point.
-    from .hy import fuzz_several
-
-    tests = [
-        t for t in _get_hypothesis_tests_with_pytest(pytest_args) if t.nodeid in nodeids
-    ]
-    if port is not None:
-        for t in tests:
-            t._report_change = partial(_post, port)  # type: ignore
-
-    fuzz_several(*tests)
-    raise NotImplementedError("unreachable")
+"""CLI and Python API for the fuzzer."""
+import io
+import sys
+from contextlib import redirect_stdout, suppress
+from functools import partial
+from typing import TYPE_CHECKING, Iterable, List, NoReturn, Optional, Tuple
+
+import pytest
+import requests
+
+if TYPE_CHECKING:
+    # We have to defer imports to within functions here, because this module
+    # is a Hypothesis entry point and is thus imported earlier than the others.
+    from .hy import FuzzProcess
+
+
+class _ItemsCollector:
+    """A pytest plugin which grabs all the fuzzable tests at the end of collection."""
+
+    def __init__(self) -> None:
+        self.fuzz_targets: List["FuzzProcess"] = []
+
+    def pytest_collection_finish(self, session: pytest.Session) -> None:
+        from .hy import FuzzProcess
+
+        for item in session.items:
+            # If the test takes a fixture, we skip it - the fuzzer doesn't have
+            # pytest scopes, so we just can't support them.  TODO: note skips.
+            if item._request._fixturemanager.getfixtureinfo(
+                node=item, func=item.function, cls=None
+            ).name2fixturedefs:
+                continue
+            # For parametrized tests, we have to pass the parametrized args into
+            # wrapped_test.hypothesis.get_strategy() to avoid trivial TypeErrors
+            # from missing required arguments.
+            extra_kw = item.callspec.params if hasattr(item, "callspec") else {}
+            # Wrap it up in a FuzzTarget and we're done!
+            fuzz = FuzzProcess.from_hypothesis_test(
+                item.obj, nodeid=item.nodeid, extra_kw=extra_kw
+            )
+            self.fuzz_targets.append(fuzz)
+
+
+def _get_hypothesis_tests_with_pytest(args: Iterable[str]) -> List["FuzzProcess"]:
+    """Find the hypothesis-only test functions run by pytest.
+
+    This basically uses `pytest --collect-only -m hypothesis $args`.
+    """
+    collector = _ItemsCollector()
+    out = io.StringIO()
+    with redirect_stdout(out):
+        ret = pytest.main(
+            args=[
+                "--collect-only",
+                "-m=hypothesis",
+                "--pythonwarnings=ignore::pytest.PytestAssertRewriteWarning",
+                *args,
+            ],
+            plugins=[collector],
+        )
+    if ret:
+        print(out.getvalue())  # noqa
+        print(f"Exiting because pytest returned exit code {ret}")  # noqa
+        sys.exit(ret)
+    return collector.fuzz_targets
+
+
+def _post(port: int, data: dict) -> None:
+    with suppress(Exception):
+        requests.post(f"http://localhost:{port}/", json=data, timeout=30)
+
+
+def _fuzz_several(
+    pytest_args: Tuple[str, ...], nodeids: List[str], port: Optional[int] = None
+) -> NoReturn:
+    """Collect and fuzz tests.
+
+    Designed to be used inside a multiprocessing.Process started with the spawn()
+    method - requires picklable arguments but works on Windows too.
+    """
+    # Import within the function to break an import cycle when used as an entry point.
+    from .hy import fuzz_several
+
+    tests = [
+        t for t in _get_hypothesis_tests_with_pytest(pytest_args) if t.nodeid in nodeids
+    ]
+    if port is not None:
+        for t in tests:
+            t._report_change = partial(_post, port)  # type: ignore
+
+    fuzz_several(*tests)
+    raise NotImplementedError("unreachable")
```

### Comparing `hypofuzz-23.4.1/src/hypofuzz.egg-info/PKG-INFO` & `hypofuzz-23.5.1/src/hypofuzz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypofuzz
-Version: 23.4.1
+Version: 23.5.1
 Summary: Adaptive fuzzing for property-based tests
 Home-page: https://hypofuzz.com/
 Author: Zac Hatfield-Dodds
 Author-email: zac@hypofuzz.com
 License: AGPL-3.0
 Project-URL: Documentation, https://hypofuzz.com/docs/
 Project-URL: Changelog, https://hypofuzz.com/docs/changelog.html
```

### Comparing `hypofuzz-23.4.1/src/hypofuzz.egg-info/SOURCES.txt` & `hypofuzz-23.5.1/src/hypofuzz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.4.1/tests/test_corpus.py` & `hypofuzz-23.5.1/tests/test_corpus.py`

 * *Files identical despite different names*

### Comparing `hypofuzz-23.4.1/tests/test_version.py` & `hypofuzz-23.5.1/tests/test_version.py`

 * *Files identical despite different names*

