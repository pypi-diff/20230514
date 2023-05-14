# Comparing `tmp/aleksis_app_dashboardfeeds-3.0.tar.gz` & `tmp/aleksis_app_dashboardfeeds-3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_app_dashboardfeeds-3.0.tar", max compression
+gzip compressed data, was "aleksis_app_dashboardfeeds-3.0b0.tar", max compression
```

## Comparing `aleksis_app_dashboardfeeds-3.0.tar` & `aleksis_app_dashboardfeeds-3.0b0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     2265 2023-05-14 18:06:25.779835 aleksis_app_dashboardfeeds-3.0/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2023-05-14 18:06:25.779835 aleksis_app_dashboardfeeds-3.0/LICENCE.rst
--rw-r--r--   0        0        0     1311 2023-05-14 18:06:25.779835 aleksis_app_dashboardfeeds-3.0/README.rst
--rw-r--r--   0        0        0      160 2023-05-14 18:06:25.779835 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/__init__.py
--rw-r--r--   0        0        0      468 2023-05-14 18:20:13.335090 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      623 2023-05-14 18:20:17.967310 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0        0        0     1021 2023-05-14 18:20:14.603150 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0        0        0     6354 2023-05-14 18:20:17.659295 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/__pycache__/models.cpython-311.pyc
--rw-r--r--   0        0        0      230 2023-05-14 18:20:13.339090 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0        0        0      218 2023-05-14 18:06:25.779835 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/admin.py
--rw-r--r--   0        0        0      577 2023-05-14 18:06:25.779835 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/apps.py
--rw-r--r--   0        0        0        0 2023-05-14 18:06:25.779835 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/locale/.keepdir
--rw-r--r--   0        0        0      463 2023-05-14 18:20:18.979358 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2797 2023-05-14 18:06:25.779835 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2094 2023-05-14 18:20:18.967357 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3872 2023-05-14 18:06:25.779835 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2023-05-14 18:20:18.999359 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2713 2023-05-14 18:06:25.779835 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-05-14 18:20:18.991358 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2667 2023-05-14 18:06:25.779835 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-05-14 18:20:18.991358 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2667 2023-05-14 18:06:25.779835 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2675 2023-05-14 18:20:19.023360 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4040 2023-05-14 18:06:25.779835 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-05-14 18:20:18.959357 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2667 2023-05-14 18:06:25.783835 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2723 2023-05-14 18:20:18.979358 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4088 2023-05-14 18:06:25.783835 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2243 2023-05-14 18:06:25.783835 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/migrations/0001_initial.py
--rw-r--r--   0        0        0      809 2023-05-14 18:06:25.783835 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/migrations/0002_link_field_optional.py
--rw-r--r--   0        0        0        0 2023-05-14 18:06:25.783835 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/migrations/__init__.py
--rw-r--r--   0        0        0     3507 2023-05-14 18:06:25.783835 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/models.py
--rw-r--r--   0        0        0       34 2023-05-14 18:06:25.783835 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/settings.py
--rw-r--r--   0        0        0        0 2023-05-14 18:06:25.783835 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/static/.keepdir
--rw-r--r--   0        0        0       41 2023-05-14 18:06:25.783835 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/static/dashboardfeeds/css/style.css
--rw-r--r--   0        0        0    51251 2023-05-14 18:06:25.783835 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/static/dashboardfeeds/image_not_found.png
--rw-r--r--   0        0        0      255 2023-05-14 18:06:25.783835 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/tasks.py
--rw-r--r--   0        0        0      609 2023-05-14 18:06:25.783835 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/templates/dashboardfeeds/ical.html
--rw-r--r--   0        0        0     1581 2023-05-14 18:06:25.783835 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/templates/dashboardfeeds/rss.html
--rw-r--r--   0        0        0        0 2023-05-14 18:06:25.783835 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/util/__init__.py
--rw-r--r--   0        0        0      205 2023-05-14 18:20:17.663295 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/util/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3210 2023-05-14 18:20:17.663295 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/util/__pycache__/event_feed.cpython-311.pyc
--rw-r--r--   0        0        0     2588 2023-05-14 18:06:25.783835 aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/util/event_feed.py
--rw-r--r--   0        0        0      581 2023-05-14 18:06:25.783835 aleksis_app_dashboardfeeds-3.0/docs/Makefile
--rw-r--r--   0        0        0   103963 2023-05-14 18:06:25.783835 aleksis_app_dashboardfeeds-3.0/docs/_static/create_ical_widget.png
--rw-r--r--   0        0        0    99698 2023-05-14 18:06:25.787835 aleksis_app_dashboardfeeds-3.0/docs/_static/create_rss_widget.png
--rw-r--r--   0        0        0    46434 2023-05-14 18:06:25.787835 aleksis_app_dashboardfeeds-3.0/docs/_static/rss_widget.png
--rw-r--r--   0        0        0      120 2023-05-14 18:06:25.787835 aleksis_app_dashboardfeeds-3.0/docs/admin/00_index.rst
--rw-r--r--   0        0        0      251 2023-05-14 18:06:25.787835 aleksis_app_dashboardfeeds-3.0/docs/admin/01_introduction.rst
--rw-r--r--   0        0        0     1108 2023-05-14 18:06:25.787835 aleksis_app_dashboardfeeds-3.0/docs/admin/10_rss_feed_widget.rst
--rw-r--r--   0        0        0      732 2023-05-14 18:06:25.787835 aleksis_app_dashboardfeeds-3.0/docs/admin/11_ical_feed_widget.rst
--rw-r--r--   0        0        0     6405 2023-05-14 18:06:25.795836 aleksis_app_dashboardfeeds-3.0/docs/conf.py
--rw-r--r--   0        0        0      315 2023-05-14 18:06:25.807836 aleksis_app_dashboardfeeds-3.0/docs/index.rst
--rw-r--r--   0        0        0      787 2023-05-14 18:06:25.807836 aleksis_app_dashboardfeeds-3.0/docs/make.bat
--rw-r--r--   0        0        0     1815 2023-05-14 18:08:29.977725 aleksis_app_dashboardfeeds-3.0/pyproject.toml
--rw-r--r--   0        0        0     2563 2023-05-14 18:06:25.811837 aleksis_app_dashboardfeeds-3.0/tox.ini
--rw-r--r--   0        0        0     3259 1970-01-01 00:00:00.000000 aleksis_app_dashboardfeeds-3.0/setup.py
--rw-r--r--   0        0        0     2619 1970-01-01 00:00:00.000000 aleksis_app_dashboardfeeds-3.0/PKG-INFO
+-rw-r--r--   0        0        0     2122 2023-02-27 16:38:43.011530 aleksis_app_dashboardfeeds-3.0b0/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2023-02-27 16:38:43.011530 aleksis_app_dashboardfeeds-3.0b0/LICENCE.rst
+-rw-r--r--   0        0        0     1311 2023-02-27 16:38:43.011530 aleksis_app_dashboardfeeds-3.0b0/README.rst
+-rw-r--r--   0        0        0      160 2023-02-27 16:38:43.011530 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/__init__.py
+-rw-r--r--   0        0        0      468 2023-02-27 16:41:53.515179 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      623 2023-02-27 16:41:54.679177 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0        0        0     1021 2023-02-27 16:41:53.943179 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0        0        0     6354 2023-02-27 16:41:54.563178 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0        0        0      230 2023-02-27 16:41:53.519180 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0        0        0      218 2023-02-27 16:38:43.011530 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/admin.py
+-rw-r--r--   0        0        0      577 2023-02-27 16:38:43.011530 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/apps.py
+-rw-r--r--   0        0        0        0 2023-02-27 16:38:43.011530 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/locale/.keepdir
+-rw-r--r--   0        0        0      463 2023-02-27 16:41:54.951177 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2797 2023-02-27 16:38:43.011530 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2094 2023-02-27 16:41:54.947177 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3872 2023-02-27 16:38:43.011530 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2023-02-27 16:41:54.955177 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2713 2023-02-27 16:38:43.011530 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-02-27 16:41:54.951177 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2667 2023-02-27 16:38:43.011530 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-02-27 16:41:54.943177 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2667 2023-02-27 16:38:43.011530 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2675 2023-02-27 16:41:54.947177 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4040 2023-02-27 16:38:43.011530 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-02-27 16:41:54.951177 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2667 2023-02-27 16:38:43.011530 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2723 2023-02-27 16:41:54.955177 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4088 2023-02-27 16:38:43.011530 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2243 2023-02-27 16:38:43.011530 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/migrations/0001_initial.py
+-rw-r--r--   0        0        0      809 2023-02-27 16:38:43.011530 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/migrations/0002_link_field_optional.py
+-rw-r--r--   0        0        0        0 2023-02-27 16:38:43.011530 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/migrations/__init__.py
+-rw-r--r--   0        0        0     3507 2023-02-27 16:38:43.011530 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/models.py
+-rw-r--r--   0        0        0       34 2023-02-27 16:38:43.011530 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/settings.py
+-rw-r--r--   0        0        0        0 2023-02-27 16:38:43.011530 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/static/.keepdir
+-rw-r--r--   0        0        0       41 2023-02-27 16:38:43.015530 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/static/dashboardfeeds/css/style.css
+-rw-r--r--   0        0        0    51251 2023-02-27 16:38:43.015530 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/static/dashboardfeeds/image_not_found.png
+-rw-r--r--   0        0        0      255 2023-02-27 16:38:43.015530 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/tasks.py
+-rw-r--r--   0        0        0      609 2023-02-27 16:38:43.015530 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/templates/dashboardfeeds/ical.html
+-rw-r--r--   0        0        0     1581 2023-02-27 16:38:43.015530 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/templates/dashboardfeeds/rss.html
+-rw-r--r--   0        0        0        0 2023-02-27 16:38:43.015530 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/util/__init__.py
+-rw-r--r--   0        0        0      205 2023-02-27 16:41:54.563178 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/util/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3210 2023-02-27 16:41:54.567178 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/util/__pycache__/event_feed.cpython-311.pyc
+-rw-r--r--   0        0        0     2588 2023-02-27 16:38:43.015530 aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/util/event_feed.py
+-rw-r--r--   0        0        0      581 2023-02-27 16:38:43.015530 aleksis_app_dashboardfeeds-3.0b0/docs/Makefile
+-rw-r--r--   0        0        0   103963 2023-02-27 16:38:43.015530 aleksis_app_dashboardfeeds-3.0b0/docs/_static/create_ical_widget.png
+-rw-r--r--   0        0        0    99698 2023-02-27 16:38:43.015530 aleksis_app_dashboardfeeds-3.0b0/docs/_static/create_rss_widget.png
+-rw-r--r--   0        0        0    46434 2023-02-27 16:38:43.015530 aleksis_app_dashboardfeeds-3.0b0/docs/_static/rss_widget.png
+-rw-r--r--   0        0        0      120 2023-02-27 16:38:43.015530 aleksis_app_dashboardfeeds-3.0b0/docs/admin/00_index.rst
+-rw-r--r--   0        0        0      251 2023-02-27 16:38:43.015530 aleksis_app_dashboardfeeds-3.0b0/docs/admin/01_introduction.rst
+-rw-r--r--   0        0        0     1108 2023-02-27 16:38:43.015530 aleksis_app_dashboardfeeds-3.0b0/docs/admin/10_rss_feed_widget.rst
+-rw-r--r--   0        0        0      732 2023-02-27 16:38:43.015530 aleksis_app_dashboardfeeds-3.0b0/docs/admin/11_ical_feed_widget.rst
+-rw-r--r--   0        0        0     6407 2023-02-27 16:38:43.019530 aleksis_app_dashboardfeeds-3.0b0/docs/conf.py
+-rw-r--r--   0        0        0      315 2023-02-27 16:38:43.019530 aleksis_app_dashboardfeeds-3.0b0/docs/index.rst
+-rw-r--r--   0        0        0      787 2023-02-27 16:38:43.019530 aleksis_app_dashboardfeeds-3.0b0/docs/make.bat
+-rw-r--r--   0        0        0     1819 2023-02-27 16:39:21.143461 aleksis_app_dashboardfeeds-3.0b0/pyproject.toml
+-rw-r--r--   0        0        0     2563 2023-02-27 16:38:43.023530 aleksis_app_dashboardfeeds-3.0b0/tox.ini
+-rw-r--r--   0        0        0     3263 1970-01-01 00:00:00.000000 aleksis_app_dashboardfeeds-3.0b0/setup.py
+-rw-r--r--   0        0        0     2623 1970-01-01 00:00:00.000000 aleksis_app_dashboardfeeds-3.0b0/PKG-INFO
```

### Comparing `aleksis_app_dashboardfeeds-3.0/CHANGELOG.rst` & `aleksis_app_dashboardfeeds-3.0b0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,20 +2,15 @@
 =========
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
-`3.0`_ - 2023-05-14
--------------------
-
-Nothing changed.
-
-`3.0b0`_ - 2023-02-22
+`3.0b0` - 2023-02-22
 --------------------
 
 This version requires AlekSIS-Core 3.0. It is incompatible with any previous
 version.
 
 `2.1`_ - 2022-06-23
 -------------------
@@ -97,8 +92,7 @@
 .. _2.0a2: https://edugit.org/AlekSIS/Official/AlekSIS-App-DashboardFeeds/-/tags/2.0a2
 .. _2.0b0: https://edugit.org/AlekSIS/Official/AlekSIS-App-DashboardFeeds/-/tags/2.0b0
 .. _2.0rc1: https://edugit.org/AlekSIS/Official/AlekSIS-App-DashboardFeeds/-/tags/2.0rc1
 .. _2.0: https://edugit.org/AlekSIS/Official/AlekSIS-App-DashboardFeeds/-/tags/2.0
 .. _2.0.1: https://edugit.org/AlekSIS/Official/AlekSIS-App-DashboardFeeds/-/tags/2.0.1
 .. _2.1: https://edugit.org/AlekSIS/Official/AlekSIS-App-DashboardFeeds/-/tags/2.1
 .. _3.0b0: https://edugit.org/AlekSIS/Official/AlekSIS-App-DashboardFeeds/-/tags/3.0b0
-.. _3.0: https://edugit.org/AlekSIS/Official/AlekSIS-App-DashboardFeeds/-/tags/3.0
```

### Comparing `aleksis_app_dashboardfeeds-3.0/LICENCE.rst` & `aleksis_app_dashboardfeeds-3.0b0/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_dashboardfeeds-3.0/README.rst` & `aleksis_app_dashboardfeeds-3.0b0/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/__pycache__/admin.cpython-311.pyc` & `aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/__pycache__/admin.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x21236164 (Sun May 14 18:06:25 2023 UTC)
+moddate:  0x93dcfc63 (Mon Feb 27 16:38:43 2023 UTC)
 files sz: 218
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
```

### Comparing `aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/__pycache__/apps.cpython-311.pyc` & `aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/__pycache__/apps.cpython-311.pyc`

 * *Files 14% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x21236164 (Sun May 14 18:06:25 2023 UTC)
+moddate:  0x93dcfc63 (Mon Feb 27 16:38:43 2023 UTC)
 files sz: 577
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/__pycache__/models.cpython-311.pyc` & `aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/__pycache__/models.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x21236164 (Sun May 14 18:06:25 2023 UTC)
+moddate:  0x93dcfc63 (Mon Feb 27 16:38:43 2023 UTC)
 files sz: 3507
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/apps.py` & `aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/locale/ar/LC_MESSAGES/django.po` & `aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/locale/fr/LC_MESSAGES/django.po` & `aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/locale/la/LC_MESSAGES/django.po` & `aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/locale/ru/LC_MESSAGES/django.mo` & `aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/locale/ru/LC_MESSAGES/django.po` & `aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/locale/uk/LC_MESSAGES/django.mo` & `aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/locale/uk/LC_MESSAGES/django.po` & `aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/migrations/0001_initial.py` & `aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/migrations/0002_link_field_optional.py` & `aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/migrations/0002_link_field_optional.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/models.py` & `aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/models.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/static/dashboardfeeds/image_not_found.png` & `aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/static/dashboardfeeds/image_not_found.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/templates/dashboardfeeds/ical.html` & `aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/templates/dashboardfeeds/ical.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/templates/dashboardfeeds/rss.html` & `aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/templates/dashboardfeeds/rss.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/util/__pycache__/event_feed.cpython-311.pyc` & `aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/util/__pycache__/event_feed.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x21236164 (Sun May 14 18:06:25 2023 UTC)
+moddate:  0x93dcfc63 (Mon Feb 27 16:38:43 2023 UTC)
 files sz: 2588
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
```

### Comparing `aleksis_app_dashboardfeeds-3.0/aleksis/apps/dashboardfeeds/util/event_feed.py` & `aleksis_app_dashboardfeeds-3.0b0/aleksis/apps/dashboardfeeds/util/event_feed.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_dashboardfeeds-3.0/docs/Makefile` & `aleksis_app_dashboardfeeds-3.0b0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aleksis_app_dashboardfeeds-3.0/docs/_static/create_ical_widget.png` & `aleksis_app_dashboardfeeds-3.0b0/docs/_static/create_ical_widget.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_dashboardfeeds-3.0/docs/_static/create_rss_widget.png` & `aleksis_app_dashboardfeeds-3.0b0/docs/_static/create_rss_widget.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_dashboardfeeds-3.0/docs/_static/rss_widget.png` & `aleksis_app_dashboardfeeds-3.0b0/docs/_static/rss_widget.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_dashboardfeeds-3.0/docs/admin/10_rss_feed_widget.rst` & `aleksis_app_dashboardfeeds-3.0b0/docs/admin/10_rss_feed_widget.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_dashboardfeeds-3.0/docs/admin/11_ical_feed_widget.rst` & `aleksis_app_dashboardfeeds-3.0b0/docs/admin/11_ical_feed_widget.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_dashboardfeeds-3.0/docs/conf.py` & `aleksis_app_dashboardfeeds-3.0b0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 project = "AlekSIS-App-DashboardFeeds"
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

### Comparing `aleksis_app_dashboardfeeds-3.0/docs/make.bat` & `aleksis_app_dashboardfeeds-3.0b0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aleksis_app_dashboardfeeds-3.0/pyproject.toml` & `aleksis_app_dashboardfeeds-3.0b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-App-DashboardFeeds"
-version = "3.0"
+version = "3.0b0"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = [
     { path = "aleksis/**/*.mo", format = ["sdist", "wheel"] },
     { path = "*.rst", format = "sdist" },
@@ -37,15 +37,15 @@
 secondary = true
 
 [tool.poetry.dependencies]
 python = "^3.9"
 feedparser = "^6.0.0"
 django-feed-reader = "^1.0.0"
 ics = "^0.7"
-aleksis-core = "^3.0"
+aleksis-core = "^3.0b0"
 
 [tool.poetry.dev-dependencies]
 aleksis-builddeps = "*"
 
 [tool.poetry.plugins."aleksis.app"]
 dashboardfeeds = "aleksis.apps.dashboardfeeds.apps:DefaultConfig"
```

### Comparing `aleksis_app_dashboardfeeds-3.0/tox.ini` & `aleksis_app_dashboardfeeds-3.0b0/tox.ini`

 * *Files identical despite different names*

### Comparing `aleksis_app_dashboardfeeds-3.0/setup.py` & `aleksis_app_dashboardfeeds-3.0b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,26 +20,26 @@
                                  'locale/uk/LC_MESSAGES/*',
                                  'static/*',
                                  'static/dashboardfeeds/*',
                                  'static/dashboardfeeds/css/*',
                                  'templates/dashboardfeeds/*']}
 
 install_requires = \
-['aleksis-core>=3.0,<4.0',
+['aleksis-core>=3.0b0,<4.0',
  'django-feed-reader>=1.0.0,<2.0.0',
  'feedparser>=6.0.0,<7.0.0',
  'ics>=0.7,<0.8']
 
 entry_points = \
 {'aleksis.app': ['dashboardfeeds = '
                  'aleksis.apps.dashboardfeeds.apps:DefaultConfig']}
 
 setup_kwargs = {
     'name': 'aleksis-app-dashboardfeeds',
-    'version': '3.0',
+    'version': '3.0b0',
     'description': 'AlekSIS (School Information System)\u200a—\u200aApp Dashboard Feeds (Include feeds from external resources as widgets on dashboard)',
     'long_description': 'AlekSIS (School Information System)\u200a—\u200aApp Dashboard Feeds (Include feeds from external resources as widgets on dashboard)\n=========================================================================================================================\n\nAlekSIS\n-------\n\nThis is an application for use with the `AlekSIS®`_ platform.\n\nFeatures\n--------\n\n* Add RSS widgets to dashboard\n* Add iCal widgets to dashboard\n\nLicence\n-------\n\n::\n\n  Copyright © 2020 Dominik George <dominik.george@teckids.org>\n  Copyright © 2020 Julian Leucker <leuckerj@gmail.com>\n  Copyright © 2022 Jonathan Weth <dev@jonathanweth.de>\n\n  Licenced under the EUPL, version 1.2 or later, by Teckids e.V. (Bonn, Germany).\n\nPlease see the LICENCE.rst file accompanying this distribution for the\nfull licence text or on the `European Union Public Licence`_ website\nhttps://joinup.ec.europa.eu/collection/eupl/guidelines-users-and-developers\n(including all other official language versions).\n\nTrademark\n---------\n\nAlekSIS® is a registered trademark of the AlekSIS open source project, represented\nby Teckids e.V. Please refer to the `trademark policy`_ for hints on using the trademark\nAlekSIS®.\n\n.. _AlekSIS®: https://aleksis.org/\n.. _European Union Public Licence: https://eupl.eu/\n.. _trademark policy: https://aleksis.org/pages/about\n',
     'author': 'Julian Leucker',
     'author_email': 'leuckerj@gmail.com',
     'maintainer': 'Jonathan Weth',
     'maintainer_email': 'wethjo@katharineum.de',
     'url': 'https://aleksis.org/',
```

### Comparing `aleksis_app_dashboardfeeds-3.0/PKG-INFO` & `aleksis_app_dashboardfeeds-3.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleksis-app-dashboardfeeds
-Version: 3.0
+Version: 3.0b0
 Summary: AlekSIS (School Information System) — App Dashboard Feeds (Include feeds from external resources as widgets on dashboard)
 Home-page: https://aleksis.org/
 License: EUPL-1.2-or-later
 Keywords: SIS,education,school,calendar,rss
 Author: Julian Leucker
 Author-email: leuckerj@gmail.com
 Maintainer: Jonathan Weth
@@ -17,15 +17,15 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
 Classifier: Typing :: Typed
-Requires-Dist: aleksis-core (>=3.0,<4.0)
+Requires-Dist: aleksis-core (>=3.0b0,<4.0)
 Requires-Dist: django-feed-reader (>=1.0.0,<2.0.0)
 Requires-Dist: feedparser (>=6.0.0,<7.0.0)
 Requires-Dist: ics (>=0.7,<0.8)
 Project-URL: Documentation, https://aleksis.org/AlekSIS/docs/html/
 Project-URL: Repository, https://edugit.org/AlekSIS/official/AlekSIS-App-DashboardFeeds
 Description-Content-Type: text/x-rst
```

