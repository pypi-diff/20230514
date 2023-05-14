# Comparing `tmp/sherpa-onnx-1.4.1.tar.gz` & `tmp/sherpa-onnx-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sherpa-onnx-1.4.1.tar", last modified: Wed Apr 12 11:33:58 2023, max compression
+gzip compressed data, was "sherpa-onnx-1.4.3.tar", last modified: Sun May 14 14:53:58 2023, max compression
```

## Comparing `sherpa-onnx-1.4.1.tar` & `sherpa-onnx-1.4.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:33:58.851428 sherpa-onnx-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-12 11:22:47.000000 sherpa-onnx-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-12 11:33:58.851428 sherpa-onnx-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-12 11:22:47.000000 sherpa-onnx-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 11:33:58.851428 sherpa-onnx-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-12 11:22:47.000000 sherpa-onnx-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:33:58.847428 sherpa-onnx-1.4.1/sherpa-onnx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:33:58.847428 sherpa-onnx-1.4.1/sherpa-onnx/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:33:58.847428 sherpa-onnx-1.4.1/sherpa-onnx/python/sherpa_onnx/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-12 11:33:58.000000 sherpa-onnx-1.4.1/sherpa-onnx/python/sherpa_onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-04-12 11:22:47.000000 sherpa-onnx-1.4.1/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-04-12 11:22:47.000000 sherpa-onnx-1.4.1/sherpa-onnx/python/sherpa_onnx/online_recognizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:33:58.851428 sherpa-onnx-1.4.1/sherpa_onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-12 11:33:58.000000 sherpa-onnx-1.4.1/sherpa_onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-12 11:33:58.000000 sherpa-onnx-1.4.1/sherpa_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 11:33:58.000000 sherpa-onnx-1.4.1/sherpa_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 11:33:58.000000 sherpa-onnx-1.4.1/sherpa_onnx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 11:33:58.000000 sherpa-onnx-1.4.1/sherpa_onnx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 11:33:58.000000 sherpa-onnx-1.4.1/sherpa_onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:53:58.030425 sherpa-onnx-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-14 14:43:38.000000 sherpa-onnx-1.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-14 14:53:58.030425 sherpa-onnx-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-14 14:43:38.000000 sherpa-onnx-1.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 14:53:58.030425 sherpa-onnx-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-14 14:43:38.000000 sherpa-onnx-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:53:58.030425 sherpa-onnx-1.4.3/sherpa-onnx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:53:58.030425 sherpa-onnx-1.4.3/sherpa-onnx/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:53:58.030425 sherpa-onnx-1.4.3/sherpa-onnx/python/sherpa_onnx/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-14 14:53:57.000000 sherpa-onnx-1.4.3/sherpa-onnx/python/sherpa_onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-05-14 14:43:38.000000 sherpa-onnx-1.4.3/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-14 14:43:38.000000 sherpa-onnx-1.4.3/sherpa-onnx/python/sherpa_onnx/online_recognizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:53:58.030425 sherpa-onnx-1.4.3/sherpa_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-14 14:53:58.000000 sherpa-onnx-1.4.3/sherpa_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-14 14:53:58.000000 sherpa-onnx-1.4.3/sherpa_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 14:53:58.000000 sherpa-onnx-1.4.3/sherpa_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 14:53:58.000000 sherpa-onnx-1.4.3/sherpa_onnx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 14:53:58.000000 sherpa-onnx-1.4.3/sherpa_onnx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-14 14:53:58.000000 sherpa-onnx-1.4.3/sherpa_onnx.egg-info/top_level.txt
```

### Comparing `sherpa-onnx-1.4.1/LICENSE` & `sherpa-onnx-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.4.1/PKG-INFO` & `sherpa-onnx-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherpa-onnx
-Version: 1.4.1
+Version: 1.4.3
 Summary: UNKNOWN
 Home-page: https://github.com/k2-fsa/sherpa-onnx
 Author: The sherpa-onnx development team
 Author-email: dpovey@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
```

### Comparing `sherpa-onnx-1.4.1/setup.py` & `sherpa-onnx-1.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.4.1/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py` & `sherpa-onnx-1.4.3/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         joiner: str,
         tokens: str,
         num_threads: int,
         sample_rate: int = 16000,
         feature_dim: int = 80,
         decoding_method: str = "greedy_search",
         debug: bool = False,
+        provider: str = "cpu",
     ):
         """
         Please refer to
         `<https://k2-fsa.github.io/sherpa/onnx/pretrained_models/index.html>`_
         to download pre-trained models for different languages, e.g., Chinese,
         English, etc.
 
@@ -66,25 +67,28 @@
             Sample rate of the training data used to train the model.
           feature_dim:
             Dimension of the feature used to train the model.
           decoding_method:
             Support only greedy_search for now.
           debug:
             True to show debug messages.
+          provider:
+            onnxruntime execution providers. Valid values are: cpu, cuda, coreml.
         """
         self = cls.__new__(cls)
         model_config = OfflineModelConfig(
             transducer=OfflineTransducerModelConfig(
                 encoder_filename=encoder,
                 decoder_filename=decoder,
                 joiner_filename=joiner,
             ),
             tokens=tokens,
             num_threads=num_threads,
             debug=debug,
+            provider=provider,
         )
 
         feat_config = OfflineFeatureExtractorConfig(
             sampling_rate=sample_rate,
             feature_dim=feature_dim,
         )
```

### Comparing `sherpa-onnx-1.4.1/sherpa-onnx/python/sherpa_onnx/online_recognizer.py` & `sherpa-onnx-1.4.3/sherpa-onnx/python/sherpa_onnx/online_recognizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         feature_dim: int = 80,
         enable_endpoint_detection: bool = False,
         rule1_min_trailing_silence: float = 2.4,
         rule2_min_trailing_silence: float = 1.2,
         rule3_min_utterance_length: float = 20.0,
         decoding_method: str = "greedy_search",
         max_active_paths: int = 4,
+        provider: str = "cpu",
     ):
         """
         Please refer to
         `<https://k2-fsa.github.io/sherpa/onnx/pretrained_models/index.html>`_
         to download pre-trained models for different languages, e.g., Chinese,
         English, etc.
 
@@ -82,28 +83,31 @@
             length in seconds is larger than this value, we assume an endpoint
             is detected.
           decoding_method:
             Valid values are greedy_search, modified_beam_search.
           max_active_paths:
             Use only when decoding_method is modified_beam_search. It specifies
             the maximum number of active paths during beam search.
+          provider:
+            onnxruntime execution providers. Valid values are: cpu, cuda, coreml.
         """
         _assert_file_exists(tokens)
         _assert_file_exists(encoder)
         _assert_file_exists(decoder)
         _assert_file_exists(joiner)
 
         assert num_threads > 0, num_threads
 
         model_config = OnlineTransducerModelConfig(
             encoder_filename=encoder,
             decoder_filename=decoder,
             joiner_filename=joiner,
             tokens=tokens,
             num_threads=num_threads,
+            provider=provider,
         )
 
         feat_config = FeatureExtractorConfig(
             sampling_rate=sample_rate,
             feature_dim=feature_dim,
         )
```

### Comparing `sherpa-onnx-1.4.1/sherpa_onnx.egg-info/PKG-INFO` & `sherpa-onnx-1.4.3/sherpa_onnx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherpa-onnx
-Version: 1.4.1
+Version: 1.4.3
 Summary: UNKNOWN
 Home-page: https://github.com/k2-fsa/sherpa-onnx
 Author: The sherpa-onnx development team
 Author-email: dpovey@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
```

