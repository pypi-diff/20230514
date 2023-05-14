# Comparing `tmp/jutility-0.0.3.tar.gz` & `tmp/jutility-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Jake\Documents\Programming\jutility\dist\.tmp-v_olvpca\jutility-0.0.3.tar", last modified: Sun May 14 16:00:29 2023, max compression
+gzip compressed data, was "C:\Users\Jake\Documents\Programming\jutility\dist\.tmp-z__i0rbk\jutility-0.0.4.tar", last modified: Sun May 14 16:35:33 2023, max compression
```

## Comparing `jutility-0.0.3.tar` & `jutility-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 16:00:29.000000 jutility-0.0.3/
--rw-rw-rw-   0        0        0     1087 2023-05-13 21:09:33.000000 jutility-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2777 2023-05-14 16:00:29.000000 jutility-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2125 2023-05-14 15:59:42.000000 jutility-0.0.3/README.md
--rw-rw-rw-   0        0        0      766 2023-05-14 15:58:41.000000 jutility-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-14 16:00:29.000000 jutility-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-14 16:00:29.000000 jutility-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-14 16:00:29.000000 jutility-0.0.3/src/jutility/
--rw-rw-rw-   0        0        0        0 2023-05-13 20:59:58.000000 jutility-0.0.3/src/jutility/__init__.py
--rw-rw-rw-   0        0        0    16215 2023-05-13 21:31:01.000000 jutility-0.0.3/src/jutility/plotting.py
--rw-rw-rw-   0        0        0    10048 2023-05-13 21:30:51.000000 jutility-0.0.3/src/jutility/sweep.py
--rw-rw-rw-   0        0        0    13209 2023-05-14 15:33:41.000000 jutility-0.0.3/src/jutility/util.py
-drwxrwxrwx   0        0        0        0 2023-05-14 16:00:29.000000 jutility-0.0.3/src/jutility.egg-info/
--rw-rw-rw-   0        0        0     2777 2023-05-14 16:00:29.000000 jutility-0.0.3/src/jutility.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2023-05-14 16:00:29.000000 jutility-0.0.3/src/jutility.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 16:00:29.000000 jutility-0.0.3/src/jutility.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-14 16:00:29.000000 jutility-0.0.3/src/jutility.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-14 16:00:29.000000 jutility-0.0.3/src/jutility.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-14 16:00:29.000000 jutility-0.0.3/tests/
--rw-rw-rw-   0        0        0     9100 2023-05-14 15:22:52.000000 jutility-0.0.3/tests/test_plotting.py
--rw-rw-rw-   0        0        0     9206 2023-05-13 21:45:28.000000 jutility-0.0.3/tests/test_sweep.py
--rw-rw-rw-   0        0        0    12140 2023-05-14 15:40:12.000000 jutility-0.0.3/tests/test_util.py
+drwxrwxrwx   0        0        0        0 2023-05-14 16:35:33.000000 jutility-0.0.4/
+-rw-rw-rw-   0        0        0     1087 2023-05-13 21:09:33.000000 jutility-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2724 2023-05-14 16:35:33.000000 jutility-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2125 2023-05-14 16:32:17.000000 jutility-0.0.4/README.md
+-rw-rw-rw-   0        0        0      735 2023-05-14 16:32:23.000000 jutility-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-14 16:35:33.000000 jutility-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-14 16:35:33.000000 jutility-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-14 16:35:33.000000 jutility-0.0.4/src/jutility/
+-rw-rw-rw-   0        0        0        0 2023-05-13 20:59:58.000000 jutility-0.0.4/src/jutility/__init__.py
+-rw-rw-rw-   0        0        0    16215 2023-05-13 21:31:01.000000 jutility-0.0.4/src/jutility/plotting.py
+-rw-rw-rw-   0        0        0    10048 2023-05-13 21:30:51.000000 jutility-0.0.4/src/jutility/sweep.py
+-rw-rw-rw-   0        0        0    13209 2023-05-14 15:33:41.000000 jutility-0.0.4/src/jutility/util.py
+drwxrwxrwx   0        0        0        0 2023-05-14 16:35:33.000000 jutility-0.0.4/src/jutility.egg-info/
+-rw-rw-rw-   0        0        0     2724 2023-05-14 16:35:33.000000 jutility-0.0.4/src/jutility.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-05-14 16:35:33.000000 jutility-0.0.4/src/jutility.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 16:35:33.000000 jutility-0.0.4/src/jutility.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-14 16:35:33.000000 jutility-0.0.4/src/jutility.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-14 16:35:33.000000 jutility-0.0.4/src/jutility.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 16:35:33.000000 jutility-0.0.4/tests/
+-rw-rw-rw-   0        0        0     9100 2023-05-14 15:22:52.000000 jutility-0.0.4/tests/test_plotting.py
+-rw-rw-rw-   0        0        0     9206 2023-05-13 21:45:28.000000 jutility-0.0.4/tests/test_sweep.py
+-rw-rw-rw-   0        0        0    12140 2023-05-14 15:40:12.000000 jutility-0.0.4/tests/test_util.py
```

### Comparing `jutility-0.0.3/LICENSE` & `jutility-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jutility-0.0.3/PKG-INFO` & `jutility-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: jutility
-Version: 0.0.3
+Version: 0.0.4
 Summary: Collection of Python utilities intended to be useful for machine learning research and experiments
 Author-email: Jake Levi <jakelevi@hotmail.co.uk>
-Project-URL: Homepage, https://github.com/jakelevi1996/jutility
-Project-URL: Bug Tracker, https://github.com/jakelevi1996/jutility/issues
+License: MIT License
+Project-URL: homepage, https://github.com/jakelevi1996/jutility
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jutility-0.0.3/README.md` & `jutility-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `jutility-0.0.3/src/jutility/plotting.py` & `jutility-0.0.4/src/jutility/plotting.py`

 * *Files identical despite different names*

### Comparing `jutility-0.0.3/src/jutility/sweep.py` & `jutility-0.0.4/src/jutility/sweep.py`

 * *Files identical despite different names*

### Comparing `jutility-0.0.3/src/jutility/util.py` & `jutility-0.0.4/src/jutility/util.py`

 * *Files identical despite different names*

### Comparing `jutility-0.0.3/src/jutility.egg-info/PKG-INFO` & `jutility-0.0.4/src/jutility.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: jutility
-Version: 0.0.3
+Version: 0.0.4
 Summary: Collection of Python utilities intended to be useful for machine learning research and experiments
 Author-email: Jake Levi <jakelevi@hotmail.co.uk>
-Project-URL: Homepage, https://github.com/jakelevi1996/jutility
-Project-URL: Bug Tracker, https://github.com/jakelevi1996/jutility/issues
+License: MIT License
+Project-URL: homepage, https://github.com/jakelevi1996/jutility
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jutility-0.0.3/tests/test_plotting.py` & `jutility-0.0.4/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `jutility-0.0.3/tests/test_sweep.py` & `jutility-0.0.4/tests/test_sweep.py`

 * *Files identical despite different names*

### Comparing `jutility-0.0.3/tests/test_util.py` & `jutility-0.0.4/tests/test_util.py`

 * *Files identical despite different names*

