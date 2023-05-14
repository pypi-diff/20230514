# Comparing `tmp/persian_num2words-1.0.0.tar.gz` & `tmp/persian_num2words-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "persian_num2words-1.0.0.tar", last modified: Sun May 14 12:08:18 2023, max compression
+gzip compressed data, was "persian_num2words-1.0.1.tar", last modified: Sun May 14 13:23:58 2023, max compression
```

## Comparing `persian_num2words-1.0.0.tar` & `persian_num2words-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,20 @@
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-14 12:08:18.390839 persian_num2words-1.0.0/
--rw-r--r--   0 mostafa    (501) staff       (20)     1068 2023-05-14 12:03:58.000000 persian_num2words-1.0.0/LICENSE.txt
--rw-r--r--   0 mostafa    (501) staff       (20)     1848 2023-05-14 12:08:18.390893 persian_num2words-1.0.0/PKG-INFO
--rw-r--r--   0 mostafa    (501) staff       (20)      163 2023-05-14 12:03:02.000000 persian_num2words-1.0.0/README.md
--rw-r--r--   0 mostafa    (501) staff       (20)       84 2023-05-14 12:00:11.000000 persian_num2words-1.0.0/pyproject.toml
--rw-r--r--   0 mostafa    (501) staff       (20)      738 2023-05-14 12:08:18.391121 persian_num2words-1.0.0/setup.cfg
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-14 12:08:18.389601 persian_num2words-1.0.0/src/
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-14 12:08:18.390612 persian_num2words-1.0.0/src/persian_num2words.egg-info/
--rw-r--r--   0 mostafa    (501) staff       (20)     1848 2023-05-14 12:08:18.000000 persian_num2words-1.0.0/src/persian_num2words.egg-info/PKG-INFO
--rw-r--r--   0 mostafa    (501) staff       (20)      249 2023-05-14 12:08:18.000000 persian_num2words-1.0.0/src/persian_num2words.egg-info/SOURCES.txt
--rw-r--r--   0 mostafa    (501) staff       (20)        1 2023-05-14 12:08:18.000000 persian_num2words-1.0.0/src/persian_num2words.egg-info/dependency_links.txt
--rw-r--r--   0 mostafa    (501) staff       (20)        1 2023-05-14 12:08:18.000000 persian_num2words-1.0.0/src/persian_num2words.egg-info/top_level.txt
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-14 12:08:18.390733 persian_num2words-1.0.0/tests/
--rw-r--r--   0 mostafa    (501) staff       (20)      228 2023-05-14 11:52:26.000000 persian_num2words-1.0.0/tests/test_num2word.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-14 13:23:58.497972 persian_num2words-1.0.1/
+-rw-r--r--   0 mostafa    (501) staff       (20)     1068 2023-05-14 12:03:58.000000 persian_num2words-1.0.1/LICENSE.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)     1846 2023-05-14 13:23:58.498019 persian_num2words-1.0.1/PKG-INFO
+-rw-r--r--   0 mostafa    (501) staff       (20)      163 2023-05-14 12:03:02.000000 persian_num2words-1.0.1/README.md
+-rw-r--r--   0 mostafa    (501) staff       (20)       84 2023-05-14 12:00:11.000000 persian_num2words-1.0.1/pyproject.toml
+-rw-r--r--   0 mostafa    (501) staff       (20)      736 2023-05-14 13:23:58.498233 persian_num2words-1.0.1/setup.cfg
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-14 13:23:58.496505 persian_num2words-1.0.1/src/
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-14 13:23:58.497163 persian_num2words-1.0.1/src/main_module/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2023-05-14 11:40:42.000000 persian_num2words-1.0.1/src/main_module/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    12591 2023-05-14 13:15:42.000000 persian_num2words-1.0.1/src/main_module/num2words.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-14 13:23:58.497592 persian_num2words-1.0.1/src/persian_num2words.egg-info/
+-rw-r--r--   0 mostafa    (501) staff       (20)     1846 2023-05-14 13:23:58.000000 persian_num2words-1.0.1/src/persian_num2words.egg-info/PKG-INFO
+-rw-r--r--   0 mostafa    (501) staff       (20)      370 2023-05-14 13:23:58.000000 persian_num2words-1.0.1/src/persian_num2words.egg-info/SOURCES.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)        1 2023-05-14 13:23:58.000000 persian_num2words-1.0.1/src/persian_num2words.egg-info/dependency_links.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)       25 2023-05-14 13:23:58.000000 persian_num2words-1.0.1/src/persian_num2words.egg-info/top_level.txt
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-14 13:23:58.497771 persian_num2words-1.0.1/src/small_module/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2023-05-14 11:40:42.000000 persian_num2words-1.0.1/src/small_module/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)      156 2023-05-13 19:21:29.000000 persian_num2words-1.0.1/src/small_module/small_function.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-14 13:23:58.497874 persian_num2words-1.0.1/tests/
+-rw-r--r--   0 mostafa    (501) staff       (20)      228 2023-05-14 11:52:26.000000 persian_num2words-1.0.1/tests/test_num2word.py
```

### Comparing `persian_num2words-1.0.0/LICENSE.txt` & `persian_num2words-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `persian_num2words-1.0.0/PKG-INFO` & `persian_num2words-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: persian_num2words
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Package to Convert Numbers to Words in Persian.
 Home-page: https://github.com/mosihere/persian_num2words
 Author: Mosihere
 Author-email: mosihere@gmail.com
-Project-URL: Bug Tracker, https://github.com/mosihere/persian_num2words/-/issues
-Project-URL: repository, https://gitlab.com/mosihere/persian_num2words
+Project-URL: Bug Tracker, https://github.com/mosihere/persian_num2words/issues
+Project-URL: repository, https://github.com/mosihere/persian_num2words
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `persian_num2words-1.0.0/setup.cfg` & `persian_num2words-1.0.1/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [metadata]
 name = persian_num2words
-version = 1.0.0
+version = 1.0.1
 author = Mosihere
 author_email = mosihere@gmail.com
 description = A Package to Convert Numbers to Words in Persian.
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/mosihere/persian_num2words
 project_urls = 
-	Bug Tracker = https://github.com/mosihere/persian_num2words/-/issues
-	repository = https://gitlab.com/mosihere/persian_num2words
+	Bug Tracker = https://github.com/mosihere/persian_num2words/issues
+	repository = https://github.com/mosihere/persian_num2words
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir =
```

### Comparing `persian_num2words-1.0.0/src/persian_num2words.egg-info/PKG-INFO` & `persian_num2words-1.0.1/src/persian_num2words.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: persian-num2words
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Package to Convert Numbers to Words in Persian.
 Home-page: https://github.com/mosihere/persian_num2words
 Author: Mosihere
 Author-email: mosihere@gmail.com
-Project-URL: Bug Tracker, https://github.com/mosihere/persian_num2words/-/issues
-Project-URL: repository, https://gitlab.com/mosihere/persian_num2words
+Project-URL: Bug Tracker, https://github.com/mosihere/persian_num2words/issues
+Project-URL: repository, https://github.com/mosihere/persian_num2words
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

