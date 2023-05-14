# Comparing `tmp/featurizerai-1.6.8.tar.gz` & `tmp/featurizerai-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurizerai-1.6.8.tar", last modified: Sun May 14 02:45:14 2023, max compression
+gzip compressed data, was "featurizerai-1.6.9.tar", last modified: Sun May 14 02:52:36 2023, max compression
```

## Comparing `featurizerai-1.6.8.tar` & `featurizerai-1.6.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-05-14 02:45:14.113171 featurizerai-1.6.8/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.6.8/LICENSE
--rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.6.8/MANIFEST.in
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-05-14 02:45:14.113236 featurizerai-1.6.8/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.6.8/pyproject.toml
--rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-05-14 02:45:14.113572 featurizerai-1.6.8/setup.cfg
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-05-14 02:45:08.000000 featurizerai-1.6.8/setup.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-05-14 02:45:14.109017 featurizerai-1.6.8/src/
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-05-14 02:45:14.112282 featurizerai-1.6.8/src/features/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.6.8/src/features/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      686 2023-04-22 23:39:43.000000 featurizerai-1.6.8/src/features/authenticate.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4223 2023-04-28 19:36:07.000000 featurizerai-1.6.8/src/features/create_stream.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1306 2023-05-14 02:44:54.000000 featurizerai-1.6.8/src/features/custom_schema.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4872 2023-04-30 04:27:45.000000 featurizerai-1.6.8/src/features/materialize.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     6558 2023-04-30 00:07:16.000000 featurizerai-1.6.8/src/features/test.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-05-14 02:45:14.113049 featurizerai-1.6.8/src/featurizerai.egg-info/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-05-14 02:45:14.000000 featurizerai-1.6.8/src/featurizerai.egg-info/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)      415 2023-05-14 02:45:14.000000 featurizerai-1.6.8/src/featurizerai.egg-info/SOURCES.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-05-14 02:45:14.000000 featurizerai-1.6.8/src/featurizerai.egg-info/dependency_links.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-05-14 02:45:14.000000 featurizerai-1.6.8/src/featurizerai.egg-info/requires.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-05-14 02:45:14.000000 featurizerai-1.6.8/src/featurizerai.egg-info/top_level.txt
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-05-14 02:52:36.997644 featurizerai-1.6.9/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.6.9/LICENSE
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.6.9/MANIFEST.in
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-05-14 02:52:36.997713 featurizerai-1.6.9/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.6.9/pyproject.toml
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-05-14 02:52:36.997934 featurizerai-1.6.9/setup.cfg
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-05-14 02:50:39.000000 featurizerai-1.6.9/setup.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-05-14 02:52:36.994685 featurizerai-1.6.9/src/
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-05-14 02:52:36.996603 featurizerai-1.6.9/src/features/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.6.9/src/features/__init__.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      686 2023-04-22 23:39:43.000000 featurizerai-1.6.9/src/features/authenticate.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4223 2023-04-28 19:36:07.000000 featurizerai-1.6.9/src/features/create_stream.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      932 2023-05-14 02:52:31.000000 featurizerai-1.6.9/src/features/custom_schema.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4872 2023-04-30 04:27:45.000000 featurizerai-1.6.9/src/features/materialize.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     6558 2023-04-30 00:07:16.000000 featurizerai-1.6.9/src/features/test.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-05-14 02:52:36.997512 featurizerai-1.6.9/src/featurizerai.egg-info/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-05-14 02:52:36.000000 featurizerai-1.6.9/src/featurizerai.egg-info/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      415 2023-05-14 02:52:36.000000 featurizerai-1.6.9/src/featurizerai.egg-info/SOURCES.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-05-14 02:52:36.000000 featurizerai-1.6.9/src/featurizerai.egg-info/dependency_links.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-05-14 02:52:36.000000 featurizerai-1.6.9/src/featurizerai.egg-info/requires.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-05-14 02:52:36.000000 featurizerai-1.6.9/src/featurizerai.egg-info/top_level.txt
```

### Comparing `featurizerai-1.6.8/LICENSE` & `featurizerai-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `featurizerai-1.6.8/PKG-INFO` & `featurizerai-1.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.6.8
+Version: 1.6.9
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.6.8/setup.py` & `featurizerai-1.6.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name='featurizerai',
     author='Burak',
-    version='1.6.8',
+    version='1.6.9',
     author_email='burakgblobal@gmail.com',
     description='Python library for Featurizer AI',
     keywords='featurizer, package',
     url='https://github.com/burakglobal/featurizerai',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
```

### Comparing `featurizerai-1.6.8/src/features/authenticate.py` & `featurizerai-1.6.9/src/features/authenticate.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.6.8/src/features/create_stream.py` & `featurizerai-1.6.9/src/features/create_stream.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.6.8/src/features/materialize.py` & `featurizerai-1.6.9/src/features/materialize.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.6.8/src/features/test.py` & `featurizerai-1.6.9/src/features/test.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.6.8/src/featurizerai.egg-info/PKG-INFO` & `featurizerai-1.6.9/src/featurizerai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.6.8
+Version: 1.6.9
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

