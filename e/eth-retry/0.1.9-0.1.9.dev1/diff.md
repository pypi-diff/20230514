# Comparing `tmp/eth_retry-0.1.9.tar.gz` & `tmp/eth_retry-0.1.9.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth_retry-0.1.9.tar", last modified: Mon Oct  3 17:27:12 2022, max compression
+gzip compressed data, was "eth_retry-0.1.9.dev1.tar", last modified: Mon Oct  3 17:27:02 2022, max compression
```

## Comparing `eth_retry-0.1.9.tar` & `eth_retry-0.1.9.dev1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 17:27:12.834892 eth_retry-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-10-03 17:27:02.000000 eth_retry-0.1.9/.env.sample
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 17:27:12.830892 eth_retry-0.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 17:27:12.834892 eth_retry-0.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-10-03 17:27:02.000000 eth_retry-0.1.9/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-10-03 17:27:02.000000 eth_retry-0.1.9/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-10-03 17:27:02.000000 eth_retry-0.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-10-03 17:27:12.834892 eth_retry-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2001 2022-10-03 17:27:02.000000 eth_retry-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 17:27:12.834892 eth_retry-0.1.9/eth_retry/
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-10-03 17:27:02.000000 eth_retry-0.1.9/eth_retry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-10-03 17:27:02.000000 eth_retry-0.1.9/eth_retry/conditional_imports.py
--rw-r--r--   0 runner    (1001) docker     (121)     4268 2022-10-03 17:27:02.000000 eth_retry-0.1.9/eth_retry/eth_retry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 17:27:12.834892 eth_retry-0.1.9/eth_retry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-10-03 17:27:12.000000 eth_retry-0.1.9/eth_retry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-10-03 17:27:12.000000 eth_retry-0.1.9/eth_retry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 17:27:12.000000 eth_retry-0.1.9/eth_retry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-03 17:27:12.000000 eth_retry-0.1.9/eth_retry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-10-03 17:27:02.000000 eth_retry-0.1.9/license
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-03 17:27:12.834892 eth_retry-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-10-03 17:27:02.000000 eth_retry-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 17:27:12.834892 eth_retry-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 17:27:02.000000 eth_retry-0.1.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-10-03 17:27:02.000000 eth_retry-0.1.9/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-10-03 17:27:02.000000 eth_retry-0.1.9/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-10-03 17:27:02.000000 eth_retry-0.1.9/tests/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 17:27:02.886628 eth_retry-0.1.9.dev1/
+-rw-r--r--   0 runner    (1001) docker     (121)      231 2022-10-03 17:26:49.000000 eth_retry-0.1.9.dev1/.env.sample
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 17:27:02.886628 eth_retry-0.1.9.dev1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 17:27:02.886628 eth_retry-0.1.9.dev1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-10-03 17:26:49.000000 eth_retry-0.1.9.dev1/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      612 2022-10-03 17:26:49.000000 eth_retry-0.1.9.dev1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2022-10-03 17:26:49.000000 eth_retry-0.1.9.dev1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      370 2022-10-03 17:27:02.886628 eth_retry-0.1.9.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2001 2022-10-03 17:26:49.000000 eth_retry-0.1.9.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 17:27:02.886628 eth_retry-0.1.9.dev1/eth_retry/
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2022-10-03 17:26:49.000000 eth_retry-0.1.9.dev1/eth_retry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      474 2022-10-03 17:26:49.000000 eth_retry-0.1.9.dev1/eth_retry/conditional_imports.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4268 2022-10-03 17:26:49.000000 eth_retry-0.1.9.dev1/eth_retry/eth_retry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 17:27:02.886628 eth_retry-0.1.9.dev1/eth_retry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      370 2022-10-03 17:27:02.000000 eth_retry-0.1.9.dev1/eth_retry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      403 2022-10-03 17:27:02.000000 eth_retry-0.1.9.dev1/eth_retry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 17:27:02.000000 eth_retry-0.1.9.dev1/eth_retry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-03 17:27:02.000000 eth_retry-0.1.9.dev1/eth_retry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-10-03 17:26:49.000000 eth_retry-0.1.9.dev1/license
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-03 17:27:02.886628 eth_retry-0.1.9.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      696 2022-10-03 17:26:49.000000 eth_retry-0.1.9.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 17:27:02.886628 eth_retry-0.1.9.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 17:26:49.000000 eth_retry-0.1.9.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-10-03 17:26:49.000000 eth_retry-0.1.9.dev1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      576 2022-10-03 17:26:49.000000 eth_retry-0.1.9.dev1/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (121)      226 2022-10-03 17:26:49.000000 eth_retry-0.1.9.dev1/tests/test_sync.py
```

### Comparing `eth_retry-0.1.9/.github/workflows/release.yaml` & `eth_retry-0.1.9.dev1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `eth_retry-0.1.9/README.md` & `eth_retry-0.1.9.dev1/README.md`

 * *Files identical despite different names*

### Comparing `eth_retry-0.1.9/eth_retry/eth_retry.py` & `eth_retry-0.1.9.dev1/eth_retry/eth_retry.py`

 * *Files identical despite different names*

### Comparing `eth_retry-0.1.9/license` & `eth_retry-0.1.9.dev1/license`

 * *Files identical despite different names*

### Comparing `eth_retry-0.1.9/setup.py` & `eth_retry-0.1.9.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `eth_retry-0.1.9/tests/test_async.py` & `eth_retry-0.1.9.dev1/tests/test_async.py`

 * *Files identical despite different names*

