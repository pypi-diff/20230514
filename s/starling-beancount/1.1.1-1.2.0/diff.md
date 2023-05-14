# Comparing `tmp/starling-beancount-1.1.1.tar.gz` & `tmp/starling-beancount-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starling-beancount-1.1.1.tar", last modified: Thu Feb  2 22:35:52 2023, max compression
+gzip compressed data, was "starling-beancount-1.2.0.tar", last modified: Sun May 14 07:05:55 2023, max compression
```

## Comparing `starling-beancount-1.1.1.tar` & `starling-beancount-1.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 22:35:52.825597 starling-beancount-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-02-02 22:35:42.000000 starling-beancount-1.1.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 22:35:52.825597 starling-beancount-1.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 22:35:52.825597 starling-beancount-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-02-02 22:35:42.000000 starling-beancount-1.1.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-02-02 22:35:42.000000 starling-beancount-1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-02 22:35:42.000000 starling-beancount-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-02-02 22:35:52.825597 starling-beancount-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-02-02 22:35:42.000000 starling-beancount-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-02-02 22:35:42.000000 starling-beancount-1.1.1/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-02-02 22:35:42.000000 starling-beancount-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-02 22:35:52.825597 starling-beancount-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 22:35:52.825597 starling-beancount-1.1.1/starling_beancount/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 22:35:42.000000 starling-beancount-1.1.1/starling_beancount/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-02-02 22:35:42.000000 starling-beancount-1.1.1/starling_beancount/extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-02-02 22:35:42.000000 starling-beancount-1.1.1/starling_beancount/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 22:35:42.000000 starling-beancount-1.1.1/starling_beancount/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 22:35:52.825597 starling-beancount-1.1.1/starling_beancount.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-02-02 22:35:52.000000 starling-beancount-1.1.1/starling_beancount.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-02-02 22:35:52.000000 starling-beancount-1.1.1/starling_beancount.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 22:35:52.000000 starling-beancount-1.1.1/starling_beancount.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-02 22:35:52.000000 starling-beancount-1.1.1/starling_beancount.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-02 22:35:52.000000 starling-beancount-1.1.1/starling_beancount.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-02 22:35:52.000000 starling-beancount-1.1.1/starling_beancount.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:05:55.043928 starling-beancount-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-14 07:05:45.000000 starling-beancount-1.2.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:05:55.039928 starling-beancount-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:05:55.039928 starling-beancount-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-14 07:05:45.000000 starling-beancount-1.2.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-14 07:05:45.000000 starling-beancount-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-14 07:05:45.000000 starling-beancount-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-05-14 07:05:55.043928 starling-beancount-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-14 07:05:45.000000 starling-beancount-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-14 07:05:45.000000 starling-beancount-1.2.0/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-14 07:05:45.000000 starling-beancount-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 07:05:55.043928 starling-beancount-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:05:55.043928 starling-beancount-1.2.0/starling_beancount/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 07:05:45.000000 starling-beancount-1.2.0/starling_beancount/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-05-14 07:05:45.000000 starling-beancount-1.2.0/starling_beancount/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-14 07:05:45.000000 starling-beancount-1.2.0/starling_beancount/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 07:05:45.000000 starling-beancount-1.2.0/starling_beancount/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:05:55.043928 starling-beancount-1.2.0/starling_beancount.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-05-14 07:05:55.000000 starling-beancount-1.2.0/starling_beancount.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-14 07:05:55.000000 starling-beancount-1.2.0/starling_beancount.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 07:05:55.000000 starling-beancount-1.2.0/starling_beancount.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-14 07:05:55.000000 starling-beancount-1.2.0/starling_beancount.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-14 07:05:55.000000 starling-beancount-1.2.0/starling_beancount.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 07:05:55.000000 starling-beancount-1.2.0/starling_beancount.egg-info/top_level.txt
```

### Comparing `starling-beancount-1.1.1/.github/workflows/publish.yml` & `starling-beancount-1.2.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `starling-beancount-1.1.1/.gitignore` & `starling-beancount-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `starling-beancount-1.1.1/LICENSE` & `starling-beancount-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starling-beancount-1.1.1/PKG-INFO` & `starling-beancount-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starling-beancount
-Version: 1.1.1
+Version: 1.2.0
 Summary: Import Starling Bank transactions in Beancount
 Author-email: Chris Arderne <chris@rdrn.me>
 License: MIT License
         
         Copyright (c) 2021 Chris Arderne
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `starling-beancount-1.1.1/README.md` & `starling-beancount-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `starling-beancount-1.1.1/pyproject.toml` & `starling-beancount-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `starling-beancount-1.1.1/starling_beancount/extractor.py` & `starling-beancount-1.2.0/starling_beancount/extractor.py`

 * *Files identical despite different names*

### Comparing `starling-beancount-1.1.1/starling_beancount/importer.py` & `starling-beancount-1.2.0/starling_beancount/importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import date
+from datetime import date, timedelta
 from pathlib import Path
 from typing import Any
 
 import beancount.loader
 from beancount.core.data import Note
 from beancount.ingest import importer  # type: ignore[import]
 
@@ -52,15 +52,15 @@
     def name(self) -> str:
         return self.account_name
 
     def identify(self, file: "FileMemo") -> bool:
         return self.acc in file.name
 
     def extract(self, file: str) -> list:
-        since = last_date(self.bean_path, self.account_name)
+        since = last_date(self.bean_path, self.account_name) - timedelta(days=3)
         res = extractor.extract(self.config_path, self.acc, self.token_path, since)
         return res
 
     def file_account(self, file):
         return self.account_name
 
     def file_name(self, file):
```

### Comparing `starling-beancount-1.1.1/starling_beancount.egg-info/PKG-INFO` & `starling-beancount-1.2.0/starling_beancount.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starling-beancount
-Version: 1.1.1
+Version: 1.2.0
 Summary: Import Starling Bank transactions in Beancount
 Author-email: Chris Arderne <chris@rdrn.me>
 License: MIT License
         
         Copyright (c) 2021 Chris Arderne
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

