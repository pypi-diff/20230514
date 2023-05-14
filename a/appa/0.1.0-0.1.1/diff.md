# Comparing `tmp/appa-0.1.0.tar.gz` & `tmp/appa-0.1.1.tar.gz`

## Comparing `appa-0.1.0.tar` & `appa-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 appa-0.1.0/src/appa/__init__.py
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 appa-0.1.0/src/appa/propagator.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 appa-0.1.0/src/appa/solarsystem.py
--rw-r--r--   0        0        0     7233 2020-02-02 00:00:00.000000 appa-0.1.0/src/appa/spacecraft.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 appa-0.1.0/src/appa/stop_conditions.py
--rw-r--r--   0        0        0    11541 2020-02-02 00:00:00.000000 appa-0.1.0/src/appa/toolbox.py
--rw-r--r--   0        0        0 10895360 2020-02-02 00:00:00.000000 appa-0.1.0/src/appa/spice_data/de432s.bsp
--rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 appa-0.1.0/src/appa/spice_data/latest_leapseconds.tls
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 appa-0.1.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 appa-0.1.0/LICENSE
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 appa-0.1.0/README.md
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 appa-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 appa-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 appa-0.1.1/src/appa/__init__.py
+-rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 appa-0.1.1/src/appa/propagator.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 appa-0.1.1/src/appa/solarsystem.py
+-rw-r--r--   0        0        0     7233 2020-02-02 00:00:00.000000 appa-0.1.1/src/appa/spacecraft.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 appa-0.1.1/src/appa/stop_conditions.py
+-rw-r--r--   0        0        0    11541 2020-02-02 00:00:00.000000 appa-0.1.1/src/appa/toolbox.py
+-rw-r--r--   0        0        0 10895360 2020-02-02 00:00:00.000000 appa-0.1.1/src/appa/spice_data/de432s.bsp
+-rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 appa-0.1.1/src/appa/spice_data/latest_leapseconds.tls
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 appa-0.1.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 appa-0.1.1/LICENSE
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 appa-0.1.1/README.md
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 appa-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 appa-0.1.1/PKG-INFO
```

### Comparing `appa-0.1.0/src/appa/propagator.py` & `appa-0.1.1/src/appa/propagator.py`

 * *Files identical despite different names*

### Comparing `appa-0.1.0/src/appa/spacecraft.py` & `appa-0.1.1/src/appa/spacecraft.py`

 * *Files identical despite different names*

### Comparing `appa-0.1.0/src/appa/stop_conditions.py` & `appa-0.1.1/src/appa/stop_conditions.py`

 * *Files identical despite different names*

### Comparing `appa-0.1.0/src/appa/toolbox.py` & `appa-0.1.1/src/appa/toolbox.py`

 * *Files identical despite different names*

### Comparing `appa-0.1.0/src/appa/spice_data/de432s.bsp` & `appa-0.1.1/src/appa/spice_data/de432s.bsp`

 * *Files identical despite different names*

### Comparing `appa-0.1.0/src/appa/spice_data/latest_leapseconds.tls` & `appa-0.1.1/src/appa/spice_data/latest_leapseconds.tls`

 * *Files identical despite different names*

### Comparing `appa-0.1.0/LICENSE` & `appa-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `appa-0.1.0/pyproject.toml` & `appa-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
-name = "APPA"
-version = "0.1.0"
+name = "appa"
+version = "0.1.1"
 authors = [
   { name="C. Cooper"},
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `appa-0.1.0/PKG-INFO` & `appa-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: APPA
-Version: 0.1.0
+Name: appa
+Version: 0.1.1
 Project-URL: Homepage, https://github.com/coope248/APPA
 Project-URL: Bug Tracker, https://github.com/coope248/APPA/issues
 Author: C. Cooper
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

