# Comparing `tmp/moarc-framework-0.9.5.6.tar.gz` & `tmp/moarc-framework-0.9.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\moarc-framework-0.9.5.6.tar", last modified: Sun May 14 14:38:55 2023, max compression
+gzip compressed data, was "dist\moarc-framework-0.9.5.7.tar", last modified: Sun May 14 14:40:43 2023, max compression
```

## Comparing `moarc-framework-0.9.5.6.tar` & `moarc-framework-0.9.5.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 14:38:55.753257 moarc-framework-0.9.5.6/
--rw-rw-rw-   0        0        0     1596 2022-02-20 16:21:00.000000 moarc-framework-0.9.5.6/LICENSE
--rw-rw-rw-   0        0        0      142 2022-09-13 03:58:24.000000 moarc-framework-0.9.5.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1756 2023-05-14 14:38:55.753257 moarc-framework-0.9.5.6/PKG-INFO
--rw-rw-rw-   0        0        0      609 2022-02-20 16:18:57.000000 moarc-framework-0.9.5.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-14 14:38:55.690257 moarc-framework-0.9.5.6/moarc_framework.egg-info/
--rw-rw-rw-   0        0        0     1756 2023-05-14 14:38:55.000000 moarc-framework-0.9.5.6/moarc_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1428 2023-05-14 14:38:55.000000 moarc-framework-0.9.5.6/moarc_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 14:38:55.000000 moarc-framework-0.9.5.6/moarc_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-05-14 14:38:55.000000 moarc-framework-0.9.5.6/moarc_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-14 14:38:55.000000 moarc-framework-0.9.5.6/moarc_framework.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-14 14:38:55.693257 moarc-framework-0.9.5.6/moarcframework/
--rw-rw-rw-   0        0        0       25 2022-02-20 16:14:26.000000 moarc-framework-0.9.5.6/moarcframework/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:38:55.696260 moarc-framework-0.9.5.6/moarcframework/helpers/
--rw-rw-rw-   0        0        0       25 2022-02-20 03:31:52.000000 moarc-framework-0.9.5.6/moarcframework/helpers/__init__.py
--rw-rw-rw-   0        0        0      200 2022-05-11 22:13:28.000000 moarc-framework-0.9.5.6/moarcframework/helpers/auth.py
--rw-rw-rw-   0        0        0     2314 2022-05-21 15:36:43.000000 moarc-framework-0.9.5.6/moarcframework/helpers/paginator.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:38:55.700258 moarc-framework-0.9.5.6/moarcframework/http/
--rw-rw-rw-   0        0        0       25 2022-02-20 01:02:24.000000 moarc-framework-0.9.5.6/moarcframework/http/__init__.py
--rw-rw-rw-   0        0        0      764 2022-05-18 22:46:28.000000 moarc-framework-0.9.5.6/moarcframework/http/decorators.py
--rw-rw-rw-   0        0        0      191 2022-02-20 15:42:53.000000 moarc-framework-0.9.5.6/moarcframework/http/generic_serializer.py
--rw-rw-rw-   0        0        0     1089 2022-05-25 03:31:33.000000 moarc-framework-0.9.5.6/moarcframework/http/http.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:38:55.701257 moarc-framework-0.9.5.6/moarcframework/management/
--rw-rw-rw-   0        0        0        0 2020-08-29 16:49:19.000000 moarc-framework-0.9.5.6/moarcframework/management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:38:55.705258 moarc-framework-0.9.5.6/moarcframework/management/commands/
--rw-rw-rw-   0        0        0        0 2020-08-29 16:49:19.000000 moarc-framework-0.9.5.6/moarcframework/management/commands/__init__.py
--rw-rw-rw-   0        0        0      511 2020-08-29 16:49:19.000000 moarc-framework-0.9.5.6/moarcframework/management/commands/clean_migrations.py
--rw-rw-rw-   0        0        0      692 2022-02-20 03:39:41.000000 moarc-framework-0.9.5.6/moarcframework/management/commands/refresh_template.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:38:55.707255 moarc-framework-0.9.5.6/moarcframework/middleware/
--rw-rw-rw-   0        0        0       25 2022-02-20 03:32:40.000000 moarc-framework-0.9.5.6/moarcframework/middleware/__init__.py
--rw-rw-rw-   0        0        0     1388 2020-08-29 16:49:21.000000 moarc-framework-0.9.5.6/moarcframework/middleware/thread_local_user_middleware.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:38:55.729258 moarc-framework-0.9.5.6/moarcframework/migrations/
--rw-rw-rw-   0        0        0     9620 2022-05-11 22:37:17.000000 moarc-framework-0.9.5.6/moarcframework/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      598 2022-05-25 02:27:59.000000 moarc-framework-0.9.5.6/moarcframework/migrations/0002_menu_permission.py
--rw-rw-rw-   0        0        0     2078 2023-04-10 03:17:03.000000 moarc-framework-0.9.5.6/moarcframework/migrations/0003_sequence.py
--rw-rw-rw-   0        0        0      755 2023-05-14 14:38:41.000000 moarc-framework-0.9.5.6/moarcframework/migrations/0004_attachment_mimetype_alter_attachment_file.py
--rw-rw-rw-   0        0        0        0 2022-05-11 22:32:56.000000 moarc-framework-0.9.5.6/moarcframework/migrations/__init__.py
--rw-rw-rw-   0        0        0    10949 2023-05-14 14:37:46.000000 moarc-framework-0.9.5.6/moarcframework/models.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:38:55.734258 moarc-framework-0.9.5.6/moarcframework/orm/
--rw-rw-rw-   0        0        0       25 2022-02-20 00:41:47.000000 moarc-framework-0.9.5.6/moarcframework/orm/__init__.py
--rw-rw-rw-   0        0        0     9330 2022-09-11 14:11:40.000000 moarc-framework-0.9.5.6/moarcframework/orm/base_model.py
--rw-rw-rw-   0        0        0     2628 2022-02-20 03:41:43.000000 moarc-framework-0.9.5.6/moarcframework/orm/fields.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:38:55.741257 moarc-framework-0.9.5.6/moarcframework/templatetags/
--rw-rw-rw-   0        0        0       25 2021-12-05 04:03:37.000000 moarc-framework-0.9.5.6/moarcframework/templatetags/__init__.py
--rw-rw-rw-   0        0        0      339 2021-12-23 00:32:40.000000 moarc-framework-0.9.5.6/moarcframework/templatetags/custom_tags.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:38:55.752264 moarc-framework-0.9.5.6/moarcframework/ui/
--rw-rw-rw-   0        0        0       25 2022-02-20 00:41:55.000000 moarc-framework-0.9.5.6/moarcframework/ui/__init__.py
--rw-rw-rw-   0        0        0     4200 2021-12-24 19:18:04.000000 moarc-framework-0.9.5.6/moarcframework/ui/form.html
--rw-rw-rw-   0        0        0     3525 2021-12-24 19:15:05.000000 moarc-framework-0.9.5.6/moarcframework/ui/import.html
--rw-rw-rw-   0        0        0     1921 2021-12-24 19:13:19.000000 moarc-framework-0.9.5.6/moarcframework/ui/table.html
--rw-rw-rw-   0        0        0      968 2022-05-11 17:38:21.000000 moarc-framework-0.9.5.6/moarcframework/urls.py
--rw-rw-rw-   0        0        0      445 2022-05-11 22:59:46.000000 moarc-framework-0.9.5.6/moarcframework/views.py
--rw-rw-rw-   0        0        0        0 2022-02-20 16:22:45.000000 moarc-framework-0.9.5.6/pyproject.toml
--rw-rw-rw-   0        0        0      910 2023-05-14 14:38:55.769257 moarc-framework-0.9.5.6/setup.cfg
--rw-rw-rw-   0        0        0      141 2022-06-09 04:50:44.000000 moarc-framework-0.9.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:40:43.694069 moarc-framework-0.9.5.7/
+-rw-rw-rw-   0        0        0     1596 2022-02-20 16:21:00.000000 moarc-framework-0.9.5.7/LICENSE
+-rw-rw-rw-   0        0        0      142 2022-09-13 03:58:24.000000 moarc-framework-0.9.5.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1756 2023-05-14 14:40:43.694069 moarc-framework-0.9.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2022-02-20 16:18:57.000000 moarc-framework-0.9.5.7/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-14 14:40:43.669074 moarc-framework-0.9.5.7/moarc_framework.egg-info/
+-rw-rw-rw-   0        0        0     1756 2023-05-14 14:40:43.000000 moarc-framework-0.9.5.7/moarc_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1428 2023-05-14 14:40:43.000000 moarc-framework-0.9.5.7/moarc_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 14:40:43.000000 moarc-framework-0.9.5.7/moarc_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-14 14:40:43.000000 moarc-framework-0.9.5.7/moarc_framework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-14 14:40:43.000000 moarc-framework-0.9.5.7/moarc_framework.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 14:40:43.673074 moarc-framework-0.9.5.7/moarcframework/
+-rw-rw-rw-   0        0        0       25 2022-02-20 16:14:26.000000 moarc-framework-0.9.5.7/moarcframework/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:40:43.676061 moarc-framework-0.9.5.7/moarcframework/helpers/
+-rw-rw-rw-   0        0        0       25 2022-02-20 03:31:52.000000 moarc-framework-0.9.5.7/moarcframework/helpers/__init__.py
+-rw-rw-rw-   0        0        0      200 2022-05-11 22:13:28.000000 moarc-framework-0.9.5.7/moarcframework/helpers/auth.py
+-rw-rw-rw-   0        0        0     2314 2022-05-21 15:36:43.000000 moarc-framework-0.9.5.7/moarcframework/helpers/paginator.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:40:43.679062 moarc-framework-0.9.5.7/moarcframework/http/
+-rw-rw-rw-   0        0        0       25 2022-02-20 01:02:24.000000 moarc-framework-0.9.5.7/moarcframework/http/__init__.py
+-rw-rw-rw-   0        0        0      764 2022-05-18 22:46:28.000000 moarc-framework-0.9.5.7/moarcframework/http/decorators.py
+-rw-rw-rw-   0        0        0      191 2022-02-20 15:42:53.000000 moarc-framework-0.9.5.7/moarcframework/http/generic_serializer.py
+-rw-rw-rw-   0        0        0     1089 2022-05-25 03:31:33.000000 moarc-framework-0.9.5.7/moarcframework/http/http.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:40:43.679062 moarc-framework-0.9.5.7/moarcframework/management/
+-rw-rw-rw-   0        0        0        0 2020-08-29 16:49:19.000000 moarc-framework-0.9.5.7/moarcframework/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:40:43.681062 moarc-framework-0.9.5.7/moarcframework/management/commands/
+-rw-rw-rw-   0        0        0        0 2020-08-29 16:49:19.000000 moarc-framework-0.9.5.7/moarcframework/management/commands/__init__.py
+-rw-rw-rw-   0        0        0      511 2020-08-29 16:49:19.000000 moarc-framework-0.9.5.7/moarcframework/management/commands/clean_migrations.py
+-rw-rw-rw-   0        0        0      692 2022-02-20 03:39:41.000000 moarc-framework-0.9.5.7/moarcframework/management/commands/refresh_template.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:40:43.683061 moarc-framework-0.9.5.7/moarcframework/middleware/
+-rw-rw-rw-   0        0        0       25 2022-02-20 03:32:40.000000 moarc-framework-0.9.5.7/moarcframework/middleware/__init__.py
+-rw-rw-rw-   0        0        0     1388 2020-08-29 16:49:21.000000 moarc-framework-0.9.5.7/moarcframework/middleware/thread_local_user_middleware.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:40:43.687063 moarc-framework-0.9.5.7/moarcframework/migrations/
+-rw-rw-rw-   0        0        0     9620 2022-05-11 22:37:17.000000 moarc-framework-0.9.5.7/moarcframework/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      598 2022-05-25 02:27:59.000000 moarc-framework-0.9.5.7/moarcframework/migrations/0002_menu_permission.py
+-rw-rw-rw-   0        0        0     2078 2023-04-10 03:17:03.000000 moarc-framework-0.9.5.7/moarcframework/migrations/0003_sequence.py
+-rw-rw-rw-   0        0        0      686 2023-05-14 14:40:35.000000 moarc-framework-0.9.5.7/moarcframework/migrations/0004_attachment_mimetype_alter_attachment_file.py
+-rw-rw-rw-   0        0        0        0 2022-05-11 22:32:56.000000 moarc-framework-0.9.5.7/moarcframework/migrations/__init__.py
+-rw-rw-rw-   0        0        0    10949 2023-05-14 14:37:46.000000 moarc-framework-0.9.5.7/moarcframework/models.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:40:43.689062 moarc-framework-0.9.5.7/moarcframework/orm/
+-rw-rw-rw-   0        0        0       25 2022-02-20 00:41:47.000000 moarc-framework-0.9.5.7/moarcframework/orm/__init__.py
+-rw-rw-rw-   0        0        0     9330 2022-09-11 14:11:40.000000 moarc-framework-0.9.5.7/moarcframework/orm/base_model.py
+-rw-rw-rw-   0        0        0     2628 2022-02-20 03:41:43.000000 moarc-framework-0.9.5.7/moarcframework/orm/fields.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:40:43.690063 moarc-framework-0.9.5.7/moarcframework/templatetags/
+-rw-rw-rw-   0        0        0       25 2021-12-05 04:03:37.000000 moarc-framework-0.9.5.7/moarcframework/templatetags/__init__.py
+-rw-rw-rw-   0        0        0      339 2021-12-23 00:32:40.000000 moarc-framework-0.9.5.7/moarcframework/templatetags/custom_tags.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:40:43.693062 moarc-framework-0.9.5.7/moarcframework/ui/
+-rw-rw-rw-   0        0        0       25 2022-02-20 00:41:55.000000 moarc-framework-0.9.5.7/moarcframework/ui/__init__.py
+-rw-rw-rw-   0        0        0     4200 2021-12-24 19:18:04.000000 moarc-framework-0.9.5.7/moarcframework/ui/form.html
+-rw-rw-rw-   0        0        0     3525 2021-12-24 19:15:05.000000 moarc-framework-0.9.5.7/moarcframework/ui/import.html
+-rw-rw-rw-   0        0        0     1921 2021-12-24 19:13:19.000000 moarc-framework-0.9.5.7/moarcframework/ui/table.html
+-rw-rw-rw-   0        0        0      968 2022-05-11 17:38:21.000000 moarc-framework-0.9.5.7/moarcframework/urls.py
+-rw-rw-rw-   0        0        0      445 2022-05-11 22:59:46.000000 moarc-framework-0.9.5.7/moarcframework/views.py
+-rw-rw-rw-   0        0        0        0 2022-02-20 16:22:45.000000 moarc-framework-0.9.5.7/pyproject.toml
+-rw-rw-rw-   0        0        0      910 2023-05-14 14:40:43.695063 moarc-framework-0.9.5.7/setup.cfg
+-rw-rw-rw-   0        0        0      141 2022-06-09 04:50:44.000000 moarc-framework-0.9.5.7/setup.py
```

### Comparing `moarc-framework-0.9.5.6/LICENSE` & `moarc-framework-0.9.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.6/PKG-INFO` & `moarc-framework-0.9.5.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moarc-framework
-Version: 0.9.5.6
+Version: 0.9.5.7
 Summary: A Django app Moarc Framework.
 Home-page: https://www.example.com/
 Author: Eduardo Moron
 Author-email: danix799@gmail.com
 License: BSD-3-Clause
 Description: =====
         Moarc Framework
```

### Comparing `moarc-framework-0.9.5.6/README.rst` & `moarc-framework-0.9.5.7/README.rst`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.6/moarc_framework.egg-info/PKG-INFO` & `moarc-framework-0.9.5.7/moarc_framework.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moarc-framework
-Version: 0.9.5.6
+Version: 0.9.5.7
 Summary: A Django app Moarc Framework.
 Home-page: https://www.example.com/
 Author: Eduardo Moron
 Author-email: danix799@gmail.com
 License: BSD-3-Clause
 Description: =====
         Moarc Framework
```

### Comparing `moarc-framework-0.9.5.6/moarc_framework.egg-info/SOURCES.txt` & `moarc-framework-0.9.5.7/moarc_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.6/moarcframework/helpers/paginator.py` & `moarc-framework-0.9.5.7/moarcframework/helpers/paginator.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.6/moarcframework/http/decorators.py` & `moarc-framework-0.9.5.7/moarcframework/http/decorators.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.6/moarcframework/http/http.py` & `moarc-framework-0.9.5.7/moarcframework/http/http.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.6/moarcframework/management/commands/refresh_template.py` & `moarc-framework-0.9.5.7/moarcframework/management/commands/refresh_template.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.6/moarcframework/middleware/thread_local_user_middleware.py` & `moarc-framework-0.9.5.7/moarcframework/middleware/thread_local_user_middleware.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.6/moarcframework/migrations/0001_initial.py` & `moarc-framework-0.9.5.7/moarcframework/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.6/moarcframework/migrations/0002_menu_permission.py` & `moarc-framework-0.9.5.7/moarcframework/migrations/0002_menu_permission.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.6/moarcframework/migrations/0003_sequence.py` & `moarc-framework-0.9.5.7/moarcframework/migrations/0003_sequence.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.6/moarcframework/migrations/0004_attachment_mimetype_alter_attachment_file.py` & `moarc-framework-0.9.5.7/moarcframework/migrations/0004_attachment_mimetype_alter_attachment_file.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Generated by Django 4.0.2 on 2023-05-14 14:38
 
-import apps.moarc-framework.moarcframework.orm.fields
+from ..orm import fields
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ('moarcframework', '0003_sequence'),
     ]
 
     operations = [
         migrations.AddField(
             model_name='attachment',
             name='mimetype',
-            field=apps.moarc-framework.moarcframework.orm.fields.CharField(blank=True, default='', max_length=200, null=True, verbose_name='Tipo de archivo'),
+            field=fields.CharField(blank=True, default='', max_length=200, null=True, verbose_name='Tipo de archivo'),
         ),
         migrations.AlterField(
             model_name='attachment',
             name='file',
             field=models.FileField(upload_to='static/attachments/%Y/%m/%d/'),
         ),
     ]
```

### Comparing `moarc-framework-0.9.5.6/moarcframework/models.py` & `moarc-framework-0.9.5.7/moarcframework/models.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.6/moarcframework/orm/base_model.py` & `moarc-framework-0.9.5.7/moarcframework/orm/base_model.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.6/moarcframework/orm/fields.py` & `moarc-framework-0.9.5.7/moarcframework/orm/fields.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.6/moarcframework/ui/form.html` & `moarc-framework-0.9.5.7/moarcframework/ui/form.html`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.6/moarcframework/ui/import.html` & `moarc-framework-0.9.5.7/moarcframework/ui/import.html`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.6/moarcframework/ui/table.html` & `moarc-framework-0.9.5.7/moarcframework/ui/table.html`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.6/moarcframework/urls.py` & `moarc-framework-0.9.5.7/moarcframework/urls.py`

 * *Files identical despite different names*

### Comparing `moarc-framework-0.9.5.6/setup.cfg` & `moarc-framework-0.9.5.7/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6f61 7263 2d66 7261 6d65 776f   = moarc-framewo
 00000020: 726b 0d0a 7665 7273 696f 6e20 3d20 302e  rk..version = 0.
-00000030: 392e 352e 360d 0a64 6573 6372 6970 7469  9.5.6..descripti
+00000030: 392e 352e 370d 0a64 6573 6372 6970 7469  9.5.7..descripti
 00000040: 6f6e 203d 2041 2044 6a61 6e67 6f20 6170  on = A Django ap
 00000050: 7020 4d6f 6172 6320 4672 616d 6577 6f72  p Moarc Framewor
 00000060: 6b2e 0d0a 6c6f 6e67 5f64 6573 6372 6970  k...long_descrip
 00000070: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000080: 444d 452e 7273 740d 0a75 726c 203d 2068  DME.rst..url = h
 00000090: 7474 7073 3a2f 2f77 7777 2e65 7861 6d70  ttps://www.examp
 000000a0: 6c65 2e63 6f6d 2f0d 0a61 7574 686f 7220  le.com/..author
```

