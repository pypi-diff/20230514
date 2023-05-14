# Comparing `tmp/omnidep-0.3.4.tar.gz` & `tmp/omnidep-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnidep-0.3.4.tar", max compression
+gzip compressed data, was "omnidep-0.3.5.tar", max compression
```

## Comparing `omnidep-0.3.4.tar` & `omnidep-0.3.5.tar`

### file list

```diff
@@ -1,25 +1,47 @@
--rw-r--r--   0        0        0     1069 2022-06-11 17:48:28.000000 omnidep-0.3.4/LICENSE
--rw-r--r--   0        0        0        0 2022-06-11 16:57:02.840000 omnidep-0.3.4/omnidep/__init__.py
--rw-r--r--   0        0        0       90 2023-04-07 18:02:26.000000 omnidep-0.3.4/omnidep/__main__.py
--rw-r--r--   0        0        0     5128 2022-12-13 00:57:08.000000 omnidep-0.3.4/omnidep/command.py
--rw-r--r--   0        0        0     3349 2022-11-29 18:45:06.000000 omnidep-0.3.4/omnidep/errors.py
--rw-r--r--   0        0        0     2083 2022-06-12 12:45:12.000000 omnidep-0.3.4/omnidep/imports.py
--rw-r--r--   0        0        0     1413 2023-04-07 18:02:26.000000 omnidep-0.3.4/omnidep/main.py
--rw-r--r--   0        0        0     3046 2022-11-28 18:05:04.000000 omnidep-0.3.4/omnidep/packages.py
--rw-r--r--   0        0        0     7620 2023-04-07 18:02:26.000000 omnidep-0.3.4/omnidep/project.py
--rw-r--r--   0        0        0        0 2022-11-28 18:05:02.570000 omnidep-0.3.4/omnidep/tst/__init__.py
--rw-r--r--   0        0        0     9636 2022-12-24 13:36:52.000000 omnidep-0.3.4/omnidep/tst/errors_test.py
--rw-r--r--   0        0        0     1504 2022-06-12 12:45:12.000000 omnidep-0.3.4/omnidep/tst/imports_test.py
--rw-r--r--   0        0        0     2602 2022-06-11 17:48:28.000000 omnidep-0.3.4/omnidep/tst/packages_test.py
--rw-r--r--   0        0        0     1692 2022-12-24 13:49:46.000000 omnidep-0.3.4/omnidep/tst/project_test.py
--rw-r--r--   0        0        0      314 2022-10-07 14:23:06.000000 omnidep-0.3.4/omnidep/tst/test_cases/case_insensitive_sorted/pyproject.toml
--rw-r--r--   0        0        0      314 2022-10-07 14:23:06.000000 omnidep-0.3.4/omnidep/tst/test_cases/case_sensitive_sorted/pyproject.toml
--rw-r--r--   0        0        0      257 2022-12-13 00:37:56.000000 omnidep-0.3.4/omnidep/tst/test_cases/dependency_in_test_code/pyproject.toml
--rw-r--r--   0        0        0      138 2022-12-13 01:05:38.000000 omnidep-0.3.4/omnidep/tst/test_cases/dependency_in_test_code/tests/test_code.py
--rw-r--r--   0        0        0      291 2022-11-29 18:45:06.000000 omnidep-0.3.4/omnidep/tst/test_cases/dev_dependencies_new/pyproject.toml
--rw-r--r--   0        0        0      285 2022-11-29 18:45:06.000000 omnidep-0.3.4/omnidep/tst/test_cases/dev_dependencies_old/pyproject.toml
--rw-r--r--   0        0        0     2266 2022-06-11 17:48:28.000000 omnidep-0.3.4/omnidep/tst/test_cases/every_import.py~
--rw-r--r--   0        0        0      293 2022-10-07 14:23:06.000000 omnidep-0.3.4/omnidep/tst/test_cases/unsorted/pyproject.toml
--rw-r--r--   0        0        0     1529 2023-04-07 18:02:26.000000 omnidep-0.3.4/pyproject.toml
--rw-r--r--   0        0        0    13401 2023-04-07 18:02:26.000000 omnidep-0.3.4/README.rst
--rw-r--r--   0        0        0    14216 1970-01-01 00:00:00.000000 omnidep-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-06-11 17:48:28.000000 omnidep-0.3.5/LICENSE
+-rw-r--r--   0        0        0        0 2022-06-11 16:57:02.840000 omnidep-0.3.5/omnidep/__init__.py
+-rw-r--r--   0        0        0       90 2023-05-14 16:28:24.000000 omnidep-0.3.5/omnidep/__main__.py
+-rw-r--r--   0        0        0     4921 2023-05-13 16:25:24.000000 omnidep-0.3.5/omnidep/command.py
+-rw-r--r--   0        0        0     3348 2023-05-13 16:25:26.000000 omnidep-0.3.5/omnidep/errors.py
+-rw-r--r--   0        0        0     2142 2023-05-14 15:03:32.000000 omnidep-0.3.5/omnidep/imports.py
+-rw-r--r--   0        0        0     1406 2023-05-13 16:25:26.000000 omnidep-0.3.5/omnidep/main.py
+-rw-r--r--   0        0        0     3203 2023-05-14 16:43:54.000000 omnidep-0.3.5/omnidep/packages.py
+-rw-r--r--   0        0        0     7719 2023-05-14 16:43:54.000000 omnidep-0.3.5/omnidep/project.py
+-rw-r--r--   0        0        0        0 2022-11-28 18:05:02.570000 omnidep-0.3.5/omnidep/tst/__init__.py
+-rw-r--r--   0        0        0     9636 2022-12-24 13:36:52.000000 omnidep-0.3.5/omnidep/tst/errors_test.py
+-rw-r--r--   0        0        0     1504 2022-06-12 12:45:12.000000 omnidep-0.3.5/omnidep/tst/imports_test.py
+-rw-r--r--   0        0        0     2602 2022-06-11 17:48:28.000000 omnidep-0.3.5/omnidep/tst/packages_test.py
+-rw-r--r--   0        0        0     2636 2023-05-14 15:03:34.000000 omnidep-0.3.5/omnidep/tst/project_test.py
+-rw-r--r--   0        0        0      314 2022-10-07 14:23:06.000000 omnidep-0.3.5/omnidep/tst/test_cases/case_insensitive_sorted/pyproject.toml
+-rw-r--r--   0        0        0      314 2022-10-07 14:23:06.000000 omnidep-0.3.5/omnidep/tst/test_cases/case_sensitive_sorted/pyproject.toml
+-rw-r--r--   0        0        0      273 2023-05-14 15:03:34.000000 omnidep-0.3.5/omnidep/tst/test_cases/dependency_in_test_code/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-08 13:11:17.810000 omnidep-0.3.5/omnidep/tst/test_cases/dependency_in_test_code/tests/__init__.py
+-rw-r--r--   0        0        0      398 2023-05-14 15:03:34.000000 omnidep-0.3.5/omnidep/tst/test_cases/dependency_in_test_code/tests/test_code.py
+-rw-r--r--   0        0        0      291 2022-11-29 18:45:06.000000 omnidep-0.3.5/omnidep/tst/test_cases/dev_dependencies_new/pyproject.toml
+-rw-r--r--   0        0        0      285 2022-11-29 18:45:06.000000 omnidep-0.3.5/omnidep/tst/test_cases/dev_dependencies_old/pyproject.toml
+-rw-r--r--   0        0        0     2266 2022-06-11 17:48:28.000000 omnidep-0.3.5/omnidep/tst/test_cases/every_import.py~
+-rw-r--r--   0        0        0        0 2023-05-14 15:03:33.360000 omnidep-0.3.5/omnidep/tst/test_cases/failed_import/failed_import/__init__.py
+-rw-r--r--   0        0        0      157 2023-05-14 15:03:34.000000 omnidep-0.3.5/omnidep/tst/test_cases/failed_import/failed_import/code.py
+-rw-r--r--   0        0        0      218 2023-05-14 15:03:34.000000 omnidep-0.3.5/omnidep/tst/test_cases/failed_import/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-14 15:03:34.950000 omnidep-0.3.5/omnidep/tst/test_cases/failed_import_but_ignored/failed_import/__init__.py
+-rw-r--r--   0        0        0      157 2023-05-14 15:03:36.000000 omnidep-0.3.5/omnidep/tst/test_cases/failed_import_but_ignored/failed_import/code.py
+-rw-r--r--   0        0        0      270 2023-05-14 15:03:36.000000 omnidep-0.3.5/omnidep/tst/test_cases/failed_import_but_ignored/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-14 15:03:35.090000 omnidep-0.3.5/omnidep/tst/test_cases/namespace_none_declared/namespace_code/__init__.py
+-rw-r--r--   0        0        0      170 2023-05-14 15:03:36.000000 omnidep-0.3.5/omnidep/tst/test_cases/namespace_none_declared/namespace_code/code.py
+-rw-r--r--   0        0        0      219 2023-05-14 15:03:36.000000 omnidep-0.3.5/omnidep/tst/test_cases/namespace_none_declared/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-14 15:03:35.180000 omnidep-0.3.5/omnidep/tst/test_cases/namespace_one_declared/namespace_code/__init__.py
+-rw-r--r--   0        0        0      170 2023-05-14 15:03:36.000000 omnidep-0.3.5/omnidep/tst/test_cases/namespace_one_declared/namespace_code/code.py
+-rw-r--r--   0        0        0      244 2023-05-14 15:03:36.000000 omnidep-0.3.5/omnidep/tst/test_cases/namespace_one_declared/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-14 15:03:35.290000 omnidep-0.3.5/omnidep/tst/test_cases/namespace_three_declared/namespace_code/__init__.py
+-rw-r--r--   0        0        0      170 2023-05-14 15:03:36.000000 omnidep-0.3.5/omnidep/tst/test_cases/namespace_three_declared/namespace_code/code.py
+-rw-r--r--   0        0        0      309 2023-05-14 15:03:36.000000 omnidep-0.3.5/omnidep/tst/test_cases/namespace_three_declared/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-14 15:03:35.320000 omnidep-0.3.5/omnidep/tst/test_cases/parent_child_configured/parent_child/__init__.py
+-rw-r--r--   0        0        0      237 2023-05-14 15:03:36.000000 omnidep-0.3.5/omnidep/tst/test_cases/parent_child_configured/parent_child/code.py
+-rw-r--r--   0        0        0      298 2023-05-14 15:03:36.000000 omnidep-0.3.5/omnidep/tst/test_cases/parent_child_configured/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-14 15:03:35.390000 omnidep-0.3.5/omnidep/tst/test_cases/parent_child_misconfigured/parent_child/__init__.py
+-rw-r--r--   0        0        0      237 2023-05-14 15:03:36.000000 omnidep-0.3.5/omnidep/tst/test_cases/parent_child_misconfigured/parent_child/code.py
+-rw-r--r--   0        0        0      367 2023-05-14 15:03:36.000000 omnidep-0.3.5/omnidep/tst/test_cases/parent_child_misconfigured/pyproject.toml
+-rw-r--r--   0        0        0      293 2022-10-07 14:23:06.000000 omnidep-0.3.5/omnidep/tst/test_cases/unsorted/pyproject.toml
+-rw-r--r--   0        0        0     3069 2023-05-14 16:48:04.000000 omnidep-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0    13567 2023-05-14 16:49:04.000000 omnidep-0.3.5/README.rst
+-rw-r--r--   0        0        0    14516 1970-01-01 00:00:00.000000 omnidep-0.3.5/PKG-INFO
```

### Comparing `omnidep-0.3.4/LICENSE` & `omnidep-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `omnidep-0.3.4/omnidep/command.py` & `omnidep-0.3.5/omnidep/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,41 +78,42 @@
             key = orig_key.replace('-', '_')
             # Warn for typos or misunderstandings. Also rejects options from
             # future versions of the code. That's OK because the same project
             # file containing the options can require a version of omnidep that
             # supports them.
             if key not in allowed:
                 raise ConfigError(f"Config option {orig_key!r} not recognised")
-            # Try to give a useful error message for misconfigurations.
-            # Not many types needed, so just hack them rather than add a
-            # dependency on pydantic.
-            check: Dict[str, Callable[[object], bool]]
-            check = {
-                'bool': lambda val: isinstance(val, bool),
-                'List[str]': lambda val: (
-                    isinstance(val, list) and
-                    all(isinstance(x, str) for x in val)
-                ),
-                'List[Path]': lambda val: (
-                    isinstance(val, list) and
-                    all(isinstance(x, str) for x in val)
-                ),
-                'Dict[str, List[str]]': lambda val: (
-                    isinstance(val, dict) and
-                    all(isinstance(key, str) for key in val) and
-                    all(map(check['List[str]'], val.values()))
-                ),
-            }
             convert: Dict[str, Callable[[Any], Any]] = {
                 'List[Path]': lambda val: list(map(Path, val))
             }
             # It already is a str due to "import annotations". But mypy doesn't
             # seem to know that, so coerce it.
             expected_type = str(allowed[key].type)
-            if not check[expected_type](value):
+            # Try to give a useful error message for misconfigurations.
+            if not check_type[expected_type](value):
                 raise ConfigError(f"Config option {orig_key!r}: expected {expected_type}, got {value!r}")
             converter = convert.get(expected_type, lambda x: x)
             args[key] = converter(value)
         if 'local_test_paths' in args and toml_file:
             new_paths = [toml_file.parent / path for path in args['local_test_paths']]
             args['local_test_paths'] = new_paths
         return Config(**args)
+
+# Not many types needed, so just hack them rather than add a
+# dependency on pydantic.
+check_type: Dict[str, Callable[[object], bool]]
+check_type = {
+    'bool': lambda val: isinstance(val, bool),
+    'List[str]': lambda val: (
+        isinstance(val, list) and
+        all(isinstance(x, str) for x in val)
+    ),
+    'List[Path]': lambda val: (
+        isinstance(val, list) and
+        all(isinstance(x, str) for x in val)
+    ),
+    'Dict[str, List[str]]': lambda val: (
+        isinstance(val, dict) and
+        all(isinstance(key, str) for key in val) and
+        all(map(check_type['List[str]'], val.values()))
+    ),
+}
```

### Comparing `omnidep-0.3.4/omnidep/errors.py` & `omnidep-0.3.5/omnidep/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     def set(self, value: U) -> Warned[U]:
         """Set a new value without changing the warnings"""
         return Warned(value, self.warnings)
 
     def warn(self, warning: Warn) -> Warned[T]:
         """Append one warning without changing the value"""
         # This is like the function tell of cats.Writer
-        return Warned(self.value, self.warnings + (warning,))
+        return Warned(self.value, (*self.warnings, warning))
     def warnAll(self, warnings: Iterable[Warn]) -> Warned[T]:
         """Append any number of warnings without changing the value"""
         return Warned(self.value, self.warnings + tuple(warnings))
 
     def as_tuple(self) -> Tuple[T, Tuple[Warn, ...]]:
         """Return (value, warnings)"""
         return self.value, self.warnings
```

### Comparing `omnidep-0.3.4/omnidep/imports.py` & `omnidep-0.3.5/omnidep/imports.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,36 +22,37 @@
         elif node is None:
             pass
         elif isinstance(node, list):
             to_process.extend(node)
         elif isinstance(node, ast.AST):
             to_process.extend(getattr(node, name) for name in node._fields)
         elif not isinstance(node, basic_types):
-            raise NotImplementedError(f'unhandled {type(node)} {node!r}')
+            raise NotImplementedError(f"unhandled {type(node)} {node!r}")
 
 def find_source_files(path: Path) -> Iterable[Path]:
     if path.is_file() and path.suffix == '.py':
         return [path]
     return path.glob('**/*.py')
 
 def iter_modules(path: Path) -> Iterable[str]:
     for file in find_source_files(path):
-        with open(file, encoding='utf8') as infile:
+        with file.open(encoding='utf8') as infile:
             # print(file)
             tree = ast.parse(infile.read())
             yield from iter_import_names(tree)
 
 def is_external(module: str) -> bool:
     if module in ('setuptools', 'pkg_resources'):
         # Debateable: not technically part of Python, but distributed with it.
         return False
     if sys.version_info >= (3, 10):
         if module == '__future__':
             return False
         return module not in sys.stdlib_module_names
-    else:
+    else:  # noqa: RET505: disagrees with mypy
+        # Older Python
         from isort import place_module
         return str(place_module(module)) not in ('STDLIB', 'FUTURE')
 
 def get_external_modules(paths: Iterable[Path]) -> List[str]:
     all_modules = itertools.chain.from_iterable(map(iter_modules, paths))
     return sorted(set(filter(is_external, all_modules)))
```

### Comparing `omnidep-0.3.4/omnidep/main.py` & `omnidep-0.3.5/omnidep/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,24 +27,24 @@
         .collect(lambda x: x.check_dev_dependencies(args.tests))
     ).warnings
 
     if warnings:
         print('\n'.join(w.report for w in warnings))
         print("See https://github.com/sjjessop/omnidep#error-codes-explained")
         return 1
-    else:
-        logger.info("No issues found")
-        return 0
+
+    logger.info("No issues found")
+    return 0
 
 def script_entry_point() -> NoReturn:
     args = CommandLine.parse()
     if args.log_level is not None:
         logging.basicConfig(level=args.log_level)
     try:
         raise SystemExit(main(args))
     except ConfigError as e:
-        raise SystemExit(str(e))
+        raise SystemExit(str(e)) from None
     finally:
         print("")
 
 if __name__ == '__main__':
     script_entry_point()
```

### Comparing `omnidep-0.3.4/omnidep/packages.py` & `omnidep-0.3.5/omnidep/packages.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,38 +3,44 @@
 import contextlib
 import functools
 from pathlib import Path
 import re
 import sys
 from typing import FrozenSet, List, Mapping, Optional
 
-import importlib_metadata as metadata
+if sys.version_info < (3, 8):
+    import importlib_metadata as metadata
+else:
+    from importlib import metadata
 
 from .errors import Violation as V
 from .errors import Warned
 
 punctuation = re.compile(r'[\-._]+')
 
 # In Python 3.9+, should use functools.cache instead of lru_cache
 # In Python 3.10+, there is metadata.packages_distributions, but all it checks
 # is top_level.txt, so we still need to search for files as well.
 @functools.lru_cache()
 def packages_distributions() -> Mapping[str, List[str]]:
     pkg_to_dist = collections.defaultdict(set)
     for dist in metadata.distributions():
+        dist_name = dist.metadata['Name']
         def add_to(pkg: str) -> None:
-            pkg_to_dist[pkg].add(dist.metadata['Name'])
+            pkg_to_dist[pkg].add(dist_name)
         for toplevel in (dist.read_text('top_level.txt') or '').split():
             add_to(toplevel)
         for file in dist.files or ():
             # TODO - maybe the package could contain .pyc or .pyd but no .py
             if file.name == '__init__.py':
                 add_to(str(file.parent))
             elif str(file.parent) == '.' and file.suffix == '.py':
                 add_to(file.stem)
+            else:
+                add_to(file.parts[0])
     # TODO - make the return immutable, since it's cached
     return {key: sorted(value) for key, value in pkg_to_dist.items()}
 
 def find_packages(module: str, local_packages: FrozenSet[str]) -> Warned[List[str]]:
     """
     Given a top-level code module, which installed package(s) provide it?
     This is a difficult question because Python packaging doesn't try to fully
@@ -50,15 +56,15 @@
     package = packages_distributions().get(module)
     if package is not None:
         return Warned(list(package))
     # Maybe the package is on the path, in which case no package dependency is
     # needed provided that it remains available on the path.
     if any((Path(path) / module).is_dir() for path in sys.path):
         return Warned([module]).warn(
-            V.ODEP008(f'Module {module!r} not under package management but found on python path')
+            V.ODEP008(f"Module {module!r} not under package management but found on python path")
         )
     return Warned([])
 
 def canon(package_name: str) -> str:
     """
     Return the normalized name per PEP 503:
     https://peps.python.org/pep-0503/#normalized-names
@@ -68,10 +74,10 @@
 def get_preferred_name(package: str) -> Optional[str]:
     """
     Return the name the project calls itself.
     """
     # importlib_metadata.PackageNotFoundError inherits from FileNotFoundError
     # in old versions (<3) and ImportError more recently.
     with contextlib.suppress(FileNotFoundError, ImportError):
-        name: Optional[str] = metadata.distribution(package).metadata.get('Name')
+        name: Optional[str] = metadata.distribution(package).metadata['Name']
         return name
     return None
```

### Comparing `omnidep-0.3.4/omnidep/project.py` & `omnidep-0.3.5/omnidep/project.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 
 from __future__ import annotations
 
 from dataclasses import dataclass
 import itertools
 import logging
 from pathlib import Path
+import sys
 from typing import (
     Any, Collection, Container, Dict, FrozenSet, Iterable, Optional, Set,
     Tuple,
 )
 
-import tomli
+if sys.version_info >= (3, 11):
+    import tomllib
+else:
+    import tomli as tomllib
 
 from .command import Config
 from .errors import Violation as V
 from .errors import Warn, Warned
 from .imports import find_source_files, get_external_modules
 from .packages import canon, find_packages, get_preferred_name
 
@@ -78,33 +82,33 @@
         )
 
     def check_modules(
         self, paths: Iterable[Path], packages: Collection[str], local_packages: FrozenSet[str],
         *, label: str = 'dependencies', check_unused: bool = True, exclude: Iterable[Path] = (),
     ) -> Iterable[Warn]:
         paths = list(paths)
-        logger.info(f'searching {", ".join(map(str, paths))}')
+        logger.info(f"searching {', '.join(map(str, paths))}")
         def get_files(paths: Iterable[Path]) -> Set[Path]:
             return set(itertools.chain.from_iterable(map(find_source_files, paths)))
         included_paths = get_files(paths) - get_files(exclude)
         modules = [
             module for module in get_external_modules(included_paths)
             if not self.ignore_import(module)
         ]
-        logger.info(f'{label} imported: {modules}')
+        logger.info(f"{label} imported: {modules}")
         used: Set[str] = {'python'}
         for module in modules:
             founds = find_packages(module, local_packages)
             yield from founds.warnings
             found = list(map(canon, founds.value))
             if len(found) == 1:
                 package = found[0]
                 used.add(package)
                 if package not in local_packages and not self.required(package, packages):
-                    yield V.ODEP001(f'Package {package!r} is imported but not listed in {label}', package)
+                    yield V.ODEP001(f"Package {package!r} is imported but not listed in {label}", package)
             elif len(found) == 0:
                 yield V.ODEP002(f"Module {module!r} is imported but not installed, so I don't know what package is needed", module)
             else:
                 # Namespace package - implemented across multiple installed
                 # packages. So for any given import, we don't know which
                 # package supplies that part of the namespace package.
                 options = [pkg in local_packages or self.required(pkg, packages) for pkg in found]
@@ -115,15 +119,15 @@
                     yield V.ODEP003(f"Namespace package found: any of {found} might provide {module!r}")
                     used.update(found)
                 else:
                     yield V.ODEP004(f"Namespace package found: any of {found} might provide {module!r}, and there are no dependencies on any of them", module)
         if check_unused:
             unused = set(packages) - used - set(self.config.ignore_dependencies)
             if unused:
-                yield V.ODEP005(f'Unused {label} in project file: {sorted(unused)}')
+                yield V.ODEP005(f"Unused {label} in project file: {sorted(unused)}")
 
     def ignore_import(self, module: str) -> bool:
         return bool(self.config) and module in self.config.ignore_imports
 
     def required(self, package: str, packages: Container[str]) -> bool:
         def mentioned(pkg: str) -> bool:
             return pkg in packages or pkg in self.local_packages
@@ -134,38 +138,38 @@
                 return True
         return False
 
 def read_poetry(toml_file: Optional[Path]) -> Warned[Project]:
     if toml_file is None:
         logger.error("pyproject.toml not specified")
         return Warned(Project((), (), Config.make()))
-    with open(toml_file, 'rb') as infile:
-        tools = tomli.load(infile)['tool']
+    with toml_file.open('rb') as infile:
+        tools = tomllib.load(infile)['tool']
     poetry_data = tools['poetry']
     config = Config.make(tools.get('omnidep'), toml_file)
 
-    def process(deps: Dict[str, Any], dev: bool) -> Warned[FrozenSet[str]]:
+    def process(deps: Dict[str, Any], *, dev: bool) -> Warned[FrozenSet[str]]:
         if dev:
             ignore = config.ignore_dev_dependencies_order
             key = 'dev-dependencies'
         else:
             ignore = config.ignore_dependencies_order
             key = 'dependencies'
         return (
             Warned(deps)
             .collect(lambda x: () if ignore else check_order(x, key))
             .flatMap(fix_canonical_names)
         )
 
-    deps = process(poetry_data['dependencies'], False)
+    deps = process(poetry_data['dependencies'], dev=False)
     # Poetry 1.2.0+ has two different places you can specify dev dependencies
     old_dev_data = poetry_data.get('dev-dependencies', {})
-    old_dev_deps = process(old_dev_data, True)
+    old_dev_deps = process(old_dev_data, dev=True)
     new_dev_data = poetry_data.get('group', {}).get('dev', {}).get('dependencies', {})
-    new_dev_deps = process(new_dev_data, True)
+    new_dev_deps = process(new_dev_data, dev=True)
     dev_deps: Warned[FrozenSet[str]] = (
         Warned.gather([old_dev_deps, new_dev_deps])
         .map(lambda x: frozenset(itertools.chain.from_iterable(x)))
     )
 
     pkgs = {pack['include'] for pack in poetry_data['packages']}
     project = Project(
```

### Comparing `omnidep-0.3.4/omnidep/tst/errors_test.py` & `omnidep-0.3.5/omnidep/tst/errors_test.py`

 * *Files identical despite different names*

### Comparing `omnidep-0.3.4/omnidep/tst/imports_test.py` & `omnidep-0.3.5/omnidep/tst/imports_test.py`

 * *Files identical despite different names*

### Comparing `omnidep-0.3.4/omnidep/tst/packages_test.py` & `omnidep-0.3.5/omnidep/tst/packages_test.py`

 * *Files identical despite different names*

### Comparing `omnidep-0.3.4/omnidep/tst/test_cases/every_import.py~` & `omnidep-0.3.5/omnidep/tst/test_cases/every_import.py~`

 * *Files identical despite different names*

### Comparing `omnidep-0.3.4/README.rst` & `omnidep-0.3.5/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 A Python linter to compare a project's declared dependencies against the import
 statements in its source code.
 
 .. image:: https://github.com/sjjessop/omnidep/workflows/tests/badge.svg?branch=develop
    :alt: Test status
    :target: https://github.com/sjjessop/omnidep/actions?query=workflow%3Atests+branch%3Adevelop
 
-.. image:: https://img.shields.io/badge/CI%20python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg
+.. image:: https://img.shields.io/badge/Tested%20python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg
    :alt: Tested with Python versions 3.7 3.8 3.9 3.10 3.11
    :target: https://www.python.org/downloads/
 
 .. image:: https://img.shields.io/pypi/pyversions/omnidep
    :alt: PyPI project
    :target: https://pypi.org/project/omnidep/
 
@@ -40,15 +40,15 @@
 
 Optionally, you can also run the test suite. This would be a good idea if
 you're using a new (or pre-release) version of Python not included in this
 repo's CI testing.
 
 .. code-block:: bash
 
-    pip install pyOpenSSL pytest
+    pip install pyOpenSSL opentelemetry-api opentelemetry-sdk pytest
     pytest --pyargs omnidep.tst
 
 Usage
 -----
 
 .. code-block:: bash
 
@@ -325,25 +325,30 @@
 omnidep cannot find any project that provides X, but it is available to import.
 This can happen for example if you have set up the ``PYTHONPATH`` to find the
 code, instead of installing it as a dependency.
 
 To fix, choose one of the following:
 
 * If this is an error, list a suitable dependency.
-* If this occors when your test code is importing other modules also within
+* If this occurs when your test code is importing other modules also within
   your test code (for example helper utilities) then you can configure
   ``local-test-packages = ["X"]`` in your ``[tool.omnidep]`` config, and/or
   ``local-test-paths`` with the location of the test source.
 * If you know what you're doing, and users of your project will know how to
   supply the code that you're importing, then ignore the import with
   ``ignore-imports = ["X"]`` in your ``[tool.omnidep]`` config.
 
 Changelog
 =========
 
+0.3.5
+-----
+* No longer depends on importlib-metadata or tomli in Python versions that
+  have equivalent built-in libraries.
+
 0.3.4
 -----
 * Report unused dependencies as a sorted list
 * Allow `python -m omnidep` (https://github.com/sjjessop/omnidep/issues/2)
 
 0.3.3
 -----
```

### Comparing `omnidep-0.3.4/PKG-INFO` & `omnidep-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 Metadata-Version: 2.1
 Name: omnidep
-Version: 0.3.4
+Version: 0.3.5
 Summary: Linter to compare project dependencies against imports in source code
 Home-page: https://github.com/sjjessop/omnidep
 License: MIT
 Author: Steve Jessop
 Author-email: 68118527+sjjessop@users.noreply.github.com
 Requires-Python: >=3.7.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: importlib-metadata (>=1.1.0)
+Requires-Dist: importlib-metadata (>=1.1.0) ; python_version < "3.8"
 Requires-Dist: isort (>=5.0.1) ; python_version < "3.10"
-Requires-Dist: tomli (>=1.1.0)
+Requires-Dist: tomli (>=1.1.0) ; python_version < "3.11"
+Project-URL: Changelog, https://github.com/sjjessop/omnidep/tree/develop#changelog
 Description-Content-Type: text/x-rst
 
 =======
 Omnidep
 =======
 
 A Python linter to compare a project's declared dependencies against the import
 statements in its source code.
 
 .. image:: https://github.com/sjjessop/omnidep/workflows/tests/badge.svg?branch=develop
    :alt: Test status
    :target: https://github.com/sjjessop/omnidep/actions?query=workflow%3Atests+branch%3Adevelop
 
-.. image:: https://img.shields.io/badge/CI%20python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg
+.. image:: https://img.shields.io/badge/Tested%20python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg
    :alt: Tested with Python versions 3.7 3.8 3.9 3.10 3.11
    :target: https://www.python.org/downloads/
 
 .. image:: https://img.shields.io/pypi/pyversions/omnidep
    :alt: PyPI project
    :target: https://pypi.org/project/omnidep/
 
@@ -61,15 +62,15 @@
 
 Optionally, you can also run the test suite. This would be a good idea if
 you're using a new (or pre-release) version of Python not included in this
 repo's CI testing.
 
 .. code-block:: bash
 
-    pip install pyOpenSSL pytest
+    pip install pyOpenSSL opentelemetry-api opentelemetry-sdk pytest
     pytest --pyargs omnidep.tst
 
 Usage
 -----
 
 .. code-block:: bash
 
@@ -346,25 +347,30 @@
 omnidep cannot find any project that provides X, but it is available to import.
 This can happen for example if you have set up the ``PYTHONPATH`` to find the
 code, instead of installing it as a dependency.
 
 To fix, choose one of the following:
 
 * If this is an error, list a suitable dependency.
-* If this occors when your test code is importing other modules also within
+* If this occurs when your test code is importing other modules also within
   your test code (for example helper utilities) then you can configure
   ``local-test-packages = ["X"]`` in your ``[tool.omnidep]`` config, and/or
   ``local-test-paths`` with the location of the test source.
 * If you know what you're doing, and users of your project will know how to
   supply the code that you're importing, then ignore the import with
   ``ignore-imports = ["X"]`` in your ``[tool.omnidep]`` config.
 
 Changelog
 =========
 
+0.3.5
+-----
+* No longer depends on importlib-metadata or tomli in Python versions that
+  have equivalent built-in libraries.
+
 0.3.4
 -----
 * Report unused dependencies as a sorted list
 * Allow `python -m omnidep` (https://github.com/sjjessop/omnidep/issues/2)
 
 0.3.3
 -----
```

