# Comparing `tmp/circuitpython-laser-egismos-1.1.0.tar.gz` & `tmp/circuitpython-laser-egismos-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-laser-egismos-1.1.0.tar", last modified: Sun May 14 14:53:49 2023, max compression
+gzip compressed data, was "circuitpython-laser-egismos-1.1.1.tar", last modified: Sun May 14 15:07:03 2023, max compression
```

## Comparing `circuitpython-laser-egismos-1.1.0.tar` & `circuitpython-laser-egismos-1.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:53:49.406151 circuitpython-laser-egismos-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:53:49.398151 circuitpython-laser-egismos-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:53:49.402151 circuitpython-laser-egismos-1.1.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:53:49.402151 circuitpython-laser-egismos-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:53:49.402151 circuitpython-laser-egismos-1.1.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-14 14:53:49.406151 circuitpython-laser-egismos-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:53:49.406151 circuitpython-laser-egismos-1.1.0/circuitpython_laser_egismos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-14 14:53:49.000000 circuitpython-laser-egismos-1.1.0/circuitpython_laser_egismos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-14 14:53:49.000000 circuitpython-laser-egismos-1.1.0/circuitpython_laser_egismos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 14:53:49.000000 circuitpython-laser-egismos-1.1.0/circuitpython_laser_egismos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-14 14:53:49.000000 circuitpython-laser-egismos-1.1.0/circuitpython_laser_egismos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-14 14:53:49.000000 circuitpython-laser-egismos-1.1.0/circuitpython_laser_egismos.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:53:49.406151 circuitpython-laser-egismos-1.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:53:49.406151 circuitpython-laser-egismos-1.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:53:49.406151 circuitpython-laser-egismos-1.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-14 14:53:39.000000 circuitpython-laser-egismos-1.1.0/examples/laser_egismos_async_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-14 14:53:39.000000 circuitpython-laser-egismos-1.1.0/examples/laser_egismos_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11885 2023-05-14 14:53:39.000000 circuitpython-laser-egismos-1.1.0/laser_egismos.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-14 14:53:39.000000 circuitpython-laser-egismos-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 14:53:49.406151 circuitpython-laser-egismos-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:07:03.890231 circuitpython-laser-egismos-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:07:03.878231 circuitpython-laser-egismos-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:07:03.882231 circuitpython-laser-egismos-1.1.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:07:03.886231 circuitpython-laser-egismos-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:07:03.886231 circuitpython-laser-egismos-1.1.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-14 15:07:03.890231 circuitpython-laser-egismos-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:07:03.886231 circuitpython-laser-egismos-1.1.1/circuitpython_laser_egismos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-14 15:07:03.000000 circuitpython-laser-egismos-1.1.1/circuitpython_laser_egismos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-14 15:07:03.000000 circuitpython-laser-egismos-1.1.1/circuitpython_laser_egismos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 15:07:03.000000 circuitpython-laser-egismos-1.1.1/circuitpython_laser_egismos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-14 15:07:03.000000 circuitpython-laser-egismos-1.1.1/circuitpython_laser_egismos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-14 15:07:03.000000 circuitpython-laser-egismos-1.1.1/circuitpython_laser_egismos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:07:03.886231 circuitpython-laser-egismos-1.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:07:03.890231 circuitpython-laser-egismos-1.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:07:03.890231 circuitpython-laser-egismos-1.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-14 15:06:53.000000 circuitpython-laser-egismos-1.1.1/examples/laser_egismos_async_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-14 15:06:53.000000 circuitpython-laser-egismos-1.1.1/examples/laser_egismos_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-05-14 15:06:53.000000 circuitpython-laser-egismos-1.1.1/laser_egismos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-14 15:06:53.000000 circuitpython-laser-egismos-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-14 15:06:40.000000 circuitpython-laser-egismos-1.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 15:07:03.890231 circuitpython-laser-egismos-1.1.1/setup.cfg
```

### Comparing `circuitpython-laser-egismos-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-laser-egismos-1.1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.0/.gitignore` & `circuitpython-laser-egismos-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.0/.pre-commit-config.yaml` & `circuitpython-laser-egismos-1.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.0/.pylintrc` & `circuitpython-laser-egismos-1.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.0/CODE_OF_CONDUCT.md` & `circuitpython-laser-egismos-1.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.0/LICENSE` & `circuitpython-laser-egismos-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.0/LICENSES/CC-BY-4.0.txt` & `circuitpython-laser-egismos-1.1.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.0/LICENSES/MIT.txt` & `circuitpython-laser-egismos-1.1.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.0/LICENSES/Unlicense.txt` & `circuitpython-laser-egismos-1.1.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.0/PKG-INFO` & `circuitpython-laser-egismos-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-laser-egismos
-Version: 1.1.0
+Version: 1.1.1
 Summary: Device driver for the egismos series of lasers, available at https://www.egismos.com/laser-measuring-optoelectronics-module
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/furbrain/CircuitPython_laser_egismos
 Keywords: adafruit,blinka,circuitpython,micropython,laser_egismos,laser,egismos,rangefinder,distance
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-laser-egismos-1.1.0/README.rst` & `circuitpython-laser-egismos-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.0/circuitpython_laser_egismos.egg-info/PKG-INFO` & `circuitpython-laser-egismos-1.1.1/circuitpython_laser_egismos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-laser-egismos
-Version: 1.1.0
+Version: 1.1.1
 Summary: Device driver for the egismos series of lasers, available at https://www.egismos.com/laser-measuring-optoelectronics-module
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/furbrain/CircuitPython_laser_egismos
 Keywords: adafruit,blinka,circuitpython,micropython,laser_egismos,laser,egismos,rangefinder,distance
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-laser-egismos-1.1.0/circuitpython_laser_egismos.egg-info/SOURCES.txt` & `circuitpython-laser-egismos-1.1.1/circuitpython_laser_egismos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.0/docs/_static/favicon.ico` & `circuitpython-laser-egismos-1.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.0/docs/conf.py` & `circuitpython-laser-egismos-1.1.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     "sphinx.ext.todo",
 ]
 
 # TODO: Please Read!
 # Uncomment the below if you use native CircuitPython modules such as
 # digitalio, micropython and busio. List the modules you use. Without it, the
 # autodoc module docs will fail to generate with a warning.
-# autodoc_mock_imports = ["digitalio", "busio"]
+autodoc_mock_imports = ["digitalio", "busio", "asyncio"]
 
 autodoc_preserve_defaults = True
 
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
     "CircuitPython": ("https://docs.circuitpython.org/en/latest/", None),
```

### Comparing `circuitpython-laser-egismos-1.1.0/docs/index.rst` & `circuitpython-laser-egismos-1.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.0/examples/laser_egismos_async_test.py` & `circuitpython-laser-egismos-1.1.1/examples/laser_egismos_async_test.py`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.1.0/examples/laser_egismos_simpletest.py` & `circuitpython-laser-egismos-1.1.1/examples/laser_egismos_simpletest.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,20 +7,26 @@
 import board
 import busio
 import digitalio
 
 from laser_egismos import Laser
 
 periph_power = digitalio.DigitalInOut(board.D5)
-periph_power.switch_to_output(True)
+periph_power.switch_to_output(False)
 laser_power = digitalio.DigitalInOut(board.D0)
-laser_power.switch_to_output(True)
+laser_power.switch_to_output(False)
 
-time.sleep(0.5)
+time.sleep(0.3)
+print("power on")
+periph_power.switch_to_output(True)
+print("laser power enable")
+laser_power.switch_to_output(True)
+time.sleep(0.1)
 uart = busio.UART(board.D2, board.D1, baudrate=9600)
+print("start talking")
 laser = Laser(uart)
 laser.set_buzzer(False)
 laser.set_laser(True)
 time.sleep(1)
 laser.set_laser(False)
 time.sleep(0.1)
 print(f"Distance is {laser.distance}cm")
```

### Comparing `circuitpython-laser-egismos-1.1.0/laser_egismos.py` & `circuitpython-laser-egismos-1.1.1/laser_egismos.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   *  `Egismos laser <https://www.egismos.com/laser-measuring-optoelectronics-module>`_
 
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://circuitpython.org/downloads
 """
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 __repo__ = "https://github.com/furbrain/CircuitPython_laser_egismos.git"
 
 try:
     from typing import Sequence, Tuple
 except ImportError:
     pass
 
@@ -271,15 +271,15 @@
         :raises: Same as `measure`
         """
         return self.measure() / 10.0
 
 
 class AsyncLaser(_LaserBase):
     """
-    Same as `Laser`, but with async methods, requires the `~asyncio` module
+    Same as `Laser`, but with async methods, requires the `asyncio` module
     """
 
     def __init__(self, uart: busio.UART, address=0x01):
         # pylint: disable=import-outside-toplevel
         import asyncio
 
         uart.timeout = 0
```

### Comparing `circuitpython-laser-egismos-1.1.0/pyproject.toml` & `circuitpython-laser-egismos-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-laser-egismos"
 description = "Device driver for the egismos series of lasers, available at https://www.egismos.com/laser-measuring-optoelectronics-module"
-version = "1.1.0"
+version = "1.1.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/furbrain/CircuitPython_laser_egismos"}
 keywords = [
     "adafruit",
```

