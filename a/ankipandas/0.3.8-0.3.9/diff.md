# Comparing `tmp/ankipandas-0.3.8.tar.gz` & `tmp/ankipandas-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ankipandas-0.3.8.tar", last modified: Sun Dec  6 12:56:14 2020, max compression
+gzip compressed data, was "dist/ankipandas-0.3.9.tar", last modified: Thu Dec 17 11:46:11 2020, max compression
```

## Comparing `ankipandas-0.3.8.tar` & `ankipandas-0.3.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 fuchur    (1000) fuchur    (1000)        0 2020-12-06 12:56:14.000000 ankipandas-0.3.8/
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)    12632 2020-12-06 12:56:14.000000 ankipandas-0.3.8/PKG-INFO
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)    10036 2020-12-06 12:56:00.000000 ankipandas-0.3.8/README.md
-drwxr-xr-x   0 fuchur    (1000) fuchur    (1000)        0 2020-12-06 12:56:14.000000 ankipandas-0.3.8/ankipandas/
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)      359 2020-12-05 17:02:42.000000 ankipandas-0.3.8/ankipandas/__init__.py
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)     3725 2020-11-28 14:59:25.000000 ankipandas-0.3.8/ankipandas/_columns.py
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)    72824 2020-12-06 11:27:15.000000 ankipandas-0.3.8/ankipandas/ankidf.py
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)    13181 2020-12-06 12:54:00.000000 ankipandas-0.3.8/ankipandas/collection.py
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)       99 2020-12-06 10:48:56.000000 ankipandas-0.3.8/ankipandas/conftest.py
-drwxr-xr-x   0 fuchur    (1000) fuchur    (1000)        0 2020-12-06 12:56:14.000000 ankipandas-0.3.8/ankipandas/data/
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)     5478 2020-01-09 18:40:17.000000 ankipandas-0.3.8/ankipandas/data/anki_fields.csv
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)     9260 2020-12-06 12:01:53.000000 ankipandas-0.3.8/ankipandas/paths.py
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)    14681 2020-12-06 12:14:56.000000 ankipandas-0.3.8/ankipandas/raw.py
-drwxr-xr-x   0 fuchur    (1000) fuchur    (1000)        0 2020-12-06 12:56:14.000000 ankipandas-0.3.8/ankipandas/test/
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)        0 2020-01-09 18:40:17.000000 ankipandas-0.3.8/ankipandas/test/__init__.py
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)    35967 2020-12-05 16:26:09.000000 ankipandas-0.3.8/ankipandas/test/test_ankidf.py
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)     3456 2020-12-06 11:20:07.000000 ankipandas-0.3.8/ankipandas/test/test_collection.py
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)     6351 2020-12-05 16:45:25.000000 ankipandas-0.3.8/ankipandas/test/test_paths.py
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)     9686 2020-12-05 16:26:09.000000 ankipandas-0.3.8/ankipandas/test/test_raw.py
--rwxr-xr-x   0 fuchur    (1000) fuchur    (1000)      489 2020-12-06 11:35:42.000000 ankipandas-0.3.8/ankipandas/test/test_regression.py
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)      397 2020-12-06 11:19:28.000000 ankipandas-0.3.8/ankipandas/test/util.py
-drwxr-xr-x   0 fuchur    (1000) fuchur    (1000)        0 2020-12-06 12:56:14.000000 ankipandas-0.3.8/ankipandas/util/
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)      298 2020-12-05 15:42:10.000000 ankipandas-0.3.8/ankipandas/util/__init__.py
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)     2025 2020-01-09 18:40:17.000000 ankipandas-0.3.8/ankipandas/util/checksum.py
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)     5151 2020-12-06 11:34:04.000000 ankipandas-0.3.8/ankipandas/util/dataframe.py
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)      698 2020-01-09 18:40:17.000000 ankipandas-0.3.8/ankipandas/util/guid.py
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)     1601 2020-12-05 16:24:24.000000 ankipandas-0.3.8/ankipandas/util/log.py
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)     1449 2020-08-26 12:48:26.000000 ankipandas-0.3.8/ankipandas/util/misc.py
-drwxr-xr-x   0 fuchur    (1000) fuchur    (1000)        0 2020-12-06 12:56:14.000000 ankipandas-0.3.8/ankipandas/util/test/
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)        0 2020-01-09 18:40:17.000000 ankipandas-0.3.8/ankipandas/util/test/__init__.py
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)      538 2020-01-09 18:40:17.000000 ankipandas-0.3.8/ankipandas/util/test/test_dataframe.py
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)      593 2020-01-09 18:40:17.000000 ankipandas-0.3.8/ankipandas/util/test/test_log.py
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)      433 2020-01-09 18:40:17.000000 ankipandas-0.3.8/ankipandas/util/test/test_misc.py
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)     1164 2020-12-05 16:26:46.000000 ankipandas-0.3.8/ankipandas/util/test/test_types.py
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)      663 2020-01-09 18:40:17.000000 ankipandas-0.3.8/ankipandas/util/types.py
-drwxr-xr-x   0 fuchur    (1000) fuchur    (1000)        0 2020-12-06 12:56:14.000000 ankipandas-0.3.8/ankipandas.egg-info/
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)    12632 2020-12-06 12:56:14.000000 ankipandas-0.3.8/ankipandas.egg-info/PKG-INFO
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)      963 2020-12-06 12:56:14.000000 ankipandas-0.3.8/ankipandas.egg-info/SOURCES.txt
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)        1 2020-12-06 12:56:14.000000 ankipandas-0.3.8/ankipandas.egg-info/dependency_links.txt
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)       37 2020-12-06 12:56:14.000000 ankipandas-0.3.8/ankipandas.egg-info/requires.txt
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)       11 2020-12-06 12:56:14.000000 ankipandas-0.3.8/ankipandas.egg-info/top_level.txt
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)       56 2020-01-09 18:40:17.000000 ankipandas-0.3.8/pyproject.toml
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)       80 2020-12-06 12:56:14.000000 ankipandas-0.3.8/setup.cfg
--rw-r--r--   0 fuchur    (1000) fuchur    (1000)     2245 2020-12-05 15:27:51.000000 ankipandas-0.3.8/setup.py
+drwxr-xr-x   0 fuchur    (1000) fuchur    (1000)        0 2020-12-17 11:46:11.000000 ankipandas-0.3.9/
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)    12986 2020-12-17 11:46:11.000000 ankipandas-0.3.9/PKG-INFO
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)    10382 2020-12-16 16:15:51.000000 ankipandas-0.3.9/README.md
+drwxr-xr-x   0 fuchur    (1000) fuchur    (1000)        0 2020-12-17 11:46:11.000000 ankipandas-0.3.9/ankipandas/
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)     1033 2020-12-17 11:39:15.000000 ankipandas-0.3.9/ankipandas/__init__.py
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)     3725 2020-11-28 14:59:25.000000 ankipandas-0.3.9/ankipandas/_columns.py
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)    72824 2020-12-06 11:27:15.000000 ankipandas-0.3.9/ankipandas/ankidf.py
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)    13181 2020-12-06 12:54:00.000000 ankipandas-0.3.9/ankipandas/collection.py
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)       99 2020-12-06 10:48:56.000000 ankipandas-0.3.9/ankipandas/conftest.py
+drwxr-xr-x   0 fuchur    (1000) fuchur    (1000)        0 2020-12-17 11:46:11.000000 ankipandas-0.3.9/ankipandas/data/
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)     5478 2020-01-09 18:40:17.000000 ankipandas-0.3.9/ankipandas/data/anki_fields.csv
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)     9260 2020-12-06 12:01:53.000000 ankipandas-0.3.9/ankipandas/paths.py
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)    14681 2020-12-06 12:14:56.000000 ankipandas-0.3.9/ankipandas/raw.py
+drwxr-xr-x   0 fuchur    (1000) fuchur    (1000)        0 2020-12-17 11:46:11.000000 ankipandas-0.3.9/ankipandas/test/
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)        0 2020-01-09 18:40:17.000000 ankipandas-0.3.9/ankipandas/test/__init__.py
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)    35967 2020-12-05 16:26:09.000000 ankipandas-0.3.9/ankipandas/test/test_ankidf.py
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)     3456 2020-12-06 11:20:07.000000 ankipandas-0.3.9/ankipandas/test/test_collection.py
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)     6351 2020-12-05 16:45:25.000000 ankipandas-0.3.9/ankipandas/test/test_paths.py
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)     9686 2020-12-05 16:26:09.000000 ankipandas-0.3.9/ankipandas/test/test_raw.py
+-rwxr-xr-x   0 fuchur    (1000) fuchur    (1000)      489 2020-12-06 11:35:42.000000 ankipandas-0.3.9/ankipandas/test/test_regression.py
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)      397 2020-12-06 11:19:28.000000 ankipandas-0.3.9/ankipandas/test/util.py
+drwxr-xr-x   0 fuchur    (1000) fuchur    (1000)        0 2020-12-17 11:46:11.000000 ankipandas-0.3.9/ankipandas/util/
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)      298 2020-12-05 15:42:10.000000 ankipandas-0.3.9/ankipandas/util/__init__.py
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)     2025 2020-01-09 18:40:17.000000 ankipandas-0.3.9/ankipandas/util/checksum.py
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)     5151 2020-12-06 11:34:04.000000 ankipandas-0.3.9/ankipandas/util/dataframe.py
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)      698 2020-01-09 18:40:17.000000 ankipandas-0.3.9/ankipandas/util/guid.py
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)     1601 2020-12-05 16:24:24.000000 ankipandas-0.3.9/ankipandas/util/log.py
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)     1449 2020-08-26 12:48:26.000000 ankipandas-0.3.9/ankipandas/util/misc.py
+drwxr-xr-x   0 fuchur    (1000) fuchur    (1000)        0 2020-12-17 11:46:11.000000 ankipandas-0.3.9/ankipandas/util/test/
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)        0 2020-01-09 18:40:17.000000 ankipandas-0.3.9/ankipandas/util/test/__init__.py
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)      538 2020-01-09 18:40:17.000000 ankipandas-0.3.9/ankipandas/util/test/test_dataframe.py
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)      593 2020-01-09 18:40:17.000000 ankipandas-0.3.9/ankipandas/util/test/test_log.py
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)      433 2020-01-09 18:40:17.000000 ankipandas-0.3.9/ankipandas/util/test/test_misc.py
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)     1164 2020-12-05 16:26:46.000000 ankipandas-0.3.9/ankipandas/util/test/test_types.py
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)      663 2020-01-09 18:40:17.000000 ankipandas-0.3.9/ankipandas/util/types.py
+drwxr-xr-x   0 fuchur    (1000) fuchur    (1000)        0 2020-12-17 11:46:11.000000 ankipandas-0.3.9/ankipandas.egg-info/
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)    12986 2020-12-17 11:46:11.000000 ankipandas-0.3.9/ankipandas.egg-info/PKG-INFO
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)      963 2020-12-17 11:46:11.000000 ankipandas-0.3.9/ankipandas.egg-info/SOURCES.txt
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)        1 2020-12-17 11:46:11.000000 ankipandas-0.3.9/ankipandas.egg-info/dependency_links.txt
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)       37 2020-12-17 11:46:11.000000 ankipandas-0.3.9/ankipandas.egg-info/requires.txt
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)       11 2020-12-17 11:46:11.000000 ankipandas-0.3.9/ankipandas.egg-info/top_level.txt
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)       56 2020-01-09 18:40:17.000000 ankipandas-0.3.9/pyproject.toml
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)       80 2020-12-17 11:46:11.000000 ankipandas-0.3.9/setup.cfg
+-rw-r--r--   0 fuchur    (1000) fuchur    (1000)     2245 2020-12-05 15:27:51.000000 ankipandas-0.3.9/setup.py
```

### Comparing `ankipandas-0.3.8/PKG-INFO` & `ankipandas-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ankipandas
-Version: 0.3.8
+Version: 0.3.9
 Summary: Load your anki database as a pandas DataFrame with just one line of code!
 Home-page: https://github.com/klieret/ankipandas
 License: MIT
 Project-URL: Bug Tracker, https://github.com/klieret/ankipandas/issues
 Project-URL: Documentation, https://ankipandas.readthedocs.io/
 Project-URL: Source Code, https://github.com/klieret/ankipandas/
 Description: # Analyze and manipulate your Anki collection using pandas!
         
         <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-        [![All Contributors](https://img.shields.io/badge/all_contributors-3-orange.svg?style=flat-square)](#contributors-)
+        [![All Contributors](https://img.shields.io/badge/all_contributors-5-orange.svg?style=flat-square)](#contributors-)
         <!-- ALL-CONTRIBUTORS-BADGE:END -->
-        ![gh actions](https://github.com/klieret/AnkiPandas/workflows/testing/badge.svg)
+        [![gh actions](https://github.com/klieret/AnkiPandas/workflows/testing/badge.svg)](https://github.com/klieret/AnkiPandas/actions)
         [![Coveralls](https://coveralls.io/repos/github/klieret/AnkiPandas/badge.svg?branch=master)](https://coveralls.io/github/klieret/AnkiPandas?branch=master)
         [![Documentation Status](https://readthedocs.org/projects/ankipandas/badge/?version=latest)](https://ankipandas.readthedocs.io/)
         [![Pypi status](https://badge.fury.io/py/ankipandas.svg)](https://pypi.org/project/ankipandas/)
         [![Gitter](https://img.shields.io/gitter/room/ankipandas/community.svg)](https://gitter.im/ankipandas/community)
         [![License](https://img.shields.io/github/license/klieret/ankipandas.svg)](https://github.com/klieret/ankipandas/blob/master/LICENSE.txt)
         [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
         
@@ -227,14 +227,15 @@
         <!-- markdownlint-disable -->
         <table>
           <tr>
             <td align="center"><a href="https://github.com/exc4l"><img src="https://avatars3.githubusercontent.com/u/74188442?v=4" width="100px;" alt=""/><br /><sub><b>exc4l</b></sub></a><br /><a href="https://github.com/klieret/AnkiPandas/issues?q=author%3Aexc4l" title="Bug reports">🐛</a> <a href="https://github.com/klieret/AnkiPandas/commits?author=exc4l" title="Code">💻</a></td>
             <td align="center"><a href="https://github.com/CalculusAce"><img src="https://avatars3.githubusercontent.com/u/42630988?v=4" width="100px;" alt=""/><br /><sub><b>CalculusAce</b></sub></a><br /><a href="https://github.com/klieret/AnkiPandas/issues?q=author%3ACalculusAce" title="Bug reports">🐛</a></td>
             <td align="center"><a href="http://thomasbrownback.com/"><img src="https://avatars2.githubusercontent.com/u/26754?v=4" width="100px;" alt=""/><br /><sub><b>Thomas Brownback</b></sub></a><br /><a href="https://github.com/klieret/AnkiPandas/issues?q=author%3Abrownbat" title="Bug reports">🐛</a></td>
             <td align="center"><a href="https://github.com/p4nix"><img src="https://avatars1.githubusercontent.com/u/7038116?v=4" width="100px;" alt=""/><br /><sub><b>p4nix</b></sub></a><br /><a href="https://github.com/klieret/AnkiPandas/issues?q=author%3Ap4nix" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://github.com/eumiro"><img src="https://avatars0.githubusercontent.com/u/6774676?v=4" width="100px;" alt=""/><br /><sub><b>Miroslav Šedivý</b></sub></a><br /><a href="https://github.com/klieret/AnkiPandas/commits?author=eumiro" title="Tests">⚠️</a></td>
           </tr>
         </table>
         
         <!-- markdownlint-enable -->
         <!-- prettier-ignore-end -->
         <!-- ALL-CONTRIBUTORS-LIST:END -->
```

### Comparing `ankipandas-0.3.8/README.md` & `ankipandas-0.3.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Analyze and manipulate your Anki collection using pandas!
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-3-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-5-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
-![gh actions](https://github.com/klieret/AnkiPandas/workflows/testing/badge.svg)
+[![gh actions](https://github.com/klieret/AnkiPandas/workflows/testing/badge.svg)](https://github.com/klieret/AnkiPandas/actions)
 [![Coveralls](https://coveralls.io/repos/github/klieret/AnkiPandas/badge.svg?branch=master)](https://coveralls.io/github/klieret/AnkiPandas?branch=master)
 [![Documentation Status](https://readthedocs.org/projects/ankipandas/badge/?version=latest)](https://ankipandas.readthedocs.io/)
 [![Pypi status](https://badge.fury.io/py/ankipandas.svg)](https://pypi.org/project/ankipandas/)
 [![Gitter](https://img.shields.io/gitter/room/ankipandas/community.svg)](https://gitter.im/ankipandas/community)
 [![License](https://img.shields.io/github/license/klieret/ankipandas.svg)](https://github.com/klieret/ankipandas/blob/master/LICENSE.txt)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 
@@ -218,14 +218,15 @@
 <!-- markdownlint-disable -->
 <table>
   <tr>
     <td align="center"><a href="https://github.com/exc4l"><img src="https://avatars3.githubusercontent.com/u/74188442?v=4" width="100px;" alt=""/><br /><sub><b>exc4l</b></sub></a><br /><a href="https://github.com/klieret/AnkiPandas/issues?q=author%3Aexc4l" title="Bug reports">🐛</a> <a href="https://github.com/klieret/AnkiPandas/commits?author=exc4l" title="Code">💻</a></td>
     <td align="center"><a href="https://github.com/CalculusAce"><img src="https://avatars3.githubusercontent.com/u/42630988?v=4" width="100px;" alt=""/><br /><sub><b>CalculusAce</b></sub></a><br /><a href="https://github.com/klieret/AnkiPandas/issues?q=author%3ACalculusAce" title="Bug reports">🐛</a></td>
     <td align="center"><a href="http://thomasbrownback.com/"><img src="https://avatars2.githubusercontent.com/u/26754?v=4" width="100px;" alt=""/><br /><sub><b>Thomas Brownback</b></sub></a><br /><a href="https://github.com/klieret/AnkiPandas/issues?q=author%3Abrownbat" title="Bug reports">🐛</a></td>
     <td align="center"><a href="https://github.com/p4nix"><img src="https://avatars1.githubusercontent.com/u/7038116?v=4" width="100px;" alt=""/><br /><sub><b>p4nix</b></sub></a><br /><a href="https://github.com/klieret/AnkiPandas/issues?q=author%3Ap4nix" title="Bug reports">🐛</a></td>
+    <td align="center"><a href="https://github.com/eumiro"><img src="https://avatars0.githubusercontent.com/u/6774676?v=4" width="100px;" alt=""/><br /><sub><b>Miroslav Šedivý</b></sub></a><br /><a href="https://github.com/klieret/AnkiPandas/commits?author=eumiro" title="Tests">⚠️</a></td>
   </tr>
 </table>
 
 <!-- markdownlint-enable -->
 <!-- prettier-ignore-end -->
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

### Comparing `ankipandas-0.3.8/ankipandas/_columns.py` & `ankipandas-0.3.9/ankipandas/_columns.py`

 * *Files identical despite different names*

### Comparing `ankipandas-0.3.8/ankipandas/ankidf.py` & `ankipandas-0.3.9/ankipandas/ankidf.py`

 * *Files identical despite different names*

### Comparing `ankipandas-0.3.8/ankipandas/collection.py` & `ankipandas-0.3.9/ankipandas/collection.py`

 * *Files identical despite different names*

### Comparing `ankipandas-0.3.8/ankipandas/data/anki_fields.csv` & `ankipandas-0.3.9/ankipandas/data/anki_fields.csv`

 * *Files identical despite different names*

### Comparing `ankipandas-0.3.8/ankipandas/paths.py` & `ankipandas-0.3.9/ankipandas/paths.py`

 * *Files identical despite different names*

### Comparing `ankipandas-0.3.8/ankipandas/raw.py` & `ankipandas-0.3.9/ankipandas/raw.py`

 * *Files identical despite different names*

### Comparing `ankipandas-0.3.8/ankipandas/test/test_ankidf.py` & `ankipandas-0.3.9/ankipandas/test/test_ankidf.py`

 * *Files identical despite different names*

### Comparing `ankipandas-0.3.8/ankipandas/test/test_collection.py` & `ankipandas-0.3.9/ankipandas/test/test_collection.py`

 * *Files identical despite different names*

### Comparing `ankipandas-0.3.8/ankipandas/test/test_paths.py` & `ankipandas-0.3.9/ankipandas/test/test_paths.py`

 * *Files identical despite different names*

### Comparing `ankipandas-0.3.8/ankipandas/test/test_raw.py` & `ankipandas-0.3.9/ankipandas/test/test_raw.py`

 * *Files identical despite different names*

### Comparing `ankipandas-0.3.8/ankipandas/util/checksum.py` & `ankipandas-0.3.9/ankipandas/util/checksum.py`

 * *Files identical despite different names*

### Comparing `ankipandas-0.3.8/ankipandas/util/dataframe.py` & `ankipandas-0.3.9/ankipandas/util/dataframe.py`

 * *Files identical despite different names*

### Comparing `ankipandas-0.3.8/ankipandas/util/guid.py` & `ankipandas-0.3.9/ankipandas/util/guid.py`

 * *Files identical despite different names*

### Comparing `ankipandas-0.3.8/ankipandas/util/log.py` & `ankipandas-0.3.9/ankipandas/util/log.py`

 * *Files identical despite different names*

### Comparing `ankipandas-0.3.8/ankipandas/util/misc.py` & `ankipandas-0.3.9/ankipandas/util/misc.py`

 * *Files identical despite different names*

### Comparing `ankipandas-0.3.8/ankipandas/util/test/test_dataframe.py` & `ankipandas-0.3.9/ankipandas/util/test/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `ankipandas-0.3.8/ankipandas/util/test/test_log.py` & `ankipandas-0.3.9/ankipandas/util/test/test_log.py`

 * *Files identical despite different names*

### Comparing `ankipandas-0.3.8/ankipandas/util/test/test_types.py` & `ankipandas-0.3.9/ankipandas/util/test/test_types.py`

 * *Files identical despite different names*

### Comparing `ankipandas-0.3.8/ankipandas/util/types.py` & `ankipandas-0.3.9/ankipandas/util/types.py`

 * *Files identical despite different names*

### Comparing `ankipandas-0.3.8/ankipandas.egg-info/PKG-INFO` & `ankipandas-0.3.9/ankipandas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ankipandas
-Version: 0.3.8
+Version: 0.3.9
 Summary: Load your anki database as a pandas DataFrame with just one line of code!
 Home-page: https://github.com/klieret/ankipandas
 License: MIT
 Project-URL: Bug Tracker, https://github.com/klieret/ankipandas/issues
 Project-URL: Documentation, https://ankipandas.readthedocs.io/
 Project-URL: Source Code, https://github.com/klieret/ankipandas/
 Description: # Analyze and manipulate your Anki collection using pandas!
         
         <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-        [![All Contributors](https://img.shields.io/badge/all_contributors-3-orange.svg?style=flat-square)](#contributors-)
+        [![All Contributors](https://img.shields.io/badge/all_contributors-5-orange.svg?style=flat-square)](#contributors-)
         <!-- ALL-CONTRIBUTORS-BADGE:END -->
-        ![gh actions](https://github.com/klieret/AnkiPandas/workflows/testing/badge.svg)
+        [![gh actions](https://github.com/klieret/AnkiPandas/workflows/testing/badge.svg)](https://github.com/klieret/AnkiPandas/actions)
         [![Coveralls](https://coveralls.io/repos/github/klieret/AnkiPandas/badge.svg?branch=master)](https://coveralls.io/github/klieret/AnkiPandas?branch=master)
         [![Documentation Status](https://readthedocs.org/projects/ankipandas/badge/?version=latest)](https://ankipandas.readthedocs.io/)
         [![Pypi status](https://badge.fury.io/py/ankipandas.svg)](https://pypi.org/project/ankipandas/)
         [![Gitter](https://img.shields.io/gitter/room/ankipandas/community.svg)](https://gitter.im/ankipandas/community)
         [![License](https://img.shields.io/github/license/klieret/ankipandas.svg)](https://github.com/klieret/ankipandas/blob/master/LICENSE.txt)
         [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
         
@@ -227,14 +227,15 @@
         <!-- markdownlint-disable -->
         <table>
           <tr>
             <td align="center"><a href="https://github.com/exc4l"><img src="https://avatars3.githubusercontent.com/u/74188442?v=4" width="100px;" alt=""/><br /><sub><b>exc4l</b></sub></a><br /><a href="https://github.com/klieret/AnkiPandas/issues?q=author%3Aexc4l" title="Bug reports">🐛</a> <a href="https://github.com/klieret/AnkiPandas/commits?author=exc4l" title="Code">💻</a></td>
             <td align="center"><a href="https://github.com/CalculusAce"><img src="https://avatars3.githubusercontent.com/u/42630988?v=4" width="100px;" alt=""/><br /><sub><b>CalculusAce</b></sub></a><br /><a href="https://github.com/klieret/AnkiPandas/issues?q=author%3ACalculusAce" title="Bug reports">🐛</a></td>
             <td align="center"><a href="http://thomasbrownback.com/"><img src="https://avatars2.githubusercontent.com/u/26754?v=4" width="100px;" alt=""/><br /><sub><b>Thomas Brownback</b></sub></a><br /><a href="https://github.com/klieret/AnkiPandas/issues?q=author%3Abrownbat" title="Bug reports">🐛</a></td>
             <td align="center"><a href="https://github.com/p4nix"><img src="https://avatars1.githubusercontent.com/u/7038116?v=4" width="100px;" alt=""/><br /><sub><b>p4nix</b></sub></a><br /><a href="https://github.com/klieret/AnkiPandas/issues?q=author%3Ap4nix" title="Bug reports">🐛</a></td>
+            <td align="center"><a href="https://github.com/eumiro"><img src="https://avatars0.githubusercontent.com/u/6774676?v=4" width="100px;" alt=""/><br /><sub><b>Miroslav Šedivý</b></sub></a><br /><a href="https://github.com/klieret/AnkiPandas/commits?author=eumiro" title="Tests">⚠️</a></td>
           </tr>
         </table>
         
         <!-- markdownlint-enable -->
         <!-- prettier-ignore-end -->
         <!-- ALL-CONTRIBUTORS-LIST:END -->
```

### Comparing `ankipandas-0.3.8/ankipandas.egg-info/SOURCES.txt` & `ankipandas-0.3.9/ankipandas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ankipandas-0.3.8/setup.py` & `ankipandas-0.3.9/setup.py`

 * *Files identical despite different names*

