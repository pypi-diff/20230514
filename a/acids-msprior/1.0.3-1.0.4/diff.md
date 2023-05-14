# Comparing `tmp/acids-msprior-1.0.3.tar.gz` & `tmp/acids-msprior-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acids-msprior-1.0.3.tar", last modified: Fri May 12 09:25:42 2023, max compression
+gzip compressed data, was "acids-msprior-1.0.4.tar", last modified: Sat May 13 17:29:27 2023, max compression
```

## Comparing `acids-msprior-1.0.3.tar` & `acids-msprior-1.0.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:25:42.152608 acids-msprior-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-12 09:25:42.152608 acids-msprior-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:25:42.148608 acids-msprior-1.0.3/acids_msprior.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-12 09:25:42.000000 acids-msprior-1.0.3/acids_msprior.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-12 09:25:42.000000 acids-msprior-1.0.3/acids_msprior.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 09:25:42.000000 acids-msprior-1.0.3/acids_msprior.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-12 09:25:42.000000 acids-msprior-1.0.3/acids_msprior.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-12 09:25:42.000000 acids-msprior-1.0.3/acids_msprior.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-12 09:25:42.000000 acids-msprior-1.0.3/acids_msprior.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:25:42.148608 acids-msprior-1.0.3/msprior/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19774 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:25:42.152608 acids-msprior-1.0.3/msprior/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior/configs/decoder_only.gin
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior/configs/encoder_decoder.gin
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior/configs/encoder_decoder_continuous.gin
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior/configs/recurrent.gin
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9771 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior/scripted.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:25:42.152608 acids-msprior-1.0.3/msprior_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior_scripts/compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior_scripts/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior_scripts/main_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior_scripts/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior_scripts/train.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 09:25:42.152608 acids-msprior-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:25:42.152608 acids-msprior-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/tests/test_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/tests/test_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:29:27.130217 acids-msprior-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-13 17:26:10.000000 acids-msprior-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-13 17:29:27.130217 acids-msprior-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-13 17:26:10.000000 acids-msprior-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:29:27.126217 acids-msprior-1.0.4/acids_msprior.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-13 17:29:27.000000 acids-msprior-1.0.4/acids_msprior.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-13 17:29:27.000000 acids-msprior-1.0.4/acids_msprior.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 17:29:27.000000 acids-msprior-1.0.4/acids_msprior.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-13 17:29:27.000000 acids-msprior-1.0.4/acids_msprior.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-13 17:29:27.000000 acids-msprior-1.0.4/acids_msprior.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-13 17:29:27.000000 acids-msprior-1.0.4/acids_msprior.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:29:27.126217 acids-msprior-1.0.4/msprior/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-13 17:26:10.000000 acids-msprior-1.0.4/msprior/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19774 2023-05-13 17:26:10.000000 acids-msprior-1.0.4/msprior/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:29:27.126217 acids-msprior-1.0.4/msprior/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-13 17:26:10.000000 acids-msprior-1.0.4/msprior/configs/decoder_only.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-13 17:26:10.000000 acids-msprior-1.0.4/msprior/configs/encoder_decoder.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-13 17:26:10.000000 acids-msprior-1.0.4/msprior/configs/encoder_decoder_continuous.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-13 17:26:10.000000 acids-msprior-1.0.4/msprior/configs/recurrent.gin
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-13 17:26:10.000000 acids-msprior-1.0.4/msprior/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-13 17:26:10.000000 acids-msprior-1.0.4/msprior/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9771 2023-05-13 17:26:10.000000 acids-msprior-1.0.4/msprior/scripted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-13 17:26:10.000000 acids-msprior-1.0.4/msprior/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-05-13 17:26:10.000000 acids-msprior-1.0.4/msprior/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:29:27.126217 acids-msprior-1.0.4/msprior_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 17:26:10.000000 acids-msprior-1.0.4/msprior_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-13 17:26:10.000000 acids-msprior-1.0.4/msprior_scripts/compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-13 17:26:10.000000 acids-msprior-1.0.4/msprior_scripts/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-13 17:26:10.000000 acids-msprior-1.0.4/msprior_scripts/main_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-13 17:26:10.000000 acids-msprior-1.0.4/msprior_scripts/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-13 17:26:10.000000 acids-msprior-1.0.4/msprior_scripts/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-13 17:26:10.000000 acids-msprior-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 17:29:27.130217 acids-msprior-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-13 17:26:10.000000 acids-msprior-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:29:27.126217 acids-msprior-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 17:26:10.000000 acids-msprior-1.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-13 17:26:10.000000 acids-msprior-1.0.4/tests/test_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-13 17:26:10.000000 acids-msprior-1.0.4/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-13 17:26:10.000000 acids-msprior-1.0.4/tests/test_configs.py
```

### Comparing `acids-msprior-1.0.3/PKG-INFO` & `acids-msprior-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acids-msprior
-Version: 1.0.3
+Version: 1.0.4
 Summary: MSPRIOR: A multiscale prior model for realtime temporal learning
 Author: Antoine CAILLON
 Author-email: caillon@ircam.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: acids-msprior Version: 1.0.3 Summary: MSPRIOR: A
+Metadata-Version: 2.1 Name: acids-msprior Version: 1.0.4 Summary: MSPRIOR: A
 multiscale prior model for realtime temporal learning Author: Antoine CAILLON
 Author-email: caillon@ircam.fr Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
 markdown # MSPrior ### A multi(scale/stream) prior model for realtime temporal
 learning ## Disclaimer This is an experimental project that *will* be subject
 to lots of changes. ## Installation ```bash pip install acids-msprior ``` ##
```

### Comparing `acids-msprior-1.0.3/README.md` & `acids-msprior-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.3/acids_msprior.egg-info/PKG-INFO` & `acids-msprior-1.0.4/acids_msprior.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acids-msprior
-Version: 1.0.3
+Version: 1.0.4
 Summary: MSPRIOR: A multiscale prior model for realtime temporal learning
 Author: Antoine CAILLON
 Author-email: caillon@ircam.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: acids-msprior Version: 1.0.3 Summary: MSPRIOR: A
+Metadata-Version: 2.1 Name: acids-msprior Version: 1.0.4 Summary: MSPRIOR: A
 multiscale prior model for realtime temporal learning Author: Antoine CAILLON
 Author-email: caillon@ircam.fr Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
 markdown # MSPrior ### A multi(scale/stream) prior model for realtime temporal
 learning ## Disclaimer This is an experimental project that *will* be subject
 to lots of changes. ## Installation ```bash pip install acids-msprior ``` ##
```

### Comparing `acids-msprior-1.0.3/acids_msprior.egg-info/SOURCES.txt` & `acids-msprior-1.0.4/acids_msprior.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.3/msprior/attention.py` & `acids-msprior-1.0.4/msprior/attention.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.3/msprior/configs/decoder_only.gin` & `acids-msprior-1.0.4/msprior/configs/decoder_only.gin`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.3/msprior/configs/encoder_decoder.gin` & `acids-msprior-1.0.4/msprior/configs/encoder_decoder.gin`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.3/msprior/configs/encoder_decoder_continuous.gin` & `acids-msprior-1.0.4/msprior/configs/encoder_decoder_continuous.gin`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.3/msprior/dataset.py` & `acids-msprior-1.0.4/msprior/dataset.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.3/msprior/preprocessor.py` & `acids-msprior-1.0.4/msprior/preprocessor.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.3/msprior/scripted.py` & `acids-msprior-1.0.4/msprior/scripted.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.3/msprior/task.py` & `acids-msprior-1.0.4/msprior/task.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.3/msprior/utils.py` & `acids-msprior-1.0.4/msprior/utils.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.3/msprior_scripts/compact.py` & `acids-msprior-1.0.4/msprior_scripts/compact.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.3/msprior_scripts/export.py` & `acids-msprior-1.0.4/msprior_scripts/export.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.3/msprior_scripts/main_cli.py` & `acids-msprior-1.0.4/msprior_scripts/main_cli.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.3/msprior_scripts/preprocess.py` & `acids-msprior-1.0.4/msprior_scripts/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 flags.DEFINE_multi_string('preprocessor',
                           default=[],
                           help='Additional preprocessors to import')
 flags.DEFINE_integer('gpu', default=None, help='GPU to use.')
 flags.DEFINE_integer('db_size',
                      default=100,
                      help='Maximum size of the dataset (GB)')
-flags.DEFINE_integer('dyndb',
+flags.DEFINE_bool('dyndb',
                      default=True,
                      help='Allow the database to grow dynamically')
 flags.DEFINE_bool('normalize',
                   default=False,
                   help="Normalize audio before preprocessing.")
 flags.DEFINE_integer('silence_threshold',
                      default=None,
```

### Comparing `acids-msprior-1.0.3/msprior_scripts/train.py` & `acids-msprior-1.0.4/msprior_scripts/train.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.3/setup.py` & `acids-msprior-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.3/tests/test_attention.py` & `acids-msprior-1.0.4/tests/test_attention.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.3/tests/test_cache.py` & `acids-msprior-1.0.4/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.3/tests/test_configs.py` & `acids-msprior-1.0.4/tests/test_configs.py`

 * *Files identical despite different names*

