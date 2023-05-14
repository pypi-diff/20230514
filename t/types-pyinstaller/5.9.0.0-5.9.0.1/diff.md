# Comparing `tmp/types-pyinstaller-5.9.0.0.tar.gz` & `tmp/types-pyinstaller-5.9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pyinstaller-5.9.0.0.tar", last modified: Tue Mar 14 01:10:39 2023, max compression
+gzip compressed data, was "types-pyinstaller-5.9.0.1.tar", last modified: Mon Mar 27 18:25:41 2023, max compression
```

## Comparing `types-pyinstaller-5.9.0.0.tar` & `types-pyinstaller-5.9.0.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 01:10:39.334492 types-pyinstaller-5.9.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-03-14 01:10:38.000000 types-pyinstaller-5.9.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-14 01:10:38.000000 types-pyinstaller-5.9.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-03-14 01:10:39.334492 types-pyinstaller-5.9.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 01:10:39.326492 types-pyinstaller-5.9.0.0/PyInstaller-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-14 01:10:38.000000 types-pyinstaller-5.9.0.0/PyInstaller-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-14 01:10:26.000000 types-pyinstaller-5.9.0.0/PyInstaller-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-03-14 01:10:26.000000 types-pyinstaller-5.9.0.0/PyInstaller-stubs/__main__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 01:10:39.330492 types-pyinstaller-5.9.0.0/PyInstaller-stubs/building/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 01:10:26.000000 types-pyinstaller-5.9.0.0/PyInstaller-stubs/building/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-14 01:10:26.000000 types-pyinstaller-5.9.0.0/PyInstaller-stubs/building/build_main.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-03-14 01:10:26.000000 types-pyinstaller-5.9.0.0/PyInstaller-stubs/building/datastruct.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-03-14 01:10:26.000000 types-pyinstaller-5.9.0.0/PyInstaller-stubs/compat.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 01:10:39.330492 types-pyinstaller-5.9.0.0/PyInstaller-stubs/depend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 01:10:26.000000 types-pyinstaller-5.9.0.0/PyInstaller-stubs/depend/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-03-14 01:10:26.000000 types-pyinstaller-5.9.0.0/PyInstaller-stubs/depend/analysis.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-03-14 01:10:26.000000 types-pyinstaller-5.9.0.0/PyInstaller-stubs/depend/imphookapi.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 01:10:39.330492 types-pyinstaller-5.9.0.0/PyInstaller-stubs/isolated/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-14 01:10:26.000000 types-pyinstaller-5.9.0.0/PyInstaller-stubs/isolated/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-14 01:10:26.000000 types-pyinstaller-5.9.0.0/PyInstaller-stubs/isolated/_parent.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 01:10:39.330492 types-pyinstaller-5.9.0.0/PyInstaller-stubs/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 01:10:26.000000 types-pyinstaller-5.9.0.0/PyInstaller-stubs/lib/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 01:10:39.330492 types-pyinstaller-5.9.0.0/PyInstaller-stubs/lib/modulegraph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 01:10:26.000000 types-pyinstaller-5.9.0.0/PyInstaller-stubs/lib/modulegraph/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-03-14 01:10:26.000000 types-pyinstaller-5.9.0.0/PyInstaller-stubs/lib/modulegraph/modulegraph.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 01:10:39.330492 types-pyinstaller-5.9.0.0/PyInstaller-stubs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 01:10:26.000000 types-pyinstaller-5.9.0.0/PyInstaller-stubs/utils/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 01:10:39.334492 types-pyinstaller-5.9.0.0/PyInstaller-stubs/utils/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-03-14 01:10:26.000000 types-pyinstaller-5.9.0.0/PyInstaller-stubs/utils/hooks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-03-14 01:10:26.000000 types-pyinstaller-5.9.0.0/PyInstaller-stubs/utils/hooks/conda.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-14 01:10:26.000000 types-pyinstaller-5.9.0.0/PyInstaller-stubs/utils/hooks/win32.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 01:10:39.334492 types-pyinstaller-5.9.0.0/pyi_splash-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-14 01:10:38.000000 types-pyinstaller-5.9.0.0/pyi_splash-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-14 01:10:26.000000 types-pyinstaller-5.9.0.0/pyi_splash-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 01:10:39.334492 types-pyinstaller-5.9.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-03-14 01:10:38.000000 types-pyinstaller-5.9.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 01:10:39.334492 types-pyinstaller-5.9.0.0/types_pyinstaller.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-03-14 01:10:39.000000 types-pyinstaller-5.9.0.0/types_pyinstaller.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-03-14 01:10:39.000000 types-pyinstaller-5.9.0.0/types_pyinstaller.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 01:10:39.000000 types-pyinstaller-5.9.0.0/types_pyinstaller.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-14 01:10:39.000000 types-pyinstaller-5.9.0.0/types_pyinstaller.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-14 01:10:39.000000 types-pyinstaller-5.9.0.0/types_pyinstaller.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:41.283988 types-pyinstaller-5.9.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-03-27 18:25:40.000000 types-pyinstaller-5.9.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:25:40.000000 types-pyinstaller-5.9.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-03-27 18:25:41.283988 types-pyinstaller-5.9.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:41.283988 types-pyinstaller-5.9.0.1/PyInstaller-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-27 18:25:40.000000 types-pyinstaller-5.9.0.1/PyInstaller-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-27 18:21:24.000000 types-pyinstaller-5.9.0.1/PyInstaller-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-03-27 18:21:24.000000 types-pyinstaller-5.9.0.1/PyInstaller-stubs/__main__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:41.283988 types-pyinstaller-5.9.0.1/PyInstaller-stubs/building/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pyinstaller-5.9.0.1/PyInstaller-stubs/building/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-27 18:21:24.000000 types-pyinstaller-5.9.0.1/PyInstaller-stubs/building/build_main.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-03-27 18:21:24.000000 types-pyinstaller-5.9.0.1/PyInstaller-stubs/building/datastruct.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-03-27 18:21:24.000000 types-pyinstaller-5.9.0.1/PyInstaller-stubs/compat.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:41.283988 types-pyinstaller-5.9.0.1/PyInstaller-stubs/depend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pyinstaller-5.9.0.1/PyInstaller-stubs/depend/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-03-27 18:21:24.000000 types-pyinstaller-5.9.0.1/PyInstaller-stubs/depend/analysis.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-03-27 18:21:24.000000 types-pyinstaller-5.9.0.1/PyInstaller-stubs/depend/imphookapi.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:41.283988 types-pyinstaller-5.9.0.1/PyInstaller-stubs/isolated/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-27 18:21:24.000000 types-pyinstaller-5.9.0.1/PyInstaller-stubs/isolated/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-27 18:21:24.000000 types-pyinstaller-5.9.0.1/PyInstaller-stubs/isolated/_parent.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:41.283988 types-pyinstaller-5.9.0.1/PyInstaller-stubs/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pyinstaller-5.9.0.1/PyInstaller-stubs/lib/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:41.283988 types-pyinstaller-5.9.0.1/PyInstaller-stubs/lib/modulegraph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pyinstaller-5.9.0.1/PyInstaller-stubs/lib/modulegraph/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-03-27 18:21:24.000000 types-pyinstaller-5.9.0.1/PyInstaller-stubs/lib/modulegraph/modulegraph.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:41.283988 types-pyinstaller-5.9.0.1/PyInstaller-stubs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pyinstaller-5.9.0.1/PyInstaller-stubs/utils/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:41.283988 types-pyinstaller-5.9.0.1/PyInstaller-stubs/utils/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-03-27 18:21:24.000000 types-pyinstaller-5.9.0.1/PyInstaller-stubs/utils/hooks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-03-27 18:21:24.000000 types-pyinstaller-5.9.0.1/PyInstaller-stubs/utils/hooks/conda.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-27 18:21:24.000000 types-pyinstaller-5.9.0.1/PyInstaller-stubs/utils/hooks/win32.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:41.283988 types-pyinstaller-5.9.0.1/pyi_splash-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-27 18:25:40.000000 types-pyinstaller-5.9.0.1/pyi_splash-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-27 18:21:24.000000 types-pyinstaller-5.9.0.1/pyi_splash-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:25:41.283988 types-pyinstaller-5.9.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-03-27 18:25:40.000000 types-pyinstaller-5.9.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:41.283988 types-pyinstaller-5.9.0.1/types_pyinstaller.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-03-27 18:25:41.000000 types-pyinstaller-5.9.0.1/types_pyinstaller.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-03-27 18:25:41.000000 types-pyinstaller-5.9.0.1/types_pyinstaller.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:25:41.000000 types-pyinstaller-5.9.0.1/types_pyinstaller.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-27 18:25:41.000000 types-pyinstaller-5.9.0.1/types_pyinstaller.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-27 18:25:41.000000 types-pyinstaller-5.9.0.1/types_pyinstaller.egg-info/top_level.txt
```

### Comparing `types-pyinstaller-5.9.0.0/CHANGELOG.md` & `types-pyinstaller-5.9.0.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 5.9.0.1 (2023-03-27)
+
+Add default values for third-party stubs beginning with 'P' (#9957)
+
 ## 5.9.0.0 (2023-03-14)
 
 [stubsabot] Bump pyinstaller to 5.9.* (#9880)
 
 Release: https://pypi.org/pypi/pyinstaller/5.9.0
 Homepage: https://www.pyinstaller.org/
 Diff: https://github.com/pyinstaller/pyinstaller/compare/v5.8.0...v5.9.0
```

### Comparing `types-pyinstaller-5.9.0.0/PKG-INFO` & `types-pyinstaller-5.9.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyinstaller
-Version: 5.9.0.0
+Version: 5.9.0.1
 Summary: Typing stubs for pyinstaller
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyinstaller.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyinstaller`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyinstaller. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6d2d91c8f942efe5f7a00e1f5385d8d7a5a0a4e0`.
+This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
```

### Comparing `types-pyinstaller-5.9.0.0/PyInstaller-stubs/__main__.pyi` & `types-pyinstaller-5.9.0.1/PyInstaller-stubs/__main__.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-5.9.0.0/PyInstaller-stubs/building/build_main.pyi` & `types-pyinstaller-5.9.0.1/PyInstaller-stubs/building/build_main.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-5.9.0.0/PyInstaller-stubs/building/datastruct.pyi` & `types-pyinstaller-5.9.0.1/PyInstaller-stubs/building/datastruct.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-5.9.0.0/PyInstaller-stubs/compat.pyi` & `types-pyinstaller-5.9.0.1/PyInstaller-stubs/compat.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-5.9.0.0/PyInstaller-stubs/depend/analysis.pyi` & `types-pyinstaller-5.9.0.1/PyInstaller-stubs/depend/analysis.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # from altgraph.Graph import Graph
 _Graph: TypeAlias = Incomplete
 
 class PyiModuleGraph:  # incomplete
     def __init__(
         self,
         pyi_homepath: str,
-        user_hook_dirs: Iterable[StrPath] = ...,
-        excludes: Iterable[str] = ...,
+        user_hook_dirs: Iterable[StrPath] = (),
+        excludes: Iterable[str] = (),
         *,
         path: Iterable[str] | None = None,
         replace_paths: Iterable[tuple[StrPath, StrPath]] = ...,
         implies: SupportsKeysAndGetItem[str, _LazyNode] | Iterable[tuple[str, _LazyNode]] = ...,
         graph: _Graph | None = None,
         debug: bool = False,
     ) -> None: ...
```

### Comparing `types-pyinstaller-5.9.0.0/PyInstaller-stubs/depend/imphookapi.pyi` & `types-pyinstaller-5.9.0.1/PyInstaller-stubs/depend/imphookapi.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-5.9.0.0/PyInstaller-stubs/isolated/_parent.pyi` & `types-pyinstaller-5.9.0.1/PyInstaller-stubs/isolated/_parent.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-5.9.0.0/PyInstaller-stubs/lib/modulegraph/modulegraph.pyi` & `types-pyinstaller-5.9.0.1/PyInstaller-stubs/lib/modulegraph/modulegraph.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-5.9.0.0/PyInstaller-stubs/utils/hooks/__init__.pyi` & `types-pyinstaller-5.9.0.1/PyInstaller-stubs/utils/hooks/__init__.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,17 @@
 def collect_submodules(
     package: str, filter: Callable[[str], bool] = ..., on_error: Literal["ignore", "warn once", "warn", "raise"] = "warn once"
 ) -> list[str]: ...
 def is_module_or_submodule(name: str, mod_or_submod: str) -> bool: ...
 
 PY_DYLIB_PATTERNS: Final[list[str]]
 
-def collect_dynamic_libs(package: str, destdir: object = None, search_patterns: Iterable[str] = ...) -> list[tuple[str, str]]: ...
+def collect_dynamic_libs(
+    package: str, destdir: object = None, search_patterns: Iterable[str] = ["*.dll", "*.dylib", "lib*.so"]
+) -> list[tuple[str, str]]: ...
 def collect_data_files(
     package: str,
     include_py_files: bool = False,
     subdir: StrPath | None = None,
     excludes: Iterable[str] | None = None,
     includes: Iterable[str] | None = None,
 ) -> list[tuple[str, str]]: ...
```

### Comparing `types-pyinstaller-5.9.0.0/PyInstaller-stubs/utils/hooks/conda.pyi` & `types-pyinstaller-5.9.0.1/PyInstaller-stubs/utils/hooks/conda.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-5.9.0.0/setup.py` & `types-pyinstaller-5.9.0.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,32 +12,32 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyinstaller`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyinstaller. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6d2d91c8f942efe5f7a00e1f5385d8d7a5a0a4e0`.
+This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
 '''.lstrip()
 
 setup(name=name,
-      version="5.9.0.0",
+      version="5.9.0.1",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyinstaller.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=['types-setuptools'],
-      packages=['PyInstaller-stubs', 'pyi_splash-stubs'],
-      package_data={'PyInstaller-stubs': ['__init__.pyi', '__main__.pyi', 'building/__init__.pyi', 'building/build_main.pyi', 'building/datastruct.pyi', 'compat.pyi', 'depend/__init__.pyi', 'depend/analysis.pyi', 'depend/imphookapi.pyi', 'isolated/__init__.pyi', 'isolated/_parent.pyi', 'lib/__init__.pyi', 'lib/modulegraph/__init__.pyi', 'lib/modulegraph/modulegraph.pyi', 'utils/__init__.pyi', 'utils/hooks/__init__.pyi', 'utils/hooks/conda.pyi', 'utils/hooks/win32.pyi', 'METADATA.toml'], 'pyi_splash-stubs': ['__init__.pyi', 'METADATA.toml']},
+      packages=['pyi_splash-stubs', 'PyInstaller-stubs'],
+      package_data={'pyi_splash-stubs': ['__init__.pyi', 'METADATA.toml'], 'PyInstaller-stubs': ['__init__.pyi', '__main__.pyi', 'building/__init__.pyi', 'building/build_main.pyi', 'building/datastruct.pyi', 'compat.pyi', 'depend/__init__.pyi', 'depend/analysis.pyi', 'depend/imphookapi.pyi', 'isolated/__init__.pyi', 'isolated/_parent.pyi', 'lib/__init__.pyi', 'lib/modulegraph/__init__.pyi', 'lib/modulegraph/modulegraph.pyi', 'utils/__init__.pyi', 'utils/hooks/__init__.pyi', 'utils/hooks/conda.pyi', 'utils/hooks/win32.pyi', 'METADATA.toml']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-pyinstaller-5.9.0.0/types_pyinstaller.egg-info/PKG-INFO` & `types-pyinstaller-5.9.0.1/types_pyinstaller.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyinstaller
-Version: 5.9.0.0
+Version: 5.9.0.1
 Summary: Typing stubs for pyinstaller
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyinstaller.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyinstaller`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyinstaller. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6d2d91c8f942efe5f7a00e1f5385d8d7a5a0a4e0`.
+This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
```

### Comparing `types-pyinstaller-5.9.0.0/types_pyinstaller.egg-info/SOURCES.txt` & `types-pyinstaller-5.9.0.1/types_pyinstaller.egg-info/SOURCES.txt`

 * *Files identical despite different names*

