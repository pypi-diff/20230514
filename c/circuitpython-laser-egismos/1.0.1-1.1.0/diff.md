# Comparing `tmp/circuitpython-laser-egismos-1.0.1.tar.gz` & `tmp/circuitpython-laser-egismos-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-laser-egismos-1.0.1.tar", last modified: Tue Apr 18 20:46:13 2023, max compression
+gzip compressed data, was "circuitpython-laser-egismos-1.1.0.tar", last modified: Sun May 14 14:53:49 2023, max compression
```

## Comparing `circuitpython-laser-egismos-1.0.1.tar` & `circuitpython-laser-egismos-1.1.0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:13.943187 circuitpython-laser-egismos-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:13.939187 circuitpython-laser-egismos-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:13.943187 circuitpython-laser-egismos-1.0.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-18 20:45:57.000000 circuitpython-laser-egismos-1.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:13.943187 circuitpython-laser-egismos-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-18 20:45:57.000000 circuitpython-laser-egismos-1.0.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-18 20:45:57.000000 circuitpython-laser-egismos-1.0.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-18 20:45:57.000000 circuitpython-laser-egismos-1.0.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-18 20:45:57.000000 circuitpython-laser-egismos-1.0.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-18 20:45:57.000000 circuitpython-laser-egismos-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-18 20:45:57.000000 circuitpython-laser-egismos-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-18 20:45:57.000000 circuitpython-laser-egismos-1.0.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-18 20:45:57.000000 circuitpython-laser-egismos-1.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-18 20:45:57.000000 circuitpython-laser-egismos-1.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-18 20:45:57.000000 circuitpython-laser-egismos-1.0.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:13.943187 circuitpython-laser-egismos-1.0.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-18 20:45:57.000000 circuitpython-laser-egismos-1.0.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-18 20:45:57.000000 circuitpython-laser-egismos-1.0.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-18 20:45:57.000000 circuitpython-laser-egismos-1.0.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-04-18 20:46:13.943187 circuitpython-laser-egismos-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-04-18 20:45:57.000000 circuitpython-laser-egismos-1.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-18 20:45:57.000000 circuitpython-laser-egismos-1.0.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:13.943187 circuitpython-laser-egismos-1.0.1/circuitpython_laser_egismos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-04-18 20:46:13.000000 circuitpython-laser-egismos-1.0.1/circuitpython_laser_egismos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-18 20:46:13.000000 circuitpython-laser-egismos-1.0.1/circuitpython_laser_egismos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:46:13.000000 circuitpython-laser-egismos-1.0.1/circuitpython_laser_egismos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-18 20:46:13.000000 circuitpython-laser-egismos-1.0.1/circuitpython_laser_egismos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 20:46:13.000000 circuitpython-laser-egismos-1.0.1/circuitpython_laser_egismos.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:13.943187 circuitpython-laser-egismos-1.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:13.943187 circuitpython-laser-egismos-1.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-18 20:45:57.000000 circuitpython-laser-egismos-1.0.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-18 20:45:57.000000 circuitpython-laser-egismos-1.0.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-18 20:45:57.000000 circuitpython-laser-egismos-1.0.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-18 20:45:57.000000 circuitpython-laser-egismos-1.0.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-04-18 20:45:57.000000 circuitpython-laser-egismos-1.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-18 20:45:57.000000 circuitpython-laser-egismos-1.0.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-18 20:45:57.000000 circuitpython-laser-egismos-1.0.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-18 20:45:57.000000 circuitpython-laser-egismos-1.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-18 20:45:57.000000 circuitpython-laser-egismos-1.0.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-18 20:45:57.000000 circuitpython-laser-egismos-1.0.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:13.943187 circuitpython-laser-egismos-1.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-18 20:46:06.000000 circuitpython-laser-egismos-1.0.1/examples/laser_egismos_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-04-18 20:46:06.000000 circuitpython-laser-egismos-1.0.1/laser_egismos.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-18 20:45:57.000000 circuitpython-laser-egismos-1.0.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-18 20:46:06.000000 circuitpython-laser-egismos-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-18 20:45:57.000000 circuitpython-laser-egismos-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:46:13.943187 circuitpython-laser-egismos-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:53:49.406151 circuitpython-laser-egismos-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:53:49.398151 circuitpython-laser-egismos-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:53:49.402151 circuitpython-laser-egismos-1.1.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:53:49.402151 circuitpython-laser-egismos-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:53:49.402151 circuitpython-laser-egismos-1.1.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-14 14:53:49.406151 circuitpython-laser-egismos-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:53:49.406151 circuitpython-laser-egismos-1.1.0/circuitpython_laser_egismos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-14 14:53:49.000000 circuitpython-laser-egismos-1.1.0/circuitpython_laser_egismos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-14 14:53:49.000000 circuitpython-laser-egismos-1.1.0/circuitpython_laser_egismos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 14:53:49.000000 circuitpython-laser-egismos-1.1.0/circuitpython_laser_egismos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-14 14:53:49.000000 circuitpython-laser-egismos-1.1.0/circuitpython_laser_egismos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-14 14:53:49.000000 circuitpython-laser-egismos-1.1.0/circuitpython_laser_egismos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:53:49.406151 circuitpython-laser-egismos-1.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:53:49.406151 circuitpython-laser-egismos-1.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:53:49.406151 circuitpython-laser-egismos-1.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-14 14:53:39.000000 circuitpython-laser-egismos-1.1.0/examples/laser_egismos_async_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-14 14:53:39.000000 circuitpython-laser-egismos-1.1.0/examples/laser_egismos_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11885 2023-05-14 14:53:39.000000 circuitpython-laser-egismos-1.1.0/laser_egismos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-14 14:53:39.000000 circuitpython-laser-egismos-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-14 14:53:27.000000 circuitpython-laser-egismos-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 14:53:49.406151 circuitpython-laser-egismos-1.1.0/setup.cfg
```

### Comparing `circuitpython-laser-egismos-1.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-laser-egismos-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.0.1/.gitignore` & `circuitpython-laser-egismos-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.0.1/.pre-commit-config.yaml` & `circuitpython-laser-egismos-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.0.1/.pylintrc` & `circuitpython-laser-egismos-1.1.0/.pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 # all. Valid levels: HIGH, INFERENCE, INFERENCE_FAILURE, UNDEFINED
 confidence=
 
 # Disable the message, report, category or checker with the given id(s). You
 # can either give multiple identifiers separated by comma (,) or put this
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once).You can also use "--disable=all" to
-# disable everything first and then reenable specific checks. For example, if
+# disable everything first and then re-enable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
 # disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
 disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
```

### Comparing `circuitpython-laser-egismos-1.0.1/CODE_OF_CONDUCT.md` & `circuitpython-laser-egismos-1.1.0/CODE_OF_CONDUCT.md`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 4. Moderators follow a soft "three strikes" policy - the community member may
    be given another chance, if they are receptive to the warning and change their
    behavior.
 5. If the community member is unreceptive or unreasonable when warned by a
    moderator, or the warning goes unheeded, they may be banned for a first or
    second offense. Repeated offenses will result in the community member being
    banned.
-6. Disciplinary actions (warnings, bans, etc) for Code of Conduct violations apply
+6. Disciplinary actions (warnings, bans, etc.) for Code of Conduct violations apply
    to the platform where the violation occurred. However, depending on the severity
    of the violation, the disciplinary action may be applied across CircuitPython's
    other community platforms. For example, a severe violation in one Community forum
    may result in a ban on not only the CircuitPython GitHub organisation,
    but also on the CircuitPython Twitter, live stream text chats, etc.
 
 ## Scope
```

### Comparing `circuitpython-laser-egismos-1.0.1/LICENSE` & `circuitpython-laser-egismos-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.0.1/LICENSES/CC-BY-4.0.txt` & `circuitpython-laser-egismos-1.1.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.0.1/LICENSES/MIT.txt` & `circuitpython-laser-egismos-1.1.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.0.1/LICENSES/Unlicense.txt` & `circuitpython-laser-egismos-1.1.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.0.1/PKG-INFO` & `circuitpython-laser-egismos-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-laser-egismos
-Version: 1.0.1
+Version: 1.1.0
 Summary: Device driver for the egismos series of lasers, available at https://www.egismos.com/laser-measuring-optoelectronics-module
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/furbrain/CircuitPython_laser_egismos
 Keywords: adafruit,blinka,circuitpython,micropython,laser_egismos,laser,egismos,rangefinder,distance
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -36,15 +36,16 @@
     :alt: Build Status
 
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
-Device driver for the egismos series of lasers, available at https://www.egismos.com/laser-measuring-optoelectronics-module
+Device driver for the egismos series of lasers, available at
+https://www.egismos.com/laser-measuring-optoelectronics-module
 
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
@@ -111,37 +112,37 @@
 
     import time
 
     import board
     import busio
     import digitalio
 
-    from laser_egismos import Laser, LaserCommandFailedError
+    from laser_egismos import Laser
 
     laser_power = digitalio.DigitalInOut(board.D10)
     laser_power.switch_to_output(True)
 
 
     uart = busio.UART(board.D8, board.D9, baudrate=9600)
     laser = Laser(uart)
-    print(laser._send_and_receive(laser.READ_SW_VERSION))
-    laser.buzzer_off()
-    laser.laser_on()
+    laser.set_buzzer(False)
+    laser.set_laser(True)
     time.sleep(3)
-    laser.laser_off()
+    laser.set_laser_(False)
     time.sleep(0.1)
     print(f"Distance is {laser.distance}cm")
 
 
 Documentation
 =============
-API documentation for this library can be found on `Read the Docs <https://circuitpython-laser-egismos.readthedocs.io/>`_.
+API documentation for this library can be found on `Read the Docs
+<https://circuitpython-laser-egismos.readthedocs.io/>`_.
 
-For information on building library documentation, please check out
-`this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+For information on building library documentation, please check out `this guide
+<https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/furbrain/CircuitPython_laser_egismos/blob/HEAD/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `circuitpython-laser-egismos-1.0.1/README.rst` & `circuitpython-laser-egismos-1.1.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     :alt: Build Status
 
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
-Device driver for the egismos series of lasers, available at https://www.egismos.com/laser-measuring-optoelectronics-module
+Device driver for the egismos series of lasers, available at
+https://www.egismos.com/laser-measuring-optoelectronics-module
 
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
@@ -93,37 +94,37 @@
 
     import time
 
     import board
     import busio
     import digitalio
 
-    from laser_egismos import Laser, LaserCommandFailedError
+    from laser_egismos import Laser
 
     laser_power = digitalio.DigitalInOut(board.D10)
     laser_power.switch_to_output(True)
 
 
     uart = busio.UART(board.D8, board.D9, baudrate=9600)
     laser = Laser(uart)
-    print(laser._send_and_receive(laser.READ_SW_VERSION))
-    laser.buzzer_off()
-    laser.laser_on()
+    laser.set_buzzer(False)
+    laser.set_laser(True)
     time.sleep(3)
-    laser.laser_off()
+    laser.set_laser_(False)
     time.sleep(0.1)
     print(f"Distance is {laser.distance}cm")
 
 
 Documentation
 =============
-API documentation for this library can be found on `Read the Docs <https://circuitpython-laser-egismos.readthedocs.io/>`_.
+API documentation for this library can be found on `Read the Docs
+<https://circuitpython-laser-egismos.readthedocs.io/>`_.
 
-For information on building library documentation, please check out
-`this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+For information on building library documentation, please check out `this guide
+<https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/furbrain/CircuitPython_laser_egismos/blob/HEAD/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `circuitpython-laser-egismos-1.0.1/circuitpython_laser_egismos.egg-info/PKG-INFO` & `circuitpython-laser-egismos-1.1.0/circuitpython_laser_egismos.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-laser-egismos
-Version: 1.0.1
+Version: 1.1.0
 Summary: Device driver for the egismos series of lasers, available at https://www.egismos.com/laser-measuring-optoelectronics-module
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/furbrain/CircuitPython_laser_egismos
 Keywords: adafruit,blinka,circuitpython,micropython,laser_egismos,laser,egismos,rangefinder,distance
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -36,15 +36,16 @@
     :alt: Build Status
 
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
-Device driver for the egismos series of lasers, available at https://www.egismos.com/laser-measuring-optoelectronics-module
+Device driver for the egismos series of lasers, available at
+https://www.egismos.com/laser-measuring-optoelectronics-module
 
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
@@ -111,37 +112,37 @@
 
     import time
 
     import board
     import busio
     import digitalio
 
-    from laser_egismos import Laser, LaserCommandFailedError
+    from laser_egismos import Laser
 
     laser_power = digitalio.DigitalInOut(board.D10)
     laser_power.switch_to_output(True)
 
 
     uart = busio.UART(board.D8, board.D9, baudrate=9600)
     laser = Laser(uart)
-    print(laser._send_and_receive(laser.READ_SW_VERSION))
-    laser.buzzer_off()
-    laser.laser_on()
+    laser.set_buzzer(False)
+    laser.set_laser(True)
     time.sleep(3)
-    laser.laser_off()
+    laser.set_laser_(False)
     time.sleep(0.1)
     print(f"Distance is {laser.distance}cm")
 
 
 Documentation
 =============
-API documentation for this library can be found on `Read the Docs <https://circuitpython-laser-egismos.readthedocs.io/>`_.
+API documentation for this library can be found on `Read the Docs
+<https://circuitpython-laser-egismos.readthedocs.io/>`_.
 
-For information on building library documentation, please check out
-`this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+For information on building library documentation, please check out `this guide
+<https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/furbrain/CircuitPython_laser_egismos/blob/HEAD/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `circuitpython-laser-egismos-1.0.1/circuitpython_laser_egismos.egg-info/SOURCES.txt` & `circuitpython-laser-egismos-1.1.0/circuitpython_laser_egismos.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -29,8 +29,9 @@
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
 docs/requirements.txt
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
+examples/laser_egismos_async_test.py
 examples/laser_egismos_simpletest.py
```

### Comparing `circuitpython-laser-egismos-1.0.1/docs/_static/favicon.ico` & `circuitpython-laser-egismos-1.1.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.0.1/docs/conf.py` & `circuitpython-laser-egismos-1.1.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 
 if not on_rtd:  # only import and set the theme if we're building docs locally
     try:
         import sphinx_rtd_theme
 
         html_theme = "sphinx_rtd_theme"
         html_theme_path = [sphinx_rtd_theme.get_html_theme_path(), "."]
-    except:
+    except ImportError:
         html_theme = "default"
         html_theme_path = ["."]
 else:
     html_theme_path = ["."]
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
```

### Comparing `circuitpython-laser-egismos-1.0.1/docs/index.rst` & `circuitpython-laser-egismos-1.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-laser-egismos-1.0.1/examples/laser_egismos_simpletest.py` & `circuitpython-laser-egismos-1.1.0/examples/laser_egismos_simpletest.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 
 import board
 import busio
 import digitalio
 
 from laser_egismos import Laser
 
-laser_power = digitalio.DigitalInOut(board.D10)
+periph_power = digitalio.DigitalInOut(board.D5)
+periph_power.switch_to_output(True)
+laser_power = digitalio.DigitalInOut(board.D0)
 laser_power.switch_to_output(True)
 
-
-uart = busio.UART(board.D8, board.D9, baudrate=9600)
+time.sleep(0.5)
+uart = busio.UART(board.D2, board.D1, baudrate=9600)
 laser = Laser(uart)
-laser.buzzer_off()
-laser.laser_on()
-time.sleep(3)
-laser.laser_off()
+laser.set_buzzer(False)
+laser.set_laser(True)
+time.sleep(1)
+laser.set_laser(False)
 time.sleep(0.1)
 print(f"Distance is {laser.distance}cm")
```

### Comparing `circuitpython-laser-egismos-1.0.1/pyproject.toml` & `circuitpython-laser-egismos-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-laser-egismos"
 description = "Device driver for the egismos series of lasers, available at https://www.egismos.com/laser-measuring-optoelectronics-module"
-version = "1.0.1"
+version = "1.1.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/furbrain/CircuitPython_laser_egismos"}
 keywords = [
     "adafruit",
```

