# Comparing `tmp/jdfile-1.1.4.tar.gz` & `tmp/jdfile-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdfile-1.1.4.tar", max compression
+gzip compressed data, was "jdfile-1.1.5.tar", max compression
```

## Comparing `jdfile-1.1.4.tar` & `jdfile-1.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    34523 2023-03-31 17:32:56.771174 jdfile-1.1.4/LICENSE
--rw-r--r--   0        0        0     9107 2023-03-31 17:32:56.771174 jdfile-1.1.4/README.md
--rw-r--r--   0        0        0     7824 2023-03-31 17:32:56.771174 jdfile-1.1.4/pyproject.toml
--rw-r--r--   0        0        0       22 2023-03-31 17:32:56.771174 jdfile-1.1.4/src/jdfile/__init__.py
--rw-r--r--   0        0        0       44 2023-03-31 17:32:56.771174 jdfile-1.1.4/src/jdfile/__version__.py
--rw-r--r--   0        0        0       92 2023-03-31 17:32:56.771174 jdfile-1.1.4/src/jdfile/_config/__init__.py
--rw-r--r--   0        0        0    16081 2023-03-31 17:32:56.771174 jdfile-1.1.4/src/jdfile/_config/config.py
--rw-r--r--   0        0        0     2031 2023-03-31 17:32:56.771174 jdfile-1.1.4/src/jdfile/_config/default_config.toml
--rw-r--r--   0        0        0    11239 2023-03-31 17:32:56.771174 jdfile-1.1.4/src/jdfile/cli.py
--rw-r--r--   0        0        0       33 2023-03-31 17:32:56.771174 jdfile-1.1.4/src/jdfile/models/__init__.py
--rw-r--r--   0        0        0    21497 2023-03-31 17:32:56.771174 jdfile-1.1.4/src/jdfile/models/dates.py
--rw-r--r--   0        0        0    10890 2023-03-31 17:32:56.771174 jdfile-1.1.4/src/jdfile/models/file.py
--rw-r--r--   0        0        0    11190 2023-03-31 17:32:56.771174 jdfile-1.1.4/src/jdfile/models/project.py
--rw-r--r--   0        0        0       24 2023-03-31 17:32:56.771174 jdfile-1.1.4/src/jdfile/utils/__init__.py
--rw-r--r--   0        0        0     8035 2023-03-31 17:32:56.775174 jdfile-1.1.4/src/jdfile/utils/alerts.py
--rw-r--r--   0        0        0      101 2023-03-31 17:32:56.775174 jdfile-1.1.4/src/jdfile/utils/console.py
--rw-r--r--   0        0        0      690 2023-03-31 17:32:56.775174 jdfile-1.1.4/src/jdfile/utils/enums.py
--rw-r--r--   0        0        0     1596 2023-03-31 17:32:56.775174 jdfile-1.1.4/src/jdfile/utils/nltk.py
--rw-r--r--   0        0        0     1921 2023-03-31 17:32:56.775174 jdfile-1.1.4/src/jdfile/utils/questions.py
--rw-r--r--   0        0        0    25880 2023-03-31 17:32:56.775174 jdfile-1.1.4/src/jdfile/utils/strings.py
--rw-r--r--   0        0        0     4601 2023-03-31 17:32:56.775174 jdfile-1.1.4/src/jdfile/utils/utilities.py
--rw-r--r--   0        0        0     9943 1970-01-01 00:00:00.000000 jdfile-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-14 20:39:57.830863 jdfile-1.1.5/LICENSE
+-rw-r--r--   0        0        0     9107 2023-05-14 20:39:57.830863 jdfile-1.1.5/README.md
+-rw-r--r--   0        0        0     7823 2023-05-14 20:39:57.830863 jdfile-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-14 20:39:57.834863 jdfile-1.1.5/src/jdfile/__init__.py
+-rw-r--r--   0        0        0       44 2023-05-14 20:39:57.834863 jdfile-1.1.5/src/jdfile/__version__.py
+-rw-r--r--   0        0        0       92 2023-05-14 20:39:57.834863 jdfile-1.1.5/src/jdfile/_config/__init__.py
+-rw-r--r--   0        0        0    16081 2023-05-14 20:39:57.834863 jdfile-1.1.5/src/jdfile/_config/config.py
+-rw-r--r--   0        0        0     2031 2023-05-14 20:39:57.838863 jdfile-1.1.5/src/jdfile/_config/default_config.toml
+-rw-r--r--   0        0        0    11215 2023-05-14 20:39:57.838863 jdfile-1.1.5/src/jdfile/cli.py
+-rw-r--r--   0        0        0       33 2023-05-14 20:39:57.838863 jdfile-1.1.5/src/jdfile/models/__init__.py
+-rw-r--r--   0        0        0    21497 2023-05-14 20:39:57.838863 jdfile-1.1.5/src/jdfile/models/dates.py
+-rw-r--r--   0        0        0    10890 2023-05-14 20:39:57.838863 jdfile-1.1.5/src/jdfile/models/file.py
+-rw-r--r--   0        0        0    11190 2023-05-14 20:39:57.838863 jdfile-1.1.5/src/jdfile/models/project.py
+-rw-r--r--   0        0        0       24 2023-05-14 20:39:57.838863 jdfile-1.1.5/src/jdfile/utils/__init__.py
+-rw-r--r--   0        0        0     8035 2023-05-14 20:39:57.842863 jdfile-1.1.5/src/jdfile/utils/alerts.py
+-rw-r--r--   0        0        0      101 2023-05-14 20:39:57.842863 jdfile-1.1.5/src/jdfile/utils/console.py
+-rw-r--r--   0        0        0      694 2023-05-14 20:39:57.842863 jdfile-1.1.5/src/jdfile/utils/enums.py
+-rw-r--r--   0        0        0     1596 2023-05-14 20:39:57.842863 jdfile-1.1.5/src/jdfile/utils/nltk.py
+-rw-r--r--   0        0        0     1921 2023-05-14 20:39:57.842863 jdfile-1.1.5/src/jdfile/utils/questions.py
+-rw-r--r--   0        0        0    25880 2023-05-14 20:39:57.842863 jdfile-1.1.5/src/jdfile/utils/strings.py
+-rw-r--r--   0        0        0     4601 2023-05-14 20:39:57.842863 jdfile-1.1.5/src/jdfile/utils/utilities.py
+-rw-r--r--   0        0        0     9944 1970-01-01 00:00:00.000000 jdfile-1.1.5/PKG-INFO
```

### Comparing `jdfile-1.1.4/LICENSE` & `jdfile-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jdfile-1.1.4/README.md` & `jdfile-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `jdfile-1.1.4/pyproject.toml` & `jdfile-1.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,60 +6,60 @@
     authors     = ["Nate Landau <github@natenate.org>"]
     description = "File Manager for the Johnny Decimal System"
     homepage    = "https://github.com/natelandau/jdfile"
     license     = "GNU AFFERO"
     name        = "jdfile"
     readme      = "README.md"
     repository  = "https://github.com/natelandau/jdfile"
-    version     = "1.1.4"
+    version     = "1.1.5"
 
     [tool.poetry.scripts] # https://python-poetry.org/docs/pyproject/#scripts
         jdfile = "jdfile.cli:app"
 
     [tool.poetry.dependencies]
-        loguru      = "^0.6.0"
+        loguru      = "^0.7.0"
         nltk        = "^3.8.1"
         python      = "^3.10"
         questionary = "^1.10.0"
-        rich        = "^13.3.3"
+        rich        = "^13.3.5"
         shellingham = "^1.4.0"
         tomli       = "^2.0.1"
-        typer       = "^0.7.0"
+        typer       = "^0.9.0"
 
     [tool.poetry.group.test.dependencies]
-        hypothesis             = "^6.70.1"
-        pytest                 = "^7.2.2"
+        hypothesis             = "^6.75.2"
+        pytest                 = "^7.3.1"
         pytest-clarity         = "^1.0.1"
         pytest-mock            = "^3.10.0"
         pytest-pretty-terminal = "^1.1.0"
         pytest-xdist           = "^3.2.1"
 
     [tool.poetry.group.dev.dependencies]
         black                 = "^23.3.0"
-        commitizen            = "^2.42.1"
-        coverage              = "^7.2.2"
+        commitizen            = "^3.2.2"
+        coverage              = "^7.2.5"
         interrogate           = "^1.5.0"
-        mypy                  = "^1.1.1"
-        pdoc                  = "^13.1.0"
-        poethepoet            = "^0.19.0"
-        pre-commit            = "^3.2.1"
-        ruff                  = "^0.0.260"
+        mypy                  = "^1.3.0"
+        pdoc                  = "^13.1.1"
+        poethepoet            = "^0.20.0"
+        pre-commit            = "^3.3.1"
+        ruff                  = "^0.0.265"
         sh                    = "^2.0.3"
         shellcheck-py         = "^0.9.0.2"
-        typeguard             = "^3.0.2"
-        types-python-dateutil = "^2.8.19.11"
+        typeguard             = "^4.0.0"
+        types-python-dateutil = "^2.8.19.13"
         vulture               = "^2.7"
 
 [tool.black]
     line-length = 100
 [tool.commitizen]
     bump_message             = "bump(release): v$current_version → v$new_version"
     tag_format               = "v$version"
     update_changelog_on_bump = true
-    version                  = "1.1.4"
+    version                  = "1.1.5"
     version_files            = ["pyproject.toml:version", "src/jdfile/__version__.py:__version__"]
 
 [tool.coverage.report] # https://coverage.readthedocs.io/en/latest/config.html#report
     exclude_lines = [
         'def __repr__',
         'except [\w\s\._]+ as .*:',
         'log\.critical',
```

### Comparing `jdfile-1.1.4/src/jdfile/_config/config.py` & `jdfile-1.1.5/src/jdfile/_config/config.py`

 * *Files identical despite different names*

### Comparing `jdfile-1.1.4/src/jdfile/_config/default_config.toml` & `jdfile-1.1.5/src/jdfile/_config/default_config.toml`

 * *Files identical despite different names*

### Comparing `jdfile-1.1.4/src/jdfile/cli.py` & `jdfile-1.1.5/src/jdfile/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,20 +129,19 @@
         None,
         "--project",
         "-p",
         help="Specify a project from the configuration file.",
         rich_help_panel="File Organization Options",
     ),
     separator: Separator = typer.Option(
-        None,
+        "ignore",
         "--separator",
         case_sensitive=False,
         help="Word separator",
         rich_help_panel="Filename Cleaning Options",
-        show_default=False,
     ),
     split_words: bool = typer.Option(
         None,
         "--split-words/--no-split",
         help="Split words on capital letters",
         rich_help_panel="Filename Cleaning Options",
         show_default=True,
```

### Comparing `jdfile-1.1.4/src/jdfile/models/dates.py` & `jdfile-1.1.5/src/jdfile/models/dates.py`

 * *Files identical despite different names*

### Comparing `jdfile-1.1.4/src/jdfile/models/file.py` & `jdfile-1.1.5/src/jdfile/models/file.py`

 * *Files identical despite different names*

### Comparing `jdfile-1.1.4/src/jdfile/models/project.py` & `jdfile-1.1.5/src/jdfile/models/project.py`

 * *Files identical despite different names*

### Comparing `jdfile-1.1.4/src/jdfile/utils/alerts.py` & `jdfile-1.1.5/src/jdfile/utils/alerts.py`

 * *Files identical despite different names*

### Comparing `jdfile-1.1.4/src/jdfile/utils/enums.py` & `jdfile-1.1.5/src/jdfile/utils/enums.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     UPPER = "upper"
 
 
 class Separator(Enum):
     """Define choices for separator transformation."""
 
     DASH = "-"
-    IGNORE = None
+    IGNORE = "ignore"
     NONE = ""
     SPACE = " "
     UNDERSCORE = "_"
 
 
 class InsertLocation(Enum):
     """Define choices for inserting text."""
```

### Comparing `jdfile-1.1.4/src/jdfile/utils/nltk.py` & `jdfile-1.1.5/src/jdfile/utils/nltk.py`

 * *Files identical despite different names*

### Comparing `jdfile-1.1.4/src/jdfile/utils/questions.py` & `jdfile-1.1.5/src/jdfile/utils/questions.py`

 * *Files identical despite different names*

### Comparing `jdfile-1.1.4/src/jdfile/utils/strings.py` & `jdfile-1.1.5/src/jdfile/utils/strings.py`

 * *Files identical despite different names*

### Comparing `jdfile-1.1.4/src/jdfile/utils/utilities.py` & `jdfile-1.1.5/src/jdfile/utils/utilities.py`

 * *Files identical despite different names*

### Comparing `jdfile-1.1.4/PKG-INFO` & `jdfile-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: jdfile
-Version: 1.1.4
+Version: 1.1.5
 Summary: File Manager for the Johnny Decimal System
 Home-page: https://github.com/natelandau/jdfile
 License: GNU AFFERO
 Author: Nate Landau
 Author-email: github@natenate.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
-Requires-Dist: rich (>=13.3.3,<14.0.0)
+Requires-Dist: rich (>=13.3.5,<14.0.0)
 Requires-Dist: shellingham (>=1.4.0,<2.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
-Requires-Dist: typer (>=0.7.0,<0.8.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/natelandau/jdfile
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/jdfile.svg)](https://badge.fury.io/py/jdfile) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/jdfile) [![Python Code Checker](https://github.com/natelandau/jdfile/actions/workflows/automated-tests.yml/badge.svg)](https://github.com/natelandau/jdfile/actions/workflows/automated-tests.yml) [![codecov](https://codecov.io/gh/natelandau/jdfile/branch/main/graph/badge.svg?token=Y11Z883PMI)](https://codecov.io/gh/natelandau/jdfile)
 
 # jdfile
```

