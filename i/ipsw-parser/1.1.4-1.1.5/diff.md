# Comparing `tmp/ipsw_parser-1.1.4.tar.gz` & `tmp/ipsw_parser-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipsw_parser-1.1.4.tar", last modified: Wed Mar  1 12:31:27 2023, max compression
+gzip compressed data, was "ipsw_parser-1.1.5.tar", last modified: Sun May 14 06:11:51 2023, max compression
```

## Comparing `ipsw_parser-1.1.4.tar` & `ipsw_parser-1.1.5.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:31:27.319469 ipsw_parser-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-03-01 12:31:18.000000 ipsw_parser-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-03-01 12:31:27.315469 ipsw_parser-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-03-01 12:31:18.000000 ipsw_parser-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:31:27.315469 ipsw_parser-1.1.4/ipsw_parser/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:31:18.000000 ipsw_parser-1.1.4/ipsw_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-03-01 12:31:18.000000 ipsw_parser-1.1.4/ipsw_parser/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-03-01 12:31:18.000000 ipsw_parser-1.1.4/ipsw_parser/build_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-03-01 12:31:18.000000 ipsw_parser-1.1.4/ipsw_parser/build_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-03-01 12:31:18.000000 ipsw_parser-1.1.4/ipsw_parser/component.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-01 12:31:18.000000 ipsw_parser-1.1.4/ipsw_parser/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-03-01 12:31:18.000000 ipsw_parser-1.1.4/ipsw_parser/firmware.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-03-01 12:31:18.000000 ipsw_parser-1.1.4/ipsw_parser/img4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-03-01 12:31:18.000000 ipsw_parser-1.1.4/ipsw_parser/ipsw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:31:27.315469 ipsw_parser-1.1.4/ipsw_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-03-01 12:31:27.000000 ipsw_parser-1.1.4/ipsw_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-01 12:31:27.000000 ipsw_parser-1.1.4/ipsw_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 12:31:27.000000 ipsw_parser-1.1.4/ipsw_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-01 12:31:27.000000 ipsw_parser-1.1.4/ipsw_parser.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-01 12:31:27.000000 ipsw_parser-1.1.4/ipsw_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-01 12:31:27.000000 ipsw_parser-1.1.4/ipsw_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 12:31:27.319469 ipsw_parser-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-03-01 12:31:18.000000 ipsw_parser-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:11:51.591472 ipsw_parser-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-14 06:11:36.000000 ipsw_parser-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42611 2023-05-14 06:11:51.591472 ipsw_parser-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-14 06:11:36.000000 ipsw_parser-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:11:51.587472 ipsw_parser-1.1.5/ipsw_parser/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:11:36.000000 ipsw_parser-1.1.5/ipsw_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-14 06:11:36.000000 ipsw_parser-1.1.5/ipsw_parser/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-05-14 06:11:36.000000 ipsw_parser-1.1.5/ipsw_parser/build_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-14 06:11:36.000000 ipsw_parser-1.1.5/ipsw_parser/build_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-14 06:11:36.000000 ipsw_parser-1.1.5/ipsw_parser/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-14 06:11:36.000000 ipsw_parser-1.1.5/ipsw_parser/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-14 06:11:36.000000 ipsw_parser-1.1.5/ipsw_parser/firmware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-14 06:11:36.000000 ipsw_parser-1.1.5/ipsw_parser/img4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-05-14 06:11:36.000000 ipsw_parser-1.1.5/ipsw_parser/ipsw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:11:51.587472 ipsw_parser-1.1.5/ipsw_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42611 2023-05-14 06:11:51.000000 ipsw_parser-1.1.5/ipsw_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-14 06:11:51.000000 ipsw_parser-1.1.5/ipsw_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 06:11:51.000000 ipsw_parser-1.1.5/ipsw_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 06:11:51.000000 ipsw_parser-1.1.5/ipsw_parser.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-14 06:11:51.000000 ipsw_parser-1.1.5/ipsw_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 06:11:51.000000 ipsw_parser-1.1.5/ipsw_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-14 06:11:36.000000 ipsw_parser-1.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-14 06:11:36.000000 ipsw_parser-1.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 06:11:51.591472 ipsw_parser-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-14 06:11:36.000000 ipsw_parser-1.1.5/setup.py
```

### Comparing `ipsw_parser-1.1.4/LICENSE` & `ipsw_parser-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ipsw_parser-1.1.4/README.md` & `ipsw_parser-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ipsw_parser-1.1.4/ipsw_parser/__main__.py` & `ipsw_parser-1.1.5/ipsw_parser/__main__.py`

 * *Files identical despite different names*

### Comparing `ipsw_parser-1.1.4/ipsw_parser/build_identity.py` & `ipsw_parser-1.1.5/ipsw_parser/build_identity.py`

 * *Files identical despite different names*

### Comparing `ipsw_parser-1.1.4/ipsw_parser/build_manifest.py` & `ipsw_parser-1.1.5/ipsw_parser/build_manifest.py`

 * *Files identical despite different names*

### Comparing `ipsw_parser-1.1.4/ipsw_parser/component.py` & `ipsw_parser-1.1.5/ipsw_parser/component.py`

 * *Files identical despite different names*

### Comparing `ipsw_parser-1.1.4/ipsw_parser/firmware.py` & `ipsw_parser-1.1.5/ipsw_parser/firmware.py`

 * *Files identical despite different names*

### Comparing `ipsw_parser-1.1.4/ipsw_parser/img4.py` & `ipsw_parser-1.1.5/ipsw_parser/img4.py`

 * *Files identical despite different names*

### Comparing `ipsw_parser-1.1.4/ipsw_parser/ipsw.py` & `ipsw_parser-1.1.5/ipsw_parser/ipsw.py`

 * *Files identical despite different names*

### Comparing `ipsw_parser-1.1.4/setup.py` & `ipsw_parser-1.1.5/setup.py`

 * *Files identical despite different names*

