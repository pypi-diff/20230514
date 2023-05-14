# Comparing `tmp/shopcloud-django-authenticator-1.8.0.tar.gz` & `tmp/shopcloud-django-authenticator-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shopcloud-django-authenticator-1.8.0.tar", last modified: Thu Mar 30 05:03:19 2023, max compression
+gzip compressed data, was "shopcloud-django-authenticator-1.9.0.tar", last modified: Wed May  3 05:17:37 2023, max compression
```

## Comparing `shopcloud-django-authenticator-1.8.0.tar` & `shopcloud-django-authenticator-1.9.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:03:19.213813 shopcloud-django-authenticator-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-30 05:02:55.000000 shopcloud-django-authenticator-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-30 05:02:55.000000 shopcloud-django-authenticator-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-30 05:03:19.217814 shopcloud-django-authenticator-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-30 05:02:55.000000 shopcloud-django-authenticator-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:03:19.213813 shopcloud-django-authenticator-1.8.0/authenticator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 05:02:55.000000 shopcloud-django-authenticator-1.8.0/authenticator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-30 05:02:55.000000 shopcloud-django-authenticator-1.8.0/authenticator/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-30 05:02:55.000000 shopcloud-django-authenticator-1.8.0/authenticator/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:03:19.213813 shopcloud-django-authenticator-1.8.0/authenticator/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 05:02:55.000000 shopcloud-django-authenticator-1.8.0/authenticator/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-30 05:02:55.000000 shopcloud-django-authenticator-1.8.0/authenticator/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-30 05:02:55.000000 shopcloud-django-authenticator-1.8.0/authenticator/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-30 05:02:55.000000 shopcloud-django-authenticator-1.8.0/authenticator/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-03-30 05:02:55.000000 shopcloud-django-authenticator-1.8.0/authenticator/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-03-30 05:02:55.000000 shopcloud-django-authenticator-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-03-30 05:03:19.217814 shopcloud-django-authenticator-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 05:02:55.000000 shopcloud-django-authenticator-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:03:19.213813 shopcloud-django-authenticator-1.8.0/shopcloud_django_authenticator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-30 05:03:19.000000 shopcloud-django-authenticator-1.8.0/shopcloud_django_authenticator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-03-30 05:03:19.000000 shopcloud-django-authenticator-1.8.0/shopcloud_django_authenticator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 05:03:19.000000 shopcloud-django-authenticator-1.8.0/shopcloud_django_authenticator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-30 05:03:19.000000 shopcloud-django-authenticator-1.8.0/shopcloud_django_authenticator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-30 05:03:19.000000 shopcloud-django-authenticator-1.8.0/shopcloud_django_authenticator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:03:19.213813 shopcloud-django-authenticator-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 05:02:55.000000 shopcloud-django-authenticator-1.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-30 05:02:55.000000 shopcloud-django-authenticator-1.8.0/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:17:37.638676 shopcloud-django-authenticator-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-03 05:17:05.000000 shopcloud-django-authenticator-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-03 05:17:05.000000 shopcloud-django-authenticator-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-03 05:17:37.638676 shopcloud-django-authenticator-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-03 05:17:05.000000 shopcloud-django-authenticator-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:17:37.634676 shopcloud-django-authenticator-1.9.0/authenticator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:17:05.000000 shopcloud-django-authenticator-1.9.0/authenticator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-03 05:17:05.000000 shopcloud-django-authenticator-1.9.0/authenticator/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-03 05:17:05.000000 shopcloud-django-authenticator-1.9.0/authenticator/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:17:37.634676 shopcloud-django-authenticator-1.9.0/authenticator/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:17:05.000000 shopcloud-django-authenticator-1.9.0/authenticator/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-03 05:17:05.000000 shopcloud-django-authenticator-1.9.0/authenticator/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-03 05:17:05.000000 shopcloud-django-authenticator-1.9.0/authenticator/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-03 05:17:05.000000 shopcloud-django-authenticator-1.9.0/authenticator/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-05-03 05:17:05.000000 shopcloud-django-authenticator-1.9.0/authenticator/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-03 05:17:05.000000 shopcloud-django-authenticator-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-03 05:17:37.638676 shopcloud-django-authenticator-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 05:17:05.000000 shopcloud-django-authenticator-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:17:37.638676 shopcloud-django-authenticator-1.9.0/shopcloud_django_authenticator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-03 05:17:37.000000 shopcloud-django-authenticator-1.9.0/shopcloud_django_authenticator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-03 05:17:37.000000 shopcloud-django-authenticator-1.9.0/shopcloud_django_authenticator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 05:17:37.000000 shopcloud-django-authenticator-1.9.0/shopcloud_django_authenticator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-03 05:17:37.000000 shopcloud-django-authenticator-1.9.0/shopcloud_django_authenticator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-03 05:17:37.000000 shopcloud-django-authenticator-1.9.0/shopcloud_django_authenticator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:17:37.638676 shopcloud-django-authenticator-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:17:05.000000 shopcloud-django-authenticator-1.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-03 05:17:05.000000 shopcloud-django-authenticator-1.9.0/tests/urls.py
```

### Comparing `shopcloud-django-authenticator-1.8.0/LICENSE` & `shopcloud-django-authenticator-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shopcloud-django-authenticator-1.8.0/PKG-INFO` & `shopcloud-django-authenticator-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shopcloud-django-authenticator
-Version: 1.8.0
+Version: 1.9.0
 Summary: A Module for single sign in
 Home-page: https://github.com/Talk-Point/shopcloud-django-authenticator
 Author: Konstantin Stoldt
 Author-email: konstantin.stoldt@talk-point.de
 License: MIT-License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `shopcloud-django-authenticator-1.8.0/README.md` & `shopcloud-django-authenticator-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `shopcloud-django-authenticator-1.8.0/authenticator/urls.py` & `shopcloud-django-authenticator-1.9.0/authenticator/urls.py`

 * *Files identical despite different names*

### Comparing `shopcloud-django-authenticator-1.8.0/authenticator/views.py` & `shopcloud-django-authenticator-1.9.0/authenticator/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
     if user is None:
         user = User.objects.create(
             username=data.get('username'),
             password=password,
         )
 
     user.set_password(password)
+    user.is_active = True
     user.is_staff = True
     user.is_superuser = True if "admin" in data.get('scopes', []) else False
     user.save()
 
     login(request, user)
 
     return redirect('/', permanent=False)
```

### Comparing `shopcloud-django-authenticator-1.8.0/setup.cfg` & `shopcloud-django-authenticator-1.9.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shopcloud-django-authenticator
-version = 1.8.0
+version = 1.9.0
 description = A Module for single sign in
 long_description = file: README.rst
 url = https://github.com/Talk-Point/shopcloud-django-authenticator
 author = Konstantin Stoldt
 author_email = konstantin.stoldt@talk-point.de
 license = MIT-License
 classifiers =
```

### Comparing `shopcloud-django-authenticator-1.8.0/shopcloud_django_authenticator.egg-info/PKG-INFO` & `shopcloud-django-authenticator-1.9.0/shopcloud_django_authenticator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shopcloud-django-authenticator
-Version: 1.8.0
+Version: 1.9.0
 Summary: A Module for single sign in
 Home-page: https://github.com/Talk-Point/shopcloud-django-authenticator
 Author: Konstantin Stoldt
 Author-email: konstantin.stoldt@talk-point.de
 License: MIT-License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `shopcloud-django-authenticator-1.8.0/shopcloud_django_authenticator.egg-info/SOURCES.txt` & `shopcloud-django-authenticator-1.9.0/shopcloud_django_authenticator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

