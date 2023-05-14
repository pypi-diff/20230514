# Comparing `tmp/liitos-2023.5.13.tar.gz` & `tmp/liitos-2023.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liitos-2023.5.13.tar", last modified: Sun May 14 16:58:08 2023, max compression
+gzip compressed data, was "liitos-2023.5.9.tar", last modified: Tue May  9 21:01:33 2023, max compression
```

## Comparing `liitos-2023.5.13.tar` & `liitos-2023.5.9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-14 16:58:08.095257 liitos-2023.5.13/
--rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 liitos-2023.5.13/LICENSE
--rw-r--r--   0 ruth       (501) staff       (20)       95 2023-01-11 18:32:01.000000 liitos-2023.5.13/MANIFEST.in
--rw-r--r--   0 ruth       (501) staff       (20)     3037 2023-05-14 16:58:08.095104 liitos-2023.5.13/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     2068 2023-03-14 22:27:04.000000 liitos-2023.5.13/README.md
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-14 16:58:08.074148 liitos-2023.5.13/liitos/
--rw-r--r--   0 ruth       (501) staff       (20)     5001 2023-05-14 16:55:51.000000 liitos-2023.5.13/liitos/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)      125 2022-11-23 21:28:47.000000 liitos-2023.5.13/liitos/__main__.py
--rw-r--r--   0 ruth       (501) staff       (20)     3875 2023-02-04 14:18:21.000000 liitos-2023.5.13/liitos/approvals.py
--rw-r--r--   0 ruth       (501) staff       (20)     1825 2023-04-25 19:10:10.000000 liitos-2023.5.13/liitos/captions.py
--rw-r--r--   0 ruth       (501) staff       (20)     4295 2023-02-04 14:18:21.000000 liitos-2023.5.13/liitos/changes.py
--rw-r--r--   0 ruth       (501) staff       (20)    10260 2023-02-07 22:48:13.000000 liitos-2023.5.13/liitos/cli.py
--rw-r--r--   0 ruth       (501) staff       (20)    31810 2023-02-04 14:18:21.000000 liitos-2023.5.13/liitos/concat.py
--rw-r--r--   0 ruth       (501) staff       (20)     1642 2023-01-02 19:46:21.000000 liitos-2023.5.13/liitos/configure.py
--rw-r--r--   0 ruth       (501) staff       (20)     1818 2023-04-25 19:46:43.000000 liitos-2023.5.13/liitos/description_lists.py
--rw-r--r--   0 ruth       (501) staff       (20)     1958 2023-01-02 19:41:38.000000 liitos-2023.5.13/liitos/eject.py
--rw-r--r--   0 ruth       (501) staff       (20)     1688 2023-04-25 19:10:05.000000 liitos-2023.5.13/liitos/figures.py
--rw-r--r--   0 ruth       (501) staff       (20)    11799 2023-01-21 21:35:47.000000 liitos-2023.5.13/liitos/gather.py
--rw-r--r--   0 ruth       (501) staff       (20)     4375 2023-04-25 19:50:27.000000 liitos-2023.5.13/liitos/labels.py
--rw-r--r--   0 ruth       (501) staff       (20)       55 2022-09-17 11:23:46.000000 liitos-2023.5.13/liitos/liitos.py
--rw-r--r--   0 ruth       (501) staff       (20)    41648 2023-02-04 14:18:21.000000 liitos-2023.5.13/liitos/meta.py
--rw-r--r--   0 ruth       (501) staff       (20)      624 2023-01-31 19:15:44.000000 liitos-2023.5.13/liitos/patch.py
--rw-r--r--   0 ruth       (501) staff       (20)    18808 2023-05-09 18:42:29.000000 liitos-2023.5.13/liitos/render.py
--rw-r--r--   0 ruth       (501) staff       (20)    25124 2023-05-10 23:10:37.000000 liitos-2023.5.13/liitos/tables.py
--rw-r--r--   0 ruth       (501) staff       (20)     1489 2023-01-02 19:38:06.000000 liitos-2023.5.13/liitos/template_loader.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-14 16:58:08.083067 liitos-2023.5.13/liitos/templates/
--rw-r--r--   0 ruth       (501) staff       (20)      116 2022-12-01 18:05:38.000000 liitos-2023.5.13/liitos/templates/approvals.yml
--rw-r--r--   0 ruth       (501) staff       (20)     1198 2023-01-17 20:23:10.000000 liitos-2023.5.13/liitos/templates/bookmatter.tex.in
--rw-r--r--   0 ruth       (501) staff       (20)      109 2023-01-17 18:43:02.000000 liitos-2023.5.13/liitos/templates/changes.yml
--rw-r--r--   0 ruth       (501) staff       (20)      889 2023-05-10 17:17:37.000000 liitos-2023.5.13/liitos/templates/driver.tex.in
--rw-r--r--   0 ruth       (501) staff       (20)       97 2022-12-05 14:36:30.000000 liitos-2023.5.13/liitos/templates/meta-patch.yml
--rw-r--r--   0 ruth       (501) staff       (20)     1448 2023-01-17 20:30:00.000000 liitos-2023.5.13/liitos/templates/meta.yml
--rw-r--r--   0 ruth       (501) staff       (20)     2505 2023-01-17 20:37:22.000000 liitos-2023.5.13/liitos/templates/metadata.tex.in
--rw-r--r--   0 ruth       (501) staff       (20)     1538 2022-12-14 16:45:30.000000 liitos-2023.5.13/liitos/templates/mkdocs.yml.in
--rw-r--r--   0 ruth       (501) staff       (20)     1106 2023-05-09 18:17:09.000000 liitos-2023.5.13/liitos/templates/publisher.tex.in
--rw-r--r--   0 ruth       (501) staff       (20)     9709 2023-05-14 16:38:57.000000 liitos-2023.5.13/liitos/templates/setup.tex.in
--rw-r--r--   0 ruth       (501) staff       (20)     7450 2023-01-17 20:39:19.000000 liitos-2023.5.13/liitos/templates/vocabulary.yml
--rw-r--r--   0 ruth       (501) staff       (20)     7497 2023-04-25 19:15:13.000000 liitos-2023.5.13/liitos/tools.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-14 16:58:08.077189 liitos-2023.5.13/liitos.egg-info/
--rw-r--r--   0 ruth       (501) staff       (20)     3037 2023-05-14 16:58:08.000000 liitos-2023.5.13/liitos.egg-info/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     1264 2023-05-14 16:58:08.000000 liitos-2023.5.13/liitos.egg-info/SOURCES.txt
--rw-r--r--   0 ruth       (501) staff       (20)        1 2023-05-14 16:58:08.000000 liitos-2023.5.13/liitos.egg-info/dependency_links.txt
--rw-r--r--   0 ruth       (501) staff       (20)       42 2023-05-14 16:58:08.000000 liitos-2023.5.13/liitos.egg-info/entry_points.txt
--rw-r--r--   0 ruth       (501) staff       (20)      179 2023-05-14 16:58:08.000000 liitos-2023.5.13/liitos.egg-info/requires.txt
--rw-r--r--   0 ruth       (501) staff       (20)       15 2023-05-14 16:58:08.000000 liitos-2023.5.13/liitos.egg-info/top_level.txt
--rw-r--r--   0 ruth       (501) staff       (20)     2692 2023-05-14 16:50:10.000000 liitos-2023.5.13/pyproject.toml
--rw-r--r--   0 ruth       (501) staff       (20)       38 2023-05-14 16:58:08.095293 liitos-2023.5.13/setup.cfg
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-14 16:58:08.094666 liitos-2023.5.13/test/
--rw-r--r--   0 ruth       (501) staff       (20)      499 2022-12-06 21:07:15.000000 liitos-2023.5.13/test/test_approvals.py
--rw-r--r--   0 ruth       (501) staff       (20)     1708 2023-02-07 22:58:06.000000 liitos-2023.5.13/test/test_captions.py
--rw-r--r--   0 ruth       (501) staff       (20)      433 2022-12-06 21:11:22.000000 liitos-2023.5.13/test/test_changes.py
--rw-r--r--   0 ruth       (501) staff       (20)     3720 2023-02-04 14:19:55.000000 liitos-2023.5.13/test/test_cli.py
--rw-r--r--   0 ruth       (501) staff       (20)     6984 2022-12-09 17:00:57.000000 liitos-2023.5.13/test/test_concat.py
--rw-r--r--   0 ruth       (501) staff       (20)     1073 2022-12-05 16:28:35.000000 liitos-2023.5.13/test/test_eject.py
--rw-r--r--   0 ruth       (501) staff       (20)     2689 2022-12-07 18:21:39.000000 liitos-2023.5.13/test/test_figures.py
--rw-r--r--   0 ruth       (501) staff       (20)    10449 2022-11-02 19:26:27.000000 liitos-2023.5.13/test/test_gather.py
--rw-r--r--   0 ruth       (501) staff       (20)     1410 2022-12-05 16:41:47.000000 liitos-2023.5.13/test/test_labels.py
--rw-r--r--   0 ruth       (501) staff       (20)       89 2022-08-01 14:41:37.000000 liitos-2023.5.13/test/test_liitos.py
--rw-r--r--   0 ruth       (501) staff       (20)    15742 2023-02-04 14:19:02.000000 liitos-2023.5.13/test/test_meta.py
--rw-r--r--   0 ruth       (501) staff       (20)      669 2022-12-05 18:19:44.000000 liitos-2023.5.13/test/test_patch.py
--rw-r--r--   0 ruth       (501) staff       (20)      486 2023-01-31 21:27:46.000000 liitos-2023.5.13/test/test_render.py
--rw-r--r--   0 ruth       (501) staff       (20)     3608 2023-05-09 18:14:35.000000 liitos-2023.5.13/test/test_tables.py
--rw-r--r--   0 ruth       (501) staff       (20)      431 2022-12-06 20:22:36.000000 liitos-2023.5.13/test/test_template_loader.py
--rw-r--r--   0 ruth       (501) staff       (20)     1436 2023-01-31 21:28:22.000000 liitos-2023.5.13/test/test_tools.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-09 21:01:33.403590 liitos-2023.5.9/
+-rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 liitos-2023.5.9/LICENSE
+-rw-r--r--   0 ruth       (501) staff       (20)       95 2023-01-11 18:32:01.000000 liitos-2023.5.9/MANIFEST.in
+-rw-r--r--   0 ruth       (501) staff       (20)     3036 2023-05-09 21:01:33.403441 liitos-2023.5.9/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     2068 2023-03-14 22:27:04.000000 liitos-2023.5.9/README.md
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-09 21:01:33.388730 liitos-2023.5.9/liitos/
+-rw-r--r--   0 ruth       (501) staff       (20)     5000 2023-05-09 20:59:17.000000 liitos-2023.5.9/liitos/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)      125 2022-11-23 21:28:47.000000 liitos-2023.5.9/liitos/__main__.py
+-rw-r--r--   0 ruth       (501) staff       (20)     3875 2023-02-04 14:18:21.000000 liitos-2023.5.9/liitos/approvals.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1825 2023-04-25 19:10:10.000000 liitos-2023.5.9/liitos/captions.py
+-rw-r--r--   0 ruth       (501) staff       (20)     4295 2023-02-04 14:18:21.000000 liitos-2023.5.9/liitos/changes.py
+-rw-r--r--   0 ruth       (501) staff       (20)    10260 2023-02-07 22:48:13.000000 liitos-2023.5.9/liitos/cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)    31810 2023-02-04 14:18:21.000000 liitos-2023.5.9/liitos/concat.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1642 2023-01-02 19:46:21.000000 liitos-2023.5.9/liitos/configure.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1818 2023-04-25 19:46:43.000000 liitos-2023.5.9/liitos/description_lists.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1958 2023-01-02 19:41:38.000000 liitos-2023.5.9/liitos/eject.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1688 2023-04-25 19:10:05.000000 liitos-2023.5.9/liitos/figures.py
+-rw-r--r--   0 ruth       (501) staff       (20)    11799 2023-01-21 21:35:47.000000 liitos-2023.5.9/liitos/gather.py
+-rw-r--r--   0 ruth       (501) staff       (20)     4375 2023-04-25 19:50:27.000000 liitos-2023.5.9/liitos/labels.py
+-rw-r--r--   0 ruth       (501) staff       (20)       55 2022-09-17 11:23:46.000000 liitos-2023.5.9/liitos/liitos.py
+-rw-r--r--   0 ruth       (501) staff       (20)    41648 2023-02-04 14:18:21.000000 liitos-2023.5.9/liitos/meta.py
+-rw-r--r--   0 ruth       (501) staff       (20)      624 2023-01-31 19:15:44.000000 liitos-2023.5.9/liitos/patch.py
+-rw-r--r--   0 ruth       (501) staff       (20)    18808 2023-05-09 18:42:29.000000 liitos-2023.5.9/liitos/render.py
+-rw-r--r--   0 ruth       (501) staff       (20)    25061 2023-05-09 20:43:04.000000 liitos-2023.5.9/liitos/tables.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1489 2023-01-02 19:38:06.000000 liitos-2023.5.9/liitos/template_loader.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-09 21:01:33.396442 liitos-2023.5.9/liitos/templates/
+-rw-r--r--   0 ruth       (501) staff       (20)      116 2022-12-01 18:05:38.000000 liitos-2023.5.9/liitos/templates/approvals.yml
+-rw-r--r--   0 ruth       (501) staff       (20)     1198 2023-01-17 20:23:10.000000 liitos-2023.5.9/liitos/templates/bookmatter.tex.in
+-rw-r--r--   0 ruth       (501) staff       (20)      109 2023-01-17 18:43:02.000000 liitos-2023.5.9/liitos/templates/changes.yml
+-rw-r--r--   0 ruth       (501) staff       (20)      853 2022-11-29 20:13:39.000000 liitos-2023.5.9/liitos/templates/driver.tex.in
+-rw-r--r--   0 ruth       (501) staff       (20)       97 2022-12-05 14:36:30.000000 liitos-2023.5.9/liitos/templates/meta-patch.yml
+-rw-r--r--   0 ruth       (501) staff       (20)     1448 2023-01-17 20:30:00.000000 liitos-2023.5.9/liitos/templates/meta.yml
+-rw-r--r--   0 ruth       (501) staff       (20)     2505 2023-01-17 20:37:22.000000 liitos-2023.5.9/liitos/templates/metadata.tex.in
+-rw-r--r--   0 ruth       (501) staff       (20)     1538 2022-12-14 16:45:30.000000 liitos-2023.5.9/liitos/templates/mkdocs.yml.in
+-rw-r--r--   0 ruth       (501) staff       (20)     1106 2023-05-09 18:17:09.000000 liitos-2023.5.9/liitos/templates/publisher.tex.in
+-rw-r--r--   0 ruth       (501) staff       (20)     9709 2023-02-14 22:04:11.000000 liitos-2023.5.9/liitos/templates/setup.tex.in
+-rw-r--r--   0 ruth       (501) staff       (20)     7450 2023-01-17 20:39:19.000000 liitos-2023.5.9/liitos/templates/vocabulary.yml
+-rw-r--r--   0 ruth       (501) staff       (20)     7497 2023-04-25 19:15:13.000000 liitos-2023.5.9/liitos/tools.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-09 21:01:33.391412 liitos-2023.5.9/liitos.egg-info/
+-rw-r--r--   0 ruth       (501) staff       (20)     3036 2023-05-09 21:01:33.000000 liitos-2023.5.9/liitos.egg-info/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     1264 2023-05-09 21:01:33.000000 liitos-2023.5.9/liitos.egg-info/SOURCES.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        1 2023-05-09 21:01:33.000000 liitos-2023.5.9/liitos.egg-info/dependency_links.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       42 2023-05-09 21:01:33.000000 liitos-2023.5.9/liitos.egg-info/entry_points.txt
+-rw-r--r--   0 ruth       (501) staff       (20)      179 2023-05-09 21:01:33.000000 liitos-2023.5.9/liitos.egg-info/requires.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       15 2023-05-09 21:01:33.000000 liitos-2023.5.9/liitos.egg-info/top_level.txt
+-rw-r--r--   0 ruth       (501) staff       (20)     2691 2023-05-09 18:21:47.000000 liitos-2023.5.9/pyproject.toml
+-rw-r--r--   0 ruth       (501) staff       (20)       38 2023-05-09 21:01:33.403627 liitos-2023.5.9/setup.cfg
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-09 21:01:33.403142 liitos-2023.5.9/test/
+-rw-r--r--   0 ruth       (501) staff       (20)      499 2022-12-06 21:07:15.000000 liitos-2023.5.9/test/test_approvals.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1708 2023-02-07 22:58:06.000000 liitos-2023.5.9/test/test_captions.py
+-rw-r--r--   0 ruth       (501) staff       (20)      433 2022-12-06 21:11:22.000000 liitos-2023.5.9/test/test_changes.py
+-rw-r--r--   0 ruth       (501) staff       (20)     3720 2023-02-04 14:19:55.000000 liitos-2023.5.9/test/test_cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)     6984 2022-12-09 17:00:57.000000 liitos-2023.5.9/test/test_concat.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1073 2022-12-05 16:28:35.000000 liitos-2023.5.9/test/test_eject.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2689 2022-12-07 18:21:39.000000 liitos-2023.5.9/test/test_figures.py
+-rw-r--r--   0 ruth       (501) staff       (20)    10449 2022-11-02 19:26:27.000000 liitos-2023.5.9/test/test_gather.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1410 2022-12-05 16:41:47.000000 liitos-2023.5.9/test/test_labels.py
+-rw-r--r--   0 ruth       (501) staff       (20)       89 2022-08-01 14:41:37.000000 liitos-2023.5.9/test/test_liitos.py
+-rw-r--r--   0 ruth       (501) staff       (20)    15742 2023-02-04 14:19:02.000000 liitos-2023.5.9/test/test_meta.py
+-rw-r--r--   0 ruth       (501) staff       (20)      669 2022-12-05 18:19:44.000000 liitos-2023.5.9/test/test_patch.py
+-rw-r--r--   0 ruth       (501) staff       (20)      486 2023-01-31 21:27:46.000000 liitos-2023.5.9/test/test_render.py
+-rw-r--r--   0 ruth       (501) staff       (20)     3608 2023-05-09 18:14:35.000000 liitos-2023.5.9/test/test_tables.py
+-rw-r--r--   0 ruth       (501) staff       (20)      431 2022-12-06 20:22:36.000000 liitos-2023.5.9/test/test_template_loader.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1436 2023-01-31 21:28:22.000000 liitos-2023.5.9/test/test_tools.py
```

### Comparing `liitos-2023.5.13/LICENSE` & `liitos-2023.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/PKG-INFO` & `liitos-2023.5.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liitos
-Version: 2023.5.13
+Version: 2023.5.9
 Summary: Splice (Finnish liitos) contributions.
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/liitos
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/liitos
 Project-URL: Documentation, https://codes.dilettant.life/docs/liitos
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/liitos
```

### Comparing `liitos-2023.5.13/README.md` & `liitos-2023.5.9/README.md`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/liitos/__init__.py` & `liitos-2023.5.9/liitos/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import logging
 import os
 import pathlib
 import shellingham  # type: ignore
 from typing import List, no_type_check
 
 # [[[fill git_describe()]]]
-__version__ = '2023.5.13+parent.a0a02e5f'
-# [[[end]]] (checksum: 15941ff8e71997d08ae2dc303e1f13df)
+__version__ = '2023.5.9+parent.8965a930'
+# [[[end]]] (checksum: 69adc87cceb6f4a1695afccfe3f3f0ff)
 __version_info__ = tuple(
     e if '-' not in e else e.split('-')[0] for part in __version__.split('+') for e in part.split('.') if e != 'parent'
 )
 
 APP_NAME = 'Splice (Finnish liitos) contributions.'
 APP_ALIAS = 'liitos'
 APP_ENV = 'LIITOS'
```

### Comparing `liitos-2023.5.13/liitos/approvals.py` & `liitos-2023.5.9/liitos/approvals.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/liitos/captions.py` & `liitos-2023.5.9/liitos/captions.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/liitos/changes.py` & `liitos-2023.5.9/liitos/changes.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/liitos/cli.py` & `liitos-2023.5.9/liitos/cli.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/liitos/concat.py` & `liitos-2023.5.9/liitos/concat.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/liitos/configure.py` & `liitos-2023.5.9/liitos/configure.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/liitos/description_lists.py` & `liitos-2023.5.9/liitos/description_lists.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/liitos/eject.py` & `liitos-2023.5.9/liitos/eject.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/liitos/figures.py` & `liitos-2023.5.9/liitos/figures.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/liitos/gather.py` & `liitos-2023.5.9/liitos/gather.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/liitos/labels.py` & `liitos-2023.5.9/liitos/labels.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/liitos/meta.py` & `liitos-2023.5.9/liitos/meta.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/liitos/patch.py` & `liitos-2023.5.9/liitos/patch.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/liitos/render.py` & `liitos-2023.5.9/liitos/render.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/liitos/tables.py` & `liitos-2023.5.9/liitos/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -400,24 +400,16 @@
                 continue
 
 
 def parse_table_font_size_command(slot: int, text_line: str) -> tuple[bool, str, str]:
     """Parse the \\tablefontsize=footnotesize command."""
     backslash = '\\'
     known_sizes = (
-        'tiny',
-        'scriptsize',
-        'footnotesize',
-        'small',
-        'normalsize',
-        'large',
-        'Large',
-        'LARGE',
-        'huge',
-        'Huge',
+        'tiny', 'scriptsize', 'footnotesize', 'small', 'normalsize',
+        'large', 'Large', 'LARGE', 'huge', 'Huge',
     )
     if text_line.startswith(r'\tablefontsize='):
         log.info(f'trigger a fontsize mod for the next table environment at line #{slot + 1}|{text_line}')
         try:
             font_size = text_line.split('=', 1)[1].strip()  # r'\tablefontsize=Huge'  --> 'Huge'
             if font_size.startswith(backslash):
                 font_size = font_size.lstrip(backslash)
@@ -462,14 +454,15 @@
     has_column = False
     has_font_size = False
     widths: list[float] = []
     font_size = ''
     comment_outs = []
     for n, text in enumerate(incoming):
         if not table_section:
+
             if not has_font_size:
                 has_font_size, text_line, font_size = parse_table_font_size_command(n, text)
                 if has_font_size:
                     comment_outs.append(n)
             if not has_font_size:
                 continue
```

### Comparing `liitos-2023.5.13/liitos/template_loader.py` & `liitos-2023.5.9/liitos/template_loader.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/liitos/templates/bookmatter.tex.in` & `liitos-2023.5.9/liitos/templates/bookmatter.tex.in`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/liitos/templates/driver.tex.in` & `liitos-2023.5.9/liitos/templates/driver.tex.in`

 * *Files 22% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 \usepackage{xassoccnt}
 \NewTotalDocumentCounter{totalfigures}
 \NewTotalDocumentCounter{totaltables}
 \NewTotalDocumentCounter{appendixchapters}
 \DeclareAssociatedCounters{figure}{totalfigures}
 \DeclareAssociatedCounters{table}{totaltables}
 
-\setkomafont{caption}{\normalsize}
-
 \begin{document}
 \include{bookmatter.tex}
 
 \pagestyle{liitos-header-footer}
 \newpage
 \include{publisher.tex}
```

### Comparing `liitos-2023.5.13/liitos/templates/meta.yml` & `liitos-2023.5.9/liitos/templates/meta.yml`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/liitos/templates/metadata.tex.in` & `liitos-2023.5.9/liitos/templates/metadata.tex.in`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/liitos/templates/mkdocs.yml.in` & `liitos-2023.5.9/liitos/templates/mkdocs.yml.in`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/liitos/templates/publisher.tex.in` & `liitos-2023.5.9/liitos/templates/publisher.tex.in`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/liitos/templates/setup.tex.in` & `liitos-2023.5.9/liitos/templates/setup.tex.in`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
 % Hook to inject chosen logo
 \newcommand{\theChosenLogo}{VALUE.SLOT}%%_PATCH_%_CHOSEN_%_LOGO_%%
 % The liitos "Normal" pages header and footer style:
 \newpairofpagestyles{liitos-header-footer}{%%
   \clearpairofpagestyles
   \ihead*{%%
     \upshape
-    \begin{tabular*}{117mm}[t]{@{}p{55mm}p{35mm}p{25mm}@{}}%% ... tuned ... effective 115mm
+    \begin{tabular*}{116mm}[t]{@{}p{55mm}p{35mm}p{25mm}@{}}%% ... tuned ... effective 115mm
      \strut \\
       \multicolumn{3}{l}{\hskip -0.6em \LARGE\theMetaTitle} \hfill \strut \\%% ... tuned the hskip to align left without gap
       \hline {\footnotesize \textbf{\theMetaType}} \hfill & \hfill & \hfill \strut \\
       \hline {\footnotesize \theMetaDocIdLabel} \hfill & {\footnotesize \theMetaIssRevLabel} \hfill & {\footnotesize \theMetaDateLabel} \hfill \strut \\
       {\footnotesize \theMetaDocId} \hfill & {\footnotesize \theMetaIssRev} \hfill & {\footnotesize \theMetaDate} \hfill \strut \\
     \end{tabular*}
   }
```

### Comparing `liitos-2023.5.13/liitos/templates/vocabulary.yml` & `liitos-2023.5.9/liitos/templates/vocabulary.yml`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/liitos/tools.py` & `liitos-2023.5.9/liitos/tools.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/liitos.egg-info/PKG-INFO` & `liitos-2023.5.9/liitos.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liitos
-Version: 2023.5.13
+Version: 2023.5.9
 Summary: Splice (Finnish liitos) contributions.
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/liitos
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/liitos
 Project-URL: Documentation, https://codes.dilettant.life/docs/liitos
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/liitos
```

### Comparing `liitos-2023.5.13/liitos.egg-info/SOURCES.txt` & `liitos-2023.5.9/liitos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/pyproject.toml` & `liitos-2023.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "liitos"
-version = "2023.5.13"
+version = "2023.5.9"
 description = "Splice (Finnish liitos) contributions."
 readme = "README.md"
 authors = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 maintainers = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `liitos-2023.5.13/test/test_captions.py` & `liitos-2023.5.9/test/test_captions.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/test/test_cli.py` & `liitos-2023.5.9/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/test/test_concat.py` & `liitos-2023.5.9/test/test_concat.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/test/test_eject.py` & `liitos-2023.5.9/test/test_eject.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/test/test_figures.py` & `liitos-2023.5.9/test/test_figures.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/test/test_gather.py` & `liitos-2023.5.9/test/test_gather.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/test/test_labels.py` & `liitos-2023.5.9/test/test_labels.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/test/test_meta.py` & `liitos-2023.5.9/test/test_meta.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/test/test_patch.py` & `liitos-2023.5.9/test/test_patch.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/test/test_tables.py` & `liitos-2023.5.9/test/test_tables.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.5.13/test/test_tools.py` & `liitos-2023.5.9/test/test_tools.py`

 * *Files identical despite different names*

