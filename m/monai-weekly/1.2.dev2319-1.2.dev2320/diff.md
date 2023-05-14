# Comparing `tmp/monai-weekly-1.2.dev2319.tar.gz` & `tmp/monai-weekly-1.2.dev2320.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monai-weekly-1.2.dev2319.tar", last modified: Sun May  7 02:22:53 2023, max compression
+gzip compressed data, was "monai-weekly-1.2.dev2320.tar", last modified: Sun May 14 02:20:34 2023, max compression
```

## Comparing `monai-weekly-1.2.dev2319.tar` & `monai-weekly-1.2.dev2320.tar`

### file list

```diff
@@ -1,1134 +1,1134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:53.079735 monai-weekly-1.2.dev2319/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-05-07 02:22:53.079735 monai-weekly-1.2.dev2319/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:53.079735 monai-weekly-1.2.dev2319/monai/
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-07 02:20:42.000000 monai-weekly-1.2.dev2319/monai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.679730 monai-weekly-1.2.dev2319/monai/_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.679730 monai-weekly-1.2.dev2319/monai/_extensions/gmm/
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/_extensions/gmm/gmm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/_extensions/gmm/gmm.h
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/_extensions/gmm/gmm_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/_extensions/gmm/gmm_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/_extensions/gmm/gmm_cuda_linalg.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/_extensions/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-07 02:22:53.079735 monai-weekly-1.2.dev2319/monai/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.679730 monai-weekly-1.2.dev2319/monai/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.683730 monai-weekly-1.2.dev2319/monai/apps/auto3dseg/
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/auto3dseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/auto3dseg/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37011 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/auto3dseg/auto_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    26063 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/auto3dseg/bundle_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    17262 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/auto3dseg/data_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    25336 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/auto3dseg/ensemble_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    16619 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/auto3dseg/hpo_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/auto3dseg/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/auto3dseg/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34568 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.687730 monai-weekly-1.2.dev2319/monai/apps/deepedit/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/deepedit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/deepedit/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    37435 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/deepedit/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.687730 monai-weekly-1.2.dev2319/monai/apps/deepgrow/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/deepgrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/deepgrow/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/deepgrow/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    42011 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/deepgrow/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.687730 monai-weekly-1.2.dev2319/monai/apps/detection/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.687730 monai-weekly-1.2.dev2319/monai/apps/detection/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/detection/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26617 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/detection/metrics/coco.py
--rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/detection/metrics/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.691730 monai-weekly-1.2.dev2319/monai/apps/detection/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/detection/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53640 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/detection/networks/retinanet_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)    19136 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/detection/networks/retinanet_network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.691730 monai-weekly-1.2.dev2319/monai/apps/detection/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/detection/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24519 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/detection/transforms/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    17916 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/detection/transforms/box_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    68979 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/detection/transforms/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.695730 monai-weekly-1.2.dev2319/monai/apps/detection/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/detection/utils/ATSS_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/detection/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18681 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/detection/utils/anchor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/detection/utils/box_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/detection/utils/box_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/detection/utils/detector_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13890 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/detection/utils/hard_negative_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/detection/utils/predict_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.695730 monai-weekly-1.2.dev2319/monai/apps/mmars/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/mmars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/mmars/mmars.py
--rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/mmars/model_desc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.699730 monai-weekly-1.2.dev2319/monai/apps/nnunet/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/nnunet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/nnunet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45766 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/nnunet/nnunetv2_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/nnunet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.699730 monai-weekly-1.2.dev2319/monai/apps/nuclick/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/nuclick/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/nuclick/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.699730 monai-weekly-1.2.dev2319/monai/apps/pathology/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/pathology/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.699730 monai-weekly-1.2.dev2319/monai/apps/pathology/engines/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/pathology/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/pathology/engines/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.699730 monai-weekly-1.2.dev2319/monai/apps/pathology/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/pathology/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/pathology/handlers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.699730 monai-weekly-1.2.dev2319/monai/apps/pathology/inferers/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/pathology/inferers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/pathology/inferers/inferer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.699730 monai-weekly-1.2.dev2319/monai/apps/pathology/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/pathology/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/pathology/losses/hovernet_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.703730 monai-weekly-1.2.dev2319/monai/apps/pathology/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/pathology/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/pathology/metrics/lesion_froc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.703730 monai-weekly-1.2.dev2319/monai/apps/pathology/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/pathology/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.703730 monai-weekly-1.2.dev2319/monai/apps/pathology/transforms/post/
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/pathology/transforms/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37322 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/pathology/transforms/post/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    25928 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/pathology/transforms/post/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.703730 monai-weekly-1.2.dev2319/monai/apps/pathology/transforms/stain/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/pathology/transforms/stain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/pathology/transforms/stain/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/pathology/transforms/stain/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/pathology/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.707730 monai-weekly-1.2.dev2319/monai/apps/reconstruction/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/reconstruction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/reconstruction/complex_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/reconstruction/fastmri_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/reconstruction/mri_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.707730 monai-weekly-1.2.dev2319/monai/apps/reconstruction/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/reconstruction/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.707730 monai-weekly-1.2.dev2319/monai/apps/reconstruction/networks/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/reconstruction/networks/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/reconstruction/networks/blocks/varnetblock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.707730 monai-weekly-1.2.dev2319/monai/apps/reconstruction/networks/nets/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/reconstruction/networks/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/reconstruction/networks/nets/complex_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/reconstruction/networks/nets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/reconstruction/networks/nets/varnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.707730 monai-weekly-1.2.dev2319/monai/apps/reconstruction/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/reconstruction/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/reconstruction/transforms/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    15844 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/reconstruction/transforms/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.711730 monai-weekly-1.2.dev2319/monai/apps/tcia/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/tcia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/tcia/label_desc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/tcia/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13505 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/apps/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.711730 monai-weekly-1.2.dev2319/monai/auto3dseg/
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/auto3dseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/auto3dseg/algo_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    41223 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/auto3dseg/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/auto3dseg/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/auto3dseg/seg_summarizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/auto3dseg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.715731 monai-weekly-1.2.dev2319/monai/bundle/
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/bundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/bundle/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16035 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/bundle/config_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    22360 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/bundle/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/bundle/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/bundle/reference_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    64234 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/bundle/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/bundle/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19001 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/bundle/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.719730 monai-weekly-1.2.dev2319/monai/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/config/deviceconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/config/type_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.731731 monai-weekly-1.2.dev2319/monai/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50102 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/data/box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/data/csv_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/data/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    68927 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/data/dataset_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/data/decathlon_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/data/fft_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/data/folder_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    12484 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/data/grid_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/data/image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    60619 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/data/image_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    39872 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/data/image_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13309 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/data/iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/data/itk_torch_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/data/meta_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    27321 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/data/meta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/data/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/data/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/data/test_time_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/data/thread_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/data/torchscript_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    64795 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/data/video_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/data/wsi_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    49442 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/data/wsi_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.735731 monai-weekly-1.2.dev2319/monai/engines/
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24568 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/engines/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/engines/multi_gpu_supervised_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    21347 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/engines/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/engines/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/engines/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.735731 monai-weekly-1.2.dev2319/monai/fl/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/fl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.735731 monai-weekly-1.2.dev2319/monai/fl/client/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/fl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/fl/client/client_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    33232 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/fl/client/monai_algo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.735731 monai-weekly-1.2.dev2319/monai/fl/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/fl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/fl/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/fl/utils/exchange_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/fl/utils/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.747731 monai-weekly-1.2.dev2319/monai/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/checkpoint_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    16071 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/checkpoint_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/classification_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/clearml_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/decollate_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/earlystop_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/ignite_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/logfile_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/lr_schedule_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/mean_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/mean_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/metric_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/metrics_reloaded_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/metrics_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)    16845 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/mlflow_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/nvtx_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/parameter_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/probability_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/smartcache_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/stats_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    23325 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/tensorboard_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/handlers/validation_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.751731 monai-weekly-1.2.dev2319/monai/inferers/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/inferers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32256 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/inferers/inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/inferers/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/inferers/splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    20017 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/inferers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.755731 monai-weekly-1.2.dev2319/monai/losses/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/losses/contrastive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/losses/deform.py
--rw-r--r--   0 runner    (1001) docker     (123)    46326 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/losses/dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/losses/ds_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/losses/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/losses/giou_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/losses/image_dissimilarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/losses/multi_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/losses/spatial_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/losses/ssim_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/losses/tversky.py
--rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/losses/unified_focal_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.763731 monai-weekly-1.2.dev2319/monai/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/metrics/active_learning_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    15101 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/metrics/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/metrics/cumulative_average.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/metrics/f_beta_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/metrics/froc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/metrics/generalized_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/metrics/hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/metrics/loss_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/metrics/meandice.py
--rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/metrics/meaniou.py
--rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/metrics/panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)    19719 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/metrics/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/metrics/rocauc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14415 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/metrics/surface_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/metrics/surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/metrics/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/metrics/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.763731 monai-weekly-1.2.dev2319/monai/networks/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.775731 monai-weekly-1.2.dev2319/monai/networks/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/blocks/acti_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/blocks/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/blocks/aspp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/blocks/backbone_fpn_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/blocks/convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/blocks/crf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/blocks/denseblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/blocks/dints_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/blocks/downsample.py
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/blocks/dynunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/blocks/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/blocks/fcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10586 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/blocks/feature_pyramid_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/blocks/fft_utils_t.py
--rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/blocks/localnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/blocks/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/blocks/patchembedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/blocks/regunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/blocks/segresnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/blocks/selfattention.py
--rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/blocks/squeeze_and_excitation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/blocks/text_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/blocks/transformerblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/blocks/unetr_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/blocks/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/blocks/warp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.779731 monai-weekly-1.2.dev2319/monai/networks/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/layers/convutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/layers/drop_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/layers/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/layers/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/layers/gmm.py
--rw-r--r--   0 runner    (1001) docker     (123)    28470 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/layers/simplelayers.py
--rw-r--r--   0 runner    (1001) docker     (123)    25576 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/layers/spatial_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/layers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/layers/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.791731 monai-weekly-1.2.dev2319/monai/networks/nets/
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21533 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/ahnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/attentionunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/basic_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/basic_unetplusplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    44771 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/dints.py
--rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/dynunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    40643 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14147 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/flexible_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/fullyconnectednet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/highresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    28678 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/milmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/netadapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17189 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/regunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16785 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/segresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15667 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/segresnet_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)    19289 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/senet.py
--rw-r--r--   0 runner    (1001) docker     (123)    42000 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/swin_unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/torchvision_fc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16626 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/transchex.py
--rw-r--r--   0 runner    (1001) docker     (123)    13722 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/varautoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/vitautoenc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/nets/vnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    46938 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/networks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.791731 monai-weekly-1.2.dev2319/monai/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/optimizers/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/optimizers/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/optimizers/novograd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/optimizers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.795731 monai-weekly-1.2.dev2319/monai/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)    15268 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/adaptors.py
--rw-r--r--   0 runner    (1001) docker     (123)    40812 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/compose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.799731 monai-weekly-1.2.dev2319/monai/transforms/croppad/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/croppad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68231 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/croppad/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/croppad/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    54071 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/croppad/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/croppad/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.799731 monai-weekly-1.2.dev2319/monai/transforms/intensity/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/intensity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    98613 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/intensity/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    76501 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/intensity/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    18604 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/inverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/inverse_batch_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.803732 monai-weekly-1.2.dev2319/monai/transforms/io/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25430 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/io/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/io/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.803732 monai-weekly-1.2.dev2319/monai/transforms/lazy/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/lazy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/lazy/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     9851 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/lazy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.803732 monai-weekly-1.2.dev2319/monai/transforms/meta_utility/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/meta_utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/meta_utility/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/nvtx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.803732 monai-weekly-1.2.dev2319/monai/transforms/post/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/post/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    39905 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/post/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.807731 monai-weekly-1.2.dev2319/monai/transforms/signal/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16378 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/signal/array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.807731 monai-weekly-1.2.dev2319/monai/transforms/smooth_field/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/smooth_field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/smooth_field/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/smooth_field/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.811732 monai-weekly-1.2.dev2319/monai/transforms/spatial/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/spatial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   166745 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/spatial/array.py
--rw-r--r--   0 runner    (1001) docker     (123)   107151 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/spatial/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    31773 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/spatial/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/traits.py
--rw-r--r--   0 runner    (1001) docker     (123)    18234 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.811732 monai-weekly-1.2.dev2319/monai/transforms/utility/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70839 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/utility/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    76330 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/utility/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    77805 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    31081 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/utils_create_transform_ims.py
--rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/transforms/utils_pytorch_numpy_unification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.815732 monai-weekly-1.2.dev2319/monai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/utils/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/utils/deprecate_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    16807 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    15637 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/utils/jupyter_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28185 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    23631 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/utils/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/utils/nvtx.py
--rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/utils/profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/utils/state_cacher.py
--rw-r--r--   0 runner    (1001) docker     (123)    21147 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/utils/type_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.819732 monai-weekly-1.2.dev2319/monai/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16156 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/visualize/class_activation_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/visualize/gradient_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/visualize/img2tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/visualize/occlusion_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/visualize/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/monai/visualize/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:52.819732 monai-weekly-1.2.dev2319/monai_weekly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-05-07 02:22:52.000000 monai-weekly-1.2.dev2319/monai_weekly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    33903 2023-05-07 02:22:52.000000 monai-weekly-1.2.dev2319/monai_weekly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 02:22:52.000000 monai-weekly-1.2.dev2319/monai_weekly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 02:22:52.000000 monai-weekly-1.2.dev2319/monai_weekly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-07 02:22:52.000000 monai-weekly-1.2.dev2319/monai_weekly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-07 02:22:52.000000 monai-weekly-1.2.dev2319/monai_weekly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-05-07 02:22:53.079735 monai-weekly-1.2.dev2319/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:22:53.075735 monai-weekly-1.2.dev2319/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_acn_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_activationsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_adaptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_add_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_add_coordinate_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_add_coordinate_channelsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_add_extreme_points_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_add_extreme_points_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_adjust_contrast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_adjust_contrastd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_adn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_affine_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_affine_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_affined.py
--rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_ahnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_anchor_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_apply_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_arraydataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_as_channel_first.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_as_channel_firstd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_as_channel_last.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_as_channel_lastd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_as_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_as_discreted.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_atss_box_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_attentionunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    21578 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_auto3dseg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_auto3dseg_bundlegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_auto3dseg_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_auto3dseg_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_avg_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_basic_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_basic_unetplusplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_bending_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_bilateral_approx_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_bilateral_approx_cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_bilateral_precise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_blend_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_border_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_border_padd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_bounding_rect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_bounding_rectd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_box_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)    17289 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_box_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_bundle_ckpt_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_bundle_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_bundle_get_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_bundle_init_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_bundle_onnx_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_bundle_trt_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_bundle_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_bundle_verify_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_bundle_verify_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_bundle_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_cachedataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_cachedataset_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_cachedataset_persistent_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_cachentransdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_call_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_cast_to_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_cast_to_typed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_center_scale_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_center_scale_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_center_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_center_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_channel_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_check_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_check_missing_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_classes_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_classes_to_indicesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_complex_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_component_locator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_compose_get_number_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_compute_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_compute_f_beta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_compute_froc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_compute_generalized_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_compute_ho_ver_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_compute_ho_ver_maps_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_compute_meandice.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_compute_meaniou.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_compute_panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_compute_regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_compute_roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_compute_variance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_concat_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_config_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_contrastive_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_convert_data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_convert_to_multi_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_convert_to_multi_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_convert_to_onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_convert_to_torchscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_convert_to_trt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_copy_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_copy_model_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_correct_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_create_cross_validation_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)    10466 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_create_grid_and_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_crf_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_crf_cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_crop_foreground.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_crop_foregroundd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11089 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_csv_iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_csv_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_cucim_dict_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_cucim_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_cumulative.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_cumulative_average.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_cumulative_average_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_cv2_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_data_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_data_statsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_dataset_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_dataset_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_decathlondataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_decollate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_deepedit_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_deepedit_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_deepgrow_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_deepgrow_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_deepgrow_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_delete_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_denseblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_detect_envelope.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_detection_coco_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_detector_boxselector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_detector_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_dev_collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_dice_ce_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_dice_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_dints_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_dints_mixop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_dints_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_divisible_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_divisible_padd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_download_and_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_downsample_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_drop_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_ds_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_dvf2ddf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_dynunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_dynunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_ensemble_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_ensure_channel_first.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_ensure_channel_firstd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_ensure_tuple.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_ensure_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_ensure_typed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_enum_bound_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_eval_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_evenly_divisible_all_gather_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_factorized_increase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_factorized_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_fastmri_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_fft_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_fg_bg_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_fg_bg_to_indicesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_file_basename.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_fill_holes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_fill_holesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_fl_exchange_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     8696 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_fl_monai_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_fl_monai_algo_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_fl_monai_algo_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_flatten_sub_keysd.py
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_flexible_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_flipd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_folder_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_foreground_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_foreground_maskd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_fourier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_fpn_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_from_engine_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_fullyconnectednet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_gaussian_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_gaussian_sharpen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_gaussian_sharpend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_gaussian_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_gaussian_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_generalized_dice_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_generalized_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_generalized_wasserstein_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_generate_distance_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_generate_distance_mapd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_generate_instance_border.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_generate_instance_borderd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_generate_instance_centroid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_generate_instance_centroidd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_generate_instance_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_generate_instance_contourd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_generate_instance_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_generate_instance_typed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_generate_label_classes_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_generate_param_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_generate_pos_neg_label_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_generate_spatial_bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_generate_succinct_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_generate_succinct_contourd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_generate_watershed_markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_generate_watershed_markersd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_generate_watershed_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_generate_watershed_maskd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_get_equivalent_dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_get_extreme_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_get_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_get_package_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_get_unique_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_gibbs_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_gibbs_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_giou_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_global_mutual_information_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_globalnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_gmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_grid_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_grid_distortion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_grid_distortiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_grid_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_grid_patchd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_grid_pull.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_grid_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_grid_splitd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_checkpoint_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_checkpoint_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_classification_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_classification_saver_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_clearml_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_clearml_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_confusion_matrix_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_decollate_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_early_stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_logfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_mean_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_mean_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_metric_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_metrics_reloaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_metrics_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_metrics_saver_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_nvtx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_parameter_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_prob_map_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_regression_metrics_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_rocauc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_rocauc_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_smartcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_tb_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_tb_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_handler_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_hardnegsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_header_correct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_highresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_hilbert_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_histogram_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_histogram_normalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_hovernet_instance_map_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_hovernet_instance_map_post_processingd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_hovernet_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_hovernet_nuclear_type_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_hovernet_nuclear_type_post_processingd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_identityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_image_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_image_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_img2tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_init_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_integration_autorunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_integration_bundle_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_integration_classification_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_integration_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_integration_fast_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_integration_gpu_customization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_integration_lazy_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_integration_nnunetv2_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_integration_segmentation_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_integration_sliding_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_integration_stn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_integration_unet_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_integration_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_integration_workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_integration_workflows_gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_intensity_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_intensity_statsd.py
--rw-r--r--   0 runner    (1001) docker     (123)    18873 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_inverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_inverse_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_inverse_collation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_invert.py
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_invertd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_is_supported_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    18618 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_itk_torch_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_itk_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_k_space_spike_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_k_space_spike_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_keep_largest_connected_component.py
--rw-r--r--   0 runner    (1001) docker     (123)    12548 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_keep_largest_connected_componentd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_kspace_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_label_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_label_filterd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_label_quality_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_label_to_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_label_to_contourd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_label_to_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_label_to_maskd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_lambdad.py
--rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_lesion_froc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_list_data_collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_list_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_lltm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_lmdbdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_lmdbdataset_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_load_decathlon_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_load_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_load_imaged.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_load_spacing_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_loader_semaphore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_local_normalized_cross_correlation_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_localnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_localnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_look_up_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_loss_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_make_nifti.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_map_binary_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_map_classes_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_map_label_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_map_label_valued.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_map_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_mask_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_mask_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_masked_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_masked_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_masked_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_matshow3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_mean_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_mean_ensembled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_median_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_median_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_median_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_mednistdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_meta_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)    23490 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_meta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_metatensor_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_metrics_reloaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_milmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_mmar_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_module_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_monai_env_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_monai_utils_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_mri_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_multi_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_net_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_network_consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_nifti_endianness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_nifti_header_revise.py
--rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_nifti_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_normalize_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_normalize_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_npzdictitemdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_nrrd_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_nuclick_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_numpy_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_nvtx_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_nvtx_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_occlusion_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_one_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_optim_novograd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_optional_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_ori_ras_lps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_orientationd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_p3d_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_pad_collation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_pad_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_parallel_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_parallel_execution_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_partition_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_partition_dataset_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_patch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_patch_inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_patchembedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_pathology_he_stain.py
--rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_pathology_he_stain_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_pathology_prob_nms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_persistentdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_persistentdataset_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_phl_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_phl_cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_pil_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_plot_2d_or_3d_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_png_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_polyval.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_prepare_batch_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_prepare_batch_default_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_prepare_batch_extra_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_prepare_batch_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_preset_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_print_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_print_transform_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_probnms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_probnmsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_pytorch_version_after.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_query_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_adjust_contrast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_adjust_contrastd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_affine_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_affined.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_axis_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_axis_flipd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_bias_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_bias_fieldd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_coarse_dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_coarse_dropoutd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_coarse_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_coarse_shuffled.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_crop_by_label_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_crop_by_label_classesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_crop_by_pos_neg_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_crop_by_pos_neg_labeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_cucim_dict_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_cucim_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_deform_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_elastic_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_elastic_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_elasticd_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_elasticd_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_flipd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_gaussian_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_gaussian_sharpen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_gaussian_sharpend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_gaussian_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_gaussian_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_gibbs_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_gibbs_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_grid_distortion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_grid_distortiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_grid_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_grid_patchd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_histogram_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_histogram_shiftd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_k_space_spike_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_k_space_spike_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_lambdad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_rician_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_rician_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_rotate90.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_rotate90d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_scale_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_scale_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_scale_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_scale_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_spatial_crop_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_spatial_crop_samplesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_std_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_std_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_weighted_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_weighted_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_zoom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rand_zoomd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_randidentity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_random_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_randomizable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_randomizable_transform_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_randtorchvisiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rankfilter_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_recon_net_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_reference_based_normalize_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_reference_based_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_reference_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_reg_loss_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_regunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_regunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_remove_repeated_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_remove_repeated_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_remove_small_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_repeat_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_repeat_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_replace_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_require_pkg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_resample_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_resample_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_resample_to_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_resample_to_matchd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_resampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_resize_with_pad_or_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_resize_with_pad_or_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_resized.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_retinanet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_retinanet_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_retinanet_predict_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rotate90.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rotate90d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_safe_dtype_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_saliency_inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_sample_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_sampler_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_save_classificationd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_save_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_save_imaged.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_save_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_savitzky_golay_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_savitzky_golay_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_savitzky_golay_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_scale_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_scale_intensity_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_scale_intensity_range_percentiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_scale_intensity_range_percentilesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_scale_intensity_ranged.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_scale_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_se_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_se_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_seg_loss_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_segresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_segresnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_segresnet_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_select_cross_validation_folds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_select_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_selfattention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_senet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_separable_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_set_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_set_visible_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_shuffle_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_signal_continuouswavelet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_signal_fillempty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_signal_rand_add_gaussiannoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_signal_rand_add_sine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_signal_rand_add_sine_partial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_signal_rand_add_squarepulse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_signal_rand_add_squarepulse_partial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_signal_rand_drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_signal_rand_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_signal_rand_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_signal_remove_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_simple_aspp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_simulatedelay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_simulatedelayd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_skip_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_slice_inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_sliding_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_sliding_window_hovernet_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_sliding_window_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_sliding_window_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_smartcachedataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_smooth_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_sobel_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_sobel_gradientd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_some_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    14528 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_spacing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_spacingd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_spatial_combine_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_spatial_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_spatial_padd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_spatial_resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_spatial_resampled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_split_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_split_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_splitdim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_splitdimd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_squeezedim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_squeezedimd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_ssim_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_ssim_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_state_cacher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_std_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_std_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_str2bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_str2list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_subpixel_upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)    18990 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_surface_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_swin_unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_synthetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_tciadataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_testtimeaugmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_text_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_thread_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_threadcontainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_threshold_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_threshold_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_timedcall_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_to_contiguous.py
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_to_cupy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_to_cupyd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_to_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_to_deviced.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_to_from_meta_tensord.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_to_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_to_numpyd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_to_onehot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_to_pil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_to_pild.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_to_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_to_tensord.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_torchscript_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_torchvision.py
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_torchvision_fc_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_torchvisiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_traceable_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_train_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    16832 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_trainable_bilateral.py
--rw-r--r--   0 runner    (1001) docker     (123)    21398 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_trainable_joint_bilateral.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_transchex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_transformerblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_transposed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_tversky_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_unetr_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_unified_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_upsample_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_utils_pytorch_numpy_unification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_varautoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_varnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_version_leq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_video_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_vis_cam.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_vis_gradbased.py
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_vis_gradcam.py
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_vitautoenc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_vnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_vote_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_vote_ensembled.py
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_warp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_watershed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_watershedd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_weighted_random_sampler_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_with_allow_missing_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_write_metrics_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    25914 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_wsireader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_zipdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_zoom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_zoom_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/tests/test_zoomd.py
--rw-r--r--   0 runner    (1001) docker     (123)    81097 2023-05-07 02:20:37.000000 monai-weekly-1.2.dev2319/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.414329 monai-weekly-1.2.dev2320/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-05-14 02:20:34.414329 monai-weekly-1.2.dev2320/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.414329 monai-weekly-1.2.dev2320/monai/
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-14 02:18:48.000000 monai-weekly-1.2.dev2320/monai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:33.966323 monai-weekly-1.2.dev2320/monai/_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:33.970323 monai-weekly-1.2.dev2320/monai/_extensions/gmm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/_extensions/gmm/gmm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/_extensions/gmm/gmm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/_extensions/gmm/gmm_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/_extensions/gmm/gmm_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/_extensions/gmm/gmm_cuda_linalg.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/_extensions/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-14 02:20:34.414329 monai-weekly-1.2.dev2320/monai/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:33.970323 monai-weekly-1.2.dev2320/monai/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:33.974323 monai-weekly-1.2.dev2320/monai/apps/auto3dseg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/auto3dseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/auto3dseg/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37030 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/auto3dseg/auto_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26046 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/auto3dseg/bundle_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17262 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/auto3dseg/data_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27473 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/auto3dseg/ensemble_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16620 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/auto3dseg/hpo_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/auto3dseg/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/auto3dseg/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34568 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:33.974323 monai-weekly-1.2.dev2320/monai/apps/deepedit/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/deepedit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/deepedit/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37435 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/deepedit/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:33.978323 monai-weekly-1.2.dev2320/monai/apps/deepgrow/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/deepgrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/deepgrow/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/deepgrow/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42011 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/deepgrow/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:33.978323 monai-weekly-1.2.dev2320/monai/apps/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:33.978323 monai-weekly-1.2.dev2320/monai/apps/detection/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/detection/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26617 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/detection/metrics/coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/detection/metrics/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:33.978323 monai-weekly-1.2.dev2320/monai/apps/detection/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/detection/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53640 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/detection/networks/retinanet_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19136 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/detection/networks/retinanet_network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:33.982323 monai-weekly-1.2.dev2320/monai/apps/detection/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/detection/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24519 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/detection/transforms/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17916 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/detection/transforms/box_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68979 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/detection/transforms/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:33.986323 monai-weekly-1.2.dev2320/monai/apps/detection/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/detection/utils/ATSS_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/detection/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18681 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/detection/utils/anchor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/detection/utils/box_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/detection/utils/box_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/detection/utils/detector_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13890 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/detection/utils/hard_negative_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/detection/utils/predict_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:33.986323 monai-weekly-1.2.dev2320/monai/apps/mmars/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/mmars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/mmars/mmars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/mmars/model_desc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:33.990323 monai-weekly-1.2.dev2320/monai/apps/nnunet/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/nnunet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/nnunet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48597 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/nnunet/nnunetv2_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/nnunet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:33.990323 monai-weekly-1.2.dev2320/monai/apps/nuclick/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/nuclick/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/nuclick/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:33.990323 monai-weekly-1.2.dev2320/monai/apps/pathology/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/pathology/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:33.990323 monai-weekly-1.2.dev2320/monai/apps/pathology/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/pathology/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/pathology/engines/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:33.990323 monai-weekly-1.2.dev2320/monai/apps/pathology/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/pathology/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/pathology/handlers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:33.994323 monai-weekly-1.2.dev2320/monai/apps/pathology/inferers/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/pathology/inferers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/pathology/inferers/inferer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:33.994323 monai-weekly-1.2.dev2320/monai/apps/pathology/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/pathology/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/pathology/losses/hovernet_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:33.994323 monai-weekly-1.2.dev2320/monai/apps/pathology/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/pathology/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/pathology/metrics/lesion_froc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:33.994323 monai-weekly-1.2.dev2320/monai/apps/pathology/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/pathology/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:33.998323 monai-weekly-1.2.dev2320/monai/apps/pathology/transforms/post/
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/pathology/transforms/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37322 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/pathology/transforms/post/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25928 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/pathology/transforms/post/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:33.998323 monai-weekly-1.2.dev2320/monai/apps/pathology/transforms/stain/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/pathology/transforms/stain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/pathology/transforms/stain/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/pathology/transforms/stain/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/pathology/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:33.998323 monai-weekly-1.2.dev2320/monai/apps/reconstruction/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/reconstruction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/reconstruction/complex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/reconstruction/fastmri_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/reconstruction/mri_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:33.998323 monai-weekly-1.2.dev2320/monai/apps/reconstruction/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/reconstruction/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.002323 monai-weekly-1.2.dev2320/monai/apps/reconstruction/networks/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/reconstruction/networks/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/reconstruction/networks/blocks/varnetblock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.002323 monai-weekly-1.2.dev2320/monai/apps/reconstruction/networks/nets/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/reconstruction/networks/nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/reconstruction/networks/nets/complex_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/reconstruction/networks/nets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/reconstruction/networks/nets/varnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.006323 monai-weekly-1.2.dev2320/monai/apps/reconstruction/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/reconstruction/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/reconstruction/transforms/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15844 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/reconstruction/transforms/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.006323 monai-weekly-1.2.dev2320/monai/apps/tcia/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/tcia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/tcia/label_desc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/tcia/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13505 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/apps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.014324 monai-weekly-1.2.dev2320/monai/auto3dseg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/auto3dseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/auto3dseg/algo_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41223 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/auto3dseg/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/auto3dseg/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/auto3dseg/seg_summarizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/auto3dseg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.018324 monai-weekly-1.2.dev2320/monai/bundle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/bundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/bundle/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16035 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/bundle/config_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22360 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/bundle/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/bundle/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/bundle/reference_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64632 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/bundle/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/bundle/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19004 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/bundle/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.022324 monai-weekly-1.2.dev2320/monai/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/config/deviceconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/config/type_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.034324 monai-weekly-1.2.dev2320/monai/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50102 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/data/box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/data/csv_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/data/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68927 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/data/dataset_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/data/decathlon_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/data/fft_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/data/folder_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12484 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/data/grid_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/data/image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60619 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/data/image_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39872 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/data/image_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13309 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/data/iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/data/itk_torch_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/data/meta_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27321 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/data/meta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/data/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/data/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/data/test_time_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/data/thread_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/data/torchscript_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64795 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/data/video_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/data/wsi_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49510 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/data/wsi_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.038324 monai-weekly-1.2.dev2320/monai/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24568 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/engines/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/engines/multi_gpu_supervised_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21347 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/engines/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/engines/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/engines/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.038324 monai-weekly-1.2.dev2320/monai/fl/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/fl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.042324 monai-weekly-1.2.dev2320/monai/fl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/fl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/fl/client/client_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33232 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/fl/client/monai_algo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.042324 monai-weekly-1.2.dev2320/monai/fl/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/fl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/fl/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/fl/utils/exchange_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/fl/utils/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.054324 monai-weekly-1.2.dev2320/monai/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/checkpoint_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16071 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/checkpoint_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/classification_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/clearml_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/decollate_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/earlystop_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/ignite_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/logfile_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/lr_schedule_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/mean_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/mean_iou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/metric_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/metrics_reloaded_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/metrics_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16845 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/mlflow_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/nvtx_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/parameter_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/probability_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/smartcache_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/stats_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23325 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/tensorboard_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/handlers/validation_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.058324 monai-weekly-1.2.dev2320/monai/inferers/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/inferers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32256 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/inferers/inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/inferers/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/inferers/splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20017 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/inferers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.066324 monai-weekly-1.2.dev2320/monai/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/losses/contrastive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/losses/deform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46326 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/losses/dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/losses/ds_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9521 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/losses/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/losses/giou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/losses/image_dissimilarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/losses/multi_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/losses/spatial_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/losses/ssim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/losses/tversky.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/losses/unified_focal_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.074324 monai-weekly-1.2.dev2320/monai/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/metrics/active_learning_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15101 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/metrics/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/metrics/cumulative_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/metrics/f_beta_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/metrics/froc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/metrics/generalized_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/metrics/hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/metrics/loss_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/metrics/meandice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/metrics/meaniou.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/metrics/panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19719 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/metrics/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/metrics/rocauc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14415 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/metrics/surface_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/metrics/surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/metrics/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.074324 monai-weekly-1.2.dev2320/monai/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.086325 monai-weekly-1.2.dev2320/monai/networks/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/blocks/acti_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/blocks/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/blocks/aspp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/blocks/backbone_fpn_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/blocks/convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/blocks/crf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/blocks/denseblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/blocks/dints_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/blocks/downsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/blocks/dynunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/blocks/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/blocks/fcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10586 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/blocks/feature_pyramid_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/blocks/fft_utils_t.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/blocks/localnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/blocks/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/blocks/patchembedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/blocks/regunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/blocks/segresnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/blocks/selfattention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/blocks/squeeze_and_excitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/blocks/text_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/blocks/transformerblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/blocks/unetr_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/blocks/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/blocks/warp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.090325 monai-weekly-1.2.dev2320/monai/networks/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/layers/convutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/layers/drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/layers/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/layers/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/layers/gmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28470 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/layers/simplelayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25576 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/layers/spatial_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/layers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/layers/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.106325 monai-weekly-1.2.dev2320/monai/networks/nets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21564 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/ahnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/attentionunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/basic_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/basic_unetplusplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44771 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/dints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18210 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/dynunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40643 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14147 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/flexible_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/fullyconnectednet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/highresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28678 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/milmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/netadapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18662 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/regunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16785 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/segresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/segresnet_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19289 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/senet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42000 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/swin_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/torchvision_fc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16626 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/transchex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13722 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/varautoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/vitautoenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/nets/vnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47132 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/networks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.106325 monai-weekly-1.2.dev2320/monai/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/optimizers/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/optimizers/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/optimizers/novograd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/optimizers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.114325 monai-weekly-1.2.dev2320/monai/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)    15268 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/adaptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40812 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/compose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.118325 monai-weekly-1.2.dev2320/monai/transforms/croppad/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/croppad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68231 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/croppad/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/croppad/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54071 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/croppad/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/croppad/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.118325 monai-weekly-1.2.dev2320/monai/transforms/intensity/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/intensity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98613 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/intensity/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76501 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/intensity/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18604 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/inverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/inverse_batch_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.122325 monai-weekly-1.2.dev2320/monai/transforms/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25430 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/io/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/io/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.122325 monai-weekly-1.2.dev2320/monai/transforms/lazy/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/lazy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/lazy/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9851 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/lazy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.122325 monai-weekly-1.2.dev2320/monai/transforms/meta_utility/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/meta_utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/meta_utility/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/nvtx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.126325 monai-weekly-1.2.dev2320/monai/transforms/post/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/post/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39905 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/post/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.126325 monai-weekly-1.2.dev2320/monai/transforms/signal/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16378 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/signal/array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.126325 monai-weekly-1.2.dev2320/monai/transforms/smooth_field/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/smooth_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/smooth_field/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/smooth_field/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.130325 monai-weekly-1.2.dev2320/monai/transforms/spatial/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/spatial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   166745 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/spatial/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107151 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/spatial/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31773 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/spatial/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18234 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.134325 monai-weekly-1.2.dev2320/monai/transforms/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70841 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/utility/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76330 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/utility/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77806 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31081 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/utils_create_transform_ims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/transforms/utils_pytorch_numpy_unification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.142325 monai-weekly-1.2.dev2320/monai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/utils/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/utils/deprecate_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16807 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15637 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/utils/jupyter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28184 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23631 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/utils/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/utils/nvtx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/utils/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/utils/state_cacher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21147 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/utils/type_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.142325 monai-weekly-1.2.dev2320/monai/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16156 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/visualize/class_activation_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/visualize/gradient_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/visualize/img2tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/visualize/occlusion_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/visualize/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/monai/visualize/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.146325 monai-weekly-1.2.dev2320/monai_weekly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-05-14 02:20:33.000000 monai-weekly-1.2.dev2320/monai_weekly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    33903 2023-05-14 02:20:33.000000 monai-weekly-1.2.dev2320/monai_weekly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 02:20:33.000000 monai-weekly-1.2.dev2320/monai_weekly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 02:20:33.000000 monai-weekly-1.2.dev2320/monai_weekly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-14 02:20:33.000000 monai-weekly-1.2.dev2320/monai_weekly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 02:20:33.000000 monai-weekly-1.2.dev2320/monai_weekly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-14 02:20:34.414329 monai-weekly-1.2.dev2320/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:20:34.414329 monai-weekly-1.2.dev2320/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_acn_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_activationsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_adaptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_add_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_add_coordinate_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_add_coordinate_channelsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_add_extreme_points_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_add_extreme_points_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_adjust_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_adjust_contrastd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_adn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_affine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_affine_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_affined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_ahnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_anchor_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_apply_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_arraydataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_as_channel_first.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_as_channel_firstd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_as_channel_last.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_as_channel_lastd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_as_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_as_discreted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_atss_box_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_attentionunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21578 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_auto3dseg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_auto3dseg_bundlegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_auto3dseg_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_auto3dseg_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_avg_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_basic_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_basic_unetplusplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_bending_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_bilateral_approx_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_bilateral_approx_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_bilateral_precise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_blend_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_border_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_border_padd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_bounding_rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_bounding_rectd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_box_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17289 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_box_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_bundle_ckpt_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_bundle_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_bundle_get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_bundle_init_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_bundle_onnx_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_bundle_trt_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_bundle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_bundle_verify_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_bundle_verify_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_bundle_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_cachedataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_cachedataset_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_cachedataset_persistent_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_cachentransdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_call_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_cast_to_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_cast_to_typed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_center_scale_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_center_scale_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_center_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_center_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_channel_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_check_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_check_missing_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_classes_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_classes_to_indicesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_complex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_component_locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_compose_get_number_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_compute_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_compute_f_beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_compute_froc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_compute_generalized_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_compute_ho_ver_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_compute_ho_ver_maps_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_compute_meandice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_compute_meaniou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_compute_panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_compute_regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_compute_roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_compute_variance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_concat_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_config_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_contrastive_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_convert_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_convert_to_multi_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_convert_to_multi_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_convert_to_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_convert_to_torchscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_convert_to_trt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_copy_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_copy_model_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_correct_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_create_cross_validation_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10466 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_create_grid_and_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_crf_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_crf_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_crop_foreground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_crop_foregroundd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11089 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_csv_iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_csv_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_cucim_dict_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_cucim_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_cumulative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_cumulative_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_cumulative_average_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_cv2_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_data_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_data_statsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_dataset_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_dataset_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_decathlondataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_decollate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_deepedit_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_deepedit_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_deepgrow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_deepgrow_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_deepgrow_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_delete_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_denseblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_detect_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_detection_coco_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_detector_boxselector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_detector_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_dev_collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_dice_ce_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_dice_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_dints_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_dints_mixop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_dints_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_divisible_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_divisible_padd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_download_and_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_downsample_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_ds_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_dvf2ddf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_dynunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_dynunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_ensemble_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_ensure_channel_first.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_ensure_channel_firstd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_ensure_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_ensure_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_ensure_typed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_enum_bound_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_eval_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_evenly_divisible_all_gather_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_factorized_increase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_factorized_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_fastmri_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_fft_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_fg_bg_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_fg_bg_to_indicesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_file_basename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_fill_holes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_fill_holesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_fl_exchange_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8696 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_fl_monai_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_fl_monai_algo_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_fl_monai_algo_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_flatten_sub_keysd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_flexible_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_folder_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_foreground_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_foreground_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_fourier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_fpn_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_from_engine_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_fullyconnectednet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_gaussian_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_gaussian_sharpen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_gaussian_sharpend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_gaussian_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_gaussian_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_generalized_dice_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_generalized_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_generalized_wasserstein_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_generate_distance_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_generate_distance_mapd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_generate_instance_border.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_generate_instance_borderd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_generate_instance_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_generate_instance_centroidd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_generate_instance_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_generate_instance_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_generate_instance_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_generate_instance_typed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_generate_label_classes_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_generate_param_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_generate_pos_neg_label_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_generate_spatial_bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_generate_succinct_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_generate_succinct_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_generate_watershed_markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_generate_watershed_markersd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_generate_watershed_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_generate_watershed_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_get_equivalent_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_get_extreme_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_get_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_get_package_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_get_unique_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_gibbs_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_gibbs_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_giou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_global_mutual_information_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_globalnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_gmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_grid_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_grid_distortion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_grid_distortiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_grid_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_grid_patchd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_grid_pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_grid_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_grid_splitd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_checkpoint_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_checkpoint_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_classification_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_classification_saver_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_clearml_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_clearml_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_confusion_matrix_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_decollate_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_early_stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_logfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_mean_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_mean_iou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_metric_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_metrics_reloaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_metrics_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_metrics_saver_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_nvtx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_parameter_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_prob_map_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_regression_metrics_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_rocauc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_rocauc_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_smartcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_tb_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_tb_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_handler_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_hardnegsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_header_correct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_highresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_hilbert_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_histogram_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_histogram_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_hovernet_instance_map_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_hovernet_instance_map_post_processingd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_hovernet_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_hovernet_nuclear_type_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_hovernet_nuclear_type_post_processingd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_identityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_image_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_image_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_img2tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_init_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_integration_autorunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_integration_bundle_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_integration_classification_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_integration_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_integration_fast_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_integration_gpu_customization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_integration_lazy_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_integration_nnunetv2_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_integration_segmentation_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_integration_sliding_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_integration_stn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_integration_unet_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_integration_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_integration_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_integration_workflows_gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_intensity_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_intensity_statsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18873 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_inverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_inverse_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_inverse_collation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_invert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_invertd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_is_supported_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18618 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_itk_torch_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_itk_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_k_space_spike_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_k_space_spike_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_keep_largest_connected_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12548 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_keep_largest_connected_componentd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_kspace_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_label_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_label_filterd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_label_quality_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_label_to_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_label_to_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_label_to_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_label_to_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_lambdad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_lesion_froc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_list_data_collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_list_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_lltm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_lmdbdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_lmdbdataset_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_load_decathlon_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_load_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_load_imaged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_load_spacing_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_loader_semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_local_normalized_cross_correlation_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_localnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_localnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_look_up_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_loss_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_make_nifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_map_binary_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_map_classes_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_map_label_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_map_label_valued.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_map_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_mask_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_mask_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_masked_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_masked_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_masked_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_matshow3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_mean_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_mean_ensembled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_median_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_median_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_median_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_mednistdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_meta_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23490 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_meta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_metatensor_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_metrics_reloaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_milmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_mmar_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_module_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_monai_env_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_monai_utils_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_mri_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_multi_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_net_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_network_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_nifti_endianness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_nifti_header_revise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_nifti_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_normalize_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_normalize_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_npzdictitemdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_nrrd_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_nuclick_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_numpy_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_nvtx_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_nvtx_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_occlusion_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_one_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_optim_novograd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_optional_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_ori_ras_lps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_orientationd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_p3d_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_pad_collation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_pad_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_parallel_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_parallel_execution_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_partition_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_partition_dataset_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_patch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_patch_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_patchembedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_pathology_he_stain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_pathology_he_stain_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_pathology_prob_nms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_persistentdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_persistentdataset_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_phl_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_phl_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_pil_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_plot_2d_or_3d_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_png_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_polyval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_prepare_batch_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_prepare_batch_default_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_prepare_batch_extra_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_prepare_batch_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_preset_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_print_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_print_transform_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_probnms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_probnmsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_pytorch_version_after.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_query_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_adjust_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_adjust_contrastd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_affine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_affined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_axis_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_axis_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_bias_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_bias_fieldd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_coarse_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_coarse_dropoutd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_coarse_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_coarse_shuffled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_crop_by_label_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_crop_by_label_classesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_crop_by_pos_neg_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_crop_by_pos_neg_labeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_cucim_dict_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_cucim_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_deform_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_elastic_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_elastic_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_elasticd_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_elasticd_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_gaussian_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_gaussian_sharpen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_gaussian_sharpend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_gaussian_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_gaussian_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_gibbs_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_gibbs_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_grid_distortion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_grid_distortiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_grid_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_grid_patchd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_histogram_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_histogram_shiftd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_k_space_spike_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_k_space_spike_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_lambdad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_rician_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_rician_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_rotate90.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_rotate90d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_scale_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_scale_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_scale_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_scale_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_spatial_crop_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_spatial_crop_samplesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_std_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_std_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_weighted_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_weighted_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rand_zoomd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_randidentity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_random_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_randomizable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_randomizable_transform_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_randtorchvisiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rankfilter_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_recon_net_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_reference_based_normalize_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_reference_based_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_reference_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_reg_loss_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_regunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_regunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_remove_repeated_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_remove_repeated_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_remove_small_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_repeat_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_repeat_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_replace_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_require_pkg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_resample_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_resample_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_resample_to_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_resample_to_matchd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_resampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_resize_with_pad_or_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_resize_with_pad_or_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_resized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_retinanet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_retinanet_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_retinanet_predict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rotate90.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rotate90d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_safe_dtype_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_saliency_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_sample_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_sampler_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_save_classificationd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_save_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_save_imaged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_save_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_savitzky_golay_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_savitzky_golay_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_savitzky_golay_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_scale_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_scale_intensity_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_scale_intensity_range_percentiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_scale_intensity_range_percentilesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_scale_intensity_ranged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_scale_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_se_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_se_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_seg_loss_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_segresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_segresnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_segresnet_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_select_cross_validation_folds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_select_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_selfattention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_senet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_separable_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_set_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_set_visible_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_shuffle_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_signal_continuouswavelet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_signal_fillempty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_signal_rand_add_gaussiannoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_signal_rand_add_sine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_signal_rand_add_sine_partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_signal_rand_add_squarepulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_signal_rand_add_squarepulse_partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_signal_rand_drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_signal_rand_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_signal_rand_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_signal_remove_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_simple_aspp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_simulatedelay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_simulatedelayd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_skip_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_slice_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_sliding_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_sliding_window_hovernet_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_sliding_window_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_sliding_window_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_smartcachedataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_smooth_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_sobel_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_sobel_gradientd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_some_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14528 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_spacing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_spacingd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_spatial_combine_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_spatial_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_spatial_padd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_spatial_resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_spatial_resampled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_split_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_split_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_splitdim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_splitdimd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_squeezedim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_squeezedimd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_ssim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_ssim_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_state_cacher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_std_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_std_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_str2bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_str2list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_subpixel_upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18990 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_surface_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_swin_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_tciadataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_testtimeaugmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_text_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_thread_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_threadcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_threshold_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_threshold_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_timedcall_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_to_contiguous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_to_cupy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_to_cupyd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_to_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_to_deviced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_to_from_meta_tensord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_to_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_to_numpyd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_to_onehot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_to_pil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_to_pild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_to_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_to_tensord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_torchscript_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_torchvision_fc_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_torchvisiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_traceable_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_train_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16832 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_trainable_bilateral.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21398 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_trainable_joint_bilateral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_transchex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_transformerblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_transposed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_tversky_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_unetr_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_unified_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_upsample_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_utils_pytorch_numpy_unification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_varautoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_varnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_version_leq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_video_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_vis_cam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_vis_gradbased.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_vis_gradcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_vitautoenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_vnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_vote_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_vote_ensembled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_warp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_watershed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_watershedd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_weighted_random_sampler_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_with_allow_missing_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_write_metrics_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26104 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_wsireader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_zipdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_zoom_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/tests/test_zoomd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81097 2023-05-14 02:18:45.000000 monai-weekly-1.2.dev2320/versioneer.py
```

### Comparing `monai-weekly-1.2.dev2319/LICENSE` & `monai-weekly-1.2.dev2320/LICENSE`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/PKG-INFO` & `monai-weekly-1.2.dev2320/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monai-weekly
-Version: 1.2.dev2319
+Version: 1.2.dev2320
 Summary: AI Toolkit for Healthcare Imaging
 Home-page: https://monai.io/
 Author: MONAI Consortium
 Author-email: monai.contact@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.monai.io/
 Project-URL: Bug Tracker, https://github.com/Project-MONAI/MONAI/issues
```

### Comparing `monai-weekly-1.2.dev2319/README.md` & `monai-weekly-1.2.dev2320/README.md`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/__init__.py` & `monai-weekly-1.2.dev2320/monai/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,8 +74,8 @@
     "metrics",
     "networks",
     "optimizers",
     "transforms",
     "utils",
     "visualize",
 ]
-__commit_id__ = "5fae0c1c7525bebee1e43a625c7777f594cc97a4"
+__commit_id__ = "828a4912b97b7ccfada4d61f6981a940cf71a1e4"
```

### Comparing `monai-weekly-1.2.dev2319/monai/_extensions/__init__.py` & `monai-weekly-1.2.dev2320/monai/_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/_extensions/gmm/gmm.cpp` & `monai-weekly-1.2.dev2320/monai/_extensions/gmm/gmm.cpp`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/_extensions/gmm/gmm.h` & `monai-weekly-1.2.dev2320/monai/_extensions/gmm/gmm.h`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/_extensions/gmm/gmm_cpu.cpp` & `monai-weekly-1.2.dev2320/monai/_extensions/gmm/gmm_cpu.cpp`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/_extensions/gmm/gmm_cuda.cu` & `monai-weekly-1.2.dev2320/monai/_extensions/gmm/gmm_cuda.cu`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/_extensions/gmm/gmm_cuda_linalg.cuh` & `monai-weekly-1.2.dev2320/monai/_extensions/gmm/gmm_cuda_linalg.cuh`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/_extensions/loader.py` & `monai-weekly-1.2.dev2320/monai/_extensions/loader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/__init__.py` & `monai-weekly-1.2.dev2320/monai/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/auto3dseg/__init__.py` & `monai-weekly-1.2.dev2320/monai/apps/auto3dseg/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,8 +18,8 @@
     AlgoEnsemble,
     AlgoEnsembleBestByFold,
     AlgoEnsembleBestN,
     AlgoEnsembleBuilder,
     EnsembleRunner,
 )
 from .hpo_gen import NNIGen, OptunaGen
-from .utils import export_bundle_algo_history, import_bundle_algo_history
+from .utils import export_bundle_algo_history, get_name_from_algo_id, import_bundle_algo_history
```

### Comparing `monai-weekly-1.2.dev2319/monai/apps/auto3dseg/__main__.py` & `monai-weekly-1.2.dev2320/monai/apps/auto3dseg/__main__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/auto3dseg/auto_runner.py` & `monai-weekly-1.2.dev2320/monai/apps/auto3dseg/auto_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
             work_dir = "./work_dir"
             input = "path/to/input_yaml"
             algos = ["segresnet", "dints"]
             runner = AutoRunner(work_dir=work_dir, input=input, algos=algos)
             runner.run()
 
-        - User can specify a a local folder with algorithms templates and run AutoRunner:
+        - User can specify a local folder with algorithms templates and run AutoRunner:
 
         .. code-block:: python
 
             work_dir = "./work_dir"
             input = "path/to/input_yaml"
             algos = "segresnet"
             templates_path_or_url = "./local_path_to/algorithm_templates"
@@ -410,31 +410,31 @@
         Set options for GPU-based parameter customization/optimization.
 
         Args:
             gpu_customization: the switch to determine automatically customize/optimize bundle script/config
                 parameters for each bundleAlgo based on gpus. Custom parameters are obtained through dummy
                 training to simulate the actual model training process and hyperparameter optimization (HPO)
                 experiments.
-            gpu_customization_specs (optinal): the dictionary to enable users overwrite the HPO settings. user can
+            gpu_customization_specs (optional): the dictionary to enable users overwrite the HPO settings. user can
                 overwrite part of variables as follows or all of them. The structure is as follows.
 
                 .. code-block:: python
 
                     gpu_customization_specs = {
-                        'ALOG': {
+                        'ALGO': {
                             'num_trials': 6,
                             'range_num_images_per_batch': [1, 20],
                             'range_num_sw_batch_size': [1, 20]
                         }
                     }
 
-            ALGO: the name of algorithm. It could be one of algorithm names (e.g., 'dints') or 'unversal' which
+            ALGO: the name of algorithm. It could be one of algorithm names (e.g., 'dints') or 'universal' which
                 would apply changes to all algorithms. Possible options are
 
-                - {``"unversal"``, ``"dints"``, ``"segresnet"``, ``"segresnet2d"``, ``"swinunetr"``}.
+                - {``"universal"``, ``"dints"``, ``"segresnet"``, ``"segresnet2d"``, ``"swinunetr"``}.
 
             num_trials: the number of HPO trials/experiments to run.
             range_num_images_per_batch: the range of number of images per mini-batch.
             range_num_sw_batch_size: the range of batch size in sliding-window inferer.
         """
         self.gpu_customization = gpu_customization
         if gpu_customization_specs is not None:
@@ -464,44 +464,44 @@
             For BundleAlgo objects, the training parameter to shorten the training time to a few epochs can be
                 {"num_epochs": 2, "num_epochs_per_validation": 1}
 
         """
         self.train_params = deepcopy(params) if params is not None else {}
         if "CUDA_VISIBLE_DEVICES" in self.train_params:
             warnings.warn(
-                "CUDA_VISIBLE_DEVICES is deprecated from 'set_training_params'. Use 'set_device_info' intead.",
+                "CUDA_VISIBLE_DEVICES is deprecated from 'set_training_params'. Use 'set_device_info' instead.",
                 DeprecationWarning,
             )
 
     def set_device_info(
         self,
         cuda_visible_devices: list[int] | str | None = None,
         num_nodes: int | None = None,
         mn_start_method: str | None = None,
         cmd_prefix: str | None = None,
     ) -> None:
         """
         Set the device related info
 
         Args:
-            cuda_visible_device: define GPU ids for data analyzer, training, and ensembling.
+            cuda_visible_devices: define GPU ids for data analyzer, training, and ensembling.
                 List of GPU ids [0,1,2,3] or a string "0,1,2,3".
                 Default using env "CUDA_VISIBLE_DEVICES" or all devices available.
             num_nodes: number of nodes for training and ensembling.
                 Default using env "NUM_NODES" or 1 if "NUM_NODES" is unset.
             mn_start_method: multi-node start method. Autorunner will use the method to start multi-node processes.
                 Default using env "MN_START_METHOD" or 'bcprun' if "MN_START_METHOD" is unset.
             cmd_prefix: command line prefix for subprocess running in BundleAlgo and EnsembleRunner.
                 Default using env "CMD_PREFIX" or None, examples are:
 
                     - single GPU/CPU or multinode bcprun: "python " or "/opt/conda/bin/python3.8 ",
                     - single node multi-GPU running "torchrun --nnodes=1 --nproc_per_node=2 "
 
                 If user define this prefix, please make sure --nproc_per_node matches cuda_visible_device or
-                os.env['CUDA_VISIBLE_DEVICES]. Also always set --nnodes=1. Set num_nodes for multi-node.
+                os.env['CUDA_VISIBLE_DEVICES']. Also always set --nnodes=1. Set num_nodes for multi-node.
         """
         self.device_setting: dict[str, Any] = {}
         if cuda_visible_devices is None:
             cuda_visible_devices = os.environ.get("CUDA_VISIBLE_DEVICES")
         if cuda_visible_devices is None:  # still None after reading the environ
             self.device_setting["CUDA_VISIBLE_DEVICES"] = ",".join([str(x) for x in range(torch.cuda.device_count())])
             self.device_setting["n_devices"] = torch.cuda.device_count()
@@ -523,22 +523,22 @@
         self.device_setting["MN_START_METHOD"] = mn_start_method
 
         if cmd_prefix is None:
             cmd_prefix = os.environ.get("CMD_PREFIX")
         self.device_setting["CMD_PREFIX"] = cmd_prefix
 
         if cmd_prefix is not None:
-            logger.info(f"Using user defined command running prefix {cmd_prefix}, will overide other settings")
+            logger.info(f"Using user defined command running prefix {cmd_prefix}, will override other settings")
 
     def set_ensemble_method(self, ensemble_method_name: str = "AlgoEnsembleBestByFold", **kwargs: Any) -> None:
         """
         Set the bundle ensemble method name and parameters for save image transform parameters.
 
         Args:
-            params: the name of the ensemble method. Only two methods are supported "AlgoEnsembleBestN"
+            ensemble_method_name: the name of the ensemble method. Only two methods are supported "AlgoEnsembleBestN"
                 and "AlgoEnsembleBestByFold".
             kwargs: the keyword arguments used to define the ensemble method. Currently only ``n_best`` for
                 ``AlgoEnsembleBestN`` is supported.
         """
         self.ensemble_method_name = look_up_option(
             ensemble_method_name, supported=["AlgoEnsembleBestN", "AlgoEnsembleBestByFold"]
         )
```

### Comparing `monai-weekly-1.2.dev2319/monai/apps/auto3dseg/bundle_gen.py` & `monai-weekly-1.2.dev2320/monai/apps/auto3dseg/bundle_gen.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,16 +48,16 @@
 
     ``BundleAlgo.cfg`` is a ``monai.bundle.ConfigParser`` instance.
 
     .. code-block:: python
 
         from monai.apps.auto3dseg import BundleAlgo
 
-        data_stats_yaml = "/workspace/datastats.yaml"
-        algo = BundleAlgo(template_path=../algorithms/templates/segresnet2d/configs)
+        data_stats_yaml = "../datastats.yaml"
+        algo = BundleAlgo(template_path="../algorithm_templates")
         algo.set_data_stats(data_stats_yaml)
         # algo.set_data_src("../data_src.json")
         algo.export_to_disk(".", algo_name="segresnet2d_1")
 
     This class creates MONAI bundles from a directory of 'bundle template'. Different from the regular MONAI bundle
     format, the bundle template may contain placeholders that must be filled using ``fill_template_config`` during
     ``export_to_disk``. Then created bundle keeps the same file structure as the template.
@@ -65,15 +65,16 @@
     """
 
     def __init__(self, template_path: PathLike):
         """
         Create an Algo instance based on the predefined Algo template.
 
         Args:
-            template_path: path to the root of the algo template.
+            template_path: path to a folder that contains the algorithm templates.
+                Please check https://github.com/Project-MONAI/research-contributions/tree/main/auto3dseg/algorithm_templates
 
         """
 
         self.template_path = template_path
         self.data_stats_files = ""
         self.data_list_file = ""
         self.output_path = ""
@@ -150,15 +151,16 @@
 
         """
         if kwargs.pop("copy_dirs", True):
             self.output_path = os.path.join(output_path, algo_name)
             os.makedirs(self.output_path, exist_ok=True)
             if os.path.isdir(self.output_path):
                 shutil.rmtree(self.output_path)
-            shutil.copytree(str(self.template_path), self.output_path)
+            # copy algorithm_templates/<Algo> to the working directory output_path
+            shutil.copytree(os.path.join(str(self.template_path), self.name), self.output_path)
         else:
             self.output_path = str(self.template_path)
         if kwargs.pop("fill_template", True):
             self.fill_records = self.fill_template_config(self.data_stats_files, self.output_path, **kwargs)
         logger.info(f"Generated:{self.output_path}")
 
     def _create_cmd(self, train_params: None | dict = None) -> tuple[str, str]:
@@ -248,16 +250,16 @@
     ) -> subprocess.CompletedProcess:
         """
         Load the run function in the training script of each model. Training parameter is predefined by the
         algo_config.yaml file, which is pre-filled by the fill_template_config function in the same instance.
 
         Args:
             train_params:  training parameters
-            device_settings: device related settings, should follow the device_setting in auto_runner.set_device_info.
-            'CUDA_VISIBLE_DEVICES' should be a string e.g. '0,1,2,3'
+            device_setting: device related settings, should follow the device_setting in auto_runner.set_device_info.
+                'CUDA_VISIBLE_DEVICES' should be a string e.g. '0,1,2,3'
         """
         if device_setting is not None:
             self.device_setting.update(device_setting)
             self.device_setting["n_devices"] = len(str(self.device_setting["CUDA_VISIBLE_DEVICES"]).split(","))
 
         if train_params is not None and "CUDA_VISIBLE_DEVICES" in train_params:
             warnings.warn("CUDA_VISIBLE_DEVICES is deprecated from train_params!")
@@ -338,18 +340,18 @@
 # path to download the algo_templates
 default_algo_zip = (
     f"https://github.com/Project-MONAI/research-contributions/releases/download/algo_templates/{ALGO_HASH}.tar.gz"
 )
 
 # default algorithms
 default_algos = {
-    "segresnet2d": dict(_target_="segresnet2d.scripts.algo.Segresnet2dAlgo", template_path="segresnet2d"),
-    "dints": dict(_target_="dints.scripts.algo.DintsAlgo", template_path="dints"),
-    "swinunetr": dict(_target_="swinunetr.scripts.algo.SwinunetrAlgo", template_path="swinunetr"),
-    "segresnet": dict(_target_="segresnet.scripts.algo.SegresnetAlgo", template_path="segresnet"),
+    "segresnet2d": dict(_target_="segresnet2d.scripts.algo.Segresnet2dAlgo"),
+    "dints": dict(_target_="dints.scripts.algo.DintsAlgo"),
+    "swinunetr": dict(_target_="swinunetr.scripts.algo.SwinunetrAlgo"),
+    "segresnet": dict(_target_="segresnet.scripts.algo.SegresnetAlgo"),
 }
 
 
 def _download_algos_url(url: str, at_path: str) -> dict[str, dict[str, str]]:
     """
     Downloads the algorithm templates release archive, and extracts it into a parent directory of the at_path folder.
     Returns a dictionary of the algorithm templates.
@@ -373,15 +375,15 @@
         else:
             break
 
     zip_download_dir.cleanup()
 
     algos_all = deepcopy(default_algos)
     for name in algos_all:
-        algos_all[name]["template_path"] = os.path.join(at_path, algos_all[name]["template_path"])
+        algos_all[name]["template_path"] = at_path
 
     return algos_all
 
 
 def _copy_algos_folder(folder, at_path):
     """
     Copies the algorithm templates folder to at_path.
@@ -394,17 +396,15 @@
         if os.path.exists(at_path):
             shutil.rmtree(at_path)
         shutil.copytree(folder, at_path)
 
     algos_all = {}
     for name in os.listdir(at_path):
         if os.path.exists(os.path.join(folder, name, "scripts", "algo.py")):
-            algos_all[name] = dict(
-                _target_=f"{name}.scripts.algo.{name.capitalize()}Algo", template_path=os.path.join(at_path, name)
-            )
+            algos_all[name] = dict(_target_=f"{name}.scripts.algo.{name.capitalize()}Algo", template_path=at_path)
             logger.info(f"Copying template: {name} -- {algos_all[name]}")
     if not algos_all:
         raise ValueError(f"Unable to find any algos in {folder}")
 
     return algos_all
 
 
@@ -459,15 +459,15 @@
                     raise ValueError(f"Unable to find provided algos in {algos_all}")
             else:
                 algos = algos_all
 
         self.algos: Any = []
         if isinstance(algos, dict):
             for algo_name, algo_params in sorted(algos.items()):
-                template_path = os.path.dirname(algo_params.get("template_path", "."))
+                template_path = algo_params.get("template_path", ".")
                 if len(template_path) > 0 and template_path not in sys.path:
                     sys.path.append(template_path)
 
                 try:
                     onealgo = ConfigParser(algo_params).get_parsed_content()
                     onealgo.name = algo_name
                     self.algos.append(onealgo)
@@ -482,15 +482,15 @@
                             └── validate.py
                     """
                     raise RuntimeError(msg) from e
         else:
             raise ValueError("Unexpected error algos is not a dict")
 
         self.data_stats_filename = data_stats_filename
-        self.data_src_cfg_filename = data_src_cfg_name
+        self.data_src_cfg_name = data_src_cfg_name
         self.history: list[dict] = []
 
     def set_data_stats(self, data_stats_filename: str) -> None:
         """
         Set the data stats filename
 
         Args:
@@ -498,26 +498,26 @@
         """
         self.data_stats_filename = data_stats_filename
 
     def get_data_stats(self):
         """Get the filename of the data stats"""
         return self.data_stats_filename
 
-    def set_data_src(self, data_src_cfg_filename):
+    def set_data_src(self, data_src_cfg_name):
         """
         Set the data source filename
 
         Args:
-            data_src_cfg_filename: filename of data_source file
+            data_src_cfg_name: filename of data_source file
         """
-        self.data_src_cfg_filename = data_src_cfg_filename
+        self.data_src_cfg_name = data_src_cfg_name
 
     def get_data_src(self):
         """Get the data source filename"""
-        return self.data_src_cfg_filename
+        return self.data_src_cfg_name
 
     def get_history(self) -> list:
         """Get the history of the bundleAlgo object with their names/identifiers"""
         return self.history
 
     def generate(
         self,
@@ -541,25 +541,25 @@
                 overwrite part of variables as follows or all of them. The structure is as follows.
             allow_skip: a switch to determine if some Algo in the default templates can be skipped based on the
                 analysis on the dataset from Auto3DSeg DataAnalyzer.
 
                 .. code-block:: python
 
                     gpu_customization_specs = {
-                        'ALOG': {
+                        'ALGO': {
                             'num_trials': 6,
                             'range_num_images_per_batch': [1, 20],
                             'range_num_sw_batch_size': [1, 20]
                         }
                     }
 
-            ALGO: the name of algorithm. It could be one of algorithm names (e.g., 'dints') or 'unversal' which
+            ALGO: the name of algorithm. It could be one of algorithm names (e.g., 'dints') or 'universal' which
                 would apply changes to all algorithms. Possible options are
 
-                - {``"unversal"``, ``"dints"``, ``"segresnet"``, ``"segresnet2d"``, ``"swinunetr"``}.
+                - {``"universal"``, ``"dints"``, ``"segresnet"``, ``"segresnet2d"``, ``"swinunetr"``}.
 
             num_trials: the number of HPO trials/experiments to run.
             range_num_images_per_batch: the range of number of images per mini-batch.
             range_num_sw_batch_size: the range of batch size in sliding-window inferer.
         """
         fold_idx = list(range(num_fold))
         for algo in self.algos:
```

### Comparing `monai-weekly-1.2.dev2319/monai/apps/auto3dseg/data_analyzer.py` & `monai-weekly-1.2.dev2320/monai/apps/auto3dseg/data_analyzer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/auto3dseg/ensemble_builder.py` & `monai-weekly-1.2.dev2320/monai/apps/auto3dseg/ensemble_builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,22 +20,22 @@
 from warnings import warn
 
 import numpy as np
 import torch
 import torch.distributed as dist
 
 from monai.apps.auto3dseg.bundle_gen import BundleAlgo
-from monai.apps.auto3dseg.utils import import_bundle_algo_history
+from monai.apps.auto3dseg.utils import get_name_from_algo_id, import_bundle_algo_history
 from monai.apps.utils import get_logger
 from monai.auto3dseg import concat_val_to_np
 from monai.auto3dseg.utils import datafold_read
 from monai.bundle import ConfigParser
 from monai.data import partition_dataset
 from monai.transforms import MeanEnsemble, SaveImage, VoteEnsemble
-from monai.utils import RankFilter
+from monai.utils import RankFilter, deprecated_arg
 from monai.utils.enums import AlgoKeys
 from monai.utils.misc import check_kwargs_exist_in_class_init, prob2class
 from monai.utils.module import look_up_option, optional_import
 
 tqdm, has_tqdm = optional_import("tqdm", name="tqdm")
 
 logger = get_logger(module_name=__name__)
@@ -80,15 +80,15 @@
 
     def set_infer_files(self, dataroot: str, data_list_or_path: str | list, data_key: str = "testing") -> None:
         """
         Set the files to perform model inference.
 
         Args:
             dataroot: the path of the files
-            data_src_cfg_file: the data source file path
+            data_list_or_path: the data source file path
         """
 
         self.infer_files = []
 
         if isinstance(data_list_or_path, list):
             self.infer_files = data_list_or_path
         elif isinstance(data_list_or_path, str):
@@ -123,14 +123,33 @@
         elif self.mode == "vote":
             classes = [prob2class(p, dim=0, keepdim=True, sigmoid=sigmoid) for p in preds]
             if sigmoid:
                 return VoteEnsemble()(classes)  # do not specify num_classes for one-hot encoding
             else:
                 return VoteEnsemble(num_classes=preds[0].shape[0])(classes)
 
+    def _apply_algo_specific_param(self, algo_spec_param: dict, param: dict, algo_name: str) -> dict:
+        """
+        Apply the model-specific params to the prediction params based on the name of the Algo.
+
+        Args:
+            algo_spec_param: a dict that has structure of {"<name of algo>": "<pred_params for that algo>"}.
+            param: the prediction params to override.
+            algo_name: name of the Algo
+
+        Returns:
+            param after being updated with the model-specific param
+        """
+        _param_to_override = deepcopy(algo_spec_param)
+        _param = deepcopy(param)
+        for k, v in _param_to_override.items():
+            if k.lower() == algo_name.lower():
+                _param.update(v)
+        return _param
+
     def __call__(self, pred_param: dict | None = None) -> list:
         """
         Use the ensembled model to predict result.
 
         Args:
             pred_param: prediction parameter dictionary. The key has two groups: the first one will be consumed
                 in this function, and the second group will be passed to the `InferClass` to override the
@@ -142,14 +161,16 @@
                       only make prediction on the infer_files[file_slices].
                     - ``"mode"``: ensemble mode. Currently "mean" and "vote" (majority voting) schemes are supported.
                     - ``"image_save_func"``: a dictionary used to instantiate the ``SaveImage`` transform. When specified,
                       the ensemble prediction will save the prediciton files, instead of keeping the files in the memory.
                       Example: `{"_target_": "SaveImage", "output_dir": "./"}`
                     - ``"sigmoid"``: use the sigmoid function (e.g. x > 0.5) to convert the prediction probability map
                       to the label class prediction, otherwise argmax(x) is used.
+                    - ``"algo_spec_params"``: a dictionary to add pred_params that are specific to a model.
+                      The dict has a format of {"<name of algo>": "<pred_params for that algo>"}.
 
                 The parameters in the second group is defined in the ``config`` of each Algo templates. Please check:
                 https://github.com/Project-MONAI/research-contributions/tree/main/auto3dseg/algorithm_templates
 
         Returns:
             A list of tensors or file paths, depending on whether ``"image_save_func"`` is set.
         """
@@ -168,24 +189,28 @@
             self.mode = look_up_option(mode, supported=["mean", "vote"])
 
         sigmoid = param.pop("sigmoid", False)
 
         if "image_save_func" in param:
             img_saver = ConfigParser(param["image_save_func"]).get_parsed_content()
 
+        algo_spec_params = param.pop("algo_spec_params", {})
+
         outputs = []
         for _, file in (
             enumerate(tqdm(files, desc="Ensembling (rank 0)..."))
             if has_tqdm and pred_param and pred_param.get("rank", 0) == 0
             else enumerate(files)
         ):
             preds = []
             for algo in self.algo_ensemble:
+                infer_algo_name = get_name_from_algo_id(algo[AlgoKeys.ID])
                 infer_instance = algo[AlgoKeys.ALGO]
-                pred = infer_instance.predict(predict_files=[file], predict_params=param)
+                _param = self._apply_algo_specific_param(algo_spec_params, param, infer_algo_name)
+                pred = infer_instance.predict(predict_files=[file], predict_params=_param)
                 preds.append(pred[0])
             if "image_save_func" in param:
                 try:
                     ensemble_preds = self.ensemble_pred(preds, sigmoid=sigmoid)
                 except BaseException:
                     ensemble_preds = self.ensemble_pred([_.to("cpu") for _ in preds], sigmoid=sigmoid)
                 res = img_saver(ensemble_preds)
@@ -286,33 +311,40 @@
 
 class AlgoEnsembleBuilder:
     """
     Build ensemble workflow from configs and arguments.
 
     Args:
         history: a collection of trained bundleAlgo algorithms.
-        data_src_cfg_filename: filename of the data source.
+        data_src_cfg_name: filename of the data source.
 
     Examples:
 
         .. code-block:: python
 
             builder = AlgoEnsembleBuilder(history, data_src_cfg)
             builder.set_ensemble_method(BundleAlgoEnsembleBestN(3))
             ensemble = builder.get_ensemble()
 
     """
 
-    def __init__(self, history: Sequence[dict[str, Any]], data_src_cfg_filename: str | None = None):
+    @deprecated_arg(
+        "data_src_cfg_filename",
+        since="1.2",
+        removed="1.3",
+        new_name="data_src_cfg_name",
+        msg_suffix="please use `data_src_cfg_name` instead.",
+    )
+    def __init__(self, history: Sequence[dict[str, Any]], data_src_cfg_name: str | None = None):
         self.infer_algos: list[dict[AlgoKeys, Any]] = []
         self.ensemble: AlgoEnsemble
         self.data_src_cfg = ConfigParser(globals=False)
 
-        if data_src_cfg_filename is not None and os.path.exists(str(data_src_cfg_filename)):
-            self.data_src_cfg.read_config(data_src_cfg_filename)
+        if data_src_cfg_name is not None and os.path.exists(str(data_src_cfg_name)):
+            self.data_src_cfg.read_config(data_src_cfg_name)
 
         for algo_dict in history:
             # load inference_config_paths
 
             name = algo_dict[AlgoKeys.ID]
             gen_algo = algo_dict[AlgoKeys.ALGO]
 
@@ -362,25 +394,29 @@
         """Get the ensemble"""
 
         return self.ensemble
 
 
 class EnsembleRunner:
     """
-    The Runner for ensembler
+    The Runner for ensembler. It ensembles predictions and saves them to the disk with a support of using multi-GPU.
 
     Args:
-        work_dir: working directory to save the intermediate and final results.
         data_src_cfg_name: filename of the data source.
-        num_fold: number of fold.
-        ensemble_method_name: method to ensemble predictions from different model.
-                              Suported methods: ["AlgoEnsembleBestN", "AlgoEnsembleBestByFold"].
-        mgpu: if using multi-gpu.
+        work_dir: working directory to save the intermediate and final results. Default is `./work_dir`.
+        num_fold: number of fold. Default is 5.
+        ensemble_method_name: method to ensemble predictions from different model. Default is AlgoEnsembleBestByFold.
+                              Supported methods: ["AlgoEnsembleBestN", "AlgoEnsembleBestByFold"].
+        mgpu: if using multi-gpu. Default is True.
         kwargs: additional image writing, ensembling parameters and prediction parameters for the ensemble inference.
-    Examples:
+              - for image saving, please check the supported parameters in SaveImage transform.
+              - for prediction parameters, please check the supported parameters in the ``AlgoEnsemble`` callables.
+              - for ensemble parameters, please check the documentation of the selected AlgoEnsemble callable.
+
+    Example:
 
         .. code-block:: python
 
             ensemble_runner = EnsembleRunner(data_src_cfg_name,
                                              work_dir,
                                              ensemble_method_name,
                                              mgpu=device_setting['n_devices']>1,
@@ -388,15 +424,15 @@
                                              **pred_params)
             ensemble_runner.run(device_setting)
 
     """
 
     def __init__(
         self,
-        data_src_cfg_name: str = "./work_dir/input.yaml",
+        data_src_cfg_name: str,
         work_dir: str = "./work_dir",
         num_fold: int = 5,
         ensemble_method_name: str = "AlgoEnsembleBestByFold",
         mgpu: bool = True,
         **kwargs: Any,
     ) -> None:
         self.data_src_cfg_name = data_src_cfg_name
@@ -455,22 +491,27 @@
             output_dir = os.path.join(self.work_dir, "ensemble_output")
             logger.info(f"The output_dir is not specified. {output_dir} will be used to save ensemble predictions.")
 
         if not os.path.isdir(output_dir):
             os.makedirs(output_dir, exist_ok=True)
             logger.info(f"Directory {output_dir} is created to save ensemble predictions")
 
+        input_yaml = ConfigParser.load_config_file(self.data_src_cfg_name)
+        data_root_dir = input_yaml.get("dataroot", "")
+
         save_image = {
             "_target_": "SaveImage",
             "output_dir": output_dir,
             "output_postfix": kwargs.pop("output_postfix", "ensemble"),
             "output_dtype": kwargs.pop("output_dtype", "$np.uint8"),
             "resample": kwargs.pop("resample", False),
             "print_log": False,
             "savepath_in_metadict": True,
+            "data_root_dir": kwargs.pop("data_root_dir", data_root_dir),
+            "separate_folder": kwargs.pop("separate_folder", False),
         }
 
         are_all_args_save_image, extra_args = check_kwargs_exist_in_class_init(SaveImage, kwargs)
         if are_all_args_save_image:
             save_image.update(kwargs)
         else:
             # kwargs has extra values for other purposes, for example, pred_params
@@ -561,17 +602,16 @@
 
     def run(self, device_setting: dict | None = None) -> None:
         """
         Load the run function in the training script of each model. Training parameter is predefined by the
         algo_config.yaml file, which is pre-filled by the fill_template_config function in the same instance.
 
         Args:
-            train_params:  training parameters
-            device_settings: device related settings, should follow the device_setting in auto_runner.set_device_info.
-            'CUDA_VISIBLE_DEVICES' should be a string e.g. '0,1,2,3'
+            device_setting: device related settings, should follow the device_setting in auto_runner.set_device_info.
+                'CUDA_VISIBLE_DEVICES' should be a string e.g. '0,1,2,3'
         """
         # device_setting set default value and sanity check, in case device_setting not from autorunner
         if device_setting is not None:
             self.device_setting.update(device_setting)
             self.device_setting["n_devices"] = len(str(self.device_setting["CUDA_VISIBLE_DEVICES"]).split(","))
         self._create_cmd()
```

### Comparing `monai-weekly-1.2.dev2319/monai/apps/auto3dseg/hpo_gen.py` & `monai-weekly-1.2.dev2320/monai/apps/auto3dseg/hpo_gen.py`

 * *Files 0% similar despite different names*

```diff
@@ -320,15 +320,15 @@
         """Set the Optuna trial"""
         self.trial = trial
 
     def __call__(
         self, trial: Any, obj_filename: str, output_folder: str = ".", template_path: PathLike | None = None
     ) -> Any:
         """
-        Callabe that Optuna will use to optimize the hyper-parameters
+        Callable that Optuna will use to optimize the hyper-parameters
 
         Args:
             obj_filename: the pickle-exported Algo object.
             output_folder: the root path of the algorithms templates.
             template_path: the algorithm_template. It must contain algo.py in the follow path:
                 ``{algorithm_templates_dir}/{network}/scripts/algo.py``
         """
```

### Comparing `monai-weekly-1.2.dev2319/monai/apps/auto3dseg/transforms.py` & `monai-weekly-1.2.dev2320/monai/apps/auto3dseg/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/auto3dseg/utils.py` & `monai-weekly-1.2.dev2320/monai/apps/auto3dseg/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 import os
 
 from monai.apps.auto3dseg.bundle_gen import BundleAlgo
 from monai.auto3dseg import algo_from_pickle, algo_to_pickle
 from monai.utils.enums import AlgoKeys
 
+__all__ = ["import_bundle_algo_history", "export_bundle_algo_history", "get_name_from_algo_id"]
+
 
 def import_bundle_algo_history(
     output_folder: str = ".", template_path: str | None = None, only_trained: bool = True
 ) -> list:
     """
     import the history of the bundleAlgo objects as a list of algo dicts.
     each algo_dict has keys name (folder name), algo (bundleAlgo), is_trained (bool),
@@ -69,7 +71,20 @@
 
     Args:
         history: a List of Bundle. Typically, the history can be obtained from BundleGen get_history method
     """
     for algo_dict in history:
         algo = algo_dict[AlgoKeys.ALGO]
         algo_to_pickle(algo, template_path=algo.template_path)
+
+
+def get_name_from_algo_id(id: str) -> str:
+    """
+    Get the name of Algo from the identifier of the Algo.
+
+    Args:
+        id: identifier which follows a convention of "name_fold_other".
+
+    Returns:
+        name of the Algo.
+    """
+    return id.split("_")[0]
```

### Comparing `monai-weekly-1.2.dev2319/monai/apps/datasets.py` & `monai-weekly-1.2.dev2320/monai/apps/datasets.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/deepedit/__init__.py` & `monai-weekly-1.2.dev2320/monai/apps/deepedit/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/deepedit/interaction.py` & `monai-weekly-1.2.dev2320/monai/apps/deepedit/interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/deepedit/transforms.py` & `monai-weekly-1.2.dev2320/monai/apps/deepedit/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/deepgrow/__init__.py` & `monai-weekly-1.2.dev2320/monai/apps/deepgrow/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/deepgrow/dataset.py` & `monai-weekly-1.2.dev2320/monai/apps/deepgrow/dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/deepgrow/interaction.py` & `monai-weekly-1.2.dev2320/monai/apps/deepgrow/interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/deepgrow/transforms.py` & `monai-weekly-1.2.dev2320/monai/apps/deepgrow/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/detection/__init__.py` & `monai-weekly-1.2.dev2320/monai/apps/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/detection/metrics/__init__.py` & `monai-weekly-1.2.dev2320/monai/apps/detection/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/detection/metrics/coco.py` & `monai-weekly-1.2.dev2320/monai/apps/detection/metrics/coco.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/detection/metrics/matching.py` & `monai-weekly-1.2.dev2320/monai/apps/detection/metrics/matching.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/detection/networks/__init__.py` & `monai-weekly-1.2.dev2320/monai/apps/detection/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/detection/networks/retinanet_detector.py` & `monai-weekly-1.2.dev2320/monai/apps/detection/networks/retinanet_detector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/detection/networks/retinanet_network.py` & `monai-weekly-1.2.dev2320/monai/apps/detection/networks/retinanet_network.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/detection/transforms/__init__.py` & `monai-weekly-1.2.dev2320/monai/apps/detection/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/detection/transforms/array.py` & `monai-weekly-1.2.dev2320/monai/apps/detection/transforms/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/detection/transforms/box_ops.py` & `monai-weekly-1.2.dev2320/monai/apps/detection/transforms/box_ops.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/detection/transforms/dictionary.py` & `monai-weekly-1.2.dev2320/monai/apps/detection/transforms/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/detection/utils/ATSS_matcher.py` & `monai-weekly-1.2.dev2320/monai/apps/detection/utils/ATSS_matcher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/detection/utils/__init__.py` & `monai-weekly-1.2.dev2320/monai/apps/detection/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/detection/utils/anchor_utils.py` & `monai-weekly-1.2.dev2320/monai/apps/detection/utils/anchor_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/detection/utils/box_coder.py` & `monai-weekly-1.2.dev2320/monai/apps/detection/utils/box_coder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/detection/utils/box_selector.py` & `monai-weekly-1.2.dev2320/monai/apps/detection/utils/box_selector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/detection/utils/detector_utils.py` & `monai-weekly-1.2.dev2320/monai/apps/detection/utils/detector_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/detection/utils/hard_negative_sampler.py` & `monai-weekly-1.2.dev2320/monai/apps/detection/utils/hard_negative_sampler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/detection/utils/predict_utils.py` & `monai-weekly-1.2.dev2320/monai/apps/detection/utils/predict_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/mmars/__init__.py` & `monai-weekly-1.2.dev2320/monai/apps/mmars/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/mmars/mmars.py` & `monai-weekly-1.2.dev2320/monai/apps/mmars/mmars.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/mmars/model_desc.py` & `monai-weekly-1.2.dev2320/monai/apps/mmars/model_desc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/nnunet/__init__.py` & `monai-weekly-1.2.dev2320/monai/apps/nnunet/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/nnunet/__main__.py` & `monai-weekly-1.2.dev2320/monai/apps/nnunet/__main__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/nnunet/nnunetv2_runner.py` & `monai-weekly-1.2.dev2320/monai/apps/nnunet/nnunetv2_runner.py`

 * *Files 9% similar despite different names*

```diff
@@ -60,14 +60,20 @@
             Currently, the configuration supports these optional keys:
             - ``"nnunet_raw"``: File path that will be written to env variable for nnU-Net
             - ``"nnunet_preprocessed"``: File path that will be written to env variable for nnU-Net
             - ``"nnunet_results"``: File path that will be written to env variable for nnU-Net
             - ``"nnUNet_trained_models"``
             - ``"dataset_name_or_id"``: Name or Integer ID of the dataset
             If an optional key is not specified, then the pipeline will use the default values.
+        trainer_class_name: the trainer class names offered by nnUNetV2 exhibit variations in training duration.
+            Default: "nnUNetTrainer". Other options: "nnUNetTrainer_Xepoch". X could be one of 1,5,10,20,50,100,
+            250,2000,4000,8000.
+        export_validation_probabilities: True to save softmax predictions from final validation as npz
+            files (in addition to predicted segmentations). Needed for finding the best ensemble.
+            Default: True.
         work_dir: working directory to save the intermediate and final results.
 
     Examples:
         - Use the one-liner to start the nnU-Net workflow
 
         .. code-block:: bash
 
@@ -111,25 +117,25 @@
                 --trainer_class_name "nnUNetTrainer_5epochs" \\
                 --export_validation_probabilities True
 
         - training for all 20 models (4 configurations by 5 folds) on 2 GPUs
 
         .. code-block:: bash
 
-            python -m monai.apps.nnunet nnUNetV2Runner train --input_config "./input.yaml" --device_ids "(0,1)"
+            python -m monai.apps.nnunet nnUNetV2Runner train --input_config "./input.yaml" --gpu_id_for_all "0,1"
 
         - 5-fold training for a single model on 2 GPUs. Here ``configs`` is used to specify the configurations.
 
         .. code-block:: bash
 
             python -m monai.apps.nnunet nnUNetV2Runner train --input_config "./input.yaml" \\
                 --configs "3d_fullres" \\
                 --trainer_class_name "nnUNetTrainer_5epochs" \\
                 --export_validation_probabilities True \\
-                --device_ids "(0,1)"
+                --gpu_id_for_all "0,1"
 
         - find the best configuration
 
         .. code-block:: bash
 
             python -m monai.apps.nnunet nnUNetV2Runner find_best_configuration --input_config "./input.yaml"
 
@@ -137,17 +143,25 @@
 
         .. code-block:: bash
 
             python -m monai.apps.nnunet nnUNetV2Runner predict_ensemble_postprocessing --input_config "./input.yaml"
 
     """
 
-    def __init__(self, input_config: Any, work_dir: str = "work_dir") -> None:
+    def __init__(
+        self,
+        input_config: Any,
+        trainer_class_name: str = "nnUNetTrainer",
+        work_dir: str = "work_dir",
+        export_validation_probabilities: bool = True,
+    ) -> None:
         self.input_info: dict = {}
         self.input_config_or_dict = input_config
+        self.trainer_class_name = trainer_class_name
+        self.export_validation_probabilities = export_validation_probabilities
         self.work_dir = work_dir
 
         if isinstance(self.input_config_or_dict, dict):
             self.input_info = self.input_config_or_dict
         elif isinstance(self.input_config_or_dict, str) and os.path.isfile(self.input_config_or_dict):
             self.input_info = ConfigParser.load_config_file(self.input_config_or_dict)
         else:
@@ -466,93 +480,132 @@
         """
         self.extract_fingerprints(fpe, npfp, verify_dataset_integrity, clean, verbose)
         self.plan_experiments(pl, gpu_memory_target, preprocessor_name, overwrite_target_spacing, overwrite_plans_name)
 
         if not no_pp:
             self.preprocess(c, n_proc, overwrite_plans_name, verbose)
 
-    def train_single_model(self, config: Any, fold: int, gpu_id: int = 0, **kwargs: Any) -> None:
+    def train_single_model(self, config: Any, fold: int, gpu_id: tuple | list | int = 0, **kwargs: Any) -> None:
         """
         Run the training on a single GPU with one specified configuration provided.
         Note: this will override the environment variable `CUDA_VISIBLE_DEVICES`.
 
         Args:
             config: configuration that should be trained. Examples: "2d", "3d_fullres", "3d_lowres".
             fold: fold of the 5-fold cross-validation. Should be an int between 0 and 4.
-            gpu_id: an integer to select the device to use. Default: 0.
+            gpu_id: an integer to select the device to use, or a tuple/list of GPU device indices used for multi-GPU
+                training (e.g., (0,1)). Default: 0.
         from nnunetv2.run.run_training import run_training
             kwargs: this optional parameter allows you to specify additional arguments in
                 ``nnunetv2.run.run_training.run_training``. Currently supported args are
-                    - trainer_class_name: name of the custom trainer class. Default: "nnUNetTrainer".
                     - plans_identifier: custom plans identifier. Default: "nnUNetPlans".
                     - pretrained_weights: path to nnU-Net checkpoint file to be used as pretrained model. Will only be
                         used when actually training. Beta. Use with caution. Default: False.
                     - use_compressed_data: True to use compressed data for training. Reading compressed data is much
                         more CPU and (potentially) RAM intensive and should only be used if you know what you are
                         doing. Default: False.
-                    - export_validation_probabilities: True to save softmax predictions from final validation as npz
-                        files (in addition to predicted segmentations). Needed for finding the best ensemble.
-                        Default: False.
                     - continue_training: continue training from latest checkpoint. Default: False.
                     - only_run_validation: True to run the validation only. Requires training to have finished.
                         Default: False.
                     - disable_checkpointing: True to disable checkpointing. Ideal for testing things out and you
                         don't want to flood your hard drive with checkpoints. Default: False.
         """
-        os.environ["CUDA_VISIBLE_DEVICES"] = f"{gpu_id}"
+        if "num_gpus" in kwargs:
+            kwargs.pop("num_gpus")
+            logger.warning("please use gpu_id to set the GPUs to use")
+
+        if "trainer_class_name" in kwargs:
+            kwargs.pop("trainer_class_name")
+            logger.warning("please specify the `trainer_class_name` in the __init__ of `nnUNetV2Runner`.")
+
+        if "export_validation_probabilities" in kwargs:
+            kwargs.pop("export_validation_probabilities")
+            logger.warning("please specify the `export_validation_probabilities` in the __init__ of `nnUNetV2Runner`.")
+
+        if isinstance(gpu_id, tuple) or isinstance(gpu_id, list):
+            if len(gpu_id) > 1:
+                gpu_ids_str = ""
+                for _i in range(len(gpu_id)):
+                    gpu_ids_str += f"{gpu_id[_i]},"
+                os.environ["CUDA_VISIBLE_DEVICES"] = gpu_ids_str[:-1]
+            else:
+                os.environ["CUDA_VISIBLE_DEVICES"] = f"{gpu_id[0]}"
+        else:
+            os.environ["CUDA_VISIBLE_DEVICES"] = f"{gpu_id}"
 
         from nnunetv2.run.run_training import run_training
 
-        run_training(dataset_name_or_id=self.dataset_name_or_id, configuration=config, fold=fold, **kwargs)
+        if isinstance(gpu_id, int) or len(gpu_id) == 1:
+            run_training(
+                dataset_name_or_id=self.dataset_name_or_id,
+                configuration=config,
+                fold=fold,
+                trainer_class_name=self.trainer_class_name,
+                export_validation_probabilities=self.export_validation_probabilities,
+                **kwargs,
+            )
+        else:
+            run_training(
+                dataset_name_or_id=self.dataset_name_or_id,
+                configuration=config,
+                fold=fold,
+                num_gpus=len(gpu_id),
+                trainer_class_name=self.trainer_class_name,
+                export_validation_probabilities=self.export_validation_probabilities,
+                **kwargs,
+            )
 
     def train(
         self,
         configs: tuple | str = (M.N_3D_FULLRES, M.N_2D, M.N_3D_LOWRES, M.N_3D_CASCADE_FULLRES),
-        device_ids: tuple | None = None,
+        gpu_id_for_all: tuple | list | int | None = None,
         **kwargs: Any,
     ) -> None:
         """
         Run the training for all the models specified by the configurations.
-        Note: to set the number of GPUs to use, use ``devices_ids`` instead of the `CUDA_VISIBLE_DEVICES`
+        Note: to set the number of GPUs to use, use ``gpu_id_for_all`` instead of the `CUDA_VISIBLE_DEVICES`
         environment variable.
 
         Args:
             configs: configurations that should be trained.
                 Default: ("2d", "3d_fullres", "3d_lowres", "3d_cascade_fullres").
-            device_ids: a tuple/list of GPU device IDs to use for the training. Default: None (all available GPUs).
+            gpu_id_for_all: a tuple/list/integer of GPU device ID(s) to use for the training. Default:
+                None (all available GPUs).
             kwargs: this optional parameter allows you to specify additional arguments defined in the
                 ``train_single_model`` method.
         """
-
-        if device_ids is None:
+        if gpu_id_for_all is None:
             result = subprocess.run(["nvidia-smi", "--list-gpus"], stdout=subprocess.PIPE)
             output = result.stdout.decode("utf-8")
             num_gpus = len(output.strip().split("\n"))
-            device_ids = tuple(range(num_gpus))
-        logger.info(f"number of GPUs is {len(device_ids)}, device ids are {device_ids}")
-        if len(device_ids) > 1:
-            self.train_parallel(configs=ensure_tuple(configs), device_ids=device_ids, **kwargs)
+            gpu_id_for_all = tuple(range(num_gpus))
+        elif isinstance(gpu_id_for_all, int):
+            gpu_id_for_all = ensure_tuple(gpu_id_for_all)
+        logger.info(f"number of GPUs is {len(gpu_id_for_all)}, device ids are {gpu_id_for_all}")
+        if len(gpu_id_for_all) > 1:
+            self.train_parallel(configs=ensure_tuple(configs), gpu_id_for_all=gpu_id_for_all, **kwargs)
         else:
             for cfg in ensure_tuple(configs):
                 for _fold in range(self.num_folds):
-                    self.train_single_model(config=cfg, fold=_fold, **kwargs)
+                    self.train_single_model(config=cfg, fold=_fold, gpu_id=gpu_id_for_all, **kwargs)
 
     def train_parallel_cmd(
         self,
         configs: tuple | str = (M.N_3D_FULLRES, M.N_2D, M.N_3D_LOWRES, M.N_3D_CASCADE_FULLRES),
-        device_ids: tuple | None = None,
+        gpu_id_for_all: tuple | list | int | None = None,
         **kwargs: Any,
     ) -> list:
         """
         Create the line command for subprocess call for parallel training.
 
         Args:
             configs: configurations that should be trained.
                 Default: ("2d", "3d_fullres", "3d_lowres", "3d_cascade_fullres").
-            device_ids: a tuple of GPU device IDs to use for the training. Default: None (all available GPUs).
+            gpu_id_for_all: a tuple/list/integer of GPU device ID(s) to use for the training. Default:
+                None (all available GPUs).
             kwargs: this optional parameter allows you to specify additional arguments defined in the
                 ``train_single_model`` method.
         """
         # unpack compressed files
         folder_names = []
         for root, _, files in os.walk(os.path.join(self.nnunet_preprocessed, self.dataset_name)):
             if any(file.endswith(".npz") for file in files):
@@ -567,71 +620,75 @@
                 unpack_segmentation=True,
                 overwrite_existing=False,
                 num_processes=self.default_num_processes,
             )
 
         # model training
         kwargs = kwargs or {}
-        devices = ensure_tuple(device_ids)
+        devices = ensure_tuple(gpu_id_for_all)
         n_devices = len(devices)
         _configs = [[M.N_3D_FULLRES, M.N_2D, M.N_3D_LOWRES], [M.N_3D_CASCADE_FULLRES]]
         all_cmds: list = []
         for _stage in range(len(_configs)):
             all_cmds.append({_j: [] for _j in devices})
             _index = 0
 
             for _config in _configs[_stage]:
                 if _config in ensure_tuple(configs):
                     for _i in range(self.num_folds):
-                        the_device = device_ids[_index % n_devices]  # type: ignore
+                        the_device = gpu_id_for_all[_index % n_devices]  # type: ignore
                         cmd = (
                             "python -m monai.apps.nnunet nnUNetV2Runner train_single_model "
                             + f"--input_config '{self.input_config_or_dict}' --work_dir '{self.work_dir}' "
-                            + f"--config '{_config}' --fold {_i} --gpu_id {the_device}"
+                            + f"--config '{_config}' --fold {_i} --gpu_id {the_device} "
+                            + f"--trainer_class_name {self.trainer_class_name} "
+                            + f"--export_validation_probabilities {self.export_validation_probabilities}"
                         )
                         for _key, _value in kwargs.items():
                             cmd += f" --{_key} {_value}"
                         all_cmds[-1][the_device].append(cmd)
                         _index += 1
         return all_cmds
 
     def train_parallel(
         self,
         configs: tuple | str = (M.N_3D_FULLRES, M.N_2D, M.N_3D_LOWRES, M.N_3D_CASCADE_FULLRES),
-        device_ids: tuple | None = None,
+        gpu_id_for_all: tuple | list | int | None = None,
         **kwargs: Any,
     ) -> None:
         """
         Create the line command for subprocess call for parallel training.
-        Note: to set the number of GPUs to use, use ``devices_ids`` instead of the `CUDA_VISIBLE_DEVICES`
+        Note: to set the number of GPUs to use, use ``gpu_id_for_all`` instead of the `CUDA_VISIBLE_DEVICES`
         environment variable.
 
         Args:
             configs: configurations that should be trained.
                 default: ("2d", "3d_fullres", "3d_lowres", "3d_cascade_fullres").
-            device_ids: a tuple of GPU device IDs to use for the training. Default: None (all available GPUs).
+            gpu_id_for_all: a tuple/list/integer of GPU device ID(s) to use for the training. Default:
+                None (all available GPUs).
             kwargs: this optional parameter allows you to specify additional arguments defined in the
                 ``train_single_model`` method.
         """
-        all_cmds = self.train_parallel_cmd(configs=configs, device_ids=device_ids, **kwargs)
+        all_cmds = self.train_parallel_cmd(configs=configs, gpu_id_for_all=gpu_id_for_all, **kwargs)
         for s, cmds in enumerate(all_cmds):
             for gpu_id, gpu_cmd in cmds.items():
                 if not gpu_cmd:
                     continue
                 logger.info(
-                    f"\ntraining - stage {s + 1}:\n"
+                    f"training - stage {s + 1}:\n"
                     f"for gpu {gpu_id}, commands: {gpu_cmd}\n"
                     f"log '.txt' inside '{os.path.join(self.nnunet_results, self.dataset_name)}'"
                 )
         for stage in all_cmds:
             processes = []
             for device_id in stage:
                 if not stage[device_id]:
                     continue
                 cmd_str = "; ".join(stage[device_id])
+                logger.info(f"Current running command on GPU device {device_id}:\n{cmd_str}\n")
                 processes.append(subprocess.Popen(cmd_str, shell=True, stdout=subprocess.DEVNULL))
             # finish this stage first
             for p in processes:
                 p.wait()
 
     def validate_single_model(self, config: str, fold: int, **kwargs: Any) -> None:
         """
@@ -661,42 +718,45 @@
             for _fold in range(self.num_folds):
                 self.validate_single_model(config=cfg, fold=_fold, **kwargs)
 
     def find_best_configuration(
         self,
         plans: tuple | str = "nnUNetPlans",
         configs: tuple | str = (M.N_2D, M.N_3D_FULLRES, M.N_3D_LOWRES, M.N_3D_CASCADE_FULLRES),
-        trainers: tuple | str = "nnUNetTrainer",
+        trainers: tuple | str | None = None,
         allow_ensembling: bool = True,
         num_processes: int = -1,
         overwrite: bool = True,
         folds: list[int] | tuple[int, ...] = (0, 1, 2, 3, 4),
         strict: bool = False,
     ) -> None:
         """
         Find the best model configurations.
 
         Args:
             plans: list of plan identifiers. Default: nnUNetPlans.
             configs: list of configurations. Default: ["2d", "3d_fullres", "3d_lowres", "3d_cascade_fullres"].
             trainers: list of trainers. Default: nnUNetTrainer.
-            allow_ensembling: Set this flag to enable ensembling.
+            allow_ensembling: set this flag to enable ensembling.
             num_processes: number of processes to use for ensembling, postprocessing, etc.
-            overwrite: If set we will overwrite already ensembled files etc. May speed up consecutive
+            overwrite: if set we will overwrite already ensembled files etc. May speed up consecutive
                 runs of this command (not recommended) at the risk of not updating outdated results.
             folds: folds to use. Default: (0, 1, 2, 3, 4).
             strict: a switch that triggers RunTimeError if the logging folder cannot be found. Default: False.
         """
         from nnunetv2.evaluation.find_best_configuration import (
             dumb_trainer_config_plans_to_trained_models_dict,
             find_best_configuration,
         )
 
         configs = ensure_tuple(configs)
         plans = ensure_tuple(plans)
+
+        if trainers is None:
+            trainers = self.trainer_class_name
         trainers = ensure_tuple(trainers)
 
         models = dumb_trainer_config_plans_to_trained_models_dict(trainers, configs, plans)
         num_processes = self.default_num_processes if num_processes < 0 else num_processes
         find_best_configuration(
             int(self.dataset_name_or_id),
             models,
```

### Comparing `monai-weekly-1.2.dev2319/monai/apps/nnunet/utils.py` & `monai-weekly-1.2.dev2320/monai/apps/nnunet/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/nuclick/__init__.py` & `monai-weekly-1.2.dev2320/monai/apps/nuclick/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/nuclick/transforms.py` & `monai-weekly-1.2.dev2320/monai/apps/nuclick/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/pathology/__init__.py` & `monai-weekly-1.2.dev2320/monai/apps/pathology/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/pathology/engines/__init__.py` & `monai-weekly-1.2.dev2320/monai/apps/pathology/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/pathology/engines/utils.py` & `monai-weekly-1.2.dev2320/monai/apps/pathology/engines/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/pathology/handlers/__init__.py` & `monai-weekly-1.2.dev2320/monai/apps/pathology/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/pathology/handlers/utils.py` & `monai-weekly-1.2.dev2320/monai/apps/pathology/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/pathology/inferers/__init__.py` & `monai-weekly-1.2.dev2320/monai/apps/pathology/inferers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/pathology/inferers/inferer.py` & `monai-weekly-1.2.dev2320/monai/apps/pathology/inferers/inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/pathology/losses/__init__.py` & `monai-weekly-1.2.dev2320/monai/apps/pathology/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/pathology/losses/hovernet_loss.py` & `monai-weekly-1.2.dev2320/monai/apps/pathology/losses/hovernet_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/pathology/metrics/__init__.py` & `monai-weekly-1.2.dev2320/monai/apps/pathology/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/pathology/metrics/lesion_froc.py` & `monai-weekly-1.2.dev2320/monai/apps/pathology/metrics/lesion_froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/pathology/transforms/__init__.py` & `monai-weekly-1.2.dev2320/monai/apps/pathology/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/pathology/transforms/post/__init__.py` & `monai-weekly-1.2.dev2320/monai/apps/pathology/transforms/post/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/pathology/transforms/post/array.py` & `monai-weekly-1.2.dev2320/monai/apps/pathology/transforms/post/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/pathology/transforms/post/dictionary.py` & `monai-weekly-1.2.dev2320/monai/apps/pathology/transforms/post/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/pathology/transforms/stain/__init__.py` & `monai-weekly-1.2.dev2320/monai/apps/pathology/transforms/stain/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/pathology/transforms/stain/array.py` & `monai-weekly-1.2.dev2320/monai/apps/pathology/transforms/stain/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/pathology/transforms/stain/dictionary.py` & `monai-weekly-1.2.dev2320/monai/apps/pathology/transforms/stain/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/pathology/utils.py` & `monai-weekly-1.2.dev2320/monai/apps/pathology/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/reconstruction/__init__.py` & `monai-weekly-1.2.dev2320/monai/apps/reconstruction/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/reconstruction/complex_utils.py` & `monai-weekly-1.2.dev2320/monai/apps/reconstruction/complex_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/reconstruction/fastmri_reader.py` & `monai-weekly-1.2.dev2320/monai/apps/reconstruction/fastmri_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/reconstruction/mri_utils.py` & `monai-weekly-1.2.dev2320/monai/apps/reconstruction/mri_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/reconstruction/networks/__init__.py` & `monai-weekly-1.2.dev2320/monai/apps/reconstruction/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/reconstruction/networks/blocks/__init__.py` & `monai-weekly-1.2.dev2320/monai/apps/reconstruction/networks/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/reconstruction/networks/blocks/varnetblock.py` & `monai-weekly-1.2.dev2320/monai/apps/reconstruction/networks/blocks/varnetblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/reconstruction/networks/nets/__init__.py` & `monai-weekly-1.2.dev2320/monai/apps/reconstruction/networks/nets/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py` & `monai-weekly-1.2.dev2320/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/reconstruction/networks/nets/complex_unet.py` & `monai-weekly-1.2.dev2320/monai/apps/reconstruction/networks/nets/complex_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/reconstruction/networks/nets/utils.py` & `monai-weekly-1.2.dev2320/monai/apps/reconstruction/networks/nets/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/reconstruction/networks/nets/varnet.py` & `monai-weekly-1.2.dev2320/monai/apps/reconstruction/networks/nets/varnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/reconstruction/transforms/__init__.py` & `monai-weekly-1.2.dev2320/monai/apps/reconstruction/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/reconstruction/transforms/array.py` & `monai-weekly-1.2.dev2320/monai/apps/reconstruction/transforms/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/reconstruction/transforms/dictionary.py` & `monai-weekly-1.2.dev2320/monai/apps/reconstruction/transforms/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/tcia/__init__.py` & `monai-weekly-1.2.dev2320/monai/apps/tcia/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/tcia/label_desc.py` & `monai-weekly-1.2.dev2320/monai/apps/tcia/label_desc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/tcia/utils.py` & `monai-weekly-1.2.dev2320/monai/apps/tcia/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/apps/utils.py` & `monai-weekly-1.2.dev2320/monai/apps/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/auto3dseg/__init__.py` & `monai-weekly-1.2.dev2320/monai/auto3dseg/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/auto3dseg/algo_gen.py` & `monai-weekly-1.2.dev2320/monai/auto3dseg/algo_gen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/auto3dseg/analyzer.py` & `monai-weekly-1.2.dev2320/monai/auto3dseg/analyzer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/auto3dseg/operations.py` & `monai-weekly-1.2.dev2320/monai/auto3dseg/operations.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/auto3dseg/seg_summarizer.py` & `monai-weekly-1.2.dev2320/monai/auto3dseg/seg_summarizer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/auto3dseg/utils.py` & `monai-weekly-1.2.dev2320/monai/auto3dseg/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,15 +308,15 @@
 
     Returns:
         algo: the Algo object saved in the pickle file.
         algo_meta_data: additional keyword saved in the pickle file, for example, acc/best_metrics.
 
     Raises:
         ValueError if the pkl_filename does not contain a dict, or the dict does not contain `algo_bytes`.
-        ModuleNotFoundError if it is unable to instiante the Algo class.
+        ModuleNotFoundError if it is unable to instantiate the Algo class.
 
     """
     with open(pkl_filename, "rb") as f_pi:
         data_bytes = f_pi.read()
     data = pickle.loads(data_bytes)
 
     if not isinstance(data, dict):
```

### Comparing `monai-weekly-1.2.dev2319/monai/bundle/__init__.py` & `monai-weekly-1.2.dev2320/monai/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/bundle/__main__.py` & `monai-weekly-1.2.dev2320/monai/bundle/__main__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/bundle/config_item.py` & `monai-weekly-1.2.dev2320/monai/bundle/config_item.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/bundle/config_parser.py` & `monai-weekly-1.2.dev2320/monai/bundle/config_parser.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/bundle/properties.py` & `monai-weekly-1.2.dev2320/monai/bundle/properties.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/bundle/reference_resolver.py` & `monai-weekly-1.2.dev2320/monai/bundle/reference_resolver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/bundle/scripts.py` & `monai-weekly-1.2.dev2320/monai/bundle/scripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -644,15 +644,15 @@
             https://docs.python.org/3/library/logging.config.html#logging.config.fileConfig.
             Default to "configs/logging.conf", which is commonly used for bundles in MONAI model zoo.
         tracking: if not None, enable the experiment tracking at runtime with optionally configurable and extensible.
             if "mlflow", will add `MLFlowHandler` to the parsed bundle with default tracking settings,
             if other string, treat it as file path to load the tracking settings.
             if `dict`, treat it as tracking settings.
             will patch the target config content with `tracking handlers` and the top-level items of `configs`.
-            for detailed usage examples, plesae check the tutorial:
+            for detailed usage examples, please check the tutorial:
             https://github.com/Project-MONAI/tutorials/blob/main/experiment_management/bundle_integrate_mlflow.ipynb.
         args_file: a JSON or YAML file to provide default values for `runner_id`, `meta_file`,
             `config_file`, `logging`, and override pairs. so that the command line inputs can be simplified.
         override: id-value pairs to override or add the corresponding config content.
             e.g. ``--net#input_chns 42``, ``--net %/data/other.json#net_arg``.
 
     """
@@ -695,15 +695,15 @@
     workflow.run()
     workflow.finalize()
 
 
 def run_workflow(workflow: str | BundleWorkflow | None = None, args_file: str | None = None, **kwargs: Any) -> None:
     """
     Specify `bundle workflow` to run monai bundle components and workflows.
-    The workflow should be suclass of `BundleWorkflow` and be available to import.
+    The workflow should be subclass of `BundleWorkflow` and be available to import.
     It can be MONAI existing bundle workflows or user customized workflows.
 
     Typical usage examples:
 
     .. code-block:: bash
 
         # Execute this module as a CLI entry with default ConfigWorkflow:
@@ -858,14 +858,15 @@
     net_id: str | None = None,
     meta_file: str | Sequence[str] | None = None,
     config_file: str | Sequence[str] | None = None,
     device: str | None = None,
     p: int | None = None,
     n: int | None = None,
     any: int | None = None,
+    extra_forward_args: dict | None = None,
     args_file: str | None = None,
     **override: Any,
 ) -> None:
     """
     Verify the input and output data shape and data type of network defined in the metadata.
     Will test with fake Tensor data according to the required data shape in `metadata`.
 
@@ -881,14 +882,16 @@
             if it is a list of file paths, the content of them will be merged.
         config_file: filepath of the config file to get network definition, if `None`, must be provided in `args_file`.
             if it is a list of file paths, the content of them will be merged.
         device: target device to run the network forward computation, if None, prefer to "cuda" if existing.
         p: power factor to generate fake data shape if dim of expected shape is "x**p", default to 1.
         n: multiply factor to generate fake data shape if dim of expected shape is "x*n", default to 1.
         any: specified size to generate fake data shape if dim of expected shape is "*", default to 1.
+        extra_forward_args: a dictionary that contains other args for the forward function of the network.
+            Default to an empty dictionary.
         args_file: a JSON or YAML file to provide default values for `net_id`, `meta_file`, `config_file`,
             `device`, `p`, `n`, `any`, and override pairs. so that the command line inputs can be simplified.
         override: id-value pairs to override or add the corresponding config content.
             e.g. ``--_meta#network_data_format#inputs#image#num_channels 3``.
 
     """
 
@@ -897,19 +900,28 @@
         net_id=net_id,
         meta_file=meta_file,
         config_file=config_file,
         device=device,
         p=p,
         n=n,
         any=any,
+        extra_forward_args=extra_forward_args,
         **override,
     )
     _log_input_summary(tag="verify_net_in_out", args=_args)
-    config_file_, meta_file_, net_id_, device_, p_, n_, any_ = _pop_args(
-        _args, "config_file", "meta_file", net_id="", device="cuda:0" if is_available() else "cpu", p=1, n=1, any=1
+    config_file_, meta_file_, net_id_, device_, p_, n_, any_, extra_forward_args_ = _pop_args(
+        _args,
+        "config_file",
+        "meta_file",
+        net_id="",
+        device="cuda:0" if is_available() else "cpu",
+        p=1,
+        n=1,
+        any=1,
+        extra_forward_args={},
     )
 
     parser = ConfigParser()
     parser.read_config(f=config_file_)
     parser.read_meta(f=meta_file_)
 
     # the rest key-values in the _args are to override config content
@@ -929,18 +941,18 @@
         test_data = torch.rand(*(1, input_channels, *spatial_shape), dtype=input_dtype, device=device_)
         if input_dtype == torch.float16:
             # fp16 can only be executed in gpu mode
             net.to("cuda")
             from torch.cuda.amp import autocast
 
             with autocast():
-                output = net(test_data.cuda())
+                output = net(test_data.cuda(), **extra_forward_args_)
             net.to(device_)
         else:
-            output = net(test_data)
+            output = net(test_data, **extra_forward_args_)
         if output.shape[1] != output_channels:
             raise ValueError(f"output channel number `{output.shape[1]}` doesn't match: `{output_channels}`.")
         if output.dtype != output_dtype:
             raise ValueError(f"dtype of output data `{output.dtype}` doesn't match: {output_dtype}.")
     logger.info("data shape of network is verified with no error.")
```

### Comparing `monai-weekly-1.2.dev2319/monai/bundle/utils.py` & `monai-weekly-1.2.dev2320/monai/bundle/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/bundle/workflows.py` & `monai-weekly-1.2.dev2320/monai/bundle/workflows.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,16 +128,16 @@
         Get the workflow type, it can be `None`, "train", or "infer".
 
         """
         return self.workflow
 
     def add_property(self, name: str, required: str, desc: str | None = None) -> None:
         """
-        Besides the default predefined properties, some 3rd party aplications may need the bundle
-        definition to provide additonal properties for the specific use cases, if the bundlle can't
+        Besides the default predefined properties, some 3rd party applications may need the bundle
+        definition to provide additional properties for the specific use cases, if the bundle can't
         provide the property, means it can't work with the application.
         This utility adds the property for the application requirements check and access.
 
         Args:
             name: the name of target property.
             required: whether the property is "must-have".
             desc: descriptions for the property.
@@ -179,15 +179,15 @@
             https://docs.python.org/3/library/logging.config.html#logging.config.fileConfig.
             Default to "configs/logging.conf", which is commonly used for bundles in MONAI model zoo.
         tracking: if not None, enable the experiment tracking at runtime with optionally configurable and extensible.
             if "mlflow", will add `MLFlowHandler` to the parsed bundle with default tracking settings,
             if other string, treat it as file path to load the tracking settings.
             if `dict`, treat it as tracking settings.
             will patch the target config content with `tracking handlers` and the top-level items of `configs`.
-            for detailed usage examples, plesae check the tutorial:
+            for detailed usage examples, please check the tutorial:
             https://github.com/Project-MONAI/tutorials/blob/main/experiment_management/bundle_integrate_mlflow.ipynb.
         workflow: specifies the workflow type: "train" or "training" for a training workflow,
             or "infer", "inference", "eval", "evaluation" for a inference workflow,
             other unsupported string will raise a ValueError.
             default to `None` for common workflow.
         override: id-value pairs to override or add the corresponding config content.
             e.g. ``--net#input_chns 42``, ``--net %/data/other.json#net_arg``
@@ -267,16 +267,16 @@
 
         """
         return self._run_expr(id=self.final_id)
 
     def check_properties(self) -> list[str] | None:
         """
         Check whether the required properties are existing in the bundle workflow.
-        If the optional properties have reference in the config, will also check whether the properties are exising.
-        If no workflow type specified, return None, otherwise, return a list of required but missing properites.
+        If the optional properties have reference in the config, will also check whether the properties are existing.
+        If no workflow type specified, return None, otherwise, return a list of required but missing properties.
 
         """
         ret = super().check_properties()
         if self.properties is None:
             warnings.warn("No available properties had been set, skipping check.")
             return None
         if ret:
@@ -335,16 +335,16 @@
             self._is_initialized = False
             self.parser.ref_resolver.reset()
 
     def add_property(  # type: ignore[override]
         self, name: str, required: str, config_id: str, desc: str | None = None
     ) -> None:
         """
-        Besides the default predefined properties, some 3rd party aplications may need the bundle
-        definition to provide additonal properties for the specific use cases, if the bundlle can't
+        Besides the default predefined properties, some 3rd party applications may need the bundle
+        definition to provide additional properties for the specific use cases, if the bundle can't
         provide the property, means it can't work with the application.
         This utility adds the property for the application requirements check and access.
 
         Args:
             name: the name of target property.
             required: whether the property is "must-have".
             config_id: the config ID of target property in the bundle definition.
```

### Comparing `monai-weekly-1.2.dev2319/monai/config/__init__.py` & `monai-weekly-1.2.dev2320/monai/config/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/config/deviceconfig.py` & `monai-weekly-1.2.dev2320/monai/config/deviceconfig.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/config/type_definitions.py` & `monai-weekly-1.2.dev2320/monai/config/type_definitions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/data/__init__.py` & `monai-weekly-1.2.dev2320/monai/data/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/data/box_utils.py` & `monai-weekly-1.2.dev2320/monai/data/box_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/data/csv_saver.py` & `monai-weekly-1.2.dev2320/monai/data/csv_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/data/dataloader.py` & `monai-weekly-1.2.dev2320/monai/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/data/dataset.py` & `monai-weekly-1.2.dev2320/monai/data/dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/data/dataset_summary.py` & `monai-weekly-1.2.dev2320/monai/data/dataset_summary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/data/decathlon_datalist.py` & `monai-weekly-1.2.dev2320/monai/data/decathlon_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/data/fft_utils.py` & `monai-weekly-1.2.dev2320/monai/data/fft_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/data/folder_layout.py` & `monai-weekly-1.2.dev2320/monai/data/folder_layout.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/data/grid_dataset.py` & `monai-weekly-1.2.dev2320/monai/data/grid_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/data/image_dataset.py` & `monai-weekly-1.2.dev2320/monai/data/image_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/data/image_reader.py` & `monai-weekly-1.2.dev2320/monai/data/image_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/data/image_writer.py` & `monai-weekly-1.2.dev2320/monai/data/image_writer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/data/iterable_dataset.py` & `monai-weekly-1.2.dev2320/monai/data/iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/data/itk_torch_bridge.py` & `monai-weekly-1.2.dev2320/monai/data/itk_torch_bridge.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/data/meta_obj.py` & `monai-weekly-1.2.dev2320/monai/data/meta_obj.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/data/meta_tensor.py` & `monai-weekly-1.2.dev2320/monai/data/meta_tensor.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/data/samplers.py` & `monai-weekly-1.2.dev2320/monai/data/samplers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/data/synthetic.py` & `monai-weekly-1.2.dev2320/monai/data/synthetic.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/data/test_time_augmentation.py` & `monai-weekly-1.2.dev2320/monai/data/test_time_augmentation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/data/thread_buffer.py` & `monai-weekly-1.2.dev2320/monai/data/thread_buffer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/data/torchscript_utils.py` & `monai-weekly-1.2.dev2320/monai/data/torchscript_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/data/utils.py` & `monai-weekly-1.2.dev2320/monai/data/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/data/video_dataset.py` & `monai-weekly-1.2.dev2320/monai/data/video_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/data/wsi_datasets.py` & `monai-weekly-1.2.dev2320/monai/data/wsi_datasets.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/data/wsi_reader.py` & `monai-weekly-1.2.dev2320/monai/data/wsi_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -820,15 +820,15 @@
         # Check if the color channel is 3 (RGB) or 4 (RGBA)
         if mode in "RGB":
             if patch.shape[self.channel_dim] not in [3, 4]:
                 raise ValueError(
                     f"The image is expected to have three or four color channels in '{mode}' mode but has "
                     f"{patch.shape[self.channel_dim]}. "
                 )
-            patch = patch[:3]
+            patch = np.take(patch, [0, 1, 2], self.channel_dim)
 
         return patch
 
 
 @require_pkg(pkg_name="openslide")
 class OpenSlideWSIReader(BaseWSIReader):
     """
@@ -1179,10 +1179,10 @@
         # Check if the color channel is 3 (RGB) or 4 (RGBA)
         if mode in "RGB":
             if patch.shape[self.channel_dim] not in [3, 4]:
                 raise ValueError(
                     f"The image is expected to have three or four color channels in '{mode}' mode but has "
                     f"{patch.shape[self.channel_dim]}. "
                 )
-            patch = patch[:3]
+            patch = np.take(patch, [0, 1, 2], self.channel_dim)
 
         return patch
```

### Comparing `monai-weekly-1.2.dev2319/monai/engines/__init__.py` & `monai-weekly-1.2.dev2320/monai/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/engines/evaluator.py` & `monai-weekly-1.2.dev2320/monai/engines/evaluator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/engines/multi_gpu_supervised_trainer.py` & `monai-weekly-1.2.dev2320/monai/engines/multi_gpu_supervised_trainer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/engines/trainer.py` & `monai-weekly-1.2.dev2320/monai/engines/trainer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/engines/utils.py` & `monai-weekly-1.2.dev2320/monai/engines/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/engines/workflow.py` & `monai-weekly-1.2.dev2320/monai/engines/workflow.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/fl/__init__.py` & `monai-weekly-1.2.dev2320/monai/fl/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/fl/client/__init__.py` & `monai-weekly-1.2.dev2320/monai/fl/client/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/fl/client/client_algo.py` & `monai-weekly-1.2.dev2320/monai/fl/client/client_algo.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/fl/client/monai_algo.py` & `monai-weekly-1.2.dev2320/monai/fl/client/monai_algo.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/fl/utils/__init__.py` & `monai-weekly-1.2.dev2320/monai/fl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/fl/utils/constants.py` & `monai-weekly-1.2.dev2320/monai/fl/utils/constants.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/fl/utils/exchange_object.py` & `monai-weekly-1.2.dev2320/monai/fl/utils/exchange_object.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/fl/utils/filters.py` & `monai-weekly-1.2.dev2320/monai/fl/utils/filters.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/__init__.py` & `monai-weekly-1.2.dev2320/monai/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/checkpoint_loader.py` & `monai-weekly-1.2.dev2320/monai/handlers/checkpoint_loader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/checkpoint_saver.py` & `monai-weekly-1.2.dev2320/monai/handlers/checkpoint_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/classification_saver.py` & `monai-weekly-1.2.dev2320/monai/handlers/classification_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/clearml_handlers.py` & `monai-weekly-1.2.dev2320/monai/handlers/clearml_handlers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/confusion_matrix.py` & `monai-weekly-1.2.dev2320/monai/handlers/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/decollate_batch.py` & `monai-weekly-1.2.dev2320/monai/handlers/decollate_batch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/earlystop_handler.py` & `monai-weekly-1.2.dev2320/monai/handlers/earlystop_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/garbage_collector.py` & `monai-weekly-1.2.dev2320/monai/handlers/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/hausdorff_distance.py` & `monai-weekly-1.2.dev2320/monai/handlers/hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/ignite_metric.py` & `monai-weekly-1.2.dev2320/monai/handlers/ignite_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/logfile_handler.py` & `monai-weekly-1.2.dev2320/monai/handlers/logfile_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/lr_schedule_handler.py` & `monai-weekly-1.2.dev2320/monai/handlers/lr_schedule_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/mean_dice.py` & `monai-weekly-1.2.dev2320/monai/handlers/mean_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/mean_iou.py` & `monai-weekly-1.2.dev2320/monai/handlers/mean_iou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/metric_logger.py` & `monai-weekly-1.2.dev2320/monai/handlers/metric_logger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/metrics_reloaded_handler.py` & `monai-weekly-1.2.dev2320/monai/handlers/metrics_reloaded_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/metrics_saver.py` & `monai-weekly-1.2.dev2320/monai/handlers/metrics_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/mlflow_handler.py` & `monai-weekly-1.2.dev2320/monai/handlers/mlflow_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/nvtx_handlers.py` & `monai-weekly-1.2.dev2320/monai/handlers/nvtx_handlers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/panoptic_quality.py` & `monai-weekly-1.2.dev2320/monai/handlers/panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/parameter_scheduler.py` & `monai-weekly-1.2.dev2320/monai/handlers/parameter_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/postprocessing.py` & `monai-weekly-1.2.dev2320/monai/handlers/postprocessing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/probability_maps.py` & `monai-weekly-1.2.dev2320/monai/handlers/probability_maps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/regression_metrics.py` & `monai-weekly-1.2.dev2320/monai/handlers/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/roc_auc.py` & `monai-weekly-1.2.dev2320/monai/handlers/roc_auc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/smartcache_handler.py` & `monai-weekly-1.2.dev2320/monai/handlers/smartcache_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/stats_handler.py` & `monai-weekly-1.2.dev2320/monai/handlers/stats_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/surface_distance.py` & `monai-weekly-1.2.dev2320/monai/handlers/surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/tensorboard_handlers.py` & `monai-weekly-1.2.dev2320/monai/handlers/tensorboard_handlers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/utils.py` & `monai-weekly-1.2.dev2320/monai/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/handlers/validation_handler.py` & `monai-weekly-1.2.dev2320/monai/handlers/validation_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/inferers/__init__.py` & `monai-weekly-1.2.dev2320/monai/inferers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/inferers/inferer.py` & `monai-weekly-1.2.dev2320/monai/inferers/inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/inferers/merger.py` & `monai-weekly-1.2.dev2320/monai/inferers/merger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/inferers/splitter.py` & `monai-weekly-1.2.dev2320/monai/inferers/splitter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/inferers/utils.py` & `monai-weekly-1.2.dev2320/monai/inferers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/losses/__init__.py` & `monai-weekly-1.2.dev2320/monai/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/losses/contrastive.py` & `monai-weekly-1.2.dev2320/monai/losses/contrastive.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/losses/deform.py` & `monai-weekly-1.2.dev2320/monai/losses/deform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/losses/dice.py` & `monai-weekly-1.2.dev2320/monai/losses/dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/losses/ds_loss.py` & `monai-weekly-1.2.dev2320/monai/losses/ds_loss.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+from typing import Union
+
 import torch
 import torch.nn.functional as F
 from torch.nn.modules.loss import _Loss
 
 from monai.utils import pytorch_after
 
 
@@ -66,19 +68,21 @@
         and downsizing targets if necessary (using nearest neighbor interpolation)
         Generally downsizing occurs for all level, except for the first (level==0)
         """
         if input.shape[2:] != target.shape[2:]:
             target = F.interpolate(target, size=input.shape[2:], mode=self.interp_mode)
         return self.loss(input, target)  # type: ignore[no-any-return]
 
-    def forward(self, input: torch.Tensor | list[torch.Tensor], target: torch.Tensor) -> torch.Tensor:
+    def forward(self, input: Union[None, torch.Tensor, list[torch.Tensor]], target: torch.Tensor) -> torch.Tensor:
         if isinstance(input, (list, tuple)):
             weights = self.get_weights(levels=len(input))
             loss = torch.tensor(0, dtype=torch.float, device=target.device)
             for l in range(len(input)):
                 loss += weights[l] * self.get_loss(input[l].float(), target)
             return loss
+        if input is None:
+            raise ValueError("input shouldn't be None.")
 
         return self.loss(input.float(), target)  # type: ignore[no-any-return]
 
 
 ds_loss = DeepSupervisionLoss
```

### Comparing `monai-weekly-1.2.dev2319/monai/losses/focal_loss.py` & `monai-weekly-1.2.dev2320/monai/losses/focal_loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import warnings
 from collections.abc import Sequence
+from typing import Optional
 
 import torch
 import torch.nn.functional as F
 from torch.nn.modules.loss import _Loss
 
 from monai.networks import one_hot
 from monai.utils import LossReduction
@@ -150,15 +151,15 @@
 
         # computing binary cross entropy with logits
         # see also https://github.com/pytorch/pytorch/blob/v1.9.0/aten/src/ATen/native/Loss.cpp#L231
         max_val = (-i).clamp(min=0)
         ce = i - i * t + max_val + ((-max_val).exp() + (-i - max_val).exp()).log()
 
         if self.weight is not None:
-            class_weight: torch.Tensor | None = None
+            class_weight: Optional[torch.Tensor] = None
             if isinstance(self.weight, (float, int)):
                 class_weight = torch.as_tensor([self.weight] * i.size(1))
             else:
                 class_weight = torch.as_tensor(self.weight)
                 if class_weight.size(0) != i.size(1):
                     raise ValueError(
                         "the length of the weight sequence should be the same as the number of classes. "
```

### Comparing `monai-weekly-1.2.dev2319/monai/losses/giou_loss.py` & `monai-weekly-1.2.dev2320/monai/losses/giou_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/losses/image_dissimilarity.py` & `monai-weekly-1.2.dev2320/monai/losses/image_dissimilarity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/losses/multi_scale.py` & `monai-weekly-1.2.dev2320/monai/losses/multi_scale.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/losses/spatial_mask.py` & `monai-weekly-1.2.dev2320/monai/losses/spatial_mask.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 import inspect
 import warnings
 from collections.abc import Callable
-from typing import Any
+from typing import Any, Optional
 
 import torch
 from torch.nn.modules.loss import _Loss
 
 __all__ = ["MaskedLoss"]
 
 
@@ -43,15 +43,15 @@
         super().__init__()
         self.loss: Callable[[torch.Tensor, torch.Tensor], torch.Tensor] = (
             loss(*loss_args, **loss_kwargs) if inspect.isclass(loss) else loss
         )
         if not callable(self.loss):
             raise ValueError("The loss function is not callable.")
 
-    def forward(self, input: torch.Tensor, target: torch.Tensor, mask: torch.Tensor | None = None) -> torch.Tensor:
+    def forward(self, input: torch.Tensor, target: torch.Tensor, mask: Optional[torch.Tensor] = None) -> torch.Tensor:
         """
         Args:
             input: the shape should be BNH[WD].
             target: the shape should be BNH[WD].
             mask: the shape should be B1H[WD] or 11H[WD].
         """
         if mask is None:
```

### Comparing `monai-weekly-1.2.dev2319/monai/losses/ssim_loss.py` & `monai-weekly-1.2.dev2320/monai/losses/ssim_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/losses/tversky.py` & `monai-weekly-1.2.dev2320/monai/losses/tversky.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/losses/unified_focal_loss.py` & `monai-weekly-1.2.dev2320/monai/losses/unified_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/metrics/__init__.py` & `monai-weekly-1.2.dev2320/monai/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/metrics/active_learning_metrics.py` & `monai-weekly-1.2.dev2320/monai/metrics/active_learning_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/metrics/confusion_matrix.py` & `monai-weekly-1.2.dev2320/monai/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/metrics/cumulative_average.py` & `monai-weekly-1.2.dev2320/monai/metrics/cumulative_average.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/metrics/f_beta_score.py` & `monai-weekly-1.2.dev2320/monai/metrics/f_beta_score.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/metrics/froc.py` & `monai-weekly-1.2.dev2320/monai/metrics/froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/metrics/generalized_dice.py` & `monai-weekly-1.2.dev2320/monai/metrics/generalized_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/metrics/hausdorff_distance.py` & `monai-weekly-1.2.dev2320/monai/metrics/hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/metrics/loss_metric.py` & `monai-weekly-1.2.dev2320/monai/metrics/loss_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/metrics/meandice.py` & `monai-weekly-1.2.dev2320/monai/metrics/meandice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/metrics/meaniou.py` & `monai-weekly-1.2.dev2320/monai/metrics/meaniou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/metrics/metric.py` & `monai-weekly-1.2.dev2320/monai/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/metrics/panoptic_quality.py` & `monai-weekly-1.2.dev2320/monai/metrics/panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/metrics/regression.py` & `monai-weekly-1.2.dev2320/monai/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/metrics/rocauc.py` & `monai-weekly-1.2.dev2320/monai/metrics/rocauc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/metrics/surface_dice.py` & `monai-weekly-1.2.dev2320/monai/metrics/surface_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/metrics/surface_distance.py` & `monai-weekly-1.2.dev2320/monai/metrics/surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/metrics/utils.py` & `monai-weekly-1.2.dev2320/monai/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/metrics/wrapper.py` & `monai-weekly-1.2.dev2320/monai/metrics/wrapper.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/__init__.py` & `monai-weekly-1.2.dev2320/monai/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/blocks/__init__.py` & `monai-weekly-1.2.dev2320/monai/networks/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/blocks/acti_norm.py` & `monai-weekly-1.2.dev2320/monai/networks/blocks/acti_norm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/blocks/activation.py` & `monai-weekly-1.2.dev2320/monai/networks/blocks/activation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/blocks/aspp.py` & `monai-weekly-1.2.dev2320/monai/networks/blocks/aspp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/blocks/backbone_fpn_utils.py` & `monai-weekly-1.2.dev2320/monai/networks/blocks/backbone_fpn_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/blocks/convolutions.py` & `monai-weekly-1.2.dev2320/monai/networks/blocks/convolutions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/blocks/crf.py` & `monai-weekly-1.2.dev2320/monai/networks/blocks/crf.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/blocks/denseblock.py` & `monai-weekly-1.2.dev2320/monai/networks/blocks/denseblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/blocks/dints_block.py` & `monai-weekly-1.2.dev2320/monai/networks/blocks/dints_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/blocks/downsample.py` & `monai-weekly-1.2.dev2320/monai/networks/blocks/downsample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/blocks/dynunet_block.py` & `monai-weekly-1.2.dev2320/monai/networks/blocks/dynunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/blocks/encoder.py` & `monai-weekly-1.2.dev2320/monai/networks/blocks/encoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/blocks/fcn.py` & `monai-weekly-1.2.dev2320/monai/networks/blocks/fcn.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/blocks/feature_pyramid_network.py` & `monai-weekly-1.2.dev2320/monai/networks/blocks/feature_pyramid_network.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/blocks/fft_utils_t.py` & `monai-weekly-1.2.dev2320/monai/networks/blocks/fft_utils_t.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/blocks/localnet_block.py` & `monai-weekly-1.2.dev2320/monai/networks/blocks/localnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/blocks/mlp.py` & `monai-weekly-1.2.dev2320/monai/networks/blocks/mlp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/blocks/patchembedding.py` & `monai-weekly-1.2.dev2320/monai/networks/blocks/patchembedding.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/blocks/regunet_block.py` & `monai-weekly-1.2.dev2320/monai/networks/blocks/regunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/blocks/segresnet_block.py` & `monai-weekly-1.2.dev2320/monai/networks/blocks/segresnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/blocks/selfattention.py` & `monai-weekly-1.2.dev2320/monai/networks/blocks/selfattention.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/blocks/squeeze_and_excitation.py` & `monai-weekly-1.2.dev2320/monai/networks/blocks/squeeze_and_excitation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/blocks/text_embedding.py` & `monai-weekly-1.2.dev2320/monai/networks/blocks/text_embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 from __future__ import annotations
 
 import torch
 from torch import nn
 from torch.utils import model_zoo
 
 url_map = {
-    "clip_encoding_univeral_model_32": (
+    "clip_encoding_universal_model_32": (
         "https://github.com/Project-MONAI/MONAI-extra-test-data/"
-        "releases/download/0.8.1/clip_encoding_univeral_model.pth"
+        "releases/download/0.8.1/clip_encoding_universal_model.pth"
     )
 }
 
 
 class TextEncoder(nn.Module):
     """
     Text to vision encoding by Contrastive Language-Image Pre-training (CLIP) or random embedding.
@@ -37,20 +37,20 @@
 
     def __init__(
         self,
         out_channels: int,
         spatial_dims: int = 3,
         text_dim: int = 512,
         hidden_size: int = 256,
-        encoding: str = "clip_encoding_univeral_model_32",
+        encoding: str = "clip_encoding_universal_model_32",
         pretrained: bool = True,
     ) -> None:
         """
         Args:
-            out_channels: number of output channels, to control text-baesd embedding for classes.
+            out_channels: number of output channels, to control text-based embedding for classes.
             spatial_dims: number of spatial dims.
             text_dim: dimension of text embeddings.
             hidden_size: dimension of hidden features, compatible to different vision feature dimensions.
             encoding: the text embedding type, default to use clip text pretrained weights.
             pretrained: whether to load pretrained weights from e.g., (CLIP) to initialize text embeddings, default to False.
         """
         super().__init__()
```

### Comparing `monai-weekly-1.2.dev2319/monai/networks/blocks/transformerblock.py` & `monai-weekly-1.2.dev2320/monai/networks/blocks/transformerblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/blocks/unetr_block.py` & `monai-weekly-1.2.dev2320/monai/networks/blocks/unetr_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/blocks/upsample.py` & `monai-weekly-1.2.dev2320/monai/networks/blocks/upsample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/blocks/warp.py` & `monai-weekly-1.2.dev2320/monai/networks/blocks/warp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/layers/__init__.py` & `monai-weekly-1.2.dev2320/monai/networks/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/layers/convutils.py` & `monai-weekly-1.2.dev2320/monai/networks/layers/convutils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/layers/drop_path.py` & `monai-weekly-1.2.dev2320/monai/networks/layers/drop_path.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/layers/factories.py` & `monai-weekly-1.2.dev2320/monai/networks/layers/factories.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/layers/filtering.py` & `monai-weekly-1.2.dev2320/monai/networks/layers/filtering.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/layers/gmm.py` & `monai-weekly-1.2.dev2320/monai/networks/layers/gmm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/layers/simplelayers.py` & `monai-weekly-1.2.dev2320/monai/networks/layers/simplelayers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/layers/spatial_transforms.py` & `monai-weekly-1.2.dev2320/monai/networks/layers/spatial_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/layers/utils.py` & `monai-weekly-1.2.dev2320/monai/networks/layers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/layers/weight_init.py` & `monai-weekly-1.2.dev2320/monai/networks/layers/weight_init.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/__init__.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/ahnet.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/ahnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import math
 from collections.abc import Sequence
+from typing import Union
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from monai.networks.blocks.fcn import FCN
 from monai.networks.layers.factories import Act, Conv, Norm, Pool
@@ -275,15 +276,15 @@
         if self.upsample_mode == "transpose":
             for project_module, pool_module, up_module in zip(self.project_modules, self.pool_modules, self.up_modules):
                 output = up_module(project_module(pool_module(x)))
                 outputs.append(output)
         else:
             for project_module, pool_module in zip(self.project_modules, self.pool_modules):
                 interpolate_size = x.shape[2:]
-                align_corners: bool | None = None
+                align_corners: Union[bool, None] = None
                 if self.upsample_mode in ["trilinear", "bilinear"]:
                     align_corners = True
                 output = F.interpolate(
                     project_module(pool_module(x)),
                     size=interpolate_size,
                     mode=self.upsample_mode,
                     align_corners=align_corners,
```

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/attentionunet.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/attentionunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/autoencoder.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/autoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/basic_unet.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/basic_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/basic_unetplusplus.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/basic_unetplusplus.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/classifier.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/classifier.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/densenet.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/densenet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/dints.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/dints.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/dynunet.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/dynunet.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,19 +265,18 @@
         else:
             self.filters = filters[: len(self.strides)]
 
     def forward(self, x):
         out = self.skip_layers(x)
         out = self.output_block(out)
         if self.training and self.deep_supervision:
-            out_all = torch.zeros(out.shape[0], len(self.heads) + 1, *out.shape[1:], device=out.device, dtype=out.dtype)
-            out_all[:, 0] = out
-            for idx, feature_map in enumerate(self.heads):
-                out_all[:, idx + 1] = interpolate(feature_map, out.shape[2:])
-            return out_all
+            out_all = [out]
+            for feature_map in self.heads:
+                out_all.append(interpolate(feature_map, out.shape[2:]))
+            return torch.stack(out_all, dim=1)
         return out
 
     def get_input_block(self):
         return self.conv_block(
             self.spatial_dims,
             self.in_channels,
             self.filters[0],
```

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/efficientnet.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/efficientnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/flexible_unet.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/flexible_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/fullyconnectednet.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/fullyconnectednet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/generator.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/generator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/highresnet.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/highresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/hovernet.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/milmodel.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/milmodel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/netadapter.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/netadapter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/regressor.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/regressor.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/regunet.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/regunet.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             in_channels: number of input channels
             num_channel_initial: number of initial channels
             depth: input is at level 0, bottom is at level depth.
             out_kernel_initializer: kernel initializer for the last layer
             out_activation: activation at the last layer
             out_channels: number of channels for the output
             extract_levels: list, which levels from net to extract. The maximum level must equal to ``depth``
-            pooling: for down-sampling, use non-parameterized pooling if true, otherwise use conv3d
+            pooling: for down-sampling, use non-parameterized pooling if true, otherwise use conv
             concat_skip: when up-sampling, concatenate skipped tensor if true, otherwise use addition
             encode_kernel_sizes: kernel size for down-sampling
         """
         super().__init__()
         if not extract_levels:
             extract_levels = (depth,)
         if max(extract_levels) != depth:
@@ -230,15 +230,30 @@
             outs.append(decoded)
 
         out = self.output_block(outs, image_size=image_size)
         return out
 
 
 class AffineHead(nn.Module):
-    def __init__(self, spatial_dims: int, image_size: list[int], decode_size: list[int], in_channels: int):
+    def __init__(
+        self,
+        spatial_dims: int,
+        image_size: list[int],
+        decode_size: list[int],
+        in_channels: int,
+        save_theta: bool = False,
+    ):
+        """
+        Args:
+            spatial_dims: number of spatial dimensions
+            image_size: output spatial size
+            decode_size: input spatial size (two or three integers depending on ``spatial_dims``)
+            in_channels: number of input channels
+            save_theta: whether to save the theta matrix estimation
+        """
         super().__init__()
         self.spatial_dims = spatial_dims
         if spatial_dims == 2:
             in_features = in_channels * decode_size[0] * decode_size[1]
             out_features = 6
             out_init = torch.tensor([1, 0, 0, 0, 1, 0], dtype=torch.float)
         elif spatial_dims == 3:
@@ -251,14 +266,17 @@
         self.fc = nn.Linear(in_features=in_features, out_features=out_features)
         self.grid = self.get_reference_grid(image_size)  # (spatial_dims, ...)
 
         # init weight/bias
         self.fc.weight.data.zero_()
         self.fc.bias.data.copy_(out_init)
 
+        self.save_theta = save_theta
+        self.theta = torch.Tensor()
+
     @staticmethod
     def get_reference_grid(image_size: tuple[int] | list[int]) -> torch.Tensor:
         mesh_points = [torch.arange(0, dim) for dim in image_size]
         grid = torch.stack(meshgrid_ij(*mesh_points), dim=0)  # (spatial_dims, ...)
         return grid.to(dtype=torch.float)
 
     def affine_transform(self, theta: torch.Tensor):
@@ -274,14 +292,16 @@
             raise ValueError(f"do not support spatial_dims={self.spatial_dims}")
         return grid_warped
 
     def forward(self, x: list[torch.Tensor], image_size: list[int]) -> torch.Tensor:
         f = x[0]
         self.grid = self.grid.to(device=f.device)
         theta = self.fc(f.reshape(f.shape[0], -1))
+        if self.save_theta:
+            self.theta = theta.detach()
         out: torch.Tensor = self.affine_transform(theta) - self.grid
         return out
 
 
 class GlobalNet(RegUNet):
     """
     Build GlobalNet for image registration.
@@ -301,24 +321,40 @@
         num_channel_initial: int,
         depth: int,
         out_kernel_initializer: str | None = "kaiming_uniform",
         out_activation: str | None = None,
         pooling: bool = True,
         concat_skip: bool = False,
         encode_kernel_sizes: int | list[int] = 3,
+        save_theta: bool = False,
     ):
+        """
+        Args:
+            image_size: output displacement field spatial size
+            spatial_dims: number of spatial dims
+            in_channels: number of input channels
+            num_channel_initial: number of initial channels
+            depth: input is at level 0, bottom is at level depth.
+            out_kernel_initializer: kernel initializer for the last layer
+            out_activation: activation at the last layer
+            pooling: for down-sampling, use non-parameterized pooling if true, otherwise use conv
+            concat_skip: when up-sampling, concatenate skipped tensor if true, otherwise use addition
+            encode_kernel_sizes: kernel size for down-sampling
+            save_theta: whether to save the theta matrix estimation
+        """
         for size in image_size:
             if size % (2**depth) != 0:
                 raise ValueError(
                     f"given depth {depth}, "
                     f"all input spatial dimension must be divisible by {2 ** depth}, "
                     f"got input of size {image_size}"
                 )
         self.image_size = image_size
         self.decode_size = [size // (2**depth) for size in image_size]
+        self.save_theta = save_theta
         super().__init__(
             spatial_dims=spatial_dims,
             in_channels=in_channels,
             num_channel_initial=num_channel_initial,
             depth=depth,
             out_kernel_initializer=out_kernel_initializer,
             out_activation=out_activation,
@@ -330,14 +366,15 @@
 
     def build_output_block(self):
         return AffineHead(
             spatial_dims=self.spatial_dims,
             image_size=self.image_size,
             decode_size=self.decode_size,
             in_channels=self.num_channels[-1],
+            save_theta=self.save_theta,
         )
 
 
 class AdditiveUpSampleBlock(nn.Module):
     def __init__(
         self,
         spatial_dims: int,
```

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/resnet.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/resnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/segresnet.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/segresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/segresnet_ds.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/segresnet_ds.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 from collections.abc import Callable
+from typing import Union
 
 import numpy as np
 import torch
 import torch.nn as nn
 
 from monai.networks.blocks.upsample import UpSample
 from monai.networks.layers.factories import Act, Conv, Norm, split_args
@@ -383,15 +384,15 @@
     def is_valid_shape(self, x):
         """
         Calculate if the input shape is divisible by the minimum factors for the current network configuration
         """
         a = [i % j == 0 for i, j in zip(x.shape[2:], self.shape_factor())]
         return all(a)
 
-    def _forward(self, x: torch.Tensor) -> torch.Tensor | list[torch.Tensor]:
+    def _forward(self, x: torch.Tensor) -> Union[None, torch.Tensor, list[torch.Tensor]]:
         if self.preprocess is not None:
             x = self.preprocess(x)
 
         if not self.is_valid_shape(x):
             raise ValueError(f"Input spatial dims {x.shape} must be divisible by {self.shape_factor()}")
 
         x_down = self.encoder(x)
@@ -419,9 +420,9 @@
         # in eval() mode, always return a single final output
         if not self.training or len(outputs) == 1:
             return outputs[0]
 
         # return a list of DS outputs
         return outputs
 
-    def forward(self, x: torch.Tensor) -> torch.Tensor | list[torch.Tensor]:
+    def forward(self, x: torch.Tensor) -> Union[None, torch.Tensor, list[torch.Tensor]]:
         return self._forward(x)
```

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/senet.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/senet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/swin_unetr.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/swin_unetr.py`

 * *Files 0% similar despite different names*

```diff
@@ -942,15 +942,15 @@
             norm_layer: normalization layer.
             patch_norm: add normalization after patch embedding.
             use_checkpoint: use gradient checkpointing for reduced memory usage.
             spatial_dims: spatial dimension.
             downsample: module used for downsampling, available options are `"mergingv2"`, `"merging"` and a
                 user-specified `nn.Module` following the API defined in :py:class:`monai.networks.nets.PatchMerging`.
                 The default is currently `"merging"` (the original version defined in v0.9.0).
-            use_v2: using swinunetr_v2, which adds a residual convolution block at the beggining of each swin stage.
+            use_v2: using swinunetr_v2, which adds a residual convolution block at the beginning of each swin stage.
         """
 
         super().__init__()
         self.num_layers = len(depths)
         self.embed_dim = embed_dim
         self.patch_norm = patch_norm
         self.window_size = window_size
```

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/torchvision_fc.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/torchvision_fc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/transchex.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/transchex.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/unet.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/unetr.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/unetr.py`

 * *Files 15% similar despite different names*

```diff
@@ -39,31 +39,33 @@
         pos_embed: str = "conv",
         norm_name: tuple | str = "instance",
         conv_block: bool = True,
         res_block: bool = True,
         dropout_rate: float = 0.0,
         spatial_dims: int = 3,
         qkv_bias: bool = False,
+        save_attn: bool = False,
     ) -> None:
         """
         Args:
             in_channels: dimension of input channels.
             out_channels: dimension of output channels.
             img_size: dimension of input image.
-            feature_size: dimension of network feature size.
-            hidden_size: dimension of hidden layer.
-            mlp_dim: dimension of feedforward layer.
-            num_heads: number of attention heads.
-            pos_embed: position embedding layer type.
-            norm_name: feature normalization type and arguments.
-            conv_block: bool argument to determine if convolutional block is used.
-            res_block: bool argument to determine if residual block is used.
-            dropout_rate: faction of the input units to drop.
-            spatial_dims: number of spatial dims.
-            qkv_bias: apply the bias term for the qkv linear layer in self attention block
+            feature_size: dimension of network feature size. Defaults to 16.
+            hidden_size: dimension of hidden layer. Defaults to 768.
+            mlp_dim: dimension of feedforward layer. Defaults to 3072.
+            num_heads: number of attention heads. Defaults to 12.
+            pos_embed: position embedding layer type. Defaults to "conv".
+            norm_name: feature normalization type and arguments. Defaults to "instance".
+            conv_block: if convolutional block is used. Defaults to True.
+            res_block: if residual block is used. Defaults to True.
+            dropout_rate: fraction of the input units to drop. Defaults to 0.0.
+            spatial_dims: number of spatial dims. Defaults to 3.
+            qkv_bias: apply the bias term for the qkv linear layer in self attention block. Defaults to False.
+            save_attn: to make accessible the attention in self attention block. Defaults to False.
 
         Examples::
 
             # for single channel input 4-channel output with image size of (96,96,96), feature size of 32 and batch norm
             >>> net = UNETR(in_channels=1, out_channels=4, img_size=(96,96,96), feature_size=32, norm_name='batch')
 
              # for single channel input 4-channel output with image size of (96,96), feature size of 32 and batch norm
@@ -97,14 +99,15 @@
             num_layers=self.num_layers,
             num_heads=num_heads,
             pos_embed=pos_embed,
             classification=self.classification,
             dropout_rate=dropout_rate,
             spatial_dims=spatial_dims,
             qkv_bias=qkv_bias,
+            save_attn=save_attn,
         )
         self.encoder1 = UnetrBasicBlock(
             spatial_dims=spatial_dims,
             in_channels=in_channels,
             out_channels=feature_size,
             kernel_size=3,
             stride=1,
```

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/varautoencoder.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/varautoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/vit.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/vit.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/vitautoenc.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/vitautoenc.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,29 +42,33 @@
         hidden_size: int = 768,
         mlp_dim: int = 3072,
         num_layers: int = 12,
         num_heads: int = 12,
         pos_embed: str = "conv",
         dropout_rate: float = 0.0,
         spatial_dims: int = 3,
+        qkv_bias: bool = False,
+        save_attn: bool = False,
     ) -> None:
         """
         Args:
-            in_channels: dimension of input channels or the number of channels for input
+            in_channels: dimension of input channels or the number of channels for input.
             img_size: dimension of input image.
-            patch_size: dimension of patch size.
-            hidden_size: dimension of hidden layer.
-            out_channels: number of output channels.
-            deconv_chns: number of channels for the deconvolution layers.
-            mlp_dim: dimension of feedforward layer.
-            num_layers: number of transformer blocks.
-            num_heads: number of attention heads.
-            pos_embed: position embedding layer type.
-            dropout_rate: faction of the input units to drop.
-            spatial_dims: number of spatial dimensions.
+            patch_size: dimension of patch size
+            out_channels:  number of output channels. Defaults to 1.
+            deconv_chns: number of channels for the deconvolution layers. Defaults to 16.
+            hidden_size: dimension of hidden layer. Defaults to 768.
+            mlp_dim: dimension of feedforward layer. Defaults to 3072.
+            num_layers:  number of transformer blocks. Defaults to 12.
+            num_heads: number of attention heads. Defaults to 12.
+            pos_embed: position embedding layer type. Defaults to "conv".
+            dropout_rate: faction of the input units to drop. Defaults to 0.0.
+            spatial_dims: number of spatial dimensions. Defaults to 3.
+            qkv_bias: apply bias to the qkv linear layer in self attention block. Defaults to False.
+            save_attn: to make accessible the attention in self attention block. Defaults to False. Defaults to False.
 
         Examples::
 
             # for single channel input with image size of (96,96,96), conv position embedding and segmentation backbone
             # It will provide an output of same size as that of the input
             >>> net = ViTAutoEnc(in_channels=1, patch_size=(16,16,16), img_size=(96,96,96), pos_embed='conv')
 
@@ -85,15 +89,18 @@
             hidden_size=hidden_size,
             num_heads=num_heads,
             pos_embed=pos_embed,
             dropout_rate=dropout_rate,
             spatial_dims=self.spatial_dims,
         )
         self.blocks = nn.ModuleList(
-            [TransformerBlock(hidden_size, mlp_dim, num_heads, dropout_rate) for i in range(num_layers)]
+            [
+                TransformerBlock(hidden_size, mlp_dim, num_heads, dropout_rate, qkv_bias, save_attn)
+                for i in range(num_layers)
+            ]
         )
         self.norm = nn.LayerNorm(hidden_size)
 
         new_patch_size = [4] * self.spatial_dims
         conv_trans = Conv[Conv.CONVTRANS, self.spatial_dims]
         # self.conv3d_transpose* is to be compatible with existing 3d model weights.
         self.conv3d_transpose = conv_trans(hidden_size, deconv_chns, kernel_size=new_patch_size, stride=new_patch_size)
```

### Comparing `monai-weekly-1.2.dev2319/monai/networks/nets/vnet.py` & `monai-weekly-1.2.dev2320/monai/networks/nets/vnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/networks/utils.py` & `monai-weekly-1.2.dev2320/monai/networks/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -691,15 +691,17 @@
             onnx_out = ort_sess.run(None, input_dict)
         else:
             sess = onnxreference.ReferenceEvaluator(onnx_model)
             onnx_out = sess.run(None, input_dict)
         set_determinism(seed=None)
         # compare onnx/ort and PyTorch results
         for r1, r2 in zip(torch_out, onnx_out):
-            torch.testing.assert_allclose(r1.cpu(), r2, rtol=rtol, atol=atol)
+            if isinstance(r1, torch.Tensor):
+                assert_fn = torch.testing.assert_close if pytorch_after(1, 11) else torch.testing.assert_allclose
+                assert_fn(r1.cpu(), convert_to_tensor(r2, dtype=r1.dtype), rtol=rtol, atol=atol)  # type: ignore
 
     return onnx_model
 
 
 def convert_to_torchscript(
     model: nn.Module,
     filename_or_obj: Any | None = None,
```

### Comparing `monai-weekly-1.2.dev2319/monai/optimizers/__init__.py` & `monai-weekly-1.2.dev2320/monai/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/optimizers/lr_finder.py` & `monai-weekly-1.2.dev2320/monai/optimizers/lr_finder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/optimizers/lr_scheduler.py` & `monai-weekly-1.2.dev2320/monai/optimizers/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/optimizers/novograd.py` & `monai-weekly-1.2.dev2320/monai/optimizers/novograd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/optimizers/utils.py` & `monai-weekly-1.2.dev2320/monai/optimizers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/__init__.py` & `monai-weekly-1.2.dev2320/monai/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/adaptors.py` & `monai-weekly-1.2.dev2320/monai/transforms/adaptors.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/compose.py` & `monai-weekly-1.2.dev2320/monai/transforms/compose.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/croppad/__init__.py` & `monai-weekly-1.2.dev2320/monai/transforms/croppad/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/croppad/array.py` & `monai-weekly-1.2.dev2320/monai/transforms/croppad/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/croppad/batch.py` & `monai-weekly-1.2.dev2320/monai/transforms/croppad/batch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/croppad/dictionary.py` & `monai-weekly-1.2.dev2320/monai/transforms/croppad/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/croppad/functional.py` & `monai-weekly-1.2.dev2320/monai/transforms/croppad/functional.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/intensity/__init__.py` & `monai-weekly-1.2.dev2320/monai/transforms/intensity/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/intensity/array.py` & `monai-weekly-1.2.dev2320/monai/transforms/intensity/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/intensity/dictionary.py` & `monai-weekly-1.2.dev2320/monai/transforms/intensity/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/inverse.py` & `monai-weekly-1.2.dev2320/monai/transforms/inverse.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/inverse_batch_transform.py` & `monai-weekly-1.2.dev2320/monai/transforms/inverse_batch_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/io/__init__.py` & `monai-weekly-1.2.dev2320/monai/transforms/io/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/io/array.py` & `monai-weekly-1.2.dev2320/monai/transforms/io/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/io/dictionary.py` & `monai-weekly-1.2.dev2320/monai/transforms/io/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/lazy/__init__.py` & `monai-weekly-1.2.dev2320/monai/transforms/lazy/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/lazy/functional.py` & `monai-weekly-1.2.dev2320/monai/transforms/lazy/functional.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/lazy/utils.py` & `monai-weekly-1.2.dev2320/monai/transforms/lazy/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/meta_utility/__init__.py` & `monai-weekly-1.2.dev2320/monai/transforms/meta_utility/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/meta_utility/dictionary.py` & `monai-weekly-1.2.dev2320/monai/transforms/meta_utility/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/nvtx.py` & `monai-weekly-1.2.dev2320/monai/transforms/nvtx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/post/__init__.py` & `monai-weekly-1.2.dev2320/monai/transforms/post/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/post/array.py` & `monai-weekly-1.2.dev2320/monai/transforms/post/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/post/dictionary.py` & `monai-weekly-1.2.dev2320/monai/transforms/post/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/signal/__init__.py` & `monai-weekly-1.2.dev2320/monai/transforms/signal/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/signal/array.py` & `monai-weekly-1.2.dev2320/monai/transforms/signal/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/smooth_field/__init__.py` & `monai-weekly-1.2.dev2320/monai/transforms/smooth_field/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/smooth_field/array.py` & `monai-weekly-1.2.dev2320/monai/transforms/smooth_field/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/smooth_field/dictionary.py` & `monai-weekly-1.2.dev2320/monai/transforms/smooth_field/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/spatial/__init__.py` & `monai-weekly-1.2.dev2320/monai/transforms/spatial/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/spatial/array.py` & `monai-weekly-1.2.dev2320/monai/transforms/spatial/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/spatial/dictionary.py` & `monai-weekly-1.2.dev2320/monai/transforms/spatial/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/spatial/functional.py` & `monai-weekly-1.2.dev2320/monai/transforms/spatial/functional.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/traits.py` & `monai-weekly-1.2.dev2320/monai/transforms/traits.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/transform.py` & `monai-weekly-1.2.dev2320/monai/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/utility/__init__.py` & `monai-weekly-1.2.dev2320/monai/transforms/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/utility/array.py` & `monai-weekly-1.2.dev2320/monai/transforms/utility/array.py`

 * *Files 0% similar despite different names*

```diff
@@ -1649,17 +1649,17 @@
                 f"{type(filter)} is not supported."
                 "Supported types are `class 'str'`, `class 'torch.Tensor'`, `class 'np.ndarray'`, "
                 "`class 'torch.nn.modules.module.Module'`, `class 'monai.transforms.Transform'`"
             )
 
     def _check_kwargs_are_present(self, filter, **kwargs):
         if filter == "gauss" and "sigma" not in kwargs.keys():
-            raise KeyError("`filter='gauss', requires the additonal keyword argument `sigma`")
+            raise KeyError("`filter='gauss', requires the additional keyword argument `sigma`")
         if filter == "savitzky_golay" and "order" not in kwargs.keys():
-            raise KeyError("`filter='savitzky_golay', requires the additonal keyword argument `order`")
+            raise KeyError("`filter='savitzky_golay', requires the additional keyword argument `order`")
 
     def _get_filter_from_string(self, filter: str, size: int, ndim: int) -> nn.Module | Callable:
         if filter == "mean":
             return MeanFilter(ndim, size)
         elif filter == "laplace":
             return LaplaceFilter(ndim, size)
         elif filter == "elliptical":
```

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/utility/dictionary.py` & `monai-weekly-1.2.dev2320/monai/transforms/utility/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/utils.py` & `monai-weekly-1.2.dev2320/monai/transforms/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1409,15 +1409,15 @@
         return {
             k: convert_applied_interp_mode(trans_info[k], mode=mode, align_corners=align_corners) for k in trans_info
         }
     return trans_info
 
 
 def reset_ops_id(data):
-    """find MetaTensors in list or dict `data` and (in-place) set ``TraceKeys.ID`` to ``Tracekys.NONE``."""
+    """find MetaTensors in list or dict `data` and (in-place) set ``TraceKeys.ID`` to ``Tracekeys.NONE``."""
     if isinstance(data, (list, tuple)):
         return [reset_ops_id(d) for d in data]
     if isinstance(data, monai.data.MetaTensor):
         data.applied_operations = reset_ops_id(data.applied_operations)
         return data
     if not isinstance(data, Mapping):
         return data
@@ -1927,15 +1927,15 @@
     Automatically adjust the resampling interpolation mode and padding mode,
     so that they are compatible with the corresponding API of the `backend`.
     Depending on the availability of the backends, when there's no exact
     equivalent, a similar mode is returned.
 
     Args:
         interp_mode: interpolation mode.
-        padding_mdoe: padding mode.
+        padding_mode: padding mode.
         backend: optional backend of `TransformBackends`. If None, the backend will be decided from `interp_mode`.
         kwargs: additional keyword arguments. currently support ``torch_interpolate_spatial_nd``, to provide
             additional information to determine ``linear``, ``bilinear`` and ``trilinear``;
             ``use_compiled`` to use MONAI's precompiled backend (pytorch c++ extensions), default to ``False``.
     """
     _interp_mode, _padding_mode, _kwargs = None, None, (kwargs or {}).copy()
     if backend is None:  # infer backend
```

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/utils_create_transform_ims.py` & `monai-weekly-1.2.dev2320/monai/transforms/utils_create_transform_ims.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/transforms/utils_pytorch_numpy_unification.py` & `monai-weekly-1.2.dev2320/monai/transforms/utils_pytorch_numpy_unification.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/utils/__init__.py` & `monai-weekly-1.2.dev2320/monai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/utils/aliases.py` & `monai-weekly-1.2.dev2320/monai/utils/aliases.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/utils/decorators.py` & `monai-weekly-1.2.dev2320/monai/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/utils/deprecate_utils.py` & `monai-weekly-1.2.dev2320/monai/utils/deprecate_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/utils/dist.py` & `monai-weekly-1.2.dev2320/monai/utils/dist.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,14 +194,14 @@
     def __init__(self, rank: int | None = None, filter_fn: Callable = lambda rank: rank == 0):
         super().__init__()
         self.filter_fn: Callable = filter_fn
         if dist.is_available() and dist.is_initialized():
             self.rank: int = rank if rank is not None else dist.get_rank()
         else:
             warnings.warn(
-                "The torch.distributed is either unavailable and uninitiated when RankFilter is instiantiated. "
+                "The torch.distributed is either unavailable and uninitiated when RankFilter is instantiated. "
                 "If torch.distributed is used, please ensure that the RankFilter() is called "
                 "after torch.distributed.init_process_group() in the script."
             )
 
     def filter(self, *_args):
         return self.filter_fn(self.rank)
```

### Comparing `monai-weekly-1.2.dev2319/monai/utils/enums.py` & `monai-weekly-1.2.dev2320/monai/utils/enums.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/utils/jupyter_utils.py` & `monai-weekly-1.2.dev2320/monai/utils/jupyter_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/utils/misc.py` & `monai-weekly-1.2.dev2320/monai/utils/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -808,15 +808,15 @@
     Check if the all keys in kwargs exist in the __init__ method of the class.
 
     Args:
         cls: the class to check.
         kwargs: kwargs to examine.
 
     Returns:
-        a boolean inidicating if all keys exist.
+        a boolean indicating if all keys exist.
         a set of extra keys that are not used in the __init__.
     """
     init_signature = inspect.signature(cls.__init__)
     init_params = set(init_signature.parameters) - {"self"}  # Exclude 'self' from the parameter list
     input_kwargs = set(kwargs)
     extra_kwargs = input_kwargs - init_params
```

### Comparing `monai-weekly-1.2.dev2319/monai/utils/module.py` & `monai-weekly-1.2.dev2320/monai/utils/module.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/utils/nvtx.py` & `monai-weekly-1.2.dev2320/monai/utils/nvtx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/utils/profiling.py` & `monai-weekly-1.2.dev2320/monai/utils/profiling.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/utils/state_cacher.py` & `monai-weekly-1.2.dev2320/monai/utils/state_cacher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/utils/type_conversion.py` & `monai-weekly-1.2.dev2320/monai/utils/type_conversion.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/visualize/__init__.py` & `monai-weekly-1.2.dev2320/monai/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/visualize/class_activation_maps.py` & `monai-weekly-1.2.dev2320/monai/visualize/class_activation_maps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/visualize/gradient_based.py` & `monai-weekly-1.2.dev2320/monai/visualize/gradient_based.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 
         return total_gradients / self.n_samples
 
 
 class GuidedBackpropGrad(VanillaGrad):
     """
     Based on Springenberg and Dosovitskiy et al. https://arxiv.org/abs/1412.6806,
-    compute gradient-based saliency maps by backpropagating positive graidents and inputs (see ``_AutoGradReLU``).
+    compute gradient-based saliency maps by backpropagating positive gradients and inputs (see ``_AutoGradReLU``).
 
     See also:
 
         - Springenberg and Dosovitskiy et al. Striving for Simplicity: The All Convolutional Net
           (https://arxiv.org/abs/1412.6806)
     """
```

### Comparing `monai-weekly-1.2.dev2319/monai/visualize/img2tensorboard.py` & `monai-weekly-1.2.dev2320/monai/visualize/img2tensorboard.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/visualize/occlusion_sensitivity.py` & `monai-weekly-1.2.dev2320/monai/visualize/occlusion_sensitivity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/visualize/utils.py` & `monai-weekly-1.2.dev2320/monai/visualize/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai/visualize/visualizer.py` & `monai-weekly-1.2.dev2320/monai/visualize/visualizer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai_weekly.egg-info/PKG-INFO` & `monai-weekly-1.2.dev2320/monai_weekly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monai-weekly
-Version: 1.2.dev2319
+Version: 1.2.dev2320
 Summary: AI Toolkit for Healthcare Imaging
 Home-page: https://monai.io/
 Author: MONAI Consortium
 Author-email: monai.contact@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.monai.io/
 Project-URL: Bug Tracker, https://github.com/Project-MONAI/MONAI/issues
```

### Comparing `monai-weekly-1.2.dev2319/monai_weekly.egg-info/SOURCES.txt` & `monai-weekly-1.2.dev2320/monai_weekly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/monai_weekly.egg-info/requires.txt` & `monai-weekly-1.2.dev2320/monai_weekly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/pyproject.toml` & `monai-weekly-1.2.dev2320/pyproject.toml`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/setup.cfg` & `monai-weekly-1.2.dev2320/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,15 @@
 	W504
 	C408
 	N812
 	B023
 	B905
 	B028
 	B907
+	B908
 per_file_ignores = __init__.py: F401, __main__.py: F401
 exclude = *.pyi,.git,.eggs,monai/_version.py,versioneer.py,venv,.venv,_version.py
 
 [isort]
 known_first_party = monai
 profile = black
 line_length = 120
```

### Comparing `monai-weekly-1.2.dev2319/setup.py` & `monai-weekly-1.2.dev2320/setup.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_acn_block.py` & `monai-weekly-1.2.dev2320/tests/test_acn_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_activations.py` & `monai-weekly-1.2.dev2320/tests/test_activations.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_activationsd.py` & `monai-weekly-1.2.dev2320/tests/test_activationsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_adaptors.py` & `monai-weekly-1.2.dev2320/tests/test_adaptors.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_add_channeld.py` & `monai-weekly-1.2.dev2320/tests/test_add_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_add_coordinate_channels.py` & `monai-weekly-1.2.dev2320/tests/test_add_coordinate_channels.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_add_coordinate_channelsd.py` & `monai-weekly-1.2.dev2320/tests/test_add_coordinate_channelsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_add_extreme_points_channel.py` & `monai-weekly-1.2.dev2320/tests/test_add_extreme_points_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_add_extreme_points_channeld.py` & `monai-weekly-1.2.dev2320/tests/test_add_extreme_points_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_adjust_contrast.py` & `monai-weekly-1.2.dev2320/tests/test_adjust_contrast.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_adjust_contrastd.py` & `monai-weekly-1.2.dev2320/tests/test_adjust_contrastd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_adn.py` & `monai-weekly-1.2.dev2320/tests/test_adn.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_affine.py` & `monai-weekly-1.2.dev2320/tests/test_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_affine_grid.py` & `monai-weekly-1.2.dev2320/tests/test_affine_grid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_affine_transform.py` & `monai-weekly-1.2.dev2320/tests/test_affine_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_affined.py` & `monai-weekly-1.2.dev2320/tests/test_affined.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_ahnet.py` & `monai-weekly-1.2.dev2320/tests/test_ahnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_alias.py` & `monai-weekly-1.2.dev2320/tests/test_alias.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_anchor_box.py` & `monai-weekly-1.2.dev2320/tests/test_anchor_box.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_apply.py` & `monai-weekly-1.2.dev2320/tests/test_apply.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_apply_filter.py` & `monai-weekly-1.2.dev2320/tests/test_apply_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_arraydataset.py` & `monai-weekly-1.2.dev2320/tests/test_arraydataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_as_channel_first.py` & `monai-weekly-1.2.dev2320/tests/test_as_channel_first.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_as_channel_firstd.py` & `monai-weekly-1.2.dev2320/tests/test_as_channel_firstd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_as_channel_last.py` & `monai-weekly-1.2.dev2320/tests/test_as_channel_last.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_as_channel_lastd.py` & `monai-weekly-1.2.dev2320/tests/test_as_channel_lastd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_as_discrete.py` & `monai-weekly-1.2.dev2320/tests/test_as_discrete.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_as_discreted.py` & `monai-weekly-1.2.dev2320/tests/test_as_discreted.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_atss_box_matcher.py` & `monai-weekly-1.2.dev2320/tests/test_atss_box_matcher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_attentionunet.py` & `monai-weekly-1.2.dev2320/tests/test_attentionunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_auto3dseg.py` & `monai-weekly-1.2.dev2320/tests/test_auto3dseg.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_auto3dseg_bundlegen.py` & `monai-weekly-1.2.dev2320/tests/test_auto3dseg_bundlegen.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import os
 import shutil
+import sys
 import tempfile
 import unittest
 
 import nibabel as nib
 import numpy as np
 import torch
 
@@ -122,26 +123,28 @@
             "dataroot": dataroot_dir,
             "multigpu": False,
             "class_names": ["label_class"],
         }
         data_src_cfg = os.path.join(work_dir, "data_src_cfg.yaml")
         ConfigParser.export_config_file(data_src, data_src_cfg)
 
+        sys_path = sys.path.copy()
         with skip_if_downloading_fails():
             bundle_generator = BundleGen(
                 algo_path=work_dir,
                 data_stats_filename=datastats_file,
                 data_src_cfg_name=data_src_cfg,
                 templates_path_or_url=get_testing_algo_template_path(),
             )
 
         bundle_generator.generate(work_dir, num_fold=1)
         history_before = bundle_generator.get_history()
         export_bundle_algo_history(history_before)
 
+        sys.path = sys_path  # prevent the import_bundle_algo_history from using the path "work_dir/algorithm_templates"
         tempfile.TemporaryDirectory()
         work_dir_new = os.path.join(test_path, "workdir_2")
         shutil.move(work_dir, work_dir_new)
         history_after = import_bundle_algo_history(work_dir_new, only_trained=False)
         self.assertEqual(len(history_before), len(history_after))
 
     def tearDown(self) -> None:
```

### Comparing `monai-weekly-1.2.dev2319/tests/test_auto3dseg_ensemble.py` & `monai-weekly-1.2.dev2320/tests/test_auto3dseg_ensemble.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     BundleGen,
     DataAnalyzer,
     EnsembleRunner,
 )
 from monai.bundle.config_parser import ConfigParser
 from monai.data import create_test_image_3d
 from monai.transforms import SaveImage
-from monai.utils import optional_import, set_determinism
+from monai.utils import check_parent_dir, optional_import, set_determinism
 from monai.utils.enums import AlgoKeys
 from tests.utils import (
     SkipIfBeforePyTorchVersion,
     get_testing_algo_template_path,
     skip_if_downloading_fails,
     skip_if_no_cuda,
     skip_if_quick,
@@ -42,20 +42,20 @@
 
 _, has_tb = optional_import("torch.utils.tensorboard", name="SummaryWriter")
 
 num_images_perfold = max(torch.cuda.device_count(), 4)
 num_images_per_batch = 2
 
 fake_datalist: dict[str, list[dict]] = {
-    "testing": [{"image": f"ts_image_{idx:03d}.nii.gz"} for idx in range(num_images_perfold)],
+    "testing": [{"image": f"imagesTs/ts_image_{idx:03d}.nii.gz"} for idx in range(num_images_perfold)],
     "training": [
         {
             "fold": f,
-            "image": f"tr_image_{(f * num_images_perfold + idx):03d}.nii.gz",
-            "label": f"tr_label_{(f * num_images_perfold + idx):03d}.nii.gz",
+            "image": f"imagesTr/tr_image_{(f * num_images_perfold + idx):03d}.nii.gz",
+            "label": f"labelsTr/tr_label_{(f * num_images_perfold + idx):03d}.nii.gz",
         }
         for f in range(num_images_per_batch + 1)
         for idx in range(num_images_perfold)
     ],
 }
 
 train_param = (
@@ -68,52 +68,69 @@
         "pretrained_path": "",
         "determ": True,
     }
     if torch.cuda.is_available()
     else {}
 )
 
-pred_param = {"files_slices": slice(0, 1), "mode": "mean", "sigmoid": True}
+pred_param = {
+    "files_slices": slice(0, 1),
+    "mode": "mean",
+    "sigmoid": True,
+    "algo_spec_params": {"segresnet": {"network#init_filters": 8}, "swinunetr": {"network#feature_size": 12}},
+}
+
+
+def create_sim_data(dataroot, sim_datalist, sim_dim, **kwargs):
+    """
+    Create simulated data using create_test_image_3d.
+
+    Args:
+        dataroot: data directory path that hosts the "nii.gz" image files.
+        sim_datalist: a list of data to create.
+        sim_dim: the image sizes, e.g. a tuple of (64, 64, 64).
+    """
+    if not os.path.isdir(dataroot):
+        os.makedirs(dataroot)
+
+    # Generate a fake dataset
+    for d in sim_datalist["testing"] + sim_datalist["training"]:
+        im, seg = create_test_image_3d(sim_dim[0], sim_dim[1], sim_dim[2], **kwargs)
+        nib_image = nib.Nifti1Image(im, affine=np.eye(4))
+        image_fpath = os.path.join(dataroot, d["image"])
+        check_parent_dir(image_fpath)
+        nib.save(nib_image, image_fpath)
+
+        if "label" in d:
+            nib_image = nib.Nifti1Image(seg, affine=np.eye(4))
+            label_fpath = os.path.join(dataroot, d["label"])
+            check_parent_dir(label_fpath)
+            nib.save(nib_image, label_fpath)
 
 
 @skip_if_quick
+@skip_if_no_cuda
 @SkipIfBeforePyTorchVersion((1, 11, 1))
 @unittest.skipIf(not has_tb, "no tensorboard summary writer")
 class TestEnsembleBuilder(unittest.TestCase):
     def setUp(self) -> None:
         set_determinism(0)
         self.test_dir = tempfile.TemporaryDirectory()
-
-    @skip_if_no_cuda
-    def test_ensemble(self) -> None:
         test_path = self.test_dir.name
 
         dataroot = os.path.join(test_path, "dataroot")
         work_dir = os.path.join(test_path, "workdir")
 
         da_output_yaml = os.path.join(work_dir, "datastats.yaml")
         data_src_cfg = os.path.join(work_dir, "data_src_cfg.yaml")
 
-        if not os.path.isdir(dataroot):
-            os.makedirs(dataroot)
-
         if not os.path.isdir(work_dir):
             os.makedirs(work_dir)
 
-        # Generate a fake dataset
-        for d in fake_datalist["testing"] + fake_datalist["training"]:
-            im, seg = create_test_image_3d(24, 24, 24, rad_max=10, num_seg_classes=1)
-            nib_image = nib.Nifti1Image(im, affine=np.eye(4))
-            image_fpath = os.path.join(dataroot, d["image"])
-            nib.save(nib_image, image_fpath)
-
-            if "label" in d:
-                nib_image = nib.Nifti1Image(seg, affine=np.eye(4))
-                label_fpath = os.path.join(dataroot, d["label"])
-                nib.save(nib_image, label_fpath)
+        create_sim_data(dataroot, fake_datalist, (24, 24, 24), rad_max=10, rad_min=1, num_seg_classes=1)
 
         # write to a json file
         fake_json_datalist = os.path.join(dataroot, "fake_input.json")
         ConfigParser.export_config_file(fake_datalist, fake_json_datalist)
 
         da = DataAnalyzer(fake_json_datalist, dataroot, output_path=da_output_yaml)
         da.get_all_case_stats()
@@ -126,53 +143,53 @@
             "dataroot": dataroot,
             "multigpu": False,
             "class_names": ["label_class"],
         }
 
         ConfigParser.export_config_file(data_src, data_src_cfg)
 
+        self.da_output_yaml = da_output_yaml
+        self.work_dir = work_dir
+        self.data_src_cfg_name = data_src_cfg
+
+    def test_ensemble(self) -> None:
         with skip_if_downloading_fails():
             bundle_generator = BundleGen(
-                algo_path=work_dir,
-                data_stats_filename=da_output_yaml,
-                data_src_cfg_name=data_src_cfg,
+                algo_path=self.work_dir,
+                data_stats_filename=self.da_output_yaml,
+                data_src_cfg_name=self.data_src_cfg_name,
                 templates_path_or_url=get_testing_algo_template_path(),
             )
-        bundle_generator.generate(work_dir, num_fold=1)
+        bundle_generator.generate(self.work_dir, num_fold=1)
         history = bundle_generator.get_history()
 
         for algo_dict in history:
             name = algo_dict[AlgoKeys.ID]
             algo = algo_dict[AlgoKeys.ALGO]
             _train_param = train_param.copy()
             if name.startswith("segresnet"):
                 _train_param["network#init_filters"] = 8
                 _train_param["pretrained_ckpt_name"] = ""
             elif name.startswith("swinunetr"):
                 _train_param["network#feature_size"] = 12
             algo.train(_train_param)
 
-        builder = AlgoEnsembleBuilder(history, data_src_cfg)
+        builder = AlgoEnsembleBuilder(history, data_src_cfg_name=self.data_src_cfg_name)
         builder.set_ensemble_method(AlgoEnsembleBestN(n_best=1))
         ensemble = builder.get_ensemble()
-        name = ensemble.get_algo_ensemble()[0][AlgoKeys.ID]
-        if name.startswith("segresnet"):
-            pred_param["network#init_filters"] = 8
-        elif name.startswith("swinunetr"):
-            pred_param["network#feature_size"] = 12
         preds = ensemble(pred_param)
         self.assertTupleEqual(preds[0].shape, (2, 24, 24, 24))
 
         builder.set_ensemble_method(AlgoEnsembleBestByFold(1))
         ensemble = builder.get_ensemble()
         for algo in ensemble.get_algo_ensemble():
             print(algo[AlgoKeys.ID])
 
     def test_ensemble_runner(self) -> None:
-        runner = EnsembleRunner()
+        runner = EnsembleRunner(data_src_cfg_name=self.data_src_cfg_name, mgpu=False)
         runner.set_num_fold(3)
         self.assertTrue(runner.num_fold == 3)
         runner.set_ensemble_method(ensemble_method_name="AlgoEnsembleBestByFold")
         self.assertIsInstance(runner.ensemble_method, AlgoEnsembleBestByFold)
         self.assertTrue(runner.ensemble_method.n_fold == 3)  # type: ignore
 
         runner.set_ensemble_method(ensemble_method_name="AlgoEnsembleBestN", n_best=3)
```

### Comparing `monai-weekly-1.2.dev2319/tests/test_auto3dseg_hpo.py` & `monai-weekly-1.2.dev2320/tests/test_auto3dseg_hpo.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_autoencoder.py` & `monai-weekly-1.2.dev2320/tests/test_autoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_avg_merger.py` & `monai-weekly-1.2.dev2320/tests/test_avg_merger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_basic_unet.py` & `monai-weekly-1.2.dev2320/tests/test_basic_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_basic_unetplusplus.py` & `monai-weekly-1.2.dev2320/tests/test_basic_unetplusplus.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_bending_energy.py` & `monai-weekly-1.2.dev2320/tests/test_bending_energy.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_bilateral_approx_cpu.py` & `monai-weekly-1.2.dev2320/tests/test_bilateral_approx_cpu.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_bilateral_approx_cuda.py` & `monai-weekly-1.2.dev2320/tests/test_bilateral_approx_cuda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_bilateral_precise.py` & `monai-weekly-1.2.dev2320/tests/test_bilateral_precise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_blend_images.py` & `monai-weekly-1.2.dev2320/tests/test_blend_images.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_border_pad.py` & `monai-weekly-1.2.dev2320/tests/test_border_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_border_padd.py` & `monai-weekly-1.2.dev2320/tests/test_border_padd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_bounding_rect.py` & `monai-weekly-1.2.dev2320/tests/test_bounding_rect.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_bounding_rectd.py` & `monai-weekly-1.2.dev2320/tests/test_bounding_rectd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_box_coder.py` & `monai-weekly-1.2.dev2320/tests/test_box_coder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_box_transform.py` & `monai-weekly-1.2.dev2320/tests/test_box_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_box_utils.py` & `monai-weekly-1.2.dev2320/tests/test_box_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_bundle_ckpt_export.py` & `monai-weekly-1.2.dev2320/tests/test_bundle_ckpt_export.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_bundle_download.py` & `monai-weekly-1.2.dev2320/tests/test_bundle_download.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_bundle_get_data.py` & `monai-weekly-1.2.dev2320/tests/test_bundle_get_data.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_bundle_init_bundle.py` & `monai-weekly-1.2.dev2320/tests/test_bundle_init_bundle.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_bundle_onnx_export.py` & `monai-weekly-1.2.dev2320/tests/test_bundle_onnx_export.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_bundle_trt_export.py` & `monai-weekly-1.2.dev2320/tests/test_bundle_trt_export.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_bundle_utils.py` & `monai-weekly-1.2.dev2320/tests/test_bundle_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_bundle_verify_metadata.py` & `monai-weekly-1.2.dev2320/tests/test_bundle_verify_metadata.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_bundle_verify_net.py` & `monai-weekly-1.2.dev2320/tests/test_bundle_verify_net.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import os
 import tempfile
 import unittest
 
 from parameterized import parameterized
 
-from monai.bundle import ConfigParser
+from monai.bundle import ConfigParser, verify_net_in_out
 from tests.utils import command_line_tests, skip_if_no_cuda, skip_if_windows
 
 TEST_CASE_1 = [
     os.path.join(os.path.dirname(__file__), "testing_data", "metadata.json"),
     os.path.join(os.path.dirname(__file__), "testing_data", "inference.json"),
 ]
 
@@ -51,10 +51,23 @@
             cmd = ["coverage", "run", "-m", "monai.bundle", "verify_net_in_out", "network_def", "--meta_file"]
             cmd += [meta_file, "--config_file", config_file, "-n", "4", "--any", "16", "--args_file", def_args_file]
             cmd += ["--device", "cuda", "--_meta_#network_data_format#inputs#image#spatial_shape", "[16,'*','2**p*n']"]
             cmd += ["--_meta_#network_data_format#inputs#image#dtype", "float16"]
             cmd += ["--_meta_#network_data_format#outputs#pred#dtype", "float16"]
             command_line_tests(cmd)
 
+    @parameterized.expand([TEST_CASE_1])
+    @skip_if_no_cuda
+    def test_verify_fp16_extra_forward_args(self, meta_file, config_file):
+        verify_net_in_out(
+            net_id="network_def",
+            meta_file=meta_file,
+            config_file=config_file,
+            n=4,
+            any=16,
+            extra_forward_args={"extra_arg1": 1, "extra_arg2": 2},
+            **{"network_def#_target_": "tests.testing_data.bundle_test_network.TestMultiInputUNet"},
+        )
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2319/tests/test_bundle_workflow.py` & `monai-weekly-1.2.dev2320/tests/test_bundle_workflow.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_cachedataset.py` & `monai-weekly-1.2.dev2320/tests/test_cachedataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_cachedataset_parallel.py` & `monai-weekly-1.2.dev2320/tests/test_cachedataset_parallel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_cachedataset_persistent_workers.py` & `monai-weekly-1.2.dev2320/tests/test_cachedataset_persistent_workers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_cachentransdataset.py` & `monai-weekly-1.2.dev2320/tests/test_cachentransdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_call_dist.py` & `monai-weekly-1.2.dev2320/tests/test_call_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_cast_to_type.py` & `monai-weekly-1.2.dev2320/tests/test_cast_to_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_cast_to_typed.py` & `monai-weekly-1.2.dev2320/tests/test_cast_to_typed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_center_scale_crop.py` & `monai-weekly-1.2.dev2320/tests/test_center_scale_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_center_scale_cropd.py` & `monai-weekly-1.2.dev2320/tests/test_center_scale_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_center_spatial_crop.py` & `monai-weekly-1.2.dev2320/tests/test_center_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_center_spatial_cropd.py` & `monai-weekly-1.2.dev2320/tests/test_center_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_channel_pad.py` & `monai-weekly-1.2.dev2320/tests/test_channel_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_check_hash.py` & `monai-weekly-1.2.dev2320/tests/test_check_hash.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_check_missing_files.py` & `monai-weekly-1.2.dev2320/tests/test_check_missing_files.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_classes_to_indices.py` & `monai-weekly-1.2.dev2320/tests/test_classes_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_classes_to_indicesd.py` & `monai-weekly-1.2.dev2320/tests/test_classes_to_indicesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_complex_utils.py` & `monai-weekly-1.2.dev2320/tests/test_complex_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_component_locator.py` & `monai-weekly-1.2.dev2320/tests/test_component_locator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_compose.py` & `monai-weekly-1.2.dev2320/tests/test_compose.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_compose_get_number_conversions.py` & `monai-weekly-1.2.dev2320/tests/test_compose_get_number_conversions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_compute_confusion_matrix.py` & `monai-weekly-1.2.dev2320/tests/test_compute_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_compute_f_beta.py` & `monai-weekly-1.2.dev2320/tests/test_compute_f_beta.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_compute_froc.py` & `monai-weekly-1.2.dev2320/tests/test_compute_froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_compute_generalized_dice.py` & `monai-weekly-1.2.dev2320/tests/test_compute_generalized_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_compute_ho_ver_maps.py` & `monai-weekly-1.2.dev2320/tests/test_compute_ho_ver_maps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_compute_ho_ver_maps_d.py` & `monai-weekly-1.2.dev2320/tests/test_compute_ho_ver_maps_d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_compute_meandice.py` & `monai-weekly-1.2.dev2320/tests/test_compute_meandice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_compute_meaniou.py` & `monai-weekly-1.2.dev2320/tests/test_compute_meaniou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_compute_panoptic_quality.py` & `monai-weekly-1.2.dev2320/tests/test_compute_panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_compute_regression_metrics.py` & `monai-weekly-1.2.dev2320/tests/test_compute_regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_compute_roc_auc.py` & `monai-weekly-1.2.dev2320/tests/test_compute_roc_auc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_compute_variance.py` & `monai-weekly-1.2.dev2320/tests/test_compute_variance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_concat_itemsd.py` & `monai-weekly-1.2.dev2320/tests/test_concat_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_config_item.py` & `monai-weekly-1.2.dev2320/tests/test_config_item.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_config_parser.py` & `monai-weekly-1.2.dev2320/tests/test_config_parser.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_contrastive_loss.py` & `monai-weekly-1.2.dev2320/tests/test_contrastive_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_convert_data_type.py` & `monai-weekly-1.2.dev2320/tests/test_convert_data_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_convert_to_multi_channel.py` & `monai-weekly-1.2.dev2320/tests/test_convert_to_multi_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_convert_to_multi_channeld.py` & `monai-weekly-1.2.dev2320/tests/test_convert_to_multi_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_convert_to_onnx.py` & `monai-weekly-1.2.dev2320/tests/test_convert_to_onnx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_convert_to_torchscript.py` & `monai-weekly-1.2.dev2320/tests/test_convert_to_torchscript.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_convert_to_trt.py` & `monai-weekly-1.2.dev2320/tests/test_convert_to_trt.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_convolutions.py` & `monai-weekly-1.2.dev2320/tests/test_convolutions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_copy_itemsd.py` & `monai-weekly-1.2.dev2320/tests/test_copy_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_copy_model_state.py` & `monai-weekly-1.2.dev2320/tests/test_copy_model_state.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_correct_crop_centers.py` & `monai-weekly-1.2.dev2320/tests/test_correct_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_create_cross_validation_datalist.py` & `monai-weekly-1.2.dev2320/tests/test_create_cross_validation_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_create_grid_and_affine.py` & `monai-weekly-1.2.dev2320/tests/test_create_grid_and_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_crf_cpu.py` & `monai-weekly-1.2.dev2320/tests/test_crf_cpu.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_crf_cuda.py` & `monai-weekly-1.2.dev2320/tests/test_crf_cuda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_crop_foreground.py` & `monai-weekly-1.2.dev2320/tests/test_crop_foreground.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_crop_foregroundd.py` & `monai-weekly-1.2.dev2320/tests/test_crop_foregroundd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_cross_validation.py` & `monai-weekly-1.2.dev2320/tests/test_cross_validation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_csv_dataset.py` & `monai-weekly-1.2.dev2320/tests/test_csv_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_csv_iterable_dataset.py` & `monai-weekly-1.2.dev2320/tests/test_csv_iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_csv_saver.py` & `monai-weekly-1.2.dev2320/tests/test_csv_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_cucim_dict_transform.py` & `monai-weekly-1.2.dev2320/tests/test_cucim_dict_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_cucim_transform.py` & `monai-weekly-1.2.dev2320/tests/test_cucim_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_cumulative.py` & `monai-weekly-1.2.dev2320/tests/test_cumulative.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_cumulative_average.py` & `monai-weekly-1.2.dev2320/tests/test_cumulative_average.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_cumulative_average_dist.py` & `monai-weekly-1.2.dev2320/tests/test_cumulative_average_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_cv2_dist.py` & `monai-weekly-1.2.dev2320/tests/test_cv2_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_data_stats.py` & `monai-weekly-1.2.dev2320/tests/test_data_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_data_statsd.py` & `monai-weekly-1.2.dev2320/tests/test_data_statsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_dataloader.py` & `monai-weekly-1.2.dev2320/tests/test_dataloader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_dataset.py` & `monai-weekly-1.2.dev2320/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_dataset_func.py` & `monai-weekly-1.2.dev2320/tests/test_dataset_func.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_dataset_summary.py` & `monai-weekly-1.2.dev2320/tests/test_dataset_summary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_decathlondataset.py` & `monai-weekly-1.2.dev2320/tests/test_decathlondataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_decollate.py` & `monai-weekly-1.2.dev2320/tests/test_decollate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_deepedit_interaction.py` & `monai-weekly-1.2.dev2320/tests/test_deepedit_interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_deepedit_transforms.py` & `monai-weekly-1.2.dev2320/tests/test_deepedit_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_deepgrow_dataset.py` & `monai-weekly-1.2.dev2320/tests/test_deepgrow_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_deepgrow_interaction.py` & `monai-weekly-1.2.dev2320/tests/test_deepgrow_interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_deepgrow_transforms.py` & `monai-weekly-1.2.dev2320/tests/test_deepgrow_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_delete_itemsd.py` & `monai-weekly-1.2.dev2320/tests/test_delete_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_denseblock.py` & `monai-weekly-1.2.dev2320/tests/test_denseblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_densenet.py` & `monai-weekly-1.2.dev2320/tests/test_densenet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_deprecated.py` & `monai-weekly-1.2.dev2320/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_detect_envelope.py` & `monai-weekly-1.2.dev2320/tests/test_detect_envelope.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_detection_coco_metrics.py` & `monai-weekly-1.2.dev2320/tests/test_detection_coco_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_detector_boxselector.py` & `monai-weekly-1.2.dev2320/tests/test_detector_boxselector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_detector_utils.py` & `monai-weekly-1.2.dev2320/tests/test_detector_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_dev_collate.py` & `monai-weekly-1.2.dev2320/tests/test_dev_collate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_dice_ce_loss.py` & `monai-weekly-1.2.dev2320/tests/test_dice_ce_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_dice_focal_loss.py` & `monai-weekly-1.2.dev2320/tests/test_dice_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_dice_loss.py` & `monai-weekly-1.2.dev2320/tests/test_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_dints_cell.py` & `monai-weekly-1.2.dev2320/tests/test_dints_cell.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_dints_mixop.py` & `monai-weekly-1.2.dev2320/tests/test_dints_mixop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_dints_network.py` & `monai-weekly-1.2.dev2320/tests/test_dints_network.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_discriminator.py` & `monai-weekly-1.2.dev2320/tests/test_discriminator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_divisible_pad.py` & `monai-weekly-1.2.dev2320/tests/test_divisible_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_divisible_padd.py` & `monai-weekly-1.2.dev2320/tests/test_divisible_padd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_download_and_extract.py` & `monai-weekly-1.2.dev2320/tests/test_download_and_extract.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_downsample_block.py` & `monai-weekly-1.2.dev2320/tests/test_downsample_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_drop_path.py` & `monai-weekly-1.2.dev2320/tests/test_drop_path.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_ds_loss.py` & `monai-weekly-1.2.dev2320/tests/test_ds_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_dvf2ddf.py` & `monai-weekly-1.2.dev2320/tests/test_dvf2ddf.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_dynunet.py` & `monai-weekly-1.2.dev2320/tests/test_dynunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_dynunet_block.py` & `monai-weekly-1.2.dev2320/tests/test_dynunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_efficientnet.py` & `monai-weekly-1.2.dev2320/tests/test_efficientnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_ensemble_evaluator.py` & `monai-weekly-1.2.dev2320/tests/test_ensemble_evaluator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_ensure_channel_first.py` & `monai-weekly-1.2.dev2320/tests/test_ensure_channel_first.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_ensure_channel_firstd.py` & `monai-weekly-1.2.dev2320/tests/test_ensure_channel_firstd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_ensure_tuple.py` & `monai-weekly-1.2.dev2320/tests/test_ensure_tuple.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_ensure_type.py` & `monai-weekly-1.2.dev2320/tests/test_ensure_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_ensure_typed.py` & `monai-weekly-1.2.dev2320/tests/test_ensure_typed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_enum_bound_interp.py` & `monai-weekly-1.2.dev2320/tests/test_enum_bound_interp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_eval_mode.py` & `monai-weekly-1.2.dev2320/tests/test_eval_mode.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_evenly_divisible_all_gather_dist.py` & `monai-weekly-1.2.dev2320/tests/test_evenly_divisible_all_gather_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_factorized_increase.py` & `monai-weekly-1.2.dev2320/tests/test_factorized_increase.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_factorized_reduce.py` & `monai-weekly-1.2.dev2320/tests/test_factorized_reduce.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_fastmri_reader.py` & `monai-weekly-1.2.dev2320/tests/test_fastmri_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_fft_utils.py` & `monai-weekly-1.2.dev2320/tests/test_fft_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_fg_bg_to_indices.py` & `monai-weekly-1.2.dev2320/tests/test_fg_bg_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_fg_bg_to_indicesd.py` & `monai-weekly-1.2.dev2320/tests/test_fg_bg_to_indicesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_file_basename.py` & `monai-weekly-1.2.dev2320/tests/test_file_basename.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_fill_holes.py` & `monai-weekly-1.2.dev2320/tests/test_fill_holes.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_fill_holesd.py` & `monai-weekly-1.2.dev2320/tests/test_fill_holesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_fl_exchange_object.py` & `monai-weekly-1.2.dev2320/tests/test_fl_exchange_object.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_fl_monai_algo.py` & `monai-weekly-1.2.dev2320/tests/test_fl_monai_algo.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_fl_monai_algo_dist.py` & `monai-weekly-1.2.dev2320/tests/test_fl_monai_algo_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_fl_monai_algo_stats.py` & `monai-weekly-1.2.dev2320/tests/test_fl_monai_algo_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_flatten_sub_keysd.py` & `monai-weekly-1.2.dev2320/tests/test_flatten_sub_keysd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_flexible_unet.py` & `monai-weekly-1.2.dev2320/tests/test_flexible_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_flip.py` & `monai-weekly-1.2.dev2320/tests/test_flip.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_flipd.py` & `monai-weekly-1.2.dev2320/tests/test_flipd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_focal_loss.py` & `monai-weekly-1.2.dev2320/tests/test_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_folder_layout.py` & `monai-weekly-1.2.dev2320/tests/test_folder_layout.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_foreground_mask.py` & `monai-weekly-1.2.dev2320/tests/test_foreground_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_foreground_maskd.py` & `monai-weekly-1.2.dev2320/tests/test_foreground_maskd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_fourier.py` & `monai-weekly-1.2.dev2320/tests/test_fourier.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_fpn_block.py` & `monai-weekly-1.2.dev2320/tests/test_fpn_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_from_engine_hovernet.py` & `monai-weekly-1.2.dev2320/tests/test_from_engine_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_fullyconnectednet.py` & `monai-weekly-1.2.dev2320/tests/test_fullyconnectednet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_gaussian.py` & `monai-weekly-1.2.dev2320/tests/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_gaussian_filter.py` & `monai-weekly-1.2.dev2320/tests/test_gaussian_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_gaussian_sharpen.py` & `monai-weekly-1.2.dev2320/tests/test_gaussian_sharpen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_gaussian_sharpend.py` & `monai-weekly-1.2.dev2320/tests/test_gaussian_sharpend.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_gaussian_smooth.py` & `monai-weekly-1.2.dev2320/tests/test_gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_gaussian_smoothd.py` & `monai-weekly-1.2.dev2320/tests/test_gaussian_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_generalized_dice_focal_loss.py` & `monai-weekly-1.2.dev2320/tests/test_generalized_dice_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_generalized_dice_loss.py` & `monai-weekly-1.2.dev2320/tests/test_generalized_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_generalized_wasserstein_dice_loss.py` & `monai-weekly-1.2.dev2320/tests/test_generalized_wasserstein_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_generate_distance_map.py` & `monai-weekly-1.2.dev2320/tests/test_generate_distance_map.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_generate_distance_mapd.py` & `monai-weekly-1.2.dev2320/tests/test_generate_distance_mapd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_generate_instance_border.py` & `monai-weekly-1.2.dev2320/tests/test_generate_instance_border.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_generate_instance_borderd.py` & `monai-weekly-1.2.dev2320/tests/test_generate_instance_borderd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_generate_instance_centroid.py` & `monai-weekly-1.2.dev2320/tests/test_generate_instance_centroid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_generate_instance_centroidd.py` & `monai-weekly-1.2.dev2320/tests/test_generate_instance_centroidd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_generate_instance_contour.py` & `monai-weekly-1.2.dev2320/tests/test_generate_instance_contour.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_generate_instance_contourd.py` & `monai-weekly-1.2.dev2320/tests/test_generate_instance_contourd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_generate_instance_type.py` & `monai-weekly-1.2.dev2320/tests/test_generate_instance_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_generate_instance_typed.py` & `monai-weekly-1.2.dev2320/tests/test_generate_instance_typed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_generate_label_classes_crop_centers.py` & `monai-weekly-1.2.dev2320/tests/test_generate_label_classes_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_generate_param_groups.py` & `monai-weekly-1.2.dev2320/tests/test_generate_param_groups.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_generate_pos_neg_label_crop_centers.py` & `monai-weekly-1.2.dev2320/tests/test_generate_pos_neg_label_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_generate_spatial_bounding_box.py` & `monai-weekly-1.2.dev2320/tests/test_generate_spatial_bounding_box.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_generate_succinct_contour.py` & `monai-weekly-1.2.dev2320/tests/test_generate_succinct_contour.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_generate_succinct_contourd.py` & `monai-weekly-1.2.dev2320/tests/test_generate_succinct_contourd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_generate_watershed_markers.py` & `monai-weekly-1.2.dev2320/tests/test_generate_watershed_markers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_generate_watershed_markersd.py` & `monai-weekly-1.2.dev2320/tests/test_generate_watershed_markersd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_generate_watershed_mask.py` & `monai-weekly-1.2.dev2320/tests/test_generate_watershed_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_generate_watershed_maskd.py` & `monai-weekly-1.2.dev2320/tests/test_generate_watershed_maskd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_generator.py` & `monai-weekly-1.2.dev2320/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_get_equivalent_dtype.py` & `monai-weekly-1.2.dev2320/tests/test_get_equivalent_dtype.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_get_extreme_points.py` & `monai-weekly-1.2.dev2320/tests/test_get_extreme_points.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_get_layers.py` & `monai-weekly-1.2.dev2320/tests/test_get_layers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_get_package_version.py` & `monai-weekly-1.2.dev2320/tests/test_get_package_version.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_get_unique_labels.py` & `monai-weekly-1.2.dev2320/tests/test_get_unique_labels.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_gibbs_noise.py` & `monai-weekly-1.2.dev2320/tests/test_gibbs_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_gibbs_noised.py` & `monai-weekly-1.2.dev2320/tests/test_gibbs_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_giou_loss.py` & `monai-weekly-1.2.dev2320/tests/test_giou_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_global_mutual_information_loss.py` & `monai-weekly-1.2.dev2320/tests/test_global_mutual_information_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_globalnet.py` & `monai-weekly-1.2.dev2320/tests/test_globalnet.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 import torch
 from parameterized import parameterized
 
 from monai.networks import eval_mode
 from monai.networks.blocks import Warp
 from monai.networks.nets import GlobalNet
 from monai.networks.nets.regunet import AffineHead
-from tests.utils import test_script_save
+from tests.utils import assert_allclose, test_script_save
 
 TEST_CASES_AFFINE_TRANSFORM = [
     [
-        {"spatial_dims": 3, "image_size": (2, 2, 2), "decode_size": (2, 2, 2), "in_channels": 1},
+        {"spatial_dims": 3, "image_size": (2, 2, 2), "decode_size": (2, 2, 2), "in_channels": 1, "save_theta": True},
         torch.ones(2, 12),
         torch.tensor([[[1, 2], [2, 3]], [[2, 3], [3, 4]]]).unsqueeze(0).unsqueeze(0).expand(2, 3, 2, 2, 2),
     ],
     [
         {"spatial_dims": 3, "image_size": (2, 2, 2), "decode_size": (2, 2, 2), "in_channels": 1},
         torch.arange(1, 13).reshape(1, 12).to(torch.float),
         torch.tensor(
@@ -51,25 +51,29 @@
             "num_channel_initial": 16,
             "depth": 1,
             "out_kernel_initializer": "kaiming_uniform",
             "out_activation": None,
             "pooling": True,
             "concat_skip": True,
             "encode_kernel_sizes": 3,
+            "save_theta": theta,
         },
         (1, 1, 16, 16),
         (1, 2, 16, 16),
     ]
+    for theta in (False, True)
 ]
 
 
 class TestAffineHead(unittest.TestCase):
     @parameterized.expand(TEST_CASES_AFFINE_TRANSFORM)
     def test_shape(self, input_param, theta, expected_val):
         layer = AffineHead(**input_param)
+        if input_param.get("save_theta"):
+            assert_allclose(layer.theta, torch.Tensor())
         result = layer.affine_transform(theta)
         np.testing.assert_allclose(result.cpu().numpy(), expected_val.cpu().numpy(), rtol=1e-4, atol=1e-4)
 
 
 device = "cuda" if torch.cuda.is_available() else "cpu"
 
 
@@ -77,21 +81,23 @@
     @parameterized.expand(TEST_CASES_GLOBAL_NET)
     def test_shape(self, input_param, input_shape, expected_shape):
         net = GlobalNet(**input_param).to(device)
         warp_layer = Warp()
         with eval_mode(net):
             img = torch.randn(input_shape)
             result = net(img.to(device))
+            if input_param.get("save_theta"):
+                assert_allclose(net.output_block.theta, torch.Tensor([[1.0, 0.0, 0.0, 0.0, 1.0, 0.0]]))
             warped = warp_layer(img.to(device), result)
             self.assertEqual(result.shape, expected_shape)
             # testing initial pred identity
             np.testing.assert_allclose(warped.detach().cpu().numpy(), img.detach().cpu().numpy(), rtol=1e-4, atol=1e-4)
 
-    def test_script(self):
-        input_param, input_shape, _ = TEST_CASES_GLOBAL_NET[0]
+    @parameterized.expand(TEST_CASES_GLOBAL_NET)
+    def test_script(self, input_param, input_shape, _):
         net = GlobalNet(**input_param)
         test_data = torch.randn(input_shape)
         test_script_save(net, test_data)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2319/tests/test_gmm.py` & `monai-weekly-1.2.dev2320/tests/test_gmm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_grid_dataset.py` & `monai-weekly-1.2.dev2320/tests/test_grid_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_grid_distortion.py` & `monai-weekly-1.2.dev2320/tests/test_grid_distortion.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_grid_distortiond.py` & `monai-weekly-1.2.dev2320/tests/test_grid_distortiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_grid_patch.py` & `monai-weekly-1.2.dev2320/tests/test_grid_patch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_grid_patchd.py` & `monai-weekly-1.2.dev2320/tests/test_grid_patchd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_grid_pull.py` & `monai-weekly-1.2.dev2320/tests/test_grid_pull.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_grid_split.py` & `monai-weekly-1.2.dev2320/tests/test_grid_split.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_grid_splitd.py` & `monai-weekly-1.2.dev2320/tests/test_grid_splitd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_checkpoint_loader.py` & `monai-weekly-1.2.dev2320/tests/test_handler_checkpoint_loader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_checkpoint_saver.py` & `monai-weekly-1.2.dev2320/tests/test_handler_checkpoint_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_classification_saver.py` & `monai-weekly-1.2.dev2320/tests/test_handler_classification_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_classification_saver_dist.py` & `monai-weekly-1.2.dev2320/tests/test_handler_classification_saver_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_clearml_image.py` & `monai-weekly-1.2.dev2320/tests/test_handler_clearml_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_clearml_stats.py` & `monai-weekly-1.2.dev2320/tests/test_handler_clearml_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_confusion_matrix.py` & `monai-weekly-1.2.dev2320/tests/test_handler_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_confusion_matrix_dist.py` & `monai-weekly-1.2.dev2320/tests/test_handler_confusion_matrix_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_decollate_batch.py` & `monai-weekly-1.2.dev2320/tests/test_handler_decollate_batch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_early_stop.py` & `monai-weekly-1.2.dev2320/tests/test_handler_early_stop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_garbage_collector.py` & `monai-weekly-1.2.dev2320/tests/test_handler_garbage_collector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_hausdorff_distance.py` & `monai-weekly-1.2.dev2320/tests/test_handler_hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_logfile.py` & `monai-weekly-1.2.dev2320/tests/test_handler_logfile.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_lr_scheduler.py` & `monai-weekly-1.2.dev2320/tests/test_handler_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_mean_dice.py` & `monai-weekly-1.2.dev2320/tests/test_handler_mean_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_mean_iou.py` & `monai-weekly-1.2.dev2320/tests/test_handler_mean_iou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_metric_logger.py` & `monai-weekly-1.2.dev2320/tests/test_handler_metric_logger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_metrics_reloaded.py` & `monai-weekly-1.2.dev2320/tests/test_handler_metrics_reloaded.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_metrics_saver.py` & `monai-weekly-1.2.dev2320/tests/test_handler_metrics_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_metrics_saver_dist.py` & `monai-weekly-1.2.dev2320/tests/test_handler_metrics_saver_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_mlflow.py` & `monai-weekly-1.2.dev2320/tests/test_handler_mlflow.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_nvtx.py` & `monai-weekly-1.2.dev2320/tests/test_handler_nvtx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_panoptic_quality.py` & `monai-weekly-1.2.dev2320/tests/test_handler_panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_parameter_scheduler.py` & `monai-weekly-1.2.dev2320/tests/test_handler_parameter_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_post_processing.py` & `monai-weekly-1.2.dev2320/tests/test_handler_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_prob_map_producer.py` & `monai-weekly-1.2.dev2320/tests/test_handler_prob_map_producer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_regression_metrics.py` & `monai-weekly-1.2.dev2320/tests/test_handler_regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_regression_metrics_dist.py` & `monai-weekly-1.2.dev2320/tests/test_handler_regression_metrics_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_rocauc.py` & `monai-weekly-1.2.dev2320/tests/test_handler_rocauc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_rocauc_dist.py` & `monai-weekly-1.2.dev2320/tests/test_handler_rocauc_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_smartcache.py` & `monai-weekly-1.2.dev2320/tests/test_handler_smartcache.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_stats.py` & `monai-weekly-1.2.dev2320/tests/test_handler_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_surface_distance.py` & `monai-weekly-1.2.dev2320/tests/test_handler_surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_tb_image.py` & `monai-weekly-1.2.dev2320/tests/test_handler_tb_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_tb_stats.py` & `monai-weekly-1.2.dev2320/tests/test_handler_tb_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_handler_validation.py` & `monai-weekly-1.2.dev2320/tests/test_handler_validation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_hardnegsampler.py` & `monai-weekly-1.2.dev2320/tests/test_hardnegsampler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_hashing.py` & `monai-weekly-1.2.dev2320/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_hausdorff_distance.py` & `monai-weekly-1.2.dev2320/tests/test_hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_header_correct.py` & `monai-weekly-1.2.dev2320/tests/test_header_correct.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_highresnet.py` & `monai-weekly-1.2.dev2320/tests/test_highresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_hilbert_transform.py` & `monai-weekly-1.2.dev2320/tests/test_hilbert_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_histogram_normalize.py` & `monai-weekly-1.2.dev2320/tests/test_histogram_normalize.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_histogram_normalized.py` & `monai-weekly-1.2.dev2320/tests/test_histogram_normalized.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_hovernet.py` & `monai-weekly-1.2.dev2320/tests/test_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_hovernet_instance_map_post_processing.py` & `monai-weekly-1.2.dev2320/tests/test_hovernet_instance_map_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_hovernet_instance_map_post_processingd.py` & `monai-weekly-1.2.dev2320/tests/test_hovernet_instance_map_post_processingd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_hovernet_loss.py` & `monai-weekly-1.2.dev2320/tests/test_hovernet_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_hovernet_nuclear_type_post_processing.py` & `monai-weekly-1.2.dev2320/tests/test_hovernet_nuclear_type_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_hovernet_nuclear_type_post_processingd.py` & `monai-weekly-1.2.dev2320/tests/test_hovernet_nuclear_type_post_processingd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_identity.py` & `monai-weekly-1.2.dev2320/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_identityd.py` & `monai-weekly-1.2.dev2320/tests/test_identityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_image_dataset.py` & `monai-weekly-1.2.dev2320/tests/test_image_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_image_filter.py` & `monai-weekly-1.2.dev2320/tests/test_image_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_image_rw.py` & `monai-weekly-1.2.dev2320/tests/test_image_rw.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_img2tensorboard.py` & `monai-weekly-1.2.dev2320/tests/test_img2tensorboard.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_init_reader.py` & `monai-weekly-1.2.dev2320/tests/test_init_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_integration_autorunner.py` & `monai-weekly-1.2.dev2320/tests/test_integration_autorunner.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_integration_bundle_run.py` & `monai-weekly-1.2.dev2320/tests/test_integration_bundle_run.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_integration_classification_2d.py` & `monai-weekly-1.2.dev2320/tests/test_integration_classification_2d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_integration_determinism.py` & `monai-weekly-1.2.dev2320/tests/test_integration_determinism.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_integration_fast_train.py` & `monai-weekly-1.2.dev2320/tests/test_integration_fast_train.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_integration_gpu_customization.py` & `monai-weekly-1.2.dev2320/tests/test_integration_gpu_customization.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_integration_lazy_samples.py` & `monai-weekly-1.2.dev2320/tests/test_integration_lazy_samples.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_integration_nnunetv2_runner.py` & `monai-weekly-1.2.dev2320/tests/test_integration_nnunetv2_runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,19 +77,19 @@
 
         ConfigParser.export_config_file(data_src, data_src_cfg)
         self.data_src_cfg = data_src_cfg
         self.test_path = test_path
 
     @skip_if_no_cuda
     def test_nnunetv2runner(self) -> None:
-        runner = nnUNetV2Runner(input_config=self.data_src_cfg)
+        runner = nnUNetV2Runner(input_config=self.data_src_cfg, trainer_class_name="nnUNetTrainer_1epoch")
         with skip_if_downloading_fails():
             runner.run(run_train=False, run_find_best_configuration=False, run_predict_ensemble_postprocessing=False)
-            runner.train(configs="3d_fullres", trainer_class_name="nnUNetTrainer_1epoch")
-            runner.find_best_configuration(configs="3d_fullres", trainers="nnUNetTrainer_1epoch")
+            runner.train(configs="3d_fullres")
+            runner.find_best_configuration(configs="3d_fullres")
             runner.predict_ensemble_postprocessing()
 
     def tearDown(self) -> None:
         self.test_dir.cleanup()
 
 
 if __name__ == "__main__":
```

### Comparing `monai-weekly-1.2.dev2319/tests/test_integration_segmentation_3d.py` & `monai-weekly-1.2.dev2320/tests/test_integration_segmentation_3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_integration_sliding_window.py` & `monai-weekly-1.2.dev2320/tests/test_integration_sliding_window.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_integration_stn.py` & `monai-weekly-1.2.dev2320/tests/test_integration_stn.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_integration_unet_2d.py` & `monai-weekly-1.2.dev2320/tests/test_integration_unet_2d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_integration_workers.py` & `monai-weekly-1.2.dev2320/tests/test_integration_workers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_integration_workflows.py` & `monai-weekly-1.2.dev2320/tests/test_integration_workflows.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_integration_workflows_gan.py` & `monai-weekly-1.2.dev2320/tests/test_integration_workflows_gan.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_intensity_stats.py` & `monai-weekly-1.2.dev2320/tests/test_intensity_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_intensity_statsd.py` & `monai-weekly-1.2.dev2320/tests/test_intensity_statsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_inverse.py` & `monai-weekly-1.2.dev2320/tests/test_inverse.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_inverse_array.py` & `monai-weekly-1.2.dev2320/tests/test_inverse_array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_inverse_collation.py` & `monai-weekly-1.2.dev2320/tests/test_inverse_collation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_invert.py` & `monai-weekly-1.2.dev2320/tests/test_invert.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_invertd.py` & `monai-weekly-1.2.dev2320/tests/test_invertd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_is_supported_format.py` & `monai-weekly-1.2.dev2320/tests/test_is_supported_format.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_iterable_dataset.py` & `monai-weekly-1.2.dev2320/tests/test_iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_itk_torch_bridge.py` & `monai-weekly-1.2.dev2320/tests/test_itk_torch_bridge.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_itk_writer.py` & `monai-weekly-1.2.dev2320/tests/test_itk_writer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_k_space_spike_noise.py` & `monai-weekly-1.2.dev2320/tests/test_k_space_spike_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_k_space_spike_noised.py` & `monai-weekly-1.2.dev2320/tests/test_k_space_spike_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_keep_largest_connected_component.py` & `monai-weekly-1.2.dev2320/tests/test_keep_largest_connected_component.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_keep_largest_connected_componentd.py` & `monai-weekly-1.2.dev2320/tests/test_keep_largest_connected_componentd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_kspace_mask.py` & `monai-weekly-1.2.dev2320/tests/test_kspace_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_label_filter.py` & `monai-weekly-1.2.dev2320/tests/test_label_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_label_filterd.py` & `monai-weekly-1.2.dev2320/tests/test_label_filterd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_label_quality_score.py` & `monai-weekly-1.2.dev2320/tests/test_label_quality_score.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_label_to_contour.py` & `monai-weekly-1.2.dev2320/tests/test_label_to_contour.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_label_to_contourd.py` & `monai-weekly-1.2.dev2320/tests/test_label_to_contourd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_label_to_mask.py` & `monai-weekly-1.2.dev2320/tests/test_label_to_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_label_to_maskd.py` & `monai-weekly-1.2.dev2320/tests/test_label_to_maskd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_lambda.py` & `monai-weekly-1.2.dev2320/tests/test_lambda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_lambdad.py` & `monai-weekly-1.2.dev2320/tests/test_lambdad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_lesion_froc.py` & `monai-weekly-1.2.dev2320/tests/test_lesion_froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_list_data_collate.py` & `monai-weekly-1.2.dev2320/tests/test_list_data_collate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_list_to_dict.py` & `monai-weekly-1.2.dev2320/tests/test_list_to_dict.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_lltm.py` & `monai-weekly-1.2.dev2320/tests/test_lltm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_lmdbdataset.py` & `monai-weekly-1.2.dev2320/tests/test_lmdbdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_lmdbdataset_dist.py` & `monai-weekly-1.2.dev2320/tests/test_lmdbdataset_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_load_decathlon_datalist.py` & `monai-weekly-1.2.dev2320/tests/test_load_decathlon_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_load_image.py` & `monai-weekly-1.2.dev2320/tests/test_load_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_load_imaged.py` & `monai-weekly-1.2.dev2320/tests/test_load_imaged.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_load_spacing_orientation.py` & `monai-weekly-1.2.dev2320/tests/test_load_spacing_orientation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_loader_semaphore.py` & `monai-weekly-1.2.dev2320/tests/test_loader_semaphore.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_local_normalized_cross_correlation_loss.py` & `monai-weekly-1.2.dev2320/tests/test_local_normalized_cross_correlation_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_localnet.py` & `monai-weekly-1.2.dev2320/tests/test_localnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_localnet_block.py` & `monai-weekly-1.2.dev2320/tests/test_localnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_look_up_option.py` & `monai-weekly-1.2.dev2320/tests/test_look_up_option.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_loss_metric.py` & `monai-weekly-1.2.dev2320/tests/test_loss_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_lr_finder.py` & `monai-weekly-1.2.dev2320/tests/test_lr_finder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_lr_scheduler.py` & `monai-weekly-1.2.dev2320/tests/test_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_make_nifti.py` & `monai-weekly-1.2.dev2320/tests/test_make_nifti.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_map_binary_to_indices.py` & `monai-weekly-1.2.dev2320/tests/test_map_binary_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_map_classes_to_indices.py` & `monai-weekly-1.2.dev2320/tests/test_map_classes_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_map_label_value.py` & `monai-weekly-1.2.dev2320/tests/test_map_label_value.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_map_label_valued.py` & `monai-weekly-1.2.dev2320/tests/test_map_label_valued.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_map_transform.py` & `monai-weekly-1.2.dev2320/tests/test_map_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_mask_intensity.py` & `monai-weekly-1.2.dev2320/tests/test_mask_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_mask_intensityd.py` & `monai-weekly-1.2.dev2320/tests/test_mask_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_masked_dice_loss.py` & `monai-weekly-1.2.dev2320/tests/test_masked_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_masked_loss.py` & `monai-weekly-1.2.dev2320/tests/test_masked_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_masked_patch_wsi_dataset.py` & `monai-weekly-1.2.dev2320/tests/test_masked_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_matshow3d.py` & `monai-weekly-1.2.dev2320/tests/test_matshow3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_mean_ensemble.py` & `monai-weekly-1.2.dev2320/tests/test_mean_ensemble.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_mean_ensembled.py` & `monai-weekly-1.2.dev2320/tests/test_mean_ensembled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_median_filter.py` & `monai-weekly-1.2.dev2320/tests/test_median_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_median_smooth.py` & `monai-weekly-1.2.dev2320/tests/test_median_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_median_smoothd.py` & `monai-weekly-1.2.dev2320/tests/test_median_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_mednistdataset.py` & `monai-weekly-1.2.dev2320/tests/test_mednistdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_meta_affine.py` & `monai-weekly-1.2.dev2320/tests/test_meta_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_meta_tensor.py` & `monai-weekly-1.2.dev2320/tests/test_meta_tensor.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_metatensor_integration.py` & `monai-weekly-1.2.dev2320/tests/test_metatensor_integration.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_metrics_reloaded.py` & `monai-weekly-1.2.dev2320/tests/test_metrics_reloaded.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_milmodel.py` & `monai-weekly-1.2.dev2320/tests/test_milmodel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_mlp.py` & `monai-weekly-1.2.dev2320/tests/test_mlp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_mmar_download.py` & `monai-weekly-1.2.dev2320/tests/test_mmar_download.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_module_list.py` & `monai-weekly-1.2.dev2320/tests/test_module_list.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_monai_env_vars.py` & `monai-weekly-1.2.dev2320/tests/test_monai_env_vars.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_monai_utils_misc.py` & `monai-weekly-1.2.dev2320/tests/test_monai_utils_misc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_mri_utils.py` & `monai-weekly-1.2.dev2320/tests/test_mri_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_multi_scale.py` & `monai-weekly-1.2.dev2320/tests/test_multi_scale.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_net_adapter.py` & `monai-weekly-1.2.dev2320/tests/test_net_adapter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_network_consistency.py` & `monai-weekly-1.2.dev2320/tests/test_network_consistency.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_nifti_endianness.py` & `monai-weekly-1.2.dev2320/tests/test_nifti_endianness.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_nifti_header_revise.py` & `monai-weekly-1.2.dev2320/tests/test_nifti_header_revise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_nifti_rw.py` & `monai-weekly-1.2.dev2320/tests/test_nifti_rw.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_normalize_intensity.py` & `monai-weekly-1.2.dev2320/tests/test_normalize_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_normalize_intensityd.py` & `monai-weekly-1.2.dev2320/tests/test_normalize_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_npzdictitemdataset.py` & `monai-weekly-1.2.dev2320/tests/test_npzdictitemdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_nrrd_reader.py` & `monai-weekly-1.2.dev2320/tests/test_nrrd_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_nuclick_transforms.py` & `monai-weekly-1.2.dev2320/tests/test_nuclick_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_numpy_reader.py` & `monai-weekly-1.2.dev2320/tests/test_numpy_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_nvtx_decorator.py` & `monai-weekly-1.2.dev2320/tests/test_nvtx_decorator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_nvtx_transform.py` & `monai-weekly-1.2.dev2320/tests/test_nvtx_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_occlusion_sensitivity.py` & `monai-weekly-1.2.dev2320/tests/test_occlusion_sensitivity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_one_of.py` & `monai-weekly-1.2.dev2320/tests/test_one_of.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_optim_novograd.py` & `monai-weekly-1.2.dev2320/tests/test_optim_novograd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_optional_import.py` & `monai-weekly-1.2.dev2320/tests/test_optional_import.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_ori_ras_lps.py` & `monai-weekly-1.2.dev2320/tests/test_ori_ras_lps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_orientation.py` & `monai-weekly-1.2.dev2320/tests/test_orientation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_orientationd.py` & `monai-weekly-1.2.dev2320/tests/test_orientationd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_p3d_block.py` & `monai-weekly-1.2.dev2320/tests/test_p3d_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_pad_collation.py` & `monai-weekly-1.2.dev2320/tests/test_pad_collation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_pad_mode.py` & `monai-weekly-1.2.dev2320/tests/test_pad_mode.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_parallel_execution.py` & `monai-weekly-1.2.dev2320/tests/test_parallel_execution.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_parallel_execution_dist.py` & `monai-weekly-1.2.dev2320/tests/test_parallel_execution_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_partition_dataset.py` & `monai-weekly-1.2.dev2320/tests/test_partition_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_partition_dataset_classes.py` & `monai-weekly-1.2.dev2320/tests/test_partition_dataset_classes.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_patch_dataset.py` & `monai-weekly-1.2.dev2320/tests/test_patch_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_patch_inferer.py` & `monai-weekly-1.2.dev2320/tests/test_patch_inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_patch_wsi_dataset.py` & `monai-weekly-1.2.dev2320/tests/test_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_patchembedding.py` & `monai-weekly-1.2.dev2320/tests/test_patchembedding.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_pathology_he_stain.py` & `monai-weekly-1.2.dev2320/tests/test_pathology_he_stain.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_pathology_he_stain_dict.py` & `monai-weekly-1.2.dev2320/tests/test_pathology_he_stain_dict.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_pathology_prob_nms.py` & `monai-weekly-1.2.dev2320/tests/test_pathology_prob_nms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_persistentdataset.py` & `monai-weekly-1.2.dev2320/tests/test_persistentdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_persistentdataset_dist.py` & `monai-weekly-1.2.dev2320/tests/test_persistentdataset_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_phl_cpu.py` & `monai-weekly-1.2.dev2320/tests/test_phl_cpu.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_phl_cuda.py` & `monai-weekly-1.2.dev2320/tests/test_phl_cuda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_pil_reader.py` & `monai-weekly-1.2.dev2320/tests/test_pil_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_plot_2d_or_3d_image.py` & `monai-weekly-1.2.dev2320/tests/test_plot_2d_or_3d_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_png_rw.py` & `monai-weekly-1.2.dev2320/tests/test_png_rw.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_polyval.py` & `monai-weekly-1.2.dev2320/tests/test_polyval.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_prepare_batch_default.py` & `monai-weekly-1.2.dev2320/tests/test_prepare_batch_default.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_prepare_batch_default_dist.py` & `monai-weekly-1.2.dev2320/tests/test_prepare_batch_default_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_prepare_batch_extra_input.py` & `monai-weekly-1.2.dev2320/tests/test_prepare_batch_extra_input.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_prepare_batch_hovernet.py` & `monai-weekly-1.2.dev2320/tests/test_prepare_batch_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_preset_filters.py` & `monai-weekly-1.2.dev2320/tests/test_preset_filters.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_print_info.py` & `monai-weekly-1.2.dev2320/tests/test_print_info.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_print_transform_backends.py` & `monai-weekly-1.2.dev2320/tests/test_print_transform_backends.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_probnms.py` & `monai-weekly-1.2.dev2320/tests/test_probnms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_probnmsd.py` & `monai-weekly-1.2.dev2320/tests/test_probnmsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_profiling.py` & `monai-weekly-1.2.dev2320/tests/test_profiling.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_pytorch_version_after.py` & `monai-weekly-1.2.dev2320/tests/test_pytorch_version_after.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_query_memory.py` & `monai-weekly-1.2.dev2320/tests/test_query_memory.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_adjust_contrast.py` & `monai-weekly-1.2.dev2320/tests/test_rand_adjust_contrast.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_adjust_contrastd.py` & `monai-weekly-1.2.dev2320/tests/test_rand_adjust_contrastd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_affine.py` & `monai-weekly-1.2.dev2320/tests/test_rand_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_affine_grid.py` & `monai-weekly-1.2.dev2320/tests/test_rand_affine_grid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_affined.py` & `monai-weekly-1.2.dev2320/tests/test_rand_affined.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_axis_flip.py` & `monai-weekly-1.2.dev2320/tests/test_rand_axis_flip.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_axis_flipd.py` & `monai-weekly-1.2.dev2320/tests/test_rand_axis_flipd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_bias_field.py` & `monai-weekly-1.2.dev2320/tests/test_rand_bias_field.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_bias_fieldd.py` & `monai-weekly-1.2.dev2320/tests/test_rand_bias_fieldd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_coarse_dropout.py` & `monai-weekly-1.2.dev2320/tests/test_rand_coarse_dropout.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_coarse_dropoutd.py` & `monai-weekly-1.2.dev2320/tests/test_rand_coarse_dropoutd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_coarse_shuffle.py` & `monai-weekly-1.2.dev2320/tests/test_rand_coarse_shuffle.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_coarse_shuffled.py` & `monai-weekly-1.2.dev2320/tests/test_rand_coarse_shuffled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_crop_by_label_classes.py` & `monai-weekly-1.2.dev2320/tests/test_rand_crop_by_label_classes.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_crop_by_label_classesd.py` & `monai-weekly-1.2.dev2320/tests/test_rand_crop_by_label_classesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_crop_by_pos_neg_label.py` & `monai-weekly-1.2.dev2320/tests/test_rand_crop_by_pos_neg_label.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_crop_by_pos_neg_labeld.py` & `monai-weekly-1.2.dev2320/tests/test_rand_crop_by_pos_neg_labeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_cucim_dict_transform.py` & `monai-weekly-1.2.dev2320/tests/test_rand_cucim_dict_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_cucim_transform.py` & `monai-weekly-1.2.dev2320/tests/test_rand_cucim_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_deform_grid.py` & `monai-weekly-1.2.dev2320/tests/test_rand_deform_grid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_elastic_2d.py` & `monai-weekly-1.2.dev2320/tests/test_rand_elastic_2d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_elastic_3d.py` & `monai-weekly-1.2.dev2320/tests/test_rand_elastic_3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_elasticd_2d.py` & `monai-weekly-1.2.dev2320/tests/test_rand_elasticd_2d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_elasticd_3d.py` & `monai-weekly-1.2.dev2320/tests/test_rand_elasticd_3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_flip.py` & `monai-weekly-1.2.dev2320/tests/test_rand_flip.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_flipd.py` & `monai-weekly-1.2.dev2320/tests/test_rand_flipd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_gaussian_noise.py` & `monai-weekly-1.2.dev2320/tests/test_rand_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_gaussian_noised.py` & `monai-weekly-1.2.dev2320/tests/test_rand_gaussian_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_gaussian_sharpen.py` & `monai-weekly-1.2.dev2320/tests/test_rand_gaussian_sharpen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_gaussian_sharpend.py` & `monai-weekly-1.2.dev2320/tests/test_rand_gaussian_sharpend.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_gaussian_smooth.py` & `monai-weekly-1.2.dev2320/tests/test_rand_gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_gaussian_smoothd.py` & `monai-weekly-1.2.dev2320/tests/test_rand_gaussian_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_gibbs_noise.py` & `monai-weekly-1.2.dev2320/tests/test_rand_gibbs_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_gibbs_noised.py` & `monai-weekly-1.2.dev2320/tests/test_rand_gibbs_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_grid_distortion.py` & `monai-weekly-1.2.dev2320/tests/test_rand_grid_distortion.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_grid_distortiond.py` & `monai-weekly-1.2.dev2320/tests/test_rand_grid_distortiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_grid_patch.py` & `monai-weekly-1.2.dev2320/tests/test_rand_grid_patch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_grid_patchd.py` & `monai-weekly-1.2.dev2320/tests/test_rand_grid_patchd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_histogram_shift.py` & `monai-weekly-1.2.dev2320/tests/test_rand_histogram_shift.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_histogram_shiftd.py` & `monai-weekly-1.2.dev2320/tests/test_rand_histogram_shiftd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_k_space_spike_noise.py` & `monai-weekly-1.2.dev2320/tests/test_rand_k_space_spike_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_k_space_spike_noised.py` & `monai-weekly-1.2.dev2320/tests/test_rand_k_space_spike_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_lambda.py` & `monai-weekly-1.2.dev2320/tests/test_rand_lambda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_lambdad.py` & `monai-weekly-1.2.dev2320/tests/test_rand_lambdad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_rician_noise.py` & `monai-weekly-1.2.dev2320/tests/test_rand_rician_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_rician_noised.py` & `monai-weekly-1.2.dev2320/tests/test_rand_rician_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_rotate.py` & `monai-weekly-1.2.dev2320/tests/test_rand_rotate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_rotate90.py` & `monai-weekly-1.2.dev2320/tests/test_rand_rotate90.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_rotate90d.py` & `monai-weekly-1.2.dev2320/tests/test_rand_rotate90d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_rotated.py` & `monai-weekly-1.2.dev2320/tests/test_rand_rotated.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_scale_crop.py` & `monai-weekly-1.2.dev2320/tests/test_rand_scale_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_scale_cropd.py` & `monai-weekly-1.2.dev2320/tests/test_rand_scale_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_scale_intensity.py` & `monai-weekly-1.2.dev2320/tests/test_rand_scale_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_scale_intensityd.py` & `monai-weekly-1.2.dev2320/tests/test_rand_scale_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_shift_intensity.py` & `monai-weekly-1.2.dev2320/tests/test_rand_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_shift_intensityd.py` & `monai-weekly-1.2.dev2320/tests/test_rand_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_spatial_crop.py` & `monai-weekly-1.2.dev2320/tests/test_rand_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_spatial_crop_samples.py` & `monai-weekly-1.2.dev2320/tests/test_rand_spatial_crop_samples.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_spatial_crop_samplesd.py` & `monai-weekly-1.2.dev2320/tests/test_rand_spatial_crop_samplesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_spatial_cropd.py` & `monai-weekly-1.2.dev2320/tests/test_rand_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_std_shift_intensity.py` & `monai-weekly-1.2.dev2320/tests/test_rand_std_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_std_shift_intensityd.py` & `monai-weekly-1.2.dev2320/tests/test_rand_std_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_weighted_crop.py` & `monai-weekly-1.2.dev2320/tests/test_rand_weighted_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_weighted_cropd.py` & `monai-weekly-1.2.dev2320/tests/test_rand_weighted_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_zoom.py` & `monai-weekly-1.2.dev2320/tests/test_rand_zoom.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rand_zoomd.py` & `monai-weekly-1.2.dev2320/tests/test_rand_zoomd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_randidentity.py` & `monai-weekly-1.2.dev2320/tests/test_randidentity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_random_order.py` & `monai-weekly-1.2.dev2320/tests/test_random_order.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_randomizable.py` & `monai-weekly-1.2.dev2320/tests/test_randomizable.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_randomizable_transform_type.py` & `monai-weekly-1.2.dev2320/tests/test_randomizable_transform_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_randtorchvisiond.py` & `monai-weekly-1.2.dev2320/tests/test_randtorchvisiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rankfilter_dist.py` & `monai-weekly-1.2.dev2320/tests/test_rankfilter_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_recon_net_utils.py` & `monai-weekly-1.2.dev2320/tests/test_recon_net_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_reference_based_normalize_intensity.py` & `monai-weekly-1.2.dev2320/tests/test_reference_based_normalize_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_reference_based_spatial_cropd.py` & `monai-weekly-1.2.dev2320/tests/test_reference_based_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_reference_resolver.py` & `monai-weekly-1.2.dev2320/tests/test_reference_resolver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_reg_loss_integration.py` & `monai-weekly-1.2.dev2320/tests/test_reg_loss_integration.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_regunet.py` & `monai-weekly-1.2.dev2320/tests/test_regunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_regunet_block.py` & `monai-weekly-1.2.dev2320/tests/test_regunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_remove_repeated_channel.py` & `monai-weekly-1.2.dev2320/tests/test_remove_repeated_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_remove_repeated_channeld.py` & `monai-weekly-1.2.dev2320/tests/test_remove_repeated_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_remove_small_objects.py` & `monai-weekly-1.2.dev2320/tests/test_remove_small_objects.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_repeat_channel.py` & `monai-weekly-1.2.dev2320/tests/test_repeat_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_repeat_channeld.py` & `monai-weekly-1.2.dev2320/tests/test_repeat_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_replace_module.py` & `monai-weekly-1.2.dev2320/tests/test_replace_module.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_require_pkg.py` & `monai-weekly-1.2.dev2320/tests/test_require_pkg.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_resample.py` & `monai-weekly-1.2.dev2320/tests/test_resample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_resample_backends.py` & `monai-weekly-1.2.dev2320/tests/test_resample_backends.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_resample_datalist.py` & `monai-weekly-1.2.dev2320/tests/test_resample_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_resample_to_match.py` & `monai-weekly-1.2.dev2320/tests/test_resample_to_match.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_resample_to_matchd.py` & `monai-weekly-1.2.dev2320/tests/test_resample_to_matchd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_resampler.py` & `monai-weekly-1.2.dev2320/tests/test_resampler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_resize.py` & `monai-weekly-1.2.dev2320/tests/test_resize.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_resize_with_pad_or_crop.py` & `monai-weekly-1.2.dev2320/tests/test_resize_with_pad_or_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_resize_with_pad_or_cropd.py` & `monai-weekly-1.2.dev2320/tests/test_resize_with_pad_or_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_resized.py` & `monai-weekly-1.2.dev2320/tests/test_resized.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_resnet.py` & `monai-weekly-1.2.dev2320/tests/test_resnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_retinanet.py` & `monai-weekly-1.2.dev2320/tests/test_retinanet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_retinanet_detector.py` & `monai-weekly-1.2.dev2320/tests/test_retinanet_detector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_retinanet_predict_utils.py` & `monai-weekly-1.2.dev2320/tests/test_retinanet_predict_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rotate.py` & `monai-weekly-1.2.dev2320/tests/test_rotate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rotate90.py` & `monai-weekly-1.2.dev2320/tests/test_rotate90.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rotate90d.py` & `monai-weekly-1.2.dev2320/tests/test_rotate90d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_rotated.py` & `monai-weekly-1.2.dev2320/tests/test_rotated.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_safe_dtype_range.py` & `monai-weekly-1.2.dev2320/tests/test_safe_dtype_range.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_saliency_inferer.py` & `monai-weekly-1.2.dev2320/tests/test_saliency_inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_sample_slices.py` & `monai-weekly-1.2.dev2320/tests/test_sample_slices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_sampler_dist.py` & `monai-weekly-1.2.dev2320/tests/test_sampler_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_save_classificationd.py` & `monai-weekly-1.2.dev2320/tests/test_save_classificationd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_save_image.py` & `monai-weekly-1.2.dev2320/tests/test_save_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_save_imaged.py` & `monai-weekly-1.2.dev2320/tests/test_save_imaged.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_save_state.py` & `monai-weekly-1.2.dev2320/tests/test_save_state.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_savitzky_golay_filter.py` & `monai-weekly-1.2.dev2320/tests/test_savitzky_golay_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_savitzky_golay_smooth.py` & `monai-weekly-1.2.dev2320/tests/test_savitzky_golay_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_savitzky_golay_smoothd.py` & `monai-weekly-1.2.dev2320/tests/test_savitzky_golay_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_scale_intensity.py` & `monai-weekly-1.2.dev2320/tests/test_scale_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_scale_intensity_range.py` & `monai-weekly-1.2.dev2320/tests/test_scale_intensity_range.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_scale_intensity_range_percentiles.py` & `monai-weekly-1.2.dev2320/tests/test_scale_intensity_range_percentiles.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_scale_intensity_range_percentilesd.py` & `monai-weekly-1.2.dev2320/tests/test_scale_intensity_range_percentilesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_scale_intensity_ranged.py` & `monai-weekly-1.2.dev2320/tests/test_scale_intensity_ranged.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_scale_intensityd.py` & `monai-weekly-1.2.dev2320/tests/test_scale_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_se_block.py` & `monai-weekly-1.2.dev2320/tests/test_se_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_se_blocks.py` & `monai-weekly-1.2.dev2320/tests/test_se_blocks.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_seg_loss_integration.py` & `monai-weekly-1.2.dev2320/tests/test_seg_loss_integration.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_segresnet.py` & `monai-weekly-1.2.dev2320/tests/test_segresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_segresnet_block.py` & `monai-weekly-1.2.dev2320/tests/test_segresnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_segresnet_ds.py` & `monai-weekly-1.2.dev2320/tests/test_segresnet_ds.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_select_cross_validation_folds.py` & `monai-weekly-1.2.dev2320/tests/test_select_cross_validation_folds.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_select_itemsd.py` & `monai-weekly-1.2.dev2320/tests/test_select_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_selfattention.py` & `monai-weekly-1.2.dev2320/tests/test_selfattention.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_senet.py` & `monai-weekly-1.2.dev2320/tests/test_senet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_separable_filter.py` & `monai-weekly-1.2.dev2320/tests/test_separable_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_set_determinism.py` & `monai-weekly-1.2.dev2320/tests/test_set_determinism.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_set_visible_devices.py` & `monai-weekly-1.2.dev2320/tests/test_set_visible_devices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_shift_intensity.py` & `monai-weekly-1.2.dev2320/tests/test_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_shift_intensityd.py` & `monai-weekly-1.2.dev2320/tests/test_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_shuffle_buffer.py` & `monai-weekly-1.2.dev2320/tests/test_shuffle_buffer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_signal_continuouswavelet.py` & `monai-weekly-1.2.dev2320/tests/test_signal_continuouswavelet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_signal_fillempty.py` & `monai-weekly-1.2.dev2320/tests/test_signal_fillempty.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_signal_rand_add_gaussiannoise.py` & `monai-weekly-1.2.dev2320/tests/test_signal_rand_add_gaussiannoise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_signal_rand_add_sine.py` & `monai-weekly-1.2.dev2320/tests/test_signal_rand_add_sine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_signal_rand_add_sine_partial.py` & `monai-weekly-1.2.dev2320/tests/test_signal_rand_add_sine_partial.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_signal_rand_add_squarepulse.py` & `monai-weekly-1.2.dev2320/tests/test_signal_rand_add_squarepulse.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_signal_rand_add_squarepulse_partial.py` & `monai-weekly-1.2.dev2320/tests/test_signal_rand_add_squarepulse_partial.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_signal_rand_drop.py` & `monai-weekly-1.2.dev2320/tests/test_signal_rand_drop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_signal_rand_scale.py` & `monai-weekly-1.2.dev2320/tests/test_signal_rand_scale.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_signal_rand_shift.py` & `monai-weekly-1.2.dev2320/tests/test_signal_rand_shift.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_signal_remove_frequency.py` & `monai-weekly-1.2.dev2320/tests/test_signal_remove_frequency.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_simple_aspp.py` & `monai-weekly-1.2.dev2320/tests/test_simple_aspp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_simulatedelay.py` & `monai-weekly-1.2.dev2320/tests/test_simulatedelay.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_simulatedelayd.py` & `monai-weekly-1.2.dev2320/tests/test_simulatedelayd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_skip_connection.py` & `monai-weekly-1.2.dev2320/tests/test_skip_connection.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_slice_inferer.py` & `monai-weekly-1.2.dev2320/tests/test_slice_inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_sliding_patch_wsi_dataset.py` & `monai-weekly-1.2.dev2320/tests/test_sliding_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_sliding_window_hovernet_inference.py` & `monai-weekly-1.2.dev2320/tests/test_sliding_window_hovernet_inference.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_sliding_window_inference.py` & `monai-weekly-1.2.dev2320/tests/test_sliding_window_inference.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_sliding_window_splitter.py` & `monai-weekly-1.2.dev2320/tests/test_sliding_window_splitter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_smartcachedataset.py` & `monai-weekly-1.2.dev2320/tests/test_smartcachedataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_smooth_field.py` & `monai-weekly-1.2.dev2320/tests/test_smooth_field.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_sobel_gradient.py` & `monai-weekly-1.2.dev2320/tests/test_sobel_gradient.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_sobel_gradientd.py` & `monai-weekly-1.2.dev2320/tests/test_sobel_gradientd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_some_of.py` & `monai-weekly-1.2.dev2320/tests/test_some_of.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_spacing.py` & `monai-weekly-1.2.dev2320/tests/test_spacing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_spacingd.py` & `monai-weekly-1.2.dev2320/tests/test_spacingd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_spatial_combine_transforms.py` & `monai-weekly-1.2.dev2320/tests/test_spatial_combine_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_spatial_crop.py` & `monai-weekly-1.2.dev2320/tests/test_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_spatial_cropd.py` & `monai-weekly-1.2.dev2320/tests/test_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_spatial_pad.py` & `monai-weekly-1.2.dev2320/tests/test_spatial_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_spatial_padd.py` & `monai-weekly-1.2.dev2320/tests/test_spatial_padd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_spatial_resample.py` & `monai-weekly-1.2.dev2320/tests/test_spatial_resample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_spatial_resampled.py` & `monai-weekly-1.2.dev2320/tests/test_spatial_resampled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_split_channel.py` & `monai-weekly-1.2.dev2320/tests/test_split_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_split_channeld.py` & `monai-weekly-1.2.dev2320/tests/test_split_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_splitdim.py` & `monai-weekly-1.2.dev2320/tests/test_splitdim.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_splitdimd.py` & `monai-weekly-1.2.dev2320/tests/test_splitdimd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_squeezedim.py` & `monai-weekly-1.2.dev2320/tests/test_squeezedim.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_squeezedimd.py` & `monai-weekly-1.2.dev2320/tests/test_squeezedimd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_ssim_loss.py` & `monai-weekly-1.2.dev2320/tests/test_ssim_loss.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 import unittest
 
 import numpy as np
 import torch
 
 from monai.losses.ssim_loss import SSIMLoss
 from monai.utils import set_determinism
-from tests.utils import test_script_save
+
+# from tests.utils import test_script_save
 
 
 class TestSSIMLoss(unittest.TestCase):
     def test_shape(self):
         set_determinism(0)
         preds = torch.abs(torch.randn(2, 3, 16, 16))
         target = torch.abs(torch.randn(2, 3, 16, 16))
@@ -43,15 +44,15 @@
 
         result = SSIMLoss(spatial_dims=2, data_range=1.0, kernel_type="gaussian", reduction="none").forward(
             preds, target
         )
         expected_val = [[0.9121], [0.9971]]
         np.testing.assert_allclose(result.detach().cpu().numpy(), expected_val, rtol=1e-4)
 
-    def test_script(self):
-        loss = SSIMLoss(spatial_dims=2)
-        test_input = torch.ones(2, 2, 16, 16)
-        test_script_save(loss, test_input, test_input)
+    # def test_script(self):
+    #     loss = SSIMLoss(spatial_dims=2)
+    #     test_input = torch.ones(2, 2, 16, 16)
+    #     test_script_save(loss, test_input, test_input)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2319/tests/test_ssim_metric.py` & `monai-weekly-1.2.dev2320/tests/test_ssim_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_state_cacher.py` & `monai-weekly-1.2.dev2320/tests/test_state_cacher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_std_shift_intensity.py` & `monai-weekly-1.2.dev2320/tests/test_std_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_std_shift_intensityd.py` & `monai-weekly-1.2.dev2320/tests/test_std_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_str2bool.py` & `monai-weekly-1.2.dev2320/tests/test_str2bool.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_str2list.py` & `monai-weekly-1.2.dev2320/tests/test_str2list.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_subpixel_upsample.py` & `monai-weekly-1.2.dev2320/tests/test_subpixel_upsample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_surface_dice.py` & `monai-weekly-1.2.dev2320/tests/test_surface_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_surface_distance.py` & `monai-weekly-1.2.dev2320/tests/test_surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_swin_unetr.py` & `monai-weekly-1.2.dev2320/tests/test_swin_unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_synthetic.py` & `monai-weekly-1.2.dev2320/tests/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_tciadataset.py` & `monai-weekly-1.2.dev2320/tests/test_tciadataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_testtimeaugmentation.py` & `monai-weekly-1.2.dev2320/tests/test_testtimeaugmentation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_text_encoding.py` & `monai-weekly-1.2.dev2320/tests/test_text_encoding.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,22 +18,22 @@
 
 
 class TestTextEncoder(unittest.TestCase):
     def test_test_encoding_shape(self):
         with skip_if_downloading_fails():
             # test 2D encoder
             text_encoder = TextEncoder(
-                spatial_dims=2, out_channels=32, encoding="clip_encoding_univeral_model_32", pretrained=True
+                spatial_dims=2, out_channels=32, encoding="clip_encoding_universal_model_32", pretrained=True
             )
             text_encoding = text_encoder()
             self.assertEqual(text_encoding.shape, (32, 256, 1, 1))
 
             # test 3D encoder
             text_encoder = TextEncoder(
-                spatial_dims=3, out_channels=32, encoding="clip_encoding_univeral_model_32", pretrained=True
+                spatial_dims=3, out_channels=32, encoding="clip_encoding_universal_model_32", pretrained=True
             )
             text_encoding = text_encoder()
             self.assertEqual(text_encoding.shape, (32, 256, 1, 1, 1))
 
         # test random enbedding 3D
         text_encoder = TextEncoder(spatial_dims=3, out_channels=32, encoding="rand_embedding", pretrained=True)
         text_encoding = text_encoder()
```

### Comparing `monai-weekly-1.2.dev2319/tests/test_thread_buffer.py` & `monai-weekly-1.2.dev2320/tests/test_thread_buffer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_threadcontainer.py` & `monai-weekly-1.2.dev2320/tests/test_threadcontainer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_threshold_intensity.py` & `monai-weekly-1.2.dev2320/tests/test_threshold_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_threshold_intensityd.py` & `monai-weekly-1.2.dev2320/tests/test_threshold_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_timedcall_dist.py` & `monai-weekly-1.2.dev2320/tests/test_timedcall_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_to_contiguous.py` & `monai-weekly-1.2.dev2320/tests/test_to_contiguous.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_to_cupy.py` & `monai-weekly-1.2.dev2320/tests/test_to_cupy.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_to_cupyd.py` & `monai-weekly-1.2.dev2320/tests/test_to_cupyd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_to_device.py` & `monai-weekly-1.2.dev2320/tests/test_to_device.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_to_deviced.py` & `monai-weekly-1.2.dev2320/tests/test_to_deviced.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_to_from_meta_tensord.py` & `monai-weekly-1.2.dev2320/tests/test_to_from_meta_tensord.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_to_numpy.py` & `monai-weekly-1.2.dev2320/tests/test_to_numpy.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_to_numpyd.py` & `monai-weekly-1.2.dev2320/tests/test_to_numpyd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_to_onehot.py` & `monai-weekly-1.2.dev2320/tests/test_to_onehot.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_to_pil.py` & `monai-weekly-1.2.dev2320/tests/test_to_pil.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_to_pild.py` & `monai-weekly-1.2.dev2320/tests/test_to_pild.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_to_tensor.py` & `monai-weekly-1.2.dev2320/tests/test_to_tensor.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_to_tensord.py` & `monai-weekly-1.2.dev2320/tests/test_to_tensord.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_torchscript_utils.py` & `monai-weekly-1.2.dev2320/tests/test_torchscript_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_torchvision.py` & `monai-weekly-1.2.dev2320/tests/test_torchvision.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_torchvision_fc_model.py` & `monai-weekly-1.2.dev2320/tests/test_torchvision_fc_model.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_torchvisiond.py` & `monai-weekly-1.2.dev2320/tests/test_torchvisiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_traceable_transform.py` & `monai-weekly-1.2.dev2320/tests/test_traceable_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_train_mode.py` & `monai-weekly-1.2.dev2320/tests/test_train_mode.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_trainable_bilateral.py` & `monai-weekly-1.2.dev2320/tests/test_trainable_bilateral.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_trainable_joint_bilateral.py` & `monai-weekly-1.2.dev2320/tests/test_trainable_joint_bilateral.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_transchex.py` & `monai-weekly-1.2.dev2320/tests/test_transchex.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_transform.py` & `monai-weekly-1.2.dev2320/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_transformerblock.py` & `monai-weekly-1.2.dev2320/tests/test_transformerblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_transpose.py` & `monai-weekly-1.2.dev2320/tests/test_transpose.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_transposed.py` & `monai-weekly-1.2.dev2320/tests/test_transposed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_tversky_loss.py` & `monai-weekly-1.2.dev2320/tests/test_tversky_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_unet.py` & `monai-weekly-1.2.dev2320/tests/test_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_unetr.py` & `monai-weekly-1.2.dev2320/tests/test_unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_unetr_block.py` & `monai-weekly-1.2.dev2320/tests/test_unetr_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_unified_focal_loss.py` & `monai-weekly-1.2.dev2320/tests/test_unified_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_upsample_block.py` & `monai-weekly-1.2.dev2320/tests/test_upsample_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_utils_pytorch_numpy_unification.py` & `monai-weekly-1.2.dev2320/tests/test_utils_pytorch_numpy_unification.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_varautoencoder.py` & `monai-weekly-1.2.dev2320/tests/test_varautoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_varnet.py` & `monai-weekly-1.2.dev2320/tests/test_varnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_version_leq.py` & `monai-weekly-1.2.dev2320/tests/test_version_leq.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_video_datasets.py` & `monai-weekly-1.2.dev2320/tests/test_video_datasets.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_vis_cam.py` & `monai-weekly-1.2.dev2320/tests/test_vis_cam.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_vis_gradbased.py` & `monai-weekly-1.2.dev2320/tests/test_vis_gradbased.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_vis_gradcam.py` & `monai-weekly-1.2.dev2320/tests/test_vis_gradcam.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_vit.py` & `monai-weekly-1.2.dev2320/tests/test_vit.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_vitautoenc.py` & `monai-weekly-1.2.dev2320/tests/test_vitautoenc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_vnet.py` & `monai-weekly-1.2.dev2320/tests/test_vnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_vote_ensemble.py` & `monai-weekly-1.2.dev2320/tests/test_vote_ensemble.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_vote_ensembled.py` & `monai-weekly-1.2.dev2320/tests/test_vote_ensembled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_warp.py` & `monai-weekly-1.2.dev2320/tests/test_warp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_watershed.py` & `monai-weekly-1.2.dev2320/tests/test_watershed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_watershedd.py` & `monai-weekly-1.2.dev2320/tests/test_watershedd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_weight_init.py` & `monai-weekly-1.2.dev2320/tests/test_weight_init.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_weighted_random_sampler_dist.py` & `monai-weekly-1.2.dev2320/tests/test_weighted_random_sampler_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_with_allow_missing_keys.py` & `monai-weekly-1.2.dev2320/tests/test_with_allow_missing_keys.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_write_metrics_reports.py` & `monai-weekly-1.2.dev2320/tests/test_write_metrics_reports.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_wsireader.py` & `monai-weekly-1.2.dev2320/tests/test_wsireader.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,23 +77,35 @@
     {"location": (0, 0), "size": (2, 1), "level": 8},
     np.array([[[242], [242]], [[242], [242]], [[242], [242]]], dtype=np.uint8),
 ]
 
 TEST_CASE_3 = [
     WSI_GENERIC_TIFF_PATH,
     {"channel_dim": -1},
-    {"location": (WSI_GENERIC_TIFF_HEIGHT // 2, WSI_GENERIC_TIFF_WIDTH // 2), "size": (2, 1), "level": 0},
-    np.moveaxis(np.array([[[246], [246]], [[246], [246]], [[246], [246]]], dtype=np.uint8), 0, -1),
+    {"location": (WSI_GENERIC_TIFF_HEIGHT // 2, WSI_GENERIC_TIFF_WIDTH // 2), "size": (4, 1), "level": 0},
+    np.moveaxis(
+        np.array(
+            [[[246], [246], [246], [246]], [[246], [246], [246], [246]], [[246], [246], [246], [246]]], dtype=np.uint8
+        ),
+        0,
+        -1,
+    ),
 ]
 
 TEST_CASE_4 = [
     WSI_GENERIC_TIFF_PATH,
     {"channel_dim": 2},
-    {"location": (0, 0), "size": (2, 1), "level": 8},
-    np.moveaxis(np.array([[[242], [242]], [[242], [242]], [[242], [242]]], dtype=np.uint8), 0, -1),
+    {"location": (0, 0), "size": (4, 1), "level": 8},
+    np.moveaxis(
+        np.array(
+            [[[242], [242], [242], [242]], [[242], [242], [242], [242]], [[242], [242], [242], [242]]], dtype=np.uint8
+        ),
+        0,
+        -1,
+    ),
 ]
 
 TEST_CASE_5 = [
     WSI_GENERIC_TIFF_PATH,
     {"level": 8},
     {"location": (0, 0), "size": (2, 1)},
     np.array([[[242], [242]], [[242], [242]], [[242], [242]]], dtype=np.uint8),
```

### Comparing `monai-weekly-1.2.dev2319/tests/test_zipdataset.py` & `monai-weekly-1.2.dev2320/tests/test_zipdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_zoom.py` & `monai-weekly-1.2.dev2320/tests/test_zoom.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_zoom_affine.py` & `monai-weekly-1.2.dev2320/tests/test_zoom_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/tests/test_zoomd.py` & `monai-weekly-1.2.dev2320/tests/test_zoomd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2319/versioneer.py` & `monai-weekly-1.2.dev2320/versioneer.py`

 * *Files identical despite different names*

