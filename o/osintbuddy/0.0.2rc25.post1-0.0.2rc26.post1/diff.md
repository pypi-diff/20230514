# Comparing `tmp/osintbuddy-0.0.2rc25.post1.tar.gz` & `tmp/osintbuddy-0.0.2rc26.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osintbuddy-0.0.2rc25.post1.tar", last modified: Sun May 14 00:55:29 2023, max compression
+gzip compressed data, was "osintbuddy-0.0.2rc26.post1.tar", last modified: Sun May 14 01:02:25 2023, max compression
```

## Comparing `osintbuddy-0.0.2rc25.post1.tar` & `osintbuddy-0.0.2rc26.post1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      274 2023-05-14 00:55:21.300873 osintbuddy-0.0.2rc25.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      447 2023-05-14 00:55:21.300873 osintbuddy-0.0.2rc25.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2023-05-14 00:55:21.300873 osintbuddy-0.0.2rc25.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      314 2023-05-14 00:55:21.300873 osintbuddy-0.0.2rc25.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0     1807 2023-05-14 00:55:21.300873 osintbuddy-0.0.2rc25.post1/.gitignore
--rw-r--r--   0        0        0     1540 2023-05-14 00:55:21.300873 osintbuddy-0.0.2rc25.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2023-05-14 00:55:21.300873 osintbuddy-0.0.2rc25.post1/.pypirc
--rw-r--r--   0        0        0        5 2023-05-14 00:55:21.300873 osintbuddy-0.0.2rc25.post1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      316 2023-05-14 00:55:21.300873 osintbuddy-0.0.2rc25.post1/Dockerfile
--rw-r--r--   0        0        0       11 2023-05-14 00:55:21.300873 osintbuddy-0.0.2rc25.post1/LICENSE
--rw-r--r--   0        0        0      809 2023-05-14 00:55:21.300873 osintbuddy-0.0.2rc25.post1/README.md
--rw-r--r--   0        0        0       47 2023-05-14 00:55:21.300873 osintbuddy-0.0.2rc25.post1/docs/developer.md
--rw-r--r--   0        0        0      471 2023-05-14 00:55:21.300873 osintbuddy-0.0.2rc25.post1/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2023-05-14 00:55:21.300873 osintbuddy-0.0.2rc25.post1/docs/pylint.md
--rw-r--r--   0        0        0      497 2023-05-14 00:55:21.300873 osintbuddy-0.0.2rc25.post1/docs/pyproject.md
--rw-r--r--   0        0        0      208 2023-05-14 00:55:21.300873 osintbuddy-0.0.2rc25.post1/docs/workflows.md
--rw-r--r--   0        0        0     6666 2023-05-14 00:55:21.300873 osintbuddy-0.0.2rc25.post1/pyproject.toml
--rw-r--r--   0        0        0      293 2023-05-14 00:55:21.300873 osintbuddy-0.0.2rc25.post1/src/README.md
--rw-r--r--   0        0        0      374 2023-05-14 00:55:29.089128 osintbuddy-0.0.2rc25.post1/src/osintbuddy/__init__.py
--rw-r--r--   0        0        0      151 2023-05-14 00:55:21.300873 osintbuddy-0.0.2rc25.post1/src/osintbuddy/errors.py
--rw-r--r--   0        0        0      527 2023-05-14 00:55:21.300873 osintbuddy-0.0.2rc25.post1/src/osintbuddy/examples/ip-plugin.py
--rw-r--r--   0        0        0      206 2023-05-14 00:55:21.300873 osintbuddy-0.0.2rc25.post1/src/osintbuddy/manager.py
--rw-r--r--   0        0        0      358 2023-05-14 00:55:21.300873 osintbuddy-0.0.2rc25.post1/src/osintbuddy/node/__init__.py
--rw-r--r--   0        0        0     1302 2023-05-14 00:55:21.300873 osintbuddy-0.0.2rc25.post1/src/osintbuddy/node/base.py
--rw-r--r--   0        0        0     2989 2023-05-14 00:55:21.300873 osintbuddy-0.0.2rc25.post1/src/osintbuddy/node/displays.py
--rw-r--r--   0        0        0     4099 2023-05-14 00:55:21.300873 osintbuddy-0.0.2rc25.post1/src/osintbuddy/node/inputs.py
--rw-r--r--   0        0        0     6363 2023-05-14 00:55:21.300873 osintbuddy-0.0.2rc25.post1/src/osintbuddy/plugins.py
--rw-r--r--   0        0        0     1301 2023-05-14 00:55:21.300873 osintbuddy-0.0.2rc25.post1/src/osintbuddy/utils.py
--rw-r--r--   0        0        0      964 2023-05-14 00:55:21.300873 osintbuddy-0.0.2rc25.post1/tests/conftest.py
--rw-r--r--   0        0        0      664 2023-05-14 00:55:21.300873 osintbuddy-0.0.2rc25.post1/tests/test_methods.py
--rw-r--r--   0        0        0     2661 1970-01-01 00:00:00.000000 osintbuddy-0.0.2rc25.post1/PKG-INFO
+-rw-r--r--   0        0        0      274 2023-05-14 01:02:17.971802 osintbuddy-0.0.2rc26.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      447 2023-05-14 01:02:17.971802 osintbuddy-0.0.2rc26.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2023-05-14 01:02:17.971802 osintbuddy-0.0.2rc26.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      314 2023-05-14 01:02:17.971802 osintbuddy-0.0.2rc26.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0     1807 2023-05-14 01:02:17.971802 osintbuddy-0.0.2rc26.post1/.gitignore
+-rw-r--r--   0        0        0     1540 2023-05-14 01:02:17.971802 osintbuddy-0.0.2rc26.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2023-05-14 01:02:17.971802 osintbuddy-0.0.2rc26.post1/.pypirc
+-rw-r--r--   0        0        0        5 2023-05-14 01:02:17.971802 osintbuddy-0.0.2rc26.post1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      316 2023-05-14 01:02:17.971802 osintbuddy-0.0.2rc26.post1/Dockerfile
+-rw-r--r--   0        0        0       11 2023-05-14 01:02:17.971802 osintbuddy-0.0.2rc26.post1/LICENSE
+-rw-r--r--   0        0        0     1013 2023-05-14 01:02:17.971802 osintbuddy-0.0.2rc26.post1/README.md
+-rw-r--r--   0        0        0       47 2023-05-14 01:02:17.971802 osintbuddy-0.0.2rc26.post1/docs/developer.md
+-rw-r--r--   0        0        0      471 2023-05-14 01:02:17.971802 osintbuddy-0.0.2rc26.post1/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2023-05-14 01:02:17.971802 osintbuddy-0.0.2rc26.post1/docs/pylint.md
+-rw-r--r--   0        0        0      497 2023-05-14 01:02:17.971802 osintbuddy-0.0.2rc26.post1/docs/pyproject.md
+-rw-r--r--   0        0        0      208 2023-05-14 01:02:17.971802 osintbuddy-0.0.2rc26.post1/docs/workflows.md
+-rw-r--r--   0        0        0     6666 2023-05-14 01:02:17.971802 osintbuddy-0.0.2rc26.post1/pyproject.toml
+-rw-r--r--   0        0        0      293 2023-05-14 01:02:17.971802 osintbuddy-0.0.2rc26.post1/src/README.md
+-rw-r--r--   0        0        0      374 2023-05-14 01:02:24.724007 osintbuddy-0.0.2rc26.post1/src/osintbuddy/__init__.py
+-rw-r--r--   0        0        0      151 2023-05-14 01:02:17.971802 osintbuddy-0.0.2rc26.post1/src/osintbuddy/errors.py
+-rw-r--r--   0        0        0      527 2023-05-14 01:02:17.971802 osintbuddy-0.0.2rc26.post1/src/osintbuddy/examples/ip-plugin.py
+-rw-r--r--   0        0        0      206 2023-05-14 01:02:17.971802 osintbuddy-0.0.2rc26.post1/src/osintbuddy/manager.py
+-rw-r--r--   0        0        0      358 2023-05-14 01:02:17.971802 osintbuddy-0.0.2rc26.post1/src/osintbuddy/node/__init__.py
+-rw-r--r--   0        0        0     1302 2023-05-14 01:02:17.971802 osintbuddy-0.0.2rc26.post1/src/osintbuddy/node/base.py
+-rw-r--r--   0        0        0     2989 2023-05-14 01:02:17.971802 osintbuddy-0.0.2rc26.post1/src/osintbuddy/node/displays.py
+-rw-r--r--   0        0        0     4099 2023-05-14 01:02:17.971802 osintbuddy-0.0.2rc26.post1/src/osintbuddy/node/inputs.py
+-rw-r--r--   0        0        0     6384 2023-05-14 01:02:17.971802 osintbuddy-0.0.2rc26.post1/src/osintbuddy/plugins.py
+-rw-r--r--   0        0        0     1301 2023-05-14 01:02:17.971802 osintbuddy-0.0.2rc26.post1/src/osintbuddy/utils.py
+-rw-r--r--   0        0        0      964 2023-05-14 01:02:17.971802 osintbuddy-0.0.2rc26.post1/tests/conftest.py
+-rw-r--r--   0        0        0      664 2023-05-14 01:02:17.971802 osintbuddy-0.0.2rc26.post1/tests/test_methods.py
+-rw-r--r--   0        0        0     2865 1970-01-01 00:00:00.000000 osintbuddy-0.0.2rc26.post1/PKG-INFO
```

### Comparing `osintbuddy-0.0.2rc25.post1/.gitignore` & `osintbuddy-0.0.2rc26.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc25.post1/.pre-commit-config.yaml` & `osintbuddy-0.0.2rc26.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc25.post1/README.md` & `osintbuddy-0.0.2rc26.post1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+[![Total Downloads](https://static.pepy.tech/badge/osintbuddy)](https://pepy.tech/project/osintbuddy)
+[![Downloads](https://static.pepy.tech/badge/osintbuddy/week)](https://pepy.tech/project/osintbuddy)
+
 # OSINTBuddy plugins and extensions
 
 The plugins library for [jerlendds/osintbuddy](https://github.com/jerlendds/osintbuddy), coming soon...
 
 
 This project follows the Python Standards declared in PEP 621. It uses a pyproject.yaml file to configure the project and Flit to simplify the build process and publish to PyPI.
```

### Comparing `osintbuddy-0.0.2rc25.post1/docs/pylint.md` & `osintbuddy-0.0.2rc26.post1/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc25.post1/pyproject.toml` & `osintbuddy-0.0.2rc26.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc25.post1/src/osintbuddy/examples/ip-plugin.py` & `osintbuddy-0.0.2rc26.post1/src/osintbuddy/examples/ip-plugin.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc25.post1/src/osintbuddy/node/base.py` & `osintbuddy-0.0.2rc26.post1/src/osintbuddy/node/base.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc25.post1/src/osintbuddy/node/displays.py` & `osintbuddy-0.0.2rc26.post1/src/osintbuddy/node/displays.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc25.post1/src/osintbuddy/node/inputs.py` & `osintbuddy-0.0.2rc26.post1/src/osintbuddy/node/inputs.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc25.post1/src/osintbuddy/plugins.py` & `osintbuddy-0.0.2rc26.post1/src/osintbuddy/plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,15 @@
     node: List[BaseNode]
     name: str = 'Plugin Node'
     color: str = '#145070'
     label: str = ''
     icon: str = 'atom-2'
     transform_icons: dict = {}
     show_label = True
+    style: dict = {}
 
     def __init__(self):
         transforms = self.__class__.__dict__.values()
         self.transforms = {
             func.label: func for func in transforms if hasattr(func, 'label')
         }
         self.transform_labels = [
```

### Comparing `osintbuddy-0.0.2rc25.post1/src/osintbuddy/utils.py` & `osintbuddy-0.0.2rc26.post1/src/osintbuddy/utils.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc25.post1/tests/conftest.py` & `osintbuddy-0.0.2rc26.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc25.post1/tests/test_methods.py` & `osintbuddy-0.0.2rc26.post1/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc25.post1/PKG-INFO` & `osintbuddy-0.0.2rc26.post1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osintbuddy
-Version: 0.0.2rc25.post1
+Version: 0.0.2rc26.post1
 Summary: OSINTBuddy - mine, merge, and map data for novel insights
 Author-email: jerlendds <jerlendsdev@proton.me>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -33,14 +33,17 @@
 Requires-Dist: shellcheck-py==0.9.0.2 ; extra == "test"
 Project-URL: Documentation, https://docs-osintbuddy-com.vercel.app/
 Project-URL: Source, https://github.com/jerlendds/plugins.osintbuddy.com
 Project-URL: Tracker, https://github.com/jerlendds/osintbuddy/issues
 Provides-Extra: spark
 Provides-Extra: test
 
+[![Total Downloads](https://static.pepy.tech/badge/osintbuddy)](https://pepy.tech/project/osintbuddy)
+[![Downloads](https://static.pepy.tech/badge/osintbuddy/week)](https://pepy.tech/project/osintbuddy)
+
 # OSINTBuddy plugins and extensions
 
 The plugins library for [jerlendds/osintbuddy](https://github.com/jerlendds/osintbuddy), coming soon...
 
 
 This project follows the Python Standards declared in PEP 621. It uses a pyproject.yaml file to configure the project and Flit to simplify the build process and publish to PyPI.
```

