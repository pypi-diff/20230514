# Comparing `tmp/lsst-pex-config-26.0.0a20230400.tar.gz` & `tmp/lsst-pex-config-26.0.0a20230500.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst-pex-config-26.0.0a20230400.tar", last modified: Thu Jan 26 09:54:51 2023, max compression
+gzip compressed data, was "lsst-pex-config-26.0.0a20230500.tar", last modified: Thu Feb  2 14:03:38 2023, max compression
```

## Comparing `lsst-pex-config-26.0.0a20230400.tar` & `lsst-pex-config-26.0.0a20230500.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 09:54:51.293927 lsst-pex-config-26.0.0a20230400/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-01-26 09:54:51.293927 lsst-pex-config-26.0.0a20230400/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/bsd_license.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 09:54:51.285926 lsst-pex-config-26.0.0a20230400/doc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 09:54:51.289927 lsst-pex-config-26.0.0a20230400/doc/lsst.pex.config/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/doc/lsst.pex.config/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/doc/lsst.pex.config/design-notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/doc/lsst.pex.config/field-types.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/doc/lsst.pex.config/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/doc/lsst.pex.config/inspecting-configs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/doc/lsst.pex.config/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/doc/lsst.pex.config/registry-intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/doc/lsst.pex.config/wrapping-cpp-control-objects.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/gpl-v3.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 09:54:51.285926 lsst-pex-config-26.0.0a20230400/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 09:54:51.289927 lsst-pex-config-26.0.0a20230400/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 09:54:51.289927 lsst-pex-config-26.0.0a20230400/python/lsst/pex/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/python/lsst/pex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 09:54:51.289927 lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/_doNotImportMe.py
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/callStack.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/choiceField.py
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)    60275 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    23443 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/configChoiceField.py
--rw-r--r--   0 runner    (1001) docker     (123)    10744 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/configDictField.py
--rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/configField.py
--rw-r--r--   0 runner    (1001) docker     (123)    17219 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/configurableField.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    16441 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/dictField.py
--rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/history.py
--rw-r--r--   0 runner    (1001) docker     (123)    18512 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/listField.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/rangeField.py
--rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-26 09:54:51.000000 lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12634 2023-01-26 09:54:36.000000 lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 09:54:51.293927 lsst-pex-config-26.0.0a20230400/python/lsst_pex_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-01-26 09:54:51.000000 lsst-pex-config-26.0.0a20230400/python/lsst_pex_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-01-26 09:54:51.000000 lsst-pex-config-26.0.0a20230400/python/lsst_pex_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 09:54:51.000000 lsst-pex-config-26.0.0a20230400/python/lsst_pex_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-26 09:54:51.000000 lsst-pex-config-26.0.0a20230400/python/lsst_pex_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-26 09:54:51.000000 lsst-pex-config-26.0.0a20230400/python/lsst_pex_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 09:54:50.000000 lsst-pex-config-26.0.0a20230400/python/lsst_pex_config.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-01-26 09:54:51.293927 lsst-pex-config-26.0.0a20230400/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 14:03:38.266938 lsst-pex-config-26.0.0a20230500/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-02-02 14:03:38.266938 lsst-pex-config-26.0.0a20230500/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/bsd_license.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 14:03:38.258938 lsst-pex-config-26.0.0a20230500/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 14:03:38.262938 lsst-pex-config-26.0.0a20230500/doc/lsst.pex.config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/doc/lsst.pex.config/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/doc/lsst.pex.config/design-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/doc/lsst.pex.config/field-types.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/doc/lsst.pex.config/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/doc/lsst.pex.config/inspecting-configs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/doc/lsst.pex.config/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/doc/lsst.pex.config/registry-intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/doc/lsst.pex.config/wrapping-cpp-control-objects.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/gpl-v3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 14:03:38.258938 lsst-pex-config-26.0.0a20230500/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 14:03:38.262938 lsst-pex-config-26.0.0a20230500/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 14:03:38.262938 lsst-pex-config-26.0.0a20230500/python/lsst/pex/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/python/lsst/pex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 14:03:38.266938 lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/_doNotImportMe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/callStack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/choiceField.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60214 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23443 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/configChoiceField.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10744 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/configDictField.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/configField.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17215 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/configurableField.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16441 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/dictField.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18489 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/listField.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/rangeField.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-02 14:03:37.000000 lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12634 2023-02-02 14:03:18.000000 lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 14:03:38.266938 lsst-pex-config-26.0.0a20230500/python/lsst_pex_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-02-02 14:03:38.000000 lsst-pex-config-26.0.0a20230500/python/lsst_pex_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-02-02 14:03:38.000000 lsst-pex-config-26.0.0a20230500/python/lsst_pex_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 14:03:38.000000 lsst-pex-config-26.0.0a20230500/python/lsst_pex_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-02 14:03:38.000000 lsst-pex-config-26.0.0a20230500/python/lsst_pex_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-02 14:03:38.000000 lsst-pex-config-26.0.0a20230500/python/lsst_pex_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 14:03:37.000000 lsst-pex-config-26.0.0a20230500/python/lsst_pex_config.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-02-02 14:03:38.270938 lsst-pex-config-26.0.0a20230500/setup.cfg
```

### Comparing `lsst-pex-config-26.0.0a20230400/PKG-INFO` & `lsst-pex-config-26.0.0a20230500/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-pex-config
-Version: 26.0.0a20230400
+Version: 26.0.0a20230500
 Summary: A flexible configuration system using Python files.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License, GPLv3+
 Project-URL: Homepage, https://github.com/lsst/pex_config
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-pex-config-26.0.0a20230400/README.rst` & `lsst-pex-config-26.0.0a20230500/README.rst`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.0.0a20230400/bsd_license.txt` & `lsst-pex-config-26.0.0a20230500/bsd_license.txt`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.0.0a20230400/doc/lsst.pex.config/CHANGES.rst` & `lsst-pex-config-26.0.0a20230500/doc/lsst.pex.config/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.0.0a20230400/doc/lsst.pex.config/design-notes.rst` & `lsst-pex-config-26.0.0a20230500/doc/lsst.pex.config/design-notes.rst`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.0.0a20230400/doc/lsst.pex.config/field-types.rst` & `lsst-pex-config-26.0.0a20230500/doc/lsst.pex.config/field-types.rst`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         )
 
 Examples of `ChoiceField` and `ConfigField` and the use of the `Config` object's `Config.setDefaults` and `Config.validate` methods:
 
 .. code-block:: python
 
     class InitialPsfConfig(pexConfig.Config):
-        """A config that describes the initial PSF used 
+        """A config that describes the initial PSF used
         for detection and measurement (before PSF
         determination is done).
         """
 
         model = pexConfig.ChoiceField(
             dtype=str,
             doc="PSF model type.",
```

### Comparing `lsst-pex-config-26.0.0a20230400/doc/lsst.pex.config/index.rst` & `lsst-pex-config-26.0.0a20230500/doc/lsst.pex.config/index.rst`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.0.0a20230400/doc/lsst.pex.config/inspecting-configs.rst` & `lsst-pex-config-26.0.0a20230500/doc/lsst.pex.config/inspecting-configs.rst`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.0.0a20230400/doc/lsst.pex.config/overview.rst` & `lsst-pex-config-26.0.0a20230500/doc/lsst.pex.config/overview.rst`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 ==============================
 
 Here is a config class that includes five fields:
 
 .. code-block:: python
 
    import lsst.pex.config as pexConfig
-   
+
    class IsrTaskConfig(pexConfig.Config):
        doWrite = pexConfig.Field(
            doc="Write output?",
            dtype=bool,
            default=True)
        fwhm = pexConfig.Field(
            doc="FWHM of PSF (arcsec)",
```

### Comparing `lsst-pex-config-26.0.0a20230400/doc/lsst.pex.config/registry-intro.rst` & `lsst-pex-config-26.0.0a20230500/doc/lsst.pex.config/registry-intro.rst`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.0.0a20230400/doc/lsst.pex.config/wrapping-cpp-control-objects.rst` & `lsst-pex-config-26.0.0a20230500/doc/lsst.pex.config/wrapping-cpp-control-objects.rst`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 For example, here is a C++ control object:
 
 .. code-block:: c++
 
     struct FooControl {
         LSST_CONTROL_FIELD(bar, int, "documentation for field 'bar'");
         LSST_CONTROL_FIELD(baz, double, "documentation for field 'baz'");
-        
+
         FooControl() : bar(0), baz(0.0) {}
     };
 
 Note that only ``bool``, ``int``, ``double``, and ``std::string`` fields, along with ``std::list`` and ``std::vector`` objects of those types, are fully supported.
 Nested control objects are not supported.
 
 After using pybind11, the preferred way to create the `Config` is via the `wrap` decorator:
```

### Comparing `lsst-pex-config-26.0.0a20230400/gpl-v3.0.txt` & `lsst-pex-config-26.0.0a20230500/gpl-v3.0.txt`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.0.0a20230400/pyproject.toml` & `lsst-pex-config-26.0.0a20230500/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 "lsst.pex.config" = ["py.typed"]
 
 [tool.setuptools.dynamic]
 version = { attr = "lsst_versions.get_lsst_version" }
 
 [tool.black]
 line-length = 110
-target-version = ["py38"]
+target-version = ["py310"]
 
 [tool.isort]
 profile = "black"
 line_length = 110
 
 [tool.towncrier]
     package = "lsst.pex.config"
```

### Comparing `lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/__init__.py` & `lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/callStack.py` & `lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/callStack.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/choiceField.py` & `lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/choiceField.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/comparison.py` & `lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/comparison.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/config.py` & `lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -739,17 +739,15 @@
             try:
                 return instance._storage[self.name]
             except AttributeError:
                 if not isinstance(instance, Config):
                     return self
                 else:
                     raise AttributeError(
-                        f"Config {instance} is missing "
-                        "_storage attribute, likely"
-                        " incorrectly initialized"
+                        f"Config {instance} is missing _storage attribute, likely incorrectly initialized"
                     )
 
     def __set__(
         self, instance: "Config", value: Optional[FieldTypeVar], at: Any = None, label: str = "assignment"
     ) -> None:
         """Set an attribute on the config instance.
 
@@ -1686,15 +1684,15 @@
     # Do a single regex to avoid large string copies when splitting a
     # large config into separate lines.
     matches = re.search(r"^import ([\w.]+)\nassert .*==(.*?),", config_py)
 
     if not matches:
         first_line, second_line, _ = config_py.split("\n", 2)
         raise ValueError(
-            "First two lines did not match expected form. Got:\n" f" - {first_line}\n" f" - {second_line}"
+            f"First two lines did not match expected form. Got:\n - {first_line}\n - {second_line}"
         )
 
     module_name = matches.group(1)
     module = importlib.import_module(module_name)
 
     # Second line
     full_name = matches.group(2)
```

### Comparing `lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/configChoiceField.py` & `lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/configChoiceField.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/configDictField.py` & `lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/configDictField.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/configField.py` & `lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/configField.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/configurableField.py` & `lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/configurableField.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
                 at = getCallStack()
             self._value.__delattr__(name, at=at, label=label)
 
     def __reduce__(self):
         raise UnexpectedProxyUsageError(
             f"Proxy object for config field {self._field.name} cannot "
             "be pickled; it should be converted to a normal `Config` instance "
-            f"via the `value` property before being assigned to other objects "
+            "via the `value` property before being assigned to other objects "
             "or variables."
         )
 
 
 class ConfigurableField(Field[ConfigurableInstance[FieldTypeVar]]):
     """A configuration field (`~lsst.pex.config.Field` subclass) that can be
     can be retargeted towards a different configurable (often a
@@ -272,16 +272,16 @@
         if ConfigClass is None:
             try:
                 ConfigClass = target.ConfigClass
             except Exception:
                 raise AttributeError("'target' must define attribute 'ConfigClass'")
         if not issubclass(ConfigClass, Config):
             raise TypeError(
-                "'ConfigClass' is of incorrect type %s."
-                "'ConfigClass' must be a subclass of Config" % _typeStr(ConfigClass)
+                "'ConfigClass' is of incorrect type %s.'ConfigClass' must be a subclass of Config"
+                % _typeStr(ConfigClass)
             )
         if not hasattr(target, "__call__"):
             raise ValueError("'target' must be callable")
         if not hasattr(target, "__module__") or not hasattr(target, "__name__"):
             raise ValueError(
                 "'target' must be statically defined (must have '__module__' and '__name__' attributes)"
             )
```

### Comparing `lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/convert.py` & `lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/convert.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/dictField.py` & `lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/dictField.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/history.py` & `lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/history.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/listField.py` & `lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/listField.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,16 +342,15 @@
             minLength = None
             maxLength = None
         else:
             if maxLength is not None and maxLength <= 0:
                 raise ValueError("'maxLength' (%d) must be positive" % maxLength)
             if minLength is not None and maxLength is not None and minLength > maxLength:
                 raise ValueError(
-                    "'maxLength' (%d) must be at least"
-                    " as large as 'minLength' (%d)" % (maxLength, minLength)
+                    "'maxLength' (%d) must be at least as large as 'minLength' (%d)" % (maxLength, minLength)
                 )
 
         if listCheck is not None and not hasattr(listCheck, "__call__"):
             raise ValueError("'listCheck' must be callable")
         if itemCheck is not None and not hasattr(itemCheck, "__call__"):
             raise ValueError("'itemCheck' must be callable")
```

### Comparing `lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/rangeField.py` & `lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/rangeField.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/registry.py` & `lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/registry.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.0.0a20230400/python/lsst/pex/config/wrap.py` & `lsst-pex-config-26.0.0a20230500/python/lsst/pex/config/wrap.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.0.0a20230400/python/lsst_pex_config.egg-info/PKG-INFO` & `lsst-pex-config-26.0.0a20230500/python/lsst_pex_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-pex-config
-Version: 26.0.0a20230400
+Version: 26.0.0a20230500
 Summary: A flexible configuration system using Python files.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License, GPLv3+
 Project-URL: Homepage, https://github.com/lsst/pex_config
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-pex-config-26.0.0a20230400/python/lsst_pex_config.egg-info/SOURCES.txt` & `lsst-pex-config-26.0.0a20230500/python/lsst_pex_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

