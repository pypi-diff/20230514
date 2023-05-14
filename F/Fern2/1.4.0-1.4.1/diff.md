# Comparing `tmp/Fern2-1.4.0.tar.gz` & `tmp/Fern2-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fern2-1.4.0.tar", last modified: Sat Nov 26 10:18:25 2022, max compression
+gzip compressed data, was "Fern2-1.4.1.tar", last modified: Sun May 14 15:44:45 2023, max compression
```

## Comparing `Fern2-1.4.0.tar` & `Fern2-1.4.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-26 10:18:25.219427 Fern2-1.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-26 10:18:25.215427 Fern2-1.4.0/Fern2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2789 2022-11-26 10:18:25.000000 Fern2-1.4.0/Fern2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      620 2022-11-26 10:18:25.000000 Fern2-1.4.0/Fern2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-26 10:18:25.000000 Fern2-1.4.0/Fern2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      220 2022-11-26 10:18:25.000000 Fern2-1.4.0/Fern2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2022-11-26 10:18:25.000000 Fern2-1.4.0/Fern2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2022-11-26 10:18:12.000000 Fern2-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     2789 2022-11-26 10:18:25.219427 Fern2-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1516 2022-11-26 10:18:12.000000 Fern2-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-26 10:18:25.215427 Fern2-1.4.0/fern/
--rw-r--r--   0 runner    (1001) docker     (122)      211 2022-11-26 10:18:12.000000 Fern2-1.4.0/fern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4959 2022-11-26 10:18:12.000000 Fern2-1.4.0/fern/applications.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-26 10:18:25.219427 Fern2-1.4.0/fern/data/
--rw-r--r--   0 runner    (1001) docker     (122)      335 2022-11-26 10:18:12.000000 Fern2-1.4.0/fern/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2205 2022-11-26 10:18:12.000000 Fern2-1.4.0/fern/data/data_balance.py
--rw-r--r--   0 runner    (1001) docker     (122)     3035 2022-11-26 10:18:12.000000 Fern2-1.4.0/fern/data/data_class.py
--rw-r--r--   0 runner    (1001) docker     (122)     1732 2022-11-26 10:18:12.000000 Fern2-1.4.0/fern/data/data_clean.py
--rw-r--r--   0 runner    (1001) docker     (122)     1000 2022-11-26 10:18:12.000000 Fern2-1.4.0/fern/data/data_download.py
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2022-11-26 10:18:12.000000 Fern2-1.4.0/fern/data/data_split.py
--rw-r--r--   0 runner    (1001) docker     (122)     6567 2022-11-26 10:18:12.000000 Fern2-1.4.0/fern/data/data_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (122)     3352 2022-11-26 10:18:12.000000 Fern2-1.4.0/fern/data/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     4679 2022-11-26 10:18:12.000000 Fern2-1.4.0/fern/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)     1364 2022-11-26 10:18:12.000000 Fern2-1.4.0/fern/losses.py
--rw-r--r--   0 runner    (1001) docker     (122)     1951 2022-11-26 10:18:12.000000 Fern2-1.4.0/fern/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-26 10:18:25.219427 Fern2-1.4.0/fern/models/
--rw-r--r--   0 runner    (1001) docker     (122)      205 2022-11-26 10:18:12.000000 Fern2-1.4.0/fern/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6081 2022-11-26 10:18:12.000000 Fern2-1.4.0/fern/models/layers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3334 2022-11-26 10:18:12.000000 Fern2-1.4.0/fern/models/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     5635 2022-11-26 10:18:12.000000 Fern2-1.4.0/fern/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (122)    16183 2022-11-26 10:18:12.000000 Fern2-1.4.0/fern/train.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-26 10:18:25.219427 Fern2-1.4.0/fern/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      178 2022-11-26 10:18:12.000000 Fern2-1.4.0/fern/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2674 2022-11-26 10:18:12.000000 Fern2-1.4.0/fern/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     1206 2022-11-26 10:18:12.000000 Fern2-1.4.0/fern/utils/tensor_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-26 10:18:25.219427 Fern2-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2111 2022-11-26 10:18:12.000000 Fern2-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:44:45.870461 Fern2-1.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:44:45.866461 Fern2-1.4.1/Fern2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-14 15:44:45.000000 Fern2-1.4.1/Fern2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-14 15:44:45.000000 Fern2-1.4.1/Fern2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 15:44:45.000000 Fern2-1.4.1/Fern2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-14 15:44:45.000000 Fern2-1.4.1/Fern2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-14 15:44:45.000000 Fern2-1.4.1/Fern2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 15:44:33.000000 Fern2-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-14 15:44:45.870461 Fern2-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-14 15:44:33.000000 Fern2-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:44:45.866461 Fern2-1.4.1/fern/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-14 15:44:33.000000 Fern2-1.4.1/fern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-05-14 15:44:33.000000 Fern2-1.4.1/fern/applications.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:44:45.870461 Fern2-1.4.1/fern/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-14 15:44:33.000000 Fern2-1.4.1/fern/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-14 15:44:33.000000 Fern2-1.4.1/fern/data/data_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-14 15:44:33.000000 Fern2-1.4.1/fern/data/data_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-14 15:44:33.000000 Fern2-1.4.1/fern/data/data_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-14 15:44:33.000000 Fern2-1.4.1/fern/data/data_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-14 15:44:33.000000 Fern2-1.4.1/fern/data/data_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-05-14 15:44:33.000000 Fern2-1.4.1/fern/data/data_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-14 15:44:33.000000 Fern2-1.4.1/fern/data/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-05-14 15:44:33.000000 Fern2-1.4.1/fern/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-14 15:44:33.000000 Fern2-1.4.1/fern/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-14 15:44:33.000000 Fern2-1.4.1/fern/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:44:45.870461 Fern2-1.4.1/fern/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-14 15:44:33.000000 Fern2-1.4.1/fern/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-05-14 15:44:33.000000 Fern2-1.4.1/fern/models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-14 15:44:33.000000 Fern2-1.4.1/fern/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-05-14 15:44:33.000000 Fern2-1.4.1/fern/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16183 2023-05-14 15:44:33.000000 Fern2-1.4.1/fern/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:44:45.870461 Fern2-1.4.1/fern/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-14 15:44:33.000000 Fern2-1.4.1/fern/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-14 15:44:33.000000 Fern2-1.4.1/fern/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-14 15:44:33.000000 Fern2-1.4.1/fern/utils/tensor_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 15:44:45.874461 Fern2-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-14 15:44:33.000000 Fern2-1.4.1/setup.py
```

### Comparing `Fern2-1.4.0/Fern2.egg-info/PKG-INFO` & `Fern2-1.4.1/Fern2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fern2
-Version: 1.4.0
+Version: 1.4.1
 Summary: NLP text processing toolkit for Deep Learning
 Home-page: https://github.com/Jasonsey/Fern
 Author: Jason, Lin
 Author-email: jason.m.lin@outlook.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `Fern2-1.4.0/Fern2.egg-info/SOURCES.txt` & `Fern2-1.4.1/Fern2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Fern2-1.4.0/LICENSE` & `Fern2-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Fern2-1.4.0/PKG-INFO` & `Fern2-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fern2
-Version: 1.4.0
+Version: 1.4.1
 Summary: NLP text processing toolkit for Deep Learning
 Home-page: https://github.com/Jasonsey/Fern
 Author: Jason, Lin
 Author-email: jason.m.lin@outlook.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `Fern2-1.4.0/README.md` & `Fern2-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `Fern2-1.4.0/fern/applications.py` & `Fern2-1.4.1/fern/applications.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,9 +114,9 @@
 
         Returns:
             [all_task_size, encoder_length]
         """
         txt_tokenized = self.tokenize(task_logs)
         bert_input = self.bert_pack_inputs([txt_tokenized])
         bert_output = self.encoder(bert_input)['sequence_output']  # [task_size, seq_len, 768]
-        res = bert_output[:, 0, :]  # [task_size, 768]
+        res = tf.reduce_mean(bert_output, axis=1)  # [task_size, 768]
         return res
```

### Comparing `Fern2-1.4.0/fern/data/data_balance.py` & `Fern2-1.4.1/fern/data/data_balance.py`

 * *Files identical despite different names*

### Comparing `Fern2-1.4.0/fern/data/data_class.py` & `Fern2-1.4.1/fern/data/data_class.py`

 * *Files identical despite different names*

### Comparing `Fern2-1.4.0/fern/data/data_clean.py` & `Fern2-1.4.1/fern/data/data_clean.py`

 * *Files identical despite different names*

### Comparing `Fern2-1.4.0/fern/data/data_download.py` & `Fern2-1.4.1/fern/data/data_download.py`

 * *Files identical despite different names*

### Comparing `Fern2-1.4.0/fern/data/data_split.py` & `Fern2-1.4.1/fern/data/data_split.py`

 * *Files identical despite different names*

### Comparing `Fern2-1.4.0/fern/data/data_tokenize.py` & `Fern2-1.4.1/fern/data/data_tokenize.py`

 * *Files identical despite different names*

### Comparing `Fern2-1.4.0/fern/data/data_utils.py` & `Fern2-1.4.1/fern/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `Fern2-1.4.0/fern/logging.py` & `Fern2-1.4.1/fern/logging.py`

 * *Files identical despite different names*

### Comparing `Fern2-1.4.0/fern/losses.py` & `Fern2-1.4.1/fern/losses.py`

 * *Files identical despite different names*

### Comparing `Fern2-1.4.0/fern/metrics.py` & `Fern2-1.4.1/fern/metrics.py`

 * *Files identical despite different names*

### Comparing `Fern2-1.4.0/fern/models/layers.py` & `Fern2-1.4.1/fern/models/layers.py`

 * *Files identical despite different names*

### Comparing `Fern2-1.4.0/fern/models/model.py` & `Fern2-1.4.1/fern/models/model.py`

 * *Files identical despite different names*

### Comparing `Fern2-1.4.0/fern/pipeline.py` & `Fern2-1.4.1/fern/pipeline.py`

 * *Files identical despite different names*

### Comparing `Fern2-1.4.0/fern/train.py` & `Fern2-1.4.1/fern/train.py`

 * *Files identical despite different names*

### Comparing `Fern2-1.4.0/fern/utils/common.py` & `Fern2-1.4.1/fern/utils/common.py`

 * *Files identical despite different names*

### Comparing `Fern2-1.4.0/fern/utils/tensor_ops.py` & `Fern2-1.4.1/fern/utils/tensor_ops.py`

 * *Files identical despite different names*

### Comparing `Fern2-1.4.0/setup.py` & `Fern2-1.4.1/setup.py`

 * *Files identical despite different names*

