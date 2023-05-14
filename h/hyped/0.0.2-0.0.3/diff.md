# Comparing `tmp/hyped-0.0.2.tar.gz` & `tmp/hyped-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyped-0.0.2.tar", last modified: Sun May 14 16:34:49 2023, max compression
+gzip compressed data, was "hyped-0.0.3.tar", last modified: Sun May 14 17:00:16 2023, max compression
```

## Comparing `hyped-0.0.2.tar` & `hyped-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:34:49.418187 hyped-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 16:34:40.000000 hyped-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-14 16:34:49.418187 hyped-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-14 16:34:40.000000 hyped-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:34:49.418187 hyped-0.0.2/hyped/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-14 16:34:40.000000 hyped-0.0.2/hyped/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:34:49.418187 hyped-0.0.2/hyped.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-14 16:34:49.000000 hyped-0.0.2/hyped.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-14 16:34:49.000000 hyped-0.0.2/hyped.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 16:34:49.000000 hyped-0.0.2/hyped.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-14 16:34:49.000000 hyped-0.0.2/hyped.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 16:34:49.000000 hyped-0.0.2/hyped.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 16:34:49.418187 hyped-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 16:34:40.000000 hyped-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:16.750982 hyped-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 17:00:07.000000 hyped-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-14 17:00:16.746982 hyped-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-14 17:00:07.000000 hyped-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:16.742982 hyped-0.0.3/hyped/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:16.742982 hyped-0.0.3/hyped/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/datasets/cas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:16.742982 hyped-0.0.3/hyped/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/evaluate/auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:16.746982 hyped-0.0.3/hyped/evaluate/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/evaluate/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/evaluate/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/evaluate/metrics/cls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/evaluate/metrics/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/evaluate/metrics/tagging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:16.746982 hyped-0.0.3/hyped/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/modeling/auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:16.746982 hyped-0.0.3/hyped/modeling/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/modeling/heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/modeling/heads/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/modeling/heads/cls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/modeling/heads/tagging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/modeling/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:16.746982 hyped-0.0.3/hyped/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/pipeline/auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:16.746982 hyped-0.0.3/hyped/pipeline/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/pipeline/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/pipeline/filters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/pipeline/filters/msl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/pipeline/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:16.746982 hyped-0.0.3/hyped/pipeline/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/pipeline/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/pipeline/processors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/pipeline/processors/bio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/pipeline/processors/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:16.746982 hyped-0.0.3/hyped/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/scripts/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/scripts/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:16.746982 hyped-0.0.3/hyped/scripts/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/scripts/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/scripts/utils/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/scripts/utils/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:16.746982 hyped-0.0.3/hyped/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/utils/typedlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/utils/typedmapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:16.742982 hyped-0.0.3/hyped.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-14 17:00:16.000000 hyped-0.0.3/hyped.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-14 17:00:16.000000 hyped-0.0.3/hyped.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 17:00:16.000000 hyped-0.0.3/hyped.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-14 17:00:16.000000 hyped-0.0.3/hyped.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 17:00:16.000000 hyped-0.0.3/hyped.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 17:00:16.750982 hyped-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-14 17:00:07.000000 hyped-0.0.3/setup.py
```

### Comparing `hyped-0.0.2/LICENSE` & `hyped-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hyped-0.0.2/PKG-INFO` & `hyped-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyped
-Version: 0.0.2
+Version: 0.0.3
 Summary: A collection of data pipelines to ease the training of transformer models
 Home-page: https://github.com/ndoll1998/hyped/tree/master
 Author: Niclas Doll
 Author-email: niclas@amazonis.net
 Classifier: License :: Freely Distributable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `hyped-0.0.2/README.md` & `hyped-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `hyped-0.0.2/hyped.egg-info/PKG-INFO` & `hyped-0.0.3/hyped.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyped
-Version: 0.0.2
+Version: 0.0.3
 Summary: A collection of data pipelines to ease the training of transformer models
 Home-page: https://github.com/ndoll1998/hyped/tree/master
 Author: Niclas Doll
 Author-email: niclas@amazonis.net
 Classifier: License :: Freely Distributable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `hyped-0.0.2/setup.py` & `hyped-0.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from distutils.core import setup
+from setuptools import setup, find_packages
 
 setup(
     name="hyped",
-    version="0.0.2",
+    version="0.0.3",
     description="A collection of data pipelines to ease the training of transformer models",
     long_description=open("README.md", "r").read(),
     long_description_content_type='text/markdown',
     author="Niclas Doll",
     author_email="niclas@amazonis.net",
     url="https://github.com/ndoll1998/hyped/tree/master",
-    packages=['hyped'],
+    packages=find_packages(exclude='tests'),
     package_dir={'hyped': 'hyped'},
     classifiers=[
         "License :: Freely Distributable",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.10"
     ],
     install_requires=[
```

