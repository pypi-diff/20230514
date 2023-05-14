# Comparing `tmp/enformer-pytorch-0.7.3.tar.gz` & `tmp/enformer-pytorch-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enformer-pytorch-0.7.3.tar", last modified: Wed Apr  5 14:27:59 2023, max compression
+gzip compressed data, was "enformer-pytorch-0.7.4.tar", last modified: Sun May 14 04:01:06 2023, max compression
```

## Comparing `enformer-pytorch-0.7.3.tar` & `enformer-pytorch-0.7.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:27:59.699594 enformer-pytorch-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-05 14:27:44.000000 enformer-pytorch-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-05 14:27:44.000000 enformer-pytorch-0.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-05 14:27:59.699594 enformer-pytorch-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12157 2023-04-05 14:27:44.000000 enformer-pytorch-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:27:59.695594 enformer-pytorch-0.7.3/enformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-05 14:27:44.000000 enformer-pytorch-0.7.3/enformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-05 14:27:44.000000 enformer-pytorch-0.7.3/enformer_pytorch/config_enformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-04-05 14:27:44.000000 enformer-pytorch-0.7.3/enformer_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-04-05 14:27:44.000000 enformer-pytorch-0.7.3/enformer_pytorch/finetune.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-05 14:27:44.000000 enformer-pytorch-0.7.3/enformer_pytorch/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13835 2023-04-05 14:27:44.000000 enformer-pytorch-0.7.3/enformer_pytorch/modeling_enformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:27:59.695594 enformer-pytorch-0.7.3/enformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-05 14:27:59.000000 enformer-pytorch-0.7.3/enformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-05 14:27:59.000000 enformer-pytorch-0.7.3/enformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 14:27:59.000000 enformer-pytorch-0.7.3/enformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-05 14:27:59.000000 enformer-pytorch-0.7.3/enformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-05 14:27:59.000000 enformer-pytorch-0.7.3/enformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 14:27:59.699594 enformer-pytorch-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-05 14:27:44.000000 enformer-pytorch-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 04:01:06.952199 enformer-pytorch-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-14 04:00:56.000000 enformer-pytorch-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-14 04:00:56.000000 enformer-pytorch-0.7.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-14 04:01:06.952199 enformer-pytorch-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-05-14 04:00:56.000000 enformer-pytorch-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 04:01:06.952199 enformer-pytorch-0.7.4/enformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-14 04:00:56.000000 enformer-pytorch-0.7.4/enformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-14 04:00:56.000000 enformer-pytorch-0.7.4/enformer_pytorch/config_enformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-05-14 04:00:56.000000 enformer-pytorch-0.7.4/enformer_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-05-14 04:00:56.000000 enformer-pytorch-0.7.4/enformer_pytorch/finetune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-14 04:00:56.000000 enformer-pytorch-0.7.4/enformer_pytorch/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13835 2023-05-14 04:00:56.000000 enformer-pytorch-0.7.4/enformer_pytorch/modeling_enformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 04:01:06.952199 enformer-pytorch-0.7.4/enformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-14 04:01:06.000000 enformer-pytorch-0.7.4/enformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-14 04:01:06.000000 enformer-pytorch-0.7.4/enformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 04:01:06.000000 enformer-pytorch-0.7.4/enformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-14 04:01:06.000000 enformer-pytorch-0.7.4/enformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 04:01:06.000000 enformer-pytorch-0.7.4/enformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 04:01:06.952199 enformer-pytorch-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-14 04:00:56.000000 enformer-pytorch-0.7.4/setup.py
```

### Comparing `enformer-pytorch-0.7.3/LICENSE` & `enformer-pytorch-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `enformer-pytorch-0.7.3/PKG-INFO` & `enformer-pytorch-0.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enformer-pytorch
-Version: 0.7.3
+Version: 0.7.4
 Summary: Enformer - Pytorch
 Home-page: https://github.com/lucidrains/enformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,transformer,gene-expression
 Classifier: Development Status :: 4 - Beta
```

### Comparing `enformer-pytorch-0.7.3/README.md` & `enformer-pytorch-0.7.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -245,15 +245,15 @@
 )
 
 loss.backward()
 ```
 
 ## Data
 
-You can use the `GenomicIntervalDataset` to easily fetch sequences of any length from a `.bed` file, with greater context length dynamically computed if specified
+You can use the `GenomicIntervalDataset` to easily fetch sequences of any length from a <a href="https://genome.ucsc.edu/FAQ/FAQformat.html#format1">`.bed`</a> file, with greater context length dynamically computed if specified
 
 ```python
 import torch
 import polars as pl
 from enformer_pytorch import Enformer, GenomeIntervalDataset
 
 filter_train = lambda df: df.filter(pl.col('column_4') == 'train')
```

### Comparing `enformer-pytorch-0.7.3/enformer_pytorch/config_enformer.py` & `enformer-pytorch-0.7.4/enformer_pytorch/config_enformer.py`

 * *Files identical despite different names*

### Comparing `enformer-pytorch-0.7.3/enformer_pytorch/data.py` & `enformer-pytorch-0.7.4/enformer_pytorch/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
         rc_aug = False,
         return_augs = False
     ):
         super().__init__()
         bed_path = Path(bed_file)
         assert bed_path.exists(), 'path to .bed file must exist'
 
-        df = pl.read_csv(str(bed_path), sep = '\t', has_header = False)
+        df = pl.read_csv(str(bed_path), separator = '\t', has_header = False)
         df = filter_df_fn(df)
         self.df = df
 
         # if the chromosome name in the bed file is different than the keyname in the fasta
         # can remap on the fly
         self.chr_bed_to_fasta_map = chr_bed_to_fasta_map
```

### Comparing `enformer-pytorch-0.7.3/enformer_pytorch/finetune.py` & `enformer-pytorch-0.7.4/enformer_pytorch/finetune.py`

 * *Files identical despite different names*

### Comparing `enformer-pytorch-0.7.3/enformer_pytorch/metrics.py` & `enformer-pytorch-0.7.4/enformer_pytorch/metrics.py`

 * *Files identical despite different names*

### Comparing `enformer-pytorch-0.7.3/enformer_pytorch/modeling_enformer.py` & `enformer-pytorch-0.7.4/enformer_pytorch/modeling_enformer.py`

 * *Files identical despite different names*

### Comparing `enformer-pytorch-0.7.3/enformer_pytorch.egg-info/PKG-INFO` & `enformer-pytorch-0.7.4/enformer_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enformer-pytorch
-Version: 0.7.3
+Version: 0.7.4
 Summary: Enformer - Pytorch
 Home-page: https://github.com/lucidrains/enformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,transformer,gene-expression
 Classifier: Development Status :: 4 - Beta
```

### Comparing `enformer-pytorch-0.7.3/setup.py` & `enformer-pytorch-0.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'enformer-pytorch',
   packages = find_packages(exclude=[]),
   include_package_data = True,
-  version = '0.7.3',
+  version = '0.7.4',
   license='MIT',
   description = 'Enformer - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/enformer-pytorch',
   keywords = [
```

