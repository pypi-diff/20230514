# Comparing `tmp/django-rq-2.8.0.tar.gz` & `tmp/django-rq-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-rq-2.8.0.tar", last modified: Tue May  2 03:20:05 2023, max compression
+gzip compressed data, was "django-rq-2.8.1.tar", last modified: Sun May 14 01:32:12 2023, max compression
```

## Comparing `django-rq-2.8.0.tar` & `django-rq-2.8.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-02 03:20:05.308218 django-rq-2.8.0/
--rw-r--r--   0 selwin     (501) staff       (20)     7937 2023-05-02 03:15:45.000000 django-rq-2.8.0/CHANGELOG.md
--rw-r--r--   0 selwin     (501) staff       (20)     1053 2017-12-06 00:54:06.000000 django-rq-2.8.0/LICENSE.txt
--rw-r--r--   0 selwin     (501) staff       (20)      100 2019-12-07 09:59:35.000000 django-rq-2.8.0/MANIFEST.in
--rw-r--r--   0 selwin     (501) staff       (20)    22989 2023-05-02 03:20:05.308385 django-rq-2.8.0/PKG-INFO
--rw-r--r--   0 selwin     (501) staff       (20)    17351 2023-05-02 03:15:57.000000 django-rq-2.8.0/README.rst
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-02 03:20:05.300553 django-rq-2.8.0/django_rq/
--rw-r--r--   0 selwin     (501) staff       (20)      151 2023-05-02 03:17:58.000000 django-rq-2.8.0/django_rq/__init__.py
--rw-r--r--   0 selwin     (501) staff       (20)     1174 2023-05-02 02:24:10.000000 django-rq-2.8.0/django_rq/admin.py
--rw-r--r--   0 selwin     (501) staff       (20)     1162 2023-05-02 02:24:10.000000 django-rq-2.8.0/django_rq/decorators.py
--rw-r--r--   0 selwin     (501) staff       (20)      524 2023-02-07 11:14:52.000000 django-rq-2.8.0/django_rq/jobs.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-02 03:20:05.301658 django-rq-2.8.0/django_rq/management/
--rw-r--r--   0 selwin     (501) staff       (20)        0 2020-03-08 09:24:48.000000 django-rq-2.8.0/django_rq/management/__init__.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-02 03:20:05.302733 django-rq-2.8.0/django_rq/management/commands/
--rw-r--r--   0 selwin     (501) staff       (20)        0 2020-03-08 09:24:48.000000 django-rq-2.8.0/django_rq/management/commands/__init__.py
--rw-r--r--   0 selwin     (501) staff       (20)     1060 2022-11-01 13:42:48.000000 django-rq-2.8.0/django_rq/management/commands/rqenqueue.py
--rw-r--r--   0 selwin     (501) staff       (20)     1703 2022-11-01 13:42:48.000000 django-rq-2.8.0/django_rq/management/commands/rqscheduler.py
--rw-r--r--   0 selwin     (501) staff       (20)     3033 2020-03-31 10:08:21.000000 django-rq-2.8.0/django_rq/management/commands/rqstats.py
--rw-r--r--   0 selwin     (501) staff       (20)     5681 2023-05-02 02:24:10.000000 django-rq-2.8.0/django_rq/management/commands/rqworker.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-02 03:20:05.303103 django-rq-2.8.0/django_rq/migrations/
--rw-r--r--   0 selwin     (501) staff       (20)      967 2021-11-17 00:53:40.000000 django-rq-2.8.0/django_rq/migrations/0001_initial.py
--rw-r--r--   0 selwin     (501) staff       (20)        0 2021-11-17 00:53:40.000000 django-rq-2.8.0/django_rq/migrations/__init__.py
--rw-r--r--   0 selwin     (501) staff       (20)      667 2023-05-02 02:24:10.000000 django-rq-2.8.0/django_rq/models.py
--rw-r--r--   0 selwin     (501) staff       (20)    10687 2023-05-02 02:24:10.000000 django-rq-2.8.0/django_rq/queues.py
--rw-r--r--   0 selwin     (501) staff       (20)      877 2023-02-07 11:14:43.000000 django-rq-2.8.0/django_rq/settings.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-02 03:20:05.294806 django-rq-2.8.0/django_rq/templates/
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-02 03:20:05.305148 django-rq-2.8.0/django_rq/templates/django_rq/
--rw-r--r--   0 selwin     (501) staff       (20)     1098 2020-03-08 09:24:48.000000 django-rq-2.8.0/django_rq/templates/django_rq/clear_queue.html
--rw-r--r--   0 selwin     (501) staff       (20)     1642 2020-11-08 03:24:12.000000 django-rq-2.8.0/django_rq/templates/django_rq/confirm_action.html
--rw-r--r--   0 selwin     (501) staff       (20)     1260 2020-03-08 09:24:48.000000 django-rq-2.8.0/django_rq/templates/django_rq/delete_job.html
--rw-r--r--   0 selwin     (501) staff       (20)     7833 2023-01-29 01:06:02.000000 django-rq-2.8.0/django_rq/templates/django_rq/job_detail.html
--rw-r--r--   0 selwin     (501) staff       (20)     6559 2022-11-05 01:59:59.000000 django-rq-2.8.0/django_rq/templates/django_rq/jobs.html
--rw-r--r--   0 selwin     (501) staff       (20)     1156 2020-03-08 09:24:48.000000 django-rq-2.8.0/django_rq/templates/django_rq/requeue_all.html
--rw-r--r--   0 selwin     (501) staff       (20)     3810 2023-05-02 02:24:10.000000 django-rq-2.8.0/django_rq/templates/django_rq/stats.html
--rw-r--r--   0 selwin     (501) staff       (20)        3 2020-03-08 09:24:48.000000 django-rq-2.8.0/django_rq/templates/django_rq/test.html
--rw-r--r--   0 selwin     (501) staff       (20)     3353 2020-11-08 03:24:20.000000 django-rq-2.8.0/django_rq/templates/django_rq/worker_details.html
--rw-r--r--   0 selwin     (501) staff       (20)     2871 2020-11-08 03:24:12.000000 django-rq-2.8.0/django_rq/templates/django_rq/workers.html
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-02 03:20:05.305504 django-rq-2.8.0/django_rq/templatetags/
--rw-r--r--   0 selwin     (501) staff       (20)        0 2020-03-08 09:24:48.000000 django-rq-2.8.0/django_rq/templatetags/__init__.py
--rw-r--r--   0 selwin     (501) staff       (20)      646 2021-11-17 00:53:40.000000 django-rq-2.8.0/django_rq/templatetags/django_rq.py
--rw-r--r--   0 selwin     (501) staff       (20)      152 2022-11-01 13:42:48.000000 django-rq-2.8.0/django_rq/templatetags/jquery_path.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-02 03:20:05.307974 django-rq-2.8.0/django_rq/tests/
--rw-r--r--   0 selwin     (501) staff       (20)        0 2020-03-08 09:24:48.000000 django-rq-2.8.0/django_rq/tests/__init__.py
--rw-r--r--   0 selwin     (501) staff       (20)      493 2023-05-02 02:24:10.000000 django-rq-2.8.0/django_rq/tests/fixtures.py
--rw-r--r--   0 selwin     (501) staff       (20)     5813 2023-05-02 03:15:57.000000 django-rq-2.8.0/django_rq/tests/settings.py
--rw-r--r--   0 selwin     (501) staff       (20)    14477 2023-05-02 03:15:57.000000 django-rq-2.8.0/django_rq/tests/test_views.py
--rw-r--r--   0 selwin     (501) staff       (20)    36067 2023-05-02 02:24:10.000000 django-rq-2.8.0/django_rq/tests/tests.py
--rw-r--r--   0 selwin     (501) staff       (20)      335 2023-05-02 02:24:10.000000 django-rq-2.8.0/django_rq/tests/urls.py
--rw-r--r--   0 selwin     (501) staff       (20)      548 2023-02-07 11:15:20.000000 django-rq-2.8.0/django_rq/tests/utils.py
--rw-r--r--   0 selwin     (501) staff       (20)      334 2023-02-07 11:15:18.000000 django-rq-2.8.0/django_rq/tests/views.py
--rw-r--r--   0 selwin     (501) staff       (20)     1148 2023-05-02 02:24:10.000000 django-rq-2.8.0/django_rq/thread_queue.py
--rw-r--r--   0 selwin     (501) staff       (20)     1937 2023-05-02 02:24:10.000000 django-rq-2.8.0/django_rq/urls.py
--rw-r--r--   0 selwin     (501) staff       (20)     4450 2023-05-02 02:24:10.000000 django-rq-2.8.0/django_rq/utils.py
--rw-r--r--   0 selwin     (501) staff       (20)    16450 2023-05-02 03:15:57.000000 django-rq-2.8.0/django_rq/views.py
--rw-r--r--   0 selwin     (501) staff       (20)     1689 2023-05-02 02:24:10.000000 django-rq-2.8.0/django_rq/workers.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-02 03:20:05.301555 django-rq-2.8.0/django_rq.egg-info/
--rw-r--r--   0 selwin     (501) staff       (20)    22989 2023-05-02 03:20:05.000000 django-rq-2.8.0/django_rq.egg-info/PKG-INFO
--rw-r--r--   0 selwin     (501) staff       (20)     1598 2023-05-02 03:20:05.000000 django-rq-2.8.0/django_rq.egg-info/SOURCES.txt
--rw-r--r--   0 selwin     (501) staff       (20)        1 2023-05-02 03:20:05.000000 django-rq-2.8.0/django_rq.egg-info/dependency_links.txt
--rw-r--r--   0 selwin     (501) staff       (20)        1 2017-12-06 07:07:26.000000 django-rq-2.8.0/django_rq.egg-info/not-zip-safe
--rw-r--r--   0 selwin     (501) staff       (20)       75 2023-05-02 03:20:05.000000 django-rq-2.8.0/django_rq.egg-info/requires.txt
--rw-r--r--   0 selwin     (501) staff       (20)       10 2023-05-02 03:20:05.000000 django-rq-2.8.0/django_rq.egg-info/top_level.txt
--rw-r--r--   0 selwin     (501) staff       (20)       67 2023-05-02 03:20:05.308648 django-rq-2.8.0/setup.cfg
--rw-r--r--   0 selwin     (501) staff       (20)     1416 2023-05-02 03:17:48.000000 django-rq-2.8.0/setup.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-14 01:32:12.436501 django-rq-2.8.1/
+-rw-r--r--   0 selwin     (501) staff       (20)     8173 2023-05-14 01:31:20.000000 django-rq-2.8.1/CHANGELOG.md
+-rw-r--r--   0 selwin     (501) staff       (20)     1053 2017-12-06 00:54:06.000000 django-rq-2.8.1/LICENSE.txt
+-rw-r--r--   0 selwin     (501) staff       (20)      100 2019-12-07 09:59:35.000000 django-rq-2.8.1/MANIFEST.in
+-rw-r--r--   0 selwin     (501) staff       (20)    18424 2023-05-14 01:32:12.436554 django-rq-2.8.1/PKG-INFO
+-rw-r--r--   0 selwin     (501) staff       (20)    17351 2023-05-02 03:15:57.000000 django-rq-2.8.1/README.rst
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-14 01:32:12.429965 django-rq-2.8.1/django_rq/
+-rw-r--r--   0 selwin     (501) staff       (20)      151 2023-05-14 01:27:26.000000 django-rq-2.8.1/django_rq/__init__.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1174 2023-05-02 02:24:10.000000 django-rq-2.8.1/django_rq/admin.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1162 2023-05-02 02:24:10.000000 django-rq-2.8.1/django_rq/decorators.py
+-rw-r--r--   0 selwin     (501) staff       (20)      524 2023-02-07 11:14:52.000000 django-rq-2.8.1/django_rq/jobs.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-14 01:32:12.430881 django-rq-2.8.1/django_rq/management/
+-rw-r--r--   0 selwin     (501) staff       (20)        0 2020-03-08 09:24:48.000000 django-rq-2.8.1/django_rq/management/__init__.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-14 01:32:12.431722 django-rq-2.8.1/django_rq/management/commands/
+-rw-r--r--   0 selwin     (501) staff       (20)        0 2020-03-08 09:24:48.000000 django-rq-2.8.1/django_rq/management/commands/__init__.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1060 2022-11-01 13:42:48.000000 django-rq-2.8.1/django_rq/management/commands/rqenqueue.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1703 2022-11-01 13:42:48.000000 django-rq-2.8.1/django_rq/management/commands/rqscheduler.py
+-rw-r--r--   0 selwin     (501) staff       (20)     3093 2023-05-14 01:25:52.000000 django-rq-2.8.1/django_rq/management/commands/rqstats.py
+-rw-r--r--   0 selwin     (501) staff       (20)     5681 2023-05-02 02:24:10.000000 django-rq-2.8.1/django_rq/management/commands/rqworker.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-14 01:32:12.432038 django-rq-2.8.1/django_rq/migrations/
+-rw-r--r--   0 selwin     (501) staff       (20)      967 2021-11-17 00:53:40.000000 django-rq-2.8.1/django_rq/migrations/0001_initial.py
+-rw-r--r--   0 selwin     (501) staff       (20)        0 2021-11-17 00:53:40.000000 django-rq-2.8.1/django_rq/migrations/__init__.py
+-rw-r--r--   0 selwin     (501) staff       (20)      667 2023-05-02 02:24:10.000000 django-rq-2.8.1/django_rq/models.py
+-rw-r--r--   0 selwin     (501) staff       (20)    10687 2023-05-02 02:24:10.000000 django-rq-2.8.1/django_rq/queues.py
+-rw-r--r--   0 selwin     (501) staff       (20)      877 2023-02-07 11:14:43.000000 django-rq-2.8.1/django_rq/settings.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-14 01:32:12.426276 django-rq-2.8.1/django_rq/templates/
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-14 01:32:12.433657 django-rq-2.8.1/django_rq/templates/django_rq/
+-rw-r--r--   0 selwin     (501) staff       (20)     1098 2020-03-08 09:24:48.000000 django-rq-2.8.1/django_rq/templates/django_rq/clear_queue.html
+-rw-r--r--   0 selwin     (501) staff       (20)     1642 2020-11-08 03:24:12.000000 django-rq-2.8.1/django_rq/templates/django_rq/confirm_action.html
+-rw-r--r--   0 selwin     (501) staff       (20)     1260 2020-03-08 09:24:48.000000 django-rq-2.8.1/django_rq/templates/django_rq/delete_job.html
+-rw-r--r--   0 selwin     (501) staff       (20)     8109 2023-05-14 01:25:52.000000 django-rq-2.8.1/django_rq/templates/django_rq/job_detail.html
+-rw-r--r--   0 selwin     (501) staff       (20)     6715 2023-05-14 01:25:52.000000 django-rq-2.8.1/django_rq/templates/django_rq/jobs.html
+-rw-r--r--   0 selwin     (501) staff       (20)     1156 2020-03-08 09:24:48.000000 django-rq-2.8.1/django_rq/templates/django_rq/requeue_all.html
+-rw-r--r--   0 selwin     (501) staff       (20)     3807 2023-05-14 01:25:52.000000 django-rq-2.8.1/django_rq/templates/django_rq/stats.html
+-rw-r--r--   0 selwin     (501) staff       (20)        3 2020-03-08 09:24:48.000000 django-rq-2.8.1/django_rq/templates/django_rq/test.html
+-rw-r--r--   0 selwin     (501) staff       (20)     3353 2020-11-08 03:24:20.000000 django-rq-2.8.1/django_rq/templates/django_rq/worker_details.html
+-rw-r--r--   0 selwin     (501) staff       (20)     2871 2020-11-08 03:24:12.000000 django-rq-2.8.1/django_rq/templates/django_rq/workers.html
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-14 01:32:12.433968 django-rq-2.8.1/django_rq/templatetags/
+-rw-r--r--   0 selwin     (501) staff       (20)        0 2020-03-08 09:24:48.000000 django-rq-2.8.1/django_rq/templatetags/__init__.py
+-rw-r--r--   0 selwin     (501) staff       (20)      646 2021-11-17 00:53:40.000000 django-rq-2.8.1/django_rq/templatetags/django_rq.py
+-rw-r--r--   0 selwin     (501) staff       (20)      152 2022-11-01 13:42:48.000000 django-rq-2.8.1/django_rq/templatetags/jquery_path.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-14 01:32:12.436252 django-rq-2.8.1/django_rq/tests/
+-rw-r--r--   0 selwin     (501) staff       (20)        0 2020-03-08 09:24:48.000000 django-rq-2.8.1/django_rq/tests/__init__.py
+-rw-r--r--   0 selwin     (501) staff       (20)      493 2023-05-02 02:24:10.000000 django-rq-2.8.1/django_rq/tests/fixtures.py
+-rw-r--r--   0 selwin     (501) staff       (20)     5813 2023-05-02 03:15:57.000000 django-rq-2.8.1/django_rq/tests/settings.py
+-rw-r--r--   0 selwin     (501) staff       (20)    15843 2023-05-14 01:25:52.000000 django-rq-2.8.1/django_rq/tests/test_views.py
+-rw-r--r--   0 selwin     (501) staff       (20)    36067 2023-05-02 02:24:10.000000 django-rq-2.8.1/django_rq/tests/tests.py
+-rw-r--r--   0 selwin     (501) staff       (20)      335 2023-05-02 02:24:10.000000 django-rq-2.8.1/django_rq/tests/urls.py
+-rw-r--r--   0 selwin     (501) staff       (20)      548 2023-02-07 11:15:20.000000 django-rq-2.8.1/django_rq/tests/utils.py
+-rw-r--r--   0 selwin     (501) staff       (20)      334 2023-02-07 11:15:18.000000 django-rq-2.8.1/django_rq/tests/views.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1148 2023-05-02 02:24:10.000000 django-rq-2.8.1/django_rq/thread_queue.py
+-rw-r--r--   0 selwin     (501) staff       (20)     2060 2023-05-14 01:25:52.000000 django-rq-2.8.1/django_rq/urls.py
+-rw-r--r--   0 selwin     (501) staff       (20)     4945 2023-05-14 01:25:52.000000 django-rq-2.8.1/django_rq/utils.py
+-rw-r--r--   0 selwin     (501) staff       (20)    17494 2023-05-14 01:25:52.000000 django-rq-2.8.1/django_rq/views.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1689 2023-05-02 02:24:10.000000 django-rq-2.8.1/django_rq/workers.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-14 01:32:12.430776 django-rq-2.8.1/django_rq.egg-info/
+-rw-r--r--   0 selwin     (501) staff       (20)    18424 2023-05-14 01:32:12.000000 django-rq-2.8.1/django_rq.egg-info/PKG-INFO
+-rw-r--r--   0 selwin     (501) staff       (20)     1598 2023-05-14 01:32:12.000000 django-rq-2.8.1/django_rq.egg-info/SOURCES.txt
+-rw-r--r--   0 selwin     (501) staff       (20)        1 2023-05-14 01:32:12.000000 django-rq-2.8.1/django_rq.egg-info/dependency_links.txt
+-rw-r--r--   0 selwin     (501) staff       (20)        1 2017-12-06 07:07:26.000000 django-rq-2.8.1/django_rq.egg-info/not-zip-safe
+-rw-r--r--   0 selwin     (501) staff       (20)       76 2023-05-14 01:32:12.000000 django-rq-2.8.1/django_rq.egg-info/requires.txt
+-rw-r--r--   0 selwin     (501) staff       (20)       10 2023-05-14 01:32:12.000000 django-rq-2.8.1/django_rq.egg-info/top_level.txt
+-rw-r--r--   0 selwin     (501) staff       (20)       67 2023-05-14 01:32:12.436772 django-rq-2.8.1/setup.cfg
+-rw-r--r--   0 selwin     (501) staff       (20)     1417 2023-05-14 01:27:18.000000 django-rq-2.8.1/setup.py
```

### Comparing `django-rq-2.8.0/CHANGELOG.md` & `django-rq-2.8.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# Version 2.8.1 (2023-05-14)
+* Added a button to stop currently running jobs. Thanks @gabriels1234!
+* Added a failed jobs column to rqstats command. Thanks @dangquangdon!
+* Explicitly requires RQ >= 1.14 in `setup.py`. Thanks @selwin!
+
 # Version 2.8.0 (2023-05-02)
 * Support for RQ 1.14. Thanks @Cerebro92 and @selwin!
 * Show scheduler PID information in admin interface. Thanks @gabriels1234!
 * Added `serializer` argument to `rqworker` command. Thanks @gabriels1234!
 * Added `USERNAME` and `SENTINEL_KWARGS` support. Thanks @joachimBurket!
 
 # Version 2.7.0 (2023-02-07)
```

### Comparing `django-rq-2.8.0/LICENSE.txt` & `django-rq-2.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-rq-2.8.0/PKG-INFO` & `django-rq-2.8.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,587 +1,15 @@
 Metadata-Version: 2.1
 Name: django-rq
-Version: 2.8.0
+Version: 2.8.1
 Summary: An app that provides django integration for RQ (Redis Queue)
 Home-page: https://github.com/rq/django-rq
 Author: Selwin Ong
 Author-email: selwin.ong@gmail.com
 License: MIT
-Description: =========
-        Django-RQ
-        =========
-        
-        |Build Status|
-        
-        Django integration with `RQ <https://github.com/nvie/rq>`__, a `Redis <http://redis.io/>`__
-        based Python queuing library. `Django-RQ <https://github.com/rq/django-rq>`__ is a
-        simple app that allows you to configure your queues in django's ``settings.py``
-        and easily use them in your project.
-        
-        =================
-        Support Django-RQ
-        =================
-        
-        If you find ``django-rq`` useful, please consider supporting its development via `Tidelift <https://tidelift.com/subscription/pkg/pypi-django_rq?utm_source=pypi-django-rq&utm_medium=referral&utm_campaign=readme>`_.
-        
-        ============
-        Requirements
-        ============
-        
-        * `Django <https://www.djangoproject.com/>`__ (2.0+)
-        * `RQ <https://github.com/nvie/rq>`__
-        
-        ============
-        Installation
-        ============
-        
-        * Install ``django-rq`` (or `download from PyPI <http://pypi.python.org/pypi/django-rq>`__):
-        
-        .. code-block:: python
-        
-            pip install django-rq
-        
-        * Add ``django_rq`` to ``INSTALLED_APPS`` in ``settings.py``:
-        
-        .. code-block:: python
-        
-            INSTALLED_APPS = (
-                # other apps
-                "django_rq",
-            )
-        
-        * Configure your queues in django's ``settings.py``:
-        
-        .. code-block:: python
-        
-            RQ_QUEUES = {
-                'default': {
-                    'HOST': 'localhost',
-                    'PORT': 6379,
-                    'DB': 0,
-                    'USERNAME': 'some-user',
-                    'PASSWORD': 'some-password',
-                    'DEFAULT_TIMEOUT': 360,
-                    'REDIS_CLIENT_KWARGS': {    # Eventual additional Redis connection arguments
-                        'ssl_cert_reqs': None,
-                    },
-                },
-                'with-sentinel': {
-                    'SENTINELS': [('localhost', 26736), ('localhost', 26737)],
-                    'MASTER_NAME': 'redismaster',
-                    'DB': 0,
-                    # Redis username/password
-                    'USERNAME': 'redis-user',
-                    'PASSWORD': 'secret',
-                    'SOCKET_TIMEOUT': 0.3,
-                    'CONNECTION_KWARGS': {  # Eventual additional Redis connection arguments
-                        'ssl': True
-                    }
-                    'SENTINEL_KWARGS': {    # Eventual Sentinel connection arguments
-                        # If Sentinel also has auth, username/password can be passed here
-                        'username': 'sentinel-user',
-                        'password': 'secret',
-                    },
-                },
-                'high': {
-                    'URL': os.getenv('REDISTOGO_URL', 'redis://localhost:6379/0'), # If you're on Heroku
-                    'DEFAULT_TIMEOUT': 500,
-                },
-                'low': {
-                    'HOST': 'localhost',
-                    'PORT': 6379,
-                    'DB': 0,
-                }
-            }
-        
-            RQ_EXCEPTION_HANDLERS = ['path.to.my.handler'] # If you need custom exception handlers
-        
-        * Include ``django_rq.urls`` in your ``urls.py``:
-        
-        .. code-block:: python
-        
-            urlpatterns += [
-                path('django-rq/', include('django_rq.urls'))
-            ]
-        
-        =====
-        Usage
-        =====
-        
-        Putting jobs in the queue
-        -------------------------
-        
-        `Django-RQ` allows you to easily put jobs into any of the queues defined in
-        ``settings.py``. It comes with a few utility functions:
-        
-        * ``enqueue`` - push a job to the ``default`` queue:
-        
-        .. code-block:: python
-        
-            import django_rq
-            django_rq.enqueue(func, foo, bar=baz)
-        
-        * ``get_queue`` - returns an ``Queue`` instance.
-        
-        .. code-block:: python
-        
-            import django_rq
-            queue = django_rq.get_queue('high')
-            queue.enqueue(func, foo, bar=baz)
-        
-        In addition to ``name`` argument, ``get_queue`` also accepts ``default_timeout``,
-        ``is_async``, ``autocommit``, ``connection`` and ``queue_class`` arguments. For example:
-        
-        .. code-block:: python
-        
-            queue = django_rq.get_queue('default', autocommit=True, is_async=True, default_timeout=360)
-            queue.enqueue(func, foo, bar=baz)
-        
-        You can provide your own singleton Redis connection object to this function so that it will not
-        create a new connection object for each queue definition. This will help you limit
-        number of connections to Redis server. For example:
-        
-        .. code-block:: python
-        
-            import django_rq
-            import redis
-            redis_cursor = redis.StrictRedis(host='', port='', db='', password='')
-            high_queue = django_rq.get_queue('high', connection=redis_cursor)
-            low_queue = django_rq.get_queue('low', connection=redis_cursor)
-        
-        
-        * ``get_connection`` - accepts a single queue name argument (defaults to "default")
-          and returns a connection to the queue's Redis server:
-        
-        .. code-block:: python
-        
-            import django_rq
-            redis_conn = django_rq.get_connection('high')
-        
-        * ``get_worker`` - accepts optional queue names and returns a new `RQ`
-          ``Worker`` instance for specified queues (or ``default`` queue):
-        
-        .. code-block:: python
-        
-            import django_rq
-            worker = django_rq.get_worker() # Returns a worker for "default" queue
-            worker.work()
-            worker = django_rq.get_worker('low', 'high') # Returns a worker for "low" and "high"
-        
-        
-        @job decorator
-        --------------
-        
-        To easily turn a callable into an RQ task, you can also use the ``@job``
-        decorator that comes with ``django_rq``:
-        
-        .. code-block:: python
-        
-            from django_rq import job
-        
-            @job
-            def long_running_func():
-                pass
-            long_running_func.delay() # Enqueue function in "default" queue
-        
-            @job('high')
-            def long_running_func():
-                pass
-            long_running_func.delay() # Enqueue function in "high" queue
-        
-        You can pass in any arguments that RQ's job decorator accepts:
-        
-        .. code-block:: python
-        
-            @job('default', timeout=3600)
-            def long_running_func():
-                pass
-            long_running_func.delay() # Enqueue function with a timeout of 3600 seconds.
-        
-        It's possible to specify default for ``result_ttl`` decorator keyword argument
-        via ``DEFAULT_RESULT_TTL`` setting:
-        
-        .. code-block:: python
-        
-            RQ = {
-                'DEFAULT_RESULT_TTL': 5000,
-            }
-        
-        With this setting, job decorator will set ``result_ttl`` to 5000 unless it's
-        specified explicitly.
-        
-        
-        Running workers
-        ---------------
-        django_rq provides a management command that starts a worker for every queue
-        specified as arguments::
-        
-            python manage.py rqworker high default low
-        
-        If you want to run ``rqworker`` in burst mode, you can pass in the ``--burst`` flag::
-        
-            python manage.py rqworker high default low --burst
-        
-        If you need to use custom worker, job or queue classes, it is best to use global settings
-        (see `Custom queue classes`_ and `Custom job and worker classes`_). However, it is also possible
-        to override such settings with command line options as follows.
-        
-        To use a custom worker class, you can pass in the ``--worker-class`` flag
-        with the path to your worker::
-        
-            python manage.py rqworker high default low --worker-class 'path.to.GeventWorker'
-        
-        To use a custom queue class, you can pass in the ``--queue-class`` flag
-        with the path to your queue class::
-        
-            python manage.py rqworker high default low --queue-class 'path.to.CustomQueue'
-        
-        To use a custom job class, provide ``--job-class`` flag.
-        
-        Support for scheduled jobs
-        --------------------------
-        
-        With RQ 1.2.0. you can use `built-in scheduler <https://python-rq.org/docs/scheduling/>`__
-        for your jobs. For example:
-        
-        .. code-block:: python
-        
-            from django_rq.queues import get_queue
-            queue = get_queue('default')
-            job = queue.enqueue_at(datetime(2020, 10, 10), func)
-            
-        If you are using built-in scheduler you have to start workers with scheduler support::
-        
-            python manage.py rqworker --with-scheduler
-        
-        
-        Alternatively you can use `RQ Scheduler <https://github.com/ui/rq-scheduler>`__.
-        After install you can also use the ``get_scheduler`` function to return a
-        ``Scheduler`` instance for queues defined in settings.py's ``RQ_QUEUES``.
-        For example:
-        
-        .. code-block:: python
-        
-            import django_rq
-            scheduler = django_rq.get_scheduler('default')
-            job = scheduler.enqueue_at(datetime(2020, 10, 10), func)
-        
-        You can also use the management command ``rqscheduler`` to start the scheduler::
-        
-            python manage.py rqscheduler
-        
-        
-        Support for django-redis and django-redis-cache
-        -----------------------------------------------
-        
-        If you have `django-redis <https://django-redis.readthedocs.org/>`__ or
-        `django-redis-cache <https://github.com/sebleier/django-redis-cache/>`__
-        installed, you can instruct django_rq to use the same connection information
-        from your Redis cache. This has two advantages: it's DRY and it takes advantage
-        of any optimization that may be going on in your cache setup (like using
-        connection pooling or `Hiredis <https://github.com/redis/hiredis>`__.)
-        
-        To use configure it, use a dict with the key ``USE_REDIS_CACHE`` pointing to the
-        name of the desired cache in your ``RQ_QUEUES`` dict. It goes without saying
-        that the chosen cache must exist and use the Redis backend. See your respective
-        Redis cache package docs for configuration instructions. It's also important to
-        point out that since the django-redis-cache ``ShardedClient`` splits the cache
-        over multiple Redis connections, it does not work.
-        
-        Here is an example settings fragment for `django-redis`:
-        
-        .. code-block:: python
-        
-            CACHES = {
-                'redis-cache': {
-                    'BACKEND': 'redis_cache.cache.RedisCache',
-                    'LOCATION': 'localhost:6379:1',
-                    'OPTIONS': {
-                        'CLIENT_CLASS': 'django_redis.client.DefaultClient',
-                        'MAX_ENTRIES': 5000,
-                    },
-                },
-            }
-        
-            RQ_QUEUES = {
-                'high': {
-                    'USE_REDIS_CACHE': 'redis-cache',
-                },
-                'low': {
-                    'USE_REDIS_CACHE': 'redis-cache',
-                },
-            }
-        
-        Queue Statistics
-        ----------------
-        
-        ``django_rq`` also provides a dashboard to monitor the status of your queues at
-        ``/django-rq/`` (or whatever URL you set in your ``urls.py`` during installation.
-        
-        You can also add a link to this dashboard link in ``/admin`` by adding
-        ``RQ_SHOW_ADMIN_LINK = True`` in ``settings.py``. Be careful though, this will
-        override the default admin template so it may interfere with other apps that
-        modifies the default admin template.
-        
-        These statistics are also available in JSON format via
-        ``/django-rq/stats.json``, which is accessible to staff members.
-        If you need to access this view via other
-        HTTP clients (for monitoring purposes), you can define ``RQ_API_TOKEN`` and access it via
-        ``/django-rq/stats.json/<API_TOKEN>``.
-        
-        .. image::  demo-django-rq-json-dashboard.png
-        
-        Note: Statistics of scheduled jobs display jobs from `RQ built-in scheduler <https://python-rq.org/docs/scheduling/>`__,
-        not optional `RQ scheduler <https://github.com/rq/rq-scheduler>`__.
-        
-        Additionally, these statistics are also accessible from  the command line.
-        
-        .. code-block:: bash
-        
-            python manage.py rqstats
-            python manage.py rqstats --interval=1  # Refreshes every second
-            python manage.py rqstats --json  # Output as JSON
-            python manage.py rqstats --yaml  # Output as YAML
-        
-        .. image:: demo-django-rq-cli-dashboard.gif
-        
-        Configuring Sentry
-        -------------------
-        Django-RQ >= 2.0 uses ``sentry-sdk`` instead of the deprecated ``raven`` library. Sentry
-        should be configured within the Django ``settings.py`` as described in the `Sentry docs <https://docs.sentry.io/platforms/python/django/>`__.
-        
-        You can override the default Django Sentry configuration when running the ``rqworker`` command
-        by passing the ``sentry-dsn`` option:
-        
-        ``./manage.py rqworker --sentry-dsn=https://*****@sentry.io/222222``
-        
-        This will override any existing Django configuration and reinitialise Sentry,
-        setting the following Sentry options:
-        
-        .. code-block:: python
-        
-            {
-                'debug': options.get('sentry_debug'),
-                'ca_certs': options.get('sentry_ca_certs'),
-                'integrations': [RedisIntegration(), RqIntegration(), DjangoIntegration()]
-            }
-        
-        
-        Configuring Logging
-        -------------------
-        
-        RQ uses Python's ``logging``, this means you can easily configure ``rqworker``'s logging mechanism in django's
-        ``settings.py``. For example:
-        
-        .. code-block:: python
-        
-            LOGGING = {
-                "version": 1,
-                "disable_existing_loggers": False,
-                "formatters": {
-                    "rq_console": {
-                        "format": "%(asctime)s %(message)s",
-                        "datefmt": "%H:%M:%S",
-                    },
-                },
-                "handlers": {
-                    "rq_console": {
-                        "level": "DEBUG",
-                        "class": "rq.logutils.ColorizingStreamHandler",
-                        "formatter": "rq_console",
-                        "exclude": ["%(asctime)s"],
-                    },
-                    # If you use sentry for logging
-                    'sentry': {
-                        'level': 'ERROR',
-                        'class': 'raven.contrib.django.handlers.SentryHandler',
-                    },
-                },
-                'loggers': {
-                    "rq.worker": {
-                        "handlers": ["rq_console", "sentry"],
-                        "level": "DEBUG"
-                    },
-                }
-            }
-        
-        Note: error logging to Sentry is known to be unreliable with RQ when using async
-        transports (the default transport). Please configure ``Raven`` to use
-        ``sync+https://`` or ``requests+https://`` transport in ``settings.py``:
-        
-        .. code-block:: python
-        
-            RAVEN_CONFIG = {
-                'dsn': 'sync+https://public:secret@example.com/1',
-            }
-        
-        For more info, refer to `Raven's documentation <http://raven.readthedocs.org/>`__.
-        
-        Custom Queue Classes
-        --------------------
-        
-        By default, every queue will use ``DjangoRQ`` class. If you want to use a custom queue class, you can do so
-        by adding a ``QUEUE_CLASS`` option on a per queue basis in ``RQ_QUEUES``:
-        
-        .. code-block:: python
-        
-            RQ_QUEUES = {
-                'default': {
-                    'HOST': 'localhost',
-                    'PORT': 6379,
-                    'DB': 0,
-                    'QUEUE_CLASS': 'module.path.CustomClass',
-                }
-            }
-        
-        or you can specify ``DjangoRQ`` to use a custom class for all your queues in ``RQ`` settings:
-        
-        .. code-block:: python
-        
-            RQ = {
-                'QUEUE_CLASS': 'module.path.CustomClass',
-            }
-        
-        Custom queue classes should inherit from ``django_rq.queues.DjangoRQ``.
-        
-        If you are using more than one queue class (not recommended), be sure to only run workers
-        on queues with same queue class. For example if you have two queues defined in ``RQ_QUEUES`` and
-        one has custom class specified, you would have to run at least two separate workers for each
-        queue.
-        
-        Custom Job and Worker Classes
-        -----------------------------
-        
-        Similarly to custom queue classes, global custom job and worker classes can be configured using
-        ``JOB_CLASS`` and ``WORKER_CLASS`` settings:
-        
-        .. code-block:: python
-        
-            RQ = {
-                'JOB_CLASS': 'module.path.CustomJobClass',
-                'WORKER_CLASS': 'module.path.CustomWorkerClass',
-            }
-        
-        Custom job class should inherit from ``rq.job.Job``. It will be used for all jobs
-        if configured.
-        
-        Custom worker class should inherit from ``rq.worker.Worker``. It will be used for running
-        all workers unless overridden by ``rqworker`` management command ``worker-class`` option.
-        
-        Testing Tip
-        -----------
-        
-        For an easier testing process, you can run a worker synchronously this way:
-        
-        .. code-block:: python
-        
-            from django.test import TestCase
-            from django_rq import get_worker
-        
-            class MyTest(TestCase):
-                def test_something_that_creates_jobs(self):
-                    ...                      # Stuff that init jobs.
-                    get_worker().work(burst=True)  # Processes all jobs then stop.
-                    ...                      # Asserts that the job stuff is done.
-        
-        Synchronous Mode
-        ----------------
-        
-        You can set the option ``ASYNC`` to ``False`` to make synchronous operation the
-        default for a given queue. This will cause jobs to execute immediately and on
-        the same thread as they are dispatched, which is useful for testing and
-        debugging. For example, you might add the following after you queue
-        configuration in your settings file:
-        
-        .. code-block:: python
-        
-            # ... Logic to set DEBUG and TESTING settings to True or False ...
-        
-            # ... Regular RQ_QUEUES setup code ...
-        
-            if DEBUG or TESTING:
-                for queueConfig in RQ_QUEUES.values():
-                    queueConfig['ASYNC'] = False
-        
-        Note that setting the ``is_async`` parameter explicitly when calling ``get_queue``
-        will override this setting.
-        
-        =============
-        Running Tests
-        =============
-        
-        To run ``django_rq``'s test suite::
-        
-            `which django-admin` test django_rq --settings=django_rq.tests.settings --pythonpath=.
-        
-        ===================
-        Deploying on Ubuntu
-        ===================
-        
-        Create an rqworker service that runs the high, default, and low queues.
-        
-        sudo vi /etc/systemd/system/rqworker.service
-        
-        .. code-block:: bash
-        
-            [Unit]
-            Description=Django-RQ Worker
-            After=network.target
-        
-            [Service]
-            WorkingDirectory=<<path_to_your_project_folder>>
-            ExecStart=/home/ubuntu/.virtualenv/<<your_virtualenv>>/bin/python \
-                <<path_to_your_project_folder>>/manage.py \
-                rqworker high default low
-        
-            [Install]
-            WantedBy=multi-user.target
-        
-        Enable and start the service
-        
-        .. code-block:: bash
-        
-            sudo systemctl enable rqworker
-            sudo systemctl start rqworker
-        
-        ===================
-        Deploying on Heroku
-        ===================
-        
-        Add `django-rq` to your `requirements.txt` file with:
-        
-        .. code-block:: bash
-        
-            pip freeze > requirements.txt
-        
-        Update your `Procfile` to:
-        
-        .. code-block:: bash
-        
-            web: gunicorn --pythonpath="$PWD/your_app_name" config.wsgi:application
-        
-            worker: python your_app_name/manage.py rqworker high default low
-        
-        Commit and re-deploy. Then add your new worker with:
-        
-        .. code-block:: bash
-        
-            heroku scale worker=1
-        
-        =========
-        Changelog
-        =========
-        
-        See `CHANGELOG.md <https://github.com/rq/django-rq/blob/master/CHANGELOG.md>`__.
-        
-        
-        .. |Build Status| image:: https://secure.travis-ci.org/rq/django-rq.svg?branch=master
-           :target: https://travis-ci.org/rq/django-rq
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -592,7 +20,579 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: Sentry
 Provides-Extra: testing
+License-File: LICENSE.txt
+
+=========
+Django-RQ
+=========
+
+|Build Status|
+
+Django integration with `RQ <https://github.com/nvie/rq>`__, a `Redis <http://redis.io/>`__
+based Python queuing library. `Django-RQ <https://github.com/rq/django-rq>`__ is a
+simple app that allows you to configure your queues in django's ``settings.py``
+and easily use them in your project.
+
+=================
+Support Django-RQ
+=================
+
+If you find ``django-rq`` useful, please consider supporting its development via `Tidelift <https://tidelift.com/subscription/pkg/pypi-django_rq?utm_source=pypi-django-rq&utm_medium=referral&utm_campaign=readme>`_.
+
+============
+Requirements
+============
+
+* `Django <https://www.djangoproject.com/>`__ (2.0+)
+* `RQ <https://github.com/nvie/rq>`__
+
+============
+Installation
+============
+
+* Install ``django-rq`` (or `download from PyPI <http://pypi.python.org/pypi/django-rq>`__):
+
+.. code-block:: python
+
+    pip install django-rq
+
+* Add ``django_rq`` to ``INSTALLED_APPS`` in ``settings.py``:
+
+.. code-block:: python
+
+    INSTALLED_APPS = (
+        # other apps
+        "django_rq",
+    )
+
+* Configure your queues in django's ``settings.py``:
+
+.. code-block:: python
+
+    RQ_QUEUES = {
+        'default': {
+            'HOST': 'localhost',
+            'PORT': 6379,
+            'DB': 0,
+            'USERNAME': 'some-user',
+            'PASSWORD': 'some-password',
+            'DEFAULT_TIMEOUT': 360,
+            'REDIS_CLIENT_KWARGS': {    # Eventual additional Redis connection arguments
+                'ssl_cert_reqs': None,
+            },
+        },
+        'with-sentinel': {
+            'SENTINELS': [('localhost', 26736), ('localhost', 26737)],
+            'MASTER_NAME': 'redismaster',
+            'DB': 0,
+            # Redis username/password
+            'USERNAME': 'redis-user',
+            'PASSWORD': 'secret',
+            'SOCKET_TIMEOUT': 0.3,
+            'CONNECTION_KWARGS': {  # Eventual additional Redis connection arguments
+                'ssl': True
+            }
+            'SENTINEL_KWARGS': {    # Eventual Sentinel connection arguments
+                # If Sentinel also has auth, username/password can be passed here
+                'username': 'sentinel-user',
+                'password': 'secret',
+            },
+        },
+        'high': {
+            'URL': os.getenv('REDISTOGO_URL', 'redis://localhost:6379/0'), # If you're on Heroku
+            'DEFAULT_TIMEOUT': 500,
+        },
+        'low': {
+            'HOST': 'localhost',
+            'PORT': 6379,
+            'DB': 0,
+        }
+    }
+
+    RQ_EXCEPTION_HANDLERS = ['path.to.my.handler'] # If you need custom exception handlers
+
+* Include ``django_rq.urls`` in your ``urls.py``:
+
+.. code-block:: python
+
+    urlpatterns += [
+        path('django-rq/', include('django_rq.urls'))
+    ]
+
+=====
+Usage
+=====
+
+Putting jobs in the queue
+-------------------------
+
+`Django-RQ` allows you to easily put jobs into any of the queues defined in
+``settings.py``. It comes with a few utility functions:
+
+* ``enqueue`` - push a job to the ``default`` queue:
+
+.. code-block:: python
+
+    import django_rq
+    django_rq.enqueue(func, foo, bar=baz)
+
+* ``get_queue`` - returns an ``Queue`` instance.
+
+.. code-block:: python
+
+    import django_rq
+    queue = django_rq.get_queue('high')
+    queue.enqueue(func, foo, bar=baz)
+
+In addition to ``name`` argument, ``get_queue`` also accepts ``default_timeout``,
+``is_async``, ``autocommit``, ``connection`` and ``queue_class`` arguments. For example:
+
+.. code-block:: python
+
+    queue = django_rq.get_queue('default', autocommit=True, is_async=True, default_timeout=360)
+    queue.enqueue(func, foo, bar=baz)
+
+You can provide your own singleton Redis connection object to this function so that it will not
+create a new connection object for each queue definition. This will help you limit
+number of connections to Redis server. For example:
+
+.. code-block:: python
+
+    import django_rq
+    import redis
+    redis_cursor = redis.StrictRedis(host='', port='', db='', password='')
+    high_queue = django_rq.get_queue('high', connection=redis_cursor)
+    low_queue = django_rq.get_queue('low', connection=redis_cursor)
+
+
+* ``get_connection`` - accepts a single queue name argument (defaults to "default")
+  and returns a connection to the queue's Redis server:
+
+.. code-block:: python
+
+    import django_rq
+    redis_conn = django_rq.get_connection('high')
+
+* ``get_worker`` - accepts optional queue names and returns a new `RQ`
+  ``Worker`` instance for specified queues (or ``default`` queue):
+
+.. code-block:: python
+
+    import django_rq
+    worker = django_rq.get_worker() # Returns a worker for "default" queue
+    worker.work()
+    worker = django_rq.get_worker('low', 'high') # Returns a worker for "low" and "high"
+
+
+@job decorator
+--------------
+
+To easily turn a callable into an RQ task, you can also use the ``@job``
+decorator that comes with ``django_rq``:
+
+.. code-block:: python
+
+    from django_rq import job
+
+    @job
+    def long_running_func():
+        pass
+    long_running_func.delay() # Enqueue function in "default" queue
+
+    @job('high')
+    def long_running_func():
+        pass
+    long_running_func.delay() # Enqueue function in "high" queue
+
+You can pass in any arguments that RQ's job decorator accepts:
+
+.. code-block:: python
+
+    @job('default', timeout=3600)
+    def long_running_func():
+        pass
+    long_running_func.delay() # Enqueue function with a timeout of 3600 seconds.
+
+It's possible to specify default for ``result_ttl`` decorator keyword argument
+via ``DEFAULT_RESULT_TTL`` setting:
+
+.. code-block:: python
+
+    RQ = {
+        'DEFAULT_RESULT_TTL': 5000,
+    }
+
+With this setting, job decorator will set ``result_ttl`` to 5000 unless it's
+specified explicitly.
+
+
+Running workers
+---------------
+django_rq provides a management command that starts a worker for every queue
+specified as arguments::
+
+    python manage.py rqworker high default low
+
+If you want to run ``rqworker`` in burst mode, you can pass in the ``--burst`` flag::
+
+    python manage.py rqworker high default low --burst
+
+If you need to use custom worker, job or queue classes, it is best to use global settings
+(see `Custom queue classes`_ and `Custom job and worker classes`_). However, it is also possible
+to override such settings with command line options as follows.
+
+To use a custom worker class, you can pass in the ``--worker-class`` flag
+with the path to your worker::
+
+    python manage.py rqworker high default low --worker-class 'path.to.GeventWorker'
+
+To use a custom queue class, you can pass in the ``--queue-class`` flag
+with the path to your queue class::
+
+    python manage.py rqworker high default low --queue-class 'path.to.CustomQueue'
+
+To use a custom job class, provide ``--job-class`` flag.
+
+Support for scheduled jobs
+--------------------------
+
+With RQ 1.2.0. you can use `built-in scheduler <https://python-rq.org/docs/scheduling/>`__
+for your jobs. For example:
+
+.. code-block:: python
+
+    from django_rq.queues import get_queue
+    queue = get_queue('default')
+    job = queue.enqueue_at(datetime(2020, 10, 10), func)
+    
+If you are using built-in scheduler you have to start workers with scheduler support::
+
+    python manage.py rqworker --with-scheduler
+
+
+Alternatively you can use `RQ Scheduler <https://github.com/ui/rq-scheduler>`__.
+After install you can also use the ``get_scheduler`` function to return a
+``Scheduler`` instance for queues defined in settings.py's ``RQ_QUEUES``.
+For example:
+
+.. code-block:: python
+
+    import django_rq
+    scheduler = django_rq.get_scheduler('default')
+    job = scheduler.enqueue_at(datetime(2020, 10, 10), func)
+
+You can also use the management command ``rqscheduler`` to start the scheduler::
+
+    python manage.py rqscheduler
+
+
+Support for django-redis and django-redis-cache
+-----------------------------------------------
+
+If you have `django-redis <https://django-redis.readthedocs.org/>`__ or
+`django-redis-cache <https://github.com/sebleier/django-redis-cache/>`__
+installed, you can instruct django_rq to use the same connection information
+from your Redis cache. This has two advantages: it's DRY and it takes advantage
+of any optimization that may be going on in your cache setup (like using
+connection pooling or `Hiredis <https://github.com/redis/hiredis>`__.)
+
+To use configure it, use a dict with the key ``USE_REDIS_CACHE`` pointing to the
+name of the desired cache in your ``RQ_QUEUES`` dict. It goes without saying
+that the chosen cache must exist and use the Redis backend. See your respective
+Redis cache package docs for configuration instructions. It's also important to
+point out that since the django-redis-cache ``ShardedClient`` splits the cache
+over multiple Redis connections, it does not work.
+
+Here is an example settings fragment for `django-redis`:
+
+.. code-block:: python
+
+    CACHES = {
+        'redis-cache': {
+            'BACKEND': 'redis_cache.cache.RedisCache',
+            'LOCATION': 'localhost:6379:1',
+            'OPTIONS': {
+                'CLIENT_CLASS': 'django_redis.client.DefaultClient',
+                'MAX_ENTRIES': 5000,
+            },
+        },
+    }
+
+    RQ_QUEUES = {
+        'high': {
+            'USE_REDIS_CACHE': 'redis-cache',
+        },
+        'low': {
+            'USE_REDIS_CACHE': 'redis-cache',
+        },
+    }
+
+Queue Statistics
+----------------
+
+``django_rq`` also provides a dashboard to monitor the status of your queues at
+``/django-rq/`` (or whatever URL you set in your ``urls.py`` during installation.
+
+You can also add a link to this dashboard link in ``/admin`` by adding
+``RQ_SHOW_ADMIN_LINK = True`` in ``settings.py``. Be careful though, this will
+override the default admin template so it may interfere with other apps that
+modifies the default admin template.
+
+These statistics are also available in JSON format via
+``/django-rq/stats.json``, which is accessible to staff members.
+If you need to access this view via other
+HTTP clients (for monitoring purposes), you can define ``RQ_API_TOKEN`` and access it via
+``/django-rq/stats.json/<API_TOKEN>``.
+
+.. image::  demo-django-rq-json-dashboard.png
+
+Note: Statistics of scheduled jobs display jobs from `RQ built-in scheduler <https://python-rq.org/docs/scheduling/>`__,
+not optional `RQ scheduler <https://github.com/rq/rq-scheduler>`__.
+
+Additionally, these statistics are also accessible from  the command line.
+
+.. code-block:: bash
+
+    python manage.py rqstats
+    python manage.py rqstats --interval=1  # Refreshes every second
+    python manage.py rqstats --json  # Output as JSON
+    python manage.py rqstats --yaml  # Output as YAML
+
+.. image:: demo-django-rq-cli-dashboard.gif
+
+Configuring Sentry
+-------------------
+Django-RQ >= 2.0 uses ``sentry-sdk`` instead of the deprecated ``raven`` library. Sentry
+should be configured within the Django ``settings.py`` as described in the `Sentry docs <https://docs.sentry.io/platforms/python/django/>`__.
+
+You can override the default Django Sentry configuration when running the ``rqworker`` command
+by passing the ``sentry-dsn`` option:
+
+``./manage.py rqworker --sentry-dsn=https://*****@sentry.io/222222``
+
+This will override any existing Django configuration and reinitialise Sentry,
+setting the following Sentry options:
+
+.. code-block:: python
+
+    {
+        'debug': options.get('sentry_debug'),
+        'ca_certs': options.get('sentry_ca_certs'),
+        'integrations': [RedisIntegration(), RqIntegration(), DjangoIntegration()]
+    }
+
+
+Configuring Logging
+-------------------
+
+RQ uses Python's ``logging``, this means you can easily configure ``rqworker``'s logging mechanism in django's
+``settings.py``. For example:
+
+.. code-block:: python
+
+    LOGGING = {
+        "version": 1,
+        "disable_existing_loggers": False,
+        "formatters": {
+            "rq_console": {
+                "format": "%(asctime)s %(message)s",
+                "datefmt": "%H:%M:%S",
+            },
+        },
+        "handlers": {
+            "rq_console": {
+                "level": "DEBUG",
+                "class": "rq.logutils.ColorizingStreamHandler",
+                "formatter": "rq_console",
+                "exclude": ["%(asctime)s"],
+            },
+            # If you use sentry for logging
+            'sentry': {
+                'level': 'ERROR',
+                'class': 'raven.contrib.django.handlers.SentryHandler',
+            },
+        },
+        'loggers': {
+            "rq.worker": {
+                "handlers": ["rq_console", "sentry"],
+                "level": "DEBUG"
+            },
+        }
+    }
+
+Note: error logging to Sentry is known to be unreliable with RQ when using async
+transports (the default transport). Please configure ``Raven`` to use
+``sync+https://`` or ``requests+https://`` transport in ``settings.py``:
+
+.. code-block:: python
+
+    RAVEN_CONFIG = {
+        'dsn': 'sync+https://public:secret@example.com/1',
+    }
+
+For more info, refer to `Raven's documentation <http://raven.readthedocs.org/>`__.
+
+Custom Queue Classes
+--------------------
+
+By default, every queue will use ``DjangoRQ`` class. If you want to use a custom queue class, you can do so
+by adding a ``QUEUE_CLASS`` option on a per queue basis in ``RQ_QUEUES``:
+
+.. code-block:: python
+
+    RQ_QUEUES = {
+        'default': {
+            'HOST': 'localhost',
+            'PORT': 6379,
+            'DB': 0,
+            'QUEUE_CLASS': 'module.path.CustomClass',
+        }
+    }
+
+or you can specify ``DjangoRQ`` to use a custom class for all your queues in ``RQ`` settings:
+
+.. code-block:: python
+
+    RQ = {
+        'QUEUE_CLASS': 'module.path.CustomClass',
+    }
+
+Custom queue classes should inherit from ``django_rq.queues.DjangoRQ``.
+
+If you are using more than one queue class (not recommended), be sure to only run workers
+on queues with same queue class. For example if you have two queues defined in ``RQ_QUEUES`` and
+one has custom class specified, you would have to run at least two separate workers for each
+queue.
+
+Custom Job and Worker Classes
+-----------------------------
+
+Similarly to custom queue classes, global custom job and worker classes can be configured using
+``JOB_CLASS`` and ``WORKER_CLASS`` settings:
+
+.. code-block:: python
+
+    RQ = {
+        'JOB_CLASS': 'module.path.CustomJobClass',
+        'WORKER_CLASS': 'module.path.CustomWorkerClass',
+    }
+
+Custom job class should inherit from ``rq.job.Job``. It will be used for all jobs
+if configured.
+
+Custom worker class should inherit from ``rq.worker.Worker``. It will be used for running
+all workers unless overridden by ``rqworker`` management command ``worker-class`` option.
+
+Testing Tip
+-----------
+
+For an easier testing process, you can run a worker synchronously this way:
+
+.. code-block:: python
+
+    from django.test import TestCase
+    from django_rq import get_worker
+
+    class MyTest(TestCase):
+        def test_something_that_creates_jobs(self):
+            ...                      # Stuff that init jobs.
+            get_worker().work(burst=True)  # Processes all jobs then stop.
+            ...                      # Asserts that the job stuff is done.
+
+Synchronous Mode
+----------------
+
+You can set the option ``ASYNC`` to ``False`` to make synchronous operation the
+default for a given queue. This will cause jobs to execute immediately and on
+the same thread as they are dispatched, which is useful for testing and
+debugging. For example, you might add the following after you queue
+configuration in your settings file:
+
+.. code-block:: python
+
+    # ... Logic to set DEBUG and TESTING settings to True or False ...
+
+    # ... Regular RQ_QUEUES setup code ...
+
+    if DEBUG or TESTING:
+        for queueConfig in RQ_QUEUES.values():
+            queueConfig['ASYNC'] = False
+
+Note that setting the ``is_async`` parameter explicitly when calling ``get_queue``
+will override this setting.
+
+=============
+Running Tests
+=============
+
+To run ``django_rq``'s test suite::
+
+    `which django-admin` test django_rq --settings=django_rq.tests.settings --pythonpath=.
+
+===================
+Deploying on Ubuntu
+===================
+
+Create an rqworker service that runs the high, default, and low queues.
+
+sudo vi /etc/systemd/system/rqworker.service
+
+.. code-block:: bash
+
+    [Unit]
+    Description=Django-RQ Worker
+    After=network.target
+
+    [Service]
+    WorkingDirectory=<<path_to_your_project_folder>>
+    ExecStart=/home/ubuntu/.virtualenv/<<your_virtualenv>>/bin/python \
+        <<path_to_your_project_folder>>/manage.py \
+        rqworker high default low
+
+    [Install]
+    WantedBy=multi-user.target
+
+Enable and start the service
+
+.. code-block:: bash
+
+    sudo systemctl enable rqworker
+    sudo systemctl start rqworker
+
+===================
+Deploying on Heroku
+===================
+
+Add `django-rq` to your `requirements.txt` file with:
+
+.. code-block:: bash
+
+    pip freeze > requirements.txt
+
+Update your `Procfile` to:
+
+.. code-block:: bash
+
+    web: gunicorn --pythonpath="$PWD/your_app_name" config.wsgi:application
+
+    worker: python your_app_name/manage.py rqworker high default low
+
+Commit and re-deploy. Then add your new worker with:
+
+.. code-block:: bash
+
+    heroku scale worker=1
+
+=========
+Changelog
+=========
+
+See `CHANGELOG.md <https://github.com/rq/django-rq/blob/master/CHANGELOG.md>`__.
+
+
+.. |Build Status| image:: https://secure.travis-ci.org/rq/django-rq.svg?branch=master
+   :target: https://travis-ci.org/rq/django-rq
```

### Comparing `django-rq-2.8.0/README.rst` & `django-rq-2.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-rq-2.8.0/django_rq/admin.py` & `django-rq-2.8.1/django_rq/admin.py`

 * *Files identical despite different names*

### Comparing `django-rq-2.8.0/django_rq/decorators.py` & `django-rq-2.8.1/django_rq/decorators.py`

 * *Files identical despite different names*

### Comparing `django-rq-2.8.0/django_rq/jobs.py` & `django-rq-2.8.1/django_rq/jobs.py`

 * *Files identical despite different names*

### Comparing `django-rq-2.8.0/django_rq/management/commands/rqenqueue.py` & `django-rq-2.8.1/django_rq/management/commands/rqenqueue.py`

 * *Files identical despite different names*

### Comparing `django-rq-2.8.0/django_rq/management/commands/rqscheduler.py` & `django-rq-2.8.1/django_rq/management/commands/rqscheduler.py`

 * *Files identical despite different names*

### Comparing `django-rq-2.8.0/django_rq/management/commands/rqstats.py` & `django-rq-2.8.1/django_rq/management/commands/rqstats.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,27 +49,28 @@
         click.echo()
         click.echo("Django RQ CLI Dashboard")
         click.echo()
         self._print_separator()
 
         # Header
         click.echo(
-            """| %-15s|%10s |%10s |%10s |%10s |%10s |""" %
-            ("Name", "Queued", "Active", "Deferred", "Finished", "Workers")
+            """| %-15s|%10s |%10s |%10s |%10s |%10s |%10s |""" %
+            ("Name", "Queued", "Active", "Deferred", "Finished", "Failed", "Workers")
         )
 
         self._print_separator()
 
         # Print every queues in a row
         for queue in statistics["queues"]:
             click.echo(
-                """| %-15s|%10s |%10s |%10s |%10s |%10s |""" %
+                """| %-15s|%10s |%10s |%10s |%10s |%10s |%10s |""" %
                 (queue["name"], queue["jobs"],
                  queue["started_jobs"], queue["deferred_jobs"],
-                 queue["finished_jobs"], queue["workers"])
+                 queue["finished_jobs"],queue["failed_jobs"],
+                 queue["workers"])
             )
 
         self._print_separator()
 
         if self.interval:
             click.echo()
             click.echo("Press 'Ctrl+c' to quit")
@@ -91,15 +92,15 @@
             yaml.Dumper.ignore_aliases = lambda *args: True
             click.echo(yaml.dump(get_statistics(), default_flow_style=False))
             return
 
         self.interval = options.get("interval")
 
         # Arbitrary
-        self.table_width = 78
+        self.table_width = 90
 
         # Do not continuously poll
         if not self.interval:
             self._print_stats_dashboard(get_statistics())
             return
 
         # Abuse clicks to 'live' render CLI dashboard TODO: Use curses instead
```

### Comparing `django-rq-2.8.0/django_rq/management/commands/rqworker.py` & `django-rq-2.8.1/django_rq/management/commands/rqworker.py`

 * *Files identical despite different names*

### Comparing `django-rq-2.8.0/django_rq/migrations/0001_initial.py` & `django-rq-2.8.1/django_rq/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-rq-2.8.0/django_rq/models.py` & `django-rq-2.8.1/django_rq/models.py`

 * *Files identical despite different names*

### Comparing `django-rq-2.8.0/django_rq/queues.py` & `django-rq-2.8.1/django_rq/queues.py`

 * *Files identical despite different names*

### Comparing `django-rq-2.8.0/django_rq/settings.py` & `django-rq-2.8.1/django_rq/settings.py`

 * *Files identical despite different names*

### Comparing `django-rq-2.8.0/django_rq/templates/django_rq/clear_queue.html` & `django-rq-2.8.1/django_rq/templates/django_rq/clear_queue.html`

 * *Files identical despite different names*

### Comparing `django-rq-2.8.0/django_rq/templates/django_rq/confirm_action.html` & `django-rq-2.8.1/django_rq/templates/django_rq/confirm_action.html`

 * *Files identical despite different names*

### Comparing `django-rq-2.8.0/django_rq/templates/django_rq/delete_job.html` & `django-rq-2.8.1/django_rq/templates/django_rq/delete_job.html`

 * *Files identical despite different names*

### Comparing `django-rq-2.8.0/django_rq/templates/django_rq/job_detail.html` & `django-rq-2.8.1/django_rq/templates/django_rq/job_detail.html`

 * *Files 1% similar despite different names*

```diff
@@ -182,14 +182,20 @@
         {% endif %}
 
     </fieldset>
         
 
     <div class="submit-row">
         <p class="deletelink-box"><a href="delete/" class="deletelink">Delete</a></p>
+        {% if job.is_started %}
+            <form method = 'POST' action = "{% url 'rq_stop_job' queue_index job.id %}">
+                {% csrf_token %}
+                <input type="submit" value="Stop" class="deletelink" name="stop">
+            </form>
+        {% endif %}
         {% if job.is_failed %}
             <form method = 'POST' action = "{% url 'rq_requeue_job' queue_index job.id %}">
                 {% csrf_token %}
                 <input type="submit" value="Requeue" class="default" name="requeue">
             </form>
         {% endif %}
         {% if not job.is_queued and not job.is_failed %}
```

#### html2text {}

```diff
@@ -50,15 +50,17 @@
 Exception:
 {% if job.exc_info %}{{ job.exc_info|linebreaks }}{% endif %}
 {% endif %} {% if job.legacy_result %}
 Result:
 {{ job.result }}
 {% endif %}
 Delete
-{% if job.is_failed %}
+{% if job.is_started %}
+{% csrf_token %} [Stop]
+{% endif %} {% if job.is_failed %}
 {% csrf_token %} [Requeue]
 {% endif %} {% if not job.is_queued and not job.is_failed %}
 {% csrf_token %} [Enqueue]
 {% endif %}
 {% for result in job.results %}
 ***** Result {{ result.id }} *****
 Type:
```

### Comparing `django-rq-2.8.0/django_rq/templates/django_rq/jobs.html` & `django-rq-2.8.1/django_rq/templates/django_rq/jobs.html`

 * *Files 7% similar despite different names*

```diff
@@ -50,14 +50,17 @@
                 <label>Actions:
                     <select name="action">
                         <option value="" selected="selected">---------</option>
                         <option value="delete">Delete</option>
                         {% if job_status == 'Failed' %}
                             <option value="requeue">Requeue</option>
                         {% endif %}
+                        {% if job_status == 'Started' %}
+                            <option value="stop">Stop</option>
+                        {% endif %}
                     </select>
                 </label>
                 <button type="submit" class="button" title="Execute selected action" name="index" value="0">Go</button>
             </div>
             <div class="results">
                 <table id="result_list">
                     <thead>
```

### Comparing `django-rq-2.8.0/django_rq/templates/django_rq/requeue_all.html` & `django-rq-2.8.1/django_rq/templates/django_rq/requeue_all.html`

 * *Files identical despite different names*

### Comparing `django-rq-2.8.0/django_rq/templates/django_rq/stats.html` & `django-rq-2.8.1/django_rq/templates/django_rq/stats.html`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 {% block title %}Queues {{ block.super }}{% endblock %}
 
 {% block extrastyle %}
     {{ block.super }}
     <style>table {width: 100%;}</style>
 {% endblock %}
 
-{% block content_title %}<h1>RQ Queues</h1>{% endblock %}
+{% block content_title %}<h1>Queues</h1>{% endblock %}
 
 {% block breadcrumbs %}
     <div class="breadcrumbs">
         <a href="{% url 'admin:index' %}">Home</a> &rsaquo;
         <a href="{% url 'rq_home' %}">Django RQ</a>
     </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 {% extends "admin/base_site.html" %} {% block title %}Queues {{ block.super }}
 {% endblock %} {% block extrastyle %} {{ block.super }}
  {% endblock %} {% block content_title %}
-****** RQ Queues ******
+****** Queues ******
 {% endblock %} {% block breadcrumbs %}
 Home › Django_RQ
 {% endblock %} {% block content %}
 Name       Queued     Oldest Queued Job          Active Jobs        Deferred Jobs       Finished Jobs       Failed Jobs       Scheduled Jobs       Workers       Host                         Port                         DB                         Scheduler PID
            Jobs
 {          {          {                          {                  {                   {                   {                 {                    {             {                            {                            {                          {
 {          {          {                          {                  {                   {                   {                 {                    {             {                            {                            {                          {
```

### Comparing `django-rq-2.8.0/django_rq/templates/django_rq/worker_details.html` & `django-rq-2.8.1/django_rq/templates/django_rq/worker_details.html`

 * *Files identical despite different names*

### Comparing `django-rq-2.8.0/django_rq/templates/django_rq/workers.html` & `django-rq-2.8.1/django_rq/templates/django_rq/workers.html`

 * *Files identical despite different names*

### Comparing `django-rq-2.8.0/django_rq/templatetags/django_rq.py` & `django-rq-2.8.1/django_rq/templatetags/django_rq.py`

 * *Files identical despite different names*

### Comparing `django-rq-2.8.0/django_rq/tests/settings.py` & `django-rq-2.8.1/django_rq/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-rq-2.8.0/django_rq/tests/test_views.py` & `django-rq-2.8.1/django_rq/tests/test_views.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import uuid
 from datetime import datetime
 from unittest.mock import PropertyMock, patch
 
+
 from django.contrib.auth.models import User
 from django.test import TestCase, override_settings
 from django.test.client import Client
 from django.urls import reverse
 from rq.job import Job, JobStatus
 from rq.registry import (
     DeferredJobRegistry,
@@ -358,7 +359,39 @@
                 self.assertNotIn('"error": true', response.content.decode('utf-8'))
 
                 # Wrong token
                 response = self.client.get(reverse('rq_home_json', args=["wrong_token"]))
                 self.assertEqual(response.status_code, 200)
                 self.assertNotIn("name", response.content.decode('utf-8'))
                 self.assertIn('"error": true', response.content.decode('utf-8'))
+
+    def test_action_stop_jobs(self):
+        queue = get_queue('django_rq_test')
+        queue_index = get_queue_index('django_rq_test')
+
+        # Enqueue some jobs
+        job_ids, jobs = [], []
+        worker = get_worker('django_rq_test')
+        for _ in range(3):
+            job = queue.enqueue(access_self)
+            job_ids.append(job.id)
+            jobs.append(job)
+            worker.prepare_job_execution(job)
+
+        # Check if the jobs are started
+        for job_id in job_ids:
+            job = Job.fetch(job_id, connection=queue.connection)
+            self.assertEqual(job.get_status(), JobStatus.STARTED)
+
+        # Stop those jobs using the view
+        started_job_registry = StartedJobRegistry(queue.name, connection=queue.connection)
+        self.assertEqual(len(started_job_registry), len(job_ids))
+        self.client.post(reverse('rq_actions', args=[queue_index]), {'action': 'stop', 'job_ids': job_ids})
+        for job in jobs:
+            worker.monitor_work_horse(job, queue)  # Sets the job as Failed and removes from Started
+        self.assertEqual(len(started_job_registry), 0)
+
+        canceled_job_registry = FailedJobRegistry(queue.name, connection=queue.connection)
+        self.assertEqual(len(canceled_job_registry), len(job_ids))
+
+        for job_id in job_ids:
+            self.assertIn(job_id, canceled_job_registry)
```

### Comparing `django-rq-2.8.0/django_rq/tests/tests.py` & `django-rq-2.8.1/django_rq/tests/tests.py`

 * *Files identical despite different names*

### Comparing `django-rq-2.8.0/django_rq/tests/utils.py` & `django-rq-2.8.1/django_rq/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django-rq-2.8.0/django_rq/thread_queue.py` & `django-rq-2.8.1/django_rq/thread_queue.py`

 * *Files identical despite different names*

### Comparing `django-rq-2.8.0/django_rq/urls.py` & `django-rq-2.8.1/django_rq/urls.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,8 +25,11 @@
         r'^queues/(?P<queue_index>[\d]+)/(?P<job_id>[^/]+)/requeue/$',
         views.requeue_job_view,
         name='rq_requeue_job',
     ),
     re_path(
         r'^queues/(?P<queue_index>[\d]+)/(?P<job_id>[^/]+)/enqueue/$', views.enqueue_job, name='rq_enqueue_job'
     ),
+    re_path(
+        r'^queues/(?P<queue_index>[\d]+)/(?P<job_id>[^/]+)/stop/$', views.stop_job, name='rq_stop_job'
+    ),
 ]
```

### Comparing `django-rq-2.8.0/django_rq/utils.py` & `django-rq-2.8.1/django_rq/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
     DeferredJobRegistry,
     FailedJobRegistry,
     FinishedJobRegistry,
     ScheduledJobRegistry,
     StartedJobRegistry,
     clean_registries,
 )
+from rq.command import send_stop_job_command
 from rq.worker import Worker
 from rq.worker_registration import clean_worker_registry
 
 
 from .queues import get_connection, get_queue_by_index, get_scheduler
 from .settings import QUEUES_LIST
 from .templatetags.django_rq import to_localtime
@@ -102,7 +103,20 @@
         if job is None:
             if registry:
                 registry.remove(job_ids[i])
         else:
             valid_jobs.append(job)
 
     return valid_jobs
+
+def stop_jobs(queue, job_ids):
+    job_ids = job_ids if isinstance(job_ids, (list, tuple)) else [job_ids]
+    stopped_job_ids = []
+    failed_to_stop_job_ids = []
+    for job_id in job_ids:
+        try:
+            send_stop_job_command(queue.connection, job_id)
+        except Exception:
+            failed_to_stop_job_ids.append(job_id)
+            continue
+        stopped_job_ids.append(job_id)
+    return stopped_job_ids, failed_to_stop_job_ids
```

### Comparing `django-rq-2.8.0/django_rq/views.py` & `django-rq-2.8.1/django_rq/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,32 +4,34 @@
 
 from django.contrib import admin, messages
 from django.contrib.admin.views.decorators import staff_member_required
 from django.http import Http404, JsonResponse
 from django.shortcuts import redirect, render
 from django.urls import reverse
 from django.views.decorators.cache import never_cache
+from django.views.decorators.http import require_POST
 
 from redis.exceptions import ResponseError
 from rq import requeue_job
 from rq.exceptions import NoSuchJobError
 from rq.job import Job, JobStatus
 from rq.registry import (
     DeferredJobRegistry,
     FailedJobRegistry,
     FinishedJobRegistry,
     ScheduledJobRegistry,
     StartedJobRegistry,
 )
 from rq.worker import Worker
 from rq.worker_registration import clean_worker_registry
+from rq.command import send_stop_job_command
 
 from .queues import get_queue_by_index
 from .settings import API_TOKEN
-from .utils import get_statistics, get_jobs
+from .utils import get_statistics, get_jobs, stop_jobs
 
 
 @never_cache
 @staff_member_required
 def stats(request):
     context_data = {**admin.site.each_context(request), **get_statistics(run_maintenance_tasks=True)}
     return render(request, 'django_rq/stats.html', context_data)
@@ -489,14 +491,20 @@
                     queue.connection.lrem(queue.key, 0, job.id)
                     job.delete()
                 messages.info(request, 'You have successfully deleted %s jobs!' % len(job_ids))
             elif request.POST['action'] == 'requeue':
                 for job_id in job_ids:
                     requeue_job(job_id, connection=queue.connection)
                 messages.info(request, 'You have successfully requeued %d  jobs!' % len(job_ids))
+            elif request.POST['action'] == 'stop':
+                stopped, failed_to_stop = stop_jobs(queue, job_ids)
+                if len(stopped) >0 :
+                    messages.info(request, 'You have successfully stopped %d jobs!' % len(stopped))
+                if len(failed_to_stop) >0 :
+                    messages.error(request, '%d jobs failed to stop!' % len(failed_to_stop))
 
     return redirect(next_url)
 
 
 @never_cache
 @staff_member_required
 def enqueue_job(request, queue_index, job_id):
@@ -530,7 +538,23 @@
     context_data = {
         **admin.site.each_context(request),
         'queue_index': queue_index,
         'job': job,
         'queue': queue,
     }
     return render(request, 'django_rq/delete_job.html', context_data)
+
+
+@never_cache
+@staff_member_required
+@require_POST
+def stop_job(request, queue_index, job_id):
+    """Stop started job"""
+    queue_index = int(queue_index)
+    queue = get_queue_by_index(queue_index)
+    stopped, _ = stop_jobs(queue, job_id)
+    if len(stopped) == 1:
+        messages.info(request, 'You have successfully stopped %s' % job_id)
+        return redirect('rq_job_detail', queue_index, job_id)
+    else:
+        messages.error(request, 'Failed to stop %s' % job_id)
+        return redirect('rq_job_detail', queue_index, job_id)
```

### Comparing `django-rq-2.8.0/django_rq/workers.py` & `django-rq-2.8.1/django_rq/workers.py`

 * *Files identical despite different names*

### Comparing `django-rq-2.8.0/django_rq.egg-info/PKG-INFO` & `django-rq-2.8.1/django_rq.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,587 +1,15 @@
 Metadata-Version: 2.1
 Name: django-rq
-Version: 2.8.0
+Version: 2.8.1
 Summary: An app that provides django integration for RQ (Redis Queue)
 Home-page: https://github.com/rq/django-rq
 Author: Selwin Ong
 Author-email: selwin.ong@gmail.com
 License: MIT
-Description: =========
-        Django-RQ
-        =========
-        
-        |Build Status|
-        
-        Django integration with `RQ <https://github.com/nvie/rq>`__, a `Redis <http://redis.io/>`__
-        based Python queuing library. `Django-RQ <https://github.com/rq/django-rq>`__ is a
-        simple app that allows you to configure your queues in django's ``settings.py``
-        and easily use them in your project.
-        
-        =================
-        Support Django-RQ
-        =================
-        
-        If you find ``django-rq`` useful, please consider supporting its development via `Tidelift <https://tidelift.com/subscription/pkg/pypi-django_rq?utm_source=pypi-django-rq&utm_medium=referral&utm_campaign=readme>`_.
-        
-        ============
-        Requirements
-        ============
-        
-        * `Django <https://www.djangoproject.com/>`__ (2.0+)
-        * `RQ <https://github.com/nvie/rq>`__
-        
-        ============
-        Installation
-        ============
-        
-        * Install ``django-rq`` (or `download from PyPI <http://pypi.python.org/pypi/django-rq>`__):
-        
-        .. code-block:: python
-        
-            pip install django-rq
-        
-        * Add ``django_rq`` to ``INSTALLED_APPS`` in ``settings.py``:
-        
-        .. code-block:: python
-        
-            INSTALLED_APPS = (
-                # other apps
-                "django_rq",
-            )
-        
-        * Configure your queues in django's ``settings.py``:
-        
-        .. code-block:: python
-        
-            RQ_QUEUES = {
-                'default': {
-                    'HOST': 'localhost',
-                    'PORT': 6379,
-                    'DB': 0,
-                    'USERNAME': 'some-user',
-                    'PASSWORD': 'some-password',
-                    'DEFAULT_TIMEOUT': 360,
-                    'REDIS_CLIENT_KWARGS': {    # Eventual additional Redis connection arguments
-                        'ssl_cert_reqs': None,
-                    },
-                },
-                'with-sentinel': {
-                    'SENTINELS': [('localhost', 26736), ('localhost', 26737)],
-                    'MASTER_NAME': 'redismaster',
-                    'DB': 0,
-                    # Redis username/password
-                    'USERNAME': 'redis-user',
-                    'PASSWORD': 'secret',
-                    'SOCKET_TIMEOUT': 0.3,
-                    'CONNECTION_KWARGS': {  # Eventual additional Redis connection arguments
-                        'ssl': True
-                    }
-                    'SENTINEL_KWARGS': {    # Eventual Sentinel connection arguments
-                        # If Sentinel also has auth, username/password can be passed here
-                        'username': 'sentinel-user',
-                        'password': 'secret',
-                    },
-                },
-                'high': {
-                    'URL': os.getenv('REDISTOGO_URL', 'redis://localhost:6379/0'), # If you're on Heroku
-                    'DEFAULT_TIMEOUT': 500,
-                },
-                'low': {
-                    'HOST': 'localhost',
-                    'PORT': 6379,
-                    'DB': 0,
-                }
-            }
-        
-            RQ_EXCEPTION_HANDLERS = ['path.to.my.handler'] # If you need custom exception handlers
-        
-        * Include ``django_rq.urls`` in your ``urls.py``:
-        
-        .. code-block:: python
-        
-            urlpatterns += [
-                path('django-rq/', include('django_rq.urls'))
-            ]
-        
-        =====
-        Usage
-        =====
-        
-        Putting jobs in the queue
-        -------------------------
-        
-        `Django-RQ` allows you to easily put jobs into any of the queues defined in
-        ``settings.py``. It comes with a few utility functions:
-        
-        * ``enqueue`` - push a job to the ``default`` queue:
-        
-        .. code-block:: python
-        
-            import django_rq
-            django_rq.enqueue(func, foo, bar=baz)
-        
-        * ``get_queue`` - returns an ``Queue`` instance.
-        
-        .. code-block:: python
-        
-            import django_rq
-            queue = django_rq.get_queue('high')
-            queue.enqueue(func, foo, bar=baz)
-        
-        In addition to ``name`` argument, ``get_queue`` also accepts ``default_timeout``,
-        ``is_async``, ``autocommit``, ``connection`` and ``queue_class`` arguments. For example:
-        
-        .. code-block:: python
-        
-            queue = django_rq.get_queue('default', autocommit=True, is_async=True, default_timeout=360)
-            queue.enqueue(func, foo, bar=baz)
-        
-        You can provide your own singleton Redis connection object to this function so that it will not
-        create a new connection object for each queue definition. This will help you limit
-        number of connections to Redis server. For example:
-        
-        .. code-block:: python
-        
-            import django_rq
-            import redis
-            redis_cursor = redis.StrictRedis(host='', port='', db='', password='')
-            high_queue = django_rq.get_queue('high', connection=redis_cursor)
-            low_queue = django_rq.get_queue('low', connection=redis_cursor)
-        
-        
-        * ``get_connection`` - accepts a single queue name argument (defaults to "default")
-          and returns a connection to the queue's Redis server:
-        
-        .. code-block:: python
-        
-            import django_rq
-            redis_conn = django_rq.get_connection('high')
-        
-        * ``get_worker`` - accepts optional queue names and returns a new `RQ`
-          ``Worker`` instance for specified queues (or ``default`` queue):
-        
-        .. code-block:: python
-        
-            import django_rq
-            worker = django_rq.get_worker() # Returns a worker for "default" queue
-            worker.work()
-            worker = django_rq.get_worker('low', 'high') # Returns a worker for "low" and "high"
-        
-        
-        @job decorator
-        --------------
-        
-        To easily turn a callable into an RQ task, you can also use the ``@job``
-        decorator that comes with ``django_rq``:
-        
-        .. code-block:: python
-        
-            from django_rq import job
-        
-            @job
-            def long_running_func():
-                pass
-            long_running_func.delay() # Enqueue function in "default" queue
-        
-            @job('high')
-            def long_running_func():
-                pass
-            long_running_func.delay() # Enqueue function in "high" queue
-        
-        You can pass in any arguments that RQ's job decorator accepts:
-        
-        .. code-block:: python
-        
-            @job('default', timeout=3600)
-            def long_running_func():
-                pass
-            long_running_func.delay() # Enqueue function with a timeout of 3600 seconds.
-        
-        It's possible to specify default for ``result_ttl`` decorator keyword argument
-        via ``DEFAULT_RESULT_TTL`` setting:
-        
-        .. code-block:: python
-        
-            RQ = {
-                'DEFAULT_RESULT_TTL': 5000,
-            }
-        
-        With this setting, job decorator will set ``result_ttl`` to 5000 unless it's
-        specified explicitly.
-        
-        
-        Running workers
-        ---------------
-        django_rq provides a management command that starts a worker for every queue
-        specified as arguments::
-        
-            python manage.py rqworker high default low
-        
-        If you want to run ``rqworker`` in burst mode, you can pass in the ``--burst`` flag::
-        
-            python manage.py rqworker high default low --burst
-        
-        If you need to use custom worker, job or queue classes, it is best to use global settings
-        (see `Custom queue classes`_ and `Custom job and worker classes`_). However, it is also possible
-        to override such settings with command line options as follows.
-        
-        To use a custom worker class, you can pass in the ``--worker-class`` flag
-        with the path to your worker::
-        
-            python manage.py rqworker high default low --worker-class 'path.to.GeventWorker'
-        
-        To use a custom queue class, you can pass in the ``--queue-class`` flag
-        with the path to your queue class::
-        
-            python manage.py rqworker high default low --queue-class 'path.to.CustomQueue'
-        
-        To use a custom job class, provide ``--job-class`` flag.
-        
-        Support for scheduled jobs
-        --------------------------
-        
-        With RQ 1.2.0. you can use `built-in scheduler <https://python-rq.org/docs/scheduling/>`__
-        for your jobs. For example:
-        
-        .. code-block:: python
-        
-            from django_rq.queues import get_queue
-            queue = get_queue('default')
-            job = queue.enqueue_at(datetime(2020, 10, 10), func)
-            
-        If you are using built-in scheduler you have to start workers with scheduler support::
-        
-            python manage.py rqworker --with-scheduler
-        
-        
-        Alternatively you can use `RQ Scheduler <https://github.com/ui/rq-scheduler>`__.
-        After install you can also use the ``get_scheduler`` function to return a
-        ``Scheduler`` instance for queues defined in settings.py's ``RQ_QUEUES``.
-        For example:
-        
-        .. code-block:: python
-        
-            import django_rq
-            scheduler = django_rq.get_scheduler('default')
-            job = scheduler.enqueue_at(datetime(2020, 10, 10), func)
-        
-        You can also use the management command ``rqscheduler`` to start the scheduler::
-        
-            python manage.py rqscheduler
-        
-        
-        Support for django-redis and django-redis-cache
-        -----------------------------------------------
-        
-        If you have `django-redis <https://django-redis.readthedocs.org/>`__ or
-        `django-redis-cache <https://github.com/sebleier/django-redis-cache/>`__
-        installed, you can instruct django_rq to use the same connection information
-        from your Redis cache. This has two advantages: it's DRY and it takes advantage
-        of any optimization that may be going on in your cache setup (like using
-        connection pooling or `Hiredis <https://github.com/redis/hiredis>`__.)
-        
-        To use configure it, use a dict with the key ``USE_REDIS_CACHE`` pointing to the
-        name of the desired cache in your ``RQ_QUEUES`` dict. It goes without saying
-        that the chosen cache must exist and use the Redis backend. See your respective
-        Redis cache package docs for configuration instructions. It's also important to
-        point out that since the django-redis-cache ``ShardedClient`` splits the cache
-        over multiple Redis connections, it does not work.
-        
-        Here is an example settings fragment for `django-redis`:
-        
-        .. code-block:: python
-        
-            CACHES = {
-                'redis-cache': {
-                    'BACKEND': 'redis_cache.cache.RedisCache',
-                    'LOCATION': 'localhost:6379:1',
-                    'OPTIONS': {
-                        'CLIENT_CLASS': 'django_redis.client.DefaultClient',
-                        'MAX_ENTRIES': 5000,
-                    },
-                },
-            }
-        
-            RQ_QUEUES = {
-                'high': {
-                    'USE_REDIS_CACHE': 'redis-cache',
-                },
-                'low': {
-                    'USE_REDIS_CACHE': 'redis-cache',
-                },
-            }
-        
-        Queue Statistics
-        ----------------
-        
-        ``django_rq`` also provides a dashboard to monitor the status of your queues at
-        ``/django-rq/`` (or whatever URL you set in your ``urls.py`` during installation.
-        
-        You can also add a link to this dashboard link in ``/admin`` by adding
-        ``RQ_SHOW_ADMIN_LINK = True`` in ``settings.py``. Be careful though, this will
-        override the default admin template so it may interfere with other apps that
-        modifies the default admin template.
-        
-        These statistics are also available in JSON format via
-        ``/django-rq/stats.json``, which is accessible to staff members.
-        If you need to access this view via other
-        HTTP clients (for monitoring purposes), you can define ``RQ_API_TOKEN`` and access it via
-        ``/django-rq/stats.json/<API_TOKEN>``.
-        
-        .. image::  demo-django-rq-json-dashboard.png
-        
-        Note: Statistics of scheduled jobs display jobs from `RQ built-in scheduler <https://python-rq.org/docs/scheduling/>`__,
-        not optional `RQ scheduler <https://github.com/rq/rq-scheduler>`__.
-        
-        Additionally, these statistics are also accessible from  the command line.
-        
-        .. code-block:: bash
-        
-            python manage.py rqstats
-            python manage.py rqstats --interval=1  # Refreshes every second
-            python manage.py rqstats --json  # Output as JSON
-            python manage.py rqstats --yaml  # Output as YAML
-        
-        .. image:: demo-django-rq-cli-dashboard.gif
-        
-        Configuring Sentry
-        -------------------
-        Django-RQ >= 2.0 uses ``sentry-sdk`` instead of the deprecated ``raven`` library. Sentry
-        should be configured within the Django ``settings.py`` as described in the `Sentry docs <https://docs.sentry.io/platforms/python/django/>`__.
-        
-        You can override the default Django Sentry configuration when running the ``rqworker`` command
-        by passing the ``sentry-dsn`` option:
-        
-        ``./manage.py rqworker --sentry-dsn=https://*****@sentry.io/222222``
-        
-        This will override any existing Django configuration and reinitialise Sentry,
-        setting the following Sentry options:
-        
-        .. code-block:: python
-        
-            {
-                'debug': options.get('sentry_debug'),
-                'ca_certs': options.get('sentry_ca_certs'),
-                'integrations': [RedisIntegration(), RqIntegration(), DjangoIntegration()]
-            }
-        
-        
-        Configuring Logging
-        -------------------
-        
-        RQ uses Python's ``logging``, this means you can easily configure ``rqworker``'s logging mechanism in django's
-        ``settings.py``. For example:
-        
-        .. code-block:: python
-        
-            LOGGING = {
-                "version": 1,
-                "disable_existing_loggers": False,
-                "formatters": {
-                    "rq_console": {
-                        "format": "%(asctime)s %(message)s",
-                        "datefmt": "%H:%M:%S",
-                    },
-                },
-                "handlers": {
-                    "rq_console": {
-                        "level": "DEBUG",
-                        "class": "rq.logutils.ColorizingStreamHandler",
-                        "formatter": "rq_console",
-                        "exclude": ["%(asctime)s"],
-                    },
-                    # If you use sentry for logging
-                    'sentry': {
-                        'level': 'ERROR',
-                        'class': 'raven.contrib.django.handlers.SentryHandler',
-                    },
-                },
-                'loggers': {
-                    "rq.worker": {
-                        "handlers": ["rq_console", "sentry"],
-                        "level": "DEBUG"
-                    },
-                }
-            }
-        
-        Note: error logging to Sentry is known to be unreliable with RQ when using async
-        transports (the default transport). Please configure ``Raven`` to use
-        ``sync+https://`` or ``requests+https://`` transport in ``settings.py``:
-        
-        .. code-block:: python
-        
-            RAVEN_CONFIG = {
-                'dsn': 'sync+https://public:secret@example.com/1',
-            }
-        
-        For more info, refer to `Raven's documentation <http://raven.readthedocs.org/>`__.
-        
-        Custom Queue Classes
-        --------------------
-        
-        By default, every queue will use ``DjangoRQ`` class. If you want to use a custom queue class, you can do so
-        by adding a ``QUEUE_CLASS`` option on a per queue basis in ``RQ_QUEUES``:
-        
-        .. code-block:: python
-        
-            RQ_QUEUES = {
-                'default': {
-                    'HOST': 'localhost',
-                    'PORT': 6379,
-                    'DB': 0,
-                    'QUEUE_CLASS': 'module.path.CustomClass',
-                }
-            }
-        
-        or you can specify ``DjangoRQ`` to use a custom class for all your queues in ``RQ`` settings:
-        
-        .. code-block:: python
-        
-            RQ = {
-                'QUEUE_CLASS': 'module.path.CustomClass',
-            }
-        
-        Custom queue classes should inherit from ``django_rq.queues.DjangoRQ``.
-        
-        If you are using more than one queue class (not recommended), be sure to only run workers
-        on queues with same queue class. For example if you have two queues defined in ``RQ_QUEUES`` and
-        one has custom class specified, you would have to run at least two separate workers for each
-        queue.
-        
-        Custom Job and Worker Classes
-        -----------------------------
-        
-        Similarly to custom queue classes, global custom job and worker classes can be configured using
-        ``JOB_CLASS`` and ``WORKER_CLASS`` settings:
-        
-        .. code-block:: python
-        
-            RQ = {
-                'JOB_CLASS': 'module.path.CustomJobClass',
-                'WORKER_CLASS': 'module.path.CustomWorkerClass',
-            }
-        
-        Custom job class should inherit from ``rq.job.Job``. It will be used for all jobs
-        if configured.
-        
-        Custom worker class should inherit from ``rq.worker.Worker``. It will be used for running
-        all workers unless overridden by ``rqworker`` management command ``worker-class`` option.
-        
-        Testing Tip
-        -----------
-        
-        For an easier testing process, you can run a worker synchronously this way:
-        
-        .. code-block:: python
-        
-            from django.test import TestCase
-            from django_rq import get_worker
-        
-            class MyTest(TestCase):
-                def test_something_that_creates_jobs(self):
-                    ...                      # Stuff that init jobs.
-                    get_worker().work(burst=True)  # Processes all jobs then stop.
-                    ...                      # Asserts that the job stuff is done.
-        
-        Synchronous Mode
-        ----------------
-        
-        You can set the option ``ASYNC`` to ``False`` to make synchronous operation the
-        default for a given queue. This will cause jobs to execute immediately and on
-        the same thread as they are dispatched, which is useful for testing and
-        debugging. For example, you might add the following after you queue
-        configuration in your settings file:
-        
-        .. code-block:: python
-        
-            # ... Logic to set DEBUG and TESTING settings to True or False ...
-        
-            # ... Regular RQ_QUEUES setup code ...
-        
-            if DEBUG or TESTING:
-                for queueConfig in RQ_QUEUES.values():
-                    queueConfig['ASYNC'] = False
-        
-        Note that setting the ``is_async`` parameter explicitly when calling ``get_queue``
-        will override this setting.
-        
-        =============
-        Running Tests
-        =============
-        
-        To run ``django_rq``'s test suite::
-        
-            `which django-admin` test django_rq --settings=django_rq.tests.settings --pythonpath=.
-        
-        ===================
-        Deploying on Ubuntu
-        ===================
-        
-        Create an rqworker service that runs the high, default, and low queues.
-        
-        sudo vi /etc/systemd/system/rqworker.service
-        
-        .. code-block:: bash
-        
-            [Unit]
-            Description=Django-RQ Worker
-            After=network.target
-        
-            [Service]
-            WorkingDirectory=<<path_to_your_project_folder>>
-            ExecStart=/home/ubuntu/.virtualenv/<<your_virtualenv>>/bin/python \
-                <<path_to_your_project_folder>>/manage.py \
-                rqworker high default low
-        
-            [Install]
-            WantedBy=multi-user.target
-        
-        Enable and start the service
-        
-        .. code-block:: bash
-        
-            sudo systemctl enable rqworker
-            sudo systemctl start rqworker
-        
-        ===================
-        Deploying on Heroku
-        ===================
-        
-        Add `django-rq` to your `requirements.txt` file with:
-        
-        .. code-block:: bash
-        
-            pip freeze > requirements.txt
-        
-        Update your `Procfile` to:
-        
-        .. code-block:: bash
-        
-            web: gunicorn --pythonpath="$PWD/your_app_name" config.wsgi:application
-        
-            worker: python your_app_name/manage.py rqworker high default low
-        
-        Commit and re-deploy. Then add your new worker with:
-        
-        .. code-block:: bash
-        
-            heroku scale worker=1
-        
-        =========
-        Changelog
-        =========
-        
-        See `CHANGELOG.md <https://github.com/rq/django-rq/blob/master/CHANGELOG.md>`__.
-        
-        
-        .. |Build Status| image:: https://secure.travis-ci.org/rq/django-rq.svg?branch=master
-           :target: https://travis-ci.org/rq/django-rq
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -592,7 +20,579 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: Sentry
 Provides-Extra: testing
+License-File: LICENSE.txt
+
+=========
+Django-RQ
+=========
+
+|Build Status|
+
+Django integration with `RQ <https://github.com/nvie/rq>`__, a `Redis <http://redis.io/>`__
+based Python queuing library. `Django-RQ <https://github.com/rq/django-rq>`__ is a
+simple app that allows you to configure your queues in django's ``settings.py``
+and easily use them in your project.
+
+=================
+Support Django-RQ
+=================
+
+If you find ``django-rq`` useful, please consider supporting its development via `Tidelift <https://tidelift.com/subscription/pkg/pypi-django_rq?utm_source=pypi-django-rq&utm_medium=referral&utm_campaign=readme>`_.
+
+============
+Requirements
+============
+
+* `Django <https://www.djangoproject.com/>`__ (2.0+)
+* `RQ <https://github.com/nvie/rq>`__
+
+============
+Installation
+============
+
+* Install ``django-rq`` (or `download from PyPI <http://pypi.python.org/pypi/django-rq>`__):
+
+.. code-block:: python
+
+    pip install django-rq
+
+* Add ``django_rq`` to ``INSTALLED_APPS`` in ``settings.py``:
+
+.. code-block:: python
+
+    INSTALLED_APPS = (
+        # other apps
+        "django_rq",
+    )
+
+* Configure your queues in django's ``settings.py``:
+
+.. code-block:: python
+
+    RQ_QUEUES = {
+        'default': {
+            'HOST': 'localhost',
+            'PORT': 6379,
+            'DB': 0,
+            'USERNAME': 'some-user',
+            'PASSWORD': 'some-password',
+            'DEFAULT_TIMEOUT': 360,
+            'REDIS_CLIENT_KWARGS': {    # Eventual additional Redis connection arguments
+                'ssl_cert_reqs': None,
+            },
+        },
+        'with-sentinel': {
+            'SENTINELS': [('localhost', 26736), ('localhost', 26737)],
+            'MASTER_NAME': 'redismaster',
+            'DB': 0,
+            # Redis username/password
+            'USERNAME': 'redis-user',
+            'PASSWORD': 'secret',
+            'SOCKET_TIMEOUT': 0.3,
+            'CONNECTION_KWARGS': {  # Eventual additional Redis connection arguments
+                'ssl': True
+            }
+            'SENTINEL_KWARGS': {    # Eventual Sentinel connection arguments
+                # If Sentinel also has auth, username/password can be passed here
+                'username': 'sentinel-user',
+                'password': 'secret',
+            },
+        },
+        'high': {
+            'URL': os.getenv('REDISTOGO_URL', 'redis://localhost:6379/0'), # If you're on Heroku
+            'DEFAULT_TIMEOUT': 500,
+        },
+        'low': {
+            'HOST': 'localhost',
+            'PORT': 6379,
+            'DB': 0,
+        }
+    }
+
+    RQ_EXCEPTION_HANDLERS = ['path.to.my.handler'] # If you need custom exception handlers
+
+* Include ``django_rq.urls`` in your ``urls.py``:
+
+.. code-block:: python
+
+    urlpatterns += [
+        path('django-rq/', include('django_rq.urls'))
+    ]
+
+=====
+Usage
+=====
+
+Putting jobs in the queue
+-------------------------
+
+`Django-RQ` allows you to easily put jobs into any of the queues defined in
+``settings.py``. It comes with a few utility functions:
+
+* ``enqueue`` - push a job to the ``default`` queue:
+
+.. code-block:: python
+
+    import django_rq
+    django_rq.enqueue(func, foo, bar=baz)
+
+* ``get_queue`` - returns an ``Queue`` instance.
+
+.. code-block:: python
+
+    import django_rq
+    queue = django_rq.get_queue('high')
+    queue.enqueue(func, foo, bar=baz)
+
+In addition to ``name`` argument, ``get_queue`` also accepts ``default_timeout``,
+``is_async``, ``autocommit``, ``connection`` and ``queue_class`` arguments. For example:
+
+.. code-block:: python
+
+    queue = django_rq.get_queue('default', autocommit=True, is_async=True, default_timeout=360)
+    queue.enqueue(func, foo, bar=baz)
+
+You can provide your own singleton Redis connection object to this function so that it will not
+create a new connection object for each queue definition. This will help you limit
+number of connections to Redis server. For example:
+
+.. code-block:: python
+
+    import django_rq
+    import redis
+    redis_cursor = redis.StrictRedis(host='', port='', db='', password='')
+    high_queue = django_rq.get_queue('high', connection=redis_cursor)
+    low_queue = django_rq.get_queue('low', connection=redis_cursor)
+
+
+* ``get_connection`` - accepts a single queue name argument (defaults to "default")
+  and returns a connection to the queue's Redis server:
+
+.. code-block:: python
+
+    import django_rq
+    redis_conn = django_rq.get_connection('high')
+
+* ``get_worker`` - accepts optional queue names and returns a new `RQ`
+  ``Worker`` instance for specified queues (or ``default`` queue):
+
+.. code-block:: python
+
+    import django_rq
+    worker = django_rq.get_worker() # Returns a worker for "default" queue
+    worker.work()
+    worker = django_rq.get_worker('low', 'high') # Returns a worker for "low" and "high"
+
+
+@job decorator
+--------------
+
+To easily turn a callable into an RQ task, you can also use the ``@job``
+decorator that comes with ``django_rq``:
+
+.. code-block:: python
+
+    from django_rq import job
+
+    @job
+    def long_running_func():
+        pass
+    long_running_func.delay() # Enqueue function in "default" queue
+
+    @job('high')
+    def long_running_func():
+        pass
+    long_running_func.delay() # Enqueue function in "high" queue
+
+You can pass in any arguments that RQ's job decorator accepts:
+
+.. code-block:: python
+
+    @job('default', timeout=3600)
+    def long_running_func():
+        pass
+    long_running_func.delay() # Enqueue function with a timeout of 3600 seconds.
+
+It's possible to specify default for ``result_ttl`` decorator keyword argument
+via ``DEFAULT_RESULT_TTL`` setting:
+
+.. code-block:: python
+
+    RQ = {
+        'DEFAULT_RESULT_TTL': 5000,
+    }
+
+With this setting, job decorator will set ``result_ttl`` to 5000 unless it's
+specified explicitly.
+
+
+Running workers
+---------------
+django_rq provides a management command that starts a worker for every queue
+specified as arguments::
+
+    python manage.py rqworker high default low
+
+If you want to run ``rqworker`` in burst mode, you can pass in the ``--burst`` flag::
+
+    python manage.py rqworker high default low --burst
+
+If you need to use custom worker, job or queue classes, it is best to use global settings
+(see `Custom queue classes`_ and `Custom job and worker classes`_). However, it is also possible
+to override such settings with command line options as follows.
+
+To use a custom worker class, you can pass in the ``--worker-class`` flag
+with the path to your worker::
+
+    python manage.py rqworker high default low --worker-class 'path.to.GeventWorker'
+
+To use a custom queue class, you can pass in the ``--queue-class`` flag
+with the path to your queue class::
+
+    python manage.py rqworker high default low --queue-class 'path.to.CustomQueue'
+
+To use a custom job class, provide ``--job-class`` flag.
+
+Support for scheduled jobs
+--------------------------
+
+With RQ 1.2.0. you can use `built-in scheduler <https://python-rq.org/docs/scheduling/>`__
+for your jobs. For example:
+
+.. code-block:: python
+
+    from django_rq.queues import get_queue
+    queue = get_queue('default')
+    job = queue.enqueue_at(datetime(2020, 10, 10), func)
+    
+If you are using built-in scheduler you have to start workers with scheduler support::
+
+    python manage.py rqworker --with-scheduler
+
+
+Alternatively you can use `RQ Scheduler <https://github.com/ui/rq-scheduler>`__.
+After install you can also use the ``get_scheduler`` function to return a
+``Scheduler`` instance for queues defined in settings.py's ``RQ_QUEUES``.
+For example:
+
+.. code-block:: python
+
+    import django_rq
+    scheduler = django_rq.get_scheduler('default')
+    job = scheduler.enqueue_at(datetime(2020, 10, 10), func)
+
+You can also use the management command ``rqscheduler`` to start the scheduler::
+
+    python manage.py rqscheduler
+
+
+Support for django-redis and django-redis-cache
+-----------------------------------------------
+
+If you have `django-redis <https://django-redis.readthedocs.org/>`__ or
+`django-redis-cache <https://github.com/sebleier/django-redis-cache/>`__
+installed, you can instruct django_rq to use the same connection information
+from your Redis cache. This has two advantages: it's DRY and it takes advantage
+of any optimization that may be going on in your cache setup (like using
+connection pooling or `Hiredis <https://github.com/redis/hiredis>`__.)
+
+To use configure it, use a dict with the key ``USE_REDIS_CACHE`` pointing to the
+name of the desired cache in your ``RQ_QUEUES`` dict. It goes without saying
+that the chosen cache must exist and use the Redis backend. See your respective
+Redis cache package docs for configuration instructions. It's also important to
+point out that since the django-redis-cache ``ShardedClient`` splits the cache
+over multiple Redis connections, it does not work.
+
+Here is an example settings fragment for `django-redis`:
+
+.. code-block:: python
+
+    CACHES = {
+        'redis-cache': {
+            'BACKEND': 'redis_cache.cache.RedisCache',
+            'LOCATION': 'localhost:6379:1',
+            'OPTIONS': {
+                'CLIENT_CLASS': 'django_redis.client.DefaultClient',
+                'MAX_ENTRIES': 5000,
+            },
+        },
+    }
+
+    RQ_QUEUES = {
+        'high': {
+            'USE_REDIS_CACHE': 'redis-cache',
+        },
+        'low': {
+            'USE_REDIS_CACHE': 'redis-cache',
+        },
+    }
+
+Queue Statistics
+----------------
+
+``django_rq`` also provides a dashboard to monitor the status of your queues at
+``/django-rq/`` (or whatever URL you set in your ``urls.py`` during installation.
+
+You can also add a link to this dashboard link in ``/admin`` by adding
+``RQ_SHOW_ADMIN_LINK = True`` in ``settings.py``. Be careful though, this will
+override the default admin template so it may interfere with other apps that
+modifies the default admin template.
+
+These statistics are also available in JSON format via
+``/django-rq/stats.json``, which is accessible to staff members.
+If you need to access this view via other
+HTTP clients (for monitoring purposes), you can define ``RQ_API_TOKEN`` and access it via
+``/django-rq/stats.json/<API_TOKEN>``.
+
+.. image::  demo-django-rq-json-dashboard.png
+
+Note: Statistics of scheduled jobs display jobs from `RQ built-in scheduler <https://python-rq.org/docs/scheduling/>`__,
+not optional `RQ scheduler <https://github.com/rq/rq-scheduler>`__.
+
+Additionally, these statistics are also accessible from  the command line.
+
+.. code-block:: bash
+
+    python manage.py rqstats
+    python manage.py rqstats --interval=1  # Refreshes every second
+    python manage.py rqstats --json  # Output as JSON
+    python manage.py rqstats --yaml  # Output as YAML
+
+.. image:: demo-django-rq-cli-dashboard.gif
+
+Configuring Sentry
+-------------------
+Django-RQ >= 2.0 uses ``sentry-sdk`` instead of the deprecated ``raven`` library. Sentry
+should be configured within the Django ``settings.py`` as described in the `Sentry docs <https://docs.sentry.io/platforms/python/django/>`__.
+
+You can override the default Django Sentry configuration when running the ``rqworker`` command
+by passing the ``sentry-dsn`` option:
+
+``./manage.py rqworker --sentry-dsn=https://*****@sentry.io/222222``
+
+This will override any existing Django configuration and reinitialise Sentry,
+setting the following Sentry options:
+
+.. code-block:: python
+
+    {
+        'debug': options.get('sentry_debug'),
+        'ca_certs': options.get('sentry_ca_certs'),
+        'integrations': [RedisIntegration(), RqIntegration(), DjangoIntegration()]
+    }
+
+
+Configuring Logging
+-------------------
+
+RQ uses Python's ``logging``, this means you can easily configure ``rqworker``'s logging mechanism in django's
+``settings.py``. For example:
+
+.. code-block:: python
+
+    LOGGING = {
+        "version": 1,
+        "disable_existing_loggers": False,
+        "formatters": {
+            "rq_console": {
+                "format": "%(asctime)s %(message)s",
+                "datefmt": "%H:%M:%S",
+            },
+        },
+        "handlers": {
+            "rq_console": {
+                "level": "DEBUG",
+                "class": "rq.logutils.ColorizingStreamHandler",
+                "formatter": "rq_console",
+                "exclude": ["%(asctime)s"],
+            },
+            # If you use sentry for logging
+            'sentry': {
+                'level': 'ERROR',
+                'class': 'raven.contrib.django.handlers.SentryHandler',
+            },
+        },
+        'loggers': {
+            "rq.worker": {
+                "handlers": ["rq_console", "sentry"],
+                "level": "DEBUG"
+            },
+        }
+    }
+
+Note: error logging to Sentry is known to be unreliable with RQ when using async
+transports (the default transport). Please configure ``Raven`` to use
+``sync+https://`` or ``requests+https://`` transport in ``settings.py``:
+
+.. code-block:: python
+
+    RAVEN_CONFIG = {
+        'dsn': 'sync+https://public:secret@example.com/1',
+    }
+
+For more info, refer to `Raven's documentation <http://raven.readthedocs.org/>`__.
+
+Custom Queue Classes
+--------------------
+
+By default, every queue will use ``DjangoRQ`` class. If you want to use a custom queue class, you can do so
+by adding a ``QUEUE_CLASS`` option on a per queue basis in ``RQ_QUEUES``:
+
+.. code-block:: python
+
+    RQ_QUEUES = {
+        'default': {
+            'HOST': 'localhost',
+            'PORT': 6379,
+            'DB': 0,
+            'QUEUE_CLASS': 'module.path.CustomClass',
+        }
+    }
+
+or you can specify ``DjangoRQ`` to use a custom class for all your queues in ``RQ`` settings:
+
+.. code-block:: python
+
+    RQ = {
+        'QUEUE_CLASS': 'module.path.CustomClass',
+    }
+
+Custom queue classes should inherit from ``django_rq.queues.DjangoRQ``.
+
+If you are using more than one queue class (not recommended), be sure to only run workers
+on queues with same queue class. For example if you have two queues defined in ``RQ_QUEUES`` and
+one has custom class specified, you would have to run at least two separate workers for each
+queue.
+
+Custom Job and Worker Classes
+-----------------------------
+
+Similarly to custom queue classes, global custom job and worker classes can be configured using
+``JOB_CLASS`` and ``WORKER_CLASS`` settings:
+
+.. code-block:: python
+
+    RQ = {
+        'JOB_CLASS': 'module.path.CustomJobClass',
+        'WORKER_CLASS': 'module.path.CustomWorkerClass',
+    }
+
+Custom job class should inherit from ``rq.job.Job``. It will be used for all jobs
+if configured.
+
+Custom worker class should inherit from ``rq.worker.Worker``. It will be used for running
+all workers unless overridden by ``rqworker`` management command ``worker-class`` option.
+
+Testing Tip
+-----------
+
+For an easier testing process, you can run a worker synchronously this way:
+
+.. code-block:: python
+
+    from django.test import TestCase
+    from django_rq import get_worker
+
+    class MyTest(TestCase):
+        def test_something_that_creates_jobs(self):
+            ...                      # Stuff that init jobs.
+            get_worker().work(burst=True)  # Processes all jobs then stop.
+            ...                      # Asserts that the job stuff is done.
+
+Synchronous Mode
+----------------
+
+You can set the option ``ASYNC`` to ``False`` to make synchronous operation the
+default for a given queue. This will cause jobs to execute immediately and on
+the same thread as they are dispatched, which is useful for testing and
+debugging. For example, you might add the following after you queue
+configuration in your settings file:
+
+.. code-block:: python
+
+    # ... Logic to set DEBUG and TESTING settings to True or False ...
+
+    # ... Regular RQ_QUEUES setup code ...
+
+    if DEBUG or TESTING:
+        for queueConfig in RQ_QUEUES.values():
+            queueConfig['ASYNC'] = False
+
+Note that setting the ``is_async`` parameter explicitly when calling ``get_queue``
+will override this setting.
+
+=============
+Running Tests
+=============
+
+To run ``django_rq``'s test suite::
+
+    `which django-admin` test django_rq --settings=django_rq.tests.settings --pythonpath=.
+
+===================
+Deploying on Ubuntu
+===================
+
+Create an rqworker service that runs the high, default, and low queues.
+
+sudo vi /etc/systemd/system/rqworker.service
+
+.. code-block:: bash
+
+    [Unit]
+    Description=Django-RQ Worker
+    After=network.target
+
+    [Service]
+    WorkingDirectory=<<path_to_your_project_folder>>
+    ExecStart=/home/ubuntu/.virtualenv/<<your_virtualenv>>/bin/python \
+        <<path_to_your_project_folder>>/manage.py \
+        rqworker high default low
+
+    [Install]
+    WantedBy=multi-user.target
+
+Enable and start the service
+
+.. code-block:: bash
+
+    sudo systemctl enable rqworker
+    sudo systemctl start rqworker
+
+===================
+Deploying on Heroku
+===================
+
+Add `django-rq` to your `requirements.txt` file with:
+
+.. code-block:: bash
+
+    pip freeze > requirements.txt
+
+Update your `Procfile` to:
+
+.. code-block:: bash
+
+    web: gunicorn --pythonpath="$PWD/your_app_name" config.wsgi:application
+
+    worker: python your_app_name/manage.py rqworker high default low
+
+Commit and re-deploy. Then add your new worker with:
+
+.. code-block:: bash
+
+    heroku scale worker=1
+
+=========
+Changelog
+=========
+
+See `CHANGELOG.md <https://github.com/rq/django-rq/blob/master/CHANGELOG.md>`__.
+
+
+.. |Build Status| image:: https://secure.travis-ci.org/rq/django-rq.svg?branch=master
+   :target: https://travis-ci.org/rq/django-rq
```

### Comparing `django-rq-2.8.0/django_rq.egg-info/SOURCES.txt` & `django-rq-2.8.1/django_rq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-rq-2.8.0/setup.py` & `django-rq-2.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 setup(
     name='django-rq',
-    version='2.8.0',
+    version='2.8.1',
     author='Selwin Ong',
     author_email='selwin.ong@gmail.com',
     packages=['django_rq'],
     url='https://github.com/rq/django-rq',
     license='MIT',
     description='An app that provides django integration for RQ (Redis Queue)',
     long_description=open('README.rst').read(),
     zip_safe=False,
     include_package_data=True,
     package_data={'': ['README.rst']},
-    install_requires=['django>=2.0', 'rq>=1.2', 'redis>=3'],
+    install_requires=['django>=2.0', 'rq>=1.14', 'redis>=3'],
     extras_require={
         'Sentry': ['raven>=6.1.0'],
         'testing': ['mock>=2.0.0'],
     },
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: Web Environment',
```

