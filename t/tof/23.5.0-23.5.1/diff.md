# Comparing `tmp/tof-23.5.0.tar.gz` & `tmp/tof-23.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tof-23.5.0.tar", last modified: Fri May 12 11:01:54 2023, max compression
+gzip compressed data, was "tof-23.5.1.tar", last modified: Sun May 14 07:53:46 2023, max compression
```

## Comparing `tof-23.5.0.tar` & `tof-23.5.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:01:54.479665 tof-23.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-12 11:01:42.000000 tof-23.5.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:01:54.467665 tof-23.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:01:54.471665 tof-23.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-12 11:01:42.000000 tof-23.5.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-12 11:01:42.000000 tof-23.5.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-12 11:01:42.000000 tof-23.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-12 11:01:42.000000 tof-23.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-12 11:01:42.000000 tof-23.5.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-12 11:01:42.000000 tof-23.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-12 11:01:54.479665 tof-23.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-12 11:01:42.000000 tof-23.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:01:54.471665 tof-23.5.0/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-12 11:01:42.000000 tof-23.5.0/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:01:54.475665 tof-23.5.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:01:54.475665 tof-23.5.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    22254 2023-05-12 11:01:42.000000 tof-23.5.0/docs/_static/detector.png
--rw-r--r--   0 runner    (1001) docker     (123)   137750 2023-05-12 11:01:42.000000 tof-23.5.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-05-12 11:01:42.000000 tof-23.5.0/docs/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    96012 2023-05-12 11:01:42.000000 tof-23.5.0/docs/_static/model.png
--rw-r--r--   0 runner    (1001) docker     (123)    32531 2023-05-12 11:01:42.000000 tof-23.5.0/docs/_static/pulse.png
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-12 11:01:42.000000 tof-23.5.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-05-12 11:01:42.000000 tof-23.5.0/docs/components.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-12 11:01:42.000000 tof-23.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-12 11:01:42.000000 tof-23.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-05-12 11:01:42.000000 tof-23.5.0/docs/pulses.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-12 11:01:42.000000 tof-23.5.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-05-12 11:01:42.000000 tof-23.5.0/docs/short-example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-12 11:01:42.000000 tof-23.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:01:54.475665 tof-23.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 11:01:42.000000 tof-23.5.0/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-12 11:01:42.000000 tof-23.5.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-12 11:01:42.000000 tof-23.5.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-05-12 11:01:42.000000 tof-23.5.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-12 11:01:42.000000 tof-23.5.0/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-12 11:01:42.000000 tof-23.5.0/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 11:01:42.000000 tof-23.5.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-12 11:01:42.000000 tof-23.5.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-12 11:01:42.000000 tof-23.5.0/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-12 11:01:42.000000 tof-23.5.0/requirements/wheels.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 11:01:54.479665 tof-23.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:01:54.467665 tof-23.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:01:54.471665 tof-23.5.0/src/tof/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-12 11:01:42.000000 tof-23.5.0/src/tof/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-12 11:01:42.000000 tof-23.5.0/src/tof/chopper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-12 11:01:42.000000 tof-23.5.0/src/tof/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-12 11:01:42.000000 tof-23.5.0/src/tof/detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:01:54.471665 tof-23.5.0/src/tof/facilities/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-12 11:01:42.000000 tof-23.5.0/src/tof/facilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-05-12 11:01:42.000000 tof-23.5.0/src/tof/facilities/ess_pulse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-05-12 11:01:42.000000 tof-23.5.0/src/tof/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13337 2023-05-12 11:01:42.000000 tof-23.5.0/src/tof/pulse.py
--rw-r--r--   0 runner    (1001) docker     (123)    10689 2023-05-12 11:01:42.000000 tof-23.5.0/src/tof/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-12 11:01:42.000000 tof-23.5.0/src/tof/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:01:54.471665 tof-23.5.0/src/tof.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-12 11:01:54.000000 tof-23.5.0/src/tof.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-12 11:01:54.000000 tof-23.5.0/src/tof.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 11:01:54.000000 tof-23.5.0/src/tof.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 11:01:54.000000 tof-23.5.0/src/tof.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-12 11:01:54.000000 tof-23.5.0/src/tof.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:01:54.475665 tof-23.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-12 11:01:42.000000 tof-23.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-12 11:01:42.000000 tof-23.5.0/tests/chopper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-12 11:01:42.000000 tof-23.5.0/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-05-12 11:01:42.000000 tof-23.5.0/tests/model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-12 11:01:42.000000 tof-23.5.0/tests/pulse_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-12 11:01:42.000000 tof-23.5.0/tests/result_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-12 11:01:42.000000 tof-23.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:53:46.824364 tof-23.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-14 07:53:28.000000 tof-23.5.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:53:46.804363 tof-23.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:53:46.812363 tof-23.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-14 07:53:28.000000 tof-23.5.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-14 07:53:28.000000 tof-23.5.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-14 07:53:28.000000 tof-23.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-14 07:53:28.000000 tof-23.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-14 07:53:28.000000 tof-23.5.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-14 07:53:28.000000 tof-23.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-14 07:53:46.820363 tof-23.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-14 07:53:28.000000 tof-23.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:53:46.812363 tof-23.5.1/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-14 07:53:28.000000 tof-23.5.1/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:53:46.816363 tof-23.5.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:53:46.816363 tof-23.5.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    22254 2023-05-14 07:53:28.000000 tof-23.5.1/docs/_static/detector.png
+-rw-r--r--   0 runner    (1001) docker     (123)   137750 2023-05-14 07:53:28.000000 tof-23.5.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-05-14 07:53:28.000000 tof-23.5.1/docs/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    96012 2023-05-14 07:53:28.000000 tof-23.5.1/docs/_static/model.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32531 2023-05-14 07:53:28.000000 tof-23.5.1/docs/_static/pulse.png
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-14 07:53:28.000000 tof-23.5.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-05-14 07:53:28.000000 tof-23.5.1/docs/components.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-14 07:53:28.000000 tof-23.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-14 07:53:28.000000 tof-23.5.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-05-14 07:53:28.000000 tof-23.5.1/docs/pulses.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-14 07:53:28.000000 tof-23.5.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-05-14 07:53:28.000000 tof-23.5.1/docs/short-example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-14 07:53:28.000000 tof-23.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:53:46.820363 tof-23.5.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-14 07:53:28.000000 tof-23.5.1/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-14 07:53:28.000000 tof-23.5.1/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-14 07:53:28.000000 tof-23.5.1/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-05-14 07:53:28.000000 tof-23.5.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-14 07:53:28.000000 tof-23.5.1/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-14 07:53:28.000000 tof-23.5.1/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-14 07:53:28.000000 tof-23.5.1/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-14 07:53:28.000000 tof-23.5.1/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 07:53:28.000000 tof-23.5.1/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-14 07:53:28.000000 tof-23.5.1/requirements/wheels.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 07:53:46.824364 tof-23.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:53:46.804363 tof-23.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:53:46.812363 tof-23.5.1/src/tof/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-14 07:53:28.000000 tof-23.5.1/src/tof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-14 07:53:28.000000 tof-23.5.1/src/tof/chopper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-14 07:53:28.000000 tof-23.5.1/src/tof/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-14 07:53:28.000000 tof-23.5.1/src/tof/detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:53:46.812363 tof-23.5.1/src/tof/facilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-14 07:53:28.000000 tof-23.5.1/src/tof/facilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-05-14 07:53:28.000000 tof-23.5.1/src/tof/facilities/ess_pulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-05-14 07:53:28.000000 tof-23.5.1/src/tof/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13352 2023-05-14 07:53:28.000000 tof-23.5.1/src/tof/pulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-05-14 07:53:28.000000 tof-23.5.1/src/tof/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-14 07:53:28.000000 tof-23.5.1/src/tof/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:53:46.812363 tof-23.5.1/src/tof.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-14 07:53:46.000000 tof-23.5.1/src/tof.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-14 07:53:46.000000 tof-23.5.1/src/tof.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 07:53:46.000000 tof-23.5.1/src/tof.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 07:53:46.000000 tof-23.5.1/src/tof.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-14 07:53:46.000000 tof-23.5.1/src/tof.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:53:46.820363 tof-23.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-14 07:53:28.000000 tof-23.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-14 07:53:28.000000 tof-23.5.1/tests/chopper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-14 07:53:28.000000 tof-23.5.1/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-05-14 07:53:28.000000 tof-23.5.1/tests/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-05-14 07:53:28.000000 tof-23.5.1/tests/pulse_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-14 07:53:28.000000 tof-23.5.1/tests/result_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-14 07:53:28.000000 tof-23.5.1/tox.ini
```

### Comparing `tof-23.5.0/.github/workflows/ci.yml` & `tof-23.5.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/.github/workflows/release.yml` & `tof-23.5.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/.pre-commit-config.yaml` & `tof-23.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/LICENSE` & `tof-23.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/PKG-INFO` & `tof-23.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tof
-Version: 23.5.0
+Version: 23.5.1
 Summary: A simple tool to create time-of-flight chopper cascade diagrams
 Author: Neil Vaytet
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `tof-23.5.0/README.md` & `tof-23.5.1/README.md`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/conda/meta.yaml` & `tof-23.5.1/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/docs/_static/detector.png` & `tof-23.5.1/docs/_static/detector.png`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/docs/_static/favicon.ico` & `tof-23.5.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/docs/_static/logo.svg` & `tof-23.5.1/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/docs/_static/model.png` & `tof-23.5.1/docs/_static/model.png`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/docs/_static/pulse.png` & `tof-23.5.1/docs/_static/pulse.png`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/docs/components.ipynb` & `tof-23.5.1/docs/components.ipynb`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/docs/conf.py` & `tof-23.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/docs/index.rst` & `tof-23.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/docs/pulses.ipynb` & `tof-23.5.1/docs/pulses.ipynb`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/docs/short-example.ipynb` & `tof-23.5.1/docs/short-example.ipynb`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/pyproject.toml` & `tof-23.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/requirements/ci.txt` & `tof-23.5.1/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/requirements/docs.txt` & `tof-23.5.1/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/requirements/static.txt` & `tof-23.5.1/requirements/static.txt`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/src/tof/chopper.py` & `tof-23.5.1/src/tof/chopper.py`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/src/tof/component.py` & `tof-23.5.1/src/tof/component.py`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/src/tof/detector.py` & `tof-23.5.1/src/tof/detector.py`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/src/tof/facilities/ess_pulse.py` & `tof-23.5.1/src/tof/facilities/ess_pulse.py`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/src/tof/model.py` & `tof-23.5.1/src/tof/model.py`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/src/tof/pulse.py` & `tof-23.5.1/src/tof/pulse.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,24 +226,24 @@
         tmax: Optional[sc.Variable] = None,
         wmin: Optional[sc.Variable] = None,
         wmax: Optional[sc.Variable] = None,
         neutrons: int = 1_000_000,
         sampling: int = 1000,
     ):
         self.facility = facility
-        self.neutrons = neutrons
+        self.neutrons = int(neutrons)
 
         if facility is not None:
-            dists = getattr(facilities, facility)
+            dists = getattr(facilities, self.facility)
             params = _make_pulse(
                 tmin=tmin,
                 tmax=tmax,
                 wmin=wmin,
                 wmax=wmax,
-                neutrons=neutrons,
+                neutrons=self.neutrons,
                 p_time=dists.time,
                 p_wav=dists.wavelength,
                 sampling=sampling,
             )
             self.birth_times = params['birth_times']
             self.wavelengths = params['wavelengths']
             self.speeds = params['speeds']
```

### Comparing `tof-23.5.0/src/tof/result.py` & `tof-23.5.1/src/tof/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,23 +256,24 @@
                 cbar=cbar,
                 wavelengths=wavelengths,
                 wmin=self._pulse.wmin,
                 wmax=self._pulse.wmax,
             )
 
         tof_max = tofs.max().value
+        dx = 0.05 * tof_max
         # Plot choppers
         for ch in self._choppers.values():
             x0 = ch.open_times.to(unit='us').values
             x1 = ch.close_times.to(unit='us').values
             x = np.empty(3 * x0.size, dtype=x0.dtype)
             x[0::3] = x0
             x[1::3] = 0.5 * (x0 + x1)
             x[2::3] = x1
-            x = np.concatenate([[0], x])
+            x = np.concatenate([[0], x] + ([[tof_max + dx]] if x[-1] < tof_max else []))
             y = np.full_like(x, ch.distance.value)
             y[2::3] = None
             ax.plot(x, y, color="k")
             ax.text(
                 tof_max, ch.distance.value, ch.name, ha="right", va="bottom", color="k"
             )
 
@@ -291,15 +292,14 @@
             color="gray",
             lw=3,
         )
         ax.text(tmin, 0, "Pulse", ha="left", va="top", color="gray")
 
         ax.set_xlabel("Time-of-flight (us)")
         ax.set_ylabel("Distance (m)")
-        dx = 0.05 * tof_max
         ax.set_xlim(0 - dx, tof_max + dx)
         fig.tight_layout()
         return Plot(fig=fig, ax=ax)
 
     def __repr__(self) -> str:
         out = f"Result:\n  Pulse: {self._pulse.neutrons} neutrons.\n  Choppers:\n"
         for name, ch in self._choppers.items():
```

### Comparing `tof-23.5.0/src/tof/utils.py` & `tof-23.5.1/src/tof/utils.py`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/src/tof.egg-info/PKG-INFO` & `tof-23.5.1/src/tof.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tof
-Version: 23.5.0
+Version: 23.5.1
 Summary: A simple tool to create time-of-flight chopper cascade diagrams
 Author: Neil Vaytet
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `tof-23.5.0/src/tof.egg-info/SOURCES.txt` & `tof-23.5.1/src/tof.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/tests/chopper_test.py` & `tof-23.5.1/tests/chopper_test.py`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/tests/common.py` & `tof-23.5.1/tests/common.py`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/tests/model_test.py` & `tof-23.5.1/tests/model_test.py`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/tests/pulse_test.py` & `tof-23.5.1/tests/pulse_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,7 +144,12 @@
     a = pulse_float.birth_times.hist(time=tedges).data
     b = pulse_int.birth_times.hist(time=tedges).data
     c = pulse_float.wavelengths.hist(wavelength=wedges).data
     d = pulse_int.wavelengths.hist(wavelength=wedges).data
 
     assert sc.allclose(a, b, atol=0.1 * a.max())
     assert sc.allclose(c, d, atol=0.1 * c.max())
+
+
+def test_non_integer_neutrons():
+    pulse = tof.Pulse(facility='ess', neutrons=1e5)
+    assert pulse.neutrons == 100_000
```

### Comparing `tof-23.5.0/tests/result_test.py` & `tof-23.5.1/tests/result_test.py`

 * *Files identical despite different names*

### Comparing `tof-23.5.0/tox.ini` & `tof-23.5.1/tox.ini`

 * *Files identical despite different names*

