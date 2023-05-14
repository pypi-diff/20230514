# Comparing `tmp/docbuild-0.1.107.tar.gz` & `tmp/docbuild-0.1.108.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docbuild-0.1.107.tar", last modified: Thu May 11 14:33:03 2023, max compression
+gzip compressed data, was "docbuild-0.1.108.tar", last modified: Sun May 14 09:02:55 2023, max compression
```

## Comparing `docbuild-0.1.107.tar` & `docbuild-0.1.108.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-11 14:33:03.684638 docbuild-0.1.107/
--rw-r--r--   0 moran      (501) staff       (20)      566 2023-05-11 14:33:03.684442 docbuild-0.1.107/PKG-INFO
--rw-r--r--   0 moran      (501) staff       (20)       81 2023-04-19 09:08:24.000000 docbuild-0.1.107/README.md
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-11 14:33:03.680322 docbuild-0.1.107/docbuild/
--rw-r--r--   0 moran      (501) staff       (20)       63 2023-05-11 14:32:02.000000 docbuild-0.1.107/docbuild/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)      439 2023-04-20 11:04:19.000000 docbuild-0.1.107/docbuild/constants.py
--rw-r--r--   0 moran      (501) staff       (20)     5392 2023-04-19 07:35:54.000000 docbuild-0.1.107/docbuild/graph.py
--rw-r--r--   0 moran      (501) staff       (20)     4478 2023-04-19 09:10:05.000000 docbuild-0.1.107/docbuild/hocr_parser.py
--rw-r--r--   0 moran      (501) staff       (20)     7055 2023-05-11 14:28:20.000000 docbuild-0.1.107/docbuild/page_creator.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-11 14:33:03.682676 docbuild-0.1.107/docbuild/paragraph_detection/
--rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:00:49.000000 docbuild-0.1.107/docbuild/paragraph_detection/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)      175 2023-04-19 06:33:46.000000 docbuild-0.1.107/docbuild/paragraph_detection/constants.py
--rw-r--r--   0 moran      (501) staff       (20)     6831 2023-04-20 11:03:50.000000 docbuild-0.1.107/docbuild/paragraph_detection/paragraph_extractor.py
--rw-r--r--   0 moran      (501) staff       (20)     2416 2023-04-19 06:16:08.000000 docbuild-0.1.107/docbuild/paragraph_detection/paragraph_sorter.py
--rw-r--r--   0 moran      (501) staff       (20)     2703 2023-04-19 06:00:43.000000 docbuild-0.1.107/docbuild/paragraph_detection/two_columns.py
--rw-r--r--   0 moran      (501) staff       (20)     6087 2023-05-08 09:07:21.000000 docbuild-0.1.107/docbuild/textract_parser.py
--rw-r--r--   0 moran      (501) staff       (20)      816 2023-04-19 06:53:00.000000 docbuild-0.1.107/docbuild/utils.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-11 14:33:03.683932 docbuild-0.1.107/docbuild/visual_detection/
--rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:03:44.000000 docbuild-0.1.107/docbuild/visual_detection/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)    12923 2023-05-09 11:47:03.000000 docbuild-0.1.107/docbuild/visual_detection/bordered_table_extraction.py
--rw-r--r--   0 moran      (501) staff       (20)      218 2023-04-30 11:54:41.000000 docbuild-0.1.107/docbuild/visual_detection/constants.py
--rw-r--r--   0 moran      (501) staff       (20)    16349 2023-05-11 14:30:30.000000 docbuild-0.1.107/docbuild/visual_detection/vis_line_detection.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-11 14:33:03.681321 docbuild-0.1.107/docbuild.egg-info/
--rw-r--r--   0 moran      (501) staff       (20)      566 2023-05-11 14:33:03.000000 docbuild-0.1.107/docbuild.egg-info/PKG-INFO
--rw-r--r--   0 moran      (501) staff       (20)      741 2023-05-11 14:33:03.000000 docbuild-0.1.107/docbuild.egg-info/SOURCES.txt
--rw-r--r--   0 moran      (501) staff       (20)        1 2023-05-11 14:33:03.000000 docbuild-0.1.107/docbuild.egg-info/dependency_links.txt
--rw-r--r--   0 moran      (501) staff       (20)       97 2023-05-11 14:33:03.000000 docbuild-0.1.107/docbuild.egg-info/requires.txt
--rw-r--r--   0 moran      (501) staff       (20)        9 2023-05-11 14:33:03.000000 docbuild-0.1.107/docbuild.egg-info/top_level.txt
--rw-r--r--   0 moran      (501) staff       (20)       38 2023-05-11 14:33:03.684687 docbuild-0.1.107/setup.cfg
--rw-r--r--   0 moran      (501) staff       (20)      856 2023-05-11 14:31:56.000000 docbuild-0.1.107/setup.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-14 09:02:55.472605 docbuild-0.1.108/
+-rw-r--r--   0 moran      (501) staff       (20)      566 2023-05-14 09:02:55.472454 docbuild-0.1.108/PKG-INFO
+-rw-r--r--   0 moran      (501) staff       (20)       81 2023-04-19 09:08:24.000000 docbuild-0.1.108/README.md
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-14 09:02:55.468318 docbuild-0.1.108/docbuild/
+-rw-r--r--   0 moran      (501) staff       (20)       63 2023-05-14 09:02:45.000000 docbuild-0.1.108/docbuild/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)      439 2023-04-20 11:04:19.000000 docbuild-0.1.108/docbuild/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)     5392 2023-04-19 07:35:54.000000 docbuild-0.1.108/docbuild/graph.py
+-rw-r--r--   0 moran      (501) staff       (20)     4478 2023-04-19 09:10:05.000000 docbuild-0.1.108/docbuild/hocr_parser.py
+-rw-r--r--   0 moran      (501) staff       (20)     7055 2023-05-11 14:28:20.000000 docbuild-0.1.108/docbuild/page_creator.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-14 09:02:55.470611 docbuild-0.1.108/docbuild/paragraph_detection/
+-rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:00:49.000000 docbuild-0.1.108/docbuild/paragraph_detection/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)      175 2023-04-19 06:33:46.000000 docbuild-0.1.108/docbuild/paragraph_detection/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)     6831 2023-04-20 11:03:50.000000 docbuild-0.1.108/docbuild/paragraph_detection/paragraph_extractor.py
+-rw-r--r--   0 moran      (501) staff       (20)     2416 2023-04-19 06:16:08.000000 docbuild-0.1.108/docbuild/paragraph_detection/paragraph_sorter.py
+-rw-r--r--   0 moran      (501) staff       (20)     2703 2023-04-19 06:00:43.000000 docbuild-0.1.108/docbuild/paragraph_detection/two_columns.py
+-rw-r--r--   0 moran      (501) staff       (20)     6087 2023-05-08 09:07:21.000000 docbuild-0.1.108/docbuild/textract_parser.py
+-rw-r--r--   0 moran      (501) staff       (20)      816 2023-04-19 06:53:00.000000 docbuild-0.1.108/docbuild/utils.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-14 09:02:55.472137 docbuild-0.1.108/docbuild/visual_detection/
+-rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:03:44.000000 docbuild-0.1.108/docbuild/visual_detection/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)    12923 2023-05-09 11:47:03.000000 docbuild-0.1.108/docbuild/visual_detection/bordered_table_extraction.py
+-rw-r--r--   0 moran      (501) staff       (20)      218 2023-04-30 11:54:41.000000 docbuild-0.1.108/docbuild/visual_detection/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)    16349 2023-05-11 14:30:30.000000 docbuild-0.1.108/docbuild/visual_detection/vis_line_detection.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-14 09:02:55.469336 docbuild-0.1.108/docbuild.egg-info/
+-rw-r--r--   0 moran      (501) staff       (20)      566 2023-05-14 09:02:55.000000 docbuild-0.1.108/docbuild.egg-info/PKG-INFO
+-rw-r--r--   0 moran      (501) staff       (20)      741 2023-05-14 09:02:55.000000 docbuild-0.1.108/docbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 moran      (501) staff       (20)        1 2023-05-14 09:02:55.000000 docbuild-0.1.108/docbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 moran      (501) staff       (20)       97 2023-05-14 09:02:55.000000 docbuild-0.1.108/docbuild.egg-info/requires.txt
+-rw-r--r--   0 moran      (501) staff       (20)        9 2023-05-14 09:02:55.000000 docbuild-0.1.108/docbuild.egg-info/top_level.txt
+-rw-r--r--   0 moran      (501) staff       (20)       38 2023-05-14 09:02:55.472663 docbuild-0.1.108/setup.cfg
+-rw-r--r--   0 moran      (501) staff       (20)      856 2023-05-14 09:02:46.000000 docbuild-0.1.108/setup.py
```

### Comparing `docbuild-0.1.107/PKG-INFO` & `docbuild-0.1.108/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docbuild
-Version: 0.1.107
+Version: 0.1.108
 Summary: A package for building a document from a textract response, for more information see the docstruct package
 Home-page: https://github.com/smrt-co/docbuild
 Author: Moran Nechushtan, Serah Tapia, Shlomo Agishtein
 Author-email: moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `docbuild-0.1.107/docbuild/graph.py` & `docbuild-0.1.108/docbuild/graph.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.107/docbuild/hocr_parser.py` & `docbuild-0.1.108/docbuild/hocr_parser.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.107/docbuild/page_creator.py` & `docbuild-0.1.108/docbuild/page_creator.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.107/docbuild/paragraph_detection/paragraph_extractor.py` & `docbuild-0.1.108/docbuild/paragraph_detection/paragraph_extractor.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.107/docbuild/paragraph_detection/paragraph_sorter.py` & `docbuild-0.1.108/docbuild/paragraph_detection/paragraph_sorter.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.107/docbuild/paragraph_detection/two_columns.py` & `docbuild-0.1.108/docbuild/paragraph_detection/two_columns.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.107/docbuild/textract_parser.py` & `docbuild-0.1.108/docbuild/textract_parser.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.107/docbuild/utils.py` & `docbuild-0.1.108/docbuild/utils.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.107/docbuild/visual_detection/bordered_table_extraction.py` & `docbuild-0.1.108/docbuild/visual_detection/bordered_table_extraction.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.107/docbuild/visual_detection/vis_line_detection.py` & `docbuild-0.1.108/docbuild/visual_detection/vis_line_detection.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.107/docbuild.egg-info/PKG-INFO` & `docbuild-0.1.108/docbuild.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docbuild
-Version: 0.1.107
+Version: 0.1.108
 Summary: A package for building a document from a textract response, for more information see the docstruct package
 Home-page: https://github.com/smrt-co/docbuild
 Author: Moran Nechushtan, Serah Tapia, Shlomo Agishtein
 Author-email: moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `docbuild-0.1.107/docbuild.egg-info/SOURCES.txt` & `docbuild-0.1.108/docbuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.107/setup.py` & `docbuild-0.1.108/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from setuptools import setup
 
 setup(
     name="docbuild",
-    version="0.1.107",
+    version="0.1.108",
     description="A package for building a document from a textract response, for more information see the docstruct package",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Moran Nechushtan, Serah Tapia, Shlomo Agishtein",
     author_email="moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com",
     url="https://github.com/smrt-co/docbuild",
     packages=setuptools.find_packages(),
```

