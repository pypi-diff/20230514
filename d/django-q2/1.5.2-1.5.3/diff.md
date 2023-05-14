# Comparing `tmp/django_q2-1.5.2.tar.gz` & `tmp/django_q2-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_q2-1.5.2.tar", max compression
+gzip compressed data, was "django_q2-1.5.3.tar", max compression
```

## Comparing `django_q2-1.5.2.tar` & `django_q2-1.5.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0    62496 2023-04-12 23:40:17.343231 django_q2-1.5.2/CHANGELOG.md
--rw-r--r--   0        0        0     1088 2023-04-12 23:40:17.343231 django_q2-1.5.2/LICENSE
--rw-r--r--   0        0        0     7073 2023-04-12 23:40:17.343231 django_q2-1.5.2/README.rst
--rw-r--r--   0        0        0      169 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/__init__.py
--rw-r--r--   0        0        0     4547 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/admin.py
--rw-r--r--   0        0        0      289 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/apps.py
--rw-r--r--   0        0        0     5161 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/brokers/__init__.py
--rw-r--r--   0        0        0     3243 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/brokers/aws_sqs.py
--rw-r--r--   0        0        0     1404 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/brokers/ironmq.py
--rw-r--r--   0        0        0     2327 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/brokers/mongo.py
--rw-r--r--   0        0        0     2767 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/brokers/orm.py
--rw-r--r--   0        0        0     1951 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/brokers/redis_broker.py
--rw-r--r--   0        0        0    31002 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/cluster.py
--rw-r--r--   0        0        0     9270 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/conf.py
--rw-r--r--   0        0        0     2711 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/core_signing.py
--rw-r--r--   0        0        0     7253 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/humanhash.py
--rw-r--r--   0        0        0    11421 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    11403 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    11241 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/locale/tr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/management/commands/__init__.py
--rw-r--r--   0        0        0     1283 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/management/commands/qcluster.py
--rw-r--r--   0        0        0     1566 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/management/commands/qinfo.py
--rw-r--r--   0        0        0      889 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/management/commands/qmemory.py
--rw-r--r--   0        0        0      609 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/management/commands/qmonitor.py
--rw-r--r--   0        0        0     4886 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0001_initial.py
--rw-r--r--   0        0        0      629 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0002_auto_20150630_1624.py
--rw-r--r--   0        0        0     1213 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0003_auto_20150708_1326.py
--rw-r--r--   0        0        0      823 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0004_auto_20150710_1043.py
--rw-r--r--   0        0        0      524 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0005_auto_20150718_1506.py
--rw-r--r--   0        0        0     1088 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0006_auto_20150805_1817.py
--rw-r--r--   0        0        0      888 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0007_ormq.py
--rw-r--r--   0        0        0      348 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0008_auto_20160224_1026.py
--rw-r--r--   0        0        0      467 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0009_auto_20171009_0915.py
--rw-r--r--   0        0        0      882 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0010_auto_20200610_0856.py
--rw-r--r--   0        0        0     1113 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0011_auto_20200628_1055.py
--rw-r--r--   0        0        0      603 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0012_auto_20200702_1608.py
--rw-r--r--   0        0        0      389 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0013_task_attempt_count.py
--rw-r--r--   0        0        0      426 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0014_schedule_cluster.py
--rw-r--r--   0        0        0      958 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0015_alter_schedule_schedule_type.py
--rw-r--r--   0        0        0      655 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0016_schedule_intended_date_kwarg.py
--rw-r--r--   0        0        0     1211 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0017_task_cluster_alter.py
--rw-r--r--   0        0        0        0 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/__init__.py
--rw-r--r--   0        0        0    11724 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/models.py
--rw-r--r--   0        0        0    18239 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/monitor.py
--rw-r--r--   0        0        0     2905 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/queues.py
--rw-r--r--   0        0        0     1206 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/signals.py
--rw-r--r--   0        0        0      989 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/signing.py
--rw-r--r--   0        0        0     3632 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/status.py
--rw-r--r--   0        0        0    22128 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/tasks.py
--rw-r--r--   0        0        0        0 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/tests/__init__.py
--rw-r--r--   0        0        0     3101 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/tests/settings.py
--rw-r--r--   0        0        0      712 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/tests/tasks.py
--rw-r--r--   0        0        0     3018 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/tests/test_admin.py
--rw-r--r--   0        0        0     8658 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/tests/test_brokers.py
--rw-r--r--   0        0        0     6812 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/tests/test_cached.py
--rw-r--r--   0        0        0    24279 2023-04-12 23:40:17.347231 django_q2-1.5.2/django_q/tests/test_cluster.py
--rw-r--r--   0        0        0      531 2023-04-12 23:40:17.347231 django_q2-1.5.2/django_q/tests/test_commands.py
--rw-r--r--   0        0        0     1231 2023-04-12 23:40:17.347231 django_q2-1.5.2/django_q/tests/test_monitor.py
--rw-r--r--   0        0        0    14840 2023-04-12 23:40:17.347231 django_q2-1.5.2/django_q/tests/test_scheduler.py
--rw-r--r--   0        0        0        0 2023-04-12 23:40:17.347231 django_q2-1.5.2/django_q/tests/testing_utilities/__init__.py
--rw-r--r--   0        0        0      918 2023-04-12 23:40:17.347231 django_q2-1.5.2/django_q/tests/testing_utilities/multiple_database_routers.py
--rw-r--r--   0        0        0      126 2023-04-12 23:40:17.347231 django_q2-1.5.2/django_q/tests/urls.py
--rw-r--r--   0        0        0     2369 2023-04-12 23:40:17.347231 django_q2-1.5.2/django_q/utils.py
--rw-r--r--   0        0        0     2736 2023-04-12 23:40:17.351232 django_q2-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     9578 1970-01-01 00:00:00.000000 django_q2-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0    62822 2023-05-14 01:24:32.415616 django_q2-1.5.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1088 2023-05-14 01:24:32.415616 django_q2-1.5.3/LICENSE
+-rw-r--r--   0        0        0     7073 2023-05-14 01:24:32.415616 django_q2-1.5.3/README.rst
+-rw-r--r--   0        0        0      169 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/__init__.py
+-rw-r--r--   0        0        0     4547 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/admin.py
+-rw-r--r--   0        0        0      289 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/apps.py
+-rw-r--r--   0        0        0     5161 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/brokers/__init__.py
+-rw-r--r--   0        0        0     3243 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/brokers/aws_sqs.py
+-rw-r--r--   0        0        0     1404 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/brokers/ironmq.py
+-rw-r--r--   0        0        0     2327 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/brokers/mongo.py
+-rw-r--r--   0        0        0     2767 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/brokers/orm.py
+-rw-r--r--   0        0        0     1951 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/brokers/redis_broker.py
+-rw-r--r--   0        0        0    31158 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/cluster.py
+-rw-r--r--   0        0        0     9270 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/conf.py
+-rw-r--r--   0        0        0     2711 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/core_signing.py
+-rw-r--r--   0        0        0     7253 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/humanhash.py
+-rw-r--r--   0        0        0    11421 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    11403 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    11241 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/locale/tr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/management/commands/__init__.py
+-rw-r--r--   0        0        0     1283 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/management/commands/qcluster.py
+-rw-r--r--   0        0        0     1566 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/management/commands/qinfo.py
+-rw-r--r--   0        0        0      889 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/management/commands/qmemory.py
+-rw-r--r--   0        0        0      609 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/management/commands/qmonitor.py
+-rw-r--r--   0        0        0     4886 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/migrations/0001_initial.py
+-rw-r--r--   0        0        0      629 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/migrations/0002_auto_20150630_1624.py
+-rw-r--r--   0        0        0     1213 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/migrations/0003_auto_20150708_1326.py
+-rw-r--r--   0        0        0      823 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/migrations/0004_auto_20150710_1043.py
+-rw-r--r--   0        0        0      524 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/migrations/0005_auto_20150718_1506.py
+-rw-r--r--   0        0        0     1088 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/migrations/0006_auto_20150805_1817.py
+-rw-r--r--   0        0        0      888 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/migrations/0007_ormq.py
+-rw-r--r--   0        0        0      348 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/migrations/0008_auto_20160224_1026.py
+-rw-r--r--   0        0        0      467 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/migrations/0009_auto_20171009_0915.py
+-rw-r--r--   0        0        0      882 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/migrations/0010_auto_20200610_0856.py
+-rw-r--r--   0        0        0     1113 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/migrations/0011_auto_20200628_1055.py
+-rw-r--r--   0        0        0      603 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/migrations/0012_auto_20200702_1608.py
+-rw-r--r--   0        0        0      389 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/migrations/0013_task_attempt_count.py
+-rw-r--r--   0        0        0      426 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/migrations/0014_schedule_cluster.py
+-rw-r--r--   0        0        0      958 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/migrations/0015_alter_schedule_schedule_type.py
+-rw-r--r--   0        0        0      655 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/migrations/0016_schedule_intended_date_kwarg.py
+-rw-r--r--   0        0        0     1211 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/migrations/0017_task_cluster_alter.py
+-rw-r--r--   0        0        0        0 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/migrations/__init__.py
+-rw-r--r--   0        0        0    11724 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/models.py
+-rw-r--r--   0        0        0    18239 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/monitor.py
+-rw-r--r--   0        0        0     2905 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/queues.py
+-rw-r--r--   0        0        0     1246 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/signals.py
+-rw-r--r--   0        0        0      989 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/signing.py
+-rw-r--r--   0        0        0     3632 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/status.py
+-rw-r--r--   0        0        0    22128 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/tasks.py
+-rw-r--r--   0        0        0        0 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/tests/__init__.py
+-rw-r--r--   0        0        0     3101 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/tests/settings.py
+-rw-r--r--   0        0        0      712 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/tests/tasks.py
+-rw-r--r--   0        0        0     3018 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/tests/test_admin.py
+-rw-r--r--   0        0        0     8658 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/tests/test_brokers.py
+-rw-r--r--   0        0        0     6812 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/tests/test_cached.py
+-rw-r--r--   0        0        0    24279 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/tests/test_cluster.py
+-rw-r--r--   0        0        0      531 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/tests/test_commands.py
+-rw-r--r--   0        0        0     1231 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/tests/test_monitor.py
+-rw-r--r--   0        0        0    14840 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/tests/test_scheduler.py
+-rw-r--r--   0        0        0        0 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/tests/testing_utilities/__init__.py
+-rw-r--r--   0        0        0      918 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/tests/testing_utilities/multiple_database_routers.py
+-rw-r--r--   0        0        0      126 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/tests/urls.py
+-rw-r--r--   0        0        0     2369 2023-05-14 01:24:32.415616 django_q2-1.5.3/django_q/utils.py
+-rw-r--r--   0        0        0     2736 2023-05-14 01:24:32.419616 django_q2-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     9578 1970-01-01 00:00:00.000000 django_q2-1.5.3/PKG-INFO
```

### Comparing `django_q2-1.5.2/CHANGELOG.md` & `django_q2-1.5.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 # Changelog
 
 ## [Unreleased](https://github.com/GDay/django-q2/tree/HEAD)
 
+## [v1.5.3](https://github.com/GDay/django-q2/tree/v1.5.3) (2023-05-14)
+
+**Merged pull requests:**
+
+- Add post_spawn signal. https://github.com/django-q2/django-q2/pull/93
+- Post spawn docs https://github.com/django-q2/django-q2/pull/95
+- Make processes identifiable with uuid4 https://github.com/django-q2/django-q2/pull/91
+
 ## [v1.5.2](https://github.com/GDay/django-q2/tree/v1.5.2) (2023-04-13)
 
 **Merged pull requests:**
 
 - Added Django 4.2 to the test matrix, fixed deprecation warning https://github.com/GDay/django-q2/pull/89
 - Updated docs to show support for 4.2
```

### Comparing `django_q2-1.5.2/LICENSE` & `django_q2-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/README.rst` & `django_q2-1.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/admin.py` & `django_q2-1.5.3/django_q/admin.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/brokers/__init__.py` & `django_q2-1.5.3/django_q/brokers/__init__.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/brokers/aws_sqs.py` & `django_q2-1.5.3/django_q/brokers/aws_sqs.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/brokers/ironmq.py` & `django_q2-1.5.3/django_q/brokers/ironmq.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/brokers/mongo.py` & `django_q2-1.5.3/django_q/brokers/mongo.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/brokers/orm.py` & `django_q2-1.5.3/django_q/brokers/orm.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/brokers/redis_broker.py` & `django_q2-1.5.3/django_q/brokers/redis_broker.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/cluster.py` & `django_q2-1.5.3/django_q/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     psutil,
     setproctitle,
     resource,
 )
 from django_q.humanhash import humanize
 from django_q.models import Schedule, Success, Task
 from django_q.queues import Queue
-from django_q.signals import post_execute, pre_execute
+from django_q.signals import post_execute, post_spawn, pre_execute
 from django_q.signing import BadSignature, SignedPackage
 from django_q.status import Stat, Status
 
 from .utils import get_func_repr, localtime
 
 
 class Cluster:
@@ -65,14 +65,15 @@
         if setproctitle:
             setproctitle.setproctitle(f"qcluster {current_process().name} {self.name}")
         # Start Sentinel
         self.stop_event = Event()
         self.start_event = Event()
         self.sentinel = Process(
             target=Sentinel,
+            name=f"Process-{uuid.uuid4().hex}",
             args=(
                 self.stop_event,
                 self.start_event,
                 self.cluster_id,
                 self.broker,
                 self.timeout,
             ),
@@ -192,15 +193,15 @@
                 return Conf.STOPPING
             return Conf.STOPPED
 
     def spawn_process(self, target, *args) -> Process:
         """
         :type target: function or class
         """
-        p = Process(target=target, args=args)
+        p = Process(target=target, args=args, name=f"Process-{uuid.uuid4().hex}")
         p.daemon = True
         if target == worker:
             p.daemon = Conf.DAEMONIZE_WORKERS
             p.timer = args[2]
             self.pool.append(p)
         p.start()
         return p
@@ -477,14 +478,15 @@
     :type timer: multiprocessing.Value
     """
     proc_name = current_process().name
     logger.info(
         _("%(proc_name)s ready for work at %(id)s")
         % {"proc_name": proc_name, "id": current_process().pid}
     )
+    post_spawn.send(sender="django_q", proc_name=proc_name)
     if setproctitle:
         setproctitle.setproctitle(f"qcluster {proc_name} idle")
     task_count = 0
     if timeout is None:
         timeout = -1
     # Start reading the task queue
     for task in iter(task_queue.get, "STOP"):
```

### Comparing `django_q2-1.5.2/django_q/conf.py` & `django_q2-1.5.3/django_q/conf.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/core_signing.py` & `django_q2-1.5.3/django_q/core_signing.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/humanhash.py` & `django_q2-1.5.3/django_q/humanhash.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/locale/de/LC_MESSAGES/django.po` & `django_q2-1.5.3/django_q/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/locale/fr/LC_MESSAGES/django.po` & `django_q2-1.5.3/django_q/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/locale/tr/LC_MESSAGES/django.po` & `django_q2-1.5.3/django_q/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/management/commands/qcluster.py` & `django_q2-1.5.3/django_q/management/commands/qcluster.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/management/commands/qinfo.py` & `django_q2-1.5.3/django_q/management/commands/qinfo.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/management/commands/qmemory.py` & `django_q2-1.5.3/django_q/management/commands/qmemory.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/management/commands/qmonitor.py` & `django_q2-1.5.3/django_q/management/commands/qmonitor.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/migrations/0001_initial.py` & `django_q2-1.5.3/django_q/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/migrations/0002_auto_20150630_1624.py` & `django_q2-1.5.3/django_q/migrations/0002_auto_20150630_1624.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/migrations/0003_auto_20150708_1326.py` & `django_q2-1.5.3/django_q/migrations/0003_auto_20150708_1326.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/migrations/0004_auto_20150710_1043.py` & `django_q2-1.5.3/django_q/migrations/0004_auto_20150710_1043.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/migrations/0005_auto_20150718_1506.py` & `django_q2-1.5.3/django_q/migrations/0005_auto_20150718_1506.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/migrations/0006_auto_20150805_1817.py` & `django_q2-1.5.3/django_q/migrations/0006_auto_20150805_1817.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/migrations/0007_ormq.py` & `django_q2-1.5.3/django_q/migrations/0007_ormq.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/migrations/0010_auto_20200610_0856.py` & `django_q2-1.5.3/django_q/migrations/0010_auto_20200610_0856.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/migrations/0011_auto_20200628_1055.py` & `django_q2-1.5.3/django_q/migrations/0011_auto_20200628_1055.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/migrations/0012_auto_20200702_1608.py` & `django_q2-1.5.3/django_q/migrations/0012_auto_20200702_1608.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/migrations/0015_alter_schedule_schedule_type.py` & `django_q2-1.5.3/django_q/migrations/0015_alter_schedule_schedule_type.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/migrations/0016_schedule_intended_date_kwarg.py` & `django_q2-1.5.3/django_q/migrations/0016_schedule_intended_date_kwarg.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/migrations/0017_task_cluster_alter.py` & `django_q2-1.5.3/django_q/migrations/0017_task_cluster_alter.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/models.py` & `django_q2-1.5.3/django_q/models.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/monitor.py` & `django_q2-1.5.3/django_q/monitor.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/queues.py` & `django_q2-1.5.3/django_q/queues.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/signals.py` & `django_q2-1.5.3/django_q/signals.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,16 @@
             f(instance)
         except Exception as e:
             logger.error(
                 _("return hook %(hook)s failed on [%(name)s] because %(error)s")
                 % {"hook": instance.hook, "name": instance.name, "error": str(e)}
             )
 
+# args: proc_name
+post_spawn = Signal()
 
 # args: task
 pre_enqueue = Signal()
 
 # args: func, task
 pre_execute = Signal()
```

### Comparing `django_q2-1.5.2/django_q/signing.py` & `django_q2-1.5.3/django_q/signing.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/status.py` & `django_q2-1.5.3/django_q/status.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/tasks.py` & `django_q2-1.5.3/django_q/tasks.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/tests/settings.py` & `django_q2-1.5.3/django_q/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/tests/tasks.py` & `django_q2-1.5.3/django_q/tests/tasks.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/tests/test_admin.py` & `django_q2-1.5.3/django_q/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/tests/test_brokers.py` & `django_q2-1.5.3/django_q/tests/test_brokers.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/tests/test_cached.py` & `django_q2-1.5.3/django_q/tests/test_cached.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/tests/test_cluster.py` & `django_q2-1.5.3/django_q/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/tests/test_commands.py` & `django_q2-1.5.3/django_q/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/tests/test_monitor.py` & `django_q2-1.5.3/django_q/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/tests/test_scheduler.py` & `django_q2-1.5.3/django_q/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/tests/testing_utilities/multiple_database_routers.py` & `django_q2-1.5.3/django_q/tests/testing_utilities/multiple_database_routers.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/django_q/utils.py` & `django_q2-1.5.3/django_q/utils.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.2/pyproject.toml` & `django_q2-1.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-q2"
-version = "1.5.2"
+version = "1.5.3"
 packages = [
     { include = "django_q" },
 ]
 description = "A multiprocessing distributed task queue for Django"
 authors = ["Stan Triepels <django-q2@stantriepels.com>", "Ilan Steemers <koed00@gmail.com>"]
 maintainers = ["Stan Triepels <django-q2@stantriepels.com>"]
 license = "MIT"
```

### Comparing `django_q2-1.5.2/PKG-INFO` & `django_q2-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-q2
-Version: 1.5.2
+Version: 1.5.3
 Summary: A multiprocessing distributed task queue for Django
 Home-page: https://django-q2.readthedocs.org
 License: MIT
 Keywords: django,distributed,multiprocessing,queue,scheduler
 Author: Stan Triepels
 Author-email: django-q2@stantriepels.com
 Maintainer: Stan Triepels
```

