# Comparing `tmp/jutility-0.0.6.tar.gz` & `tmp/jutility-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Jake\Documents\Programming\jutility\dist\.tmp-dpalhca5\jutility-0.0.6.tar", last modified: Sun May 14 18:44:48 2023, max compression
+gzip compressed data, was "C:\Users\Jake\Documents\Programming\jutility\dist\.tmp-tw3sr49v\jutility-0.0.7.tar", last modified: Sun May 14 19:06:31 2023, max compression
```

## Comparing `jutility-0.0.6.tar` & `jutility-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 18:44:48.000000 jutility-0.0.6/
--rw-rw-rw-   0        0        0     1087 2023-05-13 21:09:33.000000 jutility-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      343 2023-05-14 18:44:48.000000 jutility-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2235 2023-05-14 18:41:23.000000 jutility-0.0.6/README.md
--rw-rw-rw-   0        0        0       90 2023-05-14 18:37:23.000000 jutility-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      445 2023-05-14 18:44:48.000000 jutility-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-14 18:44:48.000000 jutility-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-14 18:44:48.000000 jutility-0.0.6/src/jutility/
--rw-rw-rw-   0        0        0        0 2023-05-13 20:59:58.000000 jutility-0.0.6/src/jutility/__init__.py
--rw-rw-rw-   0        0        0    16333 2023-05-14 17:11:46.000000 jutility-0.0.6/src/jutility/plotting.py
--rw-rw-rw-   0        0        0    10048 2023-05-13 21:30:51.000000 jutility-0.0.6/src/jutility/sweep.py
--rw-rw-rw-   0        0        0    13209 2023-05-14 15:33:41.000000 jutility-0.0.6/src/jutility/util.py
-drwxrwxrwx   0        0        0        0 2023-05-14 18:44:48.000000 jutility-0.0.6/src/jutility.egg-info/
--rw-rw-rw-   0        0        0      343 2023-05-14 18:44:48.000000 jutility-0.0.6/src/jutility.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2023-05-14 18:44:48.000000 jutility-0.0.6/src/jutility.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 18:44:48.000000 jutility-0.0.6/src/jutility.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-14 18:44:48.000000 jutility-0.0.6/src/jutility.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-14 18:44:48.000000 jutility-0.0.6/src/jutility.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-14 18:44:48.000000 jutility-0.0.6/tests/
--rw-rw-rw-   0        0        0     9100 2023-05-14 15:22:52.000000 jutility-0.0.6/tests/test_plotting.py
--rw-rw-rw-   0        0        0     9206 2023-05-13 21:45:28.000000 jutility-0.0.6/tests/test_sweep.py
--rw-rw-rw-   0        0        0    12140 2023-05-14 15:40:12.000000 jutility-0.0.6/tests/test_util.py
+drwxrwxrwx   0        0        0        0 2023-05-14 19:06:31.000000 jutility-0.0.7/
+-rw-rw-rw-   0        0        0     1087 2023-05-13 21:09:33.000000 jutility-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     2891 2023-05-14 19:06:31.000000 jutility-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2272 2023-05-14 19:01:29.000000 jutility-0.0.7/README.md
+-rw-rw-rw-   0        0        0       90 2023-05-14 18:37:23.000000 jutility-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0      713 2023-05-14 19:06:31.000000 jutility-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-14 19:06:31.000000 jutility-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-14 19:06:31.000000 jutility-0.0.7/src/jutility/
+-rw-rw-rw-   0        0        0        0 2023-05-13 20:59:58.000000 jutility-0.0.7/src/jutility/__init__.py
+-rw-rw-rw-   0        0        0    16333 2023-05-14 17:11:46.000000 jutility-0.0.7/src/jutility/plotting.py
+-rw-rw-rw-   0        0        0    10048 2023-05-13 21:30:51.000000 jutility-0.0.7/src/jutility/sweep.py
+-rw-rw-rw-   0        0        0    13209 2023-05-14 15:33:41.000000 jutility-0.0.7/src/jutility/util.py
+drwxrwxrwx   0        0        0        0 2023-05-14 19:06:31.000000 jutility-0.0.7/src/jutility.egg-info/
+-rw-rw-rw-   0        0        0     2891 2023-05-14 19:06:31.000000 jutility-0.0.7/src/jutility.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2023-05-14 19:06:31.000000 jutility-0.0.7/src/jutility.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 19:06:31.000000 jutility-0.0.7/src/jutility.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-14 19:06:31.000000 jutility-0.0.7/src/jutility.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-14 19:06:31.000000 jutility-0.0.7/src/jutility.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 19:06:31.000000 jutility-0.0.7/tests/
+-rw-rw-rw-   0        0        0     9100 2023-05-14 15:22:52.000000 jutility-0.0.7/tests/test_plotting.py
+-rw-rw-rw-   0        0        0     9206 2023-05-13 21:45:28.000000 jutility-0.0.7/tests/test_sweep.py
+-rw-rw-rw-   0        0        0    12140 2023-05-14 15:40:12.000000 jutility-0.0.7/tests/test_util.py
```

### Comparing `jutility-0.0.6/LICENSE` & `jutility-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jutility-0.0.6/README.md` & `jutility-0.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 *Coming soon*
 
 (in the meantime, see [`scripts/make_logo.py`](scripts/make_logo.py) which made the logo above, and [unit tests](tests/) for [`util`](tests/test_util.py), [`plotting`](tests/test_plotting.py), and [`sweep`](tests/test_sweep.py))
 
 ## Unit tests
 
-To run unit all unit tests, install [`pytest`](https://pypi.org/project/pytest/), and run the following command (at the time of writing, this takes about 17 seconds to run 42 unit tests, because several unit tests involve saving images or GIFs to disk, using `pytest` version 5.4.1):
+To run unit all unit tests, install [`pytest`](https://pypi.org/project/pytest/) (these tests have previously been run with `pytest` version 5.4.1), and run the following command (at the time of writing, this takes about 17 seconds to run 42 unit tests, because several unit tests involve saving images or GIFs to disk):
 
 ```
 pytest
 ```
 
 ## Build package locally
```

### Comparing `jutility-0.0.6/src/jutility/plotting.py` & `jutility-0.0.7/src/jutility/plotting.py`

 * *Files identical despite different names*

### Comparing `jutility-0.0.6/src/jutility/sweep.py` & `jutility-0.0.7/src/jutility/sweep.py`

 * *Files identical despite different names*

### Comparing `jutility-0.0.6/src/jutility/util.py` & `jutility-0.0.7/src/jutility/util.py`

 * *Files identical despite different names*

### Comparing `jutility-0.0.6/tests/test_plotting.py` & `jutility-0.0.7/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `jutility-0.0.6/tests/test_sweep.py` & `jutility-0.0.7/tests/test_sweep.py`

 * *Files identical despite different names*

### Comparing `jutility-0.0.6/tests/test_util.py` & `jutility-0.0.7/tests/test_util.py`

 * *Files identical despite different names*

