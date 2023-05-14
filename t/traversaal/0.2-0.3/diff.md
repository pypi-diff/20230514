# Comparing `tmp/traversaal-0.2.tar.gz` & `tmp/traversaal-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traversaal-0.2.tar", last modified: Sun May 14 06:30:27 2023, max compression
+gzip compressed data, was "traversaal-0.3.tar", last modified: Sun May 14 06:42:48 2023, max compression
```

## Comparing `traversaal-0.2.tar` & `traversaal-0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 aimzlicious   (501) staff       (20)        0 2023-05-14 06:30:27.261619 traversaal-0.2/
--rw-r--r--   0 aimzlicious   (501) staff       (20)      197 2023-05-14 06:30:27.261477 traversaal-0.2/PKG-INFO
--rw-r--r--   0 aimzlicious   (501) staff       (20)     1521 2023-05-14 06:27:33.000000 traversaal-0.2/README.md
--rw-r--r--   0 aimzlicious   (501) staff       (20)       38 2023-05-14 06:30:27.261657 traversaal-0.2/setup.cfg
--rw-r--r--   0 aimzlicious   (501) staff       (20)      381 2023-05-14 06:30:22.000000 traversaal-0.2/setup.py
-drwxr-xr-x   0 aimzlicious   (501) staff       (20)        0 2023-05-14 06:30:27.261314 traversaal-0.2/traversaal.egg-info/
--rw-r--r--   0 aimzlicious   (501) staff       (20)      197 2023-05-14 06:30:27.000000 traversaal-0.2/traversaal.egg-info/PKG-INFO
--rw-r--r--   0 aimzlicious   (501) staff       (20)      187 2023-05-14 06:30:27.000000 traversaal-0.2/traversaal.egg-info/SOURCES.txt
--rw-r--r--   0 aimzlicious   (501) staff       (20)        1 2023-05-14 06:30:27.000000 traversaal-0.2/traversaal.egg-info/dependency_links.txt
--rw-r--r--   0 aimzlicious   (501) staff       (20)       25 2023-05-14 06:30:27.000000 traversaal-0.2/traversaal.egg-info/requires.txt
--rw-r--r--   0 aimzlicious   (501) staff       (20)        1 2023-05-14 06:30:27.000000 traversaal-0.2/traversaal.egg-info/top_level.txt
+drwxr-xr-x   0 aimzlicious   (501) staff       (20)        0 2023-05-14 06:42:48.883797 traversaal-0.3/
+-rw-r--r--   0 aimzlicious   (501) staff       (20)     1761 2023-05-14 06:42:48.883669 traversaal-0.3/PKG-INFO
+-rw-r--r--   0 aimzlicious   (501) staff       (20)     1522 2023-05-14 06:42:38.000000 traversaal-0.3/README.md
+-rw-r--r--   0 aimzlicious   (501) staff       (20)       38 2023-05-14 06:42:48.883836 traversaal-0.3/setup.cfg
+-rw-r--r--   0 aimzlicious   (501) staff       (20)      641 2023-05-14 06:42:44.000000 traversaal-0.3/setup.py
+drwxr-xr-x   0 aimzlicious   (501) staff       (20)        0 2023-05-14 06:42:48.883500 traversaal-0.3/traversaal.egg-info/
+-rw-r--r--   0 aimzlicious   (501) staff       (20)     1761 2023-05-14 06:42:48.000000 traversaal-0.3/traversaal.egg-info/PKG-INFO
+-rw-r--r--   0 aimzlicious   (501) staff       (20)      187 2023-05-14 06:42:48.000000 traversaal-0.3/traversaal.egg-info/SOURCES.txt
+-rw-r--r--   0 aimzlicious   (501) staff       (20)        1 2023-05-14 06:42:48.000000 traversaal-0.3/traversaal.egg-info/dependency_links.txt
+-rw-r--r--   0 aimzlicious   (501) staff       (20)       25 2023-05-14 06:42:48.000000 traversaal-0.3/traversaal.egg-info/requires.txt
+-rw-r--r--   0 aimzlicious   (501) staff       (20)        1 2023-05-14 06:42:48.000000 traversaal-0.3/traversaal.egg-info/top_level.txt
```

### Comparing `traversaal-0.2/README.md` & `traversaal-0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Traversaal
+## Traversaal
 
 Traversaal is a Python package that provides a simple semantic search functionality for hotel data. It leverages large language models such as BERT to encode hotel descriptions and reviews, allowing users to perform semantic search queries and retrieve relevant results based on the provided search query.
 
 ## Features
 
 - Efficient semantic search for hotel data based on descriptions and reviews.
 - Utilizes state-of-the-art language models to encode and compare text embeddings.
```

