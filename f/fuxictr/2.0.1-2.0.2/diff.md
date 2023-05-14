# Comparing `tmp/fuxictr-2.0.1.tar.gz` & `tmp/fuxictr-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fuxictr-2.0.1.tar", last modified: Wed Feb 15 05:17:24 2023, max compression
+gzip compressed data, was "dist/fuxictr-2.0.2.tar", last modified: Sun May 14 08:27:02 2023, max compression
```

## Comparing `fuxictr-2.0.1.tar` & `fuxictr-2.0.2.tar`

### file list

```diff
@@ -1,92 +1,93 @@
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-15 05:17:24.000000 fuxictr-2.0.1/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    27357 2023-02-15 05:17:24.000000 fuxictr-2.0.1/PKG-INFO
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    25139 2023-02-15 03:29:49.000000 fuxictr-2.0.1/README.md
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-15 05:17:24.000000 fuxictr-2.0.1/fuxictr/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       32 2022-11-14 09:29:53.000000 fuxictr-2.0.1/fuxictr/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6523 2023-02-15 05:02:38.000000 fuxictr-2.0.1/fuxictr/autotuner.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-15 05:17:24.000000 fuxictr-2.0.1/fuxictr/datasets/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       64 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/datasets/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1592 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/datasets/avazu.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1231 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/datasets/criteo.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1826 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/datasets/kkbox.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5511 2023-02-14 09:47:22.000000 fuxictr-2.0.1/fuxictr/features.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4369 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/metrics.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-15 05:17:24.000000 fuxictr-2.0.1/fuxictr/preprocess/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       62 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/preprocess/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5950 2023-02-14 09:50:19.000000 fuxictr-2.0.1/fuxictr/preprocess/build_dataset.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    18559 2023-02-14 07:01:51.000000 fuxictr-2.0.1/fuxictr/preprocess/feature_processor.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     9373 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/preprocess/utils.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-15 05:17:24.000000 fuxictr-2.0.1/fuxictr/pytorch/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2021-08-10 06:39:20.000000 fuxictr-2.0.1/fuxictr/pytorch/__init__.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-15 05:17:24.000000 fuxictr-2.0.1/fuxictr/pytorch/dataloaders/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       91 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/pytorch/dataloaders/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5429 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/pytorch/dataloaders/h5_block_dataloader.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3907 2023-02-14 07:16:49.000000 fuxictr-2.0.1/fuxictr/pytorch/dataloaders/h5_dataloader.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-15 05:17:24.000000 fuxictr-2.0.1/fuxictr/pytorch/layers/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      164 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/pytorch/layers/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1463 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/pytorch/layers/activations.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-15 05:17:24.000000 fuxictr-2.0.1/fuxictr/pytorch/layers/attentions/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      108 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/pytorch/layers/attentions/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1810 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/pytorch/layers/attentions/dot_product_attention.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1750 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/pytorch/layers/attentions/squeeze_excitation.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5616 2023-02-14 09:15:25.000000 fuxictr-2.0.1/fuxictr/pytorch/layers/attentions/target_attention.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-15 05:17:24.000000 fuxictr-2.0.1/fuxictr/pytorch/layers/blocks/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      100 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/pytorch/layers/blocks/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1416 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/pytorch/layers/blocks/factorization_machine.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1489 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/pytorch/layers/blocks/logistic_regression.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3057 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/pytorch/layers/blocks/mlp_block.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-15 05:17:24.000000 fuxictr-2.0.1/fuxictr/pytorch/layers/embeddings/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       36 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/pytorch/layers/embeddings/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    11489 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/pytorch/layers/embeddings/feature_embedding.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-15 05:17:24.000000 fuxictr-2.0.1/fuxictr/pytorch/layers/interactions/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      244 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/pytorch/layers/interactions/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4734 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/pytorch/layers/interactions/bilinear_interaction.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2303 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/pytorch/layers/interactions/compressed_interaction_net.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5228 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/pytorch/layers/interactions/cross_net.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2940 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/pytorch/layers/interactions/holographic_interaction.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2924 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/pytorch/layers/interactions/inner_product.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2780 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/pytorch/layers/interactions/interaction_machine.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1820 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/pytorch/layers/pooling.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-15 05:17:24.000000 fuxictr-2.0.1/fuxictr/pytorch/models/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2761 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/pytorch/models/DNN.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       57 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/pytorch/models/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    12709 2023-02-14 07:18:08.000000 fuxictr-2.0.1/fuxictr/pytorch/models/base_model.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5363 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/pytorch/torch_utils.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-15 05:17:24.000000 fuxictr-2.0.1/fuxictr/tensorflow/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/tensorflow/__init__.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-15 05:17:24.000000 fuxictr-2.0.1/fuxictr/tensorflow/dataloaders/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       45 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/tensorflow/dataloaders/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3344 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/tensorflow/dataloaders/tf_dataloader.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-15 05:17:24.000000 fuxictr-2.0.1/fuxictr/tensorflow/layers/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      107 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/tensorflow/layers/__init__.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-15 05:17:24.000000 fuxictr-2.0.1/fuxictr/tensorflow/layers/blocks/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      123 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/tensorflow/layers/blocks/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1482 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/tensorflow/layers/blocks/factorization_machine.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1517 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/tensorflow/layers/blocks/linear.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1673 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/tensorflow/layers/blocks/logistic_regression.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3619 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/tensorflow/layers/blocks/mlp_block.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-15 05:17:24.000000 fuxictr-2.0.1/fuxictr/tensorflow/layers/embeddings/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       36 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/tensorflow/layers/embeddings/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    11853 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/tensorflow/layers/embeddings/feature_embedding.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-15 05:17:24.000000 fuxictr-2.0.1/fuxictr/tensorflow/layers/interactions/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       58 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/tensorflow/layers/interactions/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2088 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/tensorflow/layers/interactions/cross_net.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2969 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/tensorflow/layers/interactions/inner_product.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1065 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/tensorflow/layers/pooling.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-15 05:17:24.000000 fuxictr-2.0.1/fuxictr/tensorflow/models/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2572 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/tensorflow/models/DNN.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       57 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/tensorflow/models/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     9272 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/tensorflow/models/base_model.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2713 2023-01-27 08:57:12.000000 fuxictr-2.0.1/fuxictr/tensorflow/tf_utils.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4649 2023-02-15 05:02:33.000000 fuxictr-2.0.1/fuxictr/utils.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       23 2023-02-15 05:04:33.000000 fuxictr-2.0.1/fuxictr/version.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-15 05:17:24.000000 fuxictr-2.0.1/fuxictr.egg-info/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    27357 2023-02-15 05:17:23.000000 fuxictr-2.0.1/fuxictr.egg-info/PKG-INFO
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2717 2023-02-15 05:17:24.000000 fuxictr-2.0.1/fuxictr.egg-info/SOURCES.txt
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        1 2023-02-15 05:17:23.000000 fuxictr-2.0.1/fuxictr.egg-info/dependency_links.txt
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       48 2023-02-15 05:17:23.000000 fuxictr-2.0.1/fuxictr.egg-info/requires.txt
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        8 2023-02-15 05:17:23.000000 fuxictr-2.0.1/fuxictr.egg-info/top_level.txt
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-15 05:17:24.000000 fuxictr-2.0.1/model_zoo/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1356 2023-02-14 07:07:45.000000 fuxictr-2.0.1/model_zoo/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       38 2023-02-15 05:17:24.000000 fuxictr-2.0.1/setup.cfg
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1551 2023-02-15 05:03:56.000000 fuxictr-2.0.1/setup.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    29709 2023-05-14 08:27:02.000000 fuxictr-2.0.2/PKG-INFO
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    27403 2023-05-14 08:13:39.000000 fuxictr-2.0.2/README.md
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:01.000000 fuxictr-2.0.2/fuxictr/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       32 2022-11-14 09:29:53.000000 fuxictr-2.0.2/fuxictr/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6557 2023-05-11 07:17:04.000000 fuxictr-2.0.2/fuxictr/autotuner.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/datasets/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       64 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/datasets/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1592 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/datasets/avazu.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1231 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/datasets/criteo.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1826 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/datasets/kkbox.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5503 2023-02-17 01:18:00.000000 fuxictr-2.0.2/fuxictr/features.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4369 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/metrics.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/preprocess/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       62 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/preprocess/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5950 2023-02-14 09:50:19.000000 fuxictr-2.0.2/fuxictr/preprocess/build_dataset.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    18559 2023-02-14 07:01:51.000000 fuxictr-2.0.2/fuxictr/preprocess/feature_processor.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     9373 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/preprocess/utils.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/pytorch/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2021-08-10 06:39:20.000000 fuxictr-2.0.2/fuxictr/pytorch/__init__.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/pytorch/dataloaders/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       91 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/dataloaders/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5429 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/dataloaders/h5_block_dataloader.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3907 2023-02-14 07:16:49.000000 fuxictr-2.0.2/fuxictr/pytorch/dataloaders/h5_dataloader.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      164 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1463 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/activations.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/attentions/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      108 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/attentions/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1810 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/attentions/dot_product_attention.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1750 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/attentions/squeeze_excitation.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5616 2023-02-14 09:15:25.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/attentions/target_attention.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/blocks/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      100 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/blocks/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1416 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/blocks/factorization_machine.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1489 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/blocks/logistic_regression.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2797 2023-05-14 00:04:17.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/blocks/mlp_block.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/embeddings/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       36 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/embeddings/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    11489 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/embeddings/feature_embedding.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/interactions/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      244 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/interactions/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4734 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/interactions/bilinear_interaction.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2303 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/interactions/compressed_interaction_net.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5228 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/interactions/cross_net.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2940 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/interactions/holographic_interaction.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2924 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/interactions/inner_product.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2780 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/interactions/interaction_machine.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1820 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/pooling.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/pytorch/models/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       77 2023-05-14 00:00:11.000000 fuxictr-2.0.2/fuxictr/pytorch/models/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    12709 2023-02-14 07:18:08.000000 fuxictr-2.0.2/fuxictr/pytorch/models/ctr_model.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6182 2023-04-18 04:15:15.000000 fuxictr-2.0.2/fuxictr/pytorch/models/multitask_model.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5363 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/torch_utils.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/tensorflow/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/__init__.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/tensorflow/dataloaders/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       45 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/dataloaders/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3344 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/dataloaders/tf_dataloader.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      107 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/__init__.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/blocks/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      123 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/blocks/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1482 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/blocks/factorization_machine.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1517 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/blocks/linear.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1673 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/blocks/logistic_regression.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3619 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/blocks/mlp_block.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/embeddings/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       36 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/embeddings/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    11853 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/embeddings/feature_embedding.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/interactions/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       58 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/interactions/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2088 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/interactions/cross_net.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2969 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/interactions/inner_product.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1065 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/pooling.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/tensorflow/models/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       32 2023-05-14 00:02:55.000000 fuxictr-2.0.2/fuxictr/tensorflow/models/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     9272 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/models/ctr_model.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2713 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/tf_utils.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4649 2023-02-15 05:02:33.000000 fuxictr-2.0.2/fuxictr/utils.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       23 2023-05-14 08:25:19.000000 fuxictr-2.0.2/fuxictr/version.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr.egg-info/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    29709 2023-05-14 08:27:01.000000 fuxictr-2.0.2/fuxictr.egg-info/PKG-INFO
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2726 2023-05-14 08:27:01.000000 fuxictr-2.0.2/fuxictr.egg-info/SOURCES.txt
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        1 2023-05-14 08:27:01.000000 fuxictr-2.0.2/fuxictr.egg-info/dependency_links.txt
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       48 2023-05-14 08:27:01.000000 fuxictr-2.0.2/fuxictr.egg-info/requires.txt
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       18 2023-05-14 08:27:01.000000 fuxictr-2.0.2/fuxictr.egg-info/top_level.txt
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/model_zoo/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1399 2023-04-18 04:15:15.000000 fuxictr-2.0.2/model_zoo/__init__.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/model_zoo/multitask/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       69 2023-04-18 04:15:15.000000 fuxictr-2.0.2/model_zoo/multitask/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       38 2023-05-14 08:27:02.000000 fuxictr-2.0.2/setup.cfg
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1551 2023-05-14 08:25:35.000000 fuxictr-2.0.2/setup.py
```

### Comparing `fuxictr-2.0.1/PKG-INFO` & `fuxictr-2.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuxictr
-Version: 2.0.1
+Version: 2.0.2
 Summary: A configurable, tunable, and reproducible library for CTR prediction
 Home-page: https://github.com/xue-pai/FuxiCTR
 Author: zhujiem
 Author-email: zhujiem@users.noreply.github.com
 License: Apache-2.0 License
 Download-URL: https://github.com/xue-pai/FuxiCTR/tags
 Description: <div align="center">
@@ -41,70 +41,77 @@
         
         
         ## Model Zoo
         
         | No  | Publication       | Model                                    | Paper                                                                                                                                                                                                           | Benchmark                                                                                                       | Version       |
         |:---:|:-----------------:|:----------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |:---------------------------------------------------------------------------------------------------------------:|:-------------:|
         |     |                   |                                          | :point_down:**Feature Interaction Models**                                                                                                                                                                      |                                                                                                                 |               |
-        | 1   | WWW'07            | [LR](./model_zoo/LR)                     | [Predicting Clicks: Estimating the Click-Through Rate for New Ads](https://dl.acm.org/citation.cfm?id=1242643) :triangular_flag_on_post:**Microsoft**                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/LR)           | `torch`       |
-        | 2   | ICDM'10           | [FM](./model_zoo/FM)                     | [Factorization Machines](https://www.csie.ntu.edu.tw/~b97053/paper/Rendle2010FM.pdf)                                                                                                                            | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/FM)           | `torch`       |
-        | 3   | CIKM'13           | [DSSM](./model_zoo/DSSM)                 | [Learning Deep Structured Semantic Models  for Web Search using Clickthrough Data ](https://posenhuang.github.io/papers/cikm2013_DSSM_fullversion.pdf) :triangular_flag_on_post:**Microsoft**                   | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DSSM)         | `torch`       |
-        | 4   | CIKM'15           | [CCPM](./model_zoo/CCPM)                 | [A Convolutional Click Prediction Model](http://www.escience.cn/system/download/73676)                                                                                                                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/CCPM)         | `torch`       |
-        | 5   | RecSys'16         | [FFM](./model_zoo/FFM)                   | [Field-aware Factorization Machines for CTR Prediction](https://dl.acm.org/citation.cfm?id=2959134) :triangular_flag_on_post:**Criteo**                                                                         | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/FFM)          | `torch`       |
-        | 6   | RecSys'16         | [YoutubeDNN](./model_zoo/DNN)            | [Deep Neural Networks for YouTube Recommendations](http://art.yale.edu/file_columns/0001/1132/covington.pdf) :triangular_flag_on_post:**Google**                                                                | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DNN)          | `torch`, `tf` |
-        | 7   | DLRS'16           | [Wide&Deep](./model_zoo/WideDeep)        | [Wide & Deep Learning for Recommender Systems](https://arxiv.org/pdf/1606.07792.pdf) :triangular_flag_on_post:**Google**                                                                                        | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/WideDeep)     | `torch`, `tf` |
-        | 8   | ICDM'16           | [IPNN](./model_zoo/PNN)                  | [Product-based Neural Networks for User Response Prediction](https://arxiv.org/pdf/1611.00144.pdf)                                                                                                              | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/IPNN)         | `torch`       |
-        | 9   | KDD'16            | [DeepCrossing](./model_zoo/DeepCrossing) | [Deep Crossing: Web-Scale Modeling without Manually Crafted Combinatorial Features](https://www.kdd.org/kdd2016/papers/files/adf0975-shanA.pdf) :triangular_flag_on_post:**Microsoft**                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DeepCrossing) | `torch`       |
-        | 10  | NIPS'16           | [HOFM](./model_zoo/HOFM)                 | [Higher-Order Factorization Machines](https://papers.nips.cc/paper/6144-higher-order-factorization-machines.pdf)                                                                                                | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/HOFM)         | `torch`       |
-        | 11  | IJCAI'17          | [DeepFM](./model_zoo/DeepFM)             | [DeepFM: A Factorization-Machine based Neural Network for CTR Prediction](https://arxiv.org/abs/1703.04247) :triangular_flag_on_post:**Huawei**                                                                 | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DeepFM)       | `torch`, `tf` |
-        | 12  | SIGIR'17          | [NFM](./model_zoo/NFM)                   | [Neural Factorization Machines for Sparse Predictive Analytics](https://dl.acm.org/citation.cfm?id=3080777)                                                                                                     | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/NFM)          | `torch`       |
-        | 13  | IJCAI'17          | [AFM](./model_zoo/AFM)                   | [Attentional Factorization Machines: Learning the Weight of Feature Interactions via Attention Networks](http://www.ijcai.org/proceedings/2017/0435.pdf)                                                        | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/AFM)          | `torch`       |
-        | 14  | ADKDD'17          | [DCN](./model_zoo/DCN)                   | [Deep & Cross Network for Ad Click Predictions](https://arxiv.org/abs/1708.05123) :triangular_flag_on_post:**Google**                                                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DCN)          | `torch`, `tf` |
-        | 15  | WWW'18            | [FwFM](./model_zoo/FwFM)                 | [Field-weighted Factorization Machines for Click-Through Rate Prediction in Display Advertising](https://arxiv.org/pdf/1806.03514.pdf) :triangular_flag_on_post:**Oath, TouchPal, LinkedIn, Alibaba**           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/FwFM)         | `torch`       |
-        | 16  | KDD'18            | [xDeepFM](./model_zoo/xDeepFM)           | [xDeepFM: Combining Explicit and Implicit Feature Interactions for Recommender Systems](https://arxiv.org/pdf/1803.05170.pdf) :triangular_flag_on_post:**Microsoft**                                            | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/xDeepFM)      | `torch`       |
-        | 17  | CIKM'19           | [FiGNN](./model_zoo/FiGNN)               | [FiGNN: Modeling Feature Interactions via Graph Neural Networks for CTR Prediction](https://arxiv.org/abs/1910.05552)                                                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/FiGNN)        | `torch`       |
-        | 18  | CIKM'19           | [AutoInt/AutoInt+](./model_zoo/AutoInt)  | [AutoInt: Automatic Feature Interaction Learning via Self-Attentive Neural Networks](https://arxiv.org/abs/1810.11921)                                                                                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/AutoInt)      | `torch`       |
-        | 19  | RecSys'19         | [FiBiNET](./model_zoo/FiBiNET)           | [FiBiNET: Combining Feature Importance and Bilinear feature Interaction for Click-Through Rate Prediction](https://arxiv.org/abs/1905.09433) :triangular_flag_on_post:**Sina Weibo**                            | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/FiBiNET)      | `torch`       |
-        | 20  | WWW'19            | [FGCNN](./model_zoo/FGCNN)               | [Feature Generation by Convolutional Neural Network for Click-Through Rate Prediction](https://arxiv.org/abs/1904.04447) :triangular_flag_on_post:**Huawei**                                                    | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/FGCNN)        | `torch`       |
-        | 21  | AAAI'19           | [HFM/HFM+](./model_zoo/HFM)              | [Holographic Factorization Machines for Recommendation](https://ojs.aaai.org//index.php/AAAI/article/view/4448)                                                                                                 | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/HFM)          | `torch`       |
-        | 22  | Arxiv'19          | [DLRM](./model_zoo/DLRM)                 | [Deep Learning Recommendation Model for Personalization and Recommendation Systems](https://arxiv.org/abs/1906.00091) :triangular_flag_on_post:**Facebook**                                                     | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DLRM)         | `torch`       |
-        | 23  | NeuralNetworks'20 | [ONN](./model_zoo/ONN)                   | [Operation-aware Neural Networks for User Response Prediction](https://arxiv.org/pdf/1904.12579)                                                                                                                | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/ONN)          | `torch`       |
-        | 24  | AAAI'20           | [AFN/AFN+](./model_zoo/AFN)              | [Adaptive Factorization Network: Learning Adaptive-Order Feature Interactions](https://ojs.aaai.org/index.php/AAAI/article/view/5768)                                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/AFN)          | `torch`       |
-        | 25  | AAAI'20           | [LorentzFM](./model_zoo/LorentzFM)       | [Learning Feature Interactions with Lorentzian Factorization](https://arxiv.org/abs/1911.09821) :triangular_flag_on_post:**eBay**                                                                               | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/LorentzFM)    | `torch`       |
-        | 26  | WSDM'20           | [InterHAt](./model_zoo/InterHAt)         | [Interpretable Click-through Rate Prediction through Hierarchical Attention](https://dl.acm.org/doi/10.1145/3336191.3371785) :triangular_flag_on_post:**NEC Labs, Google**                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/InterHAt)     | `torch`       |
-        | 27  | DLP-KDD'20        | [FLEN](./model_zoo/FLEN)                 | [FLEN: Leveraging Field for Scalable CTR Prediction](https://arxiv.org/abs/1911.04690) :triangular_flag_on_post:**Tencent**                                                                                     | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/FLEN)         | `torch`       |
-        | 28  | CIKM'20           | [DeepIM](./model_zoo/DeepIM)             | [Deep Interaction Machine: A Simple but Effective Model for High-order Feature Interactions](https://dl.acm.org/doi/abs/10.1145/3340531.3412077) :triangular_flag_on_post:**Alibaba, RealAI**                   | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DeepIM)       | `torch`       |
-        | 29  | WWW'21            | [FmFM](./model_zoo/FmFM)                 | [FM^2: Field-matrixed Factorization Machines for Recommender Systems](https://arxiv.org/abs/2102.12994) :triangular_flag_on_post:**Yahoo**                                                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/FmFM)         | `torch`       |
-        | 30  | WWW'21            | [DCN-V2](./model_zoo/DCNv2)              | [DCN V2: Improved Deep & Cross Network and Practical Lessons for Web-scale Learning to Rank Systems](https://arxiv.org/abs/2008.13535) :triangular_flag_on_post:**Google**                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DCNv2)        | `torch`       |
-        | 31  | CIKM'21           | [DESTINE](./model_zoo/DESTINE)           | [Disentangled Self-Attentive Neural Networks for Click-Through Rate Prediction](https://arxiv.org/abs/2101.03654) :triangular_flag_on_post:**Alibaba**                                                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DESTINE)      | `torch`       |
-        | 32  | CIKM'21           | [EDCN](./model_zoo/EDCN)                 | [Enhancing Explicit and Implicit Feature Interactions via Information Sharing for Parallel Deep CTR Models](https://dlp-kdd.github.io/assets/pdf/DLP-KDD_2021_paper_12.pdf) :triangular_flag_on_post:**Huawei** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/EDCN)         | `torch`       |
-        | 33  | DLP-KDD'21        | [MaskNet](./model_zoo/MaskNet)           | [MaskNet: Introducing Feature-Wise Multiplication to CTR Ranking Models by Instance-Guided Mask](https://arxiv.org/abs/2102.07619) :triangular_flag_on_post:**Sina Weibo**                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/MaskNet)      | `torch`       |
-        | 34  | SIGIR'21          | [SAM](./model_zoo/SAM)                   | [Looking at CTR Prediction Again: Is Attention All You Need?](https://arxiv.org/abs/2105.05563) :triangular_flag_on_post:**BOSS Zhipin**                                                                        | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/SAM)          | `torch`       |
-        | 35  | KDD'21            | [AOANet](./model_zoo/AOANet)             | [Architecture and Operation Adaptive Network for Online Recommendations](https://dl.acm.org/doi/10.1145/3447548.3467133) :triangular_flag_on_post:**Didi Chuxing**                                              | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/AOANet)       | `torch`       |
-        | 36  | Blog'21           | [PPNet](./model_zoo/PPNet)               | [Parameter Personalized Net](https://www.jiqizhixin.com/articles/2021-02-03-6) :triangular_flag_on_post:**KuaiShou**                                                                                            |                                                                                                                 | `torch`       |
-        | 37  | AAAI'23           | [FinalMLP](./model_zoo/FinalMLP)         | FinalMLP: An Enhanced Two-Stream MLP Model for CTR Prediction :triangular_flag_on_post:**Huawei**                                                                                                               |                                                                                                                 | `torch`       |
+        | 1   | WWW'07            | [LR](./model_zoo/LR)                     | [Predicting Clicks: Estimating the Click-Through Rate for New Ads](https://dl.acm.org/citation.cfm?id=1242643) :triangular_flag_on_post:**Microsoft**                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/LR)           | `torch`       |
+        | 2   | ICDM'10           | [FM](./model_zoo/FM)                     | [Factorization Machines](https://www.csie.ntu.edu.tw/~b97053/paper/Rendle2010FM.pdf)                                                                                                                            | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FM)           | `torch`       |
+        | 3   | CIKM'13           | [DSSM](./model_zoo/DSSM)                 | [Learning Deep Structured Semantic Models  for Web Search using Clickthrough Data ](https://posenhuang.github.io/papers/cikm2013_DSSM_fullversion.pdf) :triangular_flag_on_post:**Microsoft**                   | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DSSM)         | `torch`       |
+        | 4   | CIKM'15           | [CCPM](./model_zoo/CCPM)                 | [A Convolutional Click Prediction Model](http://www.escience.cn/system/download/73676)                                                                                                                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/CCPM)         | `torch`       |
+        | 5   | RecSys'16         | [FFM](./model_zoo/FFM)                   | [Field-aware Factorization Machines for CTR Prediction](https://dl.acm.org/citation.cfm?id=2959134) :triangular_flag_on_post:**Criteo**                                                                         | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FFM)          | `torch`       |
+        | 6   | RecSys'16         | [DNN](./model_zoo/DNN)            | [Deep Neural Networks for YouTube Recommendations](http://art.yale.edu/file_columns/0001/1132/covington.pdf) :triangular_flag_on_post:**Google**                                                                | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DNN)          | `torch`, `tf` |
+        | 7   | DLRS'16           | [Wide&Deep](./model_zoo/WideDeep)        | [Wide & Deep Learning for Recommender Systems](https://arxiv.org/pdf/1606.07792.pdf) :triangular_flag_on_post:**Google**                                                                                        | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/WideDeep)     | `torch`, `tf` |
+        | 8   | ICDM'16           | [IPNN](./model_zoo/PNN)                  | [Product-based Neural Networks for User Response Prediction](https://arxiv.org/pdf/1611.00144.pdf)                                                                                                              | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/IPNN)         | `torch`       |
+        | 9   | KDD'16            | [DeepCrossing](./model_zoo/DeepCrossing) | [Deep Crossing: Web-Scale Modeling without Manually Crafted Combinatorial Features](https://www.kdd.org/kdd2016/papers/files/adf0975-shanA.pdf) :triangular_flag_on_post:**Microsoft**                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DeepCrossing) | `torch`       |
+        | 10  | NIPS'16           | [HOFM](./model_zoo/HOFM)                 | [Higher-Order Factorization Machines](https://papers.nips.cc/paper/6144-higher-order-factorization-machines.pdf)                                                                                                | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/HOFM)         | `torch`       |
+        | 11  | IJCAI'17          | [DeepFM](./model_zoo/DeepFM)             | [DeepFM: A Factorization-Machine based Neural Network for CTR Prediction](https://arxiv.org/abs/1703.04247) :triangular_flag_on_post:**Huawei**                                                                 | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DeepFM)       | `torch`, `tf` |
+        | 12  | SIGIR'17          | [NFM](./model_zoo/NFM)                   | [Neural Factorization Machines for Sparse Predictive Analytics](https://dl.acm.org/citation.cfm?id=3080777)                                                                                                     | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/NFM)          | `torch`       |
+        | 13  | IJCAI'17          | [AFM](./model_zoo/AFM)                   | [Attentional Factorization Machines: Learning the Weight of Feature Interactions via Attention Networks](http://www.ijcai.org/proceedings/2017/0435.pdf)                                                        | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/AFM)          | `torch`       |
+        | 14  | ADKDD'17          | [DCN](./model_zoo/DCN)                   | [Deep & Cross Network for Ad Click Predictions](https://arxiv.org/abs/1708.05123) :triangular_flag_on_post:**Google**                                                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DCN)          | `torch`, `tf` |
+        | 15  | WWW'18            | [FwFM](./model_zoo/FwFM)                 | [Field-weighted Factorization Machines for Click-Through Rate Prediction in Display Advertising](https://arxiv.org/pdf/1806.03514.pdf) :triangular_flag_on_post:**Oath, TouchPal, LinkedIn, Alibaba**           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FwFM)         | `torch`       |
+        | 16  | KDD'18            | [xDeepFM](./model_zoo/xDeepFM)           | [xDeepFM: Combining Explicit and Implicit Feature Interactions for Recommender Systems](https://arxiv.org/pdf/1803.05170.pdf) :triangular_flag_on_post:**Microsoft**                                            | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/xDeepFM)      | `torch`       |
+        | 17  | CIKM'19           | [FiGNN](./model_zoo/FiGNN)               | [FiGNN: Modeling Feature Interactions via Graph Neural Networks for CTR Prediction](https://arxiv.org/abs/1910.05552)                                                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FiGNN)        | `torch`       |
+        | 18  | CIKM'19           | [AutoInt/AutoInt+](./model_zoo/AutoInt)  | [AutoInt: Automatic Feature Interaction Learning via Self-Attentive Neural Networks](https://arxiv.org/abs/1810.11921)                                                                                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/AutoInt)      | `torch`       |
+        | 19  | RecSys'19         | [FiBiNET](./model_zoo/FiBiNET)           | [FiBiNET: Combining Feature Importance and Bilinear feature Interaction for Click-Through Rate Prediction](https://arxiv.org/abs/1905.09433) :triangular_flag_on_post:**Sina Weibo**                            | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FiBiNET)      | `torch`       |
+        | 20  | WWW'19            | [FGCNN](./model_zoo/FGCNN)               | [Feature Generation by Convolutional Neural Network for Click-Through Rate Prediction](https://arxiv.org/abs/1904.04447) :triangular_flag_on_post:**Huawei**                                                    | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FGCNN)        | `torch`       |
+        | 21  | AAAI'19           | [HFM/HFM+](./model_zoo/HFM)              | [Holographic Factorization Machines for Recommendation](https://ojs.aaai.org//index.php/AAAI/article/view/4448)                                                                                                 | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/HFM)          | `torch`       |
+        | 22  | Arxiv'19          | [DLRM](./model_zoo/DLRM)                 | [Deep Learning Recommendation Model for Personalization and Recommendation Systems](https://arxiv.org/abs/1906.00091) :triangular_flag_on_post:**Facebook**                                                     | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DLRM)         | `torch`       |
+        | 23  | NeuralNetworks'20 | [ONN](./model_zoo/ONN)                   | [Operation-aware Neural Networks for User Response Prediction](https://arxiv.org/pdf/1904.12579)                                                                                                                | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/ONN)          | `torch`       |
+        | 24  | AAAI'20           | [AFN/AFN+](./model_zoo/AFN)              | [Adaptive Factorization Network: Learning Adaptive-Order Feature Interactions](https://ojs.aaai.org/index.php/AAAI/article/view/5768)                                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/AFN)          | `torch`       |
+        | 25  | AAAI'20           | [LorentzFM](./model_zoo/LorentzFM)       | [Learning Feature Interactions with Lorentzian Factorization](https://arxiv.org/abs/1911.09821) :triangular_flag_on_post:**eBay**                                                                               | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/LorentzFM)    | `torch`       |
+        | 26  | WSDM'20           | [InterHAt](./model_zoo/InterHAt)         | [Interpretable Click-through Rate Prediction through Hierarchical Attention](https://dl.acm.org/doi/10.1145/3336191.3371785) :triangular_flag_on_post:**NEC Labs, Google**                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/InterHAt)     | `torch`       |
+        | 27  | DLP-KDD'20        | [FLEN](./model_zoo/FLEN)                 | [FLEN: Leveraging Field for Scalable CTR Prediction](https://arxiv.org/abs/1911.04690) :triangular_flag_on_post:**Tencent**                                                                                     | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FLEN)         | `torch`       |
+        | 28  | CIKM'20           | [DeepIM](./model_zoo/DeepIM)             | [Deep Interaction Machine: A Simple but Effective Model for High-order Feature Interactions](https://dl.acm.org/doi/abs/10.1145/3340531.3412077) :triangular_flag_on_post:**Alibaba, RealAI**                   | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DeepIM)       | `torch`       |
+        | 29  | WWW'21            | [FmFM](./model_zoo/FmFM)                 | [FM^2: Field-matrixed Factorization Machines for Recommender Systems](https://arxiv.org/abs/2102.12994) :triangular_flag_on_post:**Yahoo**                                                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FmFM)         | `torch`       |
+        | 30  | WWW'21            | [DCN-V2](./model_zoo/DCNv2)              | [DCN V2: Improved Deep & Cross Network and Practical Lessons for Web-scale Learning to Rank Systems](https://arxiv.org/abs/2008.13535) :triangular_flag_on_post:**Google**                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DCNv2)        | `torch`       |
+        | 31  | CIKM'21           | [DESTINE](./model_zoo/DESTINE)           | [Disentangled Self-Attentive Neural Networks for Click-Through Rate Prediction](https://arxiv.org/abs/2101.03654) :triangular_flag_on_post:**Alibaba**                                                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DESTINE)      | `torch`       |
+        | 32  | CIKM'21           | [EDCN](./model_zoo/EDCN)                 | [Enhancing Explicit and Implicit Feature Interactions via Information Sharing for Parallel Deep CTR Models](https://dlp-kdd.github.io/assets/pdf/DLP-KDD_2021_paper_12.pdf) :triangular_flag_on_post:**Huawei** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/EDCN)         | `torch`       |
+        | 33  | DLP-KDD'21        | [MaskNet](./model_zoo/MaskNet)           | [MaskNet: Introducing Feature-Wise Multiplication to CTR Ranking Models by Instance-Guided Mask](https://arxiv.org/abs/2102.07619) :triangular_flag_on_post:**Sina Weibo**                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/MaskNet)      | `torch`       |
+        | 34  | SIGIR'21          | [SAM](./model_zoo/SAM)                   | [Looking at CTR Prediction Again: Is Attention All You Need?](https://arxiv.org/abs/2105.05563) :triangular_flag_on_post:**BOSS Zhipin**                                                                        | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/SAM)          | `torch`       |
+        | 35  | KDD'21            | [AOANet](./model_zoo/AOANet)             | [Architecture and Operation Adaptive Network for Online Recommendations](https://dl.acm.org/doi/10.1145/3447548.3467133) :triangular_flag_on_post:**Didi Chuxing**                                              | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/AOANet)       | `torch`       |
+        | 36  | AAAI'23           | [FinalMLP](./model_zoo/FinalMLP)         | [FinalMLP: An Enhanced Two-Stream MLP Model for CTR Prediction](https://arxiv.org/abs/2304.00902) :triangular_flag_on_post:**Huawei**                                                                                                               |     [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FinalMLP)         | `torch`       |
+        | 37  | SIGIR'23           | [FINAL](./model_zoo/FINAL)         | FINAL: Factorized Interaction Layer for CTR Prediction :triangular_flag_on_post:**Huawei**                                                                                                               |     [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FINAL)         | `torch`       |
         |     |                   |                                          | :point_down:**User Behavior Modeling**                                                                                                                                                                          |                                                                                                                 |               |
-        | 38  | KDD'18            | [DIN](./model_zoo/DIN)                   | [Deep Interest Network for Click-Through Rate Prediction](https://www.kdd.org/kdd2018/accepted-papers/view/deep-interest-network-for-click-through-rate-prediction) :triangular_flag_on_post:**Alibaba**        |                                                                                                                 | `torch`       |
-        | 39  | AAAI'19           | [DIEN](./model_zoo/DIEN)                 | [Deep Interest Evolution Network for Click-Through Rate Prediction](https://arxiv.org/abs/1809.03672) :triangular_flag_on_post:**Alibaba**                                                                      |                                                                                                                 | `torch`       |
-        | 40  | DLP-KDD'19        | [BST](./model_zoo/BST)                   | [Behavior Sequence Transformer for E-commerce Recommendation in Alibaba](https://arxiv.org/abs/1905.06874) :triangular_flag_on_post:**Alibaba**                                                                 |                                                                                                                 | `torch`       |
+        | 38  | KDD'18            | [DIN](./model_zoo/DIN)                   | [Deep Interest Network for Click-Through Rate Prediction](https://www.kdd.org/kdd2018/accepted-papers/view/deep-interest-network-for-click-through-rate-prediction) :triangular_flag_on_post:**Alibaba**        |   [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DIN)       | `torch`       |
+        | 39  | AAAI'19           | [DIEN](./model_zoo/DIEN)                 | [Deep Interest Evolution Network for Click-Through Rate Prediction](https://arxiv.org/abs/1809.03672) :triangular_flag_on_post:**Alibaba**                                                                      |   [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DIEN)        | `torch`       |
+        | 40  | DLP-KDD'19        | [BST](./model_zoo/BST)                   | [Behavior Sequence Transformer for E-commerce Recommendation in Alibaba](https://arxiv.org/abs/1905.06874) :triangular_flag_on_post:**Alibaba**                                                                 |  [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/BST)     | `torch`       |
         | 41  | CIKM'20           | [DMIN](./model_zoo/DMIN)                 | [Deep Multi-Interest Network for Click-through Rate Prediction](https://dl.acm.org/doi/10.1145/3340531.3412092) :triangular_flag_on_post:**Alibaba**                                                            |                                                                                                                 | `torch`       |
         | 42  | AAAI'20           | [DMR](./model_zoo/DMR)                   | [Deep Match to Rank Model for Personalized Click-Through Rate Prediction](https://ojs.aaai.org/index.php/AAAI/article/view/5346) :triangular_flag_on_post:**Alibaba**                                           |                                                                                                                 | `torch`       |
         | 43  | Arxiv'21          | [ETA](./model_zoo/ETA)                   | [End-to-End User Behavior Retrieval in Click-Through RatePrediction Model](https://arxiv.org/abs/2108.04468) :triangular_flag_on_post:**Alibaba**                                                               |                                                                                                                 | `torch`       |
         | 44  | CIKM'22           | [SDIM](./model_zoo/SDIM)                 | [Sampling Is All You Need on Modeling Long-Term User Behaviors for CTR Prediction](https://arxiv.org/abs/2205.10249) :triangular_flag_on_post:**Meituan**                                                       |                                                                                                                 | `torch`       |
+        |     |                   |                                          | :point_down:**Multi-Task Models**                                                                                                                                                                          |                                                                                                                 |               |
+        | 45  |     MachineLearn'97      | [SharedBottom](./model_zoo/multitask/SharedBottom)               | [Multitask Learning](https://link.springer.com/article/10.1023/A:1007379606734)                                                                                            |                                                                                                                 | `torch`       |
+        | 46  | KDD'18          | [MMoE](./model_zoo/multitask/MMOE)               | [Modeling Task Relationships in Multi-task Learning with Multi-Gate Mixture-of-Experts](https://dl.acm.org/doi/pdf/10.1145/3219819.3220007) :triangular_flag_on_post:**Google**                                                                                            |                                                                                                                 | `torch`       |
+        |     |                   |                                          | :point_down:**Multi-Domain Models**                                                                                                                                                                          |                                                                                                                 |               |
+        | 47  | Arxiv'23           | [PPNet](./model_zoo/PPNet)/PEPNet              | [PEPNet: Parameter and Embedding Personalized Network for Infusing with Personalized Prior Information](https://arxiv.org/abs/2302.01115) :triangular_flag_on_post:**KuaiShou**                                                                                            |                                                                                                                 | `torch`       |
+        
+        
+        + :point_right: See [reusable dataset splits for CTR prediction](https://openbenchmark.github.io/BARS/datasets/README.html).
+        + :point_right: See [benchmarking configurations and steps](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks).
+        + :point_right: See [the BARS benchmark leaderboard](https://openbenchmark.github.io/BARS/ctr_prediction/leaderboard/README.html#).
         
-        + :point_right: See [reusable dataset splits for CTR prediction](https://github.com/openbenchmark/BARS/blob/master/ctr_prediction/datasets).
-        + :point_right: See [benchmarking configurations and steps](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks).
-        + :point_right: See [the BARS benchmark website](https://openbenchmark.github.io/ctr-prediction).
         
         ## Dependencies
         
         FuxiCTR has the following dependency requirements. 
         
         + python 3.6+
-        + pytorch 1.10+ (required only for torch models)
+        + pytorch 1.0/1.10+ (required only for torch models)
         + tensorflow 2.1+ (required only for tf models)
         
         Other packages can be installed via `pip install -r requirements.txt`.
         
         ## Quick Start
         
         1. Run the demo examples
@@ -120,19 +127,23 @@
         2. Run an existing model
            
             Users can easily run each model in the model zoo following the commands below, which is a demo for running DCN. In addition, users can modify the dataset config and model config files to run on their own datasets or with new hyper-parameters. More details can be found in the [readme file](./model_zoo/DCN/DCN_torch/README.md).
            
            ```
            cd model_zoo/DCN/DCN_torch
            python run_expid.py --expid DCN_test --gpu 0
+        
+           # Change `MODEL` according to the target model name
+           cd model_zoo/MODEL_PATH
+           python run_expid.py --expid MODEL_test --gpu 0
            ```
         
         3. Implement a new model
            
-            The FuxiCTR code structure is modularized, so that every part can be overwritten by users according to their needs. In many cases, only the model class needs to be implemented for a new customized model. If data preprocessing or data loader is not directly applicable, one can also overwrite a new one through the [core APIs](https://www.processon.com/view/link/63cfcfab4e30670eac4a81c7). A complete example can be found at [model_zoo/FinalMLP](./model_zoo/FinalMLP/), which implements our new model FinalMLP that has been recently published in AAAI 2023. Some other examples are also available in the model zoo.
+            The FuxiCTR code structure is modularized, so that every part can be overwritten by users according to their needs. In many cases, only the model class needs to be implemented for a new customized model. If data preprocessing or data loader is not directly applicable, one can also overwrite a new one through the [core APIs](https://www.processon.com/view/link/63cfcfab4e30670eac4a81c7). We show a concrete example which implements our new model [FinalMLP](https://github.com/xue-pai/FinalMLP) that has been recently published in AAAI 2023. More examples can be found in the [model zoo](./model_zoo/).
         
         
         ## Citation
         
         *:bell: If you find our code or benchmarks helpful in your research, please kindly cite the following papers.*
         
         > Jieming Zhu, Jinyang Liu, Shuai Yang, Qi Zhang, Xiuqiang He. [Open Benchmarking for Click-Through Rate Prediction](https://arxiv.org/abs/2009.05794). *The 30th ACM International Conference on Information and Knowledge Management (CIKM)*, 2021. [[Bibtex](https://dblp.org/rec/conf/cikm/ZhuLYZH21.html?view=bibtex)]
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fuxictr Version: 2.0.1 Summary: A configurable,
+Metadata-Version: 2.1 Name: fuxictr Version: 2.0.2 Summary: A configurable,
 tunable, and reproducible library for CTR prediction Home-page: https://
 github.com/xue-pai/FuxiCTR Author: zhujiem Author-email:
 zhujiem@users.noreply.github.com License: Apache-2.0 License Download-URL:
 https://github.com/xue-pai/FuxiCTR/tags Description:
                                     [Logo]
 [Python_version] [Pytorch_version] [Pytorch_version] [Pypi_version] [Downloads]
                           [License] [Wechat_QR_code]
@@ -24,211 +24,229 @@
 -------------------------------------------------------------------------------
 ----------------------------------------------------------------------- |:-----
 -------------------------------------------------------------------------------
 ---------------------------:|:-------------:| | | | | :point_down:**Feature
 Interaction Models** | | | | 1 | WWW'07 | [LR](./model_zoo/LR) | [Predicting
 Clicks: Estimating the Click-Through Rate for New Ads](https://dl.acm.org/
 citation.cfm?id=1242643) :triangular_flag_on_post:**Microsoft** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
 ctr_prediction/benchmarks/LR) | `torch` | | 2 | ICDM'10 | [FM](./model_zoo/FM)
 | [Factorization Machines](https://www.csie.ntu.edu.tw/~b97053/paper/
 Rendle2010FM.pdf) | [:arrow_upper_right:](https://github.com/openbenchmark/
-BARS/tree/master/ctr_prediction/benchmarks/FM) | `torch` | | 3 | CIKM'13 |
-[DSSM](./model_zoo/DSSM) | [Learning Deep Structured Semantic Models for Web
-Search using Clickthrough Data ](https://posenhuang.github.io/papers/
+BARS/tree/main/ctr_prediction/benchmarks/FM) | `torch` | | 3 | CIKM'13 | [DSSM]
+(./model_zoo/DSSM) | [Learning Deep Structured Semantic Models for Web Search
+using Clickthrough Data ](https://posenhuang.github.io/papers/
 cikm2013_DSSM_fullversion.pdf) :triangular_flag_on_post:**Microsoft** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
 ctr_prediction/benchmarks/DSSM) | `torch` | | 4 | CIKM'15 | [CCPM](./model_zoo/
 CCPM) | [A Convolutional Click Prediction Model](http://www.escience.cn/system/
 download/73676) | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/
-tree/master/ctr_prediction/benchmarks/CCPM) | `torch` | | 5 | RecSys'16 | [FFM]
+tree/main/ctr_prediction/benchmarks/CCPM) | `torch` | | 5 | RecSys'16 | [FFM]
 (./model_zoo/FFM) | [Field-aware Factorization Machines for CTR Prediction]
 (https://dl.acm.org/citation.cfm?id=2959134) :triangular_flag_on_post:
 **Criteo** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
-master/ctr_prediction/benchmarks/FFM) | `torch` | | 6 | RecSys'16 |
-[YoutubeDNN](./model_zoo/DNN) | [Deep Neural Networks for YouTube
-Recommendations](http://art.yale.edu/file_columns/0001/1132/covington.pdf) :
-triangular_flag_on_post:**Google** | [:arrow_upper_right:](https://github.com/
-openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DNN) | `torch`, `tf` |
-| 7 | DLRS'16 | [Wide&Deep](./model_zoo/WideDeep) | [Wide & Deep Learning for
-Recommender Systems](https://arxiv.org/pdf/1606.07792.pdf) :
-triangular_flag_on_post:**Google** | [:arrow_upper_right:](https://github.com/
-openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/WideDeep) | `torch`,
-`tf` | | 8 | ICDM'16 | [IPNN](./model_zoo/PNN) | [Product-based Neural Networks
-for User Response Prediction](https://arxiv.org/pdf/1611.00144.pdf) | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/IPNN) | `torch` | | 9 | KDD'16 | [DeepCrossing](./
-model_zoo/DeepCrossing) | [Deep Crossing: Web-Scale Modeling without Manually
-Crafted Combinatorial Features](https://www.kdd.org/kdd2016/papers/files/
-adf0975-shanA.pdf) :triangular_flag_on_post:**Microsoft** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/DeepCrossing) | `torch` | | 10 | NIPS'16 | [HOFM](./
-model_zoo/HOFM) | [Higher-Order Factorization Machines](https://papers.nips.cc/
-paper/6144-higher-order-factorization-machines.pdf) | [:arrow_upper_right:]
-(https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/
-HOFM) | `torch` | | 11 | IJCAI'17 | [DeepFM](./model_zoo/DeepFM) | [DeepFM: A
-Factorization-Machine based Neural Network for CTR Prediction](https://
-arxiv.org/abs/1703.04247) :triangular_flag_on_post:**Huawei** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/DeepFM) | `torch`, `tf` | | 12 | SIGIR'17 | [NFM](./
-model_zoo/NFM) | [Neural Factorization Machines for Sparse Predictive
-Analytics](https://dl.acm.org/citation.cfm?id=3080777) | [:arrow_upper_right:]
-(https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/
-NFM) | `torch` | | 13 | IJCAI'17 | [AFM](./model_zoo/AFM) | [Attentional
-Factorization Machines: Learning the Weight of Feature Interactions via
-Attention Networks](http://www.ijcai.org/proceedings/2017/0435.pdf) | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/AFM) | `torch` | | 14 | ADKDD'17 | [DCN](./model_zoo/
-DCN) | [Deep & Cross Network for Ad Click Predictions](https://arxiv.org/abs/
-1708.05123) :triangular_flag_on_post:**Google** | [:arrow_upper_right:](https:/
-/github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DCN) |
-`torch`, `tf` | | 15 | WWW'18 | [FwFM](./model_zoo/FwFM) | [Field-weighted
-Factorization Machines for Click-Through Rate Prediction in Display
-Advertising](https://arxiv.org/pdf/1806.03514.pdf) :triangular_flag_on_post:
-**Oath, TouchPal, LinkedIn, Alibaba** | [:arrow_upper_right:](https://
-github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/FwFM) |
-`torch` | | 16 | KDD'18 | [xDeepFM](./model_zoo/xDeepFM) | [xDeepFM: Combining
-Explicit and Implicit Feature Interactions for Recommender Systems](https://
-arxiv.org/pdf/1803.05170.pdf) :triangular_flag_on_post:**Microsoft** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/xDeepFM) | `torch` | | 17 | CIKM'19 | [FiGNN](./
-model_zoo/FiGNN) | [FiGNN: Modeling Feature Interactions via Graph Neural
-Networks for CTR Prediction](https://arxiv.org/abs/1910.05552) | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/FiGNN) | `torch` | | 18 | CIKM'19 | [AutoInt/
-AutoInt+](./model_zoo/AutoInt) | [AutoInt: Automatic Feature Interaction
-Learning via Self-Attentive Neural Networks](https://arxiv.org/abs/1810.11921)
-| [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/AutoInt) | `torch` | | 19 | RecSys'19 | [FiBiNET](./
-model_zoo/FiBiNET) | [FiBiNET: Combining Feature Importance and Bilinear
-feature Interaction for Click-Through Rate Prediction](https://arxiv.org/abs/
-1905.09433) :triangular_flag_on_post:**Sina Weibo** | [:arrow_upper_right:]
-(https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/
-FiBiNET) | `torch` | | 20 | WWW'19 | [FGCNN](./model_zoo/FGCNN) | [Feature
-Generation by Convolutional Neural Network for Click-Through Rate Prediction]
-(https://arxiv.org/abs/1904.04447) :triangular_flag_on_post:**Huawei** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/FGCNN) | `torch` | | 21 | AAAI'19 | [HFM/HFM+](./
-model_zoo/HFM) | [Holographic Factorization Machines for Recommendation](https:
-//ojs.aaai.org//index.php/AAAI/article/view/4448) | [:arrow_upper_right:]
-(https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/
-HFM) | `torch` | | 22 | Arxiv'19 | [DLRM](./model_zoo/DLRM) | [Deep Learning
-Recommendation Model for Personalization and Recommendation Systems](https://
-arxiv.org/abs/1906.00091) :triangular_flag_on_post:**Facebook** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/DLRM) | `torch` | | 23 | NeuralNetworks'20 | [ONN](./
-model_zoo/ONN) | [Operation-aware Neural Networks for User Response Prediction]
-(https://arxiv.org/pdf/1904.12579) | [:arrow_upper_right:](https://github.com/
-openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/ONN) | `torch` | | 24
-| AAAI'20 | [AFN/AFN+](./model_zoo/AFN) | [Adaptive Factorization Network:
-Learning Adaptive-Order Feature Interactions](https://ojs.aaai.org/index.php/
-AAAI/article/view/5768) | [:arrow_upper_right:](https://github.com/
-openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/AFN) | `torch` | | 25
-| AAAI'20 | [LorentzFM](./model_zoo/LorentzFM) | [Learning Feature Interactions
-with Lorentzian Factorization](https://arxiv.org/abs/1911.09821) :
-triangular_flag_on_post:**eBay** | [:arrow_upper_right:](https://github.com/
-openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/LorentzFM) | `torch` |
-| 26 | WSDM'20 | [InterHAt](./model_zoo/InterHAt) | [Interpretable Click-
-through Rate Prediction through Hierarchical Attention](https://dl.acm.org/doi/
-10.1145/3336191.3371785) :triangular_flag_on_post:**NEC Labs, Google** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/InterHAt) | `torch` | | 27 | DLP-KDD'20 | [FLEN](./
-model_zoo/FLEN) | [FLEN: Leveraging Field for Scalable CTR Prediction](https://
-arxiv.org/abs/1911.04690) :triangular_flag_on_post:**Tencent** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/FLEN) | `torch` | | 28 | CIKM'20 | [DeepIM](./
-model_zoo/DeepIM) | [Deep Interaction Machine: A Simple but Effective Model for
-High-order Feature Interactions](https://dl.acm.org/doi/abs/10.1145/
-3340531.3412077) :triangular_flag_on_post:**Alibaba, RealAI** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
+main/ctr_prediction/benchmarks/FFM) | `torch` | | 6 | RecSys'16 | [DNN](./
+model_zoo/DNN) | [Deep Neural Networks for YouTube Recommendations](http://
+art.yale.edu/file_columns/0001/1132/covington.pdf) :triangular_flag_on_post:
+**Google** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
+main/ctr_prediction/benchmarks/DNN) | `torch`, `tf` | | 7 | DLRS'16 |
+[Wide&Deep](./model_zoo/WideDeep) | [Wide & Deep Learning for Recommender
+Systems](https://arxiv.org/pdf/1606.07792.pdf) :triangular_flag_on_post:
+**Google** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
+main/ctr_prediction/benchmarks/WideDeep) | `torch`, `tf` | | 8 | ICDM'16 |
+[IPNN](./model_zoo/PNN) | [Product-based Neural Networks for User Response
+Prediction](https://arxiv.org/pdf/1611.00144.pdf) | [:arrow_upper_right:]
+(https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/
+IPNN) | `torch` | | 9 | KDD'16 | [DeepCrossing](./model_zoo/DeepCrossing) |
+[Deep Crossing: Web-Scale Modeling without Manually Crafted Combinatorial
+Features](https://www.kdd.org/kdd2016/papers/files/adf0975-shanA.pdf) :
+triangular_flag_on_post:**Microsoft** | [:arrow_upper_right:](https://
+github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DeepCrossing)
+| `torch` | | 10 | NIPS'16 | [HOFM](./model_zoo/HOFM) | [Higher-Order
+Factorization Machines](https://papers.nips.cc/paper/6144-higher-order-
+factorization-machines.pdf) | [:arrow_upper_right:](https://github.com/
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/HOFM) | `torch` | | 11 |
+IJCAI'17 | [DeepFM](./model_zoo/DeepFM) | [DeepFM: A Factorization-Machine
+based Neural Network for CTR Prediction](https://arxiv.org/abs/1703.04247) :
+triangular_flag_on_post:**Huawei** | [:arrow_upper_right:](https://github.com/
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DeepFM) | `torch`, `tf`
+| | 12 | SIGIR'17 | [NFM](./model_zoo/NFM) | [Neural Factorization Machines for
+Sparse Predictive Analytics](https://dl.acm.org/citation.cfm?id=3080777) | [:
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/NFM) | `torch` | | 13 | IJCAI'17 | [AFM](./model_zoo/
+AFM) | [Attentional Factorization Machines: Learning the Weight of Feature
+Interactions via Attention Networks](http://www.ijcai.org/proceedings/2017/
+0435.pdf) | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
+main/ctr_prediction/benchmarks/AFM) | `torch` | | 14 | ADKDD'17 | [DCN](./
+model_zoo/DCN) | [Deep & Cross Network for Ad Click Predictions](https://
+arxiv.org/abs/1708.05123) :triangular_flag_on_post:**Google** | [:
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/DCN) | `torch`, `tf` | | 15 | WWW'18 | [FwFM](./
+model_zoo/FwFM) | [Field-weighted Factorization Machines for Click-Through Rate
+Prediction in Display Advertising](https://arxiv.org/pdf/1806.03514.pdf) :
+triangular_flag_on_post:**Oath, TouchPal, LinkedIn, Alibaba** | [:
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/FwFM) | `torch` | | 16 | KDD'18 | [xDeepFM](./
+model_zoo/xDeepFM) | [xDeepFM: Combining Explicit and Implicit Feature
+Interactions for Recommender Systems](https://arxiv.org/pdf/1803.05170.pdf) :
+triangular_flag_on_post:**Microsoft** | [:arrow_upper_right:](https://
+github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/xDeepFM) |
+`torch` | | 17 | CIKM'19 | [FiGNN](./model_zoo/FiGNN) | [FiGNN: Modeling
+Feature Interactions via Graph Neural Networks for CTR Prediction](https://
+arxiv.org/abs/1910.05552) | [:arrow_upper_right:](https://github.com/
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FiGNN) | `torch` | | 18
+| CIKM'19 | [AutoInt/AutoInt+](./model_zoo/AutoInt) | [AutoInt: Automatic
+Feature Interaction Learning via Self-Attentive Neural Networks](https://
+arxiv.org/abs/1810.11921) | [:arrow_upper_right:](https://github.com/
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/AutoInt) | `torch` | |
+19 | RecSys'19 | [FiBiNET](./model_zoo/FiBiNET) | [FiBiNET: Combining Feature
+Importance and Bilinear feature Interaction for Click-Through Rate Prediction]
+(https://arxiv.org/abs/1905.09433) :triangular_flag_on_post:**Sina Weibo** | [:
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/FiBiNET) | `torch` | | 20 | WWW'19 | [FGCNN](./
+model_zoo/FGCNN) | [Feature Generation by Convolutional Neural Network for
+Click-Through Rate Prediction](https://arxiv.org/abs/1904.04447) :
+triangular_flag_on_post:**Huawei** | [:arrow_upper_right:](https://github.com/
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FGCNN) | `torch` | | 21
+| AAAI'19 | [HFM/HFM+](./model_zoo/HFM) | [Holographic Factorization Machines
+for Recommendation](https://ojs.aaai.org//index.php/AAAI/article/view/4448) |
+[:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/HFM) | `torch` | | 22 | Arxiv'19 | [DLRM](./
+model_zoo/DLRM) | [Deep Learning Recommendation Model for Personalization and
+Recommendation Systems](https://arxiv.org/abs/1906.00091) :
+triangular_flag_on_post:**Facebook** | [:arrow_upper_right:](https://
+github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DLRM) |
+`torch` | | 23 | NeuralNetworks'20 | [ONN](./model_zoo/ONN) | [Operation-aware
+Neural Networks for User Response Prediction](https://arxiv.org/pdf/1904.12579)
+| [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/ONN) | `torch` | | 24 | AAAI'20 | [AFN/AFN+](./
+model_zoo/AFN) | [Adaptive Factorization Network: Learning Adaptive-Order
+Feature Interactions](https://ojs.aaai.org/index.php/AAAI/article/view/5768) |
+[:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/AFN) | `torch` | | 25 | AAAI'20 | [LorentzFM](./
+model_zoo/LorentzFM) | [Learning Feature Interactions with Lorentzian
+Factorization](https://arxiv.org/abs/1911.09821) :triangular_flag_on_post:
+**eBay** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
+main/ctr_prediction/benchmarks/LorentzFM) | `torch` | | 26 | WSDM'20 |
+[InterHAt](./model_zoo/InterHAt) | [Interpretable Click-through Rate Prediction
+through Hierarchical Attention](https://dl.acm.org/doi/10.1145/3336191.3371785)
+:triangular_flag_on_post:**NEC Labs, Google** | [:arrow_upper_right:](https://
+github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/InterHAt) |
+`torch` | | 27 | DLP-KDD'20 | [FLEN](./model_zoo/FLEN) | [FLEN: Leveraging
+Field for Scalable CTR Prediction](https://arxiv.org/abs/1911.04690) :
+triangular_flag_on_post:**Tencent** | [:arrow_upper_right:](https://github.com/
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FLEN) | `torch` | | 28 |
+CIKM'20 | [DeepIM](./model_zoo/DeepIM) | [Deep Interaction Machine: A Simple
+but Effective Model for High-order Feature Interactions](https://dl.acm.org/
+doi/abs/10.1145/3340531.3412077) :triangular_flag_on_post:**Alibaba, RealAI** |
+[:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
 ctr_prediction/benchmarks/DeepIM) | `torch` | | 29 | WWW'21 | [FmFM](./
 model_zoo/FmFM) | [FM^2: Field-matrixed Factorization Machines for Recommender
 Systems](https://arxiv.org/abs/2102.12994) :triangular_flag_on_post:**Yahoo** |
-[:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
+[:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
 ctr_prediction/benchmarks/FmFM) | `torch` | | 30 | WWW'21 | [DCN-V2](./
 model_zoo/DCNv2) | [DCN V2: Improved Deep & Cross Network and Practical Lessons
 for Web-scale Learning to Rank Systems](https://arxiv.org/abs/2008.13535) :
 triangular_flag_on_post:**Google** | [:arrow_upper_right:](https://github.com/
-openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DCNv2) | `torch` | |
-31 | CIKM'21 | [DESTINE](./model_zoo/DESTINE) | [Disentangled Self-Attentive
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DCNv2) | `torch` | | 31
+| CIKM'21 | [DESTINE](./model_zoo/DESTINE) | [Disentangled Self-Attentive
 Neural Networks for Click-Through Rate Prediction](https://arxiv.org/abs/
 2101.03654) :triangular_flag_on_post:**Alibaba** | [:arrow_upper_right:](https:
-//github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DESTINE)
-| `torch` | | 32 | CIKM'21 | [EDCN](./model_zoo/EDCN) | [Enhancing Explicit and
+//github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DESTINE) |
+`torch` | | 32 | CIKM'21 | [EDCN](./model_zoo/EDCN) | [Enhancing Explicit and
 Implicit Feature Interactions via Information Sharing for Parallel Deep CTR
 Models](https://dlp-kdd.github.io/assets/pdf/DLP-KDD_2021_paper_12.pdf) :
 triangular_flag_on_post:**Huawei** | [:arrow_upper_right:](https://github.com/
-openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/EDCN) | `torch` | | 33
-| DLP-KDD'21 | [MaskNet](./model_zoo/MaskNet) | [MaskNet: Introducing Feature-
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/EDCN) | `torch` | | 33 |
+DLP-KDD'21 | [MaskNet](./model_zoo/MaskNet) | [MaskNet: Introducing Feature-
 Wise Multiplication to CTR Ranking Models by Instance-Guided Mask](https://
 arxiv.org/abs/2102.07619) :triangular_flag_on_post:**Sina Weibo** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
 ctr_prediction/benchmarks/MaskNet) | `torch` | | 34 | SIGIR'21 | [SAM](./
 model_zoo/SAM) | [Looking at CTR Prediction Again: Is Attention All You Need?]
 (https://arxiv.org/abs/2105.05563) :triangular_flag_on_post:**BOSS Zhipin** |
-[:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
+[:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
 ctr_prediction/benchmarks/SAM) | `torch` | | 35 | KDD'21 | [AOANet](./
 model_zoo/AOANet) | [Architecture and Operation Adaptive Network for Online
 Recommendations](https://dl.acm.org/doi/10.1145/3447548.3467133) :
 triangular_flag_on_post:**Didi Chuxing** | [:arrow_upper_right:](https://
-github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/AOANet) |
-`torch` | | 36 | Blog'21 | [PPNet](./model_zoo/PPNet) | [Parameter Personalized
-Net](https://www.jiqizhixin.com/articles/2021-02-03-6) :
-triangular_flag_on_post:**KuaiShou** | | `torch` | | 37 | AAAI'23 | [FinalMLP]
-(./model_zoo/FinalMLP) | FinalMLP: An Enhanced Two-Stream MLP Model for CTR
-PredictionÂ :triangular_flag_on_post:**Huawei** | | `torch` | | | | | :
-point_down:**User Behavior Modeling** | | | | 38 | KDD'18 | [DIN](./model_zoo/
-DIN) | [Deep Interest Network for Click-Through Rate Prediction](https://
-www.kdd.org/kdd2018/accepted-papers/view/deep-interest-network-for-click-
-through-rate-prediction) :triangular_flag_on_post:**Alibaba** | | `torch` | |
-39 | AAAI'19 | [DIEN](./model_zoo/DIEN) | [Deep Interest Evolution Network for
-Click-Through Rate Prediction](https://arxiv.org/abs/1809.03672)Â :
-triangular_flag_on_post:**Alibaba** | | `torch` | | 40 | DLP-KDD'19 | [BST](./
-model_zoo/BST) | [Behavior Sequence Transformer for E-commerce Recommendation
-in Alibaba](https://arxiv.org/abs/1905.06874)Â :triangular_flag_on_post:
-**Alibaba** | | `torch` | | 41 | CIKM'20 | [DMIN](./model_zoo/DMIN) | [Deep
-Multi-Interest Network for Click-through Rate Prediction](https://dl.acm.org/
-doi/10.1145/3340531.3412092)Â :triangular_flag_on_post:**Alibaba** | | `torch`
-| | 42 | AAAI'20 | [DMR](./model_zoo/DMR) | [Deep Match to Rank Model for
-Personalized Click-Through Rate Prediction](https://ojs.aaai.org/index.php/
-AAAI/article/view/5346)Â :triangular_flag_on_post:**Alibaba** | | `torch` | |
-43 | Arxiv'21 | [ETA](./model_zoo/ETA) | [End-to-End User Behavior Retrieval in
-Click-Through RatePrediction Model](https://arxiv.org/abs/2108.04468)Â :
+github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/AOANet) |
+`torch` | | 36 | AAAI'23 | [FinalMLP](./model_zoo/FinalMLP) | [FinalMLP: An
+Enhanced Two-Stream MLP Model for CTR Prediction](https://arxiv.org/abs/
+2304.00902)Â :triangular_flag_on_post:**Huawei** | [:arrow_upper_right:](https:
+//github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FinalMLP) |
+`torch` | | 37 | SIGIR'23 | [FINAL](./model_zoo/FINAL) | FINAL: Factorized
+Interaction Layer for CTR PredictionÂ :triangular_flag_on_post:**Huawei** | [:
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/FINAL) | `torch` | | | | | :point_down:**User
+Behavior Modeling** | | | | 38 | KDD'18 | [DIN](./model_zoo/DIN) | [Deep
+Interest Network for Click-Through Rate Prediction](https://www.kdd.org/
+kdd2018/accepted-papers/view/deep-interest-network-for-click-through-rate-
+prediction) :triangular_flag_on_post:**Alibaba** | [:arrow_upper_right:](https:
+//github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DIN) |
+`torch` | | 39 | AAAI'19 | [DIEN](./model_zoo/DIEN) | [Deep Interest Evolution
+Network for Click-Through Rate Prediction](https://arxiv.org/abs/1809.03672)Â :
+triangular_flag_on_post:**Alibaba** | [:arrow_upper_right:](https://github.com/
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DIEN) | `torch` | | 40 |
+DLP-KDD'19 | [BST](./model_zoo/BST) | [Behavior Sequence Transformer for E-
+commerce Recommendation in Alibaba](https://arxiv.org/abs/1905.06874)Â :
+triangular_flag_on_post:**Alibaba** | [:arrow_upper_right:](https://github.com/
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/BST) | `torch` | | 41 |
+CIKM'20 | [DMIN](./model_zoo/DMIN) | [Deep Multi-Interest Network for Click-
+through Rate Prediction](https://dl.acm.org/doi/10.1145/3340531.3412092)Â :
+triangular_flag_on_post:**Alibaba** | | `torch` | | 42 | AAAI'20 | [DMR](./
+model_zoo/DMR) | [Deep Match to Rank Model for Personalized Click-Through Rate
+Prediction](https://ojs.aaai.org/index.php/AAAI/article/view/5346)Â :
+triangular_flag_on_post:**Alibaba** | | `torch` | | 43 | Arxiv'21 | [ETA](./
+model_zoo/ETA) | [End-to-End User Behavior Retrieval in Click-Through
+RatePrediction Model](https://arxiv.org/abs/2108.04468)Â :
 triangular_flag_on_post:**Alibaba** | | `torch` | | 44 | CIKM'22 | [SDIM](./
 model_zoo/SDIM) | [Sampling Is All You Need on Modeling Long-Term User
 Behaviors for CTR Prediction](https://arxiv.org/abs/2205.10249)Â :
-triangular_flag_on_post:**Meituan** | | `torch` | + :point_right: See [reusable
-dataset splits for CTR prediction](https://github.com/openbenchmark/BARS/blob/
-master/ctr_prediction/datasets). + :point_right: See [benchmarking
-configurations and steps](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks). + :point_right: See [the BARS benchmark website]
-(https://openbenchmark.github.io/ctr-prediction). ## Dependencies FuxiCTR has
-the following dependency requirements. + python 3.6+ + pytorch 1.10+ (required
-only for torch models) + tensorflow 2.1+ (required only for tf models) Other
-packages can be installed via `pip install -r requirements.txt`. ## Quick Start
-1. Run the demo examples Examples are provided in the demo directory to show
-some basic usage of FuxiCTR. Users can run the examples for quick start and to
-understand the workflow. ``` cd demo python example1_build_dataset_to_h5.py
-python example2_DeepFM_with_h5_input.py ``` 2. Run an existing model Users can
-easily run each model in the model zoo following the commands below, which is a
-demo for running DCN. In addition, users can modify the dataset config and
-model config files to run on their own datasets or with new hyper-parameters.
-More details can be found in the [readme file](./model_zoo/DCN/DCN_torch/
-README.md). ``` cd model_zoo/DCN/DCN_torch python run_expid.py --expid DCN_test
---gpu 0 ``` 3. Implement a new model The FuxiCTR code structure is modularized,
-so that every part can be overwritten by users according to their needs. In
-many cases, only the model class needs to be implemented for a new customized
-model. If data preprocessing or data loader is not directly applicable, one can
-also overwrite a new one through the [core APIs](https://www.processon.com/
-view/link/63cfcfab4e30670eac4a81c7). A complete example can be found at
-[model_zoo/FinalMLP](./model_zoo/FinalMLP/), which implements our new model
-FinalMLP that has been recently published in AAAI 2023. Some other examples are
-also available in the model zoo. ## Citation *:bell: If you find our code or
-benchmarks helpful in your research, please kindly cite the following papers.*
-> Jieming Zhu, Jinyang Liu, Shuai Yang, Qi Zhang, Xiuqiang He. [Open
+triangular_flag_on_post:**Meituan** | | `torch` | | | | | :point_down:**Multi-
+Task Models** | | | | 45 | MachineLearn'97 | [SharedBottom](./model_zoo/
+multitask/SharedBottom) | [Multitask Learning](https://link.springer.com/
+article/10.1023/A:1007379606734) | | `torch` | | 46 | KDD'18 | [MMoE](./
+model_zoo/multitask/MMOE) | [Modeling Task Relationships in Multi-task Learning
+with Multi-Gate Mixture-of-Experts](https://dl.acm.org/doi/pdf/10.1145/
+3219819.3220007) :triangular_flag_on_post:**Google** | | `torch` | | | | | :
+point_down:**Multi-Domain Models** | | | | 47 | Arxiv'23 | [PPNet](./model_zoo/
+PPNet)/PEPNet | [PEPNet: Parameter and Embedding Personalized Network for
+Infusing with Personalized Prior Information](https://arxiv.org/abs/2302.01115)
+:triangular_flag_on_post:**KuaiShou** | | `torch` | + :point_right: See
+[reusable dataset splits for CTR prediction](https://openbenchmark.github.io/
+BARS/datasets/README.html). + :point_right: See [benchmarking configurations
+and steps](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/
+benchmarks). + :point_right: See [the BARS benchmark leaderboard](https://
+openbenchmark.github.io/BARS/ctr_prediction/leaderboard/README.html#). ##
+Dependencies FuxiCTR has the following dependency requirements. + python 3.6+ +
+pytorch 1.0/1.10+ (required only for torch models) + tensorflow 2.1+ (required
+only for tf models) Other packages can be installed via `pip install -
+r requirements.txt`. ## Quick Start 1. Run the demo examples Examples are
+provided in the demo directory to show some basic usage of FuxiCTR. Users can
+run the examples for quick start and to understand the workflow. ``` cd demo
+python example1_build_dataset_to_h5.py python example2_DeepFM_with_h5_input.py
+``` 2. Run an existing model Users can easily run each model in the model zoo
+following the commands below, which is a demo for running DCN. In addition,
+users can modify the dataset config and model config files to run on their own
+datasets or with new hyper-parameters. More details can be found in the [readme
+file](./model_zoo/DCN/DCN_torch/README.md). ``` cd model_zoo/DCN/DCN_torch
+python run_expid.py --expid DCN_test --gpu 0 # Change `MODEL` according to the
+target model name cd model_zoo/MODEL_PATH python run_expid.py --expid
+MODEL_test --gpu 0 ``` 3. Implement a new model The FuxiCTR code structure is
+modularized, so that every part can be overwritten by users according to their
+needs. In many cases, only the model class needs to be implemented for a new
+customized model. If data preprocessing or data loader is not directly
+applicable, one can also overwrite a new one through the [core APIs](https://
+www.processon.com/view/link/63cfcfab4e30670eac4a81c7). We show a concrete
+example which implements our new model [FinalMLP](https://github.com/xue-pai/
+FinalMLP) that has been recently published in AAAI 2023. More examples can be
+found in the [model zoo](./model_zoo/). ## Citation *:bell: If you find our
+code or benchmarks helpful in your research, please kindly cite the following
+papers.* > Jieming Zhu, Jinyang Liu, Shuai Yang, Qi Zhang, Xiuqiang He. [Open
 Benchmarking for Click-Through Rate Prediction](https://arxiv.org/abs/
 2009.05794). *The 30th ACM International Conference on Information and
 Knowledge Management (CIKM)*, 2021. [[Bibtex](https://dblp.org/rec/conf/cikm/
 ZhuLYZH21.html?view=bibtex)] > Jieming Zhu, Quanyu Dai, Liangcai Su, Rong Ma,
 Jinyang Liu, Guohao Cai, Xi Xiao, Rui Zhang. [BARS: Towards Open Benchmarking
 for Recommender Systems](https://arxiv.org/abs/2205.09626). *The 45th
 International ACM SIGIR Conference on Research and Development in Information
```

### Comparing `fuxictr-2.0.1/README.md` & `fuxictr-2.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -32,70 +32,77 @@
 
 
 ## Model Zoo
 
 | No  | Publication       | Model                                    | Paper                                                                                                                                                                                                           | Benchmark                                                                                                       | Version       |
 |:---:|:-----------------:|:----------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |:---------------------------------------------------------------------------------------------------------------:|:-------------:|
 |     |                   |                                          | :point_down:**Feature Interaction Models**                                                                                                                                                                      |                                                                                                                 |               |
-| 1   | WWW'07            | [LR](./model_zoo/LR)                     | [Predicting Clicks: Estimating the Click-Through Rate for New Ads](https://dl.acm.org/citation.cfm?id=1242643) :triangular_flag_on_post:**Microsoft**                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/LR)           | `torch`       |
-| 2   | ICDM'10           | [FM](./model_zoo/FM)                     | [Factorization Machines](https://www.csie.ntu.edu.tw/~b97053/paper/Rendle2010FM.pdf)                                                                                                                            | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/FM)           | `torch`       |
-| 3   | CIKM'13           | [DSSM](./model_zoo/DSSM)                 | [Learning Deep Structured Semantic Models  for Web Search using Clickthrough Data ](https://posenhuang.github.io/papers/cikm2013_DSSM_fullversion.pdf) :triangular_flag_on_post:**Microsoft**                   | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DSSM)         | `torch`       |
-| 4   | CIKM'15           | [CCPM](./model_zoo/CCPM)                 | [A Convolutional Click Prediction Model](http://www.escience.cn/system/download/73676)                                                                                                                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/CCPM)         | `torch`       |
-| 5   | RecSys'16         | [FFM](./model_zoo/FFM)                   | [Field-aware Factorization Machines for CTR Prediction](https://dl.acm.org/citation.cfm?id=2959134) :triangular_flag_on_post:**Criteo**                                                                         | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/FFM)          | `torch`       |
-| 6   | RecSys'16         | [YoutubeDNN](./model_zoo/DNN)            | [Deep Neural Networks for YouTube Recommendations](http://art.yale.edu/file_columns/0001/1132/covington.pdf) :triangular_flag_on_post:**Google**                                                                | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DNN)          | `torch`, `tf` |
-| 7   | DLRS'16           | [Wide&Deep](./model_zoo/WideDeep)        | [Wide & Deep Learning for Recommender Systems](https://arxiv.org/pdf/1606.07792.pdf) :triangular_flag_on_post:**Google**                                                                                        | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/WideDeep)     | `torch`, `tf` |
-| 8   | ICDM'16           | [IPNN](./model_zoo/PNN)                  | [Product-based Neural Networks for User Response Prediction](https://arxiv.org/pdf/1611.00144.pdf)                                                                                                              | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/IPNN)         | `torch`       |
-| 9   | KDD'16            | [DeepCrossing](./model_zoo/DeepCrossing) | [Deep Crossing: Web-Scale Modeling without Manually Crafted Combinatorial Features](https://www.kdd.org/kdd2016/papers/files/adf0975-shanA.pdf) :triangular_flag_on_post:**Microsoft**                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DeepCrossing) | `torch`       |
-| 10  | NIPS'16           | [HOFM](./model_zoo/HOFM)                 | [Higher-Order Factorization Machines](https://papers.nips.cc/paper/6144-higher-order-factorization-machines.pdf)                                                                                                | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/HOFM)         | `torch`       |
-| 11  | IJCAI'17          | [DeepFM](./model_zoo/DeepFM)             | [DeepFM: A Factorization-Machine based Neural Network for CTR Prediction](https://arxiv.org/abs/1703.04247) :triangular_flag_on_post:**Huawei**                                                                 | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DeepFM)       | `torch`, `tf` |
-| 12  | SIGIR'17          | [NFM](./model_zoo/NFM)                   | [Neural Factorization Machines for Sparse Predictive Analytics](https://dl.acm.org/citation.cfm?id=3080777)                                                                                                     | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/NFM)          | `torch`       |
-| 13  | IJCAI'17          | [AFM](./model_zoo/AFM)                   | [Attentional Factorization Machines: Learning the Weight of Feature Interactions via Attention Networks](http://www.ijcai.org/proceedings/2017/0435.pdf)                                                        | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/AFM)          | `torch`       |
-| 14  | ADKDD'17          | [DCN](./model_zoo/DCN)                   | [Deep & Cross Network for Ad Click Predictions](https://arxiv.org/abs/1708.05123) :triangular_flag_on_post:**Google**                                                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DCN)          | `torch`, `tf` |
-| 15  | WWW'18            | [FwFM](./model_zoo/FwFM)                 | [Field-weighted Factorization Machines for Click-Through Rate Prediction in Display Advertising](https://arxiv.org/pdf/1806.03514.pdf) :triangular_flag_on_post:**Oath, TouchPal, LinkedIn, Alibaba**           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/FwFM)         | `torch`       |
-| 16  | KDD'18            | [xDeepFM](./model_zoo/xDeepFM)           | [xDeepFM: Combining Explicit and Implicit Feature Interactions for Recommender Systems](https://arxiv.org/pdf/1803.05170.pdf) :triangular_flag_on_post:**Microsoft**                                            | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/xDeepFM)      | `torch`       |
-| 17  | CIKM'19           | [FiGNN](./model_zoo/FiGNN)               | [FiGNN: Modeling Feature Interactions via Graph Neural Networks for CTR Prediction](https://arxiv.org/abs/1910.05552)                                                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/FiGNN)        | `torch`       |
-| 18  | CIKM'19           | [AutoInt/AutoInt+](./model_zoo/AutoInt)  | [AutoInt: Automatic Feature Interaction Learning via Self-Attentive Neural Networks](https://arxiv.org/abs/1810.11921)                                                                                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/AutoInt)      | `torch`       |
-| 19  | RecSys'19         | [FiBiNET](./model_zoo/FiBiNET)           | [FiBiNET: Combining Feature Importance and Bilinear feature Interaction for Click-Through Rate Prediction](https://arxiv.org/abs/1905.09433) :triangular_flag_on_post:**Sina Weibo**                            | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/FiBiNET)      | `torch`       |
-| 20  | WWW'19            | [FGCNN](./model_zoo/FGCNN)               | [Feature Generation by Convolutional Neural Network for Click-Through Rate Prediction](https://arxiv.org/abs/1904.04447) :triangular_flag_on_post:**Huawei**                                                    | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/FGCNN)        | `torch`       |
-| 21  | AAAI'19           | [HFM/HFM+](./model_zoo/HFM)              | [Holographic Factorization Machines for Recommendation](https://ojs.aaai.org//index.php/AAAI/article/view/4448)                                                                                                 | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/HFM)          | `torch`       |
-| 22  | Arxiv'19          | [DLRM](./model_zoo/DLRM)                 | [Deep Learning Recommendation Model for Personalization and Recommendation Systems](https://arxiv.org/abs/1906.00091) :triangular_flag_on_post:**Facebook**                                                     | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DLRM)         | `torch`       |
-| 23  | NeuralNetworks'20 | [ONN](./model_zoo/ONN)                   | [Operation-aware Neural Networks for User Response Prediction](https://arxiv.org/pdf/1904.12579)                                                                                                                | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/ONN)          | `torch`       |
-| 24  | AAAI'20           | [AFN/AFN+](./model_zoo/AFN)              | [Adaptive Factorization Network: Learning Adaptive-Order Feature Interactions](https://ojs.aaai.org/index.php/AAAI/article/view/5768)                                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/AFN)          | `torch`       |
-| 25  | AAAI'20           | [LorentzFM](./model_zoo/LorentzFM)       | [Learning Feature Interactions with Lorentzian Factorization](https://arxiv.org/abs/1911.09821) :triangular_flag_on_post:**eBay**                                                                               | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/LorentzFM)    | `torch`       |
-| 26  | WSDM'20           | [InterHAt](./model_zoo/InterHAt)         | [Interpretable Click-through Rate Prediction through Hierarchical Attention](https://dl.acm.org/doi/10.1145/3336191.3371785) :triangular_flag_on_post:**NEC Labs, Google**                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/InterHAt)     | `torch`       |
-| 27  | DLP-KDD'20        | [FLEN](./model_zoo/FLEN)                 | [FLEN: Leveraging Field for Scalable CTR Prediction](https://arxiv.org/abs/1911.04690) :triangular_flag_on_post:**Tencent**                                                                                     | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/FLEN)         | `torch`       |
-| 28  | CIKM'20           | [DeepIM](./model_zoo/DeepIM)             | [Deep Interaction Machine: A Simple but Effective Model for High-order Feature Interactions](https://dl.acm.org/doi/abs/10.1145/3340531.3412077) :triangular_flag_on_post:**Alibaba, RealAI**                   | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DeepIM)       | `torch`       |
-| 29  | WWW'21            | [FmFM](./model_zoo/FmFM)                 | [FM^2: Field-matrixed Factorization Machines for Recommender Systems](https://arxiv.org/abs/2102.12994) :triangular_flag_on_post:**Yahoo**                                                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/FmFM)         | `torch`       |
-| 30  | WWW'21            | [DCN-V2](./model_zoo/DCNv2)              | [DCN V2: Improved Deep & Cross Network and Practical Lessons for Web-scale Learning to Rank Systems](https://arxiv.org/abs/2008.13535) :triangular_flag_on_post:**Google**                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DCNv2)        | `torch`       |
-| 31  | CIKM'21           | [DESTINE](./model_zoo/DESTINE)           | [Disentangled Self-Attentive Neural Networks for Click-Through Rate Prediction](https://arxiv.org/abs/2101.03654) :triangular_flag_on_post:**Alibaba**                                                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DESTINE)      | `torch`       |
-| 32  | CIKM'21           | [EDCN](./model_zoo/EDCN)                 | [Enhancing Explicit and Implicit Feature Interactions via Information Sharing for Parallel Deep CTR Models](https://dlp-kdd.github.io/assets/pdf/DLP-KDD_2021_paper_12.pdf) :triangular_flag_on_post:**Huawei** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/EDCN)         | `torch`       |
-| 33  | DLP-KDD'21        | [MaskNet](./model_zoo/MaskNet)           | [MaskNet: Introducing Feature-Wise Multiplication to CTR Ranking Models by Instance-Guided Mask](https://arxiv.org/abs/2102.07619) :triangular_flag_on_post:**Sina Weibo**                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/MaskNet)      | `torch`       |
-| 34  | SIGIR'21          | [SAM](./model_zoo/SAM)                   | [Looking at CTR Prediction Again: Is Attention All You Need?](https://arxiv.org/abs/2105.05563) :triangular_flag_on_post:**BOSS Zhipin**                                                                        | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/SAM)          | `torch`       |
-| 35  | KDD'21            | [AOANet](./model_zoo/AOANet)             | [Architecture and Operation Adaptive Network for Online Recommendations](https://dl.acm.org/doi/10.1145/3447548.3467133) :triangular_flag_on_post:**Didi Chuxing**                                              | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/AOANet)       | `torch`       |
-| 36  | Blog'21           | [PPNet](./model_zoo/PPNet)               | [Parameter Personalized Net](https://www.jiqizhixin.com/articles/2021-02-03-6) :triangular_flag_on_post:**KuaiShou**                                                                                            |                                                                                                                 | `torch`       |
-| 37  | AAAI'23           | [FinalMLP](./model_zoo/FinalMLP)         | FinalMLP: An Enhanced Two-Stream MLP Model for CTR Prediction :triangular_flag_on_post:**Huawei**                                                                                                               |                                                                                                                 | `torch`       |
+| 1   | WWW'07            | [LR](./model_zoo/LR)                     | [Predicting Clicks: Estimating the Click-Through Rate for New Ads](https://dl.acm.org/citation.cfm?id=1242643) :triangular_flag_on_post:**Microsoft**                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/LR)           | `torch`       |
+| 2   | ICDM'10           | [FM](./model_zoo/FM)                     | [Factorization Machines](https://www.csie.ntu.edu.tw/~b97053/paper/Rendle2010FM.pdf)                                                                                                                            | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FM)           | `torch`       |
+| 3   | CIKM'13           | [DSSM](./model_zoo/DSSM)                 | [Learning Deep Structured Semantic Models  for Web Search using Clickthrough Data ](https://posenhuang.github.io/papers/cikm2013_DSSM_fullversion.pdf) :triangular_flag_on_post:**Microsoft**                   | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DSSM)         | `torch`       |
+| 4   | CIKM'15           | [CCPM](./model_zoo/CCPM)                 | [A Convolutional Click Prediction Model](http://www.escience.cn/system/download/73676)                                                                                                                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/CCPM)         | `torch`       |
+| 5   | RecSys'16         | [FFM](./model_zoo/FFM)                   | [Field-aware Factorization Machines for CTR Prediction](https://dl.acm.org/citation.cfm?id=2959134) :triangular_flag_on_post:**Criteo**                                                                         | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FFM)          | `torch`       |
+| 6   | RecSys'16         | [DNN](./model_zoo/DNN)            | [Deep Neural Networks for YouTube Recommendations](http://art.yale.edu/file_columns/0001/1132/covington.pdf) :triangular_flag_on_post:**Google**                                                                | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DNN)          | `torch`, `tf` |
+| 7   | DLRS'16           | [Wide&Deep](./model_zoo/WideDeep)        | [Wide & Deep Learning for Recommender Systems](https://arxiv.org/pdf/1606.07792.pdf) :triangular_flag_on_post:**Google**                                                                                        | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/WideDeep)     | `torch`, `tf` |
+| 8   | ICDM'16           | [IPNN](./model_zoo/PNN)                  | [Product-based Neural Networks for User Response Prediction](https://arxiv.org/pdf/1611.00144.pdf)                                                                                                              | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/IPNN)         | `torch`       |
+| 9   | KDD'16            | [DeepCrossing](./model_zoo/DeepCrossing) | [Deep Crossing: Web-Scale Modeling without Manually Crafted Combinatorial Features](https://www.kdd.org/kdd2016/papers/files/adf0975-shanA.pdf) :triangular_flag_on_post:**Microsoft**                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DeepCrossing) | `torch`       |
+| 10  | NIPS'16           | [HOFM](./model_zoo/HOFM)                 | [Higher-Order Factorization Machines](https://papers.nips.cc/paper/6144-higher-order-factorization-machines.pdf)                                                                                                | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/HOFM)         | `torch`       |
+| 11  | IJCAI'17          | [DeepFM](./model_zoo/DeepFM)             | [DeepFM: A Factorization-Machine based Neural Network for CTR Prediction](https://arxiv.org/abs/1703.04247) :triangular_flag_on_post:**Huawei**                                                                 | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DeepFM)       | `torch`, `tf` |
+| 12  | SIGIR'17          | [NFM](./model_zoo/NFM)                   | [Neural Factorization Machines for Sparse Predictive Analytics](https://dl.acm.org/citation.cfm?id=3080777)                                                                                                     | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/NFM)          | `torch`       |
+| 13  | IJCAI'17          | [AFM](./model_zoo/AFM)                   | [Attentional Factorization Machines: Learning the Weight of Feature Interactions via Attention Networks](http://www.ijcai.org/proceedings/2017/0435.pdf)                                                        | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/AFM)          | `torch`       |
+| 14  | ADKDD'17          | [DCN](./model_zoo/DCN)                   | [Deep & Cross Network for Ad Click Predictions](https://arxiv.org/abs/1708.05123) :triangular_flag_on_post:**Google**                                                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DCN)          | `torch`, `tf` |
+| 15  | WWW'18            | [FwFM](./model_zoo/FwFM)                 | [Field-weighted Factorization Machines for Click-Through Rate Prediction in Display Advertising](https://arxiv.org/pdf/1806.03514.pdf) :triangular_flag_on_post:**Oath, TouchPal, LinkedIn, Alibaba**           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FwFM)         | `torch`       |
+| 16  | KDD'18            | [xDeepFM](./model_zoo/xDeepFM)           | [xDeepFM: Combining Explicit and Implicit Feature Interactions for Recommender Systems](https://arxiv.org/pdf/1803.05170.pdf) :triangular_flag_on_post:**Microsoft**                                            | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/xDeepFM)      | `torch`       |
+| 17  | CIKM'19           | [FiGNN](./model_zoo/FiGNN)               | [FiGNN: Modeling Feature Interactions via Graph Neural Networks for CTR Prediction](https://arxiv.org/abs/1910.05552)                                                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FiGNN)        | `torch`       |
+| 18  | CIKM'19           | [AutoInt/AutoInt+](./model_zoo/AutoInt)  | [AutoInt: Automatic Feature Interaction Learning via Self-Attentive Neural Networks](https://arxiv.org/abs/1810.11921)                                                                                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/AutoInt)      | `torch`       |
+| 19  | RecSys'19         | [FiBiNET](./model_zoo/FiBiNET)           | [FiBiNET: Combining Feature Importance and Bilinear feature Interaction for Click-Through Rate Prediction](https://arxiv.org/abs/1905.09433) :triangular_flag_on_post:**Sina Weibo**                            | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FiBiNET)      | `torch`       |
+| 20  | WWW'19            | [FGCNN](./model_zoo/FGCNN)               | [Feature Generation by Convolutional Neural Network for Click-Through Rate Prediction](https://arxiv.org/abs/1904.04447) :triangular_flag_on_post:**Huawei**                                                    | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FGCNN)        | `torch`       |
+| 21  | AAAI'19           | [HFM/HFM+](./model_zoo/HFM)              | [Holographic Factorization Machines for Recommendation](https://ojs.aaai.org//index.php/AAAI/article/view/4448)                                                                                                 | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/HFM)          | `torch`       |
+| 22  | Arxiv'19          | [DLRM](./model_zoo/DLRM)                 | [Deep Learning Recommendation Model for Personalization and Recommendation Systems](https://arxiv.org/abs/1906.00091) :triangular_flag_on_post:**Facebook**                                                     | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DLRM)         | `torch`       |
+| 23  | NeuralNetworks'20 | [ONN](./model_zoo/ONN)                   | [Operation-aware Neural Networks for User Response Prediction](https://arxiv.org/pdf/1904.12579)                                                                                                                | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/ONN)          | `torch`       |
+| 24  | AAAI'20           | [AFN/AFN+](./model_zoo/AFN)              | [Adaptive Factorization Network: Learning Adaptive-Order Feature Interactions](https://ojs.aaai.org/index.php/AAAI/article/view/5768)                                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/AFN)          | `torch`       |
+| 25  | AAAI'20           | [LorentzFM](./model_zoo/LorentzFM)       | [Learning Feature Interactions with Lorentzian Factorization](https://arxiv.org/abs/1911.09821) :triangular_flag_on_post:**eBay**                                                                               | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/LorentzFM)    | `torch`       |
+| 26  | WSDM'20           | [InterHAt](./model_zoo/InterHAt)         | [Interpretable Click-through Rate Prediction through Hierarchical Attention](https://dl.acm.org/doi/10.1145/3336191.3371785) :triangular_flag_on_post:**NEC Labs, Google**                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/InterHAt)     | `torch`       |
+| 27  | DLP-KDD'20        | [FLEN](./model_zoo/FLEN)                 | [FLEN: Leveraging Field for Scalable CTR Prediction](https://arxiv.org/abs/1911.04690) :triangular_flag_on_post:**Tencent**                                                                                     | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FLEN)         | `torch`       |
+| 28  | CIKM'20           | [DeepIM](./model_zoo/DeepIM)             | [Deep Interaction Machine: A Simple but Effective Model for High-order Feature Interactions](https://dl.acm.org/doi/abs/10.1145/3340531.3412077) :triangular_flag_on_post:**Alibaba, RealAI**                   | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DeepIM)       | `torch`       |
+| 29  | WWW'21            | [FmFM](./model_zoo/FmFM)                 | [FM^2: Field-matrixed Factorization Machines for Recommender Systems](https://arxiv.org/abs/2102.12994) :triangular_flag_on_post:**Yahoo**                                                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FmFM)         | `torch`       |
+| 30  | WWW'21            | [DCN-V2](./model_zoo/DCNv2)              | [DCN V2: Improved Deep & Cross Network and Practical Lessons for Web-scale Learning to Rank Systems](https://arxiv.org/abs/2008.13535) :triangular_flag_on_post:**Google**                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DCNv2)        | `torch`       |
+| 31  | CIKM'21           | [DESTINE](./model_zoo/DESTINE)           | [Disentangled Self-Attentive Neural Networks for Click-Through Rate Prediction](https://arxiv.org/abs/2101.03654) :triangular_flag_on_post:**Alibaba**                                                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DESTINE)      | `torch`       |
+| 32  | CIKM'21           | [EDCN](./model_zoo/EDCN)                 | [Enhancing Explicit and Implicit Feature Interactions via Information Sharing for Parallel Deep CTR Models](https://dlp-kdd.github.io/assets/pdf/DLP-KDD_2021_paper_12.pdf) :triangular_flag_on_post:**Huawei** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/EDCN)         | `torch`       |
+| 33  | DLP-KDD'21        | [MaskNet](./model_zoo/MaskNet)           | [MaskNet: Introducing Feature-Wise Multiplication to CTR Ranking Models by Instance-Guided Mask](https://arxiv.org/abs/2102.07619) :triangular_flag_on_post:**Sina Weibo**                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/MaskNet)      | `torch`       |
+| 34  | SIGIR'21          | [SAM](./model_zoo/SAM)                   | [Looking at CTR Prediction Again: Is Attention All You Need?](https://arxiv.org/abs/2105.05563) :triangular_flag_on_post:**BOSS Zhipin**                                                                        | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/SAM)          | `torch`       |
+| 35  | KDD'21            | [AOANet](./model_zoo/AOANet)             | [Architecture and Operation Adaptive Network for Online Recommendations](https://dl.acm.org/doi/10.1145/3447548.3467133) :triangular_flag_on_post:**Didi Chuxing**                                              | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/AOANet)       | `torch`       |
+| 36  | AAAI'23           | [FinalMLP](./model_zoo/FinalMLP)         | [FinalMLP: An Enhanced Two-Stream MLP Model for CTR Prediction](https://arxiv.org/abs/2304.00902) :triangular_flag_on_post:**Huawei**                                                                                                               |     [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FinalMLP)         | `torch`       |
+| 37  | SIGIR'23           | [FINAL](./model_zoo/FINAL)         | FINAL: Factorized Interaction Layer for CTR Prediction :triangular_flag_on_post:**Huawei**                                                                                                               |     [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FINAL)         | `torch`       |
 |     |                   |                                          | :point_down:**User Behavior Modeling**                                                                                                                                                                          |                                                                                                                 |               |
-| 38  | KDD'18            | [DIN](./model_zoo/DIN)                   | [Deep Interest Network for Click-Through Rate Prediction](https://www.kdd.org/kdd2018/accepted-papers/view/deep-interest-network-for-click-through-rate-prediction) :triangular_flag_on_post:**Alibaba**        |                                                                                                                 | `torch`       |
-| 39  | AAAI'19           | [DIEN](./model_zoo/DIEN)                 | [Deep Interest Evolution Network for Click-Through Rate Prediction](https://arxiv.org/abs/1809.03672) :triangular_flag_on_post:**Alibaba**                                                                      |                                                                                                                 | `torch`       |
-| 40  | DLP-KDD'19        | [BST](./model_zoo/BST)                   | [Behavior Sequence Transformer for E-commerce Recommendation in Alibaba](https://arxiv.org/abs/1905.06874) :triangular_flag_on_post:**Alibaba**                                                                 |                                                                                                                 | `torch`       |
+| 38  | KDD'18            | [DIN](./model_zoo/DIN)                   | [Deep Interest Network for Click-Through Rate Prediction](https://www.kdd.org/kdd2018/accepted-papers/view/deep-interest-network-for-click-through-rate-prediction) :triangular_flag_on_post:**Alibaba**        |   [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DIN)       | `torch`       |
+| 39  | AAAI'19           | [DIEN](./model_zoo/DIEN)                 | [Deep Interest Evolution Network for Click-Through Rate Prediction](https://arxiv.org/abs/1809.03672) :triangular_flag_on_post:**Alibaba**                                                                      |   [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DIEN)        | `torch`       |
+| 40  | DLP-KDD'19        | [BST](./model_zoo/BST)                   | [Behavior Sequence Transformer for E-commerce Recommendation in Alibaba](https://arxiv.org/abs/1905.06874) :triangular_flag_on_post:**Alibaba**                                                                 |  [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/BST)     | `torch`       |
 | 41  | CIKM'20           | [DMIN](./model_zoo/DMIN)                 | [Deep Multi-Interest Network for Click-through Rate Prediction](https://dl.acm.org/doi/10.1145/3340531.3412092) :triangular_flag_on_post:**Alibaba**                                                            |                                                                                                                 | `torch`       |
 | 42  | AAAI'20           | [DMR](./model_zoo/DMR)                   | [Deep Match to Rank Model for Personalized Click-Through Rate Prediction](https://ojs.aaai.org/index.php/AAAI/article/view/5346) :triangular_flag_on_post:**Alibaba**                                           |                                                                                                                 | `torch`       |
 | 43  | Arxiv'21          | [ETA](./model_zoo/ETA)                   | [End-to-End User Behavior Retrieval in Click-Through RatePrediction Model](https://arxiv.org/abs/2108.04468) :triangular_flag_on_post:**Alibaba**                                                               |                                                                                                                 | `torch`       |
 | 44  | CIKM'22           | [SDIM](./model_zoo/SDIM)                 | [Sampling Is All You Need on Modeling Long-Term User Behaviors for CTR Prediction](https://arxiv.org/abs/2205.10249) :triangular_flag_on_post:**Meituan**                                                       |                                                                                                                 | `torch`       |
+|     |                   |                                          | :point_down:**Multi-Task Models**                                                                                                                                                                          |                                                                                                                 |               |
+| 45  |     MachineLearn'97      | [SharedBottom](./model_zoo/multitask/SharedBottom)               | [Multitask Learning](https://link.springer.com/article/10.1023/A:1007379606734)                                                                                            |                                                                                                                 | `torch`       |
+| 46  | KDD'18          | [MMoE](./model_zoo/multitask/MMOE)               | [Modeling Task Relationships in Multi-task Learning with Multi-Gate Mixture-of-Experts](https://dl.acm.org/doi/pdf/10.1145/3219819.3220007) :triangular_flag_on_post:**Google**                                                                                            |                                                                                                                 | `torch`       |
+|     |                   |                                          | :point_down:**Multi-Domain Models**                                                                                                                                                                          |                                                                                                                 |               |
+| 47  | Arxiv'23           | [PPNet](./model_zoo/PPNet)/PEPNet              | [PEPNet: Parameter and Embedding Personalized Network for Infusing with Personalized Prior Information](https://arxiv.org/abs/2302.01115) :triangular_flag_on_post:**KuaiShou**                                                                                            |                                                                                                                 | `torch`       |
+
+
++ :point_right: See [reusable dataset splits for CTR prediction](https://openbenchmark.github.io/BARS/datasets/README.html).
++ :point_right: See [benchmarking configurations and steps](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks).
++ :point_right: See [the BARS benchmark leaderboard](https://openbenchmark.github.io/BARS/ctr_prediction/leaderboard/README.html#).
 
-+ :point_right: See [reusable dataset splits for CTR prediction](https://github.com/openbenchmark/BARS/blob/master/ctr_prediction/datasets).
-+ :point_right: See [benchmarking configurations and steps](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks).
-+ :point_right: See [the BARS benchmark website](https://openbenchmark.github.io/ctr-prediction).
 
 ## Dependencies
 
 FuxiCTR has the following dependency requirements. 
 
 + python 3.6+
-+ pytorch 1.10+ (required only for torch models)
++ pytorch 1.0/1.10+ (required only for torch models)
 + tensorflow 2.1+ (required only for tf models)
 
 Other packages can be installed via `pip install -r requirements.txt`.
 
 ## Quick Start
 
 1. Run the demo examples
@@ -111,19 +118,23 @@
 2. Run an existing model
    
     Users can easily run each model in the model zoo following the commands below, which is a demo for running DCN. In addition, users can modify the dataset config and model config files to run on their own datasets or with new hyper-parameters. More details can be found in the [readme file](./model_zoo/DCN/DCN_torch/README.md).
    
    ```
    cd model_zoo/DCN/DCN_torch
    python run_expid.py --expid DCN_test --gpu 0
+
+   # Change `MODEL` according to the target model name
+   cd model_zoo/MODEL_PATH
+   python run_expid.py --expid MODEL_test --gpu 0
    ```
 
 3. Implement a new model
    
-    The FuxiCTR code structure is modularized, so that every part can be overwritten by users according to their needs. In many cases, only the model class needs to be implemented for a new customized model. If data preprocessing or data loader is not directly applicable, one can also overwrite a new one through the [core APIs](https://www.processon.com/view/link/63cfcfab4e30670eac4a81c7). A complete example can be found at [model_zoo/FinalMLP](./model_zoo/FinalMLP/), which implements our new model FinalMLP that has been recently published in AAAI 2023. Some other examples are also available in the model zoo.
+    The FuxiCTR code structure is modularized, so that every part can be overwritten by users according to their needs. In many cases, only the model class needs to be implemented for a new customized model. If data preprocessing or data loader is not directly applicable, one can also overwrite a new one through the [core APIs](https://www.processon.com/view/link/63cfcfab4e30670eac4a81c7). We show a concrete example which implements our new model [FinalMLP](https://github.com/xue-pai/FinalMLP) that has been recently published in AAAI 2023. More examples can be found in the [model zoo](./model_zoo/).
 
 
 ## Citation
 
 *:bell: If you find our code or benchmarks helpful in your research, please kindly cite the following papers.*
 
 > Jieming Zhu, Jinyang Liu, Shuai Yang, Qi Zhang, Xiuqiang He. [Open Benchmarking for Click-Through Rate Prediction](https://arxiv.org/abs/2009.05794). *The 30th ACM International Conference on Information and Knowledge Management (CIKM)*, 2021. [[Bibtex](https://dblp.org/rec/conf/cikm/ZhuLYZH21.html?view=bibtex)]
```

#### html2text {}

```diff
@@ -19,211 +19,229 @@
 -------------------------------------------------------------------------------
 ----------------------------------------------------------------------- |:-----
 -------------------------------------------------------------------------------
 ---------------------------:|:-------------:| | | | | :point_down:**Feature
 Interaction Models** | | | | 1 | WWW'07 | [LR](./model_zoo/LR) | [Predicting
 Clicks: Estimating the Click-Through Rate for New Ads](https://dl.acm.org/
 citation.cfm?id=1242643) :triangular_flag_on_post:**Microsoft** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
 ctr_prediction/benchmarks/LR) | `torch` | | 2 | ICDM'10 | [FM](./model_zoo/FM)
 | [Factorization Machines](https://www.csie.ntu.edu.tw/~b97053/paper/
 Rendle2010FM.pdf) | [:arrow_upper_right:](https://github.com/openbenchmark/
-BARS/tree/master/ctr_prediction/benchmarks/FM) | `torch` | | 3 | CIKM'13 |
-[DSSM](./model_zoo/DSSM) | [Learning Deep Structured Semantic Models for Web
-Search using Clickthrough Data ](https://posenhuang.github.io/papers/
+BARS/tree/main/ctr_prediction/benchmarks/FM) | `torch` | | 3 | CIKM'13 | [DSSM]
+(./model_zoo/DSSM) | [Learning Deep Structured Semantic Models for Web Search
+using Clickthrough Data ](https://posenhuang.github.io/papers/
 cikm2013_DSSM_fullversion.pdf) :triangular_flag_on_post:**Microsoft** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
 ctr_prediction/benchmarks/DSSM) | `torch` | | 4 | CIKM'15 | [CCPM](./model_zoo/
 CCPM) | [A Convolutional Click Prediction Model](http://www.escience.cn/system/
 download/73676) | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/
-tree/master/ctr_prediction/benchmarks/CCPM) | `torch` | | 5 | RecSys'16 | [FFM]
+tree/main/ctr_prediction/benchmarks/CCPM) | `torch` | | 5 | RecSys'16 | [FFM]
 (./model_zoo/FFM) | [Field-aware Factorization Machines for CTR Prediction]
 (https://dl.acm.org/citation.cfm?id=2959134) :triangular_flag_on_post:
 **Criteo** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
-master/ctr_prediction/benchmarks/FFM) | `torch` | | 6 | RecSys'16 |
-[YoutubeDNN](./model_zoo/DNN) | [Deep Neural Networks for YouTube
-Recommendations](http://art.yale.edu/file_columns/0001/1132/covington.pdf) :
-triangular_flag_on_post:**Google** | [:arrow_upper_right:](https://github.com/
-openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DNN) | `torch`, `tf` |
-| 7 | DLRS'16 | [Wide&Deep](./model_zoo/WideDeep) | [Wide & Deep Learning for
-Recommender Systems](https://arxiv.org/pdf/1606.07792.pdf) :
-triangular_flag_on_post:**Google** | [:arrow_upper_right:](https://github.com/
-openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/WideDeep) | `torch`,
-`tf` | | 8 | ICDM'16 | [IPNN](./model_zoo/PNN) | [Product-based Neural Networks
-for User Response Prediction](https://arxiv.org/pdf/1611.00144.pdf) | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/IPNN) | `torch` | | 9 | KDD'16 | [DeepCrossing](./
-model_zoo/DeepCrossing) | [Deep Crossing: Web-Scale Modeling without Manually
-Crafted Combinatorial Features](https://www.kdd.org/kdd2016/papers/files/
-adf0975-shanA.pdf) :triangular_flag_on_post:**Microsoft** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/DeepCrossing) | `torch` | | 10 | NIPS'16 | [HOFM](./
-model_zoo/HOFM) | [Higher-Order Factorization Machines](https://papers.nips.cc/
-paper/6144-higher-order-factorization-machines.pdf) | [:arrow_upper_right:]
-(https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/
-HOFM) | `torch` | | 11 | IJCAI'17 | [DeepFM](./model_zoo/DeepFM) | [DeepFM: A
-Factorization-Machine based Neural Network for CTR Prediction](https://
-arxiv.org/abs/1703.04247) :triangular_flag_on_post:**Huawei** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/DeepFM) | `torch`, `tf` | | 12 | SIGIR'17 | [NFM](./
-model_zoo/NFM) | [Neural Factorization Machines for Sparse Predictive
-Analytics](https://dl.acm.org/citation.cfm?id=3080777) | [:arrow_upper_right:]
-(https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/
-NFM) | `torch` | | 13 | IJCAI'17 | [AFM](./model_zoo/AFM) | [Attentional
-Factorization Machines: Learning the Weight of Feature Interactions via
-Attention Networks](http://www.ijcai.org/proceedings/2017/0435.pdf) | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/AFM) | `torch` | | 14 | ADKDD'17 | [DCN](./model_zoo/
-DCN) | [Deep & Cross Network for Ad Click Predictions](https://arxiv.org/abs/
-1708.05123) :triangular_flag_on_post:**Google** | [:arrow_upper_right:](https:/
-/github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DCN) |
-`torch`, `tf` | | 15 | WWW'18 | [FwFM](./model_zoo/FwFM) | [Field-weighted
-Factorization Machines for Click-Through Rate Prediction in Display
-Advertising](https://arxiv.org/pdf/1806.03514.pdf) :triangular_flag_on_post:
-**Oath, TouchPal, LinkedIn, Alibaba** | [:arrow_upper_right:](https://
-github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/FwFM) |
-`torch` | | 16 | KDD'18 | [xDeepFM](./model_zoo/xDeepFM) | [xDeepFM: Combining
-Explicit and Implicit Feature Interactions for Recommender Systems](https://
-arxiv.org/pdf/1803.05170.pdf) :triangular_flag_on_post:**Microsoft** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/xDeepFM) | `torch` | | 17 | CIKM'19 | [FiGNN](./
-model_zoo/FiGNN) | [FiGNN: Modeling Feature Interactions via Graph Neural
-Networks for CTR Prediction](https://arxiv.org/abs/1910.05552) | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/FiGNN) | `torch` | | 18 | CIKM'19 | [AutoInt/
-AutoInt+](./model_zoo/AutoInt) | [AutoInt: Automatic Feature Interaction
-Learning via Self-Attentive Neural Networks](https://arxiv.org/abs/1810.11921)
-| [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/AutoInt) | `torch` | | 19 | RecSys'19 | [FiBiNET](./
-model_zoo/FiBiNET) | [FiBiNET: Combining Feature Importance and Bilinear
-feature Interaction for Click-Through Rate Prediction](https://arxiv.org/abs/
-1905.09433) :triangular_flag_on_post:**Sina Weibo** | [:arrow_upper_right:]
-(https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/
-FiBiNET) | `torch` | | 20 | WWW'19 | [FGCNN](./model_zoo/FGCNN) | [Feature
-Generation by Convolutional Neural Network for Click-Through Rate Prediction]
-(https://arxiv.org/abs/1904.04447) :triangular_flag_on_post:**Huawei** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/FGCNN) | `torch` | | 21 | AAAI'19 | [HFM/HFM+](./
-model_zoo/HFM) | [Holographic Factorization Machines for Recommendation](https:
-//ojs.aaai.org//index.php/AAAI/article/view/4448) | [:arrow_upper_right:]
-(https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/
-HFM) | `torch` | | 22 | Arxiv'19 | [DLRM](./model_zoo/DLRM) | [Deep Learning
-Recommendation Model for Personalization and Recommendation Systems](https://
-arxiv.org/abs/1906.00091) :triangular_flag_on_post:**Facebook** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/DLRM) | `torch` | | 23 | NeuralNetworks'20 | [ONN](./
-model_zoo/ONN) | [Operation-aware Neural Networks for User Response Prediction]
-(https://arxiv.org/pdf/1904.12579) | [:arrow_upper_right:](https://github.com/
-openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/ONN) | `torch` | | 24
-| AAAI'20 | [AFN/AFN+](./model_zoo/AFN) | [Adaptive Factorization Network:
-Learning Adaptive-Order Feature Interactions](https://ojs.aaai.org/index.php/
-AAAI/article/view/5768) | [:arrow_upper_right:](https://github.com/
-openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/AFN) | `torch` | | 25
-| AAAI'20 | [LorentzFM](./model_zoo/LorentzFM) | [Learning Feature Interactions
-with Lorentzian Factorization](https://arxiv.org/abs/1911.09821) :
-triangular_flag_on_post:**eBay** | [:arrow_upper_right:](https://github.com/
-openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/LorentzFM) | `torch` |
-| 26 | WSDM'20 | [InterHAt](./model_zoo/InterHAt) | [Interpretable Click-
-through Rate Prediction through Hierarchical Attention](https://dl.acm.org/doi/
-10.1145/3336191.3371785) :triangular_flag_on_post:**NEC Labs, Google** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/InterHAt) | `torch` | | 27 | DLP-KDD'20 | [FLEN](./
-model_zoo/FLEN) | [FLEN: Leveraging Field for Scalable CTR Prediction](https://
-arxiv.org/abs/1911.04690) :triangular_flag_on_post:**Tencent** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/FLEN) | `torch` | | 28 | CIKM'20 | [DeepIM](./
-model_zoo/DeepIM) | [Deep Interaction Machine: A Simple but Effective Model for
-High-order Feature Interactions](https://dl.acm.org/doi/abs/10.1145/
-3340531.3412077) :triangular_flag_on_post:**Alibaba, RealAI** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
+main/ctr_prediction/benchmarks/FFM) | `torch` | | 6 | RecSys'16 | [DNN](./
+model_zoo/DNN) | [Deep Neural Networks for YouTube Recommendations](http://
+art.yale.edu/file_columns/0001/1132/covington.pdf) :triangular_flag_on_post:
+**Google** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
+main/ctr_prediction/benchmarks/DNN) | `torch`, `tf` | | 7 | DLRS'16 |
+[Wide&Deep](./model_zoo/WideDeep) | [Wide & Deep Learning for Recommender
+Systems](https://arxiv.org/pdf/1606.07792.pdf) :triangular_flag_on_post:
+**Google** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
+main/ctr_prediction/benchmarks/WideDeep) | `torch`, `tf` | | 8 | ICDM'16 |
+[IPNN](./model_zoo/PNN) | [Product-based Neural Networks for User Response
+Prediction](https://arxiv.org/pdf/1611.00144.pdf) | [:arrow_upper_right:]
+(https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/
+IPNN) | `torch` | | 9 | KDD'16 | [DeepCrossing](./model_zoo/DeepCrossing) |
+[Deep Crossing: Web-Scale Modeling without Manually Crafted Combinatorial
+Features](https://www.kdd.org/kdd2016/papers/files/adf0975-shanA.pdf) :
+triangular_flag_on_post:**Microsoft** | [:arrow_upper_right:](https://
+github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DeepCrossing)
+| `torch` | | 10 | NIPS'16 | [HOFM](./model_zoo/HOFM) | [Higher-Order
+Factorization Machines](https://papers.nips.cc/paper/6144-higher-order-
+factorization-machines.pdf) | [:arrow_upper_right:](https://github.com/
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/HOFM) | `torch` | | 11 |
+IJCAI'17 | [DeepFM](./model_zoo/DeepFM) | [DeepFM: A Factorization-Machine
+based Neural Network for CTR Prediction](https://arxiv.org/abs/1703.04247) :
+triangular_flag_on_post:**Huawei** | [:arrow_upper_right:](https://github.com/
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DeepFM) | `torch`, `tf`
+| | 12 | SIGIR'17 | [NFM](./model_zoo/NFM) | [Neural Factorization Machines for
+Sparse Predictive Analytics](https://dl.acm.org/citation.cfm?id=3080777) | [:
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/NFM) | `torch` | | 13 | IJCAI'17 | [AFM](./model_zoo/
+AFM) | [Attentional Factorization Machines: Learning the Weight of Feature
+Interactions via Attention Networks](http://www.ijcai.org/proceedings/2017/
+0435.pdf) | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
+main/ctr_prediction/benchmarks/AFM) | `torch` | | 14 | ADKDD'17 | [DCN](./
+model_zoo/DCN) | [Deep & Cross Network for Ad Click Predictions](https://
+arxiv.org/abs/1708.05123) :triangular_flag_on_post:**Google** | [:
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/DCN) | `torch`, `tf` | | 15 | WWW'18 | [FwFM](./
+model_zoo/FwFM) | [Field-weighted Factorization Machines for Click-Through Rate
+Prediction in Display Advertising](https://arxiv.org/pdf/1806.03514.pdf) :
+triangular_flag_on_post:**Oath, TouchPal, LinkedIn, Alibaba** | [:
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/FwFM) | `torch` | | 16 | KDD'18 | [xDeepFM](./
+model_zoo/xDeepFM) | [xDeepFM: Combining Explicit and Implicit Feature
+Interactions for Recommender Systems](https://arxiv.org/pdf/1803.05170.pdf) :
+triangular_flag_on_post:**Microsoft** | [:arrow_upper_right:](https://
+github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/xDeepFM) |
+`torch` | | 17 | CIKM'19 | [FiGNN](./model_zoo/FiGNN) | [FiGNN: Modeling
+Feature Interactions via Graph Neural Networks for CTR Prediction](https://
+arxiv.org/abs/1910.05552) | [:arrow_upper_right:](https://github.com/
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FiGNN) | `torch` | | 18
+| CIKM'19 | [AutoInt/AutoInt+](./model_zoo/AutoInt) | [AutoInt: Automatic
+Feature Interaction Learning via Self-Attentive Neural Networks](https://
+arxiv.org/abs/1810.11921) | [:arrow_upper_right:](https://github.com/
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/AutoInt) | `torch` | |
+19 | RecSys'19 | [FiBiNET](./model_zoo/FiBiNET) | [FiBiNET: Combining Feature
+Importance and Bilinear feature Interaction for Click-Through Rate Prediction]
+(https://arxiv.org/abs/1905.09433) :triangular_flag_on_post:**Sina Weibo** | [:
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/FiBiNET) | `torch` | | 20 | WWW'19 | [FGCNN](./
+model_zoo/FGCNN) | [Feature Generation by Convolutional Neural Network for
+Click-Through Rate Prediction](https://arxiv.org/abs/1904.04447) :
+triangular_flag_on_post:**Huawei** | [:arrow_upper_right:](https://github.com/
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FGCNN) | `torch` | | 21
+| AAAI'19 | [HFM/HFM+](./model_zoo/HFM) | [Holographic Factorization Machines
+for Recommendation](https://ojs.aaai.org//index.php/AAAI/article/view/4448) |
+[:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/HFM) | `torch` | | 22 | Arxiv'19 | [DLRM](./
+model_zoo/DLRM) | [Deep Learning Recommendation Model for Personalization and
+Recommendation Systems](https://arxiv.org/abs/1906.00091) :
+triangular_flag_on_post:**Facebook** | [:arrow_upper_right:](https://
+github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DLRM) |
+`torch` | | 23 | NeuralNetworks'20 | [ONN](./model_zoo/ONN) | [Operation-aware
+Neural Networks for User Response Prediction](https://arxiv.org/pdf/1904.12579)
+| [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/ONN) | `torch` | | 24 | AAAI'20 | [AFN/AFN+](./
+model_zoo/AFN) | [Adaptive Factorization Network: Learning Adaptive-Order
+Feature Interactions](https://ojs.aaai.org/index.php/AAAI/article/view/5768) |
+[:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/AFN) | `torch` | | 25 | AAAI'20 | [LorentzFM](./
+model_zoo/LorentzFM) | [Learning Feature Interactions with Lorentzian
+Factorization](https://arxiv.org/abs/1911.09821) :triangular_flag_on_post:
+**eBay** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
+main/ctr_prediction/benchmarks/LorentzFM) | `torch` | | 26 | WSDM'20 |
+[InterHAt](./model_zoo/InterHAt) | [Interpretable Click-through Rate Prediction
+through Hierarchical Attention](https://dl.acm.org/doi/10.1145/3336191.3371785)
+:triangular_flag_on_post:**NEC Labs, Google** | [:arrow_upper_right:](https://
+github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/InterHAt) |
+`torch` | | 27 | DLP-KDD'20 | [FLEN](./model_zoo/FLEN) | [FLEN: Leveraging
+Field for Scalable CTR Prediction](https://arxiv.org/abs/1911.04690) :
+triangular_flag_on_post:**Tencent** | [:arrow_upper_right:](https://github.com/
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FLEN) | `torch` | | 28 |
+CIKM'20 | [DeepIM](./model_zoo/DeepIM) | [Deep Interaction Machine: A Simple
+but Effective Model for High-order Feature Interactions](https://dl.acm.org/
+doi/abs/10.1145/3340531.3412077) :triangular_flag_on_post:**Alibaba, RealAI** |
+[:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
 ctr_prediction/benchmarks/DeepIM) | `torch` | | 29 | WWW'21 | [FmFM](./
 model_zoo/FmFM) | [FM^2: Field-matrixed Factorization Machines for Recommender
 Systems](https://arxiv.org/abs/2102.12994) :triangular_flag_on_post:**Yahoo** |
-[:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
+[:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
 ctr_prediction/benchmarks/FmFM) | `torch` | | 30 | WWW'21 | [DCN-V2](./
 model_zoo/DCNv2) | [DCN V2: Improved Deep & Cross Network and Practical Lessons
 for Web-scale Learning to Rank Systems](https://arxiv.org/abs/2008.13535) :
 triangular_flag_on_post:**Google** | [:arrow_upper_right:](https://github.com/
-openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DCNv2) | `torch` | |
-31 | CIKM'21 | [DESTINE](./model_zoo/DESTINE) | [Disentangled Self-Attentive
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DCNv2) | `torch` | | 31
+| CIKM'21 | [DESTINE](./model_zoo/DESTINE) | [Disentangled Self-Attentive
 Neural Networks for Click-Through Rate Prediction](https://arxiv.org/abs/
 2101.03654) :triangular_flag_on_post:**Alibaba** | [:arrow_upper_right:](https:
-//github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DESTINE)
-| `torch` | | 32 | CIKM'21 | [EDCN](./model_zoo/EDCN) | [Enhancing Explicit and
+//github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DESTINE) |
+`torch` | | 32 | CIKM'21 | [EDCN](./model_zoo/EDCN) | [Enhancing Explicit and
 Implicit Feature Interactions via Information Sharing for Parallel Deep CTR
 Models](https://dlp-kdd.github.io/assets/pdf/DLP-KDD_2021_paper_12.pdf) :
 triangular_flag_on_post:**Huawei** | [:arrow_upper_right:](https://github.com/
-openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/EDCN) | `torch` | | 33
-| DLP-KDD'21 | [MaskNet](./model_zoo/MaskNet) | [MaskNet: Introducing Feature-
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/EDCN) | `torch` | | 33 |
+DLP-KDD'21 | [MaskNet](./model_zoo/MaskNet) | [MaskNet: Introducing Feature-
 Wise Multiplication to CTR Ranking Models by Instance-Guided Mask](https://
 arxiv.org/abs/2102.07619) :triangular_flag_on_post:**Sina Weibo** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
 ctr_prediction/benchmarks/MaskNet) | `torch` | | 34 | SIGIR'21 | [SAM](./
 model_zoo/SAM) | [Looking at CTR Prediction Again: Is Attention All You Need?]
 (https://arxiv.org/abs/2105.05563) :triangular_flag_on_post:**BOSS Zhipin** |
-[:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
+[:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
 ctr_prediction/benchmarks/SAM) | `torch` | | 35 | KDD'21 | [AOANet](./
 model_zoo/AOANet) | [Architecture and Operation Adaptive Network for Online
 Recommendations](https://dl.acm.org/doi/10.1145/3447548.3467133) :
 triangular_flag_on_post:**Didi Chuxing** | [:arrow_upper_right:](https://
-github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/AOANet) |
-`torch` | | 36 | Blog'21 | [PPNet](./model_zoo/PPNet) | [Parameter Personalized
-Net](https://www.jiqizhixin.com/articles/2021-02-03-6) :
-triangular_flag_on_post:**KuaiShou** | | `torch` | | 37 | AAAI'23 | [FinalMLP]
-(./model_zoo/FinalMLP) | FinalMLP: An Enhanced Two-Stream MLP Model for CTR
-PredictionÂ :triangular_flag_on_post:**Huawei** | | `torch` | | | | | :
-point_down:**User Behavior Modeling** | | | | 38 | KDD'18 | [DIN](./model_zoo/
-DIN) | [Deep Interest Network for Click-Through Rate Prediction](https://
-www.kdd.org/kdd2018/accepted-papers/view/deep-interest-network-for-click-
-through-rate-prediction) :triangular_flag_on_post:**Alibaba** | | `torch` | |
-39 | AAAI'19 | [DIEN](./model_zoo/DIEN) | [Deep Interest Evolution Network for
-Click-Through Rate Prediction](https://arxiv.org/abs/1809.03672)Â :
-triangular_flag_on_post:**Alibaba** | | `torch` | | 40 | DLP-KDD'19 | [BST](./
-model_zoo/BST) | [Behavior Sequence Transformer for E-commerce Recommendation
-in Alibaba](https://arxiv.org/abs/1905.06874)Â :triangular_flag_on_post:
-**Alibaba** | | `torch` | | 41 | CIKM'20 | [DMIN](./model_zoo/DMIN) | [Deep
-Multi-Interest Network for Click-through Rate Prediction](https://dl.acm.org/
-doi/10.1145/3340531.3412092)Â :triangular_flag_on_post:**Alibaba** | | `torch`
-| | 42 | AAAI'20 | [DMR](./model_zoo/DMR) | [Deep Match to Rank Model for
-Personalized Click-Through Rate Prediction](https://ojs.aaai.org/index.php/
-AAAI/article/view/5346)Â :triangular_flag_on_post:**Alibaba** | | `torch` | |
-43 | Arxiv'21 | [ETA](./model_zoo/ETA) | [End-to-End User Behavior Retrieval in
-Click-Through RatePrediction Model](https://arxiv.org/abs/2108.04468)Â :
+github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/AOANet) |
+`torch` | | 36 | AAAI'23 | [FinalMLP](./model_zoo/FinalMLP) | [FinalMLP: An
+Enhanced Two-Stream MLP Model for CTR Prediction](https://arxiv.org/abs/
+2304.00902)Â :triangular_flag_on_post:**Huawei** | [:arrow_upper_right:](https:
+//github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FinalMLP) |
+`torch` | | 37 | SIGIR'23 | [FINAL](./model_zoo/FINAL) | FINAL: Factorized
+Interaction Layer for CTR PredictionÂ :triangular_flag_on_post:**Huawei** | [:
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/FINAL) | `torch` | | | | | :point_down:**User
+Behavior Modeling** | | | | 38 | KDD'18 | [DIN](./model_zoo/DIN) | [Deep
+Interest Network for Click-Through Rate Prediction](https://www.kdd.org/
+kdd2018/accepted-papers/view/deep-interest-network-for-click-through-rate-
+prediction) :triangular_flag_on_post:**Alibaba** | [:arrow_upper_right:](https:
+//github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DIN) |
+`torch` | | 39 | AAAI'19 | [DIEN](./model_zoo/DIEN) | [Deep Interest Evolution
+Network for Click-Through Rate Prediction](https://arxiv.org/abs/1809.03672)Â :
+triangular_flag_on_post:**Alibaba** | [:arrow_upper_right:](https://github.com/
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DIEN) | `torch` | | 40 |
+DLP-KDD'19 | [BST](./model_zoo/BST) | [Behavior Sequence Transformer for E-
+commerce Recommendation in Alibaba](https://arxiv.org/abs/1905.06874)Â :
+triangular_flag_on_post:**Alibaba** | [:arrow_upper_right:](https://github.com/
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/BST) | `torch` | | 41 |
+CIKM'20 | [DMIN](./model_zoo/DMIN) | [Deep Multi-Interest Network for Click-
+through Rate Prediction](https://dl.acm.org/doi/10.1145/3340531.3412092)Â :
+triangular_flag_on_post:**Alibaba** | | `torch` | | 42 | AAAI'20 | [DMR](./
+model_zoo/DMR) | [Deep Match to Rank Model for Personalized Click-Through Rate
+Prediction](https://ojs.aaai.org/index.php/AAAI/article/view/5346)Â :
+triangular_flag_on_post:**Alibaba** | | `torch` | | 43 | Arxiv'21 | [ETA](./
+model_zoo/ETA) | [End-to-End User Behavior Retrieval in Click-Through
+RatePrediction Model](https://arxiv.org/abs/2108.04468)Â :
 triangular_flag_on_post:**Alibaba** | | `torch` | | 44 | CIKM'22 | [SDIM](./
 model_zoo/SDIM) | [Sampling Is All You Need on Modeling Long-Term User
 Behaviors for CTR Prediction](https://arxiv.org/abs/2205.10249)Â :
-triangular_flag_on_post:**Meituan** | | `torch` | + :point_right: See [reusable
-dataset splits for CTR prediction](https://github.com/openbenchmark/BARS/blob/
-master/ctr_prediction/datasets). + :point_right: See [benchmarking
-configurations and steps](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks). + :point_right: See [the BARS benchmark website]
-(https://openbenchmark.github.io/ctr-prediction). ## Dependencies FuxiCTR has
-the following dependency requirements. + python 3.6+ + pytorch 1.10+ (required
-only for torch models) + tensorflow 2.1+ (required only for tf models) Other
-packages can be installed via `pip install -r requirements.txt`. ## Quick Start
-1. Run the demo examples Examples are provided in the demo directory to show
-some basic usage of FuxiCTR. Users can run the examples for quick start and to
-understand the workflow. ``` cd demo python example1_build_dataset_to_h5.py
-python example2_DeepFM_with_h5_input.py ``` 2. Run an existing model Users can
-easily run each model in the model zoo following the commands below, which is a
-demo for running DCN. In addition, users can modify the dataset config and
-model config files to run on their own datasets or with new hyper-parameters.
-More details can be found in the [readme file](./model_zoo/DCN/DCN_torch/
-README.md). ``` cd model_zoo/DCN/DCN_torch python run_expid.py --expid DCN_test
---gpu 0 ``` 3. Implement a new model The FuxiCTR code structure is modularized,
-so that every part can be overwritten by users according to their needs. In
-many cases, only the model class needs to be implemented for a new customized
-model. If data preprocessing or data loader is not directly applicable, one can
-also overwrite a new one through the [core APIs](https://www.processon.com/
-view/link/63cfcfab4e30670eac4a81c7). A complete example can be found at
-[model_zoo/FinalMLP](./model_zoo/FinalMLP/), which implements our new model
-FinalMLP that has been recently published in AAAI 2023. Some other examples are
-also available in the model zoo. ## Citation *:bell: If you find our code or
-benchmarks helpful in your research, please kindly cite the following papers.*
-> Jieming Zhu, Jinyang Liu, Shuai Yang, Qi Zhang, Xiuqiang He. [Open
+triangular_flag_on_post:**Meituan** | | `torch` | | | | | :point_down:**Multi-
+Task Models** | | | | 45 | MachineLearn'97 | [SharedBottom](./model_zoo/
+multitask/SharedBottom) | [Multitask Learning](https://link.springer.com/
+article/10.1023/A:1007379606734) | | `torch` | | 46 | KDD'18 | [MMoE](./
+model_zoo/multitask/MMOE) | [Modeling Task Relationships in Multi-task Learning
+with Multi-Gate Mixture-of-Experts](https://dl.acm.org/doi/pdf/10.1145/
+3219819.3220007) :triangular_flag_on_post:**Google** | | `torch` | | | | | :
+point_down:**Multi-Domain Models** | | | | 47 | Arxiv'23 | [PPNet](./model_zoo/
+PPNet)/PEPNet | [PEPNet: Parameter and Embedding Personalized Network for
+Infusing with Personalized Prior Information](https://arxiv.org/abs/2302.01115)
+:triangular_flag_on_post:**KuaiShou** | | `torch` | + :point_right: See
+[reusable dataset splits for CTR prediction](https://openbenchmark.github.io/
+BARS/datasets/README.html). + :point_right: See [benchmarking configurations
+and steps](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/
+benchmarks). + :point_right: See [the BARS benchmark leaderboard](https://
+openbenchmark.github.io/BARS/ctr_prediction/leaderboard/README.html#). ##
+Dependencies FuxiCTR has the following dependency requirements. + python 3.6+ +
+pytorch 1.0/1.10+ (required only for torch models) + tensorflow 2.1+ (required
+only for tf models) Other packages can be installed via `pip install -
+r requirements.txt`. ## Quick Start 1. Run the demo examples Examples are
+provided in the demo directory to show some basic usage of FuxiCTR. Users can
+run the examples for quick start and to understand the workflow. ``` cd demo
+python example1_build_dataset_to_h5.py python example2_DeepFM_with_h5_input.py
+``` 2. Run an existing model Users can easily run each model in the model zoo
+following the commands below, which is a demo for running DCN. In addition,
+users can modify the dataset config and model config files to run on their own
+datasets or with new hyper-parameters. More details can be found in the [readme
+file](./model_zoo/DCN/DCN_torch/README.md). ``` cd model_zoo/DCN/DCN_torch
+python run_expid.py --expid DCN_test --gpu 0 # Change `MODEL` according to the
+target model name cd model_zoo/MODEL_PATH python run_expid.py --expid
+MODEL_test --gpu 0 ``` 3. Implement a new model The FuxiCTR code structure is
+modularized, so that every part can be overwritten by users according to their
+needs. In many cases, only the model class needs to be implemented for a new
+customized model. If data preprocessing or data loader is not directly
+applicable, one can also overwrite a new one through the [core APIs](https://
+www.processon.com/view/link/63cfcfab4e30670eac4a81c7). We show a concrete
+example which implements our new model [FinalMLP](https://github.com/xue-pai/
+FinalMLP) that has been recently published in AAAI 2023. More examples can be
+found in the [model zoo](./model_zoo/). ## Citation *:bell: If you find our
+code or benchmarks helpful in your research, please kindly cite the following
+papers.* > Jieming Zhu, Jinyang Liu, Shuai Yang, Qi Zhang, Xiuqiang He. [Open
 Benchmarking for Click-Through Rate Prediction](https://arxiv.org/abs/
 2009.05794). *The 30th ACM International Conference on Information and
 Knowledge Management (CIKM)*, 2021. [[Bibtex](https://dblp.org/rec/conf/cikm/
 ZhuLYZH21.html?view=bibtex)] > Jieming Zhu, Quanyu Dai, Liangcai Su, Rong Ma,
 Jinyang Liu, Guohao Cai, Xi Xiao, Rui Zhang. [BARS: Towards Open Benchmarking
 for Recommender Systems](https://arxiv.org/abs/2205.09626). *The 45th
 International ACM SIGIR Conference on Research and Development in Information
```

### Comparing `fuxictr-2.0.1/fuxictr/autotuner.py` & `fuxictr-2.0.2/fuxictr/autotuner.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,15 @@
         
     # update dataset_id into model params
     merged_param_combs = dict()
     for idx, item in enumerate(itertools.product(model_param_combs.values(),
                                                  dataset_para_combs.keys())):
         para_dict = item[0]
         para_dict["dataset_id"] = item[1]
+        del para_dict["model_id"]
         random_str = ""
         if para_dict["debug_mode"]:
             random_str = "{:06d}".format(np.random.randint(1e6)) # add a random number to avoid duplicate during debug
         hash_id = hashlib.md5(("".join(sorted(print_to_json(para_dict))) + random_str).encode("utf-8")).hexdigest()[0:8]
         hash_expid = experiment_id + "_{:03d}_{}".format(idx + 1, hash_id)
         if hash_expid not in exclude_expid:
             merged_param_combs[hash_expid] = para_dict.copy()
```

### Comparing `fuxictr-2.0.1/fuxictr/datasets/avazu.py` & `fuxictr-2.0.2/fuxictr/datasets/avazu.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/datasets/criteo.py` & `fuxictr-2.0.2/fuxictr/datasets/criteo.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/datasets/kkbox.py` & `fuxictr-2.0.2/fuxictr/datasets/kkbox.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/features.py` & `fuxictr-2.0.2/fuxictr/features.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,16 @@
         self.num_fields = feature_map["num_fields"]
         self.labels = feature_map.get("labels", [])
         self.total_features = feature_map.get("total_features", 0)
         self.input_length = feature_map.get("input_length", 0)
         self.group_id = feature_map.get("group_id", None)
         self.default_emb_dim = params.get("embedding_dim", None)
         self.features = OrderedDict((k, v) for x in feature_map["features"] for k, v in x.items())
-        if params.get("ordered_features", None):
-            self.features = OrderedDict((x, self.features[x]) for x in params["ordered_features"])
+        if params.get("use_features", None):
+            self.features = OrderedDict((x, self.features[x]) for x in params["use_features"])
         if params.get("feature_specs", None):
             self.update_feature_specs(params["feature_specs"])
         self.set_column_index()
 
     def update_feature_specs(self, feature_specs):
         for col in feature_specs:
             namelist = col["name"]
```

### Comparing `fuxictr-2.0.1/fuxictr/metrics.py` & `fuxictr-2.0.2/fuxictr/metrics.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/preprocess/build_dataset.py` & `fuxictr-2.0.2/fuxictr/preprocess/build_dataset.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/preprocess/feature_processor.py` & `fuxictr-2.0.2/fuxictr/preprocess/feature_processor.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/preprocess/utils.py` & `fuxictr-2.0.2/fuxictr/preprocess/utils.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/pytorch/dataloaders/h5_block_dataloader.py` & `fuxictr-2.0.2/fuxictr/pytorch/dataloaders/h5_block_dataloader.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/pytorch/dataloaders/h5_dataloader.py` & `fuxictr-2.0.2/fuxictr/pytorch/dataloaders/h5_dataloader.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/pytorch/layers/activations.py` & `fuxictr-2.0.2/fuxictr/pytorch/layers/activations.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/pytorch/layers/attentions/dot_product_attention.py` & `fuxictr-2.0.2/fuxictr/pytorch/layers/attentions/dot_product_attention.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/pytorch/layers/attentions/squeeze_excitation.py` & `fuxictr-2.0.2/fuxictr/pytorch/layers/attentions/squeeze_excitation.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/pytorch/layers/attentions/target_attention.py` & `fuxictr-2.0.2/fuxictr/pytorch/layers/attentions/target_attention.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/pytorch/layers/blocks/factorization_machine.py` & `fuxictr-2.0.2/fuxictr/pytorch/layers/blocks/factorization_machine.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/pytorch/layers/blocks/logistic_regression.py` & `fuxictr-2.0.2/fuxictr/pytorch/layers/blocks/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/pytorch/layers/blocks/mlp_block.py` & `fuxictr-2.0.2/fuxictr/pytorch/layers/blocks/mlp_block.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,14 @@
                  input_dim, 
                  hidden_units=[], 
                  hidden_activations="ReLU",
                  output_dim=None,
                  output_activation=None, 
                  dropout_rates=0.0,
                  batch_norm=False, 
-                 layer_norm=False,
                  norm_before_activation=True,
                  use_bias=True):
         super(MLP_Block, self).__init__()
         dense_layers = []
         if not isinstance(dropout_rates, list):
             dropout_rates = [dropout_rates] * len(hidden_units)
         if not isinstance(hidden_activations, list):
@@ -41,23 +40,19 @@
         hidden_activations = get_activation(hidden_activations, hidden_units)
         hidden_units = [input_dim] + hidden_units
         for idx in range(len(hidden_units) - 1):
             dense_layers.append(nn.Linear(hidden_units[idx], hidden_units[idx + 1], bias=use_bias))
             if norm_before_activation:
                 if batch_norm:
                     dense_layers.append(nn.BatchNorm1d(hidden_units[idx + 1]))
-                elif layer_norm:
-                    dense_layers.append(nn.LayerNorm(hidden_units[idx + 1]))
             if hidden_activations[idx]:
                 dense_layers.append(hidden_activations[idx])
             if not norm_before_activation:
                 if batch_norm:
                     dense_layers.append(nn.BatchNorm1d(hidden_units[idx + 1]))
-                elif layer_norm:
-                    dense_layers.append(nn.LayerNorm(hidden_units[idx + 1]))
             if dropout_rates[idx] > 0:
                 dense_layers.append(nn.Dropout(p=dropout_rates[idx]))
         if output_dim is not None:
             dense_layers.append(nn.Linear(hidden_units[-1], output_dim, bias=use_bias))
         if output_activation is not None:
             dense_layers.append(get_activation(output_activation))
         self.mlp = nn.Sequential(*dense_layers) # * used to unpack list
```

### Comparing `fuxictr-2.0.1/fuxictr/pytorch/layers/embeddings/feature_embedding.py` & `fuxictr-2.0.2/fuxictr/pytorch/layers/embeddings/feature_embedding.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/pytorch/layers/interactions/bilinear_interaction.py` & `fuxictr-2.0.2/fuxictr/pytorch/layers/interactions/bilinear_interaction.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/pytorch/layers/interactions/compressed_interaction_net.py` & `fuxictr-2.0.2/fuxictr/pytorch/layers/interactions/compressed_interaction_net.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/pytorch/layers/interactions/cross_net.py` & `fuxictr-2.0.2/fuxictr/pytorch/layers/interactions/cross_net.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/pytorch/layers/interactions/holographic_interaction.py` & `fuxictr-2.0.2/fuxictr/pytorch/layers/interactions/holographic_interaction.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/pytorch/layers/interactions/inner_product.py` & `fuxictr-2.0.2/fuxictr/pytorch/layers/interactions/inner_product.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/pytorch/layers/interactions/interaction_machine.py` & `fuxictr-2.0.2/fuxictr/pytorch/layers/interactions/interaction_machine.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/pytorch/layers/pooling.py` & `fuxictr-2.0.2/fuxictr/pytorch/layers/pooling.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/pytorch/models/base_model.py` & `fuxictr-2.0.2/fuxictr/pytorch/models/ctr_model.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/pytorch/torch_utils.py` & `fuxictr-2.0.2/fuxictr/pytorch/torch_utils.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/tensorflow/dataloaders/tf_dataloader.py` & `fuxictr-2.0.2/fuxictr/tensorflow/dataloaders/tf_dataloader.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/tensorflow/layers/blocks/factorization_machine.py` & `fuxictr-2.0.2/fuxictr/tensorflow/layers/blocks/factorization_machine.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/tensorflow/layers/blocks/linear.py` & `fuxictr-2.0.2/fuxictr/tensorflow/layers/blocks/linear.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/tensorflow/layers/blocks/logistic_regression.py` & `fuxictr-2.0.2/fuxictr/tensorflow/layers/blocks/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/tensorflow/layers/blocks/mlp_block.py` & `fuxictr-2.0.2/fuxictr/tensorflow/layers/blocks/mlp_block.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/tensorflow/layers/embeddings/feature_embedding.py` & `fuxictr-2.0.2/fuxictr/tensorflow/layers/embeddings/feature_embedding.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/tensorflow/layers/interactions/cross_net.py` & `fuxictr-2.0.2/fuxictr/tensorflow/layers/interactions/cross_net.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/tensorflow/layers/interactions/inner_product.py` & `fuxictr-2.0.2/fuxictr/tensorflow/layers/interactions/inner_product.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/tensorflow/layers/pooling.py` & `fuxictr-2.0.2/fuxictr/tensorflow/layers/pooling.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/tensorflow/models/base_model.py` & `fuxictr-2.0.2/fuxictr/tensorflow/models/ctr_model.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/tensorflow/tf_utils.py` & `fuxictr-2.0.2/fuxictr/tensorflow/tf_utils.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr/utils.py` & `fuxictr-2.0.2/fuxictr/utils.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.1/fuxictr.egg-info/PKG-INFO` & `fuxictr-2.0.2/fuxictr.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuxictr
-Version: 2.0.1
+Version: 2.0.2
 Summary: A configurable, tunable, and reproducible library for CTR prediction
 Home-page: https://github.com/xue-pai/FuxiCTR
 Author: zhujiem
 Author-email: zhujiem@users.noreply.github.com
 License: Apache-2.0 License
 Download-URL: https://github.com/xue-pai/FuxiCTR/tags
 Description: <div align="center">
@@ -41,70 +41,77 @@
         
         
         ## Model Zoo
         
         | No  | Publication       | Model                                    | Paper                                                                                                                                                                                                           | Benchmark                                                                                                       | Version       |
         |:---:|:-----------------:|:----------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |:---------------------------------------------------------------------------------------------------------------:|:-------------:|
         |     |                   |                                          | :point_down:**Feature Interaction Models**                                                                                                                                                                      |                                                                                                                 |               |
-        | 1   | WWW'07            | [LR](./model_zoo/LR)                     | [Predicting Clicks: Estimating the Click-Through Rate for New Ads](https://dl.acm.org/citation.cfm?id=1242643) :triangular_flag_on_post:**Microsoft**                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/LR)           | `torch`       |
-        | 2   | ICDM'10           | [FM](./model_zoo/FM)                     | [Factorization Machines](https://www.csie.ntu.edu.tw/~b97053/paper/Rendle2010FM.pdf)                                                                                                                            | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/FM)           | `torch`       |
-        | 3   | CIKM'13           | [DSSM](./model_zoo/DSSM)                 | [Learning Deep Structured Semantic Models  for Web Search using Clickthrough Data ](https://posenhuang.github.io/papers/cikm2013_DSSM_fullversion.pdf) :triangular_flag_on_post:**Microsoft**                   | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DSSM)         | `torch`       |
-        | 4   | CIKM'15           | [CCPM](./model_zoo/CCPM)                 | [A Convolutional Click Prediction Model](http://www.escience.cn/system/download/73676)                                                                                                                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/CCPM)         | `torch`       |
-        | 5   | RecSys'16         | [FFM](./model_zoo/FFM)                   | [Field-aware Factorization Machines for CTR Prediction](https://dl.acm.org/citation.cfm?id=2959134) :triangular_flag_on_post:**Criteo**                                                                         | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/FFM)          | `torch`       |
-        | 6   | RecSys'16         | [YoutubeDNN](./model_zoo/DNN)            | [Deep Neural Networks for YouTube Recommendations](http://art.yale.edu/file_columns/0001/1132/covington.pdf) :triangular_flag_on_post:**Google**                                                                | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DNN)          | `torch`, `tf` |
-        | 7   | DLRS'16           | [Wide&Deep](./model_zoo/WideDeep)        | [Wide & Deep Learning for Recommender Systems](https://arxiv.org/pdf/1606.07792.pdf) :triangular_flag_on_post:**Google**                                                                                        | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/WideDeep)     | `torch`, `tf` |
-        | 8   | ICDM'16           | [IPNN](./model_zoo/PNN)                  | [Product-based Neural Networks for User Response Prediction](https://arxiv.org/pdf/1611.00144.pdf)                                                                                                              | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/IPNN)         | `torch`       |
-        | 9   | KDD'16            | [DeepCrossing](./model_zoo/DeepCrossing) | [Deep Crossing: Web-Scale Modeling without Manually Crafted Combinatorial Features](https://www.kdd.org/kdd2016/papers/files/adf0975-shanA.pdf) :triangular_flag_on_post:**Microsoft**                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DeepCrossing) | `torch`       |
-        | 10  | NIPS'16           | [HOFM](./model_zoo/HOFM)                 | [Higher-Order Factorization Machines](https://papers.nips.cc/paper/6144-higher-order-factorization-machines.pdf)                                                                                                | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/HOFM)         | `torch`       |
-        | 11  | IJCAI'17          | [DeepFM](./model_zoo/DeepFM)             | [DeepFM: A Factorization-Machine based Neural Network for CTR Prediction](https://arxiv.org/abs/1703.04247) :triangular_flag_on_post:**Huawei**                                                                 | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DeepFM)       | `torch`, `tf` |
-        | 12  | SIGIR'17          | [NFM](./model_zoo/NFM)                   | [Neural Factorization Machines for Sparse Predictive Analytics](https://dl.acm.org/citation.cfm?id=3080777)                                                                                                     | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/NFM)          | `torch`       |
-        | 13  | IJCAI'17          | [AFM](./model_zoo/AFM)                   | [Attentional Factorization Machines: Learning the Weight of Feature Interactions via Attention Networks](http://www.ijcai.org/proceedings/2017/0435.pdf)                                                        | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/AFM)          | `torch`       |
-        | 14  | ADKDD'17          | [DCN](./model_zoo/DCN)                   | [Deep & Cross Network for Ad Click Predictions](https://arxiv.org/abs/1708.05123) :triangular_flag_on_post:**Google**                                                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DCN)          | `torch`, `tf` |
-        | 15  | WWW'18            | [FwFM](./model_zoo/FwFM)                 | [Field-weighted Factorization Machines for Click-Through Rate Prediction in Display Advertising](https://arxiv.org/pdf/1806.03514.pdf) :triangular_flag_on_post:**Oath, TouchPal, LinkedIn, Alibaba**           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/FwFM)         | `torch`       |
-        | 16  | KDD'18            | [xDeepFM](./model_zoo/xDeepFM)           | [xDeepFM: Combining Explicit and Implicit Feature Interactions for Recommender Systems](https://arxiv.org/pdf/1803.05170.pdf) :triangular_flag_on_post:**Microsoft**                                            | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/xDeepFM)      | `torch`       |
-        | 17  | CIKM'19           | [FiGNN](./model_zoo/FiGNN)               | [FiGNN: Modeling Feature Interactions via Graph Neural Networks for CTR Prediction](https://arxiv.org/abs/1910.05552)                                                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/FiGNN)        | `torch`       |
-        | 18  | CIKM'19           | [AutoInt/AutoInt+](./model_zoo/AutoInt)  | [AutoInt: Automatic Feature Interaction Learning via Self-Attentive Neural Networks](https://arxiv.org/abs/1810.11921)                                                                                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/AutoInt)      | `torch`       |
-        | 19  | RecSys'19         | [FiBiNET](./model_zoo/FiBiNET)           | [FiBiNET: Combining Feature Importance and Bilinear feature Interaction for Click-Through Rate Prediction](https://arxiv.org/abs/1905.09433) :triangular_flag_on_post:**Sina Weibo**                            | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/FiBiNET)      | `torch`       |
-        | 20  | WWW'19            | [FGCNN](./model_zoo/FGCNN)               | [Feature Generation by Convolutional Neural Network for Click-Through Rate Prediction](https://arxiv.org/abs/1904.04447) :triangular_flag_on_post:**Huawei**                                                    | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/FGCNN)        | `torch`       |
-        | 21  | AAAI'19           | [HFM/HFM+](./model_zoo/HFM)              | [Holographic Factorization Machines for Recommendation](https://ojs.aaai.org//index.php/AAAI/article/view/4448)                                                                                                 | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/HFM)          | `torch`       |
-        | 22  | Arxiv'19          | [DLRM](./model_zoo/DLRM)                 | [Deep Learning Recommendation Model for Personalization and Recommendation Systems](https://arxiv.org/abs/1906.00091) :triangular_flag_on_post:**Facebook**                                                     | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DLRM)         | `torch`       |
-        | 23  | NeuralNetworks'20 | [ONN](./model_zoo/ONN)                   | [Operation-aware Neural Networks for User Response Prediction](https://arxiv.org/pdf/1904.12579)                                                                                                                | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/ONN)          | `torch`       |
-        | 24  | AAAI'20           | [AFN/AFN+](./model_zoo/AFN)              | [Adaptive Factorization Network: Learning Adaptive-Order Feature Interactions](https://ojs.aaai.org/index.php/AAAI/article/view/5768)                                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/AFN)          | `torch`       |
-        | 25  | AAAI'20           | [LorentzFM](./model_zoo/LorentzFM)       | [Learning Feature Interactions with Lorentzian Factorization](https://arxiv.org/abs/1911.09821) :triangular_flag_on_post:**eBay**                                                                               | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/LorentzFM)    | `torch`       |
-        | 26  | WSDM'20           | [InterHAt](./model_zoo/InterHAt)         | [Interpretable Click-through Rate Prediction through Hierarchical Attention](https://dl.acm.org/doi/10.1145/3336191.3371785) :triangular_flag_on_post:**NEC Labs, Google**                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/InterHAt)     | `torch`       |
-        | 27  | DLP-KDD'20        | [FLEN](./model_zoo/FLEN)                 | [FLEN: Leveraging Field for Scalable CTR Prediction](https://arxiv.org/abs/1911.04690) :triangular_flag_on_post:**Tencent**                                                                                     | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/FLEN)         | `torch`       |
-        | 28  | CIKM'20           | [DeepIM](./model_zoo/DeepIM)             | [Deep Interaction Machine: A Simple but Effective Model for High-order Feature Interactions](https://dl.acm.org/doi/abs/10.1145/3340531.3412077) :triangular_flag_on_post:**Alibaba, RealAI**                   | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DeepIM)       | `torch`       |
-        | 29  | WWW'21            | [FmFM](./model_zoo/FmFM)                 | [FM^2: Field-matrixed Factorization Machines for Recommender Systems](https://arxiv.org/abs/2102.12994) :triangular_flag_on_post:**Yahoo**                                                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/FmFM)         | `torch`       |
-        | 30  | WWW'21            | [DCN-V2](./model_zoo/DCNv2)              | [DCN V2: Improved Deep & Cross Network and Practical Lessons for Web-scale Learning to Rank Systems](https://arxiv.org/abs/2008.13535) :triangular_flag_on_post:**Google**                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DCNv2)        | `torch`       |
-        | 31  | CIKM'21           | [DESTINE](./model_zoo/DESTINE)           | [Disentangled Self-Attentive Neural Networks for Click-Through Rate Prediction](https://arxiv.org/abs/2101.03654) :triangular_flag_on_post:**Alibaba**                                                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DESTINE)      | `torch`       |
-        | 32  | CIKM'21           | [EDCN](./model_zoo/EDCN)                 | [Enhancing Explicit and Implicit Feature Interactions via Information Sharing for Parallel Deep CTR Models](https://dlp-kdd.github.io/assets/pdf/DLP-KDD_2021_paper_12.pdf) :triangular_flag_on_post:**Huawei** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/EDCN)         | `torch`       |
-        | 33  | DLP-KDD'21        | [MaskNet](./model_zoo/MaskNet)           | [MaskNet: Introducing Feature-Wise Multiplication to CTR Ranking Models by Instance-Guided Mask](https://arxiv.org/abs/2102.07619) :triangular_flag_on_post:**Sina Weibo**                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/MaskNet)      | `torch`       |
-        | 34  | SIGIR'21          | [SAM](./model_zoo/SAM)                   | [Looking at CTR Prediction Again: Is Attention All You Need?](https://arxiv.org/abs/2105.05563) :triangular_flag_on_post:**BOSS Zhipin**                                                                        | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/SAM)          | `torch`       |
-        | 35  | KDD'21            | [AOANet](./model_zoo/AOANet)             | [Architecture and Operation Adaptive Network for Online Recommendations](https://dl.acm.org/doi/10.1145/3447548.3467133) :triangular_flag_on_post:**Didi Chuxing**                                              | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/AOANet)       | `torch`       |
-        | 36  | Blog'21           | [PPNet](./model_zoo/PPNet)               | [Parameter Personalized Net](https://www.jiqizhixin.com/articles/2021-02-03-6) :triangular_flag_on_post:**KuaiShou**                                                                                            |                                                                                                                 | `torch`       |
-        | 37  | AAAI'23           | [FinalMLP](./model_zoo/FinalMLP)         | FinalMLP: An Enhanced Two-Stream MLP Model for CTR Prediction :triangular_flag_on_post:**Huawei**                                                                                                               |                                                                                                                 | `torch`       |
+        | 1   | WWW'07            | [LR](./model_zoo/LR)                     | [Predicting Clicks: Estimating the Click-Through Rate for New Ads](https://dl.acm.org/citation.cfm?id=1242643) :triangular_flag_on_post:**Microsoft**                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/LR)           | `torch`       |
+        | 2   | ICDM'10           | [FM](./model_zoo/FM)                     | [Factorization Machines](https://www.csie.ntu.edu.tw/~b97053/paper/Rendle2010FM.pdf)                                                                                                                            | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FM)           | `torch`       |
+        | 3   | CIKM'13           | [DSSM](./model_zoo/DSSM)                 | [Learning Deep Structured Semantic Models  for Web Search using Clickthrough Data ](https://posenhuang.github.io/papers/cikm2013_DSSM_fullversion.pdf) :triangular_flag_on_post:**Microsoft**                   | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DSSM)         | `torch`       |
+        | 4   | CIKM'15           | [CCPM](./model_zoo/CCPM)                 | [A Convolutional Click Prediction Model](http://www.escience.cn/system/download/73676)                                                                                                                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/CCPM)         | `torch`       |
+        | 5   | RecSys'16         | [FFM](./model_zoo/FFM)                   | [Field-aware Factorization Machines for CTR Prediction](https://dl.acm.org/citation.cfm?id=2959134) :triangular_flag_on_post:**Criteo**                                                                         | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FFM)          | `torch`       |
+        | 6   | RecSys'16         | [DNN](./model_zoo/DNN)            | [Deep Neural Networks for YouTube Recommendations](http://art.yale.edu/file_columns/0001/1132/covington.pdf) :triangular_flag_on_post:**Google**                                                                | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DNN)          | `torch`, `tf` |
+        | 7   | DLRS'16           | [Wide&Deep](./model_zoo/WideDeep)        | [Wide & Deep Learning for Recommender Systems](https://arxiv.org/pdf/1606.07792.pdf) :triangular_flag_on_post:**Google**                                                                                        | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/WideDeep)     | `torch`, `tf` |
+        | 8   | ICDM'16           | [IPNN](./model_zoo/PNN)                  | [Product-based Neural Networks for User Response Prediction](https://arxiv.org/pdf/1611.00144.pdf)                                                                                                              | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/IPNN)         | `torch`       |
+        | 9   | KDD'16            | [DeepCrossing](./model_zoo/DeepCrossing) | [Deep Crossing: Web-Scale Modeling without Manually Crafted Combinatorial Features](https://www.kdd.org/kdd2016/papers/files/adf0975-shanA.pdf) :triangular_flag_on_post:**Microsoft**                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DeepCrossing) | `torch`       |
+        | 10  | NIPS'16           | [HOFM](./model_zoo/HOFM)                 | [Higher-Order Factorization Machines](https://papers.nips.cc/paper/6144-higher-order-factorization-machines.pdf)                                                                                                | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/HOFM)         | `torch`       |
+        | 11  | IJCAI'17          | [DeepFM](./model_zoo/DeepFM)             | [DeepFM: A Factorization-Machine based Neural Network for CTR Prediction](https://arxiv.org/abs/1703.04247) :triangular_flag_on_post:**Huawei**                                                                 | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DeepFM)       | `torch`, `tf` |
+        | 12  | SIGIR'17          | [NFM](./model_zoo/NFM)                   | [Neural Factorization Machines for Sparse Predictive Analytics](https://dl.acm.org/citation.cfm?id=3080777)                                                                                                     | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/NFM)          | `torch`       |
+        | 13  | IJCAI'17          | [AFM](./model_zoo/AFM)                   | [Attentional Factorization Machines: Learning the Weight of Feature Interactions via Attention Networks](http://www.ijcai.org/proceedings/2017/0435.pdf)                                                        | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/AFM)          | `torch`       |
+        | 14  | ADKDD'17          | [DCN](./model_zoo/DCN)                   | [Deep & Cross Network for Ad Click Predictions](https://arxiv.org/abs/1708.05123) :triangular_flag_on_post:**Google**                                                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DCN)          | `torch`, `tf` |
+        | 15  | WWW'18            | [FwFM](./model_zoo/FwFM)                 | [Field-weighted Factorization Machines for Click-Through Rate Prediction in Display Advertising](https://arxiv.org/pdf/1806.03514.pdf) :triangular_flag_on_post:**Oath, TouchPal, LinkedIn, Alibaba**           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FwFM)         | `torch`       |
+        | 16  | KDD'18            | [xDeepFM](./model_zoo/xDeepFM)           | [xDeepFM: Combining Explicit and Implicit Feature Interactions for Recommender Systems](https://arxiv.org/pdf/1803.05170.pdf) :triangular_flag_on_post:**Microsoft**                                            | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/xDeepFM)      | `torch`       |
+        | 17  | CIKM'19           | [FiGNN](./model_zoo/FiGNN)               | [FiGNN: Modeling Feature Interactions via Graph Neural Networks for CTR Prediction](https://arxiv.org/abs/1910.05552)                                                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FiGNN)        | `torch`       |
+        | 18  | CIKM'19           | [AutoInt/AutoInt+](./model_zoo/AutoInt)  | [AutoInt: Automatic Feature Interaction Learning via Self-Attentive Neural Networks](https://arxiv.org/abs/1810.11921)                                                                                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/AutoInt)      | `torch`       |
+        | 19  | RecSys'19         | [FiBiNET](./model_zoo/FiBiNET)           | [FiBiNET: Combining Feature Importance and Bilinear feature Interaction for Click-Through Rate Prediction](https://arxiv.org/abs/1905.09433) :triangular_flag_on_post:**Sina Weibo**                            | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FiBiNET)      | `torch`       |
+        | 20  | WWW'19            | [FGCNN](./model_zoo/FGCNN)               | [Feature Generation by Convolutional Neural Network for Click-Through Rate Prediction](https://arxiv.org/abs/1904.04447) :triangular_flag_on_post:**Huawei**                                                    | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FGCNN)        | `torch`       |
+        | 21  | AAAI'19           | [HFM/HFM+](./model_zoo/HFM)              | [Holographic Factorization Machines for Recommendation](https://ojs.aaai.org//index.php/AAAI/article/view/4448)                                                                                                 | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/HFM)          | `torch`       |
+        | 22  | Arxiv'19          | [DLRM](./model_zoo/DLRM)                 | [Deep Learning Recommendation Model for Personalization and Recommendation Systems](https://arxiv.org/abs/1906.00091) :triangular_flag_on_post:**Facebook**                                                     | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DLRM)         | `torch`       |
+        | 23  | NeuralNetworks'20 | [ONN](./model_zoo/ONN)                   | [Operation-aware Neural Networks for User Response Prediction](https://arxiv.org/pdf/1904.12579)                                                                                                                | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/ONN)          | `torch`       |
+        | 24  | AAAI'20           | [AFN/AFN+](./model_zoo/AFN)              | [Adaptive Factorization Network: Learning Adaptive-Order Feature Interactions](https://ojs.aaai.org/index.php/AAAI/article/view/5768)                                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/AFN)          | `torch`       |
+        | 25  | AAAI'20           | [LorentzFM](./model_zoo/LorentzFM)       | [Learning Feature Interactions with Lorentzian Factorization](https://arxiv.org/abs/1911.09821) :triangular_flag_on_post:**eBay**                                                                               | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/LorentzFM)    | `torch`       |
+        | 26  | WSDM'20           | [InterHAt](./model_zoo/InterHAt)         | [Interpretable Click-through Rate Prediction through Hierarchical Attention](https://dl.acm.org/doi/10.1145/3336191.3371785) :triangular_flag_on_post:**NEC Labs, Google**                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/InterHAt)     | `torch`       |
+        | 27  | DLP-KDD'20        | [FLEN](./model_zoo/FLEN)                 | [FLEN: Leveraging Field for Scalable CTR Prediction](https://arxiv.org/abs/1911.04690) :triangular_flag_on_post:**Tencent**                                                                                     | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FLEN)         | `torch`       |
+        | 28  | CIKM'20           | [DeepIM](./model_zoo/DeepIM)             | [Deep Interaction Machine: A Simple but Effective Model for High-order Feature Interactions](https://dl.acm.org/doi/abs/10.1145/3340531.3412077) :triangular_flag_on_post:**Alibaba, RealAI**                   | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DeepIM)       | `torch`       |
+        | 29  | WWW'21            | [FmFM](./model_zoo/FmFM)                 | [FM^2: Field-matrixed Factorization Machines for Recommender Systems](https://arxiv.org/abs/2102.12994) :triangular_flag_on_post:**Yahoo**                                                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FmFM)         | `torch`       |
+        | 30  | WWW'21            | [DCN-V2](./model_zoo/DCNv2)              | [DCN V2: Improved Deep & Cross Network and Practical Lessons for Web-scale Learning to Rank Systems](https://arxiv.org/abs/2008.13535) :triangular_flag_on_post:**Google**                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DCNv2)        | `torch`       |
+        | 31  | CIKM'21           | [DESTINE](./model_zoo/DESTINE)           | [Disentangled Self-Attentive Neural Networks for Click-Through Rate Prediction](https://arxiv.org/abs/2101.03654) :triangular_flag_on_post:**Alibaba**                                                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DESTINE)      | `torch`       |
+        | 32  | CIKM'21           | [EDCN](./model_zoo/EDCN)                 | [Enhancing Explicit and Implicit Feature Interactions via Information Sharing for Parallel Deep CTR Models](https://dlp-kdd.github.io/assets/pdf/DLP-KDD_2021_paper_12.pdf) :triangular_flag_on_post:**Huawei** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/EDCN)         | `torch`       |
+        | 33  | DLP-KDD'21        | [MaskNet](./model_zoo/MaskNet)           | [MaskNet: Introducing Feature-Wise Multiplication to CTR Ranking Models by Instance-Guided Mask](https://arxiv.org/abs/2102.07619) :triangular_flag_on_post:**Sina Weibo**                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/MaskNet)      | `torch`       |
+        | 34  | SIGIR'21          | [SAM](./model_zoo/SAM)                   | [Looking at CTR Prediction Again: Is Attention All You Need?](https://arxiv.org/abs/2105.05563) :triangular_flag_on_post:**BOSS Zhipin**                                                                        | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/SAM)          | `torch`       |
+        | 35  | KDD'21            | [AOANet](./model_zoo/AOANet)             | [Architecture and Operation Adaptive Network for Online Recommendations](https://dl.acm.org/doi/10.1145/3447548.3467133) :triangular_flag_on_post:**Didi Chuxing**                                              | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/AOANet)       | `torch`       |
+        | 36  | AAAI'23           | [FinalMLP](./model_zoo/FinalMLP)         | [FinalMLP: An Enhanced Two-Stream MLP Model for CTR Prediction](https://arxiv.org/abs/2304.00902) :triangular_flag_on_post:**Huawei**                                                                                                               |     [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FinalMLP)         | `torch`       |
+        | 37  | SIGIR'23           | [FINAL](./model_zoo/FINAL)         | FINAL: Factorized Interaction Layer for CTR Prediction :triangular_flag_on_post:**Huawei**                                                                                                               |     [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FINAL)         | `torch`       |
         |     |                   |                                          | :point_down:**User Behavior Modeling**                                                                                                                                                                          |                                                                                                                 |               |
-        | 38  | KDD'18            | [DIN](./model_zoo/DIN)                   | [Deep Interest Network for Click-Through Rate Prediction](https://www.kdd.org/kdd2018/accepted-papers/view/deep-interest-network-for-click-through-rate-prediction) :triangular_flag_on_post:**Alibaba**        |                                                                                                                 | `torch`       |
-        | 39  | AAAI'19           | [DIEN](./model_zoo/DIEN)                 | [Deep Interest Evolution Network for Click-Through Rate Prediction](https://arxiv.org/abs/1809.03672) :triangular_flag_on_post:**Alibaba**                                                                      |                                                                                                                 | `torch`       |
-        | 40  | DLP-KDD'19        | [BST](./model_zoo/BST)                   | [Behavior Sequence Transformer for E-commerce Recommendation in Alibaba](https://arxiv.org/abs/1905.06874) :triangular_flag_on_post:**Alibaba**                                                                 |                                                                                                                 | `torch`       |
+        | 38  | KDD'18            | [DIN](./model_zoo/DIN)                   | [Deep Interest Network for Click-Through Rate Prediction](https://www.kdd.org/kdd2018/accepted-papers/view/deep-interest-network-for-click-through-rate-prediction) :triangular_flag_on_post:**Alibaba**        |   [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DIN)       | `torch`       |
+        | 39  | AAAI'19           | [DIEN](./model_zoo/DIEN)                 | [Deep Interest Evolution Network for Click-Through Rate Prediction](https://arxiv.org/abs/1809.03672) :triangular_flag_on_post:**Alibaba**                                                                      |   [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DIEN)        | `torch`       |
+        | 40  | DLP-KDD'19        | [BST](./model_zoo/BST)                   | [Behavior Sequence Transformer for E-commerce Recommendation in Alibaba](https://arxiv.org/abs/1905.06874) :triangular_flag_on_post:**Alibaba**                                                                 |  [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/BST)     | `torch`       |
         | 41  | CIKM'20           | [DMIN](./model_zoo/DMIN)                 | [Deep Multi-Interest Network for Click-through Rate Prediction](https://dl.acm.org/doi/10.1145/3340531.3412092) :triangular_flag_on_post:**Alibaba**                                                            |                                                                                                                 | `torch`       |
         | 42  | AAAI'20           | [DMR](./model_zoo/DMR)                   | [Deep Match to Rank Model for Personalized Click-Through Rate Prediction](https://ojs.aaai.org/index.php/AAAI/article/view/5346) :triangular_flag_on_post:**Alibaba**                                           |                                                                                                                 | `torch`       |
         | 43  | Arxiv'21          | [ETA](./model_zoo/ETA)                   | [End-to-End User Behavior Retrieval in Click-Through RatePrediction Model](https://arxiv.org/abs/2108.04468) :triangular_flag_on_post:**Alibaba**                                                               |                                                                                                                 | `torch`       |
         | 44  | CIKM'22           | [SDIM](./model_zoo/SDIM)                 | [Sampling Is All You Need on Modeling Long-Term User Behaviors for CTR Prediction](https://arxiv.org/abs/2205.10249) :triangular_flag_on_post:**Meituan**                                                       |                                                                                                                 | `torch`       |
+        |     |                   |                                          | :point_down:**Multi-Task Models**                                                                                                                                                                          |                                                                                                                 |               |
+        | 45  |     MachineLearn'97      | [SharedBottom](./model_zoo/multitask/SharedBottom)               | [Multitask Learning](https://link.springer.com/article/10.1023/A:1007379606734)                                                                                            |                                                                                                                 | `torch`       |
+        | 46  | KDD'18          | [MMoE](./model_zoo/multitask/MMOE)               | [Modeling Task Relationships in Multi-task Learning with Multi-Gate Mixture-of-Experts](https://dl.acm.org/doi/pdf/10.1145/3219819.3220007) :triangular_flag_on_post:**Google**                                                                                            |                                                                                                                 | `torch`       |
+        |     |                   |                                          | :point_down:**Multi-Domain Models**                                                                                                                                                                          |                                                                                                                 |               |
+        | 47  | Arxiv'23           | [PPNet](./model_zoo/PPNet)/PEPNet              | [PEPNet: Parameter and Embedding Personalized Network for Infusing with Personalized Prior Information](https://arxiv.org/abs/2302.01115) :triangular_flag_on_post:**KuaiShou**                                                                                            |                                                                                                                 | `torch`       |
+        
+        
+        + :point_right: See [reusable dataset splits for CTR prediction](https://openbenchmark.github.io/BARS/datasets/README.html).
+        + :point_right: See [benchmarking configurations and steps](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks).
+        + :point_right: See [the BARS benchmark leaderboard](https://openbenchmark.github.io/BARS/ctr_prediction/leaderboard/README.html#).
         
-        + :point_right: See [reusable dataset splits for CTR prediction](https://github.com/openbenchmark/BARS/blob/master/ctr_prediction/datasets).
-        + :point_right: See [benchmarking configurations and steps](https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks).
-        + :point_right: See [the BARS benchmark website](https://openbenchmark.github.io/ctr-prediction).
         
         ## Dependencies
         
         FuxiCTR has the following dependency requirements. 
         
         + python 3.6+
-        + pytorch 1.10+ (required only for torch models)
+        + pytorch 1.0/1.10+ (required only for torch models)
         + tensorflow 2.1+ (required only for tf models)
         
         Other packages can be installed via `pip install -r requirements.txt`.
         
         ## Quick Start
         
         1. Run the demo examples
@@ -120,19 +127,23 @@
         2. Run an existing model
            
             Users can easily run each model in the model zoo following the commands below, which is a demo for running DCN. In addition, users can modify the dataset config and model config files to run on their own datasets or with new hyper-parameters. More details can be found in the [readme file](./model_zoo/DCN/DCN_torch/README.md).
            
            ```
            cd model_zoo/DCN/DCN_torch
            python run_expid.py --expid DCN_test --gpu 0
+        
+           # Change `MODEL` according to the target model name
+           cd model_zoo/MODEL_PATH
+           python run_expid.py --expid MODEL_test --gpu 0
            ```
         
         3. Implement a new model
            
-            The FuxiCTR code structure is modularized, so that every part can be overwritten by users according to their needs. In many cases, only the model class needs to be implemented for a new customized model. If data preprocessing or data loader is not directly applicable, one can also overwrite a new one through the [core APIs](https://www.processon.com/view/link/63cfcfab4e30670eac4a81c7). A complete example can be found at [model_zoo/FinalMLP](./model_zoo/FinalMLP/), which implements our new model FinalMLP that has been recently published in AAAI 2023. Some other examples are also available in the model zoo.
+            The FuxiCTR code structure is modularized, so that every part can be overwritten by users according to their needs. In many cases, only the model class needs to be implemented for a new customized model. If data preprocessing or data loader is not directly applicable, one can also overwrite a new one through the [core APIs](https://www.processon.com/view/link/63cfcfab4e30670eac4a81c7). We show a concrete example which implements our new model [FinalMLP](https://github.com/xue-pai/FinalMLP) that has been recently published in AAAI 2023. More examples can be found in the [model zoo](./model_zoo/).
         
         
         ## Citation
         
         *:bell: If you find our code or benchmarks helpful in your research, please kindly cite the following papers.*
         
         > Jieming Zhu, Jinyang Liu, Shuai Yang, Qi Zhang, Xiuqiang He. [Open Benchmarking for Click-Through Rate Prediction](https://arxiv.org/abs/2009.05794). *The 30th ACM International Conference on Information and Knowledge Management (CIKM)*, 2021. [[Bibtex](https://dblp.org/rec/conf/cikm/ZhuLYZH21.html?view=bibtex)]
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fuxictr Version: 2.0.1 Summary: A configurable,
+Metadata-Version: 2.1 Name: fuxictr Version: 2.0.2 Summary: A configurable,
 tunable, and reproducible library for CTR prediction Home-page: https://
 github.com/xue-pai/FuxiCTR Author: zhujiem Author-email:
 zhujiem@users.noreply.github.com License: Apache-2.0 License Download-URL:
 https://github.com/xue-pai/FuxiCTR/tags Description:
                                     [Logo]
 [Python_version] [Pytorch_version] [Pytorch_version] [Pypi_version] [Downloads]
                           [License] [Wechat_QR_code]
@@ -24,211 +24,229 @@
 -------------------------------------------------------------------------------
 ----------------------------------------------------------------------- |:-----
 -------------------------------------------------------------------------------
 ---------------------------:|:-------------:| | | | | :point_down:**Feature
 Interaction Models** | | | | 1 | WWW'07 | [LR](./model_zoo/LR) | [Predicting
 Clicks: Estimating the Click-Through Rate for New Ads](https://dl.acm.org/
 citation.cfm?id=1242643) :triangular_flag_on_post:**Microsoft** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
 ctr_prediction/benchmarks/LR) | `torch` | | 2 | ICDM'10 | [FM](./model_zoo/FM)
 | [Factorization Machines](https://www.csie.ntu.edu.tw/~b97053/paper/
 Rendle2010FM.pdf) | [:arrow_upper_right:](https://github.com/openbenchmark/
-BARS/tree/master/ctr_prediction/benchmarks/FM) | `torch` | | 3 | CIKM'13 |
-[DSSM](./model_zoo/DSSM) | [Learning Deep Structured Semantic Models for Web
-Search using Clickthrough Data ](https://posenhuang.github.io/papers/
+BARS/tree/main/ctr_prediction/benchmarks/FM) | `torch` | | 3 | CIKM'13 | [DSSM]
+(./model_zoo/DSSM) | [Learning Deep Structured Semantic Models for Web Search
+using Clickthrough Data ](https://posenhuang.github.io/papers/
 cikm2013_DSSM_fullversion.pdf) :triangular_flag_on_post:**Microsoft** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
 ctr_prediction/benchmarks/DSSM) | `torch` | | 4 | CIKM'15 | [CCPM](./model_zoo/
 CCPM) | [A Convolutional Click Prediction Model](http://www.escience.cn/system/
 download/73676) | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/
-tree/master/ctr_prediction/benchmarks/CCPM) | `torch` | | 5 | RecSys'16 | [FFM]
+tree/main/ctr_prediction/benchmarks/CCPM) | `torch` | | 5 | RecSys'16 | [FFM]
 (./model_zoo/FFM) | [Field-aware Factorization Machines for CTR Prediction]
 (https://dl.acm.org/citation.cfm?id=2959134) :triangular_flag_on_post:
 **Criteo** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
-master/ctr_prediction/benchmarks/FFM) | `torch` | | 6 | RecSys'16 |
-[YoutubeDNN](./model_zoo/DNN) | [Deep Neural Networks for YouTube
-Recommendations](http://art.yale.edu/file_columns/0001/1132/covington.pdf) :
-triangular_flag_on_post:**Google** | [:arrow_upper_right:](https://github.com/
-openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DNN) | `torch`, `tf` |
-| 7 | DLRS'16 | [Wide&Deep](./model_zoo/WideDeep) | [Wide & Deep Learning for
-Recommender Systems](https://arxiv.org/pdf/1606.07792.pdf) :
-triangular_flag_on_post:**Google** | [:arrow_upper_right:](https://github.com/
-openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/WideDeep) | `torch`,
-`tf` | | 8 | ICDM'16 | [IPNN](./model_zoo/PNN) | [Product-based Neural Networks
-for User Response Prediction](https://arxiv.org/pdf/1611.00144.pdf) | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/IPNN) | `torch` | | 9 | KDD'16 | [DeepCrossing](./
-model_zoo/DeepCrossing) | [Deep Crossing: Web-Scale Modeling without Manually
-Crafted Combinatorial Features](https://www.kdd.org/kdd2016/papers/files/
-adf0975-shanA.pdf) :triangular_flag_on_post:**Microsoft** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/DeepCrossing) | `torch` | | 10 | NIPS'16 | [HOFM](./
-model_zoo/HOFM) | [Higher-Order Factorization Machines](https://papers.nips.cc/
-paper/6144-higher-order-factorization-machines.pdf) | [:arrow_upper_right:]
-(https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/
-HOFM) | `torch` | | 11 | IJCAI'17 | [DeepFM](./model_zoo/DeepFM) | [DeepFM: A
-Factorization-Machine based Neural Network for CTR Prediction](https://
-arxiv.org/abs/1703.04247) :triangular_flag_on_post:**Huawei** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/DeepFM) | `torch`, `tf` | | 12 | SIGIR'17 | [NFM](./
-model_zoo/NFM) | [Neural Factorization Machines for Sparse Predictive
-Analytics](https://dl.acm.org/citation.cfm?id=3080777) | [:arrow_upper_right:]
-(https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/
-NFM) | `torch` | | 13 | IJCAI'17 | [AFM](./model_zoo/AFM) | [Attentional
-Factorization Machines: Learning the Weight of Feature Interactions via
-Attention Networks](http://www.ijcai.org/proceedings/2017/0435.pdf) | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/AFM) | `torch` | | 14 | ADKDD'17 | [DCN](./model_zoo/
-DCN) | [Deep & Cross Network for Ad Click Predictions](https://arxiv.org/abs/
-1708.05123) :triangular_flag_on_post:**Google** | [:arrow_upper_right:](https:/
-/github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DCN) |
-`torch`, `tf` | | 15 | WWW'18 | [FwFM](./model_zoo/FwFM) | [Field-weighted
-Factorization Machines for Click-Through Rate Prediction in Display
-Advertising](https://arxiv.org/pdf/1806.03514.pdf) :triangular_flag_on_post:
-**Oath, TouchPal, LinkedIn, Alibaba** | [:arrow_upper_right:](https://
-github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/FwFM) |
-`torch` | | 16 | KDD'18 | [xDeepFM](./model_zoo/xDeepFM) | [xDeepFM: Combining
-Explicit and Implicit Feature Interactions for Recommender Systems](https://
-arxiv.org/pdf/1803.05170.pdf) :triangular_flag_on_post:**Microsoft** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/xDeepFM) | `torch` | | 17 | CIKM'19 | [FiGNN](./
-model_zoo/FiGNN) | [FiGNN: Modeling Feature Interactions via Graph Neural
-Networks for CTR Prediction](https://arxiv.org/abs/1910.05552) | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/FiGNN) | `torch` | | 18 | CIKM'19 | [AutoInt/
-AutoInt+](./model_zoo/AutoInt) | [AutoInt: Automatic Feature Interaction
-Learning via Self-Attentive Neural Networks](https://arxiv.org/abs/1810.11921)
-| [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/AutoInt) | `torch` | | 19 | RecSys'19 | [FiBiNET](./
-model_zoo/FiBiNET) | [FiBiNET: Combining Feature Importance and Bilinear
-feature Interaction for Click-Through Rate Prediction](https://arxiv.org/abs/
-1905.09433) :triangular_flag_on_post:**Sina Weibo** | [:arrow_upper_right:]
-(https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/
-FiBiNET) | `torch` | | 20 | WWW'19 | [FGCNN](./model_zoo/FGCNN) | [Feature
-Generation by Convolutional Neural Network for Click-Through Rate Prediction]
-(https://arxiv.org/abs/1904.04447) :triangular_flag_on_post:**Huawei** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/FGCNN) | `torch` | | 21 | AAAI'19 | [HFM/HFM+](./
-model_zoo/HFM) | [Holographic Factorization Machines for Recommendation](https:
-//ojs.aaai.org//index.php/AAAI/article/view/4448) | [:arrow_upper_right:]
-(https://github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/
-HFM) | `torch` | | 22 | Arxiv'19 | [DLRM](./model_zoo/DLRM) | [Deep Learning
-Recommendation Model for Personalization and Recommendation Systems](https://
-arxiv.org/abs/1906.00091) :triangular_flag_on_post:**Facebook** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/DLRM) | `torch` | | 23 | NeuralNetworks'20 | [ONN](./
-model_zoo/ONN) | [Operation-aware Neural Networks for User Response Prediction]
-(https://arxiv.org/pdf/1904.12579) | [:arrow_upper_right:](https://github.com/
-openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/ONN) | `torch` | | 24
-| AAAI'20 | [AFN/AFN+](./model_zoo/AFN) | [Adaptive Factorization Network:
-Learning Adaptive-Order Feature Interactions](https://ojs.aaai.org/index.php/
-AAAI/article/view/5768) | [:arrow_upper_right:](https://github.com/
-openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/AFN) | `torch` | | 25
-| AAAI'20 | [LorentzFM](./model_zoo/LorentzFM) | [Learning Feature Interactions
-with Lorentzian Factorization](https://arxiv.org/abs/1911.09821) :
-triangular_flag_on_post:**eBay** | [:arrow_upper_right:](https://github.com/
-openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/LorentzFM) | `torch` |
-| 26 | WSDM'20 | [InterHAt](./model_zoo/InterHAt) | [Interpretable Click-
-through Rate Prediction through Hierarchical Attention](https://dl.acm.org/doi/
-10.1145/3336191.3371785) :triangular_flag_on_post:**NEC Labs, Google** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/InterHAt) | `torch` | | 27 | DLP-KDD'20 | [FLEN](./
-model_zoo/FLEN) | [FLEN: Leveraging Field for Scalable CTR Prediction](https://
-arxiv.org/abs/1911.04690) :triangular_flag_on_post:**Tencent** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks/FLEN) | `torch` | | 28 | CIKM'20 | [DeepIM](./
-model_zoo/DeepIM) | [Deep Interaction Machine: A Simple but Effective Model for
-High-order Feature Interactions](https://dl.acm.org/doi/abs/10.1145/
-3340531.3412077) :triangular_flag_on_post:**Alibaba, RealAI** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
+main/ctr_prediction/benchmarks/FFM) | `torch` | | 6 | RecSys'16 | [DNN](./
+model_zoo/DNN) | [Deep Neural Networks for YouTube Recommendations](http://
+art.yale.edu/file_columns/0001/1132/covington.pdf) :triangular_flag_on_post:
+**Google** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
+main/ctr_prediction/benchmarks/DNN) | `torch`, `tf` | | 7 | DLRS'16 |
+[Wide&Deep](./model_zoo/WideDeep) | [Wide & Deep Learning for Recommender
+Systems](https://arxiv.org/pdf/1606.07792.pdf) :triangular_flag_on_post:
+**Google** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
+main/ctr_prediction/benchmarks/WideDeep) | `torch`, `tf` | | 8 | ICDM'16 |
+[IPNN](./model_zoo/PNN) | [Product-based Neural Networks for User Response
+Prediction](https://arxiv.org/pdf/1611.00144.pdf) | [:arrow_upper_right:]
+(https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/
+IPNN) | `torch` | | 9 | KDD'16 | [DeepCrossing](./model_zoo/DeepCrossing) |
+[Deep Crossing: Web-Scale Modeling without Manually Crafted Combinatorial
+Features](https://www.kdd.org/kdd2016/papers/files/adf0975-shanA.pdf) :
+triangular_flag_on_post:**Microsoft** | [:arrow_upper_right:](https://
+github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DeepCrossing)
+| `torch` | | 10 | NIPS'16 | [HOFM](./model_zoo/HOFM) | [Higher-Order
+Factorization Machines](https://papers.nips.cc/paper/6144-higher-order-
+factorization-machines.pdf) | [:arrow_upper_right:](https://github.com/
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/HOFM) | `torch` | | 11 |
+IJCAI'17 | [DeepFM](./model_zoo/DeepFM) | [DeepFM: A Factorization-Machine
+based Neural Network for CTR Prediction](https://arxiv.org/abs/1703.04247) :
+triangular_flag_on_post:**Huawei** | [:arrow_upper_right:](https://github.com/
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DeepFM) | `torch`, `tf`
+| | 12 | SIGIR'17 | [NFM](./model_zoo/NFM) | [Neural Factorization Machines for
+Sparse Predictive Analytics](https://dl.acm.org/citation.cfm?id=3080777) | [:
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/NFM) | `torch` | | 13 | IJCAI'17 | [AFM](./model_zoo/
+AFM) | [Attentional Factorization Machines: Learning the Weight of Feature
+Interactions via Attention Networks](http://www.ijcai.org/proceedings/2017/
+0435.pdf) | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
+main/ctr_prediction/benchmarks/AFM) | `torch` | | 14 | ADKDD'17 | [DCN](./
+model_zoo/DCN) | [Deep & Cross Network for Ad Click Predictions](https://
+arxiv.org/abs/1708.05123) :triangular_flag_on_post:**Google** | [:
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/DCN) | `torch`, `tf` | | 15 | WWW'18 | [FwFM](./
+model_zoo/FwFM) | [Field-weighted Factorization Machines for Click-Through Rate
+Prediction in Display Advertising](https://arxiv.org/pdf/1806.03514.pdf) :
+triangular_flag_on_post:**Oath, TouchPal, LinkedIn, Alibaba** | [:
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/FwFM) | `torch` | | 16 | KDD'18 | [xDeepFM](./
+model_zoo/xDeepFM) | [xDeepFM: Combining Explicit and Implicit Feature
+Interactions for Recommender Systems](https://arxiv.org/pdf/1803.05170.pdf) :
+triangular_flag_on_post:**Microsoft** | [:arrow_upper_right:](https://
+github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/xDeepFM) |
+`torch` | | 17 | CIKM'19 | [FiGNN](./model_zoo/FiGNN) | [FiGNN: Modeling
+Feature Interactions via Graph Neural Networks for CTR Prediction](https://
+arxiv.org/abs/1910.05552) | [:arrow_upper_right:](https://github.com/
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FiGNN) | `torch` | | 18
+| CIKM'19 | [AutoInt/AutoInt+](./model_zoo/AutoInt) | [AutoInt: Automatic
+Feature Interaction Learning via Self-Attentive Neural Networks](https://
+arxiv.org/abs/1810.11921) | [:arrow_upper_right:](https://github.com/
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/AutoInt) | `torch` | |
+19 | RecSys'19 | [FiBiNET](./model_zoo/FiBiNET) | [FiBiNET: Combining Feature
+Importance and Bilinear feature Interaction for Click-Through Rate Prediction]
+(https://arxiv.org/abs/1905.09433) :triangular_flag_on_post:**Sina Weibo** | [:
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/FiBiNET) | `torch` | | 20 | WWW'19 | [FGCNN](./
+model_zoo/FGCNN) | [Feature Generation by Convolutional Neural Network for
+Click-Through Rate Prediction](https://arxiv.org/abs/1904.04447) :
+triangular_flag_on_post:**Huawei** | [:arrow_upper_right:](https://github.com/
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FGCNN) | `torch` | | 21
+| AAAI'19 | [HFM/HFM+](./model_zoo/HFM) | [Holographic Factorization Machines
+for Recommendation](https://ojs.aaai.org//index.php/AAAI/article/view/4448) |
+[:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/HFM) | `torch` | | 22 | Arxiv'19 | [DLRM](./
+model_zoo/DLRM) | [Deep Learning Recommendation Model for Personalization and
+Recommendation Systems](https://arxiv.org/abs/1906.00091) :
+triangular_flag_on_post:**Facebook** | [:arrow_upper_right:](https://
+github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DLRM) |
+`torch` | | 23 | NeuralNetworks'20 | [ONN](./model_zoo/ONN) | [Operation-aware
+Neural Networks for User Response Prediction](https://arxiv.org/pdf/1904.12579)
+| [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/ONN) | `torch` | | 24 | AAAI'20 | [AFN/AFN+](./
+model_zoo/AFN) | [Adaptive Factorization Network: Learning Adaptive-Order
+Feature Interactions](https://ojs.aaai.org/index.php/AAAI/article/view/5768) |
+[:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/AFN) | `torch` | | 25 | AAAI'20 | [LorentzFM](./
+model_zoo/LorentzFM) | [Learning Feature Interactions with Lorentzian
+Factorization](https://arxiv.org/abs/1911.09821) :triangular_flag_on_post:
+**eBay** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
+main/ctr_prediction/benchmarks/LorentzFM) | `torch` | | 26 | WSDM'20 |
+[InterHAt](./model_zoo/InterHAt) | [Interpretable Click-through Rate Prediction
+through Hierarchical Attention](https://dl.acm.org/doi/10.1145/3336191.3371785)
+:triangular_flag_on_post:**NEC Labs, Google** | [:arrow_upper_right:](https://
+github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/InterHAt) |
+`torch` | | 27 | DLP-KDD'20 | [FLEN](./model_zoo/FLEN) | [FLEN: Leveraging
+Field for Scalable CTR Prediction](https://arxiv.org/abs/1911.04690) :
+triangular_flag_on_post:**Tencent** | [:arrow_upper_right:](https://github.com/
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FLEN) | `torch` | | 28 |
+CIKM'20 | [DeepIM](./model_zoo/DeepIM) | [Deep Interaction Machine: A Simple
+but Effective Model for High-order Feature Interactions](https://dl.acm.org/
+doi/abs/10.1145/3340531.3412077) :triangular_flag_on_post:**Alibaba, RealAI** |
+[:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
 ctr_prediction/benchmarks/DeepIM) | `torch` | | 29 | WWW'21 | [FmFM](./
 model_zoo/FmFM) | [FM^2: Field-matrixed Factorization Machines for Recommender
 Systems](https://arxiv.org/abs/2102.12994) :triangular_flag_on_post:**Yahoo** |
-[:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
+[:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
 ctr_prediction/benchmarks/FmFM) | `torch` | | 30 | WWW'21 | [DCN-V2](./
 model_zoo/DCNv2) | [DCN V2: Improved Deep & Cross Network and Practical Lessons
 for Web-scale Learning to Rank Systems](https://arxiv.org/abs/2008.13535) :
 triangular_flag_on_post:**Google** | [:arrow_upper_right:](https://github.com/
-openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DCNv2) | `torch` | |
-31 | CIKM'21 | [DESTINE](./model_zoo/DESTINE) | [Disentangled Self-Attentive
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DCNv2) | `torch` | | 31
+| CIKM'21 | [DESTINE](./model_zoo/DESTINE) | [Disentangled Self-Attentive
 Neural Networks for Click-Through Rate Prediction](https://arxiv.org/abs/
 2101.03654) :triangular_flag_on_post:**Alibaba** | [:arrow_upper_right:](https:
-//github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/DESTINE)
-| `torch` | | 32 | CIKM'21 | [EDCN](./model_zoo/EDCN) | [Enhancing Explicit and
+//github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DESTINE) |
+`torch` | | 32 | CIKM'21 | [EDCN](./model_zoo/EDCN) | [Enhancing Explicit and
 Implicit Feature Interactions via Information Sharing for Parallel Deep CTR
 Models](https://dlp-kdd.github.io/assets/pdf/DLP-KDD_2021_paper_12.pdf) :
 triangular_flag_on_post:**Huawei** | [:arrow_upper_right:](https://github.com/
-openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/EDCN) | `torch` | | 33
-| DLP-KDD'21 | [MaskNet](./model_zoo/MaskNet) | [MaskNet: Introducing Feature-
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/EDCN) | `torch` | | 33 |
+DLP-KDD'21 | [MaskNet](./model_zoo/MaskNet) | [MaskNet: Introducing Feature-
 Wise Multiplication to CTR Ranking Models by Instance-Guided Mask](https://
 arxiv.org/abs/2102.07619) :triangular_flag_on_post:**Sina Weibo** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
 ctr_prediction/benchmarks/MaskNet) | `torch` | | 34 | SIGIR'21 | [SAM](./
 model_zoo/SAM) | [Looking at CTR Prediction Again: Is Attention All You Need?]
 (https://arxiv.org/abs/2105.05563) :triangular_flag_on_post:**BOSS Zhipin** |
-[:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/master/
+[:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
 ctr_prediction/benchmarks/SAM) | `torch` | | 35 | KDD'21 | [AOANet](./
 model_zoo/AOANet) | [Architecture and Operation Adaptive Network for Online
 Recommendations](https://dl.acm.org/doi/10.1145/3447548.3467133) :
 triangular_flag_on_post:**Didi Chuxing** | [:arrow_upper_right:](https://
-github.com/openbenchmark/BARS/tree/master/ctr_prediction/benchmarks/AOANet) |
-`torch` | | 36 | Blog'21 | [PPNet](./model_zoo/PPNet) | [Parameter Personalized
-Net](https://www.jiqizhixin.com/articles/2021-02-03-6) :
-triangular_flag_on_post:**KuaiShou** | | `torch` | | 37 | AAAI'23 | [FinalMLP]
-(./model_zoo/FinalMLP) | FinalMLP: An Enhanced Two-Stream MLP Model for CTR
-PredictionÂ :triangular_flag_on_post:**Huawei** | | `torch` | | | | | :
-point_down:**User Behavior Modeling** | | | | 38 | KDD'18 | [DIN](./model_zoo/
-DIN) | [Deep Interest Network for Click-Through Rate Prediction](https://
-www.kdd.org/kdd2018/accepted-papers/view/deep-interest-network-for-click-
-through-rate-prediction) :triangular_flag_on_post:**Alibaba** | | `torch` | |
-39 | AAAI'19 | [DIEN](./model_zoo/DIEN) | [Deep Interest Evolution Network for
-Click-Through Rate Prediction](https://arxiv.org/abs/1809.03672)Â :
-triangular_flag_on_post:**Alibaba** | | `torch` | | 40 | DLP-KDD'19 | [BST](./
-model_zoo/BST) | [Behavior Sequence Transformer for E-commerce Recommendation
-in Alibaba](https://arxiv.org/abs/1905.06874)Â :triangular_flag_on_post:
-**Alibaba** | | `torch` | | 41 | CIKM'20 | [DMIN](./model_zoo/DMIN) | [Deep
-Multi-Interest Network for Click-through Rate Prediction](https://dl.acm.org/
-doi/10.1145/3340531.3412092)Â :triangular_flag_on_post:**Alibaba** | | `torch`
-| | 42 | AAAI'20 | [DMR](./model_zoo/DMR) | [Deep Match to Rank Model for
-Personalized Click-Through Rate Prediction](https://ojs.aaai.org/index.php/
-AAAI/article/view/5346)Â :triangular_flag_on_post:**Alibaba** | | `torch` | |
-43 | Arxiv'21 | [ETA](./model_zoo/ETA) | [End-to-End User Behavior Retrieval in
-Click-Through RatePrediction Model](https://arxiv.org/abs/2108.04468)Â :
+github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/AOANet) |
+`torch` | | 36 | AAAI'23 | [FinalMLP](./model_zoo/FinalMLP) | [FinalMLP: An
+Enhanced Two-Stream MLP Model for CTR Prediction](https://arxiv.org/abs/
+2304.00902)Â :triangular_flag_on_post:**Huawei** | [:arrow_upper_right:](https:
+//github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FinalMLP) |
+`torch` | | 37 | SIGIR'23 | [FINAL](./model_zoo/FINAL) | FINAL: Factorized
+Interaction Layer for CTR PredictionÂ :triangular_flag_on_post:**Huawei** | [:
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/FINAL) | `torch` | | | | | :point_down:**User
+Behavior Modeling** | | | | 38 | KDD'18 | [DIN](./model_zoo/DIN) | [Deep
+Interest Network for Click-Through Rate Prediction](https://www.kdd.org/
+kdd2018/accepted-papers/view/deep-interest-network-for-click-through-rate-
+prediction) :triangular_flag_on_post:**Alibaba** | [:arrow_upper_right:](https:
+//github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DIN) |
+`torch` | | 39 | AAAI'19 | [DIEN](./model_zoo/DIEN) | [Deep Interest Evolution
+Network for Click-Through Rate Prediction](https://arxiv.org/abs/1809.03672)Â :
+triangular_flag_on_post:**Alibaba** | [:arrow_upper_right:](https://github.com/
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DIEN) | `torch` | | 40 |
+DLP-KDD'19 | [BST](./model_zoo/BST) | [Behavior Sequence Transformer for E-
+commerce Recommendation in Alibaba](https://arxiv.org/abs/1905.06874)Â :
+triangular_flag_on_post:**Alibaba** | [:arrow_upper_right:](https://github.com/
+openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/BST) | `torch` | | 41 |
+CIKM'20 | [DMIN](./model_zoo/DMIN) | [Deep Multi-Interest Network for Click-
+through Rate Prediction](https://dl.acm.org/doi/10.1145/3340531.3412092)Â :
+triangular_flag_on_post:**Alibaba** | | `torch` | | 42 | AAAI'20 | [DMR](./
+model_zoo/DMR) | [Deep Match to Rank Model for Personalized Click-Through Rate
+Prediction](https://ojs.aaai.org/index.php/AAAI/article/view/5346)Â :
+triangular_flag_on_post:**Alibaba** | | `torch` | | 43 | Arxiv'21 | [ETA](./
+model_zoo/ETA) | [End-to-End User Behavior Retrieval in Click-Through
+RatePrediction Model](https://arxiv.org/abs/2108.04468)Â :
 triangular_flag_on_post:**Alibaba** | | `torch` | | 44 | CIKM'22 | [SDIM](./
 model_zoo/SDIM) | [Sampling Is All You Need on Modeling Long-Term User
 Behaviors for CTR Prediction](https://arxiv.org/abs/2205.10249)Â :
-triangular_flag_on_post:**Meituan** | | `torch` | + :point_right: See [reusable
-dataset splits for CTR prediction](https://github.com/openbenchmark/BARS/blob/
-master/ctr_prediction/datasets). + :point_right: See [benchmarking
-configurations and steps](https://github.com/openbenchmark/BARS/tree/master/
-ctr_prediction/benchmarks). + :point_right: See [the BARS benchmark website]
-(https://openbenchmark.github.io/ctr-prediction). ## Dependencies FuxiCTR has
-the following dependency requirements. + python 3.6+ + pytorch 1.10+ (required
-only for torch models) + tensorflow 2.1+ (required only for tf models) Other
-packages can be installed via `pip install -r requirements.txt`. ## Quick Start
-1. Run the demo examples Examples are provided in the demo directory to show
-some basic usage of FuxiCTR. Users can run the examples for quick start and to
-understand the workflow. ``` cd demo python example1_build_dataset_to_h5.py
-python example2_DeepFM_with_h5_input.py ``` 2. Run an existing model Users can
-easily run each model in the model zoo following the commands below, which is a
-demo for running DCN. In addition, users can modify the dataset config and
-model config files to run on their own datasets or with new hyper-parameters.
-More details can be found in the [readme file](./model_zoo/DCN/DCN_torch/
-README.md). ``` cd model_zoo/DCN/DCN_torch python run_expid.py --expid DCN_test
---gpu 0 ``` 3. Implement a new model The FuxiCTR code structure is modularized,
-so that every part can be overwritten by users according to their needs. In
-many cases, only the model class needs to be implemented for a new customized
-model. If data preprocessing or data loader is not directly applicable, one can
-also overwrite a new one through the [core APIs](https://www.processon.com/
-view/link/63cfcfab4e30670eac4a81c7). A complete example can be found at
-[model_zoo/FinalMLP](./model_zoo/FinalMLP/), which implements our new model
-FinalMLP that has been recently published in AAAI 2023. Some other examples are
-also available in the model zoo. ## Citation *:bell: If you find our code or
-benchmarks helpful in your research, please kindly cite the following papers.*
-> Jieming Zhu, Jinyang Liu, Shuai Yang, Qi Zhang, Xiuqiang He. [Open
+triangular_flag_on_post:**Meituan** | | `torch` | | | | | :point_down:**Multi-
+Task Models** | | | | 45 | MachineLearn'97 | [SharedBottom](./model_zoo/
+multitask/SharedBottom) | [Multitask Learning](https://link.springer.com/
+article/10.1023/A:1007379606734) | | `torch` | | 46 | KDD'18 | [MMoE](./
+model_zoo/multitask/MMOE) | [Modeling Task Relationships in Multi-task Learning
+with Multi-Gate Mixture-of-Experts](https://dl.acm.org/doi/pdf/10.1145/
+3219819.3220007) :triangular_flag_on_post:**Google** | | `torch` | | | | | :
+point_down:**Multi-Domain Models** | | | | 47 | Arxiv'23 | [PPNet](./model_zoo/
+PPNet)/PEPNet | [PEPNet: Parameter and Embedding Personalized Network for
+Infusing with Personalized Prior Information](https://arxiv.org/abs/2302.01115)
+:triangular_flag_on_post:**KuaiShou** | | `torch` | + :point_right: See
+[reusable dataset splits for CTR prediction](https://openbenchmark.github.io/
+BARS/datasets/README.html). + :point_right: See [benchmarking configurations
+and steps](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/
+benchmarks). + :point_right: See [the BARS benchmark leaderboard](https://
+openbenchmark.github.io/BARS/ctr_prediction/leaderboard/README.html#). ##
+Dependencies FuxiCTR has the following dependency requirements. + python 3.6+ +
+pytorch 1.0/1.10+ (required only for torch models) + tensorflow 2.1+ (required
+only for tf models) Other packages can be installed via `pip install -
+r requirements.txt`. ## Quick Start 1. Run the demo examples Examples are
+provided in the demo directory to show some basic usage of FuxiCTR. Users can
+run the examples for quick start and to understand the workflow. ``` cd demo
+python example1_build_dataset_to_h5.py python example2_DeepFM_with_h5_input.py
+``` 2. Run an existing model Users can easily run each model in the model zoo
+following the commands below, which is a demo for running DCN. In addition,
+users can modify the dataset config and model config files to run on their own
+datasets or with new hyper-parameters. More details can be found in the [readme
+file](./model_zoo/DCN/DCN_torch/README.md). ``` cd model_zoo/DCN/DCN_torch
+python run_expid.py --expid DCN_test --gpu 0 # Change `MODEL` according to the
+target model name cd model_zoo/MODEL_PATH python run_expid.py --expid
+MODEL_test --gpu 0 ``` 3. Implement a new model The FuxiCTR code structure is
+modularized, so that every part can be overwritten by users according to their
+needs. In many cases, only the model class needs to be implemented for a new
+customized model. If data preprocessing or data loader is not directly
+applicable, one can also overwrite a new one through the [core APIs](https://
+www.processon.com/view/link/63cfcfab4e30670eac4a81c7). We show a concrete
+example which implements our new model [FinalMLP](https://github.com/xue-pai/
+FinalMLP) that has been recently published in AAAI 2023. More examples can be
+found in the [model zoo](./model_zoo/). ## Citation *:bell: If you find our
+code or benchmarks helpful in your research, please kindly cite the following
+papers.* > Jieming Zhu, Jinyang Liu, Shuai Yang, Qi Zhang, Xiuqiang He. [Open
 Benchmarking for Click-Through Rate Prediction](https://arxiv.org/abs/
 2009.05794). *The 30th ACM International Conference on Information and
 Knowledge Management (CIKM)*, 2021. [[Bibtex](https://dblp.org/rec/conf/cikm/
 ZhuLYZH21.html?view=bibtex)] > Jieming Zhu, Quanyu Dai, Liangcai Su, Rong Ma,
 Jinyang Liu, Guohao Cai, Xi Xiao, Rui Zhang. [BARS: Towards Open Benchmarking
 for Recommender Systems](https://arxiv.org/abs/2205.09626). *The 45th
 International ACM SIGIR Conference on Research and Development in Information
```

### Comparing `fuxictr-2.0.1/fuxictr.egg-info/SOURCES.txt` & `fuxictr-2.0.2/fuxictr.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -40,17 +40,17 @@
 fuxictr/pytorch/layers/interactions/__init__.py
 fuxictr/pytorch/layers/interactions/bilinear_interaction.py
 fuxictr/pytorch/layers/interactions/compressed_interaction_net.py
 fuxictr/pytorch/layers/interactions/cross_net.py
 fuxictr/pytorch/layers/interactions/holographic_interaction.py
 fuxictr/pytorch/layers/interactions/inner_product.py
 fuxictr/pytorch/layers/interactions/interaction_machine.py
-fuxictr/pytorch/models/DNN.py
 fuxictr/pytorch/models/__init__.py
-fuxictr/pytorch/models/base_model.py
+fuxictr/pytorch/models/ctr_model.py
+fuxictr/pytorch/models/multitask_model.py
 fuxictr/tensorflow/__init__.py
 fuxictr/tensorflow/tf_utils.py
 fuxictr/tensorflow/dataloaders/__init__.py
 fuxictr/tensorflow/dataloaders/tf_dataloader.py
 fuxictr/tensorflow/layers/__init__.py
 fuxictr/tensorflow/layers/pooling.py
 fuxictr/tensorflow/layers/blocks/__init__.py
@@ -59,11 +59,11 @@
 fuxictr/tensorflow/layers/blocks/logistic_regression.py
 fuxictr/tensorflow/layers/blocks/mlp_block.py
 fuxictr/tensorflow/layers/embeddings/__init__.py
 fuxictr/tensorflow/layers/embeddings/feature_embedding.py
 fuxictr/tensorflow/layers/interactions/__init__.py
 fuxictr/tensorflow/layers/interactions/cross_net.py
 fuxictr/tensorflow/layers/interactions/inner_product.py
-fuxictr/tensorflow/models/DNN.py
 fuxictr/tensorflow/models/__init__.py
-fuxictr/tensorflow/models/base_model.py
-model_zoo/__init__.py
+fuxictr/tensorflow/models/ctr_model.py
+model_zoo/__init__.py
+model_zoo/multitask/__init__.py
```

### Comparing `fuxictr-2.0.1/model_zoo/__init__.py` & `fuxictr-2.0.2/model_zoo/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,8 +37,9 @@
 from .NFM.src import NFM
 from .ONN.src import ONN, ONNv2
 from .PNN.src import PNN
 from .PPNet.src import PPNet
 from .SAM.src import SAM
 from .SDIM.src import SDIM
 from .WideDeep.WideDeep_torch.src import WideDeep
-from .xDeepFM.src import xDeepFM
+from .xDeepFM.src import xDeepFM
+from .multitask import SharedBottom, MMoE
```

### Comparing `fuxictr-2.0.1/setup.py` & `fuxictr-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 setuptools.setup(
     name="fuxictr",
-    version="2.0.1",
+    version="2.0.2",
     author="zhujiem",
     author_email="zhujiem@users.noreply.github.com",
     description="A configurable, tunable, and reproducible library for CTR prediction",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xue-pai/FuxiCTR",
     download_url='https://github.com/xue-pai/FuxiCTR/tags',
```

