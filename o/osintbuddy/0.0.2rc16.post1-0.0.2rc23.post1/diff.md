# Comparing `tmp/osintbuddy-0.0.2rc16.post1.tar.gz` & `tmp/osintbuddy-0.0.2rc23.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osintbuddy-0.0.2rc16.post1.tar", last modified: Sat Apr 15 21:20:22 2023, max compression
+gzip compressed data, was "osintbuddy-0.0.2rc23.post1.tar", last modified: Sat May 13 23:58:11 2023, max compression
```

## Comparing `osintbuddy-0.0.2rc16.post1.tar` & `osintbuddy-0.0.2rc23.post1.tar`

### file list

```diff
@@ -1,26 +1,31 @@
--rw-r--r--   0        0        0      274 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      447 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      314 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0     1807 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/.gitignore
--rw-r--r--   0        0        0     1540 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/.pypirc
--rw-r--r--   0        0        0        5 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      316 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/Dockerfile
--rw-r--r--   0        0        0       11 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/LICENSE
--rw-r--r--   0        0        0      809 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/README.md
--rw-r--r--   0        0        0       47 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/docs/developer.md
--rw-r--r--   0        0        0      471 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/docs/pylint.md
--rw-r--r--   0        0        0      497 2023-04-15 21:20:19.841321 osintbuddy-0.0.2rc16.post1/docs/pyproject.md
--rw-r--r--   0        0        0      208 2023-04-15 21:20:19.845321 osintbuddy-0.0.2rc16.post1/docs/workflows.md
--rw-r--r--   0        0        0     6726 2023-04-15 21:20:19.845321 osintbuddy-0.0.2rc16.post1/pyproject.toml
--rw-r--r--   0        0        0      292 2023-04-15 21:20:19.845321 osintbuddy-0.0.2rc16.post1/src/README.md
--rw-r--r--   0        0        0      374 2023-04-15 21:20:22.593318 osintbuddy-0.0.2rc16.post1/src/osintbuddy/__init__.py
--rw-r--r--   0        0        0      527 2023-04-15 21:20:19.845321 osintbuddy-0.0.2rc16.post1/src/osintbuddy/examples/ip-plugin.py
--rw-r--r--   0        0        0      206 2023-04-15 21:20:19.845321 osintbuddy-0.0.2rc16.post1/src/osintbuddy/manager.py
--rw-r--r--   0        0        0     1219 2023-04-15 21:20:19.845321 osintbuddy-0.0.2rc16.post1/src/osintbuddy/plugins.py
--rw-r--r--   0        0        0     6498 2023-04-15 21:20:19.845321 osintbuddy-0.0.2rc16.post1/src/osintbuddy/utils.py
--rw-r--r--   0        0        0      964 2023-04-15 21:20:19.845321 osintbuddy-0.0.2rc16.post1/tests/conftest.py
--rw-r--r--   0        0        0      664 2023-04-15 21:20:19.845321 osintbuddy-0.0.2rc16.post1/tests/test_methods.py
--rw-r--r--   0        0        0     2752 1970-01-01 00:00:00.000000 osintbuddy-0.0.2rc16.post1/PKG-INFO
+-rw-r--r--   0        0        0      274 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      447 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      314 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0     1807 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/.gitignore
+-rw-r--r--   0        0        0     1540 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/.pypirc
+-rw-r--r--   0        0        0        5 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      316 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/Dockerfile
+-rw-r--r--   0        0        0       11 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/LICENSE
+-rw-r--r--   0        0        0      809 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/README.md
+-rw-r--r--   0        0        0       47 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/docs/developer.md
+-rw-r--r--   0        0        0      471 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/docs/pylint.md
+-rw-r--r--   0        0        0      497 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/docs/pyproject.md
+-rw-r--r--   0        0        0      208 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/docs/workflows.md
+-rw-r--r--   0        0        0     6666 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/pyproject.toml
+-rw-r--r--   0        0        0      293 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/src/README.md
+-rw-r--r--   0        0        0      374 2023-05-13 23:58:11.451463 osintbuddy-0.0.2rc23.post1/src/osintbuddy/__init__.py
+-rw-r--r--   0        0        0      151 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/src/osintbuddy/errors.py
+-rw-r--r--   0        0        0      527 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/src/osintbuddy/examples/ip-plugin.py
+-rw-r--r--   0        0        0      206 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/src/osintbuddy/manager.py
+-rw-r--r--   0        0        0      358 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/src/osintbuddy/node/__init__.py
+-rw-r--r--   0        0        0     1302 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/src/osintbuddy/node/base.py
+-rw-r--r--   0        0        0     2989 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/src/osintbuddy/node/displays.py
+-rw-r--r--   0        0        0     4099 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/src/osintbuddy/node/inputs.py
+-rw-r--r--   0        0        0     6429 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/src/osintbuddy/plugins.py
+-rw-r--r--   0        0        0     1301 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/src/osintbuddy/utils.py
+-rw-r--r--   0        0        0      964 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/tests/conftest.py
+-rw-r--r--   0        0        0      664 2023-05-13 23:58:08.679380 osintbuddy-0.0.2rc23.post1/tests/test_methods.py
+-rw-r--r--   0        0        0     2661 1970-01-01 00:00:00.000000 osintbuddy-0.0.2rc23.post1/PKG-INFO
```

### Comparing `osintbuddy-0.0.2rc16.post1/.gitignore` & `osintbuddy-0.0.2rc23.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc16.post1/.pre-commit-config.yaml` & `osintbuddy-0.0.2rc23.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc16.post1/README.md` & `osintbuddy-0.0.2rc23.post1/README.md`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc16.post1/docs/pylint.md` & `osintbuddy-0.0.2rc23.post1/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc16.post1/pyproject.toml` & `osintbuddy-0.0.2rc23.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,14 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10"
 ]
 requires-python = ">=3.7"
 dynamic = ["version"]
 dependencies = [
-  'fastapi==0.95.1',
-  'neo4j==5.7.0',
-  'pydantic==1.10.7'
 ]
 
 [project.optional-dependencies]
 spark = [
     "pyspark>=3.0.0"
 ]
 test = [
```

### Comparing `osintbuddy-0.0.2rc16.post1/src/osintbuddy/examples/ip-plugin.py` & `osintbuddy-0.0.2rc23.post1/src/osintbuddy/examples/ip-plugin.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc16.post1/tests/conftest.py` & `osintbuddy-0.0.2rc23.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc16.post1/tests/test_methods.py` & `osintbuddy-0.0.2rc23.post1/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.2rc16.post1/PKG-INFO` & `osintbuddy-0.0.2rc23.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: osintbuddy
-Version: 0.0.2rc16.post1
+Version: 0.0.2rc23.post1
 Summary: OSINTBuddy - mine, merge, and map data for novel insights
 Author-email: jerlendds <jerlendsdev@proton.me>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: fastapi==0.95.1
-Requires-Dist: neo4j==5.7.0
-Requires-Dist: pydantic==1.10.7
 Requires-Dist: pyspark>=3.0.0 ; extra == "spark"
 Requires-Dist: bandit[toml]==1.7.4 ; extra == "test"
 Requires-Dist: black==23.1.0 ; extra == "test"
 Requires-Dist: check-manifest==0.48 ; extra == "test"
 Requires-Dist: flake8-bugbear==23.3.12 ; extra == "test"
 Requires-Dist: flake8-docstrings ; extra == "test"
 Requires-Dist: flake8-formatter_junit_xml ; extra == "test"
```

