# Comparing `tmp/osstatus-1.0.2.tar.gz` & `tmp/osstatus-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osstatus-1.0.2.tar", last modified: Thu Feb  9 17:57:21 2023, max compression
+gzip compressed data, was "osstatus-1.0.3.tar", last modified: Sun May 14 06:31:05 2023, max compression
```

## Comparing `osstatus-1.0.2.tar` & `osstatus-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 17:57:21.234971 osstatus-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-02-09 17:57:08.000000 osstatus-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-02-09 17:57:21.234971 osstatus-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-02-09 17:57:08.000000 osstatus-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 17:57:21.230971 osstatus-1.0.2/osstatus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 17:57:08.000000 osstatus-1.0.2/osstatus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-02-09 17:57:08.000000 osstatus-1.0.2/osstatus/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   626961 2023-02-09 17:57:08.000000 osstatus-1.0.2/osstatus/cache.pickle
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-02-09 17:57:08.000000 osstatus-1.0.2/osstatus/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 17:57:21.234971 osstatus-1.0.2/osstatus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-02-09 17:57:21.000000 osstatus-1.0.2/osstatus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-02-09 17:57:21.000000 osstatus-1.0.2/osstatus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 17:57:21.000000 osstatus-1.0.2/osstatus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-09 17:57:21.000000 osstatus-1.0.2/osstatus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-09 17:57:21.000000 osstatus-1.0.2/osstatus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-09 17:57:21.000000 osstatus-1.0.2/osstatus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 17:57:21.234971 osstatus-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-02-09 17:57:08.000000 osstatus-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:31:05.172983 osstatus-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-14 06:30:45.000000 osstatus-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    43698 2023-05-14 06:31:05.172983 osstatus-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-14 06:30:45.000000 osstatus-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:31:05.172983 osstatus-1.0.3/osstatus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 06:30:45.000000 osstatus-1.0.3/osstatus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-14 06:30:45.000000 osstatus-1.0.3/osstatus/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-14 06:30:45.000000 osstatus-1.0.3/osstatus/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:31:05.172983 osstatus-1.0.3/osstatus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43698 2023-05-14 06:31:05.000000 osstatus-1.0.3/osstatus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-14 06:31:05.000000 osstatus-1.0.3/osstatus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 06:31:05.000000 osstatus-1.0.3/osstatus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-14 06:31:05.000000 osstatus-1.0.3/osstatus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-14 06:31:05.000000 osstatus-1.0.3/osstatus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-14 06:31:05.000000 osstatus-1.0.3/osstatus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-14 06:30:45.000000 osstatus-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-14 06:30:45.000000 osstatus-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 06:31:05.172983 osstatus-1.0.3/setup.cfg
```

### Comparing `osstatus-1.0.2/LICENSE` & `osstatus-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `osstatus-1.0.2/README.md` & `osstatus-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `osstatus-1.0.2/osstatus/__main__.py` & `osstatus-1.0.3/osstatus/__main__.py`

 * *Files identical despite different names*

### Comparing `osstatus-1.0.2/osstatus/cache.py` & `osstatus-1.0.3/osstatus/cache.py`

 * *Files identical despite different names*

