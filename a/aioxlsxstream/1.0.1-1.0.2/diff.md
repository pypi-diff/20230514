# Comparing `tmp/aioxlsxstream-1.0.1.tar.gz` & `tmp/aioxlsxstream-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/20182177/aioxlsxstream/dist/tmp70sib4vi/aioxlsxstream-1.0.1.tar", last modified: Sat May 13 21:57:33 2023, max compression
+gzip compressed data, was "/Users/20182177/aioxlsxstream/dist/tmpzt05r0xb/aioxlsxstream-1.0.2.tar", last modified: Sat May 13 22:01:35 2023, max compression
```

## Comparing `aioxlsxstream-1.0.1.tar` & `aioxlsxstream-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 20182177 (193159553) 646495703        0 2023-05-13 21:57:33.000000 aioxlsxstream-1.0.1/
--rw-r--r--   0 20182177 (193159553) 646495703     2217 2023-05-13 21:57:33.000000 aioxlsxstream-1.0.1/PKG-INFO
-drwxr-xr-x   0 20182177 (193159553) 646495703        0 2023-05-13 21:57:33.000000 aioxlsxstream-1.0.1/aioxlsxstream.egg-info/
--rw-r--r--   0 20182177 (193159553) 646495703     2217 2023-05-13 21:57:33.000000 aioxlsxstream-1.0.1/aioxlsxstream.egg-info/PKG-INFO
--rw-r--r--   0 20182177 (193159553) 646495703      307 2023-05-13 21:57:33.000000 aioxlsxstream-1.0.1/aioxlsxstream.egg-info/SOURCES.txt
--rw-r--r--   0 20182177 (193159553) 646495703       22 2023-05-13 21:57:33.000000 aioxlsxstream-1.0.1/aioxlsxstream.egg-info/requires.txt
--rw-r--r--   0 20182177 (193159553) 646495703       14 2023-05-13 21:57:33.000000 aioxlsxstream-1.0.1/aioxlsxstream.egg-info/top_level.txt
--rw-r--r--   0 20182177 (193159553) 646495703        1 2023-05-13 21:57:33.000000 aioxlsxstream-1.0.1/aioxlsxstream.egg-info/dependency_links.txt
--rw-r--r--   0 20182177 (193159553) 646495703    35147 2023-05-13 21:02:02.000000 aioxlsxstream-1.0.1/LICENSE
--rw-r--r--   0 20182177 (193159553) 646495703     1659 2023-05-13 21:55:39.000000 aioxlsxstream-1.0.1/README.md
--rw-r--r--   0 20182177 (193159553) 646495703      828 2023-05-13 21:56:55.000000 aioxlsxstream-1.0.1/setup.py
-drwxr-xr-x   0 20182177 (193159553) 646495703        0 2023-05-13 21:57:33.000000 aioxlsxstream-1.0.1/aioxlsxstream/
-drwxr-xr-x   0 20182177 (193159553) 646495703        0 2023-05-13 21:57:33.000000 aioxlsxstream-1.0.1/aioxlsxstream/xlsx_template/
--rw-r--r--   0 20182177 (193159553) 646495703        0 2023-05-13 21:01:14.000000 aioxlsxstream-1.0.1/aioxlsxstream/xlsx_template/__init__.py
--rw-r--r--   0 20182177 (193159553) 646495703       36 2023-05-13 21:07:42.000000 aioxlsxstream-1.0.1/aioxlsxstream/__init__.py
--rw-r--r--   0 20182177 (193159553) 646495703     4077 2023-05-13 21:34:32.000000 aioxlsxstream-1.0.1/aioxlsxstream/aioxlsxstream.py
--rw-r--r--   0 20182177 (193159553) 646495703       38 2023-05-13 21:57:33.000000 aioxlsxstream-1.0.1/setup.cfg
+drwxr-xr-x   0 20182177 (193159553) 646495703        0 2023-05-13 22:01:35.000000 aioxlsxstream-1.0.2/
+-rw-r--r--   0 20182177 (193159553) 646495703     2218 2023-05-13 22:01:35.000000 aioxlsxstream-1.0.2/PKG-INFO
+drwxr-xr-x   0 20182177 (193159553) 646495703        0 2023-05-13 22:01:35.000000 aioxlsxstream-1.0.2/aioxlsxstream.egg-info/
+-rw-r--r--   0 20182177 (193159553) 646495703     2218 2023-05-13 22:01:35.000000 aioxlsxstream-1.0.2/aioxlsxstream.egg-info/PKG-INFO
+-rw-r--r--   0 20182177 (193159553) 646495703      307 2023-05-13 22:01:35.000000 aioxlsxstream-1.0.2/aioxlsxstream.egg-info/SOURCES.txt
+-rw-r--r--   0 20182177 (193159553) 646495703       22 2023-05-13 22:01:35.000000 aioxlsxstream-1.0.2/aioxlsxstream.egg-info/requires.txt
+-rw-r--r--   0 20182177 (193159553) 646495703       14 2023-05-13 22:01:35.000000 aioxlsxstream-1.0.2/aioxlsxstream.egg-info/top_level.txt
+-rw-r--r--   0 20182177 (193159553) 646495703        1 2023-05-13 22:01:35.000000 aioxlsxstream-1.0.2/aioxlsxstream.egg-info/dependency_links.txt
+-rw-r--r--   0 20182177 (193159553) 646495703    35147 2023-05-13 21:02:02.000000 aioxlsxstream-1.0.2/LICENSE
+-rw-r--r--   0 20182177 (193159553) 646495703     1660 2023-05-13 21:58:54.000000 aioxlsxstream-1.0.2/README.md
+-rw-r--r--   0 20182177 (193159553) 646495703      828 2023-05-13 21:59:00.000000 aioxlsxstream-1.0.2/setup.py
+drwxr-xr-x   0 20182177 (193159553) 646495703        0 2023-05-13 22:01:35.000000 aioxlsxstream-1.0.2/aioxlsxstream/
+drwxr-xr-x   0 20182177 (193159553) 646495703        0 2023-05-13 22:01:35.000000 aioxlsxstream-1.0.2/aioxlsxstream/xlsx_template/
+-rw-r--r--   0 20182177 (193159553) 646495703        0 2023-05-13 21:01:14.000000 aioxlsxstream-1.0.2/aioxlsxstream/xlsx_template/__init__.py
+-rw-r--r--   0 20182177 (193159553) 646495703       36 2023-05-13 21:07:42.000000 aioxlsxstream-1.0.2/aioxlsxstream/__init__.py
+-rw-r--r--   0 20182177 (193159553) 646495703     4077 2023-05-13 21:34:32.000000 aioxlsxstream-1.0.2/aioxlsxstream/aioxlsxstream.py
+-rw-r--r--   0 20182177 (193159553) 646495703       38 2023-05-13 22:01:35.000000 aioxlsxstream-1.0.2/setup.cfg
```

### Comparing `aioxlsxstream-1.0.1/PKG-INFO` & `aioxlsxstream-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxlsxstream
-Version: 1.0.1
+Version: 1.0.2
 Summary: Asynchronous xlsx files generator
 Home-page: https://github.com/lososkin/aioxlsxstream
 Author: lososkin
 Author-email: yalososka@gmail.com
 License: UNKNOWN
 Keywords: async xlsx streaming
 Platform: UNKNOWN
@@ -14,15 +14,15 @@
 Classifier: Topic :: System :: Archiving :: Compression
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # aioxlsxstream
 
-Generate the xlsx file on fly without storing enire file in memory.
+Generate the xlsx file on fly without storing entire file in memory.
 Generated excel workbook contain only one sheet. All data writes as strings.
 
 ## Installation
 
 ```
 pip install aioxlsxstream
 ```
```

### Comparing `aioxlsxstream-1.0.1/aioxlsxstream.egg-info/PKG-INFO` & `aioxlsxstream-1.0.2/aioxlsxstream.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxlsxstream
-Version: 1.0.1
+Version: 1.0.2
 Summary: Asynchronous xlsx files generator
 Home-page: https://github.com/lososkin/aioxlsxstream
 Author: lososkin
 Author-email: yalososka@gmail.com
 License: UNKNOWN
 Keywords: async xlsx streaming
 Platform: UNKNOWN
@@ -14,15 +14,15 @@
 Classifier: Topic :: System :: Archiving :: Compression
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # aioxlsxstream
 
-Generate the xlsx file on fly without storing enire file in memory.
+Generate the xlsx file on fly without storing entire file in memory.
 Generated excel workbook contain only one sheet. All data writes as strings.
 
 ## Installation
 
 ```
 pip install aioxlsxstream
 ```
```

### Comparing `aioxlsxstream-1.0.1/LICENSE` & `aioxlsxstream-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aioxlsxstream-1.0.1/README.md` & `aioxlsxstream-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 # aioxlsxstream
 
-Generate the xlsx file on fly without storing enire file in memory.
+Generate the xlsx file on fly without storing entire file in memory.
 Generated excel workbook contain only one sheet. All data writes as strings.
 
 ## Installation
 
 ```
 pip install aioxlsxstream
 ```
```

### Comparing `aioxlsxstream-1.0.1/setup.py` & `aioxlsxstream-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='aioxlsxstream',
-    version='1.0.1',
+    version='1.0.2',
     description='Asynchronous xlsx files generator',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='lososkin',
     author_email='yalososka@gmail.com',
     url='https://github.com/lososkin/aioxlsxstream',
     packages=find_packages(exclude=['tests']),
```

### Comparing `aioxlsxstream-1.0.1/aioxlsxstream/aioxlsxstream.py` & `aioxlsxstream-1.0.2/aioxlsxstream/aioxlsxstream.py`

 * *Files identical despite different names*

