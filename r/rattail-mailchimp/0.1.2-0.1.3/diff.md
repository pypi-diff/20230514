# Comparing `tmp/rattail-mailchimp-0.1.2.tar.gz` & `tmp/rattail-mailchimp-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/lance/src/rattail-mailchimp/dist/tmpxqftskk1/rattail-mailchimp-0.1.2.tar", last modified: Wed Feb 22 01:22:42 2023, max compression
+gzip compressed data, was "/home/lance/src/rattail-mailchimp/dist/tmps5m1snsm/rattail-mailchimp-0.1.3.tar", last modified: Sat May 13 22:49:44 2023, max compression
```

## Comparing `rattail-mailchimp-0.1.2.tar` & `rattail-mailchimp-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:22:42.000000 rattail-mailchimp-0.1.2/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:22:42.000000 rattail-mailchimp-0.1.2/rattail_mailchimp.egg-info/
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-02-22 01:22:42.000000 rattail-mailchimp-0.1.2/rattail_mailchimp.egg-info/dependency_links.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-02-22 01:22:41.000000 rattail-mailchimp-0.1.2/rattail_mailchimp.egg-info/not-zip-safe
--rw-r--r--   0 lance     (1000) lance     (1000)      712 2023-02-22 01:22:42.000000 rattail-mailchimp-0.1.2/rattail_mailchimp.egg-info/SOURCES.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      145 2023-02-22 01:22:42.000000 rattail-mailchimp-0.1.2/rattail_mailchimp.egg-info/entry_points.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       19 2023-02-22 01:22:42.000000 rattail-mailchimp-0.1.2/rattail_mailchimp.egg-info/requires.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       18 2023-02-22 01:22:42.000000 rattail-mailchimp-0.1.2/rattail_mailchimp.egg-info/top_level.txt
--rw-r--r--   0 lance     (1000) lance     (1000)     1155 2023-02-22 01:22:42.000000 rattail-mailchimp-0.1.2/rattail_mailchimp.egg-info/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)       95 2021-11-08 02:57:23.000000 rattail-mailchimp-0.1.2/MANIFEST.in
--rw-r--r--   0 lance     (1000) lance     (1000)     3887 2022-08-07 02:44:14.000000 rattail-mailchimp-0.1.2/setup.py
--rw-r--r--   0 lance     (1000) lance     (1000)       38 2023-02-22 01:22:42.000000 rattail-mailchimp-0.1.2/setup.cfg
--rw-r--r--   0 lance     (1000) lance     (1000)    35147 2017-07-07 15:32:34.000000 rattail-mailchimp-0.1.2/COPYING.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      347 2021-11-08 17:08:16.000000 rattail-mailchimp-0.1.2/README.rst
--rw-r--r--   0 lance     (1000) lance     (1000)      540 2023-02-22 01:21:28.000000 rattail-mailchimp-0.1.2/CHANGELOG.md
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:22:42.000000 rattail-mailchimp-0.1.2/rattail_mailchimp/
--rw-r--r--   0 lance     (1000) lance     (1000)     1689 2021-11-08 19:18:10.000000 rattail-mailchimp-0.1.2/rattail_mailchimp/commands.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:22:42.000000 rattail-mailchimp-0.1.2/rattail_mailchimp/db/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:22:42.000000 rattail-mailchimp-0.1.2/rattail_mailchimp/db/alembic/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:22:42.000000 rattail-mailchimp-0.1.2/rattail_mailchimp/db/alembic/versions/
--rw-r--r--   0 lance     (1000) lance     (1000)     2109 2021-11-08 18:08:40.000000 rattail-mailchimp-0.1.2/rattail_mailchimp/db/alembic/versions/805181d09df7_initial_tables.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2871 2023-02-22 00:13:43.000000 rattail-mailchimp-0.1.2/rattail_mailchimp/db/model.py
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2020-08-14 01:36:21.000000 rattail-mailchimp-0.1.2/rattail_mailchimp/db/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-02-22 01:21:31.000000 rattail-mailchimp-0.1.2/rattail_mailchimp/_version.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:22:42.000000 rattail-mailchimp-0.1.2/rattail_mailchimp/importing/
--rw-r--r--   0 lance     (1000) lance     (1000)     5888 2023-02-22 00:14:54.000000 rattail-mailchimp-0.1.2/rattail_mailchimp/importing/mailchimp.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2913 2023-02-21 03:54:56.000000 rattail-mailchimp-0.1.2/rattail_mailchimp/importing/model.py
--rw-r--r--   0 lance     (1000) lance     (1000)      987 2021-11-08 19:18:51.000000 rattail-mailchimp-0.1.2/rattail_mailchimp/importing/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1013 2021-11-08 19:20:40.000000 rattail-mailchimp-0.1.2/rattail_mailchimp/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1279 2021-11-08 17:32:39.000000 rattail-mailchimp-0.1.2/rattail_mailchimp/emails.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1155 2023-02-22 01:22:42.000000 rattail-mailchimp-0.1.2/PKG-INFO
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-13 22:49:44.000000 rattail-mailchimp-0.1.3/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-13 22:49:44.000000 rattail-mailchimp-0.1.3/rattail_mailchimp.egg-info/
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-05-13 22:49:44.000000 rattail-mailchimp-0.1.3/rattail_mailchimp.egg-info/dependency_links.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-05-13 22:49:43.000000 rattail-mailchimp-0.1.3/rattail_mailchimp.egg-info/not-zip-safe
+-rw-r--r--   0 lance     (1000) lance     (1000)      712 2023-05-13 22:49:44.000000 rattail-mailchimp-0.1.3/rattail_mailchimp.egg-info/SOURCES.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      145 2023-05-13 22:49:44.000000 rattail-mailchimp-0.1.3/rattail_mailchimp.egg-info/entry_points.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       19 2023-05-13 22:49:44.000000 rattail-mailchimp-0.1.3/rattail_mailchimp.egg-info/requires.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       18 2023-05-13 22:49:44.000000 rattail-mailchimp-0.1.3/rattail_mailchimp.egg-info/top_level.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)     1155 2023-05-13 22:49:44.000000 rattail-mailchimp-0.1.3/rattail_mailchimp.egg-info/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)       95 2021-11-08 02:57:23.000000 rattail-mailchimp-0.1.3/MANIFEST.in
+-rw-r--r--   0 lance     (1000) lance     (1000)     3887 2022-08-07 02:44:14.000000 rattail-mailchimp-0.1.3/setup.py
+-rw-r--r--   0 lance     (1000) lance     (1000)       38 2023-05-13 22:49:44.000000 rattail-mailchimp-0.1.3/setup.cfg
+-rw-r--r--   0 lance     (1000) lance     (1000)    35147 2017-07-07 15:32:34.000000 rattail-mailchimp-0.1.3/COPYING.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      347 2021-11-08 17:08:16.000000 rattail-mailchimp-0.1.3/README.rst
+-rw-r--r--   0 lance     (1000) lance     (1000)      622 2023-05-13 22:49:16.000000 rattail-mailchimp-0.1.3/CHANGELOG.md
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-13 22:49:44.000000 rattail-mailchimp-0.1.3/rattail_mailchimp/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1689 2021-11-08 19:18:10.000000 rattail-mailchimp-0.1.3/rattail_mailchimp/commands.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-13 22:49:44.000000 rattail-mailchimp-0.1.3/rattail_mailchimp/db/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-13 22:49:44.000000 rattail-mailchimp-0.1.3/rattail_mailchimp/db/alembic/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-13 22:49:44.000000 rattail-mailchimp-0.1.3/rattail_mailchimp/db/alembic/versions/
+-rw-r--r--   0 lance     (1000) lance     (1000)     2109 2021-11-08 18:08:40.000000 rattail-mailchimp-0.1.3/rattail_mailchimp/db/alembic/versions/805181d09df7_initial_tables.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2871 2023-02-22 00:13:43.000000 rattail-mailchimp-0.1.3/rattail_mailchimp/db/model.py
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2020-08-14 01:36:21.000000 rattail-mailchimp-0.1.3/rattail_mailchimp/db/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-05-13 22:49:19.000000 rattail-mailchimp-0.1.3/rattail_mailchimp/_version.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-13 22:49:44.000000 rattail-mailchimp-0.1.3/rattail_mailchimp/importing/
+-rw-r--r--   0 lance     (1000) lance     (1000)     5887 2023-05-05 06:54:07.000000 rattail-mailchimp-0.1.3/rattail_mailchimp/importing/mailchimp.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2913 2023-02-21 03:54:56.000000 rattail-mailchimp-0.1.3/rattail_mailchimp/importing/model.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      987 2021-11-08 19:18:51.000000 rattail-mailchimp-0.1.3/rattail_mailchimp/importing/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1013 2021-11-08 19:20:40.000000 rattail-mailchimp-0.1.3/rattail_mailchimp/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1279 2021-11-08 17:32:39.000000 rattail-mailchimp-0.1.3/rattail_mailchimp/emails.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1155 2023-05-13 22:49:44.000000 rattail-mailchimp-0.1.3/PKG-INFO
```

### Comparing `rattail-mailchimp-0.1.2/rattail_mailchimp.egg-info/SOURCES.txt` & `rattail-mailchimp-0.1.3/rattail_mailchimp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rattail-mailchimp-0.1.2/rattail_mailchimp.egg-info/PKG-INFO` & `rattail-mailchimp-0.1.3/rattail_mailchimp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattail-mailchimp
-Version: 0.1.2
+Version: 0.1.3
 Summary: Rattail Software Interfaces for MailChimp
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rattail-mailchimp-0.1.2/setup.py` & `rattail-mailchimp-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `rattail-mailchimp-0.1.2/COPYING.txt` & `rattail-mailchimp-0.1.3/COPYING.txt`

 * *Files identical despite different names*

### Comparing `rattail-mailchimp-0.1.2/CHANGELOG.md` & `rattail-mailchimp-0.1.3/CHANGELOG.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 
 # Changelog
 All notable changes to rattail-mailchimp will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
+## [0.1.3] - 2023-05-13
+### Changed
+- Avoid deprecated import for `OrderedDict`.
+
 ## [0.1.2] - 2023-02-21
 ### Changed
 - Tweak ORM relationship backrefs per SA 2.0 warnings.
 
 ## [0.1.1] - 2022-08-06
 ### Changed
 - Register email profiles provided by this pkg.
```

### Comparing `rattail-mailchimp-0.1.2/rattail_mailchimp/commands.py` & `rattail-mailchimp-0.1.3/rattail_mailchimp/commands.py`

 * *Files identical despite different names*

### Comparing `rattail-mailchimp-0.1.2/rattail_mailchimp/db/alembic/versions/805181d09df7_initial_tables.py` & `rattail-mailchimp-0.1.3/rattail_mailchimp/db/alembic/versions/805181d09df7_initial_tables.py`

 * *Files identical despite different names*

### Comparing `rattail-mailchimp-0.1.2/rattail_mailchimp/db/model.py` & `rattail-mailchimp-0.1.3/rattail_mailchimp/db/model.py`

 * *Files identical despite different names*

### Comparing `rattail-mailchimp-0.1.2/rattail_mailchimp/importing/mailchimp.py` & `rattail-mailchimp-0.1.3/rattail_mailchimp/importing/mailchimp.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 #
 ################################################################################
 """
 MailChimp -> Rattail "cache" data import
 """
 
 import datetime
+from collections import OrderedDict
 
 from mailchimp3 import MailChimp
 
 from rattail import importing
-from rattail.util import OrderedDict
 from rattail.time import localtime, make_utc
 from rattail_mailchimp import importing as mailchimp_importing
 
 
 class FromMailChimpToRattail(importing.ToRattailHandler):
     """
     Handler for MailChimp -> Rattail cache import
```

### Comparing `rattail-mailchimp-0.1.2/rattail_mailchimp/importing/model.py` & `rattail-mailchimp-0.1.3/rattail_mailchimp/importing/model.py`

 * *Files identical despite different names*

### Comparing `rattail-mailchimp-0.1.2/rattail_mailchimp/importing/__init__.py` & `rattail-mailchimp-0.1.3/rattail_mailchimp/importing/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-mailchimp-0.1.2/rattail_mailchimp/__init__.py` & `rattail-mailchimp-0.1.3/rattail_mailchimp/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-mailchimp-0.1.2/rattail_mailchimp/emails.py` & `rattail-mailchimp-0.1.3/rattail_mailchimp/emails.py`

 * *Files identical despite different names*

### Comparing `rattail-mailchimp-0.1.2/PKG-INFO` & `rattail-mailchimp-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattail-mailchimp
-Version: 0.1.2
+Version: 0.1.3
 Summary: Rattail Software Interfaces for MailChimp
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

