# Comparing `tmp/milvus_ingestion-0.1.0.tar.gz` & `tmp/milvus_ingestion-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "milvus_ingestion-0.1.0.tar", last modified: Sun May 14 11:59:06 2023, max compression
+gzip compressed data, was "milvus_ingestion-0.2.0.tar", last modified: Sun May 14 12:40:33 2023, max compression
```

## Comparing `milvus_ingestion-0.1.0.tar` & `milvus_ingestion-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 michaelmo   (501) staff       (20)        0 2023-05-14 11:59:06.103111 milvus_ingestion-0.1.0/
--rw-r--r--   0 michaelmo   (501) staff       (20)    11357 2023-05-14 11:15:24.000000 milvus_ingestion-0.1.0/LICENSE
--rw-r--r--   0 michaelmo   (501) staff       (20)      631 2023-05-14 11:59:06.102833 milvus_ingestion-0.1.0/PKG-INFO
--rw-r--r--   0 michaelmo   (501) staff       (20)       60 2023-05-14 11:53:58.000000 milvus_ingestion-0.1.0/README.md
-drwxr-xr-x   0 michaelmo   (501) staff       (20)        0 2023-05-14 11:59:06.101088 milvus_ingestion-0.1.0/milvus_ingestion/
--rw-r--r--   0 michaelmo   (501) staff       (20)      993 2023-05-14 11:15:24.000000 milvus_ingestion-0.1.0/milvus_ingestion/__init__.py
--rw-r--r--   0 michaelmo   (501) staff       (20)      712 2023-05-14 11:15:24.000000 milvus_ingestion-0.1.0/milvus_ingestion/constants.py
--rw-r--r--   0 michaelmo   (501) staff       (20)    13111 2023-05-14 11:15:24.000000 milvus_ingestion-0.1.0/milvus_ingestion/data_buffer.py
--rw-r--r--   0 michaelmo   (501) staff       (20)     3716 2023-05-14 11:36:24.000000 milvus_ingestion-0.1.0/milvus_ingestion/milvus_connector.py
--rw-r--r--   0 michaelmo   (501) staff       (20)     3159 2023-05-14 11:42:07.000000 milvus_ingestion-0.1.0/milvus_ingestion/uploader.py
--rw-r--r--   0 michaelmo   (501) staff       (20)     1292 2023-05-14 11:15:24.000000 milvus_ingestion-0.1.0/milvus_ingestion/util.py
-drwxr-xr-x   0 michaelmo   (501) staff       (20)        0 2023-05-14 11:59:06.102510 milvus_ingestion-0.1.0/milvus_ingestion.egg-info/
--rw-r--r--   0 michaelmo   (501) staff       (20)      631 2023-05-14 11:59:06.000000 milvus_ingestion-0.1.0/milvus_ingestion.egg-info/PKG-INFO
--rw-r--r--   0 michaelmo   (501) staff       (20)      407 2023-05-14 11:59:06.000000 milvus_ingestion-0.1.0/milvus_ingestion.egg-info/SOURCES.txt
--rw-r--r--   0 michaelmo   (501) staff       (20)        1 2023-05-14 11:59:06.000000 milvus_ingestion-0.1.0/milvus_ingestion.egg-info/dependency_links.txt
--rw-r--r--   0 michaelmo   (501) staff       (20)       44 2023-05-14 11:59:06.000000 milvus_ingestion-0.1.0/milvus_ingestion.egg-info/requires.txt
--rw-r--r--   0 michaelmo   (501) staff       (20)       17 2023-05-14 11:59:06.000000 milvus_ingestion-0.1.0/milvus_ingestion.egg-info/top_level.txt
--rw-r--r--   0 michaelmo   (501) staff       (20)       38 2023-05-14 11:59:06.103219 milvus_ingestion-0.1.0/setup.cfg
--rw-r--r--   0 michaelmo   (501) staff       (20)      946 2023-05-14 11:56:54.000000 milvus_ingestion-0.1.0/setup.py
+drwxr-xr-x   0 michaelmo   (501) staff       (20)        0 2023-05-14 12:40:33.758129 milvus_ingestion-0.2.0/
+-rw-r--r--   0 michaelmo   (501) staff       (20)    11357 2023-05-14 11:15:24.000000 milvus_ingestion-0.2.0/LICENSE
+-rw-r--r--   0 michaelmo   (501) staff       (20)     1908 2023-05-14 12:40:33.757406 milvus_ingestion-0.2.0/PKG-INFO
+-rw-r--r--   0 michaelmo   (501) staff       (20)     1337 2023-05-14 12:38:10.000000 milvus_ingestion-0.2.0/README.md
+drwxr-xr-x   0 michaelmo   (501) staff       (20)        0 2023-05-14 12:40:33.751191 milvus_ingestion-0.2.0/milvus_ingestion/
+-rw-r--r--   0 michaelmo   (501) staff       (20)      993 2023-05-14 11:15:24.000000 milvus_ingestion-0.2.0/milvus_ingestion/__init__.py
+-rw-r--r--   0 michaelmo   (501) staff       (20)      712 2023-05-14 11:15:24.000000 milvus_ingestion-0.2.0/milvus_ingestion/constants.py
+-rw-r--r--   0 michaelmo   (501) staff       (20)    13111 2023-05-14 11:15:24.000000 milvus_ingestion-0.2.0/milvus_ingestion/data_buffer.py
+-rw-r--r--   0 michaelmo   (501) staff       (20)     3716 2023-05-14 11:36:24.000000 milvus_ingestion-0.2.0/milvus_ingestion/milvus_connector.py
+-rw-r--r--   0 michaelmo   (501) staff       (20)     3159 2023-05-14 11:42:07.000000 milvus_ingestion-0.2.0/milvus_ingestion/uploader.py
+-rw-r--r--   0 michaelmo   (501) staff       (20)     1292 2023-05-14 11:15:24.000000 milvus_ingestion-0.2.0/milvus_ingestion/util.py
+drwxr-xr-x   0 michaelmo   (501) staff       (20)        0 2023-05-14 12:40:33.756603 milvus_ingestion-0.2.0/milvus_ingestion.egg-info/
+-rw-r--r--   0 michaelmo   (501) staff       (20)     1908 2023-05-14 12:40:33.000000 milvus_ingestion-0.2.0/milvus_ingestion.egg-info/PKG-INFO
+-rw-r--r--   0 michaelmo   (501) staff       (20)      407 2023-05-14 12:40:33.000000 milvus_ingestion-0.2.0/milvus_ingestion.egg-info/SOURCES.txt
+-rw-r--r--   0 michaelmo   (501) staff       (20)        1 2023-05-14 12:40:33.000000 milvus_ingestion-0.2.0/milvus_ingestion.egg-info/dependency_links.txt
+-rw-r--r--   0 michaelmo   (501) staff       (20)       44 2023-05-14 12:40:33.000000 milvus_ingestion-0.2.0/milvus_ingestion.egg-info/requires.txt
+-rw-r--r--   0 michaelmo   (501) staff       (20)       17 2023-05-14 12:40:33.000000 milvus_ingestion-0.2.0/milvus_ingestion.egg-info/top_level.txt
+-rw-r--r--   0 michaelmo   (501) staff       (20)       38 2023-05-14 12:40:33.758300 milvus_ingestion-0.2.0/setup.cfg
+-rw-r--r--   0 michaelmo   (501) staff       (20)      946 2023-05-14 12:39:45.000000 milvus_ingestion-0.2.0/setup.py
```

### Comparing `milvus_ingestion-0.1.0/LICENSE` & `milvus_ingestion-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `milvus_ingestion-0.1.0/milvus_ingestion/__init__.py` & `milvus_ingestion-0.2.0/milvus_ingestion/__init__.py`

 * *Files identical despite different names*

### Comparing `milvus_ingestion-0.1.0/milvus_ingestion/constants.py` & `milvus_ingestion-0.2.0/milvus_ingestion/constants.py`

 * *Files identical despite different names*

### Comparing `milvus_ingestion-0.1.0/milvus_ingestion/data_buffer.py` & `milvus_ingestion-0.2.0/milvus_ingestion/data_buffer.py`

 * *Files identical despite different names*

### Comparing `milvus_ingestion-0.1.0/milvus_ingestion/milvus_connector.py` & `milvus_ingestion-0.2.0/milvus_ingestion/milvus_connector.py`

 * *Files identical despite different names*

### Comparing `milvus_ingestion-0.1.0/milvus_ingestion/uploader.py` & `milvus_ingestion-0.2.0/milvus_ingestion/uploader.py`

 * *Files identical despite different names*

### Comparing `milvus_ingestion-0.1.0/milvus_ingestion/util.py` & `milvus_ingestion-0.2.0/milvus_ingestion/util.py`

 * *Files identical despite different names*

### Comparing `milvus_ingestion-0.1.0/setup.py` & `milvus_ingestion-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / 'README.md').read_text()
 
 setuptools.setup(
     name="milvus_ingestion",
-    version="0.1.0",
+    version="0.2.0",
     author='yihua.mo',
     author_email='yihua.mo@zilliz.com',
     description="A tool to help data ingestion for Milvus",
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/yhmo/milvus-ingestion',
     license="Apache-2.0",
```

