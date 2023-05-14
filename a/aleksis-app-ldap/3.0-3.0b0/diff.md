# Comparing `tmp/aleksis_app_ldap-3.0.tar.gz` & `tmp/aleksis_app_ldap-3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_app_ldap-3.0.tar", max compression
+gzip compressed data, was "aleksis_app_ldap-3.0b0.tar", max compression
```

## Comparing `aleksis_app_ldap-3.0.tar` & `aleksis_app_ldap-3.0b0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     2882 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/LICENCE.rst
--rw-r--r--   0        0        0     1280 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/README.rst
--rw-r--r--   0        0        0      208 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/aleksis/apps/ldap/__init__.py
--rw-r--r--   0        0        0      507 2023-05-14 18:39:14.061253 aleksis_app_ldap-3.0/aleksis/apps/ldap/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2147 2023-05-14 18:39:15.197307 aleksis_app_ldap-3.0/aleksis/apps/ldap/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0        0        0      725 2023-05-14 18:39:16.813384 aleksis_app_ldap-3.0/aleksis/apps/ldap/__pycache__/model_extensions.cpython-311.pyc
--rw-r--r--   0        0        0     9265 2023-05-14 18:39:16.901388 aleksis_app_ldap-3.0/aleksis/apps/ldap/__pycache__/preferences.cpython-311.pyc
--rw-r--r--   0        0        0     1150 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/aleksis/apps/ldap/apps.py
--rw-r--r--   0        0        0        0 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/aleksis/apps/ldap/locale/.keepdir
--rw-r--r--   0        0        0      463 2023-05-14 18:39:17.633423 aleksis_app_ldap-3.0/aleksis/apps/ldap/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3851 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/aleksis/apps/ldap/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3662 2023-05-14 18:39:17.673425 aleksis_app_ldap-3.0/aleksis/apps/ldap/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5991 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/aleksis/apps/ldap/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2023-05-14 18:39:17.697426 aleksis_app_ldap-3.0/aleksis/apps/ldap/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3767 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/aleksis/apps/ldap/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-05-14 18:39:17.641423 aleksis_app_ldap-3.0/aleksis/apps/ldap/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3721 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/aleksis/apps/ldap/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-05-14 18:39:17.709426 aleksis_app_ldap-3.0/aleksis/apps/ldap/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3721 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/aleksis/apps/ldap/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4830 2023-05-14 18:39:17.649423 aleksis_app_ldap-3.0/aleksis/apps/ldap/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     6422 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/aleksis/apps/ldap/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-05-14 18:39:17.677425 aleksis_app_ldap-3.0/aleksis/apps/ldap/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3721 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/aleksis/apps/ldap/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4818 2023-05-14 18:39:17.681425 aleksis_app_ldap-3.0/aleksis/apps/ldap/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     6404 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/aleksis/apps/ldap/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/aleksis/apps/ldap/management/commands/__init__.py
--rw-r--r--   0        0        0      197 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/aleksis/apps/ldap/management/commands/mass_ldap_import.py
--rw-r--r--   0        0        0     1152 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/aleksis/apps/ldap/migrations/0001_preferences.py
--rw-r--r--   0        0        0        0 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/aleksis/apps/ldap/migrations/__init__.py
--rw-r--r--   0        0        0      350 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/aleksis/apps/ldap/model_extensions.py
--rw-r--r--   0        0        0     5820 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/aleksis/apps/ldap/preferences.py
--rw-r--r--   0        0        0        0 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/aleksis/apps/ldap/static/.keepdir
--rw-r--r--   0        0        0      136 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/aleksis/apps/ldap/tasks.py
--rw-r--r--   0        0        0     1817 2023-05-14 18:39:15.201307 aleksis_app_ldap-3.0/aleksis/apps/ldap/util/__pycache__/ldap.cpython-311.pyc
--rw-r--r--   0        0        0     1916 2023-05-14 18:39:15.201307 aleksis_app_ldap-3.0/aleksis/apps/ldap/util/__pycache__/ldap_password.cpython-311.pyc
--rw-r--r--   0        0        0    27714 2023-05-14 18:39:15.217308 aleksis_app_ldap-3.0/aleksis/apps/ldap/util/__pycache__/ldap_sync.cpython-311.pyc
--rw-r--r--   0        0        0     1009 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/aleksis/apps/ldap/util/ldap.py
--rw-r--r--   0        0        0     1931 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/aleksis/apps/ldap/util/ldap_password.py
--rw-r--r--   0        0        0    19545 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/aleksis/apps/ldap/util/ldap_sync.py
--rw-r--r--   0        0        0      581 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/docs/Makefile
--rw-r--r--   0        0        0       82 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/docs/admin/00_index.rst
--rw-r--r--   0        0        0      641 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/docs/admin/01_intro.rst
--rw-r--r--   0        0        0     2773 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/docs/admin/10_configuring.rst
--rw-r--r--   0        0        0     1725 2023-05-14 18:12:52.854194 aleksis_app_ldap-3.0/docs/admin/20_manage_user_accounts.rst
--rw-r--r--   0        0        0     6395 2023-05-14 18:12:52.858194 aleksis_app_ldap-3.0/docs/conf.py
--rw-r--r--   0        0        0      522 2023-05-14 18:12:52.858194 aleksis_app_ldap-3.0/docs/index.rst
--rw-r--r--   0        0        0      787 2023-05-14 18:12:52.858194 aleksis_app_ldap-3.0/docs/make.bat
--rw-r--r--   0        0        0     1761 2023-05-14 18:27:07.406747 aleksis_app_ldap-3.0/pyproject.toml
--rw-r--r--   0        0        0     2563 2023-05-14 18:12:52.858194 aleksis_app_ldap-3.0/tox.ini
--rw-r--r--   0        0        0     2869 1970-01-01 00:00:00.000000 aleksis_app_ldap-3.0/setup.py
--rw-r--r--   0        0        0     2534 1970-01-01 00:00:00.000000 aleksis_app_ldap-3.0/PKG-INFO
+-rw-r--r--   0        0        0     2748 2023-03-01 22:22:36.322565 aleksis_app_ldap-3.0b0/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2023-03-01 22:22:36.322565 aleksis_app_ldap-3.0b0/LICENCE.rst
+-rw-r--r--   0        0        0     1280 2023-03-01 22:22:36.326565 aleksis_app_ldap-3.0b0/README.rst
+-rw-r--r--   0        0        0      208 2023-03-01 22:22:36.326565 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/__init__.py
+-rw-r--r--   0        0        0      507 2023-03-01 22:25:56.350159 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2147 2023-03-01 22:25:56.758159 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0        0        0      725 2023-03-01 22:25:57.530157 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/__pycache__/model_extensions.cpython-311.pyc
+-rw-r--r--   0        0        0     9265 2023-03-01 22:25:57.566157 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/__pycache__/preferences.cpython-311.pyc
+-rw-r--r--   0        0        0     1150 2023-03-01 22:22:36.326565 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/apps.py
+-rw-r--r--   0        0        0        0 2023-03-01 22:22:36.326565 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/locale/.keepdir
+-rw-r--r--   0        0        0      463 2023-03-01 22:25:57.854156 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3851 2023-03-01 22:22:36.326565 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3662 2023-03-01 22:25:57.866156 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5991 2023-03-01 22:22:36.326565 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2023-03-01 22:25:57.858156 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3767 2023-03-01 22:22:36.326565 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-03-01 22:25:57.862156 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3721 2023-03-01 22:22:36.326565 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-03-01 22:25:57.862156 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3721 2023-03-01 22:22:36.326565 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4830 2023-03-01 22:25:57.862156 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6422 2023-03-01 22:22:36.326565 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-03-01 22:25:57.862156 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3721 2023-03-01 22:22:36.326565 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4818 2023-03-01 22:25:57.862156 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6404 2023-03-01 22:22:36.326565 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-03-01 22:22:36.326565 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/management/commands/__init__.py
+-rw-r--r--   0        0        0      197 2023-03-01 22:22:36.326565 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/management/commands/mass_ldap_import.py
+-rw-r--r--   0        0        0     1152 2023-03-01 22:22:36.326565 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/migrations/0001_preferences.py
+-rw-r--r--   0        0        0        0 2023-03-01 22:22:36.326565 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/migrations/__init__.py
+-rw-r--r--   0        0        0      350 2023-03-01 22:22:36.326565 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/model_extensions.py
+-rw-r--r--   0        0        0     5820 2023-03-01 22:22:36.326565 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/preferences.py
+-rw-r--r--   0        0        0        0 2023-03-01 22:22:36.326565 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/static/.keepdir
+-rw-r--r--   0        0        0      136 2023-03-01 22:22:36.326565 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/tasks.py
+-rw-r--r--   0        0        0     1817 2023-03-01 22:25:56.762158 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/util/__pycache__/ldap.cpython-311.pyc
+-rw-r--r--   0        0        0     1916 2023-03-01 22:25:56.762158 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/util/__pycache__/ldap_password.cpython-311.pyc
+-rw-r--r--   0        0        0    27714 2023-03-01 22:25:56.770158 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/util/__pycache__/ldap_sync.cpython-311.pyc
+-rw-r--r--   0        0        0     1009 2023-03-01 22:22:36.326565 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/util/ldap.py
+-rw-r--r--   0        0        0     1931 2023-03-01 22:22:36.326565 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/util/ldap_password.py
+-rw-r--r--   0        0        0    19545 2023-03-01 22:22:36.326565 aleksis_app_ldap-3.0b0/aleksis/apps/ldap/util/ldap_sync.py
+-rw-r--r--   0        0        0      581 2023-03-01 22:22:36.330565 aleksis_app_ldap-3.0b0/docs/Makefile
+-rw-r--r--   0        0        0       82 2023-03-01 22:22:36.330565 aleksis_app_ldap-3.0b0/docs/admin/00_index.rst
+-rw-r--r--   0        0        0      641 2023-03-01 22:22:36.330565 aleksis_app_ldap-3.0b0/docs/admin/01_intro.rst
+-rw-r--r--   0        0        0     2773 2023-03-01 22:22:36.330565 aleksis_app_ldap-3.0b0/docs/admin/10_configuring.rst
+-rw-r--r--   0        0        0     1725 2023-03-01 22:22:36.330565 aleksis_app_ldap-3.0b0/docs/admin/20_manage_user_accounts.rst
+-rw-r--r--   0        0        0     6397 2023-03-01 22:22:36.330565 aleksis_app_ldap-3.0b0/docs/conf.py
+-rw-r--r--   0        0        0      522 2023-03-01 22:22:36.330565 aleksis_app_ldap-3.0b0/docs/index.rst
+-rw-r--r--   0        0        0      787 2023-03-01 22:22:36.330565 aleksis_app_ldap-3.0b0/docs/make.bat
+-rw-r--r--   0        0        0     1765 2023-03-01 22:24:39.390315 aleksis_app_ldap-3.0b0/pyproject.toml
+-rw-r--r--   0        0        0     2563 2023-03-01 22:22:36.330565 aleksis_app_ldap-3.0b0/tox.ini
+-rw-r--r--   0        0        0     2873 1970-01-01 00:00:00.000000 aleksis_app_ldap-3.0b0/setup.py
+-rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 aleksis_app_ldap-3.0b0/PKG-INFO
```

### Comparing `aleksis_app_ldap-3.0/CHANGELOG.rst` & `aleksis_app_ldap-3.0b0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,16 @@
 =========
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
-`3.0`_ - 2023-05-15
--------------------
-
-Nothing changed.
-
-`3.0b0`_ - 2023-02-22
----------------------
+`3.0b0` - 2023-02-22
+--------------------
 
 This version requires AlekSIS-Core 3.0. It is incompatible with any previous
 version.
 
 `2.2`_ - 2022-06-23
 -------------------
 
@@ -124,8 +119,7 @@
 .. _2.0rc1: https://edugit.org/AlekSIS/Official/AlekSIS-App-LDAP/-/tags/2.0rc1
 .. _2.0rc2: https://edugit.org/AlekSIS/Official/AlekSIS-App-LDAP/-/tags/2.0rc2
 .. _2.0: https://edugit.org/AlekSIS/Official/AlekSIS-App-LDAP/-/tags/2.0
 .. _2.0.1: https://edugit.org/AlekSIS/Official/AlekSIS-App-LDAP/-/tags/2.0.1
 .. _2.1: https://edugit.org/AlekSIS/Official/AlekSIS-App-LDAP/-/tags/2.1
 .. _2.2: https://edugit.org/AlekSIS/Official/AlekSIS-App-LDAP/-/tags/2.2
 .. _3.0b0: https://edugit.org/AlekSIS/Official/AlekSIS-App-LDAP/-/tags/3.0b0
-.. _3.0: https://edugit.org/AlekSIS/Official/AlekSIS-App-LDAP/-/tags/3.0
```

### Comparing `aleksis_app_ldap-3.0/LICENCE.rst` & `aleksis_app_ldap-3.0b0/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_ldap-3.0/README.rst` & `aleksis_app_ldap-3.0b0/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_ldap-3.0/aleksis/apps/ldap/__pycache__/apps.cpython-311.pyc` & `aleksis_app_ldap-3.0b0/aleksis/apps/ldap/__pycache__/apps.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xa4246164 (Sun May 14 18:12:52 2023 UTC)
+moddate:  0x2cd0ff63 (Wed Mar  1 22:22:36 2023 UTC)
 files sz: 1150
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_app_ldap-3.0/aleksis/apps/ldap/__pycache__/model_extensions.cpython-311.pyc` & `aleksis_app_ldap-3.0b0/aleksis/apps/ldap/__pycache__/model_extensions.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xa4246164 (Sun May 14 18:12:52 2023 UTC)
+moddate:  0x2cd0ff63 (Wed Mar  1 22:22:36 2023 UTC)
 files sz: 350
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `aleksis_app_ldap-3.0/aleksis/apps/ldap/__pycache__/preferences.cpython-311.pyc` & `aleksis_app_ldap-3.0b0/aleksis/apps/ldap/__pycache__/preferences.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xa4246164 (Sun May 14 18:12:52 2023 UTC)
+moddate:  0x2cd0ff63 (Wed Mar  1 22:22:36 2023 UTC)
 files sz: 5820
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_app_ldap-3.0/aleksis/apps/ldap/apps.py` & `aleksis_app_ldap-3.0b0/aleksis/apps/ldap/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_ldap-3.0/aleksis/apps/ldap/locale/ar/LC_MESSAGES/django.po` & `aleksis_app_ldap-3.0b0/aleksis/apps/ldap/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_ldap-3.0/aleksis/apps/ldap/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_app_ldap-3.0b0/aleksis/apps/ldap/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_ldap-3.0/aleksis/apps/ldap/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_app_ldap-3.0b0/aleksis/apps/ldap/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_ldap-3.0/aleksis/apps/ldap/locale/fr/LC_MESSAGES/django.po` & `aleksis_app_ldap-3.0b0/aleksis/apps/ldap/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_ldap-3.0/aleksis/apps/ldap/locale/la/LC_MESSAGES/django.po` & `aleksis_app_ldap-3.0b0/aleksis/apps/ldap/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_ldap-3.0/aleksis/apps/ldap/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_app_ldap-3.0b0/aleksis/apps/ldap/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_ldap-3.0/aleksis/apps/ldap/locale/ru/LC_MESSAGES/django.mo` & `aleksis_app_ldap-3.0b0/aleksis/apps/ldap/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_ldap-3.0/aleksis/apps/ldap/locale/ru/LC_MESSAGES/django.po` & `aleksis_app_ldap-3.0b0/aleksis/apps/ldap/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_ldap-3.0/aleksis/apps/ldap/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_app_ldap-3.0b0/aleksis/apps/ldap/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_ldap-3.0/aleksis/apps/ldap/locale/uk/LC_MESSAGES/django.mo` & `aleksis_app_ldap-3.0b0/aleksis/apps/ldap/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_ldap-3.0/aleksis/apps/ldap/locale/uk/LC_MESSAGES/django.po` & `aleksis_app_ldap-3.0b0/aleksis/apps/ldap/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_ldap-3.0/aleksis/apps/ldap/migrations/0001_preferences.py` & `aleksis_app_ldap-3.0b0/aleksis/apps/ldap/migrations/0001_preferences.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_ldap-3.0/aleksis/apps/ldap/preferences.py` & `aleksis_app_ldap-3.0b0/aleksis/apps/ldap/preferences.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_ldap-3.0/aleksis/apps/ldap/util/__pycache__/ldap.cpython-311.pyc` & `aleksis_app_ldap-3.0b0/aleksis/apps/ldap/util/__pycache__/ldap.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xa4246164 (Sun May 14 18:12:52 2023 UTC)
+moddate:  0x2cd0ff63 (Wed Mar  1 22:22:36 2023 UTC)
 files sz: 1009
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `aleksis_app_ldap-3.0/aleksis/apps/ldap/util/__pycache__/ldap_password.cpython-311.pyc` & `aleksis_app_ldap-3.0b0/aleksis/apps/ldap/util/__pycache__/ldap_password.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xa4246164 (Sun May 14 18:12:52 2023 UTC)
+moddate:  0x2cd0ff63 (Wed Mar  1 22:22:36 2023 UTC)
 files sz: 1931
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `aleksis_app_ldap-3.0/aleksis/apps/ldap/util/__pycache__/ldap_sync.cpython-311.pyc` & `aleksis_app_ldap-3.0b0/aleksis/apps/ldap/util/__pycache__/ldap_sync.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xa4246164 (Sun May 14 18:12:52 2023 UTC)
+moddate:  0x2cd0ff63 (Wed Mar  1 22:22:36 2023 UTC)
 files sz: 19545
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `aleksis_app_ldap-3.0/aleksis/apps/ldap/util/ldap.py` & `aleksis_app_ldap-3.0b0/aleksis/apps/ldap/util/ldap.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_ldap-3.0/aleksis/apps/ldap/util/ldap_password.py` & `aleksis_app_ldap-3.0b0/aleksis/apps/ldap/util/ldap_password.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_ldap-3.0/aleksis/apps/ldap/util/ldap_sync.py` & `aleksis_app_ldap-3.0b0/aleksis/apps/ldap/util/ldap_sync.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_ldap-3.0/docs/Makefile` & `aleksis_app_ldap-3.0b0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aleksis_app_ldap-3.0/docs/admin/01_intro.rst` & `aleksis_app_ldap-3.0b0/docs/admin/01_intro.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_ldap-3.0/docs/admin/10_configuring.rst` & `aleksis_app_ldap-3.0b0/docs/admin/10_configuring.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_ldap-3.0/docs/admin/20_manage_user_accounts.rst` & `aleksis_app_ldap-3.0b0/docs/admin/20_manage_user_accounts.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_ldap-3.0/docs/conf.py` & `aleksis_app_ldap-3.0b0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 project = "AlekSIS-App-LDAP"
 copyright = "2020-2022 The AlekSIS team"
 author = "The AlekSIS Team"
 
 # The short X.Y version
 version = "3.0"
 # The full version, including alpha/beta/rc tags
-release = "3.0"
+release = "3.0b0"
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `aleksis_app_ldap-3.0/docs/index.rst` & `aleksis_app_ldap-3.0b0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_ldap-3.0/docs/make.bat` & `aleksis_app_ldap-3.0b0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aleksis_app_ldap-3.0/pyproject.toml` & `aleksis_app_ldap-3.0b0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-App-LDAP"
-version = "3.0"
+version = "3.0b0"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = [
     { path = "aleksis/**/*.mo", format = ["sdist", "wheel"] },
     { path = "*.rst", format = "sdist" },
@@ -36,15 +36,15 @@
 url = "https://edugit.org/api/v4/projects/461/packages/pypi/simple"
 secondary = true
 
 [tool.poetry.dependencies]
 python = "^3.9"
 django-ldapdb = "^1.4.0"
 tqdm = "^4.44.1"
-aleksis-core = {version = "^3.0", extras = ["ldap"]}
+aleksis-core = {version = "^3.0b0", extras = ["ldap"]}
 python-magic = "^0.4.22"
 
 [tool.poetry.dev-dependencies]
 aleksis-builddeps = "*"
 
 [tool.poetry.plugins."aleksis.app"]
 ldap = "aleksis.apps.ldap.apps:LDAPConfig"
```

### Comparing `aleksis_app_ldap-3.0/tox.ini` & `aleksis_app_ldap-3.0b0/tox.ini`

 * *Files identical despite different names*

### Comparing `aleksis_app_ldap-3.0/setup.py` & `aleksis_app_ldap-3.0b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,25 +18,25 @@
                        'locale/nb_NO/LC_MESSAGES/*',
                        'locale/ru/LC_MESSAGES/*',
                        'locale/tr_TR/LC_MESSAGES/*',
                        'locale/uk/LC_MESSAGES/*',
                        'static/*']}
 
 install_requires = \
-['aleksis-core[ldap]>=3.0,<4.0',
+['aleksis-core[ldap]>=3.0b0,<4.0',
  'django-ldapdb>=1.4.0,<2.0.0',
  'python-magic>=0.4.22,<0.5.0',
  'tqdm>=4.44.1,<5.0.0']
 
 entry_points = \
 {'aleksis.app': ['ldap = aleksis.apps.ldap.apps:LDAPConfig']}
 
 setup_kwargs = {
     'name': 'aleksis-app-ldap',
-    'version': '3.0',
+    'version': '3.0b0',
     'description': 'AlekSIS (School Information System)\u200a—\u200aApp LDAP (General LDAP import/export)',
     'long_description': 'AlekSIS (School Information System)\u200a—\u200aApp LDAP (General LDAP import/export)\n==================================================================================================\n\nAlekSIS\n-------\n\nThis is an application for use with the `AlekSIS®`_ platform.\n\nFeatures\n--------\n\n* Configurable sync strategies\n* Management commands for ldap import\n* Mass import of users and groups\n* Sync LDAP users and groups on login\n\nLicence\n-------\n\n::\n\n  Copyright © 2020, 2021, 2022 Dominik George <dominik.george@teckids.org>\n  Copyright © 2020 Tom Teichler <tom.teichler@teckids.org>\n\n  Licenced under the EUPL, version 1.2 or later, by Teckids e.V. (Bonn, Germany).\n\nPlease see the LICENCE.rst file accompanying this distribution for the\nfull licence text or on the `European Union Public Licence`_ website\nhttps://joinup.ec.europa.eu/collection/eupl/guidelines-users-and-developers\n(including all other official language versions).\n\nTrademark\n---------\n\nAlekSIS® is a registered trademark of the AlekSIS open source project, represented\nby Teckids e.V. Please refer to the `trademark policy`_ for hints on using the trademark\nAlekSIS®.\n\n.. _AlekSIS®: https://aleksis.org/\n.. _European Union Public Licence: https://eupl.eu/\n.. _trademark policy: https://aleksis.org/pages/about\n',
     'author': 'Tom Teichler',
     'author_email': 'tom.teichler@teckids.org',
     'maintainer': 'Jonathan Weth',
     'maintainer_email': 'wethjo@katharineum.de',
     'url': 'https://aleksis.org/',
```

### Comparing `aleksis_app_ldap-3.0/PKG-INFO` & `aleksis_app_ldap-3.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleksis-app-ldap
-Version: 3.0
+Version: 3.0b0
 Summary: AlekSIS (School Information System) — App LDAP (General LDAP import/export)
 Home-page: https://aleksis.org/
 License: EUPL-1.2-or-later
 Keywords: SIS,education,school,ldap,users
 Author: Tom Teichler
 Author-email: tom.teichler@teckids.org
 Maintainer: Jonathan Weth
@@ -17,15 +17,15 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
 Classifier: Typing :: Typed
-Requires-Dist: aleksis-core[ldap] (>=3.0,<4.0)
+Requires-Dist: aleksis-core[ldap] (>=3.0b0,<4.0)
 Requires-Dist: django-ldapdb (>=1.4.0,<2.0.0)
 Requires-Dist: python-magic (>=0.4.22,<0.5.0)
 Requires-Dist: tqdm (>=4.44.1,<5.0.0)
 Project-URL: Documentation, https://aleksis.org/AlekSIS/docs/html/
 Project-URL: Repository, https://edugit.org/AlekSIS/official/AlekSIS-App-LDAP
 Description-Content-Type: text/x-rst
```

