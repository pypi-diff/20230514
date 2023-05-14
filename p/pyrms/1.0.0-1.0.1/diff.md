# Comparing `tmp/pyrms-1.0.0.tar.gz` & `tmp/pyrms-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/mattjohnson/RMGCODE/pyrms/dist/.tmp-kib8rf1j/pyrms-1.0.0.tar", last modified: Sun May 14 04:02:31 2023, max compression
+gzip compressed data, was "/Users/mattjohnson/RMGCODE/pyrms/dist/.tmp-ly5ww0a9/pyrms-1.0.1.tar", last modified: Sun May 14 17:56:46 2023, max compression
```

## Comparing `pyrms-1.0.0.tar` & `pyrms-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mattjohnson   (501) staff       (20)        0 2023-05-14 04:02:31.013157 pyrms-1.0.0/
--rw-r--r--   0 mattjohnson   (501) staff       (20)     1068 2020-07-20 23:27:57.000000 pyrms-1.0.0/LICENSE
--rw-r--r--   0 mattjohnson   (501) staff       (20)     2025 2023-05-14 04:02:31.012785 pyrms-1.0.0/PKG-INFO
--rw-r--r--   0 mattjohnson   (501) staff       (20)     1672 2023-05-14 03:56:44.000000 pyrms-1.0.0/README.md
-drwxr-xr-x   0 mattjohnson   (501) staff       (20)        0 2023-05-14 04:02:31.009224 pyrms-1.0.0/pyrms/
--rw-r--r--   0 mattjohnson   (501) staff       (20)       11 2023-05-14 03:56:39.000000 pyrms-1.0.0/pyrms/__init__.py
--rw-r--r--   0 mattjohnson   (501) staff       (20)     3255 2023-05-14 03:57:11.000000 pyrms-1.0.0/pyrms/rms.py
--rw-r--r--   0 mattjohnson   (501) staff       (20)      736 2019-04-15 12:19:38.000000 pyrms-1.0.0/pyrms/rmsTest.py
-drwxr-xr-x   0 mattjohnson   (501) staff       (20)        0 2023-05-14 04:02:31.012272 pyrms-1.0.0/pyrms.egg-info/
--rw-r--r--   0 mattjohnson   (501) staff       (20)     2025 2023-05-14 04:02:30.000000 pyrms-1.0.0/pyrms.egg-info/PKG-INFO
--rw-r--r--   0 mattjohnson   (501) staff       (20)      190 2023-05-14 04:02:31.000000 pyrms-1.0.0/pyrms.egg-info/SOURCES.txt
--rw-r--r--   0 mattjohnson   (501) staff       (20)        1 2023-05-14 04:02:30.000000 pyrms-1.0.0/pyrms.egg-info/dependency_links.txt
--rw-r--r--   0 mattjohnson   (501) staff       (20)        6 2023-05-14 04:02:30.000000 pyrms-1.0.0/pyrms.egg-info/top_level.txt
--rw-r--r--   0 mattjohnson   (501) staff       (20)       38 2023-05-14 04:02:31.013254 pyrms-1.0.0/setup.cfg
--rw-r--r--   0 mattjohnson   (501) staff       (20)      613 2023-05-14 04:02:15.000000 pyrms-1.0.0/setup.py
+drwxr-xr-x   0 mattjohnson   (501) staff       (20)        0 2023-05-14 17:56:46.901719 pyrms-1.0.1/
+-rw-r--r--   0 mattjohnson   (501) staff       (20)     1068 2023-05-14 15:07:22.000000 pyrms-1.0.1/LICENSE
+-rw-r--r--   0 mattjohnson   (501) staff       (20)     2025 2023-05-14 17:56:46.901342 pyrms-1.0.1/PKG-INFO
+-rw-r--r--   0 mattjohnson   (501) staff       (20)     1672 2023-05-14 03:56:44.000000 pyrms-1.0.1/README.md
+drwxr-xr-x   0 mattjohnson   (501) staff       (20)        0 2023-05-14 17:56:46.897746 pyrms-1.0.1/pyrms/
+-rw-r--r--   0 mattjohnson   (501) staff       (20)      436 2023-05-14 17:54:46.000000 pyrms-1.0.1/pyrms/__init__.py
+-rw-r--r--   0 mattjohnson   (501) staff       (20)     3255 2023-05-14 03:57:11.000000 pyrms-1.0.1/pyrms/rms.py
+-rw-r--r--   0 mattjohnson   (501) staff       (20)      736 2019-04-15 12:19:38.000000 pyrms-1.0.1/pyrms/rmsTest.py
+drwxr-xr-x   0 mattjohnson   (501) staff       (20)        0 2023-05-14 17:56:46.900950 pyrms-1.0.1/pyrms.egg-info/
+-rw-r--r--   0 mattjohnson   (501) staff       (20)     2025 2023-05-14 17:56:46.000000 pyrms-1.0.1/pyrms.egg-info/PKG-INFO
+-rw-r--r--   0 mattjohnson   (501) staff       (20)      190 2023-05-14 17:56:46.000000 pyrms-1.0.1/pyrms.egg-info/SOURCES.txt
+-rw-r--r--   0 mattjohnson   (501) staff       (20)        1 2023-05-14 17:56:46.000000 pyrms-1.0.1/pyrms.egg-info/dependency_links.txt
+-rw-r--r--   0 mattjohnson   (501) staff       (20)        6 2023-05-14 17:56:46.000000 pyrms-1.0.1/pyrms.egg-info/top_level.txt
+-rw-r--r--   0 mattjohnson   (501) staff       (20)       38 2023-05-14 17:56:46.901867 pyrms-1.0.1/setup.cfg
+-rw-r--r--   0 mattjohnson   (501) staff       (20)      613 2023-05-14 17:56:19.000000 pyrms-1.0.1/setup.py
```

### Comparing `pyrms-1.0.0/LICENSE` & `pyrms-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrms-1.0.0/PKG-INFO` & `pyrms-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrms
-Version: 1.0.0
+Version: 1.0.1
 Home-page: https://github.com/ReactionMechanismGenerator/pyrms
 Author: mjohnson541
 Author-email: mjohnson541@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pyrms-1.0.0/README.md` & `pyrms-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyrms-1.0.0/pyrms/rms.py` & `pyrms-1.0.1/pyrms/rms.py`

 * *Files identical despite different names*

### Comparing `pyrms-1.0.0/pyrms/rmsTest.py` & `pyrms-1.0.1/pyrms/rmsTest.py`

 * *Files identical despite different names*

### Comparing `pyrms-1.0.0/pyrms.egg-info/PKG-INFO` & `pyrms-1.0.1/pyrms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrms
-Version: 1.0.0
+Version: 1.0.1
 Home-page: https://github.com/ReactionMechanismGenerator/pyrms
 Author: mjohnson541
 Author-email: mjohnson541@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pyrms-1.0.0/setup.py` & `pyrms-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyrms", # Replace with your own username
-    version="1.0.0",
+    version="1.0.1",
     author="mjohnson541",
     author_email="mjohnson541@gmail.com",
     description="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ReactionMechanismGenerator/pyrms",
     packages=setuptools.find_packages(),
```

