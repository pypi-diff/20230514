# Comparing `tmp/ml-starter-0.0.38.tar.gz` & `tmp/ml-starter-0.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.38.tar", last modified: Sat May 13 07:01:19 2023, max compression
+gzip compressed data, was "ml-starter-0.0.39.tar", last modified: Sun May 14 09:26:20 2023, max compression
```

## Comparing `ml-starter-0.0.38.tar` & `ml-starter-0.0.39.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:19.927616 ml-starter-0.0.38/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-13 07:01:02.000000 ml-starter-0.0.38/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-13 07:01:02.000000 ml-starter-0.0.38/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-13 07:01:19.927616 ml-starter-0.0.38/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-13 07:01:02.000000 ml-starter-0.0.38/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:19.895616 ml-starter-0.0.38/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:19.895616 ml-starter-0.0.38/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    25200 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:19.899616 ml-starter-0.0.38/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:19.899616 ml-starter-0.0.38/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    44643 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:19.899616 ml-starter-0.0.38/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:19.899616 ml-starter-0.0.38/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:19.903616 ml-starter-0.0.38/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    23911 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16201 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:19.903616 ml-starter-0.0.38/ml/models/pretrained/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/models/pretrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41249 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/models/pretrained/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    31800 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/models/pretrained/hubert.py
--rw-r--r--   0 runner    (1001) docker     (123)    22211 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/models/pretrained/llama.py
--rw-r--r--   0 runner    (1001) docker     (123)    60772 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/models/pretrained/sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:19.907616 ml-starter-0.0.38/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:19.907616 ml-starter-0.0.38/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:19.907616 ml-starter-0.0.38/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18456 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:19.911616 ml-starter-0.0.38/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:19.911616 ml-starter-0.0.38/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:19.911616 ml-starter-0.0.38/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:19.911616 ml-starter-0.0.38/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:19.911616 ml-starter-0.0.38/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:19.915616 ml-starter-0.0.38/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20655 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/trainers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:19.915616 ml-starter-0.0.38/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/trainers/sl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/trainers/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:19.923616 ml-starter-0.0.38/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:19.923616 ml-starter-0.0.38/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/torch_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-05-13 07:01:02.000000 ml-starter-0.0.38/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:01:19.927616 ml-starter-0.0.38/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-13 07:01:19.000000 ml-starter-0.0.38/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-05-13 07:01:19.000000 ml-starter-0.0.38/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 07:01:19.000000 ml-starter-0.0.38/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-13 07:01:19.000000 ml-starter-0.0.38/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-13 07:01:19.000000 ml-starter-0.0.38/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-13 07:01:02.000000 ml-starter-0.0.38/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-13 07:01:02.000000 ml-starter-0.0.38/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-13 07:01:02.000000 ml-starter-0.0.38/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-13 07:01:02.000000 ml-starter-0.0.38/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-13 07:01:19.927616 ml-starter-0.0.38/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-13 07:01:02.000000 ml-starter-0.0.38/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.062536 ml-starter-0.0.39/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-14 09:26:08.000000 ml-starter-0.0.39/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-14 09:26:08.000000 ml-starter-0.0.39/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-14 09:26:20.062536 ml-starter-0.0.39/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-14 09:26:08.000000 ml-starter-0.0.39/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.046535 ml-starter-0.0.39/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.046535 ml-starter-0.0.39/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25200 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.046535 ml-starter-0.0.39/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.046535 ml-starter-0.0.39/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44643 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.050535 ml-starter-0.0.39/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.050535 ml-starter-0.0.39/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.050535 ml-starter-0.0.39/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25205 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16201 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.050535 ml-starter-0.0.39/ml/models/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/models/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41249 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/models/pretrained/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31800 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/models/pretrained/hubert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22211 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/models/pretrained/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60772 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/models/pretrained/sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.050535 ml-starter-0.0.39/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.054535 ml-starter-0.0.39/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.054535 ml-starter-0.0.39/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18456 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.054535 ml-starter-0.0.39/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.054535 ml-starter-0.0.39/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.054535 ml-starter-0.0.39/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.054535 ml-starter-0.0.39/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.054535 ml-starter-0.0.39/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.054535 ml-starter-0.0.39/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20655 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.058535 ml-starter-0.0.39/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/sl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.062536 ml-starter-0.0.39/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.062536 ml-starter-0.0.39/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/torch_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.062536 ml-starter-0.0.39/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-14 09:26:20.000000 ml-starter-0.0.39/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-05-14 09:26:20.000000 ml-starter-0.0.39/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 09:26:20.000000 ml-starter-0.0.39/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-14 09:26:20.000000 ml-starter-0.0.39/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-14 09:26:20.000000 ml-starter-0.0.39/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-14 09:26:08.000000 ml-starter-0.0.39/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-14 09:26:08.000000 ml-starter-0.0.39/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-14 09:26:08.000000 ml-starter-0.0.39/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-14 09:26:08.000000 ml-starter-0.0.39/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-14 09:26:20.062536 ml-starter-0.0.39/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-14 09:26:08.000000 ml-starter-0.0.39/setup.py
```

### Comparing `ml-starter-0.0.38/LICENSE` & `ml-starter-0.0.39/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/PKG-INFO` & `ml-starter-0.0.39/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.38
+Version: 0.0.39
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.38/README.md` & `ml-starter-0.0.39/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/api.py` & `ml-starter-0.0.39/ml/api.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/core/common_types.py` & `ml-starter-0.0.39/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/core/config.py` & `ml-starter-0.0.39/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/core/env.py` & `ml-starter-0.0.39/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/core/registry.py` & `ml-starter-0.0.39/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/core/state.py` & `ml-starter-0.0.39/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/launchers/base.py` & `ml-starter-0.0.39/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/launchers/mp.py` & `ml-starter-0.0.39/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/launchers/slurm.py` & `ml-starter-0.0.39/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/launchers/torchrun.py` & `ml-starter-0.0.39/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/loggers/base.py` & `ml-starter-0.0.39/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/loggers/meter.py` & `ml-starter-0.0.39/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/loggers/multi.py` & `ml-starter-0.0.39/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/loggers/stdout.py` & `ml-starter-0.0.39/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/loggers/tensorboard.py` & `ml-starter-0.0.39/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/lr_schedulers/base.py` & `ml-starter-0.0.39/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/lr_schedulers/constant.py` & `ml-starter-0.0.39/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.39/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.39/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/lr_schedulers/linear.py` & `ml-starter-0.0.39/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.39/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.39/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/models/activations.py` & `ml-starter-0.0.39/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/models/base.py` & `ml-starter-0.0.39/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/models/embeddings.py` & `ml-starter-0.0.39/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/models/init.py` & `ml-starter-0.0.39/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/models/lora.py` & `ml-starter-0.0.39/ml/models/lora.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,22 +74,24 @@
         lora_alpha: float = 1.0,
         lora_dropout: float = 0.0,
         merge: bool = False,
         padding_idx: int | None = None,
         max_norm: float | None = None,
         norm_type: float = 2.0,
         scale_grad_by_freq: bool = False,
+        sparse: bool = False,
     ) -> None:
         super().__init__(
             num_embeddings,
             embedding_dim,
             padding_idx=padding_idx,
             max_norm=max_norm,
             norm_type=norm_type,
             scale_grad_by_freq=scale_grad_by_freq,
+            sparse=sparse,
         )
 
         assert r > 0
 
         self.r = r
         self.lora_alpha = lora_alpha
         self.scaling = self.lora_alpha / self.r
@@ -604,91 +606,117 @@
     Returns:
         The LoRA version of the module.
 
     Raises:
         ValueError: If the module is not supported.
     """
     if isinstance(module, nn.Embedding):
-        return LoraEmbedding(
+        embedding = LoraEmbedding(
             module.num_embeddings,
             module.embedding_dim,
+            padding_idx=module.padding_idx,
+            max_norm=module.max_norm,
+            norm_type=module.norm_type,
+            scale_grad_by_freq=module.scale_grad_by_freq,
+            sparse=module.sparse,
             r=r,
             lora_alpha=alpha,
             merge=merge,
         )
+        embedding.weight.data.copy_(module.weight.data)
+        return embedding
 
     if isinstance(module, nn.Linear):
-        return LoraLinear(
+        linear = LoraLinear(
             module.in_features,
             module.out_features,
             r=r,
             lora_alpha=alpha,
             merge=merge,
+            bias=module.bias is not None,
         )
+        linear.weight.data.copy_(module.weight.data)
+        if module.bias is not None and linear.bias is not None:
+            linear.bias.data.copy_(module.bias.data)
+        return linear
 
     if isinstance(module, nn.Conv1d):
-        return LoraConv1d(
+        conv_1d = LoraConv1d(
             module.in_channels,
             module.out_channels,
             cast(tuple[int], module.kernel_size),
             r=r,
             lora_alpha=alpha,
             lora_dropout=dropout,
             merge=merge,
             stride=cast(tuple[int], module.stride),
             padding=cast(tuple[int], module.padding),
             dilation=cast(tuple[int], module.dilation),
             groups=module.groups,
             bias=module.bias is not None,
         )
+        conv_1d.weight.data.copy_(module.weight.data)
+        if module.bias is not None and conv_1d.bias is not None:
+            conv_1d.bias.data.copy_(module.bias.data)
+        return conv_1d
 
     if isinstance(module, nn.Conv2d):
-        return LoraConv2d(
+        conv_2d = LoraConv2d(
             module.in_channels,
             module.out_channels,
             cast(tuple[int, int], module.kernel_size),
             r=r,
             lora_alpha=alpha,
             lora_dropout=dropout,
             merge=merge,
             stride=cast(tuple[int, int], module.stride),
             padding=cast(tuple[int, int], module.padding),
             dilation=cast(tuple[int, int], module.dilation),
             groups=module.groups,
             bias=module.bias is not None,
         )
+        conv_2d.weight.data.copy_(module.weight.data)
+        if module.bias is not None and conv_2d.bias is not None:
+            conv_2d.bias.data.copy_(module.bias.data)
+        return conv_2d
 
     if isinstance(module, nn.LSTM):
         if dropout > 0.0:
             warnings.warn("LoRA dropout is not supported for LSTMs")
 
-        return LoraLSTM(
+        lstm = LoraLSTM(
             module.input_size,
             module.hidden_size,
             r=r,
             lora_alpha=alpha,
             num_layers=module.num_layers,
-            bias=module.bias,
             batch_first=module.batch_first,
             dropout=module.dropout,
             bidirectional=module.bidirectional,
             proj_size=module.proj_size,
+            bias=module.bias,
         )
+        for param_name, param_value in module.named_parameters():
+            getattr(lstm, param_name).data.copy_(param_value.data)
+        return lstm
 
     if isinstance(module, nn.GRU):
         if dropout > 0.0:
             warnings.warn("LoRA dropout is not supported for GRUs")
 
-        return LoraGRU(
+        gru = LoraGRU(
             module.input_size,
             module.hidden_size,
             r=r,
             lora_alpha=alpha,
             num_layers=module.num_layers,
             bias=module.bias,
             batch_first=module.batch_first,
             dropout=module.dropout,
             bidirectional=module.bidirectional,
             proj_size=module.proj_size,
         )
+        for param_name, param_value in module.named_parameters():
+            getattr(gru, param_name).data.copy_(param_value.data)
+        return gru
 
     raise ValueError(f"Unsupported module type {type(module)}")
```

### Comparing `ml-starter-0.0.38/ml/models/norms.py` & `ml-starter-0.0.39/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/models/parallel.py` & `ml-starter-0.0.39/ml/models/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/models/pretrained/clip.py` & `ml-starter-0.0.39/ml/models/pretrained/clip.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/models/pretrained/hubert.py` & `ml-starter-0.0.39/ml/models/pretrained/hubert.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/models/pretrained/llama.py` & `ml-starter-0.0.39/ml/models/pretrained/llama.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/models/pretrained/sam.py` & `ml-starter-0.0.39/ml/models/pretrained/sam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/optimizers/adam.py` & `ml-starter-0.0.39/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/optimizers/adamw.py` & `ml-starter-0.0.39/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/optimizers/adan.py` & `ml-starter-0.0.39/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/optimizers/base.py` & `ml-starter-0.0.39/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/optimizers/sgd.py` & `ml-starter-0.0.39/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/optimizers/shampoo.py` & `ml-starter-0.0.39/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/scripts/cli.py` & `ml-starter-0.0.39/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/scripts/stage.py` & `ml-starter-0.0.39/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/scripts/train.py` & `ml-starter-0.0.39/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/tasks/base.py` & `ml-starter-0.0.39/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.39/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.39/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/tasks/datasets/collate.py` & `ml-starter-0.0.39/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.39/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.39/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.39/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.39/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.39/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/tasks/datasets/utils.py` & `ml-starter-0.0.39/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.39/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/tasks/environments/base.py` & `ml-starter-0.0.39/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/tasks/environments/utils.py` & `ml-starter-0.0.39/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/tasks/environments/worker.py` & `ml-starter-0.0.39/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/tasks/losses/reduce.py` & `ml-starter-0.0.39/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/tasks/rl/base.py` & `ml-starter-0.0.39/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/tasks/rl/replay.py` & `ml-starter-0.0.39/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/tasks/sl/base.py` & `ml-starter-0.0.39/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/trainers/base.py` & `ml-starter-0.0.39/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/trainers/mixins/compile.py` & `ml-starter-0.0.39/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.39/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.0.39/ml/trainers/mixins/data_parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.39/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.39/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.0.39/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.39/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.0.39/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.39/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.39/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/trainers/rl.py` & `ml-starter-0.0.39/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/trainers/sl.py` & `ml-starter-0.0.39/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/trainers/vanilla.py` & `ml-starter-0.0.39/ml/trainers/vanilla.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/utils/argparse.py` & `ml-starter-0.0.39/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/utils/atomic.py` & `ml-starter-0.0.39/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/utils/augmentation.py` & `ml-starter-0.0.39/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/utils/caching.py` & `ml-starter-0.0.39/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/utils/checkpoint.py` & `ml-starter-0.0.39/ml/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/utils/cli.py` & `ml-starter-0.0.39/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/utils/colors.py` & `ml-starter-0.0.39/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/utils/config.py` & `ml-starter-0.0.39/ml/utils/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/utils/data.py` & `ml-starter-0.0.39/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/utils/datetime.py` & `ml-starter-0.0.39/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/utils/device/auto.py` & `ml-starter-0.0.39/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/utils/device/base.py` & `ml-starter-0.0.39/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/utils/device/cpu.py` & `ml-starter-0.0.39/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/utils/device/gpu.py` & `ml-starter-0.0.39/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/utils/device/metal.py` & `ml-starter-0.0.39/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/utils/distributed.py` & `ml-starter-0.0.39/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/utils/image.py` & `ml-starter-0.0.39/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/utils/large_models.py` & `ml-starter-0.0.39/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/utils/logging.py` & `ml-starter-0.0.39/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/utils/meter.py` & `ml-starter-0.0.39/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/utils/parallel.py` & `ml-starter-0.0.39/ml/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/utils/staging.py` & `ml-starter-0.0.39/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/utils/timer.py` & `ml-starter-0.0.39/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/utils/torch_distributed.py` & `ml-starter-0.0.39/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml/utils/video.py` & `ml-starter-0.0.39/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.0.39/ml_starter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.38
+Version: 0.0.39
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.38/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.39/ml_starter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/pyproject.toml` & `ml-starter-0.0.39/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.38/setup.py` & `ml-starter-0.0.39/setup.py`

 * *Files identical despite different names*

