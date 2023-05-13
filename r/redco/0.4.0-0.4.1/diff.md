# Comparing `tmp/redco-0.4.0.tar.gz` & `tmp/redco-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redco-0.4.0.tar", last modified: Wed Apr 19 18:15:22 2023, max compression
+gzip compressed data, was "redco-0.4.1.tar", last modified: Sat May 13 23:54:41 2023, max compression
```

## Comparing `redco-0.4.0.tar` & `redco-0.4.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-04-19 18:15:22.440000 redco-0.4.0/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)    11358 2023-04-19 06:11:18.000000 redco-0.4.0/LICENSE
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      174 2023-04-19 18:15:22.440000 redco-0.4.0/PKG-INFO
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      763 2023-04-19 15:10:51.000000 redco-0.4.0/README.md
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-04-19 18:15:22.440000 redco-0.4.0/redco/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      693 2023-04-19 06:51:00.000000 redco-0.4.0/redco/__init__.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-04-19 18:15:22.440000 redco-0.4.0/redco/datasets/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      663 2023-04-19 06:51:00.000000 redco-0.4.0/redco/datasets/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      745 2023-04-19 06:51:00.000000 redco-0.4.0/redco/datasets/dataset.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1109 2023-04-19 06:51:00.000000 redco-0.4.0/redco/datasets/jsonl_dataset.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-04-19 18:15:22.440000 redco-0.4.0/redco/deployers/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      625 2023-04-19 06:51:00.000000 redco-0.4.0/redco/deployers/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2065 2023-04-19 06:51:00.000000 redco-0.4.0/redco/deployers/data_utils.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     8044 2023-04-19 06:51:00.000000 redco-0.4.0/redco/deployers/deployer.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2656 2023-04-19 06:51:00.000000 redco-0.4.0/redco/deployers/log_utils.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-04-19 18:15:22.440000 redco-0.4.0/redco/deployers/model_parallel_utils/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      595 2023-04-19 06:51:00.000000 redco-0.4.0/redco/deployers/model_parallel_utils/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     5238 2023-04-19 06:51:00.000000 redco-0.4.0/redco/deployers/model_parallel_utils/mesh_utils.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2468 2023-04-19 06:51:00.000000 redco-0.4.0/redco/deployers/model_parallel_utils/partition_utils.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1835 2023-04-19 06:51:00.000000 redco-0.4.0/redco/deployers/opt_utils.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-04-19 18:15:22.440000 redco-0.4.0/redco/predictors/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      628 2023-04-19 06:51:00.000000 redco-0.4.0/redco/predictors/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     4243 2023-04-19 06:51:00.000000 redco-0.4.0/redco/predictors/predictor.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1812 2023-04-19 06:51:00.000000 redco-0.4.0/redco/predictors/utils.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-04-19 18:15:22.440000 redco-0.4.0/redco/trainers/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      624 2023-04-19 06:51:00.000000 redco-0.4.0/redco/trainers/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)    12098 2023-04-19 06:51:00.000000 redco-0.4.0/redco/trainers/trainer.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2168 2023-04-19 06:51:00.000000 redco-0.4.0/redco/trainers/utils.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-04-19 18:15:22.440000 redco-0.4.0/redco.egg-info/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      174 2023-04-19 18:15:22.000000 redco-0.4.0/redco.egg-info/PKG-INFO
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      735 2023-04-19 18:15:22.000000 redco-0.4.0/redco.egg-info/SOURCES.txt
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)        1 2023-04-19 18:15:22.000000 redco-0.4.0/redco.egg-info/dependency_links.txt
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)       21 2023-04-19 18:15:22.000000 redco-0.4.0/redco.egg-info/requires.txt
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)        6 2023-04-19 18:15:22.000000 redco-0.4.0/redco.egg-info/top_level.txt
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)       38 2023-04-19 18:15:22.440000 redco-0.4.0/setup.cfg
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      857 2023-04-19 18:12:30.000000 redco-0.4.0/setup.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-13 23:54:41.850000 redco-0.4.1/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)    11358 2023-04-19 06:11:18.000000 redco-0.4.1/LICENSE
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3628 2023-05-13 23:54:41.850000 redco-0.4.1/PKG-INFO
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3375 2023-05-11 00:01:23.000000 redco-0.4.1/README.md
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-13 23:54:41.840000 redco-0.4.1/redco/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      693 2023-04-19 06:51:00.000000 redco-0.4.1/redco/__init__.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-13 23:54:41.840000 redco-0.4.1/redco/datasets/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      663 2023-04-19 06:51:00.000000 redco-0.4.1/redco/datasets/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      745 2023-04-19 06:51:00.000000 redco-0.4.1/redco/datasets/dataset.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1109 2023-04-19 06:51:00.000000 redco-0.4.1/redco/datasets/jsonl_dataset.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-13 23:54:41.840000 redco-0.4.1/redco/deployers/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      625 2023-04-19 06:51:00.000000 redco-0.4.1/redco/deployers/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2065 2023-04-19 06:51:00.000000 redco-0.4.1/redco/deployers/data_utils.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     8044 2023-04-19 06:51:00.000000 redco-0.4.1/redco/deployers/deployer.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2656 2023-04-19 06:51:00.000000 redco-0.4.1/redco/deployers/log_utils.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-13 23:54:41.840000 redco-0.4.1/redco/deployers/model_parallel_utils/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      595 2023-04-19 06:51:00.000000 redco-0.4.1/redco/deployers/model_parallel_utils/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     5492 2023-05-11 00:14:31.000000 redco-0.4.1/redco/deployers/model_parallel_utils/mesh_utils.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2468 2023-04-19 06:51:00.000000 redco-0.4.1/redco/deployers/model_parallel_utils/partition_utils.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1835 2023-04-19 06:51:00.000000 redco-0.4.1/redco/deployers/opt_utils.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-13 23:54:41.840000 redco-0.4.1/redco/predictors/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      628 2023-04-19 06:51:00.000000 redco-0.4.1/redco/predictors/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     4243 2023-04-19 06:51:00.000000 redco-0.4.1/redco/predictors/predictor.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1812 2023-04-19 06:51:00.000000 redco-0.4.1/redco/predictors/utils.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-13 23:54:41.840000 redco-0.4.1/redco/trainers/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      624 2023-04-19 06:51:00.000000 redco-0.4.1/redco/trainers/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)    12098 2023-04-19 06:51:00.000000 redco-0.4.1/redco/trainers/trainer.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2168 2023-04-19 06:51:00.000000 redco-0.4.1/redco/trainers/utils.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-05-13 23:54:41.840000 redco-0.4.1/redco.egg-info/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3628 2023-05-13 23:54:41.000000 redco-0.4.1/redco.egg-info/PKG-INFO
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      735 2023-05-13 23:54:41.000000 redco-0.4.1/redco.egg-info/SOURCES.txt
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)        1 2023-05-13 23:54:41.000000 redco-0.4.1/redco.egg-info/dependency_links.txt
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)       21 2023-05-13 23:54:41.000000 redco-0.4.1/redco.egg-info/requires.txt
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)        6 2023-05-13 23:54:41.000000 redco-0.4.1/redco.egg-info/top_level.txt
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)       38 2023-05-13 23:54:41.850000 redco-0.4.1/setup.cfg
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1001 2023-05-13 23:52:43.000000 redco-0.4.1/setup.py
```

### Comparing `redco-0.4.0/LICENSE` & `redco-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `redco-0.4.0/redco/__init__.py` & `redco-0.4.1/redco/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.0/redco/datasets/__init__.py` & `redco-0.4.1/redco/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.0/redco/datasets/dataset.py` & `redco-0.4.1/redco/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.0/redco/datasets/jsonl_dataset.py` & `redco-0.4.1/redco/datasets/jsonl_dataset.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.0/redco/deployers/__init__.py` & `redco-0.4.1/redco/deployers/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.0/redco/deployers/data_utils.py` & `redco-0.4.1/redco/deployers/data_utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.0/redco/deployers/deployer.py` & `redco-0.4.1/redco/deployers/deployer.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.0/redco/deployers/log_utils.py` & `redco-0.4.1/redco/deployers/log_utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.0/redco/deployers/model_parallel_utils/__init__.py` & `redco-0.4.1/redco/deployers/model_parallel_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.0/redco/deployers/model_parallel_utils/mesh_utils.py` & `redco-0.4.1/redco/deployers/model_parallel_utils/mesh_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,20 @@
 
             elif under_attention(key) and rule_key[0][0] == 'o':
                 shard_rules[rule_key] = P('mp', None)
 
             elif under_attention(key) and rule_key[0][0] in ['q', 'k', 'v']:
                 shard_rules[rule_key] = P(None, 'mp')
 
+            elif under_attention(key) and rule_key[0][-1] == 'o':
+                shard_rules[rule_key] = P('mp', None)
+
+            elif under_attention(key) and rule_key[0][-1] in ['q', 'k', 'v']:
+                shard_rules[rule_key] = P(None, 'mp')
+
             else:
                 rule_tuple = [None for _ in range(len(param.shape))]
                 for dim in range(-1, -len(param.shape) - 1, -1):
                     if dim != last_dense_mp_dim and \
                             param.shape[dim] % mesh_model_shards == 0:
                         last_dense_mp_dim = dim
                         rule_tuple[dim] = 'mp'
```

### Comparing `redco-0.4.0/redco/deployers/model_parallel_utils/partition_utils.py` & `redco-0.4.1/redco/deployers/model_parallel_utils/partition_utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.0/redco/deployers/opt_utils.py` & `redco-0.4.1/redco/deployers/opt_utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.0/redco/predictors/__init__.py` & `redco-0.4.1/redco/predictors/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.0/redco/predictors/predictor.py` & `redco-0.4.1/redco/predictors/predictor.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.0/redco/predictors/utils.py` & `redco-0.4.1/redco/predictors/utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.0/redco/trainers/__init__.py` & `redco-0.4.1/redco/trainers/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.0/redco/trainers/trainer.py` & `redco-0.4.1/redco/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.0/redco/trainers/utils.py` & `redco-0.4.1/redco/trainers/utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.0/redco.egg-info/SOURCES.txt` & `redco-0.4.1/redco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

