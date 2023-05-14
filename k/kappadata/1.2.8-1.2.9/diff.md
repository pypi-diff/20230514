# Comparing `tmp/kappadata-1.2.8.tar.gz` & `tmp/kappadata-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kappadata-1.2.8.tar", last modified: Sun Apr  9 01:03:19 2023, max compression
+gzip compressed data, was "kappadata-1.2.9.tar", last modified: Wed Apr 12 21:53:00 2023, max compression
```

## Comparing `kappadata-1.2.8.tar` & `kappadata-1.2.9.tar`

### file list

```diff
@@ -1,157 +1,162 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:19.023927 kappadata-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-09 01:00:29.000000 kappadata-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-04-09 01:03:19.023927 kappadata-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-04-09 01:00:29.000000 kappadata-1.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.967926 kappadata-1.2.8/kappadata/
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-04-09 01:03:00.000000 kappadata-1.2.8/kappadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.971926 kappadata-1.2.8/kappadata/caching/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/caching/cached_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/caching/shared_dict_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.971926 kappadata-1.2.8/kappadata/collators/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/collators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.975926 kappadata-1.2.8/kappadata/collators/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/collators/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/collators/base/kd_collator_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/collators/base/kd_compose_collator.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/collators/base/kd_single_collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/collators/kd_mix_collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/collators/pad_sequences_collator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.975926 kappadata-1.2.8/kappadata/common/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.975926 kappadata-1.2.8/kappadata/common/collators/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/collators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/collators/mae_finetune_mix_collator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.975926 kappadata-1.2.8/kappadata/common/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/datasets/kd_image_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.979926 kappadata-1.2.8/kappadata/common/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/transforms/byol_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/transforms/imagenet_minaug_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/transforms/imagenet_noaug_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/transforms/mae_finetune_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.979926 kappadata-1.2.8/kappadata/common/transforms/norm/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/transforms/norm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/transforms/norm/kd_cifar100_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/transforms/norm/kd_cifar10_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/transforms/norm/kd_image_net_norm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.979926 kappadata-1.2.8/kappadata/common/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.983926 kappadata-1.2.8/kappadata/common/wrappers/sample_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/wrappers/sample_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/wrappers/sample_wrappers/byol_multi_view_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_multi_view_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_x_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/common/wrappers/sample_wrappers/imagenet_noaug_x_transform_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.983926 kappadata-1.2.8/kappadata/copying/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/copying/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/copying/image_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.987926 kappadata-1.2.8/kappadata/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/datasets/kd_concat_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/datasets/kd_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/datasets/kd_subset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/datasets/kd_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/error_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.987926 kappadata-1.2.8/kappadata/loading/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/loading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/loading/image_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.987926 kappadata-1.2.8/kappadata/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/samplers/infinite_batch_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/samplers/interleaved_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:19.003927 kappadata-1.2.8/kappadata/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/add_gaussian_noise_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:19.007927 kappadata-1.2.8/kappadata/transforms/base/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/base/kd_compose_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/base/kd_identity_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/base/kd_random_apply_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/base/kd_scheduled_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/base/kd_stochastic_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/base/kd_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/image_pos_embed_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/image_pos_embed_sincos.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_bucketize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_color_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_gaussian_blur_pil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_gaussian_blur_tv.py
--rw-r--r--   0 runner    (1001) docker     (123)     9771 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_rand_augment.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_rand_augment_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_random_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_random_color_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_random_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_random_erasing.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_random_gaussian_blur_pil.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_random_gaussian_blur_tv.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_random_grayscale.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_random_horizontal_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_random_resized_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_random_solarize.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_rearrange.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/kd_solarize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:19.007927 kappadata-1.2.8/kappadata/transforms/norm/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/norm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:19.007927 kappadata-1.2.8/kappadata/transforms/norm/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/norm/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/norm/base/kd_norm_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/norm/kd_image_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/norm/kd_image_range_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/patchify_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/patchwise_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/patchwise_random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/patchwise_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/save_state_to_context_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/transforms/unpatchify_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:19.015927 kappadata-1.2.8/kappadata/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/utils/class_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/utils/color_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/utils/magnitude_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/utils/multi_crop_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/utils/one_hot.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/utils/param_checking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/utils/pos_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/utils/save_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/utils/transform_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:19.015927 kappadata-1.2.8/kappadata/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:19.019927 kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/repeat_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/shuffle_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/subset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/mode_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:19.023927 kappadata-1.2.8/kappadata/wrappers/sample_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/sample_wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:19.023927 kappadata-1.2.8/kappadata/wrappers/sample_wrappers/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/sample_wrappers/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/sample_wrappers/kd_mix_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/sample_wrappers/one_hot_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/sample_wrappers/source_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/sample_wrappers/target_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/sample_wrappers/x_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/sample_wrappers/y_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-09 01:00:29.000000 kappadata-1.2.8/kappadata/wrappers/torch_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:03:18.967926 kappadata-1.2.8/kappadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-04-09 01:03:18.000000 kappadata-1.2.8/kappadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-04-09 01:03:18.000000 kappadata-1.2.8/kappadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 01:03:18.000000 kappadata-1.2.8/kappadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-09 01:03:18.000000 kappadata-1.2.8/kappadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-09 01:03:18.000000 kappadata-1.2.8/kappadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-09 01:00:29.000000 kappadata-1.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-09 01:03:19.023927 kappadata-1.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.370054 kappadata-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-12 21:50:51.000000 kappadata-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-04-12 21:53:00.370054 kappadata-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-04-12 21:50:51.000000 kappadata-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.346054 kappadata-1.2.9/kappadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-04-12 21:52:46.000000 kappadata-1.2.9/kappadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.346054 kappadata-1.2.9/kappadata/caching/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/caching/cached_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/caching/shared_dict_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.346054 kappadata-1.2.9/kappadata/collators/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/collators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.350054 kappadata-1.2.9/kappadata/collators/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/collators/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/collators/base/kd_collator_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/collators/base/kd_compose_collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/collators/base/kd_single_collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/collators/kd_mix_collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/collators/pad_sequences_collator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.350054 kappadata-1.2.9/kappadata/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.350054 kappadata-1.2.9/kappadata/common/collators/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/collators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/collators/mae_finetune_mix_collator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.350054 kappadata-1.2.9/kappadata/common/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/datasets/kd_image_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.354054 kappadata-1.2.9/kappadata/common/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/transforms/byol_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/transforms/imagenet_minaug_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/transforms/imagenet_noaug_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/transforms/mae_finetune_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.354054 kappadata-1.2.9/kappadata/common/transforms/norm/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/transforms/norm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/transforms/norm/kd_cifar100_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/transforms/norm/kd_cifar10_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/transforms/norm/kd_image_net_norm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.354054 kappadata-1.2.9/kappadata/common/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.358054 kappadata-1.2.9/kappadata/common/wrappers/sample_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/wrappers/sample_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/wrappers/sample_wrappers/byol_multi_view_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_multi_view_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_x_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/wrappers/sample_wrappers/imagenet_noaug_x_transform_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.358054 kappadata-1.2.9/kappadata/copying/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/copying/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/copying/image_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.358054 kappadata-1.2.9/kappadata/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/datasets/kd_concat_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/datasets/kd_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/datasets/kd_subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/datasets/kd_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/error_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.358054 kappadata-1.2.9/kappadata/loading/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/loading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/loading/image_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.358054 kappadata-1.2.9/kappadata/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/samplers/infinite_batch_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/samplers/interleaved_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.366054 kappadata-1.2.9/kappadata/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/add_gaussian_noise_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.366054 kappadata-1.2.9/kappadata/transforms/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/base/kd_compose_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/base/kd_identity_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/base/kd_random_apply_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/base/kd_scheduled_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/base/kd_stochastic_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/base/kd_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/image_pos_embed_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/image_pos_embed_sincos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_bucketize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_color_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_gaussian_blur_pil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_gaussian_blur_tv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9771 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_rand_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_rand_augment_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_random_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_random_color_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_random_erasing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_random_gaussian_blur_pil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_random_gaussian_blur_tv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_random_grayscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_random_horizontal_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_random_resized_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_random_solarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_rearrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_solarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_two_random_crop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.366054 kappadata-1.2.9/kappadata/transforms/norm/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/norm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.366054 kappadata-1.2.9/kappadata/transforms/norm/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/norm/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/norm/base/kd_norm_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/norm/kd_image_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/norm/kd_image_range_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/patchify_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/patchwise_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/patchwise_random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/patchwise_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/save_state_to_context_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/unpatchify_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.366054 kappadata-1.2.9/kappadata/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/utils/bounding_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/utils/class_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/utils/color_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/utils/magnitude_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/utils/multi_crop_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/utils/one_hot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/utils/param_checking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/utils/pos_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/utils/save_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/utils/transform_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.366054 kappadata-1.2.9/kappadata/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/visualization/visualize_two_random_crop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.370054 kappadata-1.2.9/kappadata/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.370054 kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/repeat_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/shuffle_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/subset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/mode_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.370054 kappadata-1.2.9/kappadata/wrappers/sample_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/sample_wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.370054 kappadata-1.2.9/kappadata/wrappers/sample_wrappers/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/sample_wrappers/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/sample_wrappers/kd_mix_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/sample_wrappers/one_hot_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/sample_wrappers/source_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/sample_wrappers/target_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/sample_wrappers/x_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/sample_wrappers/y_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/torch_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.346054 kappadata-1.2.9/kappadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-04-12 21:53:00.000000 kappadata-1.2.9/kappadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-04-12 21:53:00.000000 kappadata-1.2.9/kappadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 21:53:00.000000 kappadata-1.2.9/kappadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-12 21:53:00.000000 kappadata-1.2.9/kappadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 21:53:00.000000 kappadata-1.2.9/kappadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-12 21:50:51.000000 kappadata-1.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-12 21:53:00.370054 kappadata-1.2.9/setup.cfg
```

### Comparing `kappadata-1.2.8/LICENSE` & `kappadata-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/PKG-INFO` & `kappadata-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kappadata
-Version: 1.2.8
+Version: 1.2.9
 Summary: pytorch dataset wrappers for in-memory caching
 Home-page: https://github.com/BenediktAlkin/KappaData
 Project-URL: Source Code, https://github.com/BenediktAlkin/KappaData
 Project-URL: Bug Tracker, https://github.com/BenediktAlkin/KappaData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kappadata-1.2.8/README.md` & `kappadata-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/__init__.py` & `kappadata-1.2.9/kappadata/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.2.8"
+__version__ = "1.2.9"
 
 import kappadata.caching
 import kappadata.common
 import kappadata.copying
 import kappadata.datasets
 import kappadata.loading
 import kappadata.transforms
```

### Comparing `kappadata-1.2.8/kappadata/caching/cached_dataset.py` & `kappadata-1.2.9/kappadata/caching/cached_dataset.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/caching/shared_dict_dataset.py` & `kappadata-1.2.9/kappadata/caching/shared_dict_dataset.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/collators/base/kd_collator_base.py` & `kappadata-1.2.9/kappadata/collators/base/kd_collator_base.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/collators/base/kd_compose_collator.py` & `kappadata-1.2.9/kappadata/collators/base/kd_compose_collator.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/collators/base/kd_single_collator.py` & `kappadata-1.2.9/kappadata/collators/base/kd_single_collator.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/collators/kd_mix_collator.py` & `kappadata-1.2.9/kappadata/collators/kd_mix_collator.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/collators/pad_sequences_collator.py` & `kappadata-1.2.9/kappadata/collators/pad_sequences_collator.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/common/__init__.py` & `kappadata-1.2.9/kappadata/common/__init__.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/common/datasets/kd_image_folder.py` & `kappadata-1.2.9/kappadata/common/datasets/kd_image_folder.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/common/transforms/byol_transforms.py` & `kappadata-1.2.9/kappadata/common/transforms/byol_transforms.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/common/transforms/imagenet_minaug_transforms.py` & `kappadata-1.2.9/kappadata/common/transforms/imagenet_minaug_transforms.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/common/transforms/imagenet_noaug_transforms.py` & `kappadata-1.2.9/kappadata/common/transforms/imagenet_noaug_transforms.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/common/transforms/mae_finetune_transform.py` & `kappadata-1.2.9/kappadata/common/transforms/mae_finetune_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_multi_view_wrapper.py` & `kappadata-1.2.9/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_multi_view_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_x_transform_wrapper.py` & `kappadata-1.2.9/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_x_transform_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/common/wrappers/sample_wrappers/imagenet_noaug_x_transform_wrapper.py` & `kappadata-1.2.9/kappadata/common/wrappers/sample_wrappers/imagenet_noaug_x_transform_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/copying/image_folder.py` & `kappadata-1.2.9/kappadata/copying/image_folder.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/datasets/kd_concat_dataset.py` & `kappadata-1.2.9/kappadata/datasets/kd_concat_dataset.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/datasets/kd_dataset.py` & `kappadata-1.2.9/kappadata/datasets/kd_dataset.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/datasets/kd_subset.py` & `kappadata-1.2.9/kappadata/datasets/kd_subset.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/datasets/kd_wrapper.py` & `kappadata-1.2.9/kappadata/datasets/kd_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/error_messages.py` & `kappadata-1.2.9/kappadata/error_messages.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/factory.py` & `kappadata-1.2.9/kappadata/factory.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/samplers/infinite_batch_sampler.py` & `kappadata-1.2.9/kappadata/samplers/infinite_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/samplers/interleaved_sampler.py` & `kappadata-1.2.9/kappadata/samplers/interleaved_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/transforms/__init__.py` & `kappadata-1.2.9/kappadata/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/transforms/add_gaussian_noise_transform.py` & `kappadata-1.2.9/kappadata/transforms/add_gaussian_noise_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/transforms/base/kd_compose_transform.py` & `kappadata-1.2.9/kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,25 @@
-from kappadata.factory import object_to_transform
-from .kd_stochastic_transform import KDStochasticTransform
-from .kd_transform import KDTransform
+import numpy as np
 
+from kappadata.datasets.kd_wrapper import KDWrapper
+from kappadata.factory import object_to_transform
+from kappadata.transforms import KDComposeTransform, KDStochasticTransform, KDTransform
 
-class KDComposeTransform(KDTransform):
-    def __init__(self, transforms):
-        super().__init__()
-        self.transforms = [object_to_transform(transform) for transform in transforms]
 
-    def __call__(self, x, ctx=None):
-        if ctx is None:
-            ctx = {}
-        for t in self.transforms:
-            if isinstance(t, KDTransform):
-                x = t(x, ctx)
-            else:
-                x = t(x)
-        return x
+class TransformWrapperBase(KDWrapper):
+    def __init__(self, dataset, transform, seed=None):
+        super().__init__(dataset=dataset)
+        self.transform = object_to_transform(transform)
+        self.seed = seed
 
-    def set_rng(self, rng):
-        for t in self.transforms:
-            if isinstance(t, KDStochasticTransform):
-                t.set_rng(rng)
-        return self
+    def _getitem(self, item, idx, ctx=None):
+        if self.seed is not None:
+            rng = np.random.default_rng(seed=self.seed + idx)
+            if isinstance(self.transform, (KDComposeTransform, KDStochasticTransform)):
+                self.transform.set_rng(rng)
+        if isinstance(self.transform, KDTransform):
+            return self.transform(item, ctx=ctx)
+        return self.transform(item)
 
-    def _scale_strength(self, factor):
-        for t in self.transforms:
-            if isinstance(t, KDTransform):
-                t.scale_strength(factor)
+    def _worker_init_fn(self, rank, **kwargs):
+        if isinstance(self.transform, KDTransform):
+            self.transform.worker_init_fn(rank, **kwargs)
```

### Comparing `kappadata-1.2.8/kappadata/transforms/base/kd_random_apply_base.py` & `kappadata-1.2.9/kappadata/transforms/base/kd_random_apply_base.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/transforms/base/kd_scheduled_transform.py` & `kappadata-1.2.9/kappadata/transforms/base/kd_scheduled_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/transforms/base/kd_transform.py` & `kappadata-1.2.9/kappadata/transforms/base/kd_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/transforms/image_pos_embed_grid.py` & `kappadata-1.2.9/kappadata/transforms/image_pos_embed_grid.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/transforms/image_pos_embed_sincos.py` & `kappadata-1.2.9/kappadata/transforms/image_pos_embed_sincos.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/transforms/kd_bucketize.py` & `kappadata-1.2.9/kappadata/transforms/kd_bucketize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/transforms/kd_color_jitter.py` & `kappadata-1.2.9/kappadata/transforms/kd_color_jitter.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/transforms/kd_gaussian_blur_pil.py` & `kappadata-1.2.9/kappadata/transforms/kd_gaussian_blur_pil.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/transforms/kd_gaussian_blur_tv.py` & `kappadata-1.2.9/kappadata/transforms/kd_gaussian_blur_tv.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/transforms/kd_rand_augment.py` & `kappadata-1.2.9/kappadata/transforms/kd_rand_augment.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/transforms/kd_random_color_jitter.py` & `kappadata-1.2.9/kappadata/transforms/kd_random_color_jitter.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/transforms/kd_random_crop.py` & `kappadata-1.2.9/kappadata/transforms/kd_random_crop.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,32 +10,35 @@
         self.size = to_2tuple(size)
         self.padding = padding
         self.pad_if_needed = pad_if_needed
         self.fill = fill
         self.padding_mode = padding_mode
 
     def __call__(self, img, ctx=None):
+        img = self._pad_image(img)
+        i, j, h, w = self.get_params(img)
+        if ctx is not None:
+            ctx["random_crop"] = dict(i=i, j=j, h=h, w=w)
+        return crop(img, i, j, h, w)
+
+    def _pad_image(self, img):
         if self.padding is not None:
             img = pad(img, self.padding, self.fill, self.padding_mode)
 
         width, height = get_image_size(img)
         # pad the width if needed
         if self.pad_if_needed and width < self.size[1]:
             padding = [self.size[1] - width, 0]
             img = pad(img, padding, self.fill, self.padding_mode)
         # pad the height if needed
         if self.pad_if_needed and height < self.size[0]:
             padding = [0, self.size[0] - height]
             img = pad(img, padding, self.fill, self.padding_mode)
 
-        i, j, h, w = self.get_params(img)
-        if ctx is not None:
-            ctx["random_crop"] = dict(i=i, j=j, h=h, w=w)
-
-        return crop(img, i, j, h, w)
+        return img
 
     def get_params(self, img):
         w, h = get_image_size(img)
         th, tw = self.size
 
         if h + 1 < th or w + 1 < tw:
             raise ValueError(f"Required crop size {(th, tw)} is larger then input image size {(h, w)}")
```

### Comparing `kappadata-1.2.8/kappadata/transforms/kd_random_erasing.py` & `kappadata-1.2.9/kappadata/transforms/kd_random_erasing.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/transforms/kd_random_gaussian_blur_pil.py` & `kappadata-1.2.9/kappadata/transforms/kd_random_gaussian_blur_pil.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/transforms/kd_random_gaussian_blur_tv.py` & `kappadata-1.2.9/kappadata/transforms/kd_random_gaussian_blur_tv.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/transforms/kd_random_grayscale.py` & `kappadata-1.2.9/kappadata/transforms/kd_random_grayscale.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/transforms/kd_random_resized_crop.py` & `kappadata-1.2.9/kappadata/transforms/kd_random_resized_crop.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/transforms/kd_random_rotation.py` & `kappadata-1.2.9/kappadata/transforms/kd_random_rotation.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/transforms/kd_random_solarize.py` & `kappadata-1.2.9/kappadata/transforms/kd_random_solarize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/transforms/kd_resize.py` & `kappadata-1.2.9/kappadata/transforms/kd_resize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/transforms/kd_solarize.py` & `kappadata-1.2.9/kappadata/transforms/kd_solarize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/transforms/norm/base/kd_norm_base.py` & `kappadata-1.2.9/kappadata/transforms/norm/base/kd_norm_base.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/transforms/norm/kd_image_norm.py` & `kappadata-1.2.9/kappadata/transforms/norm/kd_image_norm.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/transforms/norm/kd_image_range_norm.py` & `kappadata-1.2.9/kappadata/transforms/norm/kd_image_range_norm.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/transforms/patchify_image.py` & `kappadata-1.2.9/kappadata/transforms/patchify_image.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/transforms/patchwise_norm.py` & `kappadata-1.2.9/kappadata/transforms/patchwise_norm.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/transforms/patchwise_random_rotation.py` & `kappadata-1.2.9/kappadata/transforms/patchwise_random_rotation.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/utils/class_counts.py` & `kappadata-1.2.9/kappadata/utils/class_counts.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/utils/color_histogram.py` & `kappadata-1.2.9/kappadata/utils/color_histogram.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/utils/magnitude_sampler.py` & `kappadata-1.2.9/kappadata/utils/magnitude_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/utils/multi_crop_utils.py` & `kappadata-1.2.9/kappadata/utils/multi_crop_utils.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/utils/pos_embed.py` & `kappadata-1.2.9/kappadata/utils/pos_embed.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/utils/save_image.py` & `kappadata-1.2.9/kappadata/utils/save_image.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/utils/transform_utils.py` & `kappadata-1.2.9/kappadata/utils/transform_utils.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py` & `kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py` & `kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py` & `kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py` & `kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/repeat_wrapper.py` & `kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/repeat_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/wrappers/dataset_wrappers/subset_wrapper.py` & `kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/subset_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/wrappers/mode_wrapper.py` & `kappadata-1.2.9/kappadata/wrappers/mode_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/wrappers/sample_wrappers/kd_mix_wrapper.py` & `kappadata-1.2.9/kappadata/wrappers/sample_wrappers/kd_mix_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py` & `kappadata-1.2.9/kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py` & `kappadata-1.2.9/kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata/wrappers/torch_wrapper.py` & `kappadata-1.2.9/kappadata/wrappers/torch_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.8/kappadata.egg-info/PKG-INFO` & `kappadata-1.2.9/kappadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kappadata
-Version: 1.2.8
+Version: 1.2.9
 Summary: pytorch dataset wrappers for in-memory caching
 Home-page: https://github.com/BenediktAlkin/KappaData
 Project-URL: Source Code, https://github.com/BenediktAlkin/KappaData
 Project-URL: Bug Tracker, https://github.com/BenediktAlkin/KappaData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kappadata-1.2.8/kappadata.egg-info/SOURCES.txt` & `kappadata-1.2.9/kappadata.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 kappadata/transforms/kd_random_horizontal_flip.py
 kappadata/transforms/kd_random_resized_crop.py
 kappadata/transforms/kd_random_rotation.py
 kappadata/transforms/kd_random_solarize.py
 kappadata/transforms/kd_rearrange.py
 kappadata/transforms/kd_resize.py
 kappadata/transforms/kd_solarize.py
+kappadata/transforms/kd_two_random_crop.py
 kappadata/transforms/patchify_image.py
 kappadata/transforms/patchwise_norm.py
 kappadata/transforms/patchwise_random_rotation.py
 kappadata/transforms/patchwise_shuffle.py
 kappadata/transforms/save_state_to_context_transform.py
 kappadata/transforms/unpatchify_image.py
 kappadata/transforms/base/__init__.py
@@ -92,24 +93,27 @@
 kappadata/transforms/base/kd_transform.py
 kappadata/transforms/norm/__init__.py
 kappadata/transforms/norm/kd_image_norm.py
 kappadata/transforms/norm/kd_image_range_norm.py
 kappadata/transforms/norm/base/__init__.py
 kappadata/transforms/norm/base/kd_norm_base.py
 kappadata/utils/__init__.py
+kappadata/utils/bounding_box_utils.py
 kappadata/utils/class_counts.py
 kappadata/utils/color_histogram.py
 kappadata/utils/logging.py
 kappadata/utils/magnitude_sampler.py
 kappadata/utils/multi_crop_utils.py
 kappadata/utils/one_hot.py
 kappadata/utils/param_checking.py
 kappadata/utils/pos_embed.py
 kappadata/utils/save_image.py
 kappadata/utils/transform_utils.py
+kappadata/visualization/__init__.py
+kappadata/visualization/visualize_two_random_crop.py
 kappadata/wrappers/__init__.py
 kappadata/wrappers/mode_wrapper.py
 kappadata/wrappers/torch_wrapper.py
 kappadata/wrappers/dataset_wrappers/__init__.py
 kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py
 kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py
 kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py
```

### Comparing `kappadata-1.2.8/setup.cfg` & `kappadata-1.2.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.2.8
+version = 1.2.9
 name = kappadata
 description = pytorch dataset wrappers for in-memory caching
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BenediktAlkin/KappaData
 project_urls = 
 	Source Code = https://github.com/BenediktAlkin/KappaData
```

