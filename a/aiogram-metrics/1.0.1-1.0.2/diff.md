# Comparing `tmp/aiogram_metrics-1.0.1.tar.gz` & `tmp/aiogram_metrics-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram_metrics-1.0.1.tar", last modified: Sun May 14 21:00:50 2023, max compression
+gzip compressed data, was "aiogram_metrics-1.0.2.tar", last modified: Sun May 14 21:30:34 2023, max compression
```

## Comparing `aiogram_metrics-1.0.1.tar` & `aiogram_metrics-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-05-14 19:01:49.276792 aiogram_metrics-1.0.1/LICENSE
--rw-r--r--   0        0        0       65 2023-05-14 19:01:49.277880 aiogram_metrics-1.0.1/README.md
--rw-r--r--   0        0        0      142 2023-05-14 19:01:49.278104 aiogram_metrics-1.0.1/aiogram_metrics/__init__.py
--rw-r--r--   0        0        0     2982 2023-05-14 20:29:42.408612 aiogram_metrics-1.0.1/aiogram_metrics/api.py
--rw-r--r--   0        0        0      193 2023-05-14 20:29:42.408810 aiogram_metrics-1.0.1/aiogram_metrics/hub.py
--rw-r--r--   0        0        0     1306 2023-05-14 19:01:49.278559 aiogram_metrics-1.0.1/aiogram_metrics/public.py
--rw-r--r--   0        0        0     1001 2023-05-14 20:29:42.409008 aiogram_metrics-1.0.1/aiogram_metrics/sql.py
--rw-r--r--   0        0        0      587 2023-05-14 21:00:50.013852 aiogram_metrics-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      374 1970-01-01 00:00:00.000000 aiogram_metrics-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-14 19:01:49.276792 aiogram_metrics-1.0.2/LICENSE
+-rw-r--r--   0        0        0       65 2023-05-14 19:01:49.277880 aiogram_metrics-1.0.2/README.md
+-rw-r--r--   0        0        0      142 2023-05-14 19:01:49.278104 aiogram_metrics-1.0.2/aiogram_metrics/__init__.py
+-rw-r--r--   0        0        0     2982 2023-05-14 20:29:42.408612 aiogram_metrics-1.0.2/aiogram_metrics/api.py
+-rw-r--r--   0        0        0      193 2023-05-14 20:29:42.408810 aiogram_metrics-1.0.2/aiogram_metrics/hub.py
+-rw-r--r--   0        0        0     1306 2023-05-14 19:01:49.278559 aiogram_metrics-1.0.2/aiogram_metrics/public.py
+-rw-r--r--   0        0        0     1001 2023-05-14 20:29:42.409008 aiogram_metrics-1.0.2/aiogram_metrics/sql.py
+-rw-r--r--   0        0        0      586 2023-05-14 21:30:34.187517 aiogram_metrics-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      373 1970-01-01 00:00:00.000000 aiogram_metrics-1.0.2/PKG-INFO
```

### Comparing `aiogram_metrics-1.0.1/LICENSE` & `aiogram_metrics-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogram_metrics-1.0.1/aiogram_metrics/api.py` & `aiogram_metrics-1.0.2/aiogram_metrics/api.py`

 * *Files identical despite different names*

### Comparing `aiogram_metrics-1.0.1/aiogram_metrics/public.py` & `aiogram_metrics-1.0.2/aiogram_metrics/public.py`

 * *Files identical despite different names*

### Comparing `aiogram_metrics-1.0.1/aiogram_metrics/sql.py` & `aiogram_metrics-1.0.2/aiogram_metrics/sql.py`

 * *Files identical despite different names*

### Comparing `aiogram_metrics-1.0.1/pyproject.toml` & `aiogram_metrics-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "aiogram-metrics"
-version = "1.0.1"
+version = "1.0.2"
 description = "Message metrics exporter for aiogram framework"
 authors = [
     { name = "benyamin ginzburg", email = "benyamin+git@ginzburg.io" },
 ]
 dependencies = [
     "aiogram",
-    "psycopg[binary]",
+    "psycopg-binary",
 ]
 requires-python = ">=3.7"
 readme = "README.md"
 
 [project.license]
 text = "GPL-3.0"
```

