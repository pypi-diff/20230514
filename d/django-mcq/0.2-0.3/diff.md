# Comparing `tmp/django-mcq-0.2.tar.gz` & `tmp/django-mcq-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mcq-0.2.tar", last modified: Mon May  1 02:49:00 2023, max compression
+gzip compressed data, was "django-mcq-0.3.tar", last modified: Sun May 14 04:15:48 2023, max compression
```

## Comparing `django-mcq-0.2.tar` & `django-mcq-0.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:49:00.474079 django-mcq-0.2/
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     1063 2023-05-01 02:01:55.000000 django-mcq-0.2/LICENSE
--rw-rw-r--   0 suhail    (1000) suhail    (1000)       61 2023-05-01 02:23:43.000000 django-mcq-0.2/MANIFEST.in
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     1795 2023-05-01 02:49:00.474079 django-mcq-0.2/PKG-INFO
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     1044 2023-05-01 02:48:40.000000 django-mcq-0.2/README.md
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:49:00.462079 django-mcq-0.2/django_mcq.egg-info/
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     1795 2023-05-01 02:49:00.000000 django-mcq-0.2/django_mcq.egg-info/PKG-INFO
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     1110 2023-05-01 02:49:00.000000 django-mcq-0.2/django_mcq.egg-info/SOURCES.txt
--rw-rw-r--   0 suhail    (1000) suhail    (1000)        1 2023-05-01 02:49:00.000000 django-mcq-0.2/django_mcq.egg-info/dependency_links.txt
--rw-rw-r--   0 suhail    (1000) suhail    (1000)        1 2023-05-01 02:49:00.000000 django-mcq-0.2/django_mcq.egg-info/not-zip-safe
--rw-rw-r--   0 suhail    (1000) suhail    (1000)       14 2023-05-01 02:49:00.000000 django-mcq-0.2/django_mcq.egg-info/requires.txt
--rw-rw-r--   0 suhail    (1000) suhail    (1000)        5 2023-05-01 02:49:00.000000 django-mcq-0.2/django_mcq.egg-info/top_level.txt
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      104 2023-05-01 02:01:55.000000 django-mcq-0.2/pyproject.toml
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:49:00.466079 django-mcq-0.2/quiz/
--rw-rw-r--   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/__init__.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)       63 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/admin.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      140 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/apps.py
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:49:00.466079 django-mcq-0.2/quiz/fixtures/
--rw-rw-r--   0 suhail    (1000) suhail    (1000)    16766 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/fixtures/sample_quizzes.json
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      879 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/forms.py
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:49:00.466079 django-mcq-0.2/quiz/migrations/
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     6373 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/migrations/0001_initial.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/migrations/__init__.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     2655 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/models.py
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:49:00.462079 django-mcq-0.2/quiz/static/
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:49:00.466079 django-mcq-0.2/quiz/static/datatables/
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     5222 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/static/datatables/dataTables.bootstrap4.min.css
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     2085 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/static/datatables/dataTables.bootstrap4.min.js
--rw-rw-r--   0 suhail    (1000) suhail    (1000)    82411 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/static/datatables/jquery.dataTables.min.js
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:49:00.470079 django-mcq-0.2/quiz/static/quiz/
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      533 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/static/quiz/app.css
--rw-rw-r--   0 suhail    (1000) suhail    (1000)   141997 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/static/quiz/bootstrap.min.css
--rw-rw-r--   0 suhail    (1000) suhail    (1000)    86927 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/static/quiz/jquery-3.3.1.min.js
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:49:00.462079 django-mcq-0.2/quiz/templates/
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:49:00.470079 django-mcq-0.2/quiz/templates/quiz/
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      670 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/templates/quiz/_header.html
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      801 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/templates/quiz/base.html
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      384 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/templates/quiz/interests_form.html
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     1913 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/templates/quiz/quiz_list.html
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     1683 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/templates/quiz/quiz_result.html
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     1251 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/templates/quiz/student_detail.html
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     2396 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/templates/quiz/student_list.html
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      685 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/templates/quiz/take_quiz_form.html
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      847 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/templates/quiz/taken_quiz_list.html
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:49:00.470079 django-mcq-0.2/quiz/templatetags/
--rw-rw-r--   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/templatetags/__init__.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      995 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/templatetags/quiz_extras.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)       60 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/tests.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      646 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/urls.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     6919 2023-05-01 02:38:06.000000 django-mcq-0.2/quiz/views.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)       38 2023-05-01 02:49:00.474079 django-mcq-0.2/setup.cfg
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     1078 2023-05-01 02:33:04.000000 django-mcq-0.2/setup.py
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-14 04:15:48.031310 django-mcq-0.3/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     1063 2023-05-01 02:01:55.000000 django-mcq-0.3/LICENSE
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)       61 2023-05-01 02:23:43.000000 django-mcq-0.3/MANIFEST.in
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     1795 2023-05-14 04:15:48.031310 django-mcq-0.3/PKG-INFO
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     1044 2023-05-14 04:13:58.000000 django-mcq-0.3/README.md
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-14 04:15:48.027303 django-mcq-0.3/django_mcq.egg-info/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     1795 2023-05-14 04:15:48.000000 django-mcq-0.3/django_mcq.egg-info/PKG-INFO
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     1110 2023-05-14 04:15:48.000000 django-mcq-0.3/django_mcq.egg-info/SOURCES.txt
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)        1 2023-05-14 04:15:48.000000 django-mcq-0.3/django_mcq.egg-info/dependency_links.txt
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)        1 2023-05-01 02:49:00.000000 django-mcq-0.3/django_mcq.egg-info/not-zip-safe
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)       14 2023-05-14 04:15:48.000000 django-mcq-0.3/django_mcq.egg-info/requires.txt
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)        5 2023-05-14 04:15:48.000000 django-mcq-0.3/django_mcq.egg-info/top_level.txt
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      104 2023-05-01 02:01:55.000000 django-mcq-0.3/pyproject.toml
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-14 04:15:48.027303 django-mcq-0.3/quiz/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/__init__.py
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)       63 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/admin.py
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      140 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/apps.py
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-14 04:15:48.027303 django-mcq-0.3/quiz/fixtures/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)    16766 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/fixtures/sample_quizzes.json
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      879 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/forms.py
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-14 04:15:48.027303 django-mcq-0.3/quiz/migrations/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     6373 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/migrations/0001_initial.py
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/migrations/__init__.py
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     2655 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/models.py
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-14 04:15:48.023296 django-mcq-0.3/quiz/static/
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-14 04:15:48.027303 django-mcq-0.3/quiz/static/datatables/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     5222 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/static/datatables/dataTables.bootstrap4.min.css
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     2085 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/static/datatables/dataTables.bootstrap4.min.js
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)    82411 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/static/datatables/jquery.dataTables.min.js
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-14 04:15:48.027303 django-mcq-0.3/quiz/static/quiz/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      533 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/static/quiz/app.css
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)   141997 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/static/quiz/bootstrap.min.css
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)    86927 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/static/quiz/jquery-3.3.1.min.js
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-14 04:15:48.023296 django-mcq-0.3/quiz/templates/
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-14 04:15:48.031310 django-mcq-0.3/quiz/templates/quiz/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      670 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/templates/quiz/_header.html
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      801 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/templates/quiz/base.html
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      384 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/templates/quiz/interests_form.html
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     3478 2023-05-14 04:12:39.000000 django-mcq-0.3/quiz/templates/quiz/quiz_list.html
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     1683 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/templates/quiz/quiz_result.html
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     1251 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/templates/quiz/student_detail.html
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     2396 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/templates/quiz/student_list.html
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      685 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/templates/quiz/take_quiz_form.html
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      847 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/templates/quiz/taken_quiz_list.html
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-14 04:15:48.031310 django-mcq-0.3/quiz/templatetags/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/templatetags/__init__.py
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      995 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/templatetags/quiz_extras.py
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)       60 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/tests.py
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      724 2023-05-14 04:12:39.000000 django-mcq-0.3/quiz/urls.py
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     8036 2023-05-14 04:12:39.000000 django-mcq-0.3/quiz/views.py
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)       38 2023-05-14 04:15:48.031310 django-mcq-0.3/setup.cfg
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     1078 2023-05-14 04:13:09.000000 django-mcq-0.3/setup.py
```

### Comparing `django-mcq-0.2/LICENSE` & `django-mcq-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-mcq-0.2/PKG-INFO` & `django-mcq-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mcq
-Version: 0.2
+Version: 0.3
 Summary: A configurable quiz app for Django.
 Home-page: https://github.com/suhailvs/django-mcq
 Author: Suhail VS
 Author-email: suhailvs@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-mcq Version: 0.2 Summary: A configurable
+Metadata-Version: 2.1 Name: django-mcq Version: 0.3 Summary: A configurable
 quiz app for Django. Home-page: https://github.com/suhailvs/django-mcq Author:
 Suhail VS Author-email: suhailvs@gmail.com License: MIT License Classifier:
 Environment :: Web Environment Classifier: Framework :: Django Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Internet
```

### Comparing `django-mcq-0.2/README.md` & `django-mcq-0.3/README.md`

 * *Files identical despite different names*

### Comparing `django-mcq-0.2/django_mcq.egg-info/PKG-INFO` & `django-mcq-0.3/django_mcq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mcq
-Version: 0.2
+Version: 0.3
 Summary: A configurable quiz app for Django.
 Home-page: https://github.com/suhailvs/django-mcq
 Author: Suhail VS
 Author-email: suhailvs@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-mcq Version: 0.2 Summary: A configurable
+Metadata-Version: 2.1 Name: django-mcq Version: 0.3 Summary: A configurable
 quiz app for Django. Home-page: https://github.com/suhailvs/django-mcq Author:
 Suhail VS Author-email: suhailvs@gmail.com License: MIT License Classifier:
 Environment :: Web Environment Classifier: Framework :: Django Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Internet
```

### Comparing `django-mcq-0.2/django_mcq.egg-info/SOURCES.txt` & `django-mcq-0.3/django_mcq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-mcq-0.2/quiz/fixtures/sample_quizzes.json` & `django-mcq-0.3/quiz/fixtures/sample_quizzes.json`

 * *Files identical despite different names*

### Comparing `django-mcq-0.2/quiz/forms.py` & `django-mcq-0.3/quiz/forms.py`

 * *Files identical despite different names*

### Comparing `django-mcq-0.2/quiz/migrations/0001_initial.py` & `django-mcq-0.3/quiz/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-mcq-0.2/quiz/models.py` & `django-mcq-0.3/quiz/models.py`

 * *Files identical despite different names*

### Comparing `django-mcq-0.2/quiz/static/datatables/dataTables.bootstrap4.min.css` & `django-mcq-0.3/quiz/static/datatables/dataTables.bootstrap4.min.css`

 * *Files identical despite different names*

### Comparing `django-mcq-0.2/quiz/static/datatables/dataTables.bootstrap4.min.js` & `django-mcq-0.3/quiz/static/datatables/dataTables.bootstrap4.min.js`

 * *Files identical despite different names*

### Comparing `django-mcq-0.2/quiz/static/datatables/jquery.dataTables.min.js` & `django-mcq-0.3/quiz/static/datatables/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `django-mcq-0.2/quiz/static/quiz/app.css` & `django-mcq-0.3/quiz/static/quiz/app.css`

 * *Files identical despite different names*

### Comparing `django-mcq-0.2/quiz/static/quiz/bootstrap.min.css` & `django-mcq-0.3/quiz/static/quiz/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-mcq-0.2/quiz/static/quiz/jquery-3.3.1.min.js` & `django-mcq-0.3/quiz/static/quiz/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `django-mcq-0.2/quiz/templates/quiz/_header.html` & `django-mcq-0.3/quiz/templates/quiz/_header.html`

 * *Files identical despite different names*

### Comparing `django-mcq-0.2/quiz/templates/quiz/base.html` & `django-mcq-0.3/quiz/templates/quiz/base.html`

 * *Files identical despite different names*

### Comparing `django-mcq-0.2/quiz/templates/quiz/quiz_result.html` & `django-mcq-0.3/quiz/templates/quiz/quiz_result.html`

 * *Files identical despite different names*

### Comparing `django-mcq-0.2/quiz/templates/quiz/student_detail.html` & `django-mcq-0.3/quiz/templates/quiz/student_detail.html`

 * *Files identical despite different names*

### Comparing `django-mcq-0.2/quiz/templates/quiz/student_list.html` & `django-mcq-0.3/quiz/templates/quiz/student_list.html`

 * *Files identical despite different names*

### Comparing `django-mcq-0.2/quiz/templates/quiz/take_quiz_form.html` & `django-mcq-0.3/quiz/templates/quiz/take_quiz_form.html`

 * *Files identical despite different names*

### Comparing `django-mcq-0.2/quiz/templates/quiz/taken_quiz_list.html` & `django-mcq-0.3/quiz/templates/quiz/taken_quiz_list.html`

 * *Files identical despite different names*

### Comparing `django-mcq-0.2/quiz/templatetags/quiz_extras.py` & `django-mcq-0.3/quiz/templatetags/quiz_extras.py`

 * *Files identical despite different names*

### Comparing `django-mcq-0.2/quiz/urls.py` & `django-mcq-0.3/quiz/urls.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,12 +4,13 @@
 app_name='quiz'
 
 urlpatterns = [
     path('', views.StudentList.as_view(), name='student_list'),
     path('<int:student>/', views.StudentDetail.as_view(), name='student_detail'),
     path('interests/', views.StudentInterestsView.as_view(), name='student_interests'),
     path('taken/', views.TakenQuizListView.as_view(), name='taken_quiz_list'),
+    path('create_quiz/', views.CreateQuizView.as_view(), name='create_quiz'),
     path('q/', views.QuizListView.as_view(), name='quiz_list'),
     path('q/<int:pk>/', views.take_quiz, name='take_quiz'),        
     path('q/<int:pk>/studentresults/', views.QuizResultsView.as_view(), name='student_quiz_results'),
     
 ]
```

### Comparing `django-mcq-0.2/quiz/views.py` & `django-mcq-0.3/quiz/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from django.shortcuts import get_object_or_404, redirect, render
 from django.urls import reverse_lazy
 from django.utils.decorators import method_decorator
 from django.views.generic import ListView, UpdateView
 from django.views import View
 
 from .forms import StudentInterestsForm, TakeQuizForm
-from .models import Quiz, Student, TakenQuiz, Question
+from .models import Quiz, Student, TakenQuiz, Question, Subject, Answer
 
 User = get_user_model()
 
 def get_or_create_student(user):
     try:
         return user.student
     except:
@@ -75,14 +75,38 @@
             return render(request, '404.html')
         questions = Question.objects.filter(quiz =quiz)
         
         # questions = self.form_class(initial=self.initial)
         return render(request, self.template_name, {'questions':questions, 
             'quiz':quiz, 'percentage': taken_quiz[0].percentage})
 
+from django.http import JsonResponse
+
+@method_decorator([login_required], name='dispatch')
+class CreateQuizView(View):
+    def create_quiz(self, quiz):
+        subject, _ = Subject.objects.get_or_create(name=quiz['subject'])
+        quiz_item= Quiz.objects.create(name=quiz['quiz'],subject=subject)
+        for question in quiz['questions']:
+            question_item = Question.objects.create(quiz=quiz_item,text=question['question'])
+            for answer in question['answers']:
+                is_correct = True if answer['is_correct'] == 'true' else False
+                Answer.objects.create(question = question_item, text = answer['answer'],is_correct=is_correct)
+    def post(self, request, *args, **kwargs): 
+        import json
+        try:
+            quizzes = json.loads(request.POST['txt_quizzes_json'])
+            with transaction.atomic():
+                for quiz in quizzes:
+                    self.create_quiz(quiz)
+        except Exception as e:
+            print(e)
+            return JsonResponse({'resp':'error'})
+        
+        return JsonResponse({'resp':'success'})  
 
 @method_decorator([login_required], name='dispatch')
 class TakenQuizListView(ListView):
     model = TakenQuiz
     context_object_name = 'taken_quizzes'
     template_name = 'quiz/taken_quiz_list.html'
```

### Comparing `django-mcq-0.2/setup.py` & `django-mcq-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 readme = open('README.md', encoding='utf-8')
 long_description = readme.read()
 
 
 setup(
     name='django-mcq',
-    version='0.2',
+    version='0.3',
     packages=find_packages(),
     include_package_data=True,
     license='MIT License',
     description='A configurable quiz app for Django.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/suhailvs/django-mcq',
```

