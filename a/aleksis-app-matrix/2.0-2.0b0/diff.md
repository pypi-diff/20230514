# Comparing `tmp/aleksis_app_matrix-2.0.tar.gz` & `tmp/aleksis_app_matrix-2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_app_matrix-2.0.tar", max compression
+gzip compressed data, was "aleksis_app_matrix-2.0b0.tar", max compression
```

## Comparing `aleksis_app_matrix-2.0.tar` & `aleksis_app_matrix-2.0b0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1064 2023-05-14 18:41:42.324291 aleksis_app_matrix-2.0/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2023-05-14 18:41:42.324291 aleksis_app_matrix-2.0/LICENCE.rst
--rw-r--r--   0        0        0      840 2023-05-14 18:41:42.324291 aleksis_app_matrix-2.0/README.rst
--rw-r--r--   0        0        0      152 2023-05-14 18:41:42.324291 aleksis_app_matrix-2.0/aleksis/apps/matrix/__init__.py
--rw-r--r--   0        0        0      444 2023-05-14 18:44:58.105584 aleksis_app_matrix-2.0/aleksis/apps/matrix/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1870 2023-05-14 18:44:58.701612 aleksis_app_matrix-2.0/aleksis/apps/matrix/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0        0        0     2878 2023-05-14 18:44:59.657657 aleksis_app_matrix-2.0/aleksis/apps/matrix/__pycache__/model_extensions.cpython-311.pyc
--rw-r--r--   0        0        0    21116 2023-05-14 18:44:59.545652 aleksis_app_matrix-2.0/aleksis/apps/matrix/__pycache__/models.cpython-311.pyc
--rw-r--r--   0        0        0     4700 2023-05-14 18:44:59.693659 aleksis_app_matrix-2.0/aleksis/apps/matrix/__pycache__/preferences.cpython-311.pyc
--rw-r--r--   0        0        0     1342 2023-05-14 18:44:59.617655 aleksis_app_matrix-2.0/aleksis/apps/matrix/__pycache__/rules.cpython-311.pyc
--rw-r--r--   0        0        0     2589 2023-05-14 18:44:59.829665 aleksis_app_matrix-2.0/aleksis/apps/matrix/__pycache__/signals.cpython-311.pyc
--rw-r--r--   0        0        0     2331 2023-05-14 18:44:59.657657 aleksis_app_matrix-2.0/aleksis/apps/matrix/__pycache__/tasks.cpython-311.pyc
--rw-r--r--   0        0        0     1076 2023-05-14 18:41:42.328291 aleksis_app_matrix-2.0/aleksis/apps/matrix/apps.py
--rw-r--r--   0        0        0      149 2023-05-14 18:41:42.328291 aleksis_app_matrix-2.0/aleksis/apps/matrix/filters.py
--rw-r--r--   0        0        0      544 2023-05-14 18:41:42.328291 aleksis_app_matrix-2.0/aleksis/apps/matrix/forms.py
--rw-r--r--   0        0        0      752 2023-05-14 18:41:42.328291 aleksis_app_matrix-2.0/aleksis/apps/matrix/frontend/index.js
--rw-r--r--   0        0        0      112 2023-05-14 18:41:42.328291 aleksis_app_matrix-2.0/aleksis/apps/matrix/frontend/messages/de.json
--rw-r--r--   0        0        0      110 2023-05-14 18:41:42.328291 aleksis_app_matrix-2.0/aleksis/apps/matrix/frontend/messages/en.json
--rw-r--r--   0        0        0      124 2023-05-14 18:41:42.328291 aleksis_app_matrix-2.0/aleksis/apps/matrix/frontend/messages/ru.json
--rw-r--r--   0        0        0      124 2023-05-14 18:41:42.332291 aleksis_app_matrix-2.0/aleksis/apps/matrix/frontend/messages/uk.json
--rw-r--r--   0        0        0        0 2023-05-14 18:41:42.332291 aleksis_app_matrix-2.0/aleksis/apps/matrix/locale/.keepdir
--rw-r--r--   0        0        0      463 2023-05-14 18:44:59.861667 aleksis_app_matrix-2.0/aleksis/apps/matrix/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4287 2023-05-14 18:41:42.332291 aleksis_app_matrix-2.0/aleksis/apps/matrix/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3684 2023-05-14 18:44:59.877668 aleksis_app_matrix-2.0/aleksis/apps/matrix/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5579 2023-05-14 18:41:42.348292 aleksis_app_matrix-2.0/aleksis/apps/matrix/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2023-05-14 18:44:59.869667 aleksis_app_matrix-2.0/aleksis/apps/matrix/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4203 2023-05-14 18:41:42.348292 aleksis_app_matrix-2.0/aleksis/apps/matrix/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-05-14 18:44:59.873667 aleksis_app_matrix-2.0/aleksis/apps/matrix/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4157 2023-05-14 18:41:42.348292 aleksis_app_matrix-2.0/aleksis/apps/matrix/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-05-14 18:44:59.865667 aleksis_app_matrix-2.0/aleksis/apps/matrix/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4157 2023-05-14 18:41:42.348292 aleksis_app_matrix-2.0/aleksis/apps/matrix/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4926 2023-05-14 18:44:59.881668 aleksis_app_matrix-2.0/aleksis/apps/matrix/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     6833 2023-05-14 18:41:42.348292 aleksis_app_matrix-2.0/aleksis/apps/matrix/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-05-14 18:44:59.877668 aleksis_app_matrix-2.0/aleksis/apps/matrix/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4157 2023-05-14 18:41:42.348292 aleksis_app_matrix-2.0/aleksis/apps/matrix/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4863 2023-05-14 18:44:59.861667 aleksis_app_matrix-2.0/aleksis/apps/matrix/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     6764 2023-05-14 18:41:42.348292 aleksis_app_matrix-2.0/aleksis/apps/matrix/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3608 2023-05-14 18:41:42.348292 aleksis_app_matrix-2.0/aleksis/apps/matrix/migrations/0001_initial.py
--rw-r--r--   0        0        0      509 2023-05-14 18:41:42.348292 aleksis_app_matrix-2.0/aleksis/apps/matrix/migrations/0002_drop_onetoone.py
--rw-r--r--   0        0        0        0 2023-05-14 18:41:42.348292 aleksis_app_matrix-2.0/aleksis/apps/matrix/migrations/__init__.py
--rw-r--r--   0        0        0     1330 2023-05-14 18:41:42.348292 aleksis_app_matrix-2.0/aleksis/apps/matrix/model_extensions.py
--rw-r--r--   0        0        0    12583 2023-05-14 18:41:42.348292 aleksis_app_matrix-2.0/aleksis/apps/matrix/models.py
--rw-r--r--   0        0        0     2742 2023-05-14 18:41:42.348292 aleksis_app_matrix-2.0/aleksis/apps/matrix/preferences.py
--rw-r--r--   0        0        0     1012 2023-05-14 18:41:42.348292 aleksis_app_matrix-2.0/aleksis/apps/matrix/rules.py
--rw-r--r--   0        0        0     1333 2023-05-14 18:41:42.348292 aleksis_app_matrix-2.0/aleksis/apps/matrix/signals.py
--rw-r--r--   0        0        0      387 2023-05-14 18:41:42.348292 aleksis_app_matrix-2.0/aleksis/apps/matrix/tables.py
--rw-r--r--   0        0        0      893 2023-05-14 18:41:42.348292 aleksis_app_matrix-2.0/aleksis/apps/matrix/tasks.py
--rw-r--r--   0        0        0     2211 2023-05-14 18:41:42.348292 aleksis_app_matrix-2.0/aleksis/apps/matrix/templates/matrix/room/list.html
--rw-r--r--   0        0        0     1397 2023-05-14 18:41:42.348292 aleksis_app_matrix-2.0/aleksis/apps/matrix/tests/conftest.py
--rw-r--r--   0        0        0      852 2023-05-14 18:41:42.348292 aleksis_app_matrix-2.0/aleksis/apps/matrix/tests/synapse/homeserver.yaml
--rw-r--r--   0        0        0      932 2023-05-14 18:41:42.348292 aleksis_app_matrix-2.0/aleksis/apps/matrix/tests/synapse/matrix.aleksis.example.org.log.config
--rw-r--r--   0        0        0       59 2023-05-14 18:41:42.348292 aleksis_app_matrix-2.0/aleksis/apps/matrix/tests/synapse/matrix.aleksis.example.org.signing.key
--rw-r--r--   0        0        0    21535 2023-05-14 18:41:42.352292 aleksis_app_matrix-2.0/aleksis/apps/matrix/tests/test_matrix.py
--rw-r--r--   0        0        0      146 2023-05-14 18:41:42.352292 aleksis_app_matrix-2.0/aleksis/apps/matrix/urls.py
--rw-r--r--   0        0        0     2644 2023-05-14 18:44:59.549652 aleksis_app_matrix-2.0/aleksis/apps/matrix/util/__pycache__/matrix.cpython-311.pyc
--rw-r--r--   0        0        0     1367 2023-05-14 18:41:42.352292 aleksis_app_matrix-2.0/aleksis/apps/matrix/util/matrix.py
--rw-r--r--   0        0        0     1669 2023-05-14 18:41:42.352292 aleksis_app_matrix-2.0/aleksis/apps/matrix/views.py
--rw-r--r--   0        0        0     1378 2023-05-14 18:42:19.730066 aleksis_app_matrix-2.0/pyproject.toml
--rw-r--r--   0        0        0     2495 1970-01-01 00:00:00.000000 aleksis_app_matrix-2.0/setup.py
--rw-r--r--   0        0        0     1855 1970-01-01 00:00:00.000000 aleksis_app_matrix-2.0/PKG-INFO
+-rw-r--r--   0        0        0      789 2023-03-02 14:05:46.676024 aleksis_app_matrix-2.0b0/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2023-03-02 14:05:46.676024 aleksis_app_matrix-2.0b0/LICENCE.rst
+-rw-r--r--   0        0        0      840 2023-03-02 14:05:46.676024 aleksis_app_matrix-2.0b0/README.rst
+-rw-r--r--   0        0        0      152 2023-03-02 14:05:46.676024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/__init__.py
+-rw-r--r--   0        0        0      444 2023-03-02 14:09:13.991630 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1870 2023-03-02 14:09:14.423629 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0        0        0     2878 2023-03-02 14:09:15.183627 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/__pycache__/model_extensions.cpython-311.pyc
+-rw-r--r--   0        0        0    21116 2023-03-02 14:09:15.103628 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0        0        0     4700 2023-03-02 14:09:15.215627 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/__pycache__/preferences.cpython-311.pyc
+-rw-r--r--   0        0        0     1342 2023-03-02 14:09:15.159627 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/__pycache__/rules.cpython-311.pyc
+-rw-r--r--   0        0        0     2589 2023-03-02 14:09:15.331627 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/__pycache__/signals.cpython-311.pyc
+-rw-r--r--   0        0        0     2331 2023-03-02 14:09:15.187627 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/__pycache__/tasks.cpython-311.pyc
+-rw-r--r--   0        0        0     1076 2023-03-02 14:05:46.676024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/apps.py
+-rw-r--r--   0        0        0      149 2023-03-02 14:05:46.676024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/filters.py
+-rw-r--r--   0        0        0      544 2023-03-02 14:05:46.676024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/forms.py
+-rw-r--r--   0        0        0      704 2023-03-02 14:05:46.676024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/frontend/index.js
+-rw-r--r--   0        0        0      112 2023-03-02 14:05:46.676024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/frontend/messages/de.json
+-rw-r--r--   0        0        0      110 2023-03-02 14:05:46.676024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/frontend/messages/en.json
+-rw-r--r--   0        0        0      124 2023-03-02 14:05:46.676024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/frontend/messages/ru.json
+-rw-r--r--   0        0        0      124 2023-03-02 14:05:46.676024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/frontend/messages/uk.json
+-rw-r--r--   0        0        0        0 2023-03-02 14:05:46.680024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/locale/.keepdir
+-rw-r--r--   0        0        0      463 2023-03-02 14:09:15.363627 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4287 2023-03-02 14:05:46.680024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3684 2023-03-02 14:09:15.363627 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5579 2023-03-02 14:05:46.680024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2023-03-02 14:09:15.359627 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4203 2023-03-02 14:05:46.680024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-03-02 14:09:15.371627 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4157 2023-03-02 14:05:46.680024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-03-02 14:09:15.363627 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4157 2023-03-02 14:05:46.680024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4926 2023-03-02 14:09:15.363627 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6833 2023-03-02 14:05:46.680024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-03-02 14:09:15.371627 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4157 2023-03-02 14:05:46.680024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4863 2023-03-02 14:09:15.363627 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6764 2023-03-02 14:05:46.680024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      930 2023-03-02 14:05:46.680024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/menus.py
+-rw-r--r--   0        0        0     3608 2023-03-02 14:05:46.680024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/migrations/0001_initial.py
+-rw-r--r--   0        0        0      509 2023-03-02 14:05:46.680024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/migrations/0002_drop_onetoone.py
+-rw-r--r--   0        0        0        0 2023-03-02 14:05:46.680024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/migrations/__init__.py
+-rw-r--r--   0        0        0     1330 2023-03-02 14:05:46.680024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/model_extensions.py
+-rw-r--r--   0        0        0    12583 2023-03-02 14:05:46.680024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/models.py
+-rw-r--r--   0        0        0     2742 2023-03-02 14:05:46.680024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/preferences.py
+-rw-r--r--   0        0        0     1012 2023-03-02 14:05:46.680024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/rules.py
+-rw-r--r--   0        0        0     1333 2023-03-02 14:05:46.680024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/signals.py
+-rw-r--r--   0        0        0      387 2023-03-02 14:05:46.680024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/tables.py
+-rw-r--r--   0        0        0      893 2023-03-02 14:05:46.680024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/tasks.py
+-rw-r--r--   0        0        0     2211 2023-03-02 14:05:46.680024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/templates/matrix/room/list.html
+-rw-r--r--   0        0        0     1397 2023-03-02 14:05:46.684024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/tests/conftest.py
+-rw-r--r--   0        0        0      852 2023-03-02 14:05:46.684024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/tests/synapse/homeserver.yaml
+-rw-r--r--   0        0        0      932 2023-03-02 14:05:46.684024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/tests/synapse/matrix.aleksis.example.org.log.config
+-rw-r--r--   0        0        0       59 2023-03-02 14:05:46.684024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/tests/synapse/matrix.aleksis.example.org.signing.key
+-rw-r--r--   0        0        0    21535 2023-03-02 14:05:46.684024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/tests/test_matrix.py
+-rw-r--r--   0        0        0     2644 2023-03-02 14:09:15.107627 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/util/__pycache__/matrix.cpython-311.pyc
+-rw-r--r--   0        0        0     1367 2023-03-02 14:05:46.684024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/util/matrix.py
+-rw-r--r--   0        0        0     1669 2023-03-02 14:05:46.684024 aleksis_app_matrix-2.0b0/aleksis/apps/matrix/views.py
+-rw-r--r--   0        0        0     1382 2023-03-02 14:07:48.883792 aleksis_app_matrix-2.0b0/pyproject.toml
+-rw-r--r--   0        0        0     2499 1970-01-01 00:00:00.000000 aleksis_app_matrix-2.0b0/setup.py
+-rw-r--r--   0        0        0     1859 1970-01-01 00:00:00.000000 aleksis_app_matrix-2.0b0/PKG-INFO
```

### Comparing `aleksis_app_matrix-2.0/CHANGELOG.rst` & `aleksis_app_matrix-2.0b0/CHANGELOG.rst`

 * *Files 13% similar despite different names*

```diff
@@ -2,25 +2,17 @@
 =========
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
-`2.0`_ - 2023-05-14
--------------------
-
-Fixed
-~~~~~
-
-* The Matrix groups and rooms threw a 404 error.
-* The Matrix parent menu point was displayed even though the user had no permission to see it.
 
-`2.0b0`_ - 2023-02-23
----------------------
+`2.0b0` - 2023-02-23
+--------------------
 
 This version requires AlekSIS-Core 3.0. It is incompatible with any previous
 version.
 
 Removed
 ~~~~~~~
 
@@ -40,8 +32,7 @@
 * Initial release.
 
 .. _Keep a Changelog: https://keepachangelog.com/en/1.0.0/
 .. _Semantic Versioning: https://semver.org/spec/v2.0.0.html
 
 .. _1.0: https://edugit.org/AlekSIS/Official/AlekSIS-App-Matrix/-/tags/1.0
 .. _2.0b0: https://edugit.org/AlekSIS/Official/AlekSIS-App-Matrix/-/tags/2.0b0
-.. _2.0: https://edugit.org/AlekSIS/Official/AlekSIS-App-Matrix/-/tags/2.0
```

### Comparing `aleksis_app_matrix-2.0/LICENCE.rst` & `aleksis_app_matrix-2.0b0/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_matrix-2.0/README.rst` & `aleksis_app_matrix-2.0b0/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/__pycache__/apps.cpython-311.pyc` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/__pycache__/apps.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x662b6164 (Sun May 14 18:41:42 2023 UTC)
+moddate:  0x3aad0064 (Thu Mar  2 14:05:46 2023 UTC)
 files sz: 1076
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/__pycache__/model_extensions.cpython-311.pyc` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/__pycache__/model_extensions.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x662b6164 (Sun May 14 18:41:42 2023 UTC)
+moddate:  0x3aad0064 (Thu Mar  2 14:05:46 2023 UTC)
 files sz: 1330
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
```

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/__pycache__/models.cpython-311.pyc` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/__pycache__/models.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x662b6164 (Sun May 14 18:41:42 2023 UTC)
+moddate:  0x3aad0064 (Thu Mar  2 14:05:46 2023 UTC)
 files sz: 12583
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/__pycache__/preferences.cpython-311.pyc` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/__pycache__/preferences.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x662b6164 (Sun May 14 18:41:42 2023 UTC)
+moddate:  0x3aad0064 (Thu Mar  2 14:05:46 2023 UTC)
 files sz: 2742
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/__pycache__/rules.cpython-311.pyc` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/__pycache__/rules.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x662b6164 (Sun May 14 18:41:42 2023 UTC)
+moddate:  0x3aad0064 (Thu Mar  2 14:05:46 2023 UTC)
 files sz: 1012
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/__pycache__/signals.cpython-311.pyc` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/__pycache__/signals.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x662b6164 (Sun May 14 18:41:42 2023 UTC)
+moddate:  0x3aad0064 (Thu Mar  2 14:05:46 2023 UTC)
 files sz: 1333
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/__pycache__/tasks.cpython-311.pyc` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/__pycache__/tasks.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x662b6164 (Sun May 14 18:41:42 2023 UTC)
+moddate:  0x3aad0064 (Thu Mar  2 14:05:46 2023 UTC)
 files sz: 893
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/apps.py` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/forms.py` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/frontend/index.js` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/frontend/index.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,12 @@
 export default {
     meta: {
         inMenu: true,
         titleKey: "matrix.menu_title",
         icon: "mdi-forum-outline",
-        permission: "matrix.view_matrixrooms_rule",
     },
     props: {
         byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
     },
     children: [{
         path: "rooms/",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
```

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/locale/ar/LC_MESSAGES/django.po` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/locale/fr/LC_MESSAGES/django.po` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/locale/la/LC_MESSAGES/django.po` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/locale/ru/LC_MESSAGES/django.mo` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/locale/ru/LC_MESSAGES/django.po` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/locale/uk/LC_MESSAGES/django.mo` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/locale/uk/LC_MESSAGES/django.po` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/migrations/0001_initial.py` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/model_extensions.py` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/model_extensions.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/models.py` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/models.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/preferences.py` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/preferences.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/rules.py` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/rules.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/signals.py` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/signals.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/tasks.py` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/tasks.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/templates/matrix/room/list.html` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/templates/matrix/room/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/tests/conftest.py` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/tests/synapse/homeserver.yaml` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/tests/synapse/homeserver.yaml`

 * *Files identical despite different names*

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/tests/synapse/matrix.aleksis.example.org.log.config` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/tests/synapse/matrix.aleksis.example.org.log.config`

 * *Files identical despite different names*

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/tests/test_matrix.py` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/util/__pycache__/matrix.cpython-311.pyc` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/util/__pycache__/matrix.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x662b6164 (Sun May 14 18:41:42 2023 UTC)
+moddate:  0x3aad0064 (Thu Mar  2 14:05:46 2023 UTC)
 files sz: 1367
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 11
    flags     : 0
    code
```

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/util/matrix.py` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/util/matrix.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_matrix-2.0/aleksis/apps/matrix/views.py` & `aleksis_app_matrix-2.0b0/aleksis/apps/matrix/views.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_matrix-2.0/pyproject.toml` & `aleksis_app_matrix-2.0b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-App-Matrix"
-version = "2.0"
+version = "2.0b0"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = ["CHANGELOG.rst", "LICENCE.rst", "aleksis/**/*.mo"]
 
 description = "AlekSIS (School Information System) — App Matrix (Integration with Matrix/Element)"
@@ -28,15 +28,15 @@
 [[tool.poetry.source]]
 name = "gitlab"
 url = "https://edugit.org/api/v4/projects/461/packages/pypi/simple"
 secondary = true
 
 [tool.poetry.dependencies]
 python = "^3.9"
-aleksis-core = "^3.0"
+aleksis-core = "^3.0b0"
 
 [tool.poetry.dev-dependencies]
 aleksis-builddeps = ">=2023.1.dev0"
 matrix-synapse = "^1.49.2"
 pytest-xprocess = "^0.19.0"
 pytest-mock = "^3.7.0"
```

### Comparing `aleksis_app_matrix-2.0/setup.py` & `aleksis_app_matrix-2.0b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,22 +21,22 @@
                          'locale/ru/LC_MESSAGES/*',
                          'locale/tr_TR/LC_MESSAGES/*',
                          'locale/uk/LC_MESSAGES/*',
                          'templates/matrix/room/*'],
  'aleksis.apps.matrix.tests': ['synapse/*']}
 
 install_requires = \
-['aleksis-core>=3.0,<4.0']
+['aleksis-core>=3.0b0,<4.0']
 
 entry_points = \
 {'aleksis.app': ['matrix = aleksis.apps.matrix.apps:DefaultConfig']}
 
 setup_kwargs = {
     'name': 'aleksis-app-matrix',
-    'version': '2.0',
+    'version': '2.0b0',
     'description': 'AlekSIS (School Information System)\u200a—\u200aApp Matrix (Integration with Matrix/Element)',
     'long_description': 'AlekSIS (School Information System)\u200a—\u200aApp Matrix (Integration with Matrix/Element)\n==================================================================================================\n\nAlekSIS\n-------\n\nThis is an application for use with the `AlekSIS®`_ platform.\n\nFeatures\n--------\n\nThe author of this app did not describe it yet.\n\nLicence\n-------\n\n::\n\n  Copyright © 2021, 2022 Jonathan Weth <dev@jonathanweth.de>\n\n  Licenced under the EUPL, version 1.2 or later\n\nPlease see the LICENCE.rst file accompanying this distribution for the\nfull licence text or on the `European Union Public Licence`_ website\nhttps://joinup.ec.europa.eu/collection/eupl/guidelines-users-and-developers\n(including all other official language versions).\n\n.. _AlekSIS®: https://edugit.org/AlekSIS/AlekSIS\n.. _European Union Public Licence: https://eupl.eu/\n',
     'author': 'Jonathan Weth',
     'author_email': 'dev@jonathanweth.de',
     'maintainer': 'Jonathan Weth',
     'maintainer_email': 'wethjo@katharineum.de',
     'url': 'https://aleksis.org',
```

### Comparing `aleksis_app_matrix-2.0/PKG-INFO` & `aleksis_app_matrix-2.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleksis-app-matrix
-Version: 2.0
+Version: 2.0b0
 Summary: AlekSIS (School Information System) — App Matrix (Integration with Matrix/Element)
 Home-page: https://aleksis.org
 License: EUPL-1.2-or-later
 Author: Jonathan Weth
 Author-email: dev@jonathanweth.de
 Maintainer: Jonathan Weth
 Maintainer-email: wethjo@katharineum.de
@@ -16,15 +16,15 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
 Classifier: Typing :: Typed
-Requires-Dist: aleksis-core (>=3.0,<4.0)
+Requires-Dist: aleksis-core (>=3.0b0,<4.0)
 Project-URL: Repository, https://edugit.org/AlekSIS/official/AlekSIS-App-Matrix
 Description-Content-Type: text/x-rst
 
 AlekSIS (School Information System) — App Matrix (Integration with Matrix/Element)
 ==================================================================================================
 
 AlekSIS
```

