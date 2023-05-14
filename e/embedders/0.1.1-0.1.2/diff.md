# Comparing `tmp/embedders-0.1.1-py2.py3-none-any.whl.zip` & `tmp/embedders-0.1.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 23258 bytes, number of entries: 18
+Zip file size: 23243 bytes, number of entries: 18
 -rw-r--r--  2.0 unx     6934 b- defN 22-Oct-30 14:35 embedders/__init__.py
 -rw-r--r--  2.0 unx      143 b- defN 22-Sep-07 08:19 embedders/enums.py
 -rw-r--r--  2.0 unx      399 b- defN 22-Jul-22 10:51 embedders/util.py
 -rw-r--r--  2.0 unx      178 b- defN 22-Sep-07 08:19 embedders/classification/__init__.py
 -rw-r--r--  2.0 unx     3038 b- defN 23-May-14 15:03 embedders/classification/contextual.py
 -rw-r--r--  2.0 unx     3285 b- defN 22-Jul-22 10:51 embedders/classification/count_based.py
 -rw-r--r--  2.0 unx     2170 b- defN 22-Jul-22 10:51 embedders/classification/reduce.py
 -rw-r--r--  2.0 unx      670 b- defN 22-Sep-07 08:19 embedders/extraction/__init__.py
 -rw-r--r--  2.0 unx    14751 b- defN 22-Oct-22 16:42 embedders/extraction/contextual.py
 -rw-r--r--  2.0 unx     1784 b- defN 22-Jul-22 10:51 embedders/extraction/count_based.py
 -rw-r--r--  2.0 unx     2705 b- defN 22-Jul-22 10:51 embedders/extraction/reduce.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jul-22 10:51 embedders/samples/__init__.py
 -rw-r--r--  2.0 unx     6158 b- defN 22-Jul-22 10:51 embedders/samples/clickbait.py
--rw-r--r--  2.0 unx    11340 b- defN 23-May-14 15:03 embedders-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     7049 b- defN 23-May-14 15:03 embedders-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-14 15:03 embedders-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-May-14 15:03 embedders-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1526 b- defN 23-May-14 15:03 embedders-0.1.1.dist-info/RECORD
-18 files, 62250 bytes uncompressed, 20744 bytes compressed:  66.7%
+-rw-r--r--  2.0 unx    11340 b- defN 23-May-14 15:06 embedders-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7028 b- defN 23-May-14 15:06 embedders-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-14 15:06 embedders-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-May-14 15:06 embedders-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1526 b- defN 23-May-14 15:06 embedders-0.1.2.dist-info/RECORD
+18 files, 62229 bytes uncompressed, 20729 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: embedders/samples/__init__.py
 Comment: 
 
 Filename: embedders/samples/clickbait.py
 Comment: 
 
-Filename: embedders-0.1.1.dist-info/LICENSE
+Filename: embedders-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: embedders-0.1.1.dist-info/METADATA
+Filename: embedders-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: embedders-0.1.1.dist-info/WHEEL
+Filename: embedders-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: embedders-0.1.1.dist-info/top_level.txt
+Filename: embedders-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: embedders-0.1.1.dist-info/RECORD
+Filename: embedders-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `embedders-0.1.1.dist-info/LICENSE` & `embedders-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `embedders-0.1.1.dist-info/METADATA` & `embedders-0.1.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedders
-Version: 0.1.1
+Version: 0.1.2
 Summary: High-level API for creating sentence and token embeddings
 Home-page: https://github.com/code-kern-ai/embedders
 Author: Johannes Hötter
 Author-email: johannes.hoetter@kern.ai
 License: UNKNOWN
 Keywords: kern,machine learning,representation learning,python
 Platform: UNKNOWN
@@ -16,20 +16,20 @@
 Requires-Dist: numpy
 Requires-Dist: scikit-learn
 Requires-Dist: sentence-transformers
 Requires-Dist: spacy (>=3.0.0)
 Requires-Dist: torch (>=1.6.0)
 Requires-Dist: tqdm
 Requires-Dist: transformers (<5.0.0,>=4.6.0)
-Requires-Dist: openai (==0.27.6)
-Requires-Dist: cohere (==4.4.1)
+Requires-Dist: openai
+Requires-Dist: cohere
 
 ![embedders](https://uploads-ssl.webflow.com/61e47fafb12bd56b40022a49/626ee1c35a3abf0ca872486d_embedder-banner.png)
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
-[![pypi 0.1.1](https://img.shields.io/badge/pypi-0.1.1-red.svg)](https://pypi.org/project/embedders/0.1.1/)
+[![pypi 0.1.2](https://img.shields.io/badge/pypi-0.1.2-red.svg)](https://pypi.org/project/embedders/0.1.2/)
 
 # ⚗️ embedders
 
 With `embedders`, you can easily convert your texts into sentence- or token-level embeddings within a few lines of code. Use cases for this include similarity search between texts, information extraction such as named entity recognition, or basic text classification.
 
 ## Prerequisites
```

## Comparing `embedders-0.1.1.dist-info/RECORD` & `embedders-0.1.2.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -7,12 +7,12 @@
 embedders/classification/reduce.py,sha256=hXXoK_vS-tzCmZmPFbfQ_pML2bGzqL2w-UrWhqn5gV4,2170
 embedders/extraction/__init__.py,sha256=D5YDQTnOTa7qO76CSXyqHCTtmIP559crWHXCBkTo5Co,670
 embedders/extraction/contextual.py,sha256=r0wviuKgssOqpx32iVzb5IRrTziR5TpDs-0a2TlyQWo,14751
 embedders/extraction/count_based.py,sha256=uwhg2r3D-My3faMv81OHCDkbQyjTWv3Uomft6BsxKik,1784
 embedders/extraction/reduce.py,sha256=iezo-xOkYfeuuio4O_JSUEeBfJHG6Iw1MqUmpS5enwk,2705
 embedders/samples/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 embedders/samples/clickbait.py,sha256=IiivTTmb3zIUaurod3L0ADruCQuXtHGXsU4fW4IrFQc,6158
-embedders-0.1.1.dist-info/LICENSE,sha256=JYWPdm7R90tTEXK6muMxOgQBHToBQaLT9rPehcITO4I,11340
-embedders-0.1.1.dist-info/METADATA,sha256=gXrPp9lIWOURlHZuAShVCDwwMUIZrFPT8o_8tT-c5T4,7049
-embedders-0.1.1.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
-embedders-0.1.1.dist-info/top_level.txt,sha256=iRhfbBg_ZWmtclxcpD-WZe5rD-rvHFHKGkJwcWZM_f0,10
-embedders-0.1.1.dist-info/RECORD,,
+embedders-0.1.2.dist-info/LICENSE,sha256=JYWPdm7R90tTEXK6muMxOgQBHToBQaLT9rPehcITO4I,11340
+embedders-0.1.2.dist-info/METADATA,sha256=eSYsNtzpUCL4C2JYZbmViGU1AEO5nnzm_S-w5iX6fV0,7028
+embedders-0.1.2.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
+embedders-0.1.2.dist-info/top_level.txt,sha256=iRhfbBg_ZWmtclxcpD-WZe5rD-rvHFHKGkJwcWZM_f0,10
+embedders-0.1.2.dist-info/RECORD,,
```

