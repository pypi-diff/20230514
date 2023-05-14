# Comparing `tmp/bfactory-0.4.1.tar.gz` & `tmp/bfactory-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bfactory-0.4.1.tar", last modified: Sat Apr 29 02:20:50 2023, max compression
+gzip compressed data, was "bfactory-0.4.2.tar", last modified: Sun May 14 03:15:27 2023, max compression
```

## Comparing `bfactory-0.4.1.tar` & `bfactory-0.4.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-29 02:20:50.612099 bfactory-0.4.1/
--rw-r--r--   0 blackbox  (1000) users      (985)     1063 2022-10-03 23:46:43.000000 bfactory-0.4.1/LICENSE
--rw-r--r--   0 blackbox  (1000) users      (985)      543 2023-04-29 02:20:50.612099 bfactory-0.4.1/PKG-INFO
--rw-r--r--   0 blackbox  (1000) users      (985)     1604 2022-10-03 23:46:43.000000 bfactory-0.4.1/README.md
--rw-r--r--   0 blackbox  (1000) users      (985)       87 2022-10-03 23:46:43.000000 bfactory-0.4.1/pyproject.toml
--rw-r--r--   0 blackbox  (1000) users      (985)      856 2023-04-29 02:20:50.612099 bfactory-0.4.1/setup.cfg
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-29 02:20:50.608765 bfactory-0.4.1/src/
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-29 02:20:50.608765 bfactory-0.4.1/src/bfactory/
--rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-04 00:29:45.000000 bfactory-0.4.1/src/bfactory/__init__.py
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-29 02:20:50.608765 bfactory-0.4.1/src/bfactory/config/
--rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4.1/src/bfactory/config/__init__.py
--rw-r--r--   0 blackbox  (1000) users      (985)     1253 2023-04-29 02:18:07.000000 bfactory-0.4.1/src/bfactory/config/settings.py
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-29 02:20:50.608765 bfactory-0.4.1/src/bfactory/core/
--rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4.1/src/bfactory/core/__init__.py
--rw-r--r--   0 blackbox  (1000) users      (985)     3515 2022-11-10 04:08:56.000000 bfactory-0.4.1/src/bfactory/core/engine.py
--rw-r--r--   0 blackbox  (1000) users      (985)     2130 2022-11-05 23:27:19.000000 bfactory-0.4.1/src/bfactory/core/tasks.py
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-29 02:20:50.608765 bfactory-0.4.1/src/bfactory/core/templates/
--rw-r--r--   0 blackbox  (1000) users      (985)       85 2022-10-03 23:46:43.000000 bfactory-0.4.1/src/bfactory/core/templates/READ.ME
--rw-r--r--   0 blackbox  (1000) users      (985)      570 2022-10-04 00:02:46.000000 bfactory-0.4.1/src/bfactory/core/templates/admin.py
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-29 02:20:50.608765 bfactory-0.4.1/src/bfactory/core/templates/helpers/
--rw-r--r--   0 blackbox  (1000) users      (985)     1461 2023-04-29 00:28:37.000000 bfactory-0.4.1/src/bfactory/core/templates/helpers/field.py
--rw-r--r--   0 blackbox  (1000) users      (985)     1260 2023-04-29 00:35:51.000000 bfactory-0.4.1/src/bfactory/core/templates/helpers/field_serializer.py
--rw-r--r--   0 blackbox  (1000) users      (985)      414 2023-04-29 00:35:02.000000 bfactory-0.4.1/src/bfactory/core/templates/helpers/field_type_linting.py
--rw-r--r--   0 blackbox  (1000) users      (985)      624 2022-11-06 04:00:22.000000 bfactory-0.4.1/src/bfactory/core/templates/models.py
--rw-r--r--   0 blackbox  (1000) users      (985)     2759 2022-10-04 00:02:40.000000 bfactory-0.4.1/src/bfactory/core/templates/myconf.py
--rw-r--r--   0 blackbox  (1000) users      (985)      599 2023-04-29 00:34:58.000000 bfactory-0.4.1/src/bfactory/core/templates/selectors.py
--rw-r--r--   0 blackbox  (1000) users      (985)     1621 2022-11-29 20:30:05.000000 bfactory-0.4.1/src/bfactory/core/templates/services.py
--rw-r--r--   0 blackbox  (1000) users      (985)      570 2022-11-05 23:27:19.000000 bfactory-0.4.1/src/bfactory/core/templates/urls.py
--rw-r--r--   0 blackbox  (1000) users      (985)     4388 2022-11-10 03:54:52.000000 bfactory-0.4.1/src/bfactory/core/templates/views.py
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-29 02:20:50.608765 bfactory-0.4.1/src/bfactory/inputs/
--rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4.1/src/bfactory/inputs/__init__.py
--rw-r--r--   0 blackbox  (1000) users      (985)     1550 2022-11-29 20:30:05.000000 bfactory-0.4.1/src/bfactory/inputs/arguments.py
--rw-r--r--   0 blackbox  (1000) users      (985)     2534 2022-11-10 03:35:04.000000 bfactory-0.4.1/src/bfactory/inputs/manifest.py
--rw-r--r--   0 blackbox  (1000) users      (985)     2698 2022-10-30 07:02:48.000000 bfactory-0.4.1/src/bfactory/inputs/manifest.schema.json
--rw-r--r--   0 blackbox  (1000) users      (985)      887 2022-10-03 23:46:43.000000 bfactory-0.4.1/src/bfactory/inputs/parse_manifest.py
--rw-r--r--   0 blackbox  (1000) users      (985)     1363 2022-10-03 23:46:43.000000 bfactory-0.4.1/src/bfactory/inputs/validators.py
--rwxr-xr-x   0 blackbox  (1000) users      (985)     1066 2022-10-04 00:33:18.000000 bfactory-0.4.1/src/bfactory/main.py
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-29 02:20:50.608765 bfactory-0.4.1/src/bfactory/startproject/
--rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4.1/src/bfactory/startproject/__init__.py
--rw-r--r--   0 blackbox  (1000) users      (985)      620 2022-10-04 00:19:42.000000 bfactory-0.4.1/src/bfactory/startproject/startproject.py
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-29 02:20:50.608765 bfactory-0.4.1/src/bfactory/tests/
--rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4.1/src/bfactory/tests/__init__.py
--rw-r--r--   0 blackbox  (1000) users      (985)      743 2022-11-10 04:08:38.000000 bfactory-0.4.1/src/bfactory/tests/engine_tests.py
--rw-r--r--   0 blackbox  (1000) users      (985)     1022 2023-04-29 02:19:06.000000 bfactory-0.4.1/src/bfactory/tests/manifest_test.json
--rw-r--r--   0 blackbox  (1000) users      (985)      675 2022-10-07 02:36:35.000000 bfactory-0.4.1/src/bfactory/tests/manifest_test.py
--rw-r--r--   0 blackbox  (1000) users      (985)      932 2022-10-04 00:31:46.000000 bfactory-0.4.1/src/bfactory/tests/run_tests.py
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-29 02:20:50.612099 bfactory-0.4.1/src/bfactory/utils/
--rw-r--r--   0 blackbox  (1000) users      (985)      900 2022-10-03 23:46:43.000000 bfactory-0.4.1/src/bfactory/utils/crypto.py
--rw-r--r--   0 blackbox  (1000) users      (985)     2442 2022-10-07 02:36:35.000000 bfactory-0.4.1/src/bfactory/utils/paths.py
--rw-r--r--   0 blackbox  (1000) users      (985)      450 2022-10-04 00:26:40.000000 bfactory-0.4.1/src/bfactory/utils/render.py
-drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-04-29 02:20:50.608765 bfactory-0.4.1/src/bfactory.egg-info/
--rw-r--r--   0 blackbox  (1000) users      (985)      543 2023-04-29 02:20:50.000000 bfactory-0.4.1/src/bfactory.egg-info/PKG-INFO
--rw-r--r--   0 blackbox  (1000) users      (985)     1481 2023-04-29 02:20:50.000000 bfactory-0.4.1/src/bfactory.egg-info/SOURCES.txt
--rw-r--r--   0 blackbox  (1000) users      (985)        1 2023-04-29 02:20:50.000000 bfactory-0.4.1/src/bfactory.egg-info/dependency_links.txt
--rw-r--r--   0 blackbox  (1000) users      (985)       48 2023-04-29 02:20:50.000000 bfactory-0.4.1/src/bfactory.egg-info/entry_points.txt
--rw-r--r--   0 blackbox  (1000) users      (985)       91 2023-04-29 02:20:50.000000 bfactory-0.4.1/src/bfactory.egg-info/requires.txt
--rw-r--r--   0 blackbox  (1000) users      (985)        9 2023-04-29 02:20:50.000000 bfactory-0.4.1/src/bfactory.egg-info/top_level.txt
--rwxr-xr-x   0 blackbox  (1000) users      (985)      197 2022-11-29 20:30:05.000000 bfactory-0.4.1/src/bfactory.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-14 03:15:27.875584 bfactory-0.4.2/
+-rw-r--r--   0 blackbox  (1000) users      (985)     1063 2022-10-03 23:46:43.000000 bfactory-0.4.2/LICENSE
+-rw-r--r--   0 blackbox  (1000) users      (985)      543 2023-05-14 03:15:27.875584 bfactory-0.4.2/PKG-INFO
+-rw-r--r--   0 blackbox  (1000) users      (985)     1929 2023-05-14 03:12:02.000000 bfactory-0.4.2/README.md
+-rw-r--r--   0 blackbox  (1000) users      (985)       87 2022-10-03 23:46:43.000000 bfactory-0.4.2/pyproject.toml
+-rw-r--r--   0 blackbox  (1000) users      (985)      856 2023-05-14 03:15:27.875584 bfactory-0.4.2/setup.cfg
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-14 03:15:27.872251 bfactory-0.4.2/src/
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-14 03:15:27.872251 bfactory-0.4.2/src/bfactory/
+-rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-04 00:29:45.000000 bfactory-0.4.2/src/bfactory/__init__.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-14 03:15:27.872251 bfactory-0.4.2/src/bfactory/cli/
+-rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4.2/src/bfactory/cli/__init__.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      744 2023-05-13 21:38:11.000000 bfactory-0.4.2/src/bfactory/cli/django_cli.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-14 03:15:27.872251 bfactory-0.4.2/src/bfactory/config/
+-rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4.2/src/bfactory/config/__init__.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     1253 2023-05-14 03:12:52.000000 bfactory-0.4.2/src/bfactory/config/settings.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-14 03:15:27.872251 bfactory-0.4.2/src/bfactory/core/
+-rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4.2/src/bfactory/core/__init__.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     3777 2023-05-13 21:38:24.000000 bfactory-0.4.2/src/bfactory/core/engine.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     2127 2023-05-13 20:14:24.000000 bfactory-0.4.2/src/bfactory/core/tasks.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-14 03:15:27.875584 bfactory-0.4.2/src/bfactory/core/templates/
+-rw-r--r--   0 blackbox  (1000) users      (985)       85 2022-10-03 23:46:43.000000 bfactory-0.4.2/src/bfactory/core/templates/READ.ME
+-rw-r--r--   0 blackbox  (1000) users      (985)      570 2022-10-04 00:02:46.000000 bfactory-0.4.2/src/bfactory/core/templates/admin.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-14 03:15:27.875584 bfactory-0.4.2/src/bfactory/core/templates/helpers/
+-rw-r--r--   0 blackbox  (1000) users      (985)     1463 2023-05-14 03:07:12.000000 bfactory-0.4.2/src/bfactory/core/templates/helpers/field.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     1262 2023-05-14 01:53:53.000000 bfactory-0.4.2/src/bfactory/core/templates/helpers/field_serializer.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      416 2023-05-14 01:52:12.000000 bfactory-0.4.2/src/bfactory/core/templates/helpers/field_type_linting.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      624 2022-11-06 04:00:22.000000 bfactory-0.4.2/src/bfactory/core/templates/models.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     2759 2022-10-04 00:02:40.000000 bfactory-0.4.2/src/bfactory/core/templates/myconf.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      599 2023-04-29 00:34:58.000000 bfactory-0.4.2/src/bfactory/core/templates/selectors.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     1621 2022-11-29 20:30:05.000000 bfactory-0.4.2/src/bfactory/core/templates/services.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      570 2022-11-05 23:27:19.000000 bfactory-0.4.2/src/bfactory/core/templates/urls.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     4388 2022-11-10 03:54:52.000000 bfactory-0.4.2/src/bfactory/core/templates/views.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-14 03:15:27.875584 bfactory-0.4.2/src/bfactory/inputs/
+-rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4.2/src/bfactory/inputs/__init__.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     1986 2023-05-13 21:39:17.000000 bfactory-0.4.2/src/bfactory/inputs/arguments.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     2534 2022-11-10 03:35:04.000000 bfactory-0.4.2/src/bfactory/inputs/manifest.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     2698 2022-10-30 07:02:48.000000 bfactory-0.4.2/src/bfactory/inputs/manifest.schema.json
+-rw-r--r--   0 blackbox  (1000) users      (985)      887 2022-10-03 23:46:43.000000 bfactory-0.4.2/src/bfactory/inputs/parse_manifest.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     1363 2022-10-03 23:46:43.000000 bfactory-0.4.2/src/bfactory/inputs/validators.py
+-rwxr-xr-x   0 blackbox  (1000) users      (985)     1421 2023-05-13 21:38:47.000000 bfactory-0.4.2/src/bfactory/main.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-14 03:15:27.875584 bfactory-0.4.2/src/bfactory/tests/
+-rw-r--r--   0 blackbox  (1000) users      (985)        0 2022-10-03 23:46:43.000000 bfactory-0.4.2/src/bfactory/tests/__init__.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      698 2023-05-13 21:38:08.000000 bfactory-0.4.2/src/bfactory/tests/engine_tests.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      992 2023-05-14 01:43:35.000000 bfactory-0.4.2/src/bfactory/tests/manifest_test.json
+-rw-r--r--   0 blackbox  (1000) users      (985)      673 2023-05-13 20:14:43.000000 bfactory-0.4.2/src/bfactory/tests/manifest_test.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      932 2022-10-04 00:31:46.000000 bfactory-0.4.2/src/bfactory/tests/run_tests.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-14 03:15:27.875584 bfactory-0.4.2/src/bfactory/utils/
+-rw-r--r--   0 blackbox  (1000) users      (985)      900 2022-10-03 23:46:43.000000 bfactory-0.4.2/src/bfactory/utils/crypto.py
+-rw-r--r--   0 blackbox  (1000) users      (985)      450 2022-10-04 00:26:40.000000 bfactory-0.4.2/src/bfactory/utils/render.py
+-rw-r--r--   0 blackbox  (1000) users      (985)     2830 2023-05-13 21:38:35.000000 bfactory-0.4.2/src/bfactory/utils/state.py
+drwxr-xr-x   0 blackbox  (1000) users      (985)        0 2023-05-14 03:15:27.872251 bfactory-0.4.2/src/bfactory.egg-info/
+-rw-r--r--   0 blackbox  (1000) users      (985)      543 2023-05-14 03:15:27.000000 bfactory-0.4.2/src/bfactory.egg-info/PKG-INFO
+-rw-r--r--   0 blackbox  (1000) users      (985)     1461 2023-05-14 03:15:27.000000 bfactory-0.4.2/src/bfactory.egg-info/SOURCES.txt
+-rw-r--r--   0 blackbox  (1000) users      (985)        1 2023-05-14 03:15:27.000000 bfactory-0.4.2/src/bfactory.egg-info/dependency_links.txt
+-rw-r--r--   0 blackbox  (1000) users      (985)       48 2023-05-14 03:15:27.000000 bfactory-0.4.2/src/bfactory.egg-info/entry_points.txt
+-rw-r--r--   0 blackbox  (1000) users      (985)       91 2023-05-14 03:15:27.000000 bfactory-0.4.2/src/bfactory.egg-info/requires.txt
+-rw-r--r--   0 blackbox  (1000) users      (985)        9 2023-05-14 03:15:27.000000 bfactory-0.4.2/src/bfactory.egg-info/top_level.txt
+-rwxr-xr-x   0 blackbox  (1000) users      (985)      197 2022-11-29 20:30:05.000000 bfactory-0.4.2/src/bfactory.py
```

### Comparing `bfactory-0.4.1/LICENSE` & `bfactory-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.1/PKG-INFO` & `bfactory-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfactory
-Version: 0.4.1
+Version: 0.4.2
 Summary: Build an API from a manifest file
 Home-page: https://github.com/forkear/bfactory
 Author: Forkear
 Author-email: forkear@no-spam.org
 Project-URL: Documentation, https://github.com/forkear/bfactory/blob/main/README.md
 Project-URL: Source, https://github.com/forkear/bfactory
 Project-URL: Tracker, https://github.com/forkear/bfactory/issues
```

### Comparing `bfactory-0.4.1/setup.cfg` & `bfactory-0.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.1/src/bfactory/config/settings.py` & `bfactory-0.4.2/src/bfactory/config/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 
-__version__ = '0.4.1'
+__version__ = '0.4.2'
 
 TITLE_BANNER='''\
 
 ██████╗ ███████╗ █████╗  ██████╗████████╗ ██████╗ ██████╗ ██╗   ██╗
 ██╔══██╗██╔════╝██╔══██╗██╔════╝╚══██╔══╝██╔═══██╗██╔══██╗╚██╗ ██╔╝
 ██████╔╝█████╗  ███████║██║        ██║   ██║   ██║██████╔╝ ╚████╔╝ 
 ██╔══██╗██╔══╝  ██╔══██║██║        ██║   ██║   ██║██╔══██╗  ╚██╔╝
```

### Comparing `bfactory-0.4.1/src/bfactory/core/engine.py` & `bfactory-0.4.2/src/bfactory/core/engine.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 # -*- encoding: utf-8 -*-
 
 import os
 from bfactory.core import tasks 
 from bfactory.inputs.manifest import Manifest
 from bfactory.config.settings import TITLE_BANNER
 from bfactory.utils.render import render_to_file
-from bfactory.utils.paths import Paths
+from bfactory.utils.state import State
 
-fpaths = Paths()
 
 
 class Engine():
     """
         Se encarga de crear el esqueleto del codigo fuente de la API
         Necesita conocer un manifiesto ya verificado.
     """
 
-    def __init__(self,  manifest: Manifest, force: bool = False ):
+    def __init__(self):
         """
             El objeto Manifiesto se encuentra validado
             el path es donde el engine va a trabajar.
         """
-        self.manifest = manifest
-    
+        self.state = State()
+
+
     def create_api(self) -> bool:
 
         self._clonar_proyecto()
-
-        os.chdir(fpaths.base_path)
+        
+        os.chdir(self.state.base_path)
 
         self._create_readme()
 
         self._configurar_proyecto()
         
         self._create_models()
 
@@ -52,97 +52,109 @@
 
     def __str__(self) -> str:
         return "bfactory Engine"
 
 
     def _create_admin(self) -> None:
         values = {
-            'models':self.manifest.get_models(),
+            'models':self.state.manifest.get_models(),
         } 
 
-        path_models = fpaths.path_file_from_app_api('admin.py')
+        path_models = self.state.path_file_from_app_api('admin.py')
 
         render_to_file(template='admin.py', file_name=path_models, values=values)
  
 
     def _clonar_proyecto(self) -> None:
-        
-        fpaths.mk_and_ch_dir(fpaths.base_path)
+    
+        if self.state.is_an_update():
+            return
+    
+        self.state.mk_and_ch_dir(self.state.base_path)
 
-        tasks.get_zip_base_project(slug=self.manifest.app_slug, path=fpaths.base_path)
+        tasks.get_zip_base_project(slug=self.state.manifest.app_slug, path=self.state.base_path)
 
 
     def _create_services(self) -> None:
         values = {
-            'models':self.manifest.get_models(),
+            'models':self.state.manifest.get_models(),
         } 
 
-        path_services = fpaths.path_file_from_app_api('services.py')
+        path_services = self.state.path_file_from_app_api('services.py')
 
         render_to_file(template='services.py', file_name=path_services, values=values)
 
 
     def _create_models(self) -> None:
+        
         values = {
-            'models':self.manifest.get_models(),
+            'models':self.state.manifest.get_models(),
         } 
 
-        path_models = fpaths.path_file_from_app_api('models.py')
+        path_models = self.state.path_file_from_app_api('models.py')
 
         render_to_file(template='models.py', file_name=path_models, values=values)
 
 
 
     def _create_selectors(self) -> None:
+        
         values = {
-            'models':self.manifest.get_models(),
+            'models':self.state.manifest.get_models(),
         } 
 
-        path_models = fpaths.path_file_from_app_api('selectors.py')
+        path_models = self.state.path_file_from_app_api('selectors.py')
 
         render_to_file(template='selectors.py', file_name=path_models, values=values)
 
 
 
 
     def _create_views(self) -> None:
+        
         values = {
-            'models':self.manifest.get_models(),
+            'models':self.state.manifest.get_models(),
         } 
 
-        path_models = fpaths.path_file_from_app_api('views.py')
+        path_models = self.state.path_file_from_app_api('views.py')
 
         render_to_file(template='views.py', file_name=path_models, values=values)
 
 
 
     def _create_urls(self) -> None:
 
         values = {
-            'models':self.manifest.get_models(),
+            'models':self.state.manifest.get_models(),
         } 
 
-        path_models = fpaths.path_file_from_app_api('urls.py')
+        path_models = self.state.path_file_from_app_api('urls.py')
 
         render_to_file(template='urls.py', file_name=path_models, values=values)
 
 
 
     def _create_readme(self) -> None:
+        if self.state.is_an_update():
+            return
+        
         values = {
             'banner':TITLE_BANNER,
-            'app_name':self.manifest.app_name,
-            'app_version':self.manifest.app_version
+            'app_name':self.state.manifest.app_name,
+            'app_version':self.state.manifest.app_version
         }
 
-        path_readme =  fpaths.path_file_from_project('READ.ME')
+        path_readme =  self.state.path_file_from_project('READ.ME')
 
         render_to_file(template='READ.ME', file_name=path_readme, values=values)
 
 
     def _configurar_proyecto(self) -> None:
         """
             Crea el archivo myconf.py
         """
-        tasks.crear_configuracion_del_proyecto(manifest = self.manifest)
+        if self.state.is_an_update():
+            return
+        
+        tasks.crear_configuracion_del_proyecto(manifest = self.state.manifest)
```

### Comparing `bfactory-0.4.1/src/bfactory/core/tasks.py` & `bfactory-0.4.2/src/bfactory/core/tasks.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 from zipfile import ZipFile
 from urllib.request import urlopen
 import os
 from bfactory.inputs.manifest import Manifest
 from bfactory.config.settings import URL_BASE_BACKEND
 from bfactory.utils.render import render_to_file
 from bfactory.utils.crypto import get_random_secret_key
-from bfactory.utils.paths import Paths
+from bfactory.utils.state import State
 
-fpaths = Paths()
+state = State()
 
 
 def get_zip_base_project(slug: str, path: str = None) -> bool:
     """
         Se encarga de descargar el archivo zip de un proyecto
         base creado en django para nuestra futura api. 
         Luego de descargar el zip lo descomprime en el path dado
         y a continuacion se renombran los directorios y los imports
         para que sea igual que el slug de nuestra api autogenerada
     """
 
     print("> descargando main.zip")
     if not path:
-        path = fpaths.base_path
+        path = state.base_path
 
     resp = urlopen(URL_BASE_BACKEND)
 
     base_path_name = os.path.join(path, slug)
 
     print("> main.zip en memoria")
 
@@ -69,11 +69,11 @@
 
     values = {
         'secret_key': get_random_secret_key(),
         'database': manifest.database,
         'auth': manifest.auth,
     }
     render_to_file(template='myconf.py',
-                   file_name=fpaths.path_myconf, values=values)
+                   file_name=state.path_myconf, values=values)
     return True
```

### Comparing `bfactory-0.4.1/src/bfactory/core/templates/admin.py` & `bfactory-0.4.2/src/bfactory/core/templates/admin.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.1/src/bfactory/core/templates/helpers/field.py` & `bfactory-0.4.2/src/bfactory/core/templates/helpers/field.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 {%- if field.type == 'str'  -%}
     models.CharField(max_length=128 {% if not field.req %}, null=True, blank=True {% endif %})
 {% endif %}
 {%- if field.type == 'text'  -%}
-    models.TextField({% if not field.req %}, null=True, blank=True {% endif %})
+    models.TextField({% if not field.req %} null=True, blank=True {% endif %})
 {% endif %}
 {%- if field.type == 'bool' -%}
     models.BooleanField({% if not field.req %} default=False {% endif %})
 {% endif %}
 {%- if field.type == 'user' or field.type == 'owner' -%}
     models.ForeignKey(User, related_name="{{model.name|lower}}_{{field.name|lower}}_user", on_delete=models.CASCADE{% if not field.req %}, null=True, blank=True{% endif %})
 {% endif %}
 {%- if field.type == 'int' -%}
     models.IntegerField({% if not field.req %}null=True, blank=True{% endif %})
 {% endif %}
-{%- if field.type == 'float' -%}
+{%- if field.type == 'decimal' -%}
     models.DecimalField(max_digits=10, decimal_places=2{% if not field.req %}, null=True, blank=True{% endif %})
 {% endif %}
 {%- if field.type == 'pint' -%}
     models.PositiveIntegerField({% if not field.req %}null=True, blank=True{% endif %})
 {% endif %}
 {%- if field.type == 'fk' -%}
     models.ForeignKey("{{field.fk}}", related_name="{{model.name|lower}}_{{field.name|lower}}_{{field.fk|lower}}", on_delete=models.CASCADE{% if not field.req %},null=True, blank=True{% endif %})
 {% endif %}
 {%- if field.type == 'datetime' -%}
     models.DateTimeField({% if field.default == 'now' %}auto_now=True{% endif %}{% if not field.req %}, null=True, blank=True {% endif %})
-{% endif %}
+{% endif %}
```

### Comparing `bfactory-0.4.1/src/bfactory/core/templates/helpers/field_serializer.py` & `bfactory-0.4.2/src/bfactory/core/templates/helpers/field_serializer.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,13 +15,13 @@
 {% endif %}
 {%- if field.type == 'fk' -%}
     serializers.PrimaryKeyRelatedField(many=False, queryset={{field.fk}}.objects.all(), required={{field.req}} {% if not field.req %}, allow_null=True {% endif %})
 {% endif %}
 {%- if field.type == 'datetime' -%}
     serializers.DateTimeField()
 {% endif %}
-{%- if field.type == 'float' -%}
+{%- if field.type == 'decimal' -%}
     serializers.DecimalField(max_digits=10, decimal_places=2)
 {% endif %}
 {%- if field.type == 'user' or field.type == 'owner' -%}
     serializers.PrimaryKeyRelatedField(many=False, queryset=User.objects.all(), required={{field.req}} {% if not field.req %}, allow_null=True {% endif %})
 {% endif %}
```

### Comparing `bfactory-0.4.1/src/bfactory/core/templates/models.py` & `bfactory-0.4.2/src/bfactory/core/templates/models.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.1/src/bfactory/core/templates/myconf.py` & `bfactory-0.4.2/src/bfactory/core/templates/myconf.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.1/src/bfactory/core/templates/selectors.py` & `bfactory-0.4.2/src/bfactory/core/templates/selectors.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.1/src/bfactory/core/templates/services.py` & `bfactory-0.4.2/src/bfactory/core/templates/services.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.1/src/bfactory/core/templates/urls.py` & `bfactory-0.4.2/src/bfactory/core/templates/urls.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.1/src/bfactory/core/templates/views.py` & `bfactory-0.4.2/src/bfactory/core/templates/views.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.1/src/bfactory/inputs/arguments.py` & `bfactory-0.4.2/src/bfactory/inputs/arguments.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from bfactory.config.settings import TITLE_BANNER
 from bfactory.inputs.validators import ManifestFileType
 from bfactory.tests.run_tests import run_tests
 import argparse
 import pathlib
 import textwrap
 
-
 class TestAction(argparse.Action):
 
     def __init__(self, option_strings, dest, nargs=None, **kwargs):
         super().__init__(option_strings, dest, **kwargs)
 
     def __call__(self, parser, namespace, values, option_string=None):
         if 'test' in values:
@@ -19,15 +18,15 @@
         setattr(namespace, self.dest, values)
 
 
 parser = argparse.ArgumentParser(
     prog='bfactory',
     formatter_class=argparse.RawDescriptionHelpFormatter,
     #description=textwrap.dedent(TITLE_BANNER),
-    epilog='thx to:\n\tPython\n\tDjango\n\tJinja\n\tDjango REST framework',
+    epilog='//thx_to = [ Python, Django, Jinja, Django REST framework ]\n',
 )
 
 
 parser.add_argument(
     'test',
     nargs='?',
     help='Ejecutar test de unidad',
@@ -57,17 +56,43 @@
     '-f',
     nargs='*',
     type=pathlib.Path,
     help='Si existe Path destino lo borra',
     required=False
 )
 
+parser.add_argument(
+    '--update',
+    '-u',
+    nargs='*',
+    help='Actualiza la aplicacion',
+    required=False
+)
+
 
 parser.add_argument(
     '--run',
     '-r',
     nargs='*',
     type=pathlib.Path,
     help='Ejecuta localmente la api luego de crearla',
     required=False
 )
 
+parser.add_argument(
+    '--template',
+    '-t',
+    type=pathlib.Path,
+    help='definir el path o url del template base para crear la api',
+    required=False
+)
+
+
+parser.add_argument(
+    '--createadmin',
+    '-a',
+    nargs='*',
+    type=ManifestFileType(),
+    help='Crea el usuario admin',
+    required=False
+)
+
```

### Comparing `bfactory-0.4.1/src/bfactory/inputs/manifest.py` & `bfactory-0.4.2/src/bfactory/inputs/manifest.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.1/src/bfactory/inputs/manifest.schema.json` & `bfactory-0.4.2/src/bfactory/inputs/manifest.schema.json`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.1/src/bfactory/inputs/parse_manifest.py` & `bfactory-0.4.2/src/bfactory/inputs/parse_manifest.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.1/src/bfactory/inputs/validators.py` & `bfactory-0.4.2/src/bfactory/inputs/validators.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.1/src/bfactory/startproject/startproject.py` & `bfactory-0.4.2/src/bfactory/cli/django_cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 
 import os
 from bfactory.core.engine import Engine
-from bfactory.utils.paths import Paths 
+from bfactory.utils.state import State 
 
 
-fpaths=Paths()
+state=State()
 
-class StartProject():
+class DjangoCli():
 
     def __init__(self, engine: Engine ):
-        self.engine = engine 
+        self.engine = engine
+        state.chdir_project()
+         
 
     def run(self) -> bool:
-        fpaths.chdir_project()
+        self.update()
+        os.system('python manage.py runserver 127.0.0.1:8181')
+        return True 
+
+    def update(self) -> bool:
         os.system('python manage.py makemigrations api')
         os.system('python manage.py migrate')
+        return True
+    
+    def create_admin(self) -> bool:
         os.system('python manage.py createsuperuser --username admin --email admin@local.local --skip-check')
-        os.system('python manage.py runserver 127.0.0.1:8181')
-        
-        return True 
-    
+        return True
```

### Comparing `bfactory-0.4.1/src/bfactory/tests/manifest_test.json` & `bfactory-0.4.2/src/bfactory/tests/manifest_test.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666666%*

 * *Differences: {"'schema'": "{0: {delete: ['perm']}}"}*

```diff
@@ -27,13 +27,12 @@
                 {
                     "default": "",
                     "name": "usuario",
                     "req": true,
                     "type": "owner"
                 }
             ],
-            "name": "Tarea",
-            "perm": "700"
+            "name": "Tarea"
         }
     ],
     "version": "1"
 }
```

### Comparing `bfactory-0.4.1/src/bfactory/tests/run_tests.py` & `bfactory-0.4.2/src/bfactory/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.1/src/bfactory/utils/crypto.py` & `bfactory-0.4.2/src/bfactory/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `bfactory-0.4.1/src/bfactory/utils/paths.py` & `bfactory-0.4.2/src/bfactory/utils/state.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 
 
+from argparse import Namespace
 import os
 import shutil
 from bfactory.inputs import manifest
 from bfactory.inputs.manifest import Manifest
 
 
 class Singleton (type):
     _instances = {}
 
     def __call__(cls, *args, **kwargs):
 
         if cls not in cls._instances:
-            cls._instances[cls] = super(
-                Singleton, cls).__call__(*args, **kwargs)
+            cls._instances[cls] = super(Singleton, cls).__call__(*args, **kwargs)
 
         return cls._instances[cls]
 
 
-class Paths(metaclass=Singleton):
+class State(metaclass=Singleton):
 
-    manifest: Manifest = None
-    to_path: str = ""
+    update = False 
+    run = False 
+    force = False 
+    template = None
+    run_api = False 
+    create_admin = False 
 
-    def __init__(self, manifest: Manifest = None, path: str = ""):
+
+    def init(self, manifest: Manifest = None, path: str = ""):
         self.manifest = manifest
         self.to_path = path
 
     def __str__(self):
         return f"PATH: {self.to_path} MANIFEST: {self.manifest}"
 
     @property
@@ -66,31 +71,44 @@
 
         return os.path.join(self.project, file_name)
 
     def path_file_from_app_api(self, file_name: str) -> str:
 
         return os.path.join(self.path_app_api, file_name)
 
-    def check_path(self, path: str, force: bool) -> bool:
+    def check_path(self) -> bool:
+        
+        
+        if os.path.exists(self.to_path):
+
+            if self.update:
+                print(f"[ W ] >> el path {self.to_path} se va a actualizar")
+                return True
+
 
-        if os.path.exists(path):
-            if force:
-                print(f"[ W ] >> el path {path} se va eliminar primero")
-                shutil.rmtree(path)
+            if self.force or self.update:
+                print(f"[ W ] >> el path {self.to_path} se va eliminar primero")
+                shutil.rmtree(self.to_path)
                 return True
 
-            print(f"[ E ] >> el path {path} existe, usa -f / --force para borrarlo")
+
+            print(f"[ E ] >> el path {self.to_path} existe, usa:\n \t -f [ --force ] para borrarlo\n \t -u [ --update ] si se trata de un update")
             return False
 
         return True
 
     def mk_and_ch_dir(self, path: str) -> None:
         os.mkdir(path)
         os.chdir(path)
     
+    
     def abspath(self, relative_path: str) -> str:
         """
         retorna el path absoluto en base al path de bfactory
         """
         import bfactory
         return os.path.join(os.path.dirname(bfactory.__file__), relative_path)
+    
+    
+    def is_an_update(self):
+        return self.update
```

### Comparing `bfactory-0.4.1/src/bfactory.egg-info/PKG-INFO` & `bfactory-0.4.2/src/bfactory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfactory
-Version: 0.4.1
+Version: 0.4.2
 Summary: Build an API from a manifest file
 Home-page: https://github.com/forkear/bfactory
 Author: Forkear
 Author-email: forkear@no-spam.org
 Project-URL: Documentation, https://github.com/forkear/bfactory/blob/main/README.md
 Project-URL: Source, https://github.com/forkear/bfactory
 Project-URL: Tracker, https://github.com/forkear/bfactory/issues
```

### Comparing `bfactory-0.4.1/src/bfactory.egg-info/SOURCES.txt` & `bfactory-0.4.2/src/bfactory.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 src/bfactory/main.py
 src/bfactory.egg-info/PKG-INFO
 src/bfactory.egg-info/SOURCES.txt
 src/bfactory.egg-info/dependency_links.txt
 src/bfactory.egg-info/entry_points.txt
 src/bfactory.egg-info/requires.txt
 src/bfactory.egg-info/top_level.txt
+src/bfactory/cli/__init__.py
+src/bfactory/cli/django_cli.py
 src/bfactory/config/__init__.py
 src/bfactory/config/settings.py
 src/bfactory/core/__init__.py
 src/bfactory/core/engine.py
 src/bfactory/core/tasks.py
 src/bfactory/core/templates/READ.ME
 src/bfactory/core/templates/admin.py
@@ -29,17 +31,15 @@
 src/bfactory/core/templates/helpers/field_type_linting.py
 src/bfactory/inputs/__init__.py
 src/bfactory/inputs/arguments.py
 src/bfactory/inputs/manifest.py
 src/bfactory/inputs/manifest.schema.json
 src/bfactory/inputs/parse_manifest.py
 src/bfactory/inputs/validators.py
-src/bfactory/startproject/__init__.py
-src/bfactory/startproject/startproject.py
 src/bfactory/tests/__init__.py
 src/bfactory/tests/engine_tests.py
 src/bfactory/tests/manifest_test.json
 src/bfactory/tests/manifest_test.py
 src/bfactory/tests/run_tests.py
 src/bfactory/utils/crypto.py
-src/bfactory/utils/paths.py
-src/bfactory/utils/render.py
+src/bfactory/utils/render.py
+src/bfactory/utils/state.py
```

