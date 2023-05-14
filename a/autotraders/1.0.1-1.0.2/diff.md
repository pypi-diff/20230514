# Comparing `tmp/autotraders-1.0.1.tar.gz` & `tmp/autotraders-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-1.0.1.tar", last modified: Sun May 14 00:14:57 2023, max compression
+gzip compressed data, was "autotraders-1.0.2.tar", last modified: Sun May 14 00:28:58 2023, max compression
```

## Comparing `autotraders-1.0.1.tar` & `autotraders-1.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 00:14:57.391438 autotraders-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-14 00:14:39.000000 autotraders-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-14 00:14:57.391438 autotraders-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-14 00:14:39.000000 autotraders-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 00:14:57.387438 autotraders-1.0.1/autotraders/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-14 00:14:39.000000 autotraders-1.0.1/autotraders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-14 00:14:39.000000 autotraders-1.0.1/autotraders/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-14 00:14:39.000000 autotraders-1.0.1/autotraders/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-14 00:14:39.000000 autotraders-1.0.1/autotraders/faction.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-14 00:14:39.000000 autotraders-1.0.1/autotraders/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 00:14:57.391438 autotraders-1.0.1/autotraders/ship/
--rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-05-14 00:14:39.000000 autotraders-1.0.1/autotraders/ship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-14 00:14:39.000000 autotraders-1.0.1/autotraders/ship/ship_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-14 00:14:39.000000 autotraders-1.0.1/autotraders/ship/survey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-14 00:14:39.000000 autotraders-1.0.1/autotraders/system.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-14 00:14:39.000000 autotraders-1.0.1/autotraders/trait.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-14 00:14:39.000000 autotraders-1.0.1/autotraders/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-14 00:14:39.000000 autotraders-1.0.1/autotraders/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 00:14:57.391438 autotraders-1.0.1/autotraders/waypoint_types/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-14 00:14:39.000000 autotraders-1.0.1/autotraders/waypoint_types/jumpgate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-14 00:14:39.000000 autotraders-1.0.1/autotraders/waypoint_types/marketplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-14 00:14:39.000000 autotraders-1.0.1/autotraders/waypoint_types/shipyard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 00:14:57.387438 autotraders-1.0.1/autotraders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-14 00:14:57.000000 autotraders-1.0.1/autotraders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-14 00:14:57.000000 autotraders-1.0.1/autotraders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 00:14:57.000000 autotraders-1.0.1/autotraders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 00:14:57.000000 autotraders-1.0.1/autotraders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-14 00:14:39.000000 autotraders-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 00:14:57.391438 autotraders-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 00:14:57.391438 autotraders-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-14 00:14:39.000000 autotraders-1.0.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 00:28:58.089597 autotraders-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-14 00:28:36.000000 autotraders-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-14 00:28:58.089597 autotraders-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-14 00:28:36.000000 autotraders-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 00:28:58.089597 autotraders-1.0.2/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-14 00:28:36.000000 autotraders-1.0.2/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-14 00:28:36.000000 autotraders-1.0.2/autotraders/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-14 00:28:36.000000 autotraders-1.0.2/autotraders/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-14 00:28:36.000000 autotraders-1.0.2/autotraders/faction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-14 00:28:36.000000 autotraders-1.0.2/autotraders/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 00:28:58.089597 autotraders-1.0.2/autotraders/ship/
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-05-14 00:28:36.000000 autotraders-1.0.2/autotraders/ship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-14 00:28:36.000000 autotraders-1.0.2/autotraders/ship/ship_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-14 00:28:36.000000 autotraders-1.0.2/autotraders/ship/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-14 00:28:36.000000 autotraders-1.0.2/autotraders/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-14 00:28:36.000000 autotraders-1.0.2/autotraders/trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-14 00:28:36.000000 autotraders-1.0.2/autotraders/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-14 00:28:36.000000 autotraders-1.0.2/autotraders/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 00:28:58.089597 autotraders-1.0.2/autotraders/waypoint_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-14 00:28:36.000000 autotraders-1.0.2/autotraders/waypoint_types/jumpgate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-14 00:28:36.000000 autotraders-1.0.2/autotraders/waypoint_types/marketplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-14 00:28:36.000000 autotraders-1.0.2/autotraders/waypoint_types/shipyard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 00:28:58.089597 autotraders-1.0.2/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-14 00:28:58.000000 autotraders-1.0.2/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-14 00:28:58.000000 autotraders-1.0.2/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 00:28:58.000000 autotraders-1.0.2/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 00:28:58.000000 autotraders-1.0.2/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-14 00:28:36.000000 autotraders-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 00:28:58.089597 autotraders-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 00:28:58.089597 autotraders-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-14 00:28:36.000000 autotraders-1.0.2/tests/test_util.py
```

### Comparing `autotraders-1.0.1/LICENSE` & `autotraders-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autotraders-1.0.1/PKG-INFO` & `autotraders-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.0.1
+Version: 1.0.2
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.0.1/README.md` & `autotraders-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `autotraders-1.0.1/autotraders/agent.py` & `autotraders-1.0.2/autotraders/agent.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.0.1/autotraders/contract.py` & `autotraders-1.0.2/autotraders/contract.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.0.1/autotraders/faction.py` & `autotraders-1.0.2/autotraders/faction.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.0.1/autotraders/ship/__init__.py` & `autotraders-1.0.2/autotraders/ship/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.0.1/autotraders/ship/ship_components.py` & `autotraders-1.0.2/autotraders/ship/ship_components.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 class Requirements:
     def __init__(self, data):
-        self.power = data["power"]
-        self.crew = data["crew"]
+        if "power" in data:
+            self.power = data["power"]
+        if "crew" in data:
+            self.crew = data["crew"]
         if "slots" in data:
             self.slots = data["slots"]
 
 
 class ShipComponent:
     def __init__(self, data):
         self.symbol = data["symbol"]
```

### Comparing `autotraders-1.0.1/autotraders/system.py` & `autotraders-1.0.2/autotraders/system.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.0.1/autotraders/waypoint.py` & `autotraders-1.0.2/autotraders/waypoint.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.0.1/autotraders/waypoint_types/jumpgate.py` & `autotraders-1.0.2/autotraders/waypoint_types/jumpgate.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.0.1/autotraders/waypoint_types/marketplace.py` & `autotraders-1.0.2/autotraders/waypoint_types/marketplace.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.0.1/autotraders/waypoint_types/shipyard.py` & `autotraders-1.0.2/autotraders/waypoint_types/shipyard.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.0.1/autotraders.egg-info/PKG-INFO` & `autotraders-1.0.2/autotraders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.0.1
+Version: 1.0.2
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.0.1/autotraders.egg-info/SOURCES.txt` & `autotraders-1.0.2/autotraders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotraders-1.0.1/pyproject.toml` & `autotraders-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autotraders"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Ashwin Naren", email="arihant2math@gmail.com" },
 ]
 description = "A powerful spacetraders API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

