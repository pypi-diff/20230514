# Comparing `tmp/jutility-0.0.5.tar.gz` & `tmp/jutility-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Jake\Documents\Programming\jutility\dist\.tmp-7_t82agc\jutility-0.0.5.tar", last modified: Sun May 14 17:29:19 2023, max compression
+gzip compressed data, was "C:\Users\Jake\Documents\Programming\jutility\dist\.tmp-dpalhca5\jutility-0.0.6.tar", last modified: Sun May 14 18:44:48 2023, max compression
```

## Comparing `jutility-0.0.5.tar` & `jutility-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 17:29:19.000000 jutility-0.0.5/
--rw-rw-rw-   0        0        0     1087 2023-05-13 21:09:33.000000 jutility-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     2826 2023-05-14 17:29:19.000000 jutility-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2225 2023-05-14 17:27:47.000000 jutility-0.0.5/README.md
--rw-rw-rw-   0        0        0      735 2023-05-14 17:27:41.000000 jutility-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-14 17:29:19.000000 jutility-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-14 17:29:19.000000 jutility-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-14 17:29:19.000000 jutility-0.0.5/src/jutility/
--rw-rw-rw-   0        0        0        0 2023-05-13 20:59:58.000000 jutility-0.0.5/src/jutility/__init__.py
--rw-rw-rw-   0        0        0    16333 2023-05-14 17:11:46.000000 jutility-0.0.5/src/jutility/plotting.py
--rw-rw-rw-   0        0        0    10048 2023-05-13 21:30:51.000000 jutility-0.0.5/src/jutility/sweep.py
--rw-rw-rw-   0        0        0    13209 2023-05-14 15:33:41.000000 jutility-0.0.5/src/jutility/util.py
-drwxrwxrwx   0        0        0        0 2023-05-14 17:29:19.000000 jutility-0.0.5/src/jutility.egg-info/
--rw-rw-rw-   0        0        0     2826 2023-05-14 17:29:19.000000 jutility-0.0.5/src/jutility.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2023-05-14 17:29:19.000000 jutility-0.0.5/src/jutility.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 17:29:19.000000 jutility-0.0.5/src/jutility.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-14 17:29:19.000000 jutility-0.0.5/src/jutility.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-14 17:29:19.000000 jutility-0.0.5/src/jutility.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-14 17:29:19.000000 jutility-0.0.5/tests/
--rw-rw-rw-   0        0        0     9100 2023-05-14 15:22:52.000000 jutility-0.0.5/tests/test_plotting.py
--rw-rw-rw-   0        0        0     9206 2023-05-13 21:45:28.000000 jutility-0.0.5/tests/test_sweep.py
--rw-rw-rw-   0        0        0    12140 2023-05-14 15:40:12.000000 jutility-0.0.5/tests/test_util.py
+drwxrwxrwx   0        0        0        0 2023-05-14 18:44:48.000000 jutility-0.0.6/
+-rw-rw-rw-   0        0        0     1087 2023-05-13 21:09:33.000000 jutility-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      343 2023-05-14 18:44:48.000000 jutility-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2235 2023-05-14 18:41:23.000000 jutility-0.0.6/README.md
+-rw-rw-rw-   0        0        0       90 2023-05-14 18:37:23.000000 jutility-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      445 2023-05-14 18:44:48.000000 jutility-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-14 18:44:48.000000 jutility-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-14 18:44:48.000000 jutility-0.0.6/src/jutility/
+-rw-rw-rw-   0        0        0        0 2023-05-13 20:59:58.000000 jutility-0.0.6/src/jutility/__init__.py
+-rw-rw-rw-   0        0        0    16333 2023-05-14 17:11:46.000000 jutility-0.0.6/src/jutility/plotting.py
+-rw-rw-rw-   0        0        0    10048 2023-05-13 21:30:51.000000 jutility-0.0.6/src/jutility/sweep.py
+-rw-rw-rw-   0        0        0    13209 2023-05-14 15:33:41.000000 jutility-0.0.6/src/jutility/util.py
+drwxrwxrwx   0        0        0        0 2023-05-14 18:44:48.000000 jutility-0.0.6/src/jutility.egg-info/
+-rw-rw-rw-   0        0        0      343 2023-05-14 18:44:48.000000 jutility-0.0.6/src/jutility.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2023-05-14 18:44:48.000000 jutility-0.0.6/src/jutility.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 18:44:48.000000 jutility-0.0.6/src/jutility.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-14 18:44:48.000000 jutility-0.0.6/src/jutility.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-14 18:44:48.000000 jutility-0.0.6/src/jutility.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 18:44:48.000000 jutility-0.0.6/tests/
+-rw-rw-rw-   0        0        0     9100 2023-05-14 15:22:52.000000 jutility-0.0.6/tests/test_plotting.py
+-rw-rw-rw-   0        0        0     9206 2023-05-13 21:45:28.000000 jutility-0.0.6/tests/test_sweep.py
+-rw-rw-rw-   0        0        0    12140 2023-05-14 15:40:12.000000 jutility-0.0.6/tests/test_util.py
```

### Comparing `jutility-0.0.5/LICENSE` & `jutility-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jutility-0.0.5/PKG-INFO` & `jutility-0.0.6/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,75 +1,61 @@
-Metadata-Version: 2.1
-Name: jutility
-Version: 0.0.5
-Summary: Collection of Python utilities intended to be useful for machine learning research and experiments
-Author-email: Jake Levi <jakelevi@hotmail.co.uk>
-License: MIT License
-Project-URL: homepage, https://github.com/jakelevi1996/jutility
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# jutility
-
-Collection of Python utilities intended to be useful for machine learning research and experiments.
-
-![](images/logo.png)
-
-## Contents
-
-- [jutility](#jutility)
-  - [Contents](#contents)
-  - [Install with `pip`](#install-with-pip)
-  - [Usage examples](#usage-examples)
-  - [Unit tests](#unit-tests)
-  - [Build package locally](#build-package-locally)
-  - [Updating package on PyPI](#updating-package-on-pypi)
-
-## Install with `pip`
-
-The `jutility` package is available as [a Python package on PyPI](https://pypi.org/project/jutility/), and can be installed with `pip` using the following commands:
-
-```
-python -m pip install -U pip
-python -m pip install -U jutility
-```
-
-## Usage examples
-
-*Coming soon*
-
-(in the meantime, see [`scripts/make_logo.py`](scripts/make_logo.py) which made the logo above, and [unit tests](tests/) for [`util`](tests/test_util.py), [`plotting`](tests/test_plotting.py), and [`sweep`](tests/test_sweep.py))
-
-## Unit tests
-
-To run unit all unit tests, install [`pytest`](https://pypi.org/project/pytest/), and run the following command (at the time of writing, this takes about 17 seconds to run 42 unit tests, because several unit tests involve saving images or GIFs to disk, using `pytest` version 5.4.1):
-
-```
-pytest
-```
-
-## Build package locally
-
-`jutility` can be built and installed locally using the following commands, replacing `$WHEEL_NAME` with the name of the wheel built by the `python -m build` command (for example, `jutility-0.0.5-py3-none-any.whl`):
-
-```
-python -m build
-python -m pip install --force-reinstall dist/$WHEEL_NAME
-```
-
-## Updating package on PyPI
-
-This package was uploaded to PyPI following [the Packaging Python Projects tutorial in the official Python documentation](https://packaging.python.org/en/latest/tutorials/packaging-projects/).
-
-To update PyPI with a newer version, update the `version` tag in [pyproject.toml](pyproject.toml), and then use the following commands:
-
-```
-rm -rf dist/*
-python -m build
-python -m twine upload dist/*
-```
-
-When prompted by `twine`, enter `__token__` as the username, and paste an API token from the [PyPI account management webpage](https://pypi.org/manage/account/) as the password (including the `pypi-` prefix).
+# jutility
+
+Collection of Python utilities intended to be useful for machine learning research and experiments.
+
+![](images/logo.png)
+
+## Contents
+
+- [jutility](#jutility)
+  - [Contents](#contents)
+  - [Install with `pip`](#install-with-pip)
+  - [Usage examples](#usage-examples)
+  - [Unit tests](#unit-tests)
+  - [Build package locally](#build-package-locally)
+  - [Updating package on PyPI](#updating-package-on-pypi)
+
+## Install with `pip`
+
+The `jutility` package is available as [a Python package on PyPI](https://pypi.org/project/jutility/), and can be installed with `pip` using the following commands:
+
+```
+python -m pip install -U pip
+python -m pip install -U jutility
+```
+
+## Usage examples
+
+*Coming soon*
+
+(in the meantime, see [`scripts/make_logo.py`](scripts/make_logo.py) which made the logo above, and [unit tests](tests/) for [`util`](tests/test_util.py), [`plotting`](tests/test_plotting.py), and [`sweep`](tests/test_sweep.py))
+
+## Unit tests
+
+To run unit all unit tests, install [`pytest`](https://pypi.org/project/pytest/), and run the following command (at the time of writing, this takes about 17 seconds to run 42 unit tests, because several unit tests involve saving images or GIFs to disk, using `pytest` version 5.4.1):
+
+```
+pytest
+```
+
+## Build package locally
+
+`jutility` can be built and installed locally using the following commands, replacing `$WHEEL_NAME` with the name of the wheel built by the `python -m build` command (for example, `jutility-0.0.5-py3-none-any.whl`):
+
+```
+python -m build
+python -m pip install --force-reinstall --no-deps dist/$WHEEL_NAME
+```
+
+## Updating package on PyPI
+
+This package was uploaded to PyPI following [the Packaging Python Projects tutorial in the official Python documentation](https://packaging.python.org/en/latest/tutorials/packaging-projects/).
+
+To update PyPI with a newer version, update the `version` tag in [pyproject.toml](pyproject.toml), and then use the following commands:
+
+```
+rm -rf dist/*
+python -m build
+python -m twine upload dist/*
+```
+
+When prompted by `twine`, enter `__token__` as the username, and paste an API token from the [PyPI account management webpage](https://pypi.org/manage/account/) as the password (including the `pypi-` prefix).
```

### Comparing `jutility-0.0.5/src/jutility/plotting.py` & `jutility-0.0.6/src/jutility/plotting.py`

 * *Files identical despite different names*

### Comparing `jutility-0.0.5/src/jutility/sweep.py` & `jutility-0.0.6/src/jutility/sweep.py`

 * *Files identical despite different names*

### Comparing `jutility-0.0.5/src/jutility/util.py` & `jutility-0.0.6/src/jutility/util.py`

 * *Files identical despite different names*

### Comparing `jutility-0.0.5/tests/test_plotting.py` & `jutility-0.0.6/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `jutility-0.0.5/tests/test_sweep.py` & `jutility-0.0.6/tests/test_sweep.py`

 * *Files identical despite different names*

### Comparing `jutility-0.0.5/tests/test_util.py` & `jutility-0.0.6/tests/test_util.py`

 * *Files identical despite different names*

