# Comparing `tmp/timm-0.9.1.tar.gz` & `tmp/timm-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timm-0.9.1.tar", last modified: Fri May 12 16:50:57 2023, max compression
+gzip compressed data, was "timm-0.9.2.tar", last modified: Sun May 14 15:04:59 2023, max compression
```

## Comparing `timm-0.9.1.tar` & `timm-0.9.2.tar`

### file list

```diff
@@ -1,272 +1,272 @@
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-12 16:50:57.161242 timm-0.9.1/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    11343 2023-02-24 22:35:42.000000 timm-0.9.1/LICENSE
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)       95 2023-03-31 00:49:24.000000 timm-0.9.1/MANIFEST.in
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    68314 2023-05-12 16:50:57.165243 timm-0.9.1/PKG-INFO
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    67196 2023-05-11 22:52:53.000000 timm-0.9.1/README.md
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      551 2023-03-31 00:49:24.000000 timm-0.9.1/pyproject.toml
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      126 2023-05-12 16:50:57.165243 timm-0.9.1/setup.cfg
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1935 2023-03-31 00:49:24.000000 timm-0.9.1/setup.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-12 16:50:57.145242 timm-0.9.1/timm/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      292 2023-03-31 00:49:24.000000 timm-0.9.1/timm/__init__.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-12 16:50:57.145242 timm-0.9.1/timm/data/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      819 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/__init__.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-12 16:50:57.149242 timm-0.9.1/timm/data/_info/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   118210 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/_info/imagenet12k_synsets.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   218430 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/_info/imagenet21k_goog_synsets.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    64070 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/_info/imagenet21k_goog_to_12k_indices.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   119937 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/_info/imagenet21k_goog_to_22k_indices.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   112210 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/_info/imagenet21k_miil_synsets.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   104500 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/_info/imagenet21k_miil_w21_synsets.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   218410 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/_info/imagenet22k_ms_synsets.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    63625 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/_info/imagenet22k_ms_to_12k_indices.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   119938 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/_info/imagenet22k_ms_to_22k_indices.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   218410 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/_info/imagenet22k_synsets.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    64070 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/_info/imagenet22k_to_12k_indices.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      774 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/_info/imagenet_a_indices.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2000 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/_info/imagenet_a_synsets.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      769 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/_info/imagenet_r_indices.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2000 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/_info/imagenet_r_synsets.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   388478 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/_info/imagenet_real_labels.json
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)  1748917 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/_info/imagenet_synset_to_definition.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   741457 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/_info/imagenet_synset_to_lemma.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    10000 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/_info/imagenet_synsets.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    35550 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/auto_augment.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4531 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/config.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      442 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/constants.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5833 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/dataset.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6989 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/dataset_factory.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2391 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/dataset_info.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5540 2023-02-24 22:35:42.000000 timm-0.9.1/timm/data/distributed_sampler.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4167 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/imagenet_info.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    11849 2023-04-28 20:49:14.000000 timm-0.9.1/timm/data/loader.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    14640 2023-05-10 22:09:19.000000 timm-0.9.1/timm/data/mixup.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4964 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/random_erasing.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-12 16:50:57.149242 timm-0.9.1/timm/data/readers/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)       72 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/readers/__init__.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      895 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/readers/class_map.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1482 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/readers/img_extensions.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      487 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/readers/reader.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1364 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/readers/reader_factory.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2431 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/readers/reader_hfds.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3315 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/readers/reader_image_folder.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     9182 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/readers/reader_image_in_tar.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2644 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/readers/reader_image_tar.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    17858 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/readers/reader_tfds.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    16724 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/readers/reader_wds.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      303 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/readers/shared_count.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1800 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/real_labels.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     9169 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/tf_preprocessing.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    11992 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/transforms.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     9840 2023-03-31 00:49:24.000000 timm-0.9.1/timm/data/transforms_factory.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-12 16:50:57.153242 timm-0.9.1/timm/layers/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3611 2023-05-10 14:38:22.000000 timm-0.9.1/timm/layers/__init__.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4468 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/activations.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2529 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/activations_jit.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5886 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/activations_me.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6310 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/adaptive_avgmax_pool.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4934 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/attention_pool2d.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1594 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/blur_pool.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6895 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/bottleneck_attn.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4426 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/cbam.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     7486 2023-04-28 20:49:14.000000 timm-0.9.1/timm/layers/classifier.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5199 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/cond_conv2d.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4175 2023-04-12 15:57:13.000000 timm-0.9.1/timm/layers/config.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3216 2023-04-28 20:49:14.000000 timm-0.9.1/timm/layers/conv2d_same.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3836 2023-04-28 20:49:14.000000 timm-0.9.1/timm/layers/conv_bn_act.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5320 2023-04-28 20:49:14.000000 timm-0.9.1/timm/layers/create_act.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3514 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/create_attn.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1622 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/create_conv2d.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1740 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/create_norm.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3748 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/create_norm_act.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6872 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/drop.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6386 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/eca.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    13862 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/evo_norm.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4008 2023-05-10 14:38:22.000000 timm-0.9.1/timm/layers/fast_norm.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2540 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/filter_response_norm.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1109 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/format.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3824 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/gather_excite.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2445 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/global_context.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1319 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/grn.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    10662 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/halo_attn.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1053 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/helpers.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3374 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/inplace_abn.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5941 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/lambda_layer.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      743 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/linear.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1737 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/median_pool.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1843 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/mixed_conv2d.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     7008 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/ml_decoder.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     8470 2023-05-10 14:38:22.000000 timm-0.9.1/timm/layers/mlp.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6218 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/non_local_attn.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6040 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/norm.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    17418 2023-04-28 20:49:14.000000 timm-0.9.1/timm/layers/norm_act.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2877 2023-04-28 20:49:14.000000 timm-0.9.1/timm/layers/padding.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1741 2023-04-12 15:57:13.000000 timm-0.9.1/timm/layers/patch_dropout.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     8516 2023-05-10 14:38:22.000000 timm-0.9.1/timm/layers/patch_embed.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3045 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/pool2d_same.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1678 2023-05-10 14:38:22.000000 timm-0.9.1/timm/layers/pos_embed.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    11764 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/pos_embed_rel.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    14314 2023-04-28 20:49:14.000000 timm-0.9.1/timm/layers/pos_embed_sincos.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5387 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/selective_kernel.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2620 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/separable_conv.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1775 2023-04-28 20:49:14.000000 timm-0.9.1/timm/layers/space_to_depth.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3076 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/split_attn.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3441 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/split_batchnorm.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4327 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/squeeze_excite.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5887 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/std_conv.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1996 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/test_time_pool.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      335 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/trace_utils.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4765 2023-03-31 00:49:24.000000 timm-0.9.1/timm/layers/weight_init.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-12 16:50:57.153242 timm-0.9.1/timm/loss/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      245 2023-02-24 22:35:42.000000 timm-0.9.1/timm/loss/__init__.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3343 2023-03-31 00:49:24.000000 timm-0.9.1/timm/loss/asymmetric_loss.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2030 2023-02-24 22:35:42.000000 timm-0.9.1/timm/loss/binary_cross_entropy.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1145 2023-02-24 22:35:42.000000 timm-0.9.1/timm/loss/cross_entropy.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1595 2023-02-24 22:35:42.000000 timm-0.9.1/timm/loss/jsd.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-12 16:50:57.161242 timm-0.9.1/timm/models/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3020 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/__init__.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18037 2023-05-10 22:09:19.000000 timm-0.9.1/timm/models/_builder.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    12148 2023-03-31 00:49:24.000000 timm-0.9.1/timm/models/_efficientnet_blocks.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    19879 2023-03-31 00:49:24.000000 timm-0.9.1/timm/models/_efficientnet_builder.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5069 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/_factory.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    15488 2023-03-31 00:49:24.000000 timm-0.9.1/timm/models/_features.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4743 2023-03-31 00:49:24.000000 timm-0.9.1/timm/models/_features_fx.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5940 2023-03-31 00:49:24.000000 timm-0.9.1/timm/models/_helpers.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    15370 2023-04-28 20:49:14.000000 timm-0.9.1/timm/models/_hub.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    10503 2023-03-31 00:49:24.000000 timm-0.9.1/timm/models/_manipulate.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3525 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/_pretrained.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4171 2023-03-31 00:49:24.000000 timm-0.9.1/timm/models/_prune.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-12 16:50:57.161242 timm-0.9.1/timm/models/_pruned/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     8734 2023-03-31 00:49:24.000000 timm-0.9.1/timm/models/_pruned/ecaresnet101d_pruned.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4520 2023-03-31 00:49:24.000000 timm-0.9.1/timm/models/_pruned/ecaresnet50d_pruned.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18596 2023-03-31 00:49:24.000000 timm-0.9.1/timm/models/_pruned/efficientnet_b1_pruned.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18676 2023-03-31 00:49:24.000000 timm-0.9.1/timm/models/_pruned/efficientnet_b2_pruned.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    21133 2023-03-31 00:49:24.000000 timm-0.9.1/timm/models/_pruned/efficientnet_b3_pruned.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    13506 2023-04-06 15:39:02.000000 timm-0.9.1/timm/models/_registry.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    23936 2023-05-12 16:50:51.000000 timm-0.9.1/timm/models/beit.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18985 2023-05-11 22:52:53.000000 timm-0.9.1/timm/models/byoanet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    68705 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/byobnet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18106 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/cait.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    29712 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/coat.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    15301 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/convit.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4473 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/convmixer.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    49685 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/convnext.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    24271 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/crossvit.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    40028 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/cspnet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    23064 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/davit.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18657 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/deit.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    15634 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/densenet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18599 2023-05-10 22:09:19.000000 timm-0.9.1/timm/models/dla.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    13621 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/dpn.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    21277 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/edgenext.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18911 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/efficientformer.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    24873 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/efficientformer_v2.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   101929 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/efficientnet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    39675 2023-05-12 16:50:51.000000 timm-0.9.1/timm/models/eva.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      150 2023-03-31 00:49:24.000000 timm-0.9.1/timm/models/factory.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      151 2023-03-31 00:49:24.000000 timm-0.9.1/timm/models/features.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    24033 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/focalnet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      154 2023-03-31 00:49:24.000000 timm-0.9.1/timm/models/fx_features.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    21393 2023-05-10 22:09:19.000000 timm-0.9.1/timm/models/gcvit.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    10473 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/ghostnet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     7697 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/hardcorenas.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      223 2023-03-31 00:49:24.000000 timm-0.9.1/timm/models/helpers.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    32902 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/hrnet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      145 2023-03-31 00:49:24.000000 timm-0.9.1/timm/models/hub.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    12077 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/inception_resnet_v2.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    17104 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/inception_v3.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    11076 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/inception_v4.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-12 16:50:57.161242 timm-0.9.1/timm/models/layers/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3432 2023-05-11 22:52:53.000000 timm-0.9.1/timm/models/layers/__init__.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    32443 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/levit.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    84448 2023-05-11 22:52:53.000000 timm-0.9.1/timm/models/maxxvit.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    35028 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/metaformer.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    24231 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/mlp_mixer.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    30795 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/mobilenetv3.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    25734 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/mobilevit.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    35530 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/mvitv2.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    26627 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/nasnet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    21489 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/nest.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    41085 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/nfnet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    14946 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/pit.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    15389 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/pnasnet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    17261 2023-05-10 22:09:19.000000 timm-0.9.1/timm/models/pvt_v2.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      151 2023-03-31 00:49:24.000000 timm-0.9.1/timm/models/registry.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    44020 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/regnet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     7691 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/res2net.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     9635 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/resnest.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    91012 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/resnet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    30450 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/resnetv2.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    11918 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/rexnet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    13254 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/selecsls.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18165 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/senet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    17254 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/sequencer.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     8777 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/sknet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    31900 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/swin_transformer.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    33196 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/swin_transformer_v2.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    41811 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/swin_transformer_v2_cr.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    13362 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/tnt.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    12893 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/tresnet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18988 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/twins.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    11004 2023-04-28 20:49:14.000000 timm-0.9.1/timm/models/vgg.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18957 2023-05-11 22:52:53.000000 timm-0.9.1/timm/models/visformer.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    91238 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/vision_transformer.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    16265 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/vision_transformer_hybrid.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    23853 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/vision_transformer_relpos.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    30354 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/volo.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    15477 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/vovnet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     8098 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/xception.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    14086 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/xception_aligned.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    37617 2023-05-10 14:38:22.000000 timm-0.9.1/timm/models/xcit.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-12 16:50:57.161242 timm-0.9.1/timm/optim/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      507 2023-03-31 00:49:24.000000 timm-0.9.1/timm/optim/__init__.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     9827 2023-02-24 22:35:42.000000 timm-0.9.1/timm/optim/adabelief.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     7459 2023-02-24 22:35:42.000000 timm-0.9.1/timm/optim/adafactor.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6535 2023-02-24 22:35:42.000000 timm-0.9.1/timm/optim/adahessian.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3574 2023-02-24 22:35:42.000000 timm-0.9.1/timm/optim/adamp.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5147 2023-02-24 22:35:42.000000 timm-0.9.1/timm/optim/adamw.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5071 2023-03-31 00:49:24.000000 timm-0.9.1/timm/optim/adan.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     9184 2023-02-24 22:35:42.000000 timm-0.9.1/timm/optim/lamb.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5256 2023-02-24 22:35:42.000000 timm-0.9.1/timm/optim/lars.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     7099 2023-03-31 00:49:24.000000 timm-0.9.1/timm/optim/lion.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2463 2023-02-24 22:35:42.000000 timm-0.9.1/timm/optim/lookahead.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6893 2023-02-24 22:35:42.000000 timm-0.9.1/timm/optim/madgrad.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3871 2023-02-24 22:35:42.000000 timm-0.9.1/timm/optim/nadam.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4856 2023-02-24 22:35:42.000000 timm-0.9.1/timm/optim/nvnovograd.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    15280 2023-05-10 14:38:22.000000 timm-0.9.1/timm/optim/optim_factory.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3468 2023-02-24 22:35:42.000000 timm-0.9.1/timm/optim/radam.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6143 2023-02-24 22:35:42.000000 timm-0.9.1/timm/optim/rmsprop_tf.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2296 2023-02-24 22:35:42.000000 timm-0.9.1/timm/optim/sgdp.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-12 16:50:57.161242 timm-0.9.1/timm/scheduler/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      330 2023-03-31 00:49:24.000000 timm-0.9.1/timm/scheduler/__init__.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3843 2023-03-31 00:49:24.000000 timm-0.9.1/timm/scheduler/cosine_lr.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1930 2023-03-31 00:49:24.000000 timm-0.9.1/timm/scheduler/multistep_lr.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3573 2023-03-31 00:49:24.000000 timm-0.9.1/timm/scheduler/plateau_lr.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3673 2023-03-31 00:49:24.000000 timm-0.9.1/timm/scheduler/poly_lr.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5408 2023-03-31 00:49:24.000000 timm-0.9.1/timm/scheduler/scheduler.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6622 2023-03-31 00:49:24.000000 timm-0.9.1/timm/scheduler/scheduler_factory.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1732 2023-03-31 00:49:24.000000 timm-0.9.1/timm/scheduler/step_lr.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3607 2023-03-31 00:49:24.000000 timm-0.9.1/timm/scheduler/tanh_lr.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-12 16:50:57.161242 timm-0.9.1/timm/utils/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      764 2023-03-31 00:49:24.000000 timm-0.9.1/timm/utils/__init__.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1624 2023-02-24 22:35:42.000000 timm-0.9.1/timm/utils/agc.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6133 2023-02-24 22:35:42.000000 timm-0.9.1/timm/utils/checkpoint_saver.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      796 2023-02-24 22:35:42.000000 timm-0.9.1/timm/utils/clip_grad.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2029 2023-04-28 20:49:14.000000 timm-0.9.1/timm/utils/cuda.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1762 2023-02-24 22:35:42.000000 timm-0.9.1/timm/utils/decay_batch.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4256 2023-03-31 00:49:24.000000 timm-0.9.1/timm/utils/distributed.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2203 2023-02-24 22:35:42.000000 timm-0.9.1/timm/utils/jit.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1015 2023-02-24 22:35:42.000000 timm-0.9.1/timm/utils/log.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      901 2023-02-24 22:35:42.000000 timm-0.9.1/timm/utils/metrics.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1105 2023-03-31 00:49:24.000000 timm-0.9.1/timm/utils/misc.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     9848 2023-03-31 00:49:24.000000 timm-0.9.1/timm/utils/model.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5670 2023-02-24 22:35:42.000000 timm-0.9.1/timm/utils/model_ema.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3342 2023-04-28 20:49:14.000000 timm-0.9.1/timm/utils/onnx.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      178 2023-02-24 22:35:42.000000 timm-0.9.1/timm/utils/random.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1300 2023-03-31 00:49:24.000000 timm-0.9.1/timm/utils/summary.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)       22 2023-05-12 16:50:51.000000 timm-0.9.1/timm/version.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-12 16:50:57.145242 timm-0.9.1/timm.egg-info/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    68314 2023-05-12 16:50:57.000000 timm-0.9.1/timm.egg-info/PKG-INFO
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6937 2023-05-12 16:50:57.000000 timm-0.9.1/timm.egg-info/SOURCES.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)        1 2023-05-12 16:50:57.000000 timm-0.9.1/timm.egg-info/dependency_links.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)       58 2023-05-12 16:50:57.000000 timm-0.9.1/timm.egg-info/requires.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)        5 2023-05-12 16:50:57.000000 timm-0.9.1/timm.egg-info/top_level.txt
+drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-14 15:04:59.684933 timm-0.9.2/
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    11343 2023-02-24 22:35:42.000000 timm-0.9.2/LICENSE
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)       95 2023-03-31 00:49:24.000000 timm-0.9.2/MANIFEST.in
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    68314 2023-05-14 15:04:59.684933 timm-0.9.2/PKG-INFO
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    67196 2023-05-11 22:52:53.000000 timm-0.9.2/README.md
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      551 2023-03-31 00:49:24.000000 timm-0.9.2/pyproject.toml
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      126 2023-05-14 15:04:59.684933 timm-0.9.2/setup.cfg
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1935 2023-03-31 00:49:24.000000 timm-0.9.2/setup.py
+drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-14 15:04:59.668933 timm-0.9.2/timm/
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      292 2023-03-31 00:49:24.000000 timm-0.9.2/timm/__init__.py
+drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-14 15:04:59.672933 timm-0.9.2/timm/data/
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      819 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/__init__.py
+drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-14 15:04:59.672933 timm-0.9.2/timm/data/_info/
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   118210 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/_info/imagenet12k_synsets.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   218430 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/_info/imagenet21k_goog_synsets.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    64070 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/_info/imagenet21k_goog_to_12k_indices.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   119937 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/_info/imagenet21k_goog_to_22k_indices.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   112210 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/_info/imagenet21k_miil_synsets.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   104500 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/_info/imagenet21k_miil_w21_synsets.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   218410 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/_info/imagenet22k_ms_synsets.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    63625 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/_info/imagenet22k_ms_to_12k_indices.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   119938 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/_info/imagenet22k_ms_to_22k_indices.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   218410 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/_info/imagenet22k_synsets.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    64070 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/_info/imagenet22k_to_12k_indices.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      774 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/_info/imagenet_a_indices.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2000 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/_info/imagenet_a_synsets.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      769 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/_info/imagenet_r_indices.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2000 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/_info/imagenet_r_synsets.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   388478 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/_info/imagenet_real_labels.json
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)  1748917 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/_info/imagenet_synset_to_definition.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   741457 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/_info/imagenet_synset_to_lemma.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    10000 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/_info/imagenet_synsets.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    35550 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/auto_augment.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4531 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/config.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      442 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/constants.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5833 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/dataset.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6989 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/dataset_factory.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2391 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/dataset_info.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5540 2023-02-24 22:35:42.000000 timm-0.9.2/timm/data/distributed_sampler.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4167 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/imagenet_info.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    11849 2023-04-28 20:49:14.000000 timm-0.9.2/timm/data/loader.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    14640 2023-05-10 22:09:19.000000 timm-0.9.2/timm/data/mixup.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4964 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/random_erasing.py
+drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-14 15:04:59.676933 timm-0.9.2/timm/data/readers/
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)       72 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/readers/__init__.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      895 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/readers/class_map.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1482 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/readers/img_extensions.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      487 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/readers/reader.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1364 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/readers/reader_factory.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2431 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/readers/reader_hfds.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3315 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/readers/reader_image_folder.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     9182 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/readers/reader_image_in_tar.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2644 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/readers/reader_image_tar.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    17858 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/readers/reader_tfds.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    16724 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/readers/reader_wds.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      303 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/readers/shared_count.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1800 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/real_labels.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     9169 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/tf_preprocessing.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    11992 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/transforms.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     9840 2023-03-31 00:49:24.000000 timm-0.9.2/timm/data/transforms_factory.py
+drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-14 15:04:59.676933 timm-0.9.2/timm/layers/
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3611 2023-05-10 14:38:22.000000 timm-0.9.2/timm/layers/__init__.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4468 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/activations.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2529 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/activations_jit.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5886 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/activations_me.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6310 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/adaptive_avgmax_pool.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4934 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/attention_pool2d.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1594 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/blur_pool.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6895 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/bottleneck_attn.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4426 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/cbam.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     7486 2023-04-28 20:49:14.000000 timm-0.9.2/timm/layers/classifier.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5199 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/cond_conv2d.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4175 2023-04-12 15:57:13.000000 timm-0.9.2/timm/layers/config.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3216 2023-04-28 20:49:14.000000 timm-0.9.2/timm/layers/conv2d_same.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3836 2023-04-28 20:49:14.000000 timm-0.9.2/timm/layers/conv_bn_act.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5320 2023-04-28 20:49:14.000000 timm-0.9.2/timm/layers/create_act.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3514 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/create_attn.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1622 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/create_conv2d.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1740 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/create_norm.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3748 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/create_norm_act.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6872 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/drop.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6386 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/eca.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    13862 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/evo_norm.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4008 2023-05-10 14:38:22.000000 timm-0.9.2/timm/layers/fast_norm.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2540 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/filter_response_norm.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1109 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/format.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3824 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/gather_excite.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2445 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/global_context.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1319 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/grn.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    10662 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/halo_attn.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1053 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/helpers.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3374 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/inplace_abn.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5941 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/lambda_layer.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      743 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/linear.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1737 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/median_pool.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1843 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/mixed_conv2d.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     7008 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/ml_decoder.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     8470 2023-05-10 14:38:22.000000 timm-0.9.2/timm/layers/mlp.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6218 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/non_local_attn.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6040 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/norm.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    17418 2023-04-28 20:49:14.000000 timm-0.9.2/timm/layers/norm_act.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2877 2023-04-28 20:49:14.000000 timm-0.9.2/timm/layers/padding.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1741 2023-04-12 15:57:13.000000 timm-0.9.2/timm/layers/patch_dropout.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     8516 2023-05-10 14:38:22.000000 timm-0.9.2/timm/layers/patch_embed.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3045 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/pool2d_same.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1678 2023-05-10 14:38:22.000000 timm-0.9.2/timm/layers/pos_embed.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    11764 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/pos_embed_rel.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    14314 2023-04-28 20:49:14.000000 timm-0.9.2/timm/layers/pos_embed_sincos.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5387 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/selective_kernel.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2620 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/separable_conv.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1775 2023-04-28 20:49:14.000000 timm-0.9.2/timm/layers/space_to_depth.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3076 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/split_attn.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3441 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/split_batchnorm.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4327 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/squeeze_excite.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5887 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/std_conv.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1996 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/test_time_pool.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      335 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/trace_utils.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4765 2023-03-31 00:49:24.000000 timm-0.9.2/timm/layers/weight_init.py
+drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-14 15:04:59.676933 timm-0.9.2/timm/loss/
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      245 2023-02-24 22:35:42.000000 timm-0.9.2/timm/loss/__init__.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3343 2023-03-31 00:49:24.000000 timm-0.9.2/timm/loss/asymmetric_loss.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2030 2023-02-24 22:35:42.000000 timm-0.9.2/timm/loss/binary_cross_entropy.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1145 2023-02-24 22:35:42.000000 timm-0.9.2/timm/loss/cross_entropy.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1595 2023-02-24 22:35:42.000000 timm-0.9.2/timm/loss/jsd.py
+drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-14 15:04:59.684933 timm-0.9.2/timm/models/
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3020 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/__init__.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18037 2023-05-10 22:09:19.000000 timm-0.9.2/timm/models/_builder.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    12148 2023-03-31 00:49:24.000000 timm-0.9.2/timm/models/_efficientnet_blocks.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    19879 2023-03-31 00:49:24.000000 timm-0.9.2/timm/models/_efficientnet_builder.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5069 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/_factory.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    15488 2023-03-31 00:49:24.000000 timm-0.9.2/timm/models/_features.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4743 2023-03-31 00:49:24.000000 timm-0.9.2/timm/models/_features_fx.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5940 2023-03-31 00:49:24.000000 timm-0.9.2/timm/models/_helpers.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    15370 2023-04-28 20:49:14.000000 timm-0.9.2/timm/models/_hub.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    10503 2023-03-31 00:49:24.000000 timm-0.9.2/timm/models/_manipulate.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3525 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/_pretrained.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4171 2023-03-31 00:49:24.000000 timm-0.9.2/timm/models/_prune.py
+drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-14 15:04:59.684933 timm-0.9.2/timm/models/_pruned/
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     8734 2023-03-31 00:49:24.000000 timm-0.9.2/timm/models/_pruned/ecaresnet101d_pruned.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4520 2023-03-31 00:49:24.000000 timm-0.9.2/timm/models/_pruned/ecaresnet50d_pruned.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18596 2023-03-31 00:49:24.000000 timm-0.9.2/timm/models/_pruned/efficientnet_b1_pruned.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18676 2023-03-31 00:49:24.000000 timm-0.9.2/timm/models/_pruned/efficientnet_b2_pruned.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    21133 2023-03-31 00:49:24.000000 timm-0.9.2/timm/models/_pruned/efficientnet_b3_pruned.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    13506 2023-04-06 15:39:02.000000 timm-0.9.2/timm/models/_registry.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    23936 2023-05-12 16:50:51.000000 timm-0.9.2/timm/models/beit.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18985 2023-05-11 22:52:53.000000 timm-0.9.2/timm/models/byoanet.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    68705 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/byobnet.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18106 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/cait.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    29712 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/coat.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    15301 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/convit.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4473 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/convmixer.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    49685 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/convnext.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    24271 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/crossvit.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    40028 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/cspnet.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    23064 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/davit.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18657 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/deit.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    15634 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/densenet.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18599 2023-05-10 22:09:19.000000 timm-0.9.2/timm/models/dla.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    13621 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/dpn.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    21277 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/edgenext.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18911 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/efficientformer.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    24873 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/efficientformer_v2.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   101929 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/efficientnet.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    39675 2023-05-12 16:50:51.000000 timm-0.9.2/timm/models/eva.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      150 2023-03-31 00:49:24.000000 timm-0.9.2/timm/models/factory.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      151 2023-03-31 00:49:24.000000 timm-0.9.2/timm/models/features.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    24033 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/focalnet.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      154 2023-03-31 00:49:24.000000 timm-0.9.2/timm/models/fx_features.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    21393 2023-05-10 22:09:19.000000 timm-0.9.2/timm/models/gcvit.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    10473 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/ghostnet.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     7697 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/hardcorenas.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      223 2023-03-31 00:49:24.000000 timm-0.9.2/timm/models/helpers.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    32902 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/hrnet.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      146 2023-05-14 15:02:18.000000 timm-0.9.2/timm/models/hub.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    12077 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/inception_resnet_v2.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    17104 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/inception_v3.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    11076 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/inception_v4.py
+drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-14 15:04:59.684933 timm-0.9.2/timm/models/layers/
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3432 2023-05-11 22:52:53.000000 timm-0.9.2/timm/models/layers/__init__.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    32443 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/levit.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    84448 2023-05-11 22:52:53.000000 timm-0.9.2/timm/models/maxxvit.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    35028 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/metaformer.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    24231 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/mlp_mixer.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    30795 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/mobilenetv3.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    25734 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/mobilevit.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    35530 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/mvitv2.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    26627 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/nasnet.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    21489 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/nest.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    41085 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/nfnet.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    14946 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/pit.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    15389 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/pnasnet.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    17261 2023-05-10 22:09:19.000000 timm-0.9.2/timm/models/pvt_v2.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      151 2023-03-31 00:49:24.000000 timm-0.9.2/timm/models/registry.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    44020 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/regnet.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     7691 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/res2net.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     9635 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/resnest.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    91012 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/resnet.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    30450 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/resnetv2.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    11918 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/rexnet.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    13254 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/selecsls.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18165 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/senet.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    17254 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/sequencer.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     8777 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/sknet.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    31900 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/swin_transformer.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    33196 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/swin_transformer_v2.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    41811 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/swin_transformer_v2_cr.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    13362 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/tnt.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    12893 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/tresnet.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18988 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/twins.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    11004 2023-04-28 20:49:14.000000 timm-0.9.2/timm/models/vgg.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18957 2023-05-11 22:52:53.000000 timm-0.9.2/timm/models/visformer.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    91238 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/vision_transformer.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    16265 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/vision_transformer_hybrid.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    23853 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/vision_transformer_relpos.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    30354 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/volo.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    15477 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/vovnet.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     8098 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/xception.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    14086 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/xception_aligned.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    37617 2023-05-10 14:38:22.000000 timm-0.9.2/timm/models/xcit.py
+drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-14 15:04:59.684933 timm-0.9.2/timm/optim/
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      507 2023-03-31 00:49:24.000000 timm-0.9.2/timm/optim/__init__.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     9827 2023-02-24 22:35:42.000000 timm-0.9.2/timm/optim/adabelief.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     7459 2023-02-24 22:35:42.000000 timm-0.9.2/timm/optim/adafactor.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6535 2023-02-24 22:35:42.000000 timm-0.9.2/timm/optim/adahessian.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3574 2023-02-24 22:35:42.000000 timm-0.9.2/timm/optim/adamp.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5147 2023-02-24 22:35:42.000000 timm-0.9.2/timm/optim/adamw.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5071 2023-03-31 00:49:24.000000 timm-0.9.2/timm/optim/adan.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     9184 2023-02-24 22:35:42.000000 timm-0.9.2/timm/optim/lamb.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5256 2023-02-24 22:35:42.000000 timm-0.9.2/timm/optim/lars.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     7099 2023-03-31 00:49:24.000000 timm-0.9.2/timm/optim/lion.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2463 2023-02-24 22:35:42.000000 timm-0.9.2/timm/optim/lookahead.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6893 2023-02-24 22:35:42.000000 timm-0.9.2/timm/optim/madgrad.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3871 2023-02-24 22:35:42.000000 timm-0.9.2/timm/optim/nadam.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4856 2023-02-24 22:35:42.000000 timm-0.9.2/timm/optim/nvnovograd.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    15280 2023-05-10 14:38:22.000000 timm-0.9.2/timm/optim/optim_factory.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3468 2023-02-24 22:35:42.000000 timm-0.9.2/timm/optim/radam.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6143 2023-02-24 22:35:42.000000 timm-0.9.2/timm/optim/rmsprop_tf.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2296 2023-02-24 22:35:42.000000 timm-0.9.2/timm/optim/sgdp.py
+drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-14 15:04:59.684933 timm-0.9.2/timm/scheduler/
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      330 2023-03-31 00:49:24.000000 timm-0.9.2/timm/scheduler/__init__.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3843 2023-03-31 00:49:24.000000 timm-0.9.2/timm/scheduler/cosine_lr.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1930 2023-03-31 00:49:24.000000 timm-0.9.2/timm/scheduler/multistep_lr.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3573 2023-03-31 00:49:24.000000 timm-0.9.2/timm/scheduler/plateau_lr.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3673 2023-03-31 00:49:24.000000 timm-0.9.2/timm/scheduler/poly_lr.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5408 2023-03-31 00:49:24.000000 timm-0.9.2/timm/scheduler/scheduler.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6622 2023-03-31 00:49:24.000000 timm-0.9.2/timm/scheduler/scheduler_factory.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1732 2023-03-31 00:49:24.000000 timm-0.9.2/timm/scheduler/step_lr.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3607 2023-03-31 00:49:24.000000 timm-0.9.2/timm/scheduler/tanh_lr.py
+drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-14 15:04:59.684933 timm-0.9.2/timm/utils/
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      764 2023-03-31 00:49:24.000000 timm-0.9.2/timm/utils/__init__.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1624 2023-02-24 22:35:42.000000 timm-0.9.2/timm/utils/agc.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6133 2023-02-24 22:35:42.000000 timm-0.9.2/timm/utils/checkpoint_saver.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      796 2023-02-24 22:35:42.000000 timm-0.9.2/timm/utils/clip_grad.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2029 2023-04-28 20:49:14.000000 timm-0.9.2/timm/utils/cuda.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1762 2023-02-24 22:35:42.000000 timm-0.9.2/timm/utils/decay_batch.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4256 2023-03-31 00:49:24.000000 timm-0.9.2/timm/utils/distributed.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2203 2023-02-24 22:35:42.000000 timm-0.9.2/timm/utils/jit.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1015 2023-02-24 22:35:42.000000 timm-0.9.2/timm/utils/log.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      901 2023-02-24 22:35:42.000000 timm-0.9.2/timm/utils/metrics.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1105 2023-03-31 00:49:24.000000 timm-0.9.2/timm/utils/misc.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     9848 2023-03-31 00:49:24.000000 timm-0.9.2/timm/utils/model.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5670 2023-02-24 22:35:42.000000 timm-0.9.2/timm/utils/model_ema.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3342 2023-04-28 20:49:14.000000 timm-0.9.2/timm/utils/onnx.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      178 2023-02-24 22:35:42.000000 timm-0.9.2/timm/utils/random.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1300 2023-03-31 00:49:24.000000 timm-0.9.2/timm/utils/summary.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)       22 2023-05-14 15:03:27.000000 timm-0.9.2/timm/version.py
+drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-14 15:04:59.672933 timm-0.9.2/timm.egg-info/
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    68314 2023-05-14 15:04:59.000000 timm-0.9.2/timm.egg-info/PKG-INFO
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6937 2023-05-14 15:04:59.000000 timm-0.9.2/timm.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)        1 2023-05-14 15:04:59.000000 timm-0.9.2/timm.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)       58 2023-05-14 15:04:59.000000 timm-0.9.2/timm.egg-info/requires.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)        5 2023-05-14 15:04:59.000000 timm-0.9.2/timm.egg-info/top_level.txt
```

### Comparing `timm-0.9.1/LICENSE` & `timm-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/PKG-INFO` & `timm-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timm
-Version: 0.9.1
+Version: 0.9.2
 Summary: PyTorch Image Models
 Home-page: https://github.com/huggingface/pytorch-image-models
 Author: Ross Wightman
 Author-email: ross@huggingface.co
 Keywords: pytorch pretrained models efficientnet mobilenetv3 mnasnet resnet vision transformer vit
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
```

### Comparing `timm-0.9.1/README.md` & `timm-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/pyproject.toml` & `timm-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/setup.py` & `timm-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/__init__.py` & `timm-0.9.2/timm/data/__init__.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/_info/imagenet12k_synsets.txt` & `timm-0.9.2/timm/data/_info/imagenet12k_synsets.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/_info/imagenet21k_goog_synsets.txt` & `timm-0.9.2/timm/data/_info/imagenet21k_goog_synsets.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/_info/imagenet21k_goog_to_12k_indices.txt` & `timm-0.9.2/timm/data/_info/imagenet21k_goog_to_12k_indices.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/_info/imagenet21k_goog_to_22k_indices.txt` & `timm-0.9.2/timm/data/_info/imagenet21k_goog_to_22k_indices.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/_info/imagenet21k_miil_synsets.txt` & `timm-0.9.2/timm/data/_info/imagenet21k_miil_synsets.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/_info/imagenet21k_miil_w21_synsets.txt` & `timm-0.9.2/timm/data/_info/imagenet21k_miil_w21_synsets.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/_info/imagenet22k_ms_synsets.txt` & `timm-0.9.2/timm/data/_info/imagenet22k_ms_synsets.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/_info/imagenet22k_ms_to_12k_indices.txt` & `timm-0.9.2/timm/data/_info/imagenet22k_ms_to_12k_indices.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/_info/imagenet22k_ms_to_22k_indices.txt` & `timm-0.9.2/timm/data/_info/imagenet22k_ms_to_22k_indices.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/_info/imagenet22k_synsets.txt` & `timm-0.9.2/timm/data/_info/imagenet22k_synsets.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/_info/imagenet22k_to_12k_indices.txt` & `timm-0.9.2/timm/data/_info/imagenet22k_to_12k_indices.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/_info/imagenet_a_indices.txt` & `timm-0.9.2/timm/data/_info/imagenet_a_indices.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/_info/imagenet_a_synsets.txt` & `timm-0.9.2/timm/data/_info/imagenet_a_synsets.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/_info/imagenet_r_indices.txt` & `timm-0.9.2/timm/data/_info/imagenet_r_indices.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/_info/imagenet_r_synsets.txt` & `timm-0.9.2/timm/data/_info/imagenet_r_synsets.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/_info/imagenet_real_labels.json` & `timm-0.9.2/timm/data/_info/imagenet_real_labels.json`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/_info/imagenet_synset_to_definition.txt` & `timm-0.9.2/timm/data/_info/imagenet_synset_to_definition.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/_info/imagenet_synset_to_lemma.txt` & `timm-0.9.2/timm/data/_info/imagenet_synset_to_lemma.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/_info/imagenet_synsets.txt` & `timm-0.9.2/timm/data/_info/imagenet_synsets.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/auto_augment.py` & `timm-0.9.2/timm/data/auto_augment.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/config.py` & `timm-0.9.2/timm/data/config.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/dataset.py` & `timm-0.9.2/timm/data/dataset.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/dataset_factory.py` & `timm-0.9.2/timm/data/dataset_factory.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/dataset_info.py` & `timm-0.9.2/timm/data/dataset_info.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/distributed_sampler.py` & `timm-0.9.2/timm/data/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/imagenet_info.py` & `timm-0.9.2/timm/data/imagenet_info.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/loader.py` & `timm-0.9.2/timm/data/loader.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/mixup.py` & `timm-0.9.2/timm/data/mixup.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/random_erasing.py` & `timm-0.9.2/timm/data/random_erasing.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/readers/class_map.py` & `timm-0.9.2/timm/data/readers/class_map.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/readers/img_extensions.py` & `timm-0.9.2/timm/data/readers/img_extensions.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/readers/reader_factory.py` & `timm-0.9.2/timm/data/readers/reader_factory.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/readers/reader_hfds.py` & `timm-0.9.2/timm/data/readers/reader_hfds.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/readers/reader_image_folder.py` & `timm-0.9.2/timm/data/readers/reader_image_folder.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/readers/reader_image_in_tar.py` & `timm-0.9.2/timm/data/readers/reader_image_in_tar.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/readers/reader_image_tar.py` & `timm-0.9.2/timm/data/readers/reader_image_tar.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/readers/reader_tfds.py` & `timm-0.9.2/timm/data/readers/reader_tfds.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/readers/reader_wds.py` & `timm-0.9.2/timm/data/readers/reader_wds.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/real_labels.py` & `timm-0.9.2/timm/data/real_labels.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/tf_preprocessing.py` & `timm-0.9.2/timm/data/tf_preprocessing.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/transforms.py` & `timm-0.9.2/timm/data/transforms.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/data/transforms_factory.py` & `timm-0.9.2/timm/data/transforms_factory.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/__init__.py` & `timm-0.9.2/timm/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/activations.py` & `timm-0.9.2/timm/layers/activations.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/activations_jit.py` & `timm-0.9.2/timm/layers/activations_jit.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/activations_me.py` & `timm-0.9.2/timm/layers/activations_me.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/adaptive_avgmax_pool.py` & `timm-0.9.2/timm/layers/adaptive_avgmax_pool.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/attention_pool2d.py` & `timm-0.9.2/timm/layers/attention_pool2d.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/blur_pool.py` & `timm-0.9.2/timm/layers/blur_pool.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/bottleneck_attn.py` & `timm-0.9.2/timm/layers/bottleneck_attn.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/cbam.py` & `timm-0.9.2/timm/layers/cbam.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/classifier.py` & `timm-0.9.2/timm/layers/classifier.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/cond_conv2d.py` & `timm-0.9.2/timm/layers/cond_conv2d.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/config.py` & `timm-0.9.2/timm/layers/config.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/conv2d_same.py` & `timm-0.9.2/timm/layers/conv2d_same.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/conv_bn_act.py` & `timm-0.9.2/timm/layers/conv_bn_act.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/create_act.py` & `timm-0.9.2/timm/layers/create_act.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/create_attn.py` & `timm-0.9.2/timm/layers/create_attn.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/create_conv2d.py` & `timm-0.9.2/timm/layers/create_conv2d.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/create_norm.py` & `timm-0.9.2/timm/layers/create_norm.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/create_norm_act.py` & `timm-0.9.2/timm/layers/create_norm_act.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/drop.py` & `timm-0.9.2/timm/layers/drop.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/eca.py` & `timm-0.9.2/timm/layers/eca.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/evo_norm.py` & `timm-0.9.2/timm/layers/evo_norm.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/fast_norm.py` & `timm-0.9.2/timm/layers/fast_norm.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/filter_response_norm.py` & `timm-0.9.2/timm/layers/filter_response_norm.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/format.py` & `timm-0.9.2/timm/layers/format.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/gather_excite.py` & `timm-0.9.2/timm/layers/gather_excite.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/global_context.py` & `timm-0.9.2/timm/layers/global_context.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/grn.py` & `timm-0.9.2/timm/layers/grn.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/halo_attn.py` & `timm-0.9.2/timm/layers/halo_attn.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/helpers.py` & `timm-0.9.2/timm/layers/helpers.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/inplace_abn.py` & `timm-0.9.2/timm/layers/inplace_abn.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/lambda_layer.py` & `timm-0.9.2/timm/layers/lambda_layer.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/linear.py` & `timm-0.9.2/timm/layers/linear.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/median_pool.py` & `timm-0.9.2/timm/layers/median_pool.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/mixed_conv2d.py` & `timm-0.9.2/timm/layers/mixed_conv2d.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/ml_decoder.py` & `timm-0.9.2/timm/layers/ml_decoder.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/mlp.py` & `timm-0.9.2/timm/layers/mlp.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/non_local_attn.py` & `timm-0.9.2/timm/layers/non_local_attn.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/norm.py` & `timm-0.9.2/timm/layers/norm.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/norm_act.py` & `timm-0.9.2/timm/layers/norm_act.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/padding.py` & `timm-0.9.2/timm/layers/padding.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/patch_dropout.py` & `timm-0.9.2/timm/layers/patch_dropout.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/patch_embed.py` & `timm-0.9.2/timm/layers/patch_embed.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/pool2d_same.py` & `timm-0.9.2/timm/layers/pool2d_same.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/pos_embed.py` & `timm-0.9.2/timm/layers/pos_embed.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/pos_embed_rel.py` & `timm-0.9.2/timm/layers/pos_embed_rel.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/pos_embed_sincos.py` & `timm-0.9.2/timm/layers/pos_embed_sincos.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/selective_kernel.py` & `timm-0.9.2/timm/layers/selective_kernel.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/separable_conv.py` & `timm-0.9.2/timm/layers/separable_conv.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/space_to_depth.py` & `timm-0.9.2/timm/layers/space_to_depth.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/split_attn.py` & `timm-0.9.2/timm/layers/split_attn.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/split_batchnorm.py` & `timm-0.9.2/timm/layers/split_batchnorm.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/squeeze_excite.py` & `timm-0.9.2/timm/layers/squeeze_excite.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/std_conv.py` & `timm-0.9.2/timm/layers/std_conv.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/test_time_pool.py` & `timm-0.9.2/timm/layers/test_time_pool.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/layers/weight_init.py` & `timm-0.9.2/timm/layers/weight_init.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/loss/asymmetric_loss.py` & `timm-0.9.2/timm/loss/asymmetric_loss.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/loss/binary_cross_entropy.py` & `timm-0.9.2/timm/loss/binary_cross_entropy.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/loss/cross_entropy.py` & `timm-0.9.2/timm/loss/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/loss/jsd.py` & `timm-0.9.2/timm/loss/jsd.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/__init__.py` & `timm-0.9.2/timm/models/__init__.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/_builder.py` & `timm-0.9.2/timm/models/_builder.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/_efficientnet_blocks.py` & `timm-0.9.2/timm/models/_efficientnet_blocks.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/_efficientnet_builder.py` & `timm-0.9.2/timm/models/_efficientnet_builder.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/_factory.py` & `timm-0.9.2/timm/models/_factory.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/_features.py` & `timm-0.9.2/timm/models/_features.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/_features_fx.py` & `timm-0.9.2/timm/models/_features_fx.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/_helpers.py` & `timm-0.9.2/timm/models/_helpers.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/_hub.py` & `timm-0.9.2/timm/models/_hub.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/_manipulate.py` & `timm-0.9.2/timm/models/_manipulate.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/_pretrained.py` & `timm-0.9.2/timm/models/_pretrained.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/_prune.py` & `timm-0.9.2/timm/models/_prune.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/_pruned/ecaresnet101d_pruned.txt` & `timm-0.9.2/timm/models/_pruned/ecaresnet101d_pruned.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/_pruned/ecaresnet50d_pruned.txt` & `timm-0.9.2/timm/models/_pruned/ecaresnet50d_pruned.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/_pruned/efficientnet_b1_pruned.txt` & `timm-0.9.2/timm/models/_pruned/efficientnet_b1_pruned.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/_pruned/efficientnet_b2_pruned.txt` & `timm-0.9.2/timm/models/_pruned/efficientnet_b2_pruned.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/_pruned/efficientnet_b3_pruned.txt` & `timm-0.9.2/timm/models/_pruned/efficientnet_b3_pruned.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/_registry.py` & `timm-0.9.2/timm/models/_registry.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/beit.py` & `timm-0.9.2/timm/models/beit.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/byoanet.py` & `timm-0.9.2/timm/models/byoanet.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/byobnet.py` & `timm-0.9.2/timm/models/byobnet.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/cait.py` & `timm-0.9.2/timm/models/cait.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/coat.py` & `timm-0.9.2/timm/models/coat.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/convit.py` & `timm-0.9.2/timm/models/convit.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/convmixer.py` & `timm-0.9.2/timm/models/convmixer.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/convnext.py` & `timm-0.9.2/timm/models/convnext.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/crossvit.py` & `timm-0.9.2/timm/models/crossvit.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/cspnet.py` & `timm-0.9.2/timm/models/cspnet.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/davit.py` & `timm-0.9.2/timm/models/davit.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/deit.py` & `timm-0.9.2/timm/models/deit.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/densenet.py` & `timm-0.9.2/timm/models/densenet.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/dla.py` & `timm-0.9.2/timm/models/dla.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/dpn.py` & `timm-0.9.2/timm/models/dpn.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/edgenext.py` & `timm-0.9.2/timm/models/edgenext.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/efficientformer.py` & `timm-0.9.2/timm/models/efficientformer.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/efficientformer_v2.py` & `timm-0.9.2/timm/models/efficientformer_v2.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/efficientnet.py` & `timm-0.9.2/timm/models/efficientnet.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/eva.py` & `timm-0.9.2/timm/models/eva.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/focalnet.py` & `timm-0.9.2/timm/models/focalnet.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/gcvit.py` & `timm-0.9.2/timm/models/gcvit.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/ghostnet.py` & `timm-0.9.2/timm/models/ghostnet.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/hardcorenas.py` & `timm-0.9.2/timm/models/hardcorenas.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/hrnet.py` & `timm-0.9.2/timm/models/hrnet.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/inception_resnet_v2.py` & `timm-0.9.2/timm/models/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/inception_v3.py` & `timm-0.9.2/timm/models/inception_v3.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/inception_v4.py` & `timm-0.9.2/timm/models/inception_v4.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/layers/__init__.py` & `timm-0.9.2/timm/models/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/levit.py` & `timm-0.9.2/timm/models/levit.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/maxxvit.py` & `timm-0.9.2/timm/models/maxxvit.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/metaformer.py` & `timm-0.9.2/timm/models/metaformer.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/mlp_mixer.py` & `timm-0.9.2/timm/models/mlp_mixer.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/mobilenetv3.py` & `timm-0.9.2/timm/models/mobilenetv3.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/mobilevit.py` & `timm-0.9.2/timm/models/mobilevit.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/mvitv2.py` & `timm-0.9.2/timm/models/mvitv2.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/nasnet.py` & `timm-0.9.2/timm/models/nasnet.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/nest.py` & `timm-0.9.2/timm/models/nest.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/nfnet.py` & `timm-0.9.2/timm/models/nfnet.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/pit.py` & `timm-0.9.2/timm/models/pit.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/pnasnet.py` & `timm-0.9.2/timm/models/pnasnet.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/pvt_v2.py` & `timm-0.9.2/timm/models/pvt_v2.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/regnet.py` & `timm-0.9.2/timm/models/regnet.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/res2net.py` & `timm-0.9.2/timm/models/res2net.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/resnest.py` & `timm-0.9.2/timm/models/resnest.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/resnet.py` & `timm-0.9.2/timm/models/resnet.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/resnetv2.py` & `timm-0.9.2/timm/models/resnetv2.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/rexnet.py` & `timm-0.9.2/timm/models/rexnet.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/selecsls.py` & `timm-0.9.2/timm/models/selecsls.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/senet.py` & `timm-0.9.2/timm/models/senet.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/sequencer.py` & `timm-0.9.2/timm/models/sequencer.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/sknet.py` & `timm-0.9.2/timm/models/sknet.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/swin_transformer.py` & `timm-0.9.2/timm/models/swin_transformer.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/swin_transformer_v2.py` & `timm-0.9.2/timm/models/swin_transformer_v2.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/swin_transformer_v2_cr.py` & `timm-0.9.2/timm/models/swin_transformer_v2_cr.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/tnt.py` & `timm-0.9.2/timm/models/tnt.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/tresnet.py` & `timm-0.9.2/timm/models/tresnet.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/twins.py` & `timm-0.9.2/timm/models/twins.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/vgg.py` & `timm-0.9.2/timm/models/vgg.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/visformer.py` & `timm-0.9.2/timm/models/visformer.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/vision_transformer.py` & `timm-0.9.2/timm/models/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/vision_transformer_hybrid.py` & `timm-0.9.2/timm/models/vision_transformer_hybrid.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/vision_transformer_relpos.py` & `timm-0.9.2/timm/models/vision_transformer_relpos.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/volo.py` & `timm-0.9.2/timm/models/volo.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/vovnet.py` & `timm-0.9.2/timm/models/vovnet.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/xception.py` & `timm-0.9.2/timm/models/xception.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/xception_aligned.py` & `timm-0.9.2/timm/models/xception_aligned.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/models/xcit.py` & `timm-0.9.2/timm/models/xcit.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/optim/adabelief.py` & `timm-0.9.2/timm/optim/adabelief.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/optim/adafactor.py` & `timm-0.9.2/timm/optim/adafactor.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/optim/adahessian.py` & `timm-0.9.2/timm/optim/adahessian.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/optim/adamp.py` & `timm-0.9.2/timm/optim/adamp.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/optim/adamw.py` & `timm-0.9.2/timm/optim/adamw.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/optim/adan.py` & `timm-0.9.2/timm/optim/adan.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/optim/lamb.py` & `timm-0.9.2/timm/optim/lamb.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/optim/lars.py` & `timm-0.9.2/timm/optim/lars.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/optim/lion.py` & `timm-0.9.2/timm/optim/lion.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/optim/lookahead.py` & `timm-0.9.2/timm/optim/lookahead.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/optim/madgrad.py` & `timm-0.9.2/timm/optim/madgrad.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/optim/nadam.py` & `timm-0.9.2/timm/optim/nadam.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/optim/nvnovograd.py` & `timm-0.9.2/timm/optim/nvnovograd.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/optim/optim_factory.py` & `timm-0.9.2/timm/optim/optim_factory.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/optim/radam.py` & `timm-0.9.2/timm/optim/radam.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/optim/rmsprop_tf.py` & `timm-0.9.2/timm/optim/rmsprop_tf.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/optim/sgdp.py` & `timm-0.9.2/timm/optim/sgdp.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/scheduler/cosine_lr.py` & `timm-0.9.2/timm/scheduler/cosine_lr.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/scheduler/multistep_lr.py` & `timm-0.9.2/timm/scheduler/multistep_lr.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/scheduler/plateau_lr.py` & `timm-0.9.2/timm/scheduler/plateau_lr.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/scheduler/poly_lr.py` & `timm-0.9.2/timm/scheduler/poly_lr.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/scheduler/scheduler.py` & `timm-0.9.2/timm/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/scheduler/scheduler_factory.py` & `timm-0.9.2/timm/scheduler/scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/scheduler/step_lr.py` & `timm-0.9.2/timm/scheduler/step_lr.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/scheduler/tanh_lr.py` & `timm-0.9.2/timm/scheduler/tanh_lr.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/utils/__init__.py` & `timm-0.9.2/timm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/utils/agc.py` & `timm-0.9.2/timm/utils/agc.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/utils/checkpoint_saver.py` & `timm-0.9.2/timm/utils/checkpoint_saver.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/utils/clip_grad.py` & `timm-0.9.2/timm/utils/clip_grad.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/utils/cuda.py` & `timm-0.9.2/timm/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/utils/decay_batch.py` & `timm-0.9.2/timm/utils/decay_batch.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/utils/distributed.py` & `timm-0.9.2/timm/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/utils/jit.py` & `timm-0.9.2/timm/utils/jit.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/utils/log.py` & `timm-0.9.2/timm/utils/log.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/utils/metrics.py` & `timm-0.9.2/timm/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/utils/misc.py` & `timm-0.9.2/timm/utils/misc.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/utils/model.py` & `timm-0.9.2/timm/utils/model.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/utils/model_ema.py` & `timm-0.9.2/timm/utils/model_ema.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/utils/onnx.py` & `timm-0.9.2/timm/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm/utils/summary.py` & `timm-0.9.2/timm/utils/summary.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.1/timm.egg-info/PKG-INFO` & `timm-0.9.2/timm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timm
-Version: 0.9.1
+Version: 0.9.2
 Summary: PyTorch Image Models
 Home-page: https://github.com/huggingface/pytorch-image-models
 Author: Ross Wightman
 Author-email: ross@huggingface.co
 Keywords: pytorch pretrained models efficientnet mobilenetv3 mnasnet resnet vision transformer vit
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
```

### Comparing `timm-0.9.1/timm.egg-info/SOURCES.txt` & `timm-0.9.2/timm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

