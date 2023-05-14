# Comparing `tmp/embedin-0.1.3.tar.gz` & `tmp/embedin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedin-0.1.3.tar", last modified: Sun Apr 23 00:53:51 2023, max compression
+gzip compressed data, was "embedin-0.2.0.tar", last modified: Sat May 13 23:59:15 2023, max compression
```

## Comparing `embedin-0.1.3.tar` & `embedin-0.2.0.tar`

### file list

```diff
@@ -1,60 +1,67 @@
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-23 00:53:51.272326 embedin-0.1.3/
--rw-r--r--   0 xchen375   (502) staff       (20)    11357 2023-04-10 04:12:37.000000 embedin-0.1.3/LICENSE
--rw-r--r--   0 xchen375   (502) staff       (20)     3666 2023-04-23 00:53:51.271837 embedin-0.1.3/PKG-INFO
--rw-r--r--   0 xchen375   (502) staff       (20)     3229 2023-04-23 00:43:19.000000 embedin-0.1.3/README.md
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-23 00:53:51.245940 embedin-0.1.3/embedin/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-09 17:01:17.000000 embedin-0.1.3/embedin/__init__.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-23 00:53:51.248220 embedin-0.1.3/embedin/client/
--rw-r--r--   0 xchen375   (502) staff       (20)     6261 2023-04-22 22:11:55.000000 embedin-0.1.3/embedin/client/__init__.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-23 00:53:51.249933 embedin-0.1.3/embedin/embedding/
--rw-r--r--   0 xchen375   (502) staff       (20)      130 2023-04-09 16:47:27.000000 embedin-0.1.3/embedin/embedding/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)     1817 2023-04-22 22:11:55.000000 embedin-0.1.3/embedin/embedding/sentence_transformer.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-23 00:53:51.251889 embedin-0.1.3/embedin/index/
--rw-r--r--   0 xchen375   (502) staff       (20)     1318 2023-04-22 17:06:36.000000 embedin-0.1.3/embedin/index/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)     2174 2023-04-22 22:11:55.000000 embedin-0.1.3/embedin/index/hnswlib.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-23 00:53:51.254691 embedin-0.1.3/embedin/model/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.1.3/embedin/model/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)      275 2023-04-22 15:16:27.000000 embedin-0.1.3/embedin/model/collection_model.py
--rw-r--r--   0 xchen375   (502) staff       (20)      610 2023-04-22 15:16:27.000000 embedin-0.1.3/embedin/model/embedding_model.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-23 00:53:51.257324 embedin-0.1.3/embedin/repository/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.1.3/embedin/repository/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)     2667 2023-04-22 22:11:55.000000 embedin-0.1.3/embedin/repository/collection_repository.py
--rw-r--r--   0 xchen375   (502) staff       (20)     3496 2023-04-22 22:11:55.000000 embedin-0.1.3/embedin/repository/embedding_repository.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-23 00:53:51.259933 embedin-0.1.3/embedin/service/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.1.3/embedin/service/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)     2258 2023-04-22 22:11:55.000000 embedin-0.1.3/embedin/service/collection_service.py
--rw-r--r--   0 xchen375   (502) staff       (20)     3978 2023-04-22 22:11:55.000000 embedin-0.1.3/embedin/service/embedding_service.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-23 00:53:51.260961 embedin-0.1.3/embedin/util/
--rw-r--r--   0 xchen375   (502) staff       (20)     1145 2023-04-22 22:11:55.000000 embedin-0.1.3/embedin/util/__init__.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-23 00:53:51.247835 embedin-0.1.3/embedin.egg-info/
--rw-r--r--   0 xchen375   (502) staff       (20)     3666 2023-04-23 00:53:51.000000 embedin-0.1.3/embedin.egg-info/PKG-INFO
--rw-r--r--   0 xchen375   (502) staff       (20)     1195 2023-04-23 00:53:51.000000 embedin-0.1.3/embedin.egg-info/SOURCES.txt
--rw-r--r--   0 xchen375   (502) staff       (20)        1 2023-04-23 00:53:51.000000 embedin-0.1.3/embedin.egg-info/dependency_links.txt
--rw-r--r--   0 xchen375   (502) staff       (20)      133 2023-04-23 00:53:51.000000 embedin-0.1.3/embedin.egg-info/requires.txt
--rw-r--r--   0 xchen375   (502) staff       (20)       14 2023-04-23 00:53:51.000000 embedin-0.1.3/embedin.egg-info/top_level.txt
--rw-r--r--   0 xchen375   (502) staff       (20)       38 2023-04-23 00:53:51.272467 embedin-0.1.3/setup.cfg
--rw-r--r--   0 xchen375   (502) staff       (20)      827 2023-04-23 00:43:57.000000 embedin-0.1.3/setup.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-23 00:53:51.261743 embedin-0.1.3/tests/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-10 19:13:54.000000 embedin-0.1.3/tests/__init__.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-23 00:53:51.262103 embedin-0.1.3/tests/client/
--rw-r--r--   0 xchen375   (502) staff       (20)     1795 2023-04-22 22:11:55.000000 embedin-0.1.3/tests/client/__init__.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-23 00:53:51.263600 embedin-0.1.3/tests/embedding/
--rw-r--r--   0 xchen375   (502) staff       (20)      322 2023-04-22 22:11:55.000000 embedin-0.1.3/tests/embedding/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)     1277 2023-04-22 22:11:55.000000 embedin-0.1.3/tests/embedding/test_embedding.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-23 00:53:51.264579 embedin-0.1.3/tests/index/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.1.3/tests/index/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)     1635 2023-04-22 17:06:36.000000 embedin-0.1.3/tests/index/test_hnswlib.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-23 00:53:51.266671 embedin-0.1.3/tests/model/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.1.3/tests/model/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)     1938 2023-04-22 22:11:55.000000 embedin-0.1.3/tests/model/test_collection_model.py
--rw-r--r--   0 xchen375   (502) staff       (20)     2044 2023-04-22 22:11:55.000000 embedin-0.1.3/tests/model/test_embedding_model.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-23 00:53:51.268337 embedin-0.1.3/tests/repository/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.1.3/tests/repository/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)     2479 2023-04-22 22:11:55.000000 embedin-0.1.3/tests/repository/test_collection_repository.py
--rw-r--r--   0 xchen375   (502) staff       (20)     5427 2023-04-22 22:11:55.000000 embedin-0.1.3/tests/repository/test_embedding_repository.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-23 00:53:51.270379 embedin-0.1.3/tests/service/
--rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.1.3/tests/service/__init__.py
--rw-r--r--   0 xchen375   (502) staff       (20)     1333 2023-04-22 22:11:55.000000 embedin-0.1.3/tests/service/test_collection_service.py
--rw-r--r--   0 xchen375   (502) staff       (20)     3705 2023-04-22 22:11:55.000000 embedin-0.1.3/tests/service/test_embedding_service.py
-drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-04-23 00:53:51.271098 embedin-0.1.3/tests/util/
--rw-r--r--   0 xchen375   (502) staff       (20)      827 2023-04-22 22:11:55.000000 embedin-0.1.3/tests/util/__init__.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.205288 embedin-0.2.0/
+-rw-r--r--   0 xchen375   (502) staff       (20)    11357 2023-04-10 04:12:37.000000 embedin-0.2.0/LICENSE
+-rw-r--r--   0 xchen375   (502) staff       (20)     3655 2023-05-13 23:59:15.204888 embedin-0.2.0/PKG-INFO
+-rw-r--r--   0 xchen375   (502) staff       (20)     3218 2023-05-13 23:56:49.000000 embedin-0.2.0/README.md
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.184662 embedin-0.2.0/embedin/
+-rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-09 17:01:17.000000 embedin-0.2.0/embedin/__init__.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.186886 embedin-0.2.0/embedin/client/
+-rw-r--r--   0 xchen375   (502) staff       (20)     6524 2023-05-13 23:39:26.000000 embedin-0.2.0/embedin/client/__init__.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.188462 embedin-0.2.0/embedin/embedding/
+-rw-r--r--   0 xchen375   (502) staff       (20)     1931 2023-05-13 23:39:26.000000 embedin-0.2.0/embedin/embedding/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)      134 2023-05-13 23:39:26.000000 embedin-0.2.0/embedin/embedding/embedding_base.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     1647 2023-05-13 23:39:26.000000 embedin-0.2.0/embedin/embedding/openai_embedding.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     1927 2023-05-13 23:39:26.000000 embedin-0.2.0/embedin/embedding/sentence_transformer.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.190455 embedin-0.2.0/embedin/index/
+-rw-r--r--   0 xchen375   (502) staff       (20)      693 2023-05-13 19:19:06.000000 embedin-0.2.0/embedin/index/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     2317 2023-05-13 19:19:06.000000 embedin-0.2.0/embedin/index/flat_index.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     2331 2023-05-13 19:19:06.000000 embedin-0.2.0/embedin/index/hnsw_index.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     1373 2023-05-13 19:19:06.000000 embedin-0.2.0/embedin/index/index_base.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.191821 embedin-0.2.0/embedin/model/
+-rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.2.0/embedin/model/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)      275 2023-04-22 15:16:27.000000 embedin-0.2.0/embedin/model/collection_model.py
+-rw-r--r--   0 xchen375   (502) staff       (20)      610 2023-04-22 15:16:27.000000 embedin-0.2.0/embedin/model/embedding_model.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.193244 embedin-0.2.0/embedin/repository/
+-rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.2.0/embedin/repository/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     2667 2023-04-22 22:11:55.000000 embedin-0.2.0/embedin/repository/collection_repository.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     3496 2023-04-22 22:11:55.000000 embedin-0.2.0/embedin/repository/embedding_repository.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.195504 embedin-0.2.0/embedin/service/
+-rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.2.0/embedin/service/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     2258 2023-04-22 22:11:55.000000 embedin-0.2.0/embedin/service/collection_service.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     3978 2023-04-22 22:11:55.000000 embedin-0.2.0/embedin/service/embedding_service.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.196144 embedin-0.2.0/embedin/util/
+-rw-r--r--   0 xchen375   (502) staff       (20)     1354 2023-05-13 19:19:06.000000 embedin-0.2.0/embedin/util/__init__.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.186505 embedin-0.2.0/embedin.egg-info/
+-rw-r--r--   0 xchen375   (502) staff       (20)     3655 2023-05-13 23:59:15.000000 embedin-0.2.0/embedin.egg-info/PKG-INFO
+-rw-r--r--   0 xchen375   (502) staff       (20)     1463 2023-05-13 23:59:15.000000 embedin-0.2.0/embedin.egg-info/SOURCES.txt
+-rw-r--r--   0 xchen375   (502) staff       (20)        1 2023-05-13 23:59:15.000000 embedin-0.2.0/embedin.egg-info/dependency_links.txt
+-rw-r--r--   0 xchen375   (502) staff       (20)      165 2023-05-13 23:59:15.000000 embedin-0.2.0/embedin.egg-info/requires.txt
+-rw-r--r--   0 xchen375   (502) staff       (20)       14 2023-05-13 23:59:15.000000 embedin-0.2.0/embedin.egg-info/top_level.txt
+-rw-r--r--   0 xchen375   (502) staff       (20)       38 2023-05-13 23:59:15.205399 embedin-0.2.0/setup.cfg
+-rw-r--r--   0 xchen375   (502) staff       (20)      841 2023-05-13 23:58:06.000000 embedin-0.2.0/setup.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.196664 embedin-0.2.0/tests/
+-rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-10 19:13:54.000000 embedin-0.2.0/tests/__init__.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.196976 embedin-0.2.0/tests/client/
+-rw-r--r--   0 xchen375   (502) staff       (20)     2163 2023-05-13 23:39:26.000000 embedin-0.2.0/tests/client/__init__.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.198465 embedin-0.2.0/tests/embedding/
+-rw-r--r--   0 xchen375   (502) staff       (20)     1282 2023-05-13 23:39:26.000000 embedin-0.2.0/tests/embedding/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)      296 2023-05-13 23:39:26.000000 embedin-0.2.0/tests/embedding/test_embedding_base.py
+-rw-r--r--   0 xchen375   (502) staff       (20)      818 2023-05-13 23:39:26.000000 embedin-0.2.0/tests/embedding/test_openai_embedding.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     1398 2023-05-13 23:39:26.000000 embedin-0.2.0/tests/embedding/test_sentence_transformer_embedding.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.199806 embedin-0.2.0/tests/index/
+-rw-r--r--   0 xchen375   (502) staff       (20)     2065 2023-05-13 19:19:06.000000 embedin-0.2.0/tests/index/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     2593 2023-05-13 19:19:06.000000 embedin-0.2.0/tests/index/test_flat_index.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     2939 2023-05-13 19:19:06.000000 embedin-0.2.0/tests/index/test_hnsw_index.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.201147 embedin-0.2.0/tests/model/
+-rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.2.0/tests/model/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     1938 2023-04-22 22:11:55.000000 embedin-0.2.0/tests/model/test_collection_model.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     2044 2023-04-22 22:11:55.000000 embedin-0.2.0/tests/model/test_embedding_model.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.202544 embedin-0.2.0/tests/repository/
+-rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.2.0/tests/repository/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     2479 2023-04-22 22:11:55.000000 embedin-0.2.0/tests/repository/test_collection_repository.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     5427 2023-04-22 22:11:55.000000 embedin-0.2.0/tests/repository/test_embedding_repository.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.203857 embedin-0.2.0/tests/service/
+-rw-r--r--   0 xchen375   (502) staff       (20)        0 2023-04-22 15:16:27.000000 embedin-0.2.0/tests/service/__init__.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     1333 2023-04-22 22:11:55.000000 embedin-0.2.0/tests/service/test_collection_service.py
+-rw-r--r--   0 xchen375   (502) staff       (20)     3705 2023-04-22 22:11:55.000000 embedin-0.2.0/tests/service/test_embedding_service.py
+drwxr-xr-x   0 xchen375   (502) staff       (20)        0 2023-05-13 23:59:15.204300 embedin-0.2.0/tests/util/
+-rw-r--r--   0 xchen375   (502) staff       (20)     1588 2023-05-13 19:19:06.000000 embedin-0.2.0/tests/util/__init__.py
```

### Comparing `embedin-0.1.3/LICENSE` & `embedin-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `embedin-0.1.3/PKG-INFO` & `embedin-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,29 @@
-Metadata-Version: 2.1
-Name: embedin
-Version: 0.1.3
-Summary: A lightweight vector database
-Home-page: https://github.com/EmbedInAI/EmbedInDB
-Author: EmbedInAI
-Author-email: EmbedInAI@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Embedin
+# Embedin - Empower AI with persistent memory
 [![PyPI](https://img.shields.io/pypi/v/embedin?label=embedin)](https://pypi.org/project/embedin/)
 [![Coverage Status](https://coveralls.io/repos/github/EmbedInAI/EmbedInDB/badge.svg)](https://coveralls.io/github/EmbedInAI/EmbedInDB)
 
+## What is Embedin
+Embedin is a highly efficient software library designed to seamlessly convert widely-used databases, such as MySQL, PostgreSQL, and MS SQL Server, into a vector database with minimal effort. Its lightweight design enables quick and easy integration into your existing software stack, allowing you to leverage the benefits of a vector database without the need for extensive modifications to your current system. 
+
+With fast indexing and retrieval, it's ideal for high-performance applications such as natural language processing, image recognition, and recommendation systems. Embedin's simple API and query language make it easy to use and integrate. 
+
 ## Installation
 ```bash
 pip install embedin
 ```
 
 ## Quick Start
-### Using memery DB
+### Using memory DB
 ```python
 from embedin.client import Client
 
 client = Client(collection_name="test_collection")
 client.add_data(texts=["This is a test"], meta_data=[{"source": "abc4"}])
 result = client.query("These are tests", top_k=1)
-
-print("result: ", result)
 ```
 
 ### Using sqlite with local storage
 ```python
 from embedin.client import Client
 
 url = 'sqlite:///test.db'
@@ -45,39 +34,39 @@
 
 ### Using PostgreSQL
 ```python
 import os
 
 from embedin.client import Client
 
-url = os.environ.get('EMBEDIN_POSGRES_URL', "postgresql+psycopg2://embedin:embedin@localhost/embedin_db")
+url = os.getenv('EMBEDIN_POSGRES_URL', "postgresql+psycopg2://embedin:embedin@localhost/embedin_db")
 client = Client(collection_name="test_collection", url=url)
 client.add_data(texts=["This is a test"], meta_data=[{"source": "abc4"}])
 result = client.query("These are tests", top_k=1)
 ```
 
 ### Using MySQL
 ```python
 import os
 
 from embedin.client import Client
 
-url = os.environ.get('EMBEDIN_MYSQL_URL', "mysql+pymysql://embedin:embedin@localhost/embedin_db")
+url = os.getenv('EMBEDIN_MYSQL_URL', "mysql+pymysql://embedin:embedin@localhost/embedin_db")
 client = Client(collection_name="test_collection", url=url)
 client.add_data(texts=["This is a test"], meta_data=[{"source": "abc4"}])
 result = client.query("These are tests", top_k=1)
 ```
 
 ### Using MS-SQL
 ```python
 import os
 
 from embedin.client import Client
 
-url = os.environ.get('EMBEDIN_MSSQL_URL', "mssql+pymssql://sa:StrongPassword123@localhost/tempdb")
+url = os.getenv('EMBEDIN_MSSQL_URL', "mssql+pymssql://sa:StrongPassword123@localhost/tempdb")
 client = Client(collection_name="test_collection", url=url)
 client.add_data(texts=["This is a test"], meta_data=[{"source": "abc4"}])
 result = client.query("These are tests", top_k=1)
 ```
 
 ## For development
 
@@ -100,42 +89,12 @@
 
 Start MS-SQL DB (Only necessary for using MS-SQL as the storage)
 ```bash
 cd docker
 docker-compose up embedin-mssql
 ```
 
-Start Oracle DB (Only necessary for using Oracle as the storage) - not supported yet
-
-docker login container-registry.oracle.com
-```bash
-cd docker
-docker-compose up embedin-oracle
-```yaml
-  embedin-oracle:
-    container_name: embedin-oracle
-    image: container-registry.oracle.com/database/enterprise:21.3.0.0
-    environment:
-      - ORACLE_SID=ORCLCDB
-      - ORACLE_PWD=password
-      - ORACLE_PDB=ORCLPDB1
-      - ORACLE_CHARACTERSET=AL32UTF8
-    volumes:
-      - ./oracle/data:/opt/oracle/oradata
-    ports:
-      - "1521:1521"
-```
-
 Run unit test with coverage report
 ```bash
 coverage run -m unittest discover -s tests -p '*.py'
 coverage report
-```
-
-To publish to PyPI
-```bash
-pip install twine
-```
-
-```bash
-python setup.py sdist && python setup.py bdist_wheel && twine upload dist/*
-```
+```
```

### Comparing `embedin-0.1.3/embedin/client/__init__.py` & `embedin-0.2.0/embedin/client/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,80 +1,86 @@
 import logging
 
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker
 
-from embedin.embedding.sentence_transformer import SentenceTransformerEmbedding
-from embedin.index.hnswlib import HNSWNearestNeighbors
+from embedin.embedding import Embedding
+from embedin.index import Index
 from embedin.service.collection_service import CollectionService
 from embedin.service.embedding_service import EmbeddingService
 
 # Configure the root logger to output to the console
 logging.basicConfig(
     format="%(asctime)s - %(levelname)s - %(message)s", level=logging.INFO
 )
 
 logger = logging.getLogger(__name__)
 
 
 class Client:
     """
-        Client class for managing embeddings and performing nearest neighbor search.
+    Client class for managing embeddings and performing nearest neighbor search.
 
-        Args:
-            collection_name (str): Name of the collection.
-            url (str, optional): Database URL. Defaults to None.
-            embedding_fn (EmbeddingFunction, optional): Embedding function to use. Defaults to SentenceTransformerEmbedding().
-            debug (bool, optional): Enable debug mode. Defaults to False.
-
-        Attributes:
-            collection_id (int): ID of the collection.
-            embedding_fn (EmbeddingFunction): Embedding function to use.
-            session (Session): SQLAlchemy session.
-            collection_service (CollectionService): CollectionService instance.
-            embedding_service (EmbeddingService): EmbeddingService instance.
-            embeddings (List[Embedding]): List of Embedding instances for the current collection.
-            nearest_neighbors (HNSWNearestNeighbors): HNSW nearest neighbor index for the current collection.
-
-        Methods:
-            create_or_get_collection(name): Get the ID of an existing collection or create a new one.
-            create_collection(name): Create a new collection with the given name.
-            get_collection(name): Get the ID of an existing collection with the given name.
-            add_data(texts, meta_data=None): Add new data to the collection.
-            query(query_texts, top_k=3): Find nearest neighbors for the given query text(s).
-        """
+    Args:
+        collection_name (str): Name of the collection.
+        url (str, optional): Database URL. Defaults to None.
+        embedding_fn (str or EmbeddingFunction, optional): The embedding function to use. The default is the SentenceTransformer model. Supported options are 'sentence_transformer' and 'openai'. If 'openai' is selected, the 'OPENAI_API_KEY' environment variable must be set to authenticate with the OpenAI API.
+        index_hint (str, optional): Similarity search index to use. Supports: 'flat' and 'hnsw'
+        debug (bool, optional): Enable debug mode. Defaults to False.
+
+    Attributes:
+        collection_id (int): ID of the collection.
+        embedding_fn (str or EmbeddingFunction): Embedding function to use. Support 'sentence_transformer' and 'openai'.
+        session (Session): SQLAlchemy session.
+        collection_service (CollectionService): CollectionService instance.
+        embedding_service (EmbeddingService): EmbeddingService instance.
+        embedding_rows (List[EmbeddingModel]): List of Embedding instances for the current collection.
+
+    Methods:
+        create_or_get_collection(name): Get the ID of an existing collection or create a new one.
+        create_collection(name): Create a new collection with the given name.
+        get_collection(name): Get the ID of an existing collection with the given name.
+        add_data(texts, meta_data=None): Add new data to the collection.
+        query(query_texts, top_k=3): Find nearest neighbors for the given query text(s).
+    """
 
     def __init__(
         self,
         collection_name,
         url=None,
-        embedding_fn=SentenceTransformerEmbedding(),
+        embedding_fn="sentence_transformer",
+        index_hint=None,
         debug=False,
     ):
         self.collection_id = None
-        self.embedding_fn = embedding_fn
+
+        if callable(embedding_fn):
+            self.embedding_fn = embedding_fn
+        else:
+            self.embedding_fn = Embedding.create_embedding(embedding_fn)
 
         if url is None:
             engine = create_engine("sqlite:///:memory:", echo=debug)
         else:
             engine = create_engine(url)
 
         session = sessionmaker(bind=engine)
         self.session = session()
 
         self.collection_service = CollectionService(self.session)
         self.embedding_service = EmbeddingService(self.session)
 
         collection_id = self.create_or_get_collection(collection_name)
-        self.embeddings = self.embedding_service.get_by_collection_id(collection_id)
-        embeddings = [row.embedding_data for row in self.embeddings]
+        self.embedding_rows = self.embedding_service.get_by_collection_id(collection_id)
+        embeddings = [row.embedding_data for row in self.embedding_rows]
 
-        self.nearest_neighbors = None
+        self.index_hint = index_hint
+        self.search_index = None
         if embeddings:
-            self.nearest_neighbors = HNSWNearestNeighbors(embeddings)
+            self.search_index = Index(embeddings, self.index_hint)
 
     def create_or_get_collection(self, name):
         """
         Get the ID of an existing collection or create a new one with the given name.
 
         Args:
             name (str): Name of the collection.
@@ -130,22 +136,22 @@
         """
         embeddings = self.embedding_fn(texts)
         inserted_data = self.embedding_service.add_all(
             self.collection_id, embeddings, texts, meta_data
         )
         logger.info("inserted_data: %s", inserted_data)
 
-        self.embeddings += inserted_data
+        self.embedding_rows += inserted_data
 
         inserted_embeddings = [row.embedding_data for row in inserted_data]
 
-        if self.nearest_neighbors is None:
-            self.nearest_neighbors = HNSWNearestNeighbors(embeddings)
+        if self.search_index is None:
+            self.search_index = Index(embeddings, self.index_hint)
         else:
-            self.nearest_neighbors.update_index(inserted_embeddings)
+            self.search_index.update_index(inserted_embeddings)
 
     def query(self, query_texts, top_k=3):
         """
         Search for the most similar text data in the collection to the given query text.
 
         Args:
             query_texts (list or str): List of query text strings or a single query text string.
@@ -155,14 +161,14 @@
             list of dict: A list of dictionaries containing the most similar text data in the collection to the given query text.
                           Each dictionary has the following format:
                           {'text': str, 'meta_data': object or None}
         """
         if isinstance(query_texts, str):
             query_texts = [query_texts]
         query_embeddings = self.embedding_fn(query_texts)
-        indices = self.nearest_neighbors.search(query_embeddings, top_k)
+        indices = self.search_index.search(query_embeddings, top_k)
         matched_embeddings = [
             {"text": r.text, "meta_data": r.meta_data}
-            for i, r in enumerate(self.embeddings)
+            for i, r in enumerate(self.embedding_rows)
             if i in indices
         ]
         return matched_embeddings
```

### Comparing `embedin-0.1.3/embedin/embedding/sentence_transformer.py` & `embedin-0.2.0/embedin/embedding/sentence_transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from sentence_transformers import SentenceTransformer
 
-from embedin.embedding import Embedding
+from embedin.embedding.embedding_base import EmbeddingBase
 
 
-class SentenceTransformerEmbedding(Embedding):
+class SentenceTransformerEmbedding(EmbeddingBase):
     """
     A class for generating text embeddings using the SentenceTransformer model.
 
     Args:
     model_name (str): The name or path of the SentenceTransformer model to be used for generating embeddings. Default is "all-MiniLM-L6-v2".
 
     Methods:
     __call__(texts):
     Generates embeddings for the given input text(s).
 
     Returns:
     embeddings (list): A list of embeddings generated for the input text(s). Each embedding is a list of float values.
     """
 
-    def __init__(self, model_name="all-MiniLM-L6-v2"):
+    def __init__(self, model="all-MiniLM-L6-v2"):
         """
         Initialize a SentenceTransformerEmbedding object.
 
         Args:
         model_name (str): The name or path of the SentenceTransformer model to be used for generating embeddings. Default is "all-MiniLM-L6-v2".
         """
-        self.model = SentenceTransformer(model_name)
+        self.model = SentenceTransformer(model)
 
     def __call__(self, texts):
         """
         Generates embeddings for the given input text(s).
 
         Args:
         texts (str/list): The input text(s) for which embeddings are to be generated. It can be a string or a list of strings.
@@ -38,11 +38,12 @@
         embeddings (list): A list of embeddings generated for the input text(s). Each embedding is a list of float values.
         """
         # Return it as a numpy array
         # Check if texts is a string
         if isinstance(texts, str):
             return self.model.encode([texts], convert_to_numpy=True).tolist()
         # Check if texts is a list of strings
-        elif all(isinstance(text, str) for text in texts):
-            return self.model.encode(texts, convert_to_numpy=True).tolist()
-        else:
+        if isinstance(texts, list):
+            if all(isinstance(text, str) for text in texts):
+                return self.model.encode(texts, convert_to_numpy=True).tolist()
             raise TypeError("Input must be a string, a list of strings")
+        raise TypeError("Input must be a string, a list of strings")
```

### Comparing `embedin-0.1.3/embedin/index/__init__.py` & `embedin-0.2.0/embedin/index/index_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABC, abstractmethod
 
 from embedin.util import to_np_array
 
 
-class NearestNeighbors(ABC):
+class IndexBase(ABC):
     def __init__(self, embeddings):
         """
         Args:
             embeddings: A list of embeddings, where each embedding is a list
             or array of floats.
         """
         self.embeddings = to_np_array(embeddings)
@@ -40,7 +40,10 @@
            corresponding distances.
         """
         count = len(self.embeddings)
         top_k = min(top_k, count)
         query_embeddings = to_np_array(query_embeddings)
         indices = self._search_index(query_embeddings, top_k)
         return indices
+
+    def get_embeddings(self):
+        return self.embeddings
```

### Comparing `embedin-0.1.3/embedin/index/hnswlib.py` & `embedin-0.2.0/embedin/index/hnsw_index.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 import numpy as np
-from hnswlib import Index as HNSWIndex
-from embedin.index import NearestNeighbors, to_np_array
+from hnswlib import Index
 
+from embedin.index.index_base import IndexBase
+from embedin.util import to_np_array
 
-class HNSWNearestNeighbors(NearestNeighbors):
+
+class HNSWIndex(IndexBase):
     """
     This class implements a nearest neighbors search with HNSW algorithm using cosine similarity metric.
     Inherits from the abstract class 'NearestNeighbors'.
     """
 
     # TODO: save index to DB; load index from DB
     def _build_index(self):
         """
         Build an index using the HNSW algorithm with the cosine similarity metric and returns it.
 
         Returns:
         -------
-        index: HNSWIndex
+        index: Index
             The index built using HNSW algorithm.
         """
 
-        # TODO: double check all those magic numbers
-        index = HNSWIndex("cosine", self.embeddings.shape[1])
+        # M - vertex nearest neighbors, affect index size linearly
+        # ef_construction - depth of search during build
+
+        ef_search = 128  # depth of search during search
+        d = self.embeddings.shape[1]  # dimension
+
+        index = Index("cosine", d)
         index.init_index(
-            max_elements=self.embeddings.shape[0], ef_construction=100, M=16
+            max_elements=self.embeddings.shape[0], ef_construction=64, M=32
         )
         index.add_items(self.embeddings)
-        index.set_ef(100)
+        index.set_ef(ef_search)
         return index
 
     def update_index(self, embeddings):
         """
         Updates the index with new embeddings.
 
         Parameters:
@@ -60,9 +67,9 @@
 
         Returns:
         -------
         indices: numpy array
             Array of indices representing the nearest embeddings to the given query embeddings.
         """
 
-        indices, _ = self.index.knn_query(query_embeddings, k=top_k)
-        return indices[0]
+        indices, distances = self.index.knn_query(query_embeddings, k=top_k)
+        return indices
```

### Comparing `embedin-0.1.3/embedin/model/embedding_model.py` & `embedin-0.2.0/embedin/model/embedding_model.py`

 * *Files identical despite different names*

### Comparing `embedin-0.1.3/embedin/repository/collection_repository.py` & `embedin-0.2.0/embedin/repository/collection_repository.py`

 * *Files identical despite different names*

### Comparing `embedin-0.1.3/embedin/repository/embedding_repository.py` & `embedin-0.2.0/embedin/repository/embedding_repository.py`

 * *Files identical despite different names*

### Comparing `embedin-0.1.3/embedin/service/collection_service.py` & `embedin-0.2.0/embedin/service/collection_service.py`

 * *Files identical despite different names*

### Comparing `embedin-0.1.3/embedin/service/embedding_service.py` & `embedin-0.2.0/embedin/service/embedding_service.py`

 * *Files identical despite different names*

### Comparing `embedin-0.1.3/embedin.egg-info/PKG-INFO` & `embedin-0.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 Metadata-Version: 2.1
 Name: embedin
-Version: 0.1.3
+Version: 0.2.0
 Summary: A lightweight vector database
 Home-page: https://github.com/EmbedInAI/EmbedInDB
 Author: EmbedInAI
 Author-email: EmbedInAI@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Embedin
+# Embedin - Empower AI with persistent memory
 [![PyPI](https://img.shields.io/pypi/v/embedin?label=embedin)](https://pypi.org/project/embedin/)
 [![Coverage Status](https://coveralls.io/repos/github/EmbedInAI/EmbedInDB/badge.svg)](https://coveralls.io/github/EmbedInAI/EmbedInDB)
 
+## What is Embedin
+Embedin is a highly efficient software library designed to seamlessly convert widely-used databases, such as MySQL, PostgreSQL, and MS SQL Server, into a vector database with minimal effort. Its lightweight design enables quick and easy integration into your existing software stack, allowing you to leverage the benefits of a vector database without the need for extensive modifications to your current system. 
+
+With fast indexing and retrieval, it's ideal for high-performance applications such as natural language processing, image recognition, and recommendation systems. Embedin's simple API and query language make it easy to use and integrate. 
+
 ## Installation
 ```bash
 pip install embedin
 ```
 
 ## Quick Start
-### Using memery DB
+### Using memory DB
 ```python
 from embedin.client import Client
 
 client = Client(collection_name="test_collection")
 client.add_data(texts=["This is a test"], meta_data=[{"source": "abc4"}])
 result = client.query("These are tests", top_k=1)
-
-print("result: ", result)
 ```
 
 ### Using sqlite with local storage
 ```python
 from embedin.client import Client
 
 url = 'sqlite:///test.db'
@@ -45,39 +48,39 @@
 
 ### Using PostgreSQL
 ```python
 import os
 
 from embedin.client import Client
 
-url = os.environ.get('EMBEDIN_POSGRES_URL', "postgresql+psycopg2://embedin:embedin@localhost/embedin_db")
+url = os.getenv('EMBEDIN_POSGRES_URL', "postgresql+psycopg2://embedin:embedin@localhost/embedin_db")
 client = Client(collection_name="test_collection", url=url)
 client.add_data(texts=["This is a test"], meta_data=[{"source": "abc4"}])
 result = client.query("These are tests", top_k=1)
 ```
 
 ### Using MySQL
 ```python
 import os
 
 from embedin.client import Client
 
-url = os.environ.get('EMBEDIN_MYSQL_URL', "mysql+pymysql://embedin:embedin@localhost/embedin_db")
+url = os.getenv('EMBEDIN_MYSQL_URL', "mysql+pymysql://embedin:embedin@localhost/embedin_db")
 client = Client(collection_name="test_collection", url=url)
 client.add_data(texts=["This is a test"], meta_data=[{"source": "abc4"}])
 result = client.query("These are tests", top_k=1)
 ```
 
 ### Using MS-SQL
 ```python
 import os
 
 from embedin.client import Client
 
-url = os.environ.get('EMBEDIN_MSSQL_URL', "mssql+pymssql://sa:StrongPassword123@localhost/tempdb")
+url = os.getenv('EMBEDIN_MSSQL_URL', "mssql+pymssql://sa:StrongPassword123@localhost/tempdb")
 client = Client(collection_name="test_collection", url=url)
 client.add_data(texts=["This is a test"], meta_data=[{"source": "abc4"}])
 result = client.query("These are tests", top_k=1)
 ```
 
 ## For development
 
@@ -100,42 +103,12 @@
 
 Start MS-SQL DB (Only necessary for using MS-SQL as the storage)
 ```bash
 cd docker
 docker-compose up embedin-mssql
 ```
 
-Start Oracle DB (Only necessary for using Oracle as the storage) - not supported yet
-
-docker login container-registry.oracle.com
-```bash
-cd docker
-docker-compose up embedin-oracle
-```yaml
-  embedin-oracle:
-    container_name: embedin-oracle
-    image: container-registry.oracle.com/database/enterprise:21.3.0.0
-    environment:
-      - ORACLE_SID=ORCLCDB
-      - ORACLE_PWD=password
-      - ORACLE_PDB=ORCLPDB1
-      - ORACLE_CHARACTERSET=AL32UTF8
-    volumes:
-      - ./oracle/data:/opt/oracle/oradata
-    ports:
-      - "1521:1521"
-```
-
 Run unit test with coverage report
 ```bash
 coverage run -m unittest discover -s tests -p '*.py'
 coverage report
 ```
-
-To publish to PyPI
-```bash
-pip install twine
-```
-
-```bash
-python setup.py sdist && python setup.py bdist_wheel && twine upload dist/*
-```
```

### Comparing `embedin-0.1.3/embedin.egg-info/SOURCES.txt` & `embedin-0.2.0/embedin.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -5,33 +5,40 @@
 embedin.egg-info/PKG-INFO
 embedin.egg-info/SOURCES.txt
 embedin.egg-info/dependency_links.txt
 embedin.egg-info/requires.txt
 embedin.egg-info/top_level.txt
 embedin/client/__init__.py
 embedin/embedding/__init__.py
+embedin/embedding/embedding_base.py
+embedin/embedding/openai_embedding.py
 embedin/embedding/sentence_transformer.py
 embedin/index/__init__.py
-embedin/index/hnswlib.py
+embedin/index/flat_index.py
+embedin/index/hnsw_index.py
+embedin/index/index_base.py
 embedin/model/__init__.py
 embedin/model/collection_model.py
 embedin/model/embedding_model.py
 embedin/repository/__init__.py
 embedin/repository/collection_repository.py
 embedin/repository/embedding_repository.py
 embedin/service/__init__.py
 embedin/service/collection_service.py
 embedin/service/embedding_service.py
 embedin/util/__init__.py
 tests/__init__.py
 tests/client/__init__.py
 tests/embedding/__init__.py
-tests/embedding/test_embedding.py
+tests/embedding/test_embedding_base.py
+tests/embedding/test_openai_embedding.py
+tests/embedding/test_sentence_transformer_embedding.py
 tests/index/__init__.py
-tests/index/test_hnswlib.py
+tests/index/test_flat_index.py
+tests/index/test_hnsw_index.py
 tests/model/__init__.py
 tests/model/test_collection_model.py
 tests/model/test_embedding_model.py
 tests/repository/__init__.py
 tests/repository/test_collection_repository.py
 tests/repository/test_embedding_repository.py
 tests/service/__init__.py
```

### Comparing `embedin-0.1.3/setup.py` & `embedin-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import os
 
 import setuptools
 
 
 def read(fname):
-    with open(os.path.join(os.path.dirname(__file__), fname), "r", encoding="utf-8") as fh:
+    with open(
+        os.path.join(os.path.dirname(__file__), fname), "r", encoding="utf-8"
+    ) as fh:
         return fh.read()
 
 
 setuptools.setup(
     name="embedin",
-    version="0.1.3",
+    version="0.2.0",
     author="EmbedInAI",
     author_email="EmbedInAI@gmail.com",
     description="A lightweight vector database",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/EmbedInAI/EmbedInDB",
     packages=setuptools.find_packages(exclude=["tests"]),
     install_requires=read("requirements.txt"),
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.6',
+    python_requires=">=3.6",
 )
```

### Comparing `embedin-0.1.3/tests/client/__init__.py` & `embedin-0.2.0/tests/client/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,55 @@
 import unittest
 from unittest.mock import MagicMock
+
 from embedin.client import Client
 
 
 class TestClient(unittest.TestCase):
     def setUp(self):
-        self.client = Client(
-            collection_name="test_collection",
-            embedding_fn=MagicMock(return_value=[[1, 2, 3], [4, 5, 6]]),
-        )
+        self.client = Client("test_collection")
 
     def test_create_or_get_collection(self):
-        collection_id = self.client.create_or_get_collection("new_collection")
+        name = "test_collection"
+        collection_id = self.client.create_or_get_collection(name)
+        self.assertIsNotNone(collection_id)
         self.assertEqual(self.client.collection_id, collection_id)
 
     def test_create_collection(self):
         # Test that a collection is created with the given name
-        collection_id = self.client.create_collection("new_collection")
+        name = "new_collection"
+        collection_id = self.client.create_collection(name)
+        self.assertIsNotNone(collection_id)
         self.assertEqual(self.client.collection_id, collection_id)
 
     def test_get_collection(self):
         # Test that a collection is retrieved with the given name
         collection_name = "new_collection"
         self.client.create_collection(collection_name)
         collection_id = self.client.get_collection(collection_name)
+        self.assertIsNotNone(collection_id)
         self.assertEqual(self.client.collection_id, collection_id)
 
     def test_add_data(self):
         # Test that data is added to the collection
         texts = ["text1", "text2"]
         meta_data = [{"meta1": "value1"}, {"meta2": "value2"}]
+
+        self.client.embedding_fn = MagicMock(return_value=[[1, 2, 3], [4, 5, 6]])
         self.client.add_data(texts, meta_data)
-        self.assertEqual(len(self.client.embeddings), 2)
+
+        self.client.embedding_fn.assert_called_once_with(texts)
+        self.assertEqual(len(self.client.embedding_rows), 2)
 
     def test_query(self):
         # Test that queries return the expected results
+        self.client.embedding_fn = MagicMock(return_value=[[1, 2, 3], [4, 5, 6]])
         self.client.add_data(["test", "text"])
+
+        self.client.embedding_fn = MagicMock(return_value=[[1, 2, 3]])
         result = self.client.query("test", top_k=1)
         expected_result = [{"text": "test", "meta_data": None}]
         self.assertEqual(result, expected_result)
 
     def tearDown(self):
         # Clean up any resources created by the test
         pass
```

### Comparing `embedin-0.1.3/tests/embedding/test_embedding.py` & `embedin-0.2.0/tests/embedding/test_sentence_transformer_embedding.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,10 +24,14 @@
 
     def test_embedding_invalid_input(self):
         embedding = SentenceTransformerEmbedding()
         invalid_input = 123
         with self.assertRaises(TypeError):
             embedding(invalid_input)
 
+        invalid_input = [123, "string"]
+        with self.assertRaises(TypeError):
+            embedding(invalid_input)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `embedin-0.1.3/tests/model/test_collection_model.py` & `embedin-0.2.0/tests/model/test_collection_model.py`

 * *Files identical despite different names*

### Comparing `embedin-0.1.3/tests/model/test_embedding_model.py` & `embedin-0.2.0/tests/model/test_embedding_model.py`

 * *Files identical despite different names*

### Comparing `embedin-0.1.3/tests/repository/test_collection_repository.py` & `embedin-0.2.0/tests/repository/test_collection_repository.py`

 * *Files identical despite different names*

### Comparing `embedin-0.1.3/tests/repository/test_embedding_repository.py` & `embedin-0.2.0/tests/repository/test_embedding_repository.py`

 * *Files identical despite different names*

### Comparing `embedin-0.1.3/tests/service/test_collection_service.py` & `embedin-0.2.0/tests/service/test_collection_service.py`

 * *Files identical despite different names*

### Comparing `embedin-0.1.3/tests/service/test_embedding_service.py` & `embedin-0.2.0/tests/service/test_embedding_service.py`

 * *Files identical despite different names*

