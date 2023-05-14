# Comparing `tmp/similarity-ranker-1.0.2.tar.gz` & `tmp/similarity-ranker-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "similarity-ranker-1.0.2.tar", last modified: Sat May 13 02:31:43 2023, max compression
+gzip compressed data, was "similarity-ranker-1.0.3.tar", last modified: Sun May 14 12:09:23 2023, max compression
```

## Comparing `similarity-ranker-1.0.2.tar` & `similarity-ranker-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-13 02:31:43.861741 similarity-ranker-1.0.2/
--rw-r--r--   0 chiubowen   (501) staff       (20)     2062 2023-05-13 02:31:43.861626 similarity-ranker-1.0.2/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     1887 2023-05-13 02:31:43.000000 similarity-ranker-1.0.2/README.md
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-13 02:31:43.861777 similarity-ranker-1.0.2/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      532 2023-05-13 02:31:43.000000 similarity-ranker-1.0.2/setup.py
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-13 02:31:43.861451 similarity-ranker-1.0.2/similarity_ranker.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     2062 2023-05-13 02:31:43.000000 similarity-ranker-1.0.2/similarity_ranker.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      287 2023-05-13 02:31:43.000000 similarity-ranker-1.0.2/similarity_ranker.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-13 02:31:43.000000 similarity-ranker-1.0.2/similarity_ranker.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       62 2023-05-13 02:31:43.000000 similarity-ranker-1.0.2/similarity_ranker.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       34 2023-05-13 02:31:43.000000 similarity-ranker-1.0.2/similarity_ranker.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       18 2023-05-13 02:31:43.000000 similarity-ranker-1.0.2/similarity_ranker.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     3260 2023-05-13 02:31:43.000000 similarity-ranker-1.0.2/similarity_ranker.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-14 12:09:23.739216 similarity-ranker-1.0.3/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1989 2023-05-14 12:09:23.739086 similarity-ranker-1.0.3/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1887 2023-05-14 12:09:23.000000 similarity-ranker-1.0.3/README.md
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-14 12:09:23.739253 similarity-ranker-1.0.3/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      532 2023-05-14 12:09:23.000000 similarity-ranker-1.0.3/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-14 12:09:23.738898 similarity-ranker-1.0.3/similarity_ranker.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1989 2023-05-14 12:09:23.000000 similarity-ranker-1.0.3/similarity_ranker.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      287 2023-05-14 12:09:23.000000 similarity-ranker-1.0.3/similarity_ranker.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-14 12:09:23.000000 similarity-ranker-1.0.3/similarity_ranker.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       61 2023-05-14 12:09:23.000000 similarity-ranker-1.0.3/similarity_ranker.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       34 2023-05-14 12:09:23.000000 similarity-ranker-1.0.3/similarity_ranker.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       18 2023-05-14 12:09:23.000000 similarity-ranker-1.0.3/similarity_ranker.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     3291 2023-05-14 12:09:23.000000 similarity-ranker-1.0.3/similarity_ranker.py
```

### Comparing `similarity-ranker-1.0.2/PKG-INFO` & `similarity-ranker-1.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 Metadata-Version: 2.1
 Name: similarity-ranker
-Version: 1.0.2
-Summary: UNKNOWN
-Home-page: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
+Version: 1.0.3
 Description-Content-Type: text/markdown
 
 # 積木塊 Similarity Ranker v1.0.0 by Bowen Chiu
 - 找到與給定查詢句子 v.s. 最相似的嵌入向量
 - 這東西可以用來做任意 .txt & .pt 遞迴子目錄的相似度比對
 - 找出排名最相似的 top 10 輸出 .json
 - 使用的是 Hugging Face Transformers 的 `paraphrase-multilingual-MiniLM-L12-v2` 模型。
@@ -77,9 +73,7 @@
 ```
 python3 -m similarity_ranker \
   --prompt "你的查詢句子" \
   --txt-folder "data/txt" \
   --embeddings-folder "data/embeddings" \
   --output-json "data/top_similarity.json"
 ```
-
-
```

### Comparing `similarity-ranker-1.0.2/README.md` & `similarity-ranker-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `similarity-ranker-1.0.2/setup.py` & `similarity-ranker-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="similarity-ranker",
-    version="1.0.2",
+    version="1.0.3",
     packages=find_packages(),
     py_modules=['similarity_ranker'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'similarity_ranker = similarity_ranker:main',
         ],
```

### Comparing `similarity-ranker-1.0.2/similarity_ranker.egg-info/PKG-INFO` & `similarity-ranker-1.0.3/similarity_ranker.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 Metadata-Version: 2.1
 Name: similarity-ranker
-Version: 1.0.2
-Summary: UNKNOWN
-Home-page: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
+Version: 1.0.3
 Description-Content-Type: text/markdown
 
 # 積木塊 Similarity Ranker v1.0.0 by Bowen Chiu
 - 找到與給定查詢句子 v.s. 最相似的嵌入向量
 - 這東西可以用來做任意 .txt & .pt 遞迴子目錄的相似度比對
 - 找出排名最相似的 top 10 輸出 .json
 - 使用的是 Hugging Face Transformers 的 `paraphrase-multilingual-MiniLM-L12-v2` 模型。
@@ -77,9 +73,7 @@
 ```
 python3 -m similarity_ranker \
   --prompt "你的查詢句子" \
   --txt-folder "data/txt" \
   --embeddings-folder "data/embeddings" \
   --output-json "data/top_similarity.json"
 ```
-
-
```

### Comparing `similarity-ranker-1.0.2/similarity_ranker.py` & `similarity-ranker-1.0.3/similarity_ranker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 #!/usr/bin/env python
 # similarity_ranker
 import argparse
 import glob
 import heapq
 import json
 import os
+from time import time
 
 import torch
 from scipy.spatial.distance import cosine
 # 1.2s 慢速瓶頸
 from sentence_transformers import SentenceTransformer
 
 
 def find_files(folder, extension):
     return glob.glob(f"{folder}/**/*{extension}", recursive=True)
 
 
+# 1.5s 慢速瓶頸
+model = SentenceTransformer('paraphrase-multilingual-MiniLM-L12-v2')
+
+
 def query_embeddings(query, embeddings_folder, top_n):
-    # 1.5s 慢速瓶頸
-    model = SentenceTransformer('paraphrase-multilingual-MiniLM-L12-v2')
     query_embedding = model.encode(query)
     embeddings_files = find_files(embeddings_folder, '.pt')
     max_heap = []
+    t = time()
     for embed_file in embeddings_files:
         embedding = torch.load(embed_file)
         similarity = 1 - cosine(query_embedding, embedding)
         if len(max_heap) < top_n:
             heapq.heappush(max_heap, (similarity, embed_file))
         elif max_heap[0][0] < similarity:
             heapq.heappop(max_heap)
```

