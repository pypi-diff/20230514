# Comparing `tmp/ml-starter-0.0.39.tar.gz` & `tmp/ml-starter-0.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.39.tar", last modified: Sun May 14 09:26:20 2023, max compression
+gzip compressed data, was "ml-starter-0.0.40.tar", last modified: Sun May 14 11:20:28 2023, max compression
```

## Comparing `ml-starter-0.0.39.tar` & `ml-starter-0.0.40.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.062536 ml-starter-0.0.39/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-14 09:26:08.000000 ml-starter-0.0.39/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-14 09:26:08.000000 ml-starter-0.0.39/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-14 09:26:20.062536 ml-starter-0.0.39/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-14 09:26:08.000000 ml-starter-0.0.39/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.046535 ml-starter-0.0.39/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.046535 ml-starter-0.0.39/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    25200 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.046535 ml-starter-0.0.39/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.046535 ml-starter-0.0.39/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    44643 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.050535 ml-starter-0.0.39/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.050535 ml-starter-0.0.39/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.050535 ml-starter-0.0.39/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    25205 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16201 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.050535 ml-starter-0.0.39/ml/models/pretrained/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/models/pretrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41249 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/models/pretrained/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    31800 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/models/pretrained/hubert.py
--rw-r--r--   0 runner    (1001) docker     (123)    22211 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/models/pretrained/llama.py
--rw-r--r--   0 runner    (1001) docker     (123)    60772 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/models/pretrained/sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.050535 ml-starter-0.0.39/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.054535 ml-starter-0.0.39/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.054535 ml-starter-0.0.39/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18456 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.054535 ml-starter-0.0.39/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.054535 ml-starter-0.0.39/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.054535 ml-starter-0.0.39/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.054535 ml-starter-0.0.39/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.054535 ml-starter-0.0.39/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.054535 ml-starter-0.0.39/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20655 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.058535 ml-starter-0.0.39/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/sl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/trainers/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.062536 ml-starter-0.0.39/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.062536 ml-starter-0.0.39/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/torch_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-05-14 09:26:08.000000 ml-starter-0.0.39/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:26:20.062536 ml-starter-0.0.39/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-14 09:26:20.000000 ml-starter-0.0.39/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-05-14 09:26:20.000000 ml-starter-0.0.39/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 09:26:20.000000 ml-starter-0.0.39/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-14 09:26:20.000000 ml-starter-0.0.39/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-14 09:26:20.000000 ml-starter-0.0.39/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-14 09:26:08.000000 ml-starter-0.0.39/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-14 09:26:08.000000 ml-starter-0.0.39/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-14 09:26:08.000000 ml-starter-0.0.39/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-14 09:26:08.000000 ml-starter-0.0.39/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-14 09:26:20.062536 ml-starter-0.0.39/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-14 09:26:08.000000 ml-starter-0.0.39/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.961558 ml-starter-0.0.40/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-14 11:20:16.000000 ml-starter-0.0.40/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-14 11:20:16.000000 ml-starter-0.0.40/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-14 11:20:28.961558 ml-starter-0.0.40/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-14 11:20:16.000000 ml-starter-0.0.40/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.945558 ml-starter-0.0.40/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.945558 ml-starter-0.0.40/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25200 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.945558 ml-starter-0.0.40/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.949558 ml-starter-0.0.40/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44643 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.949558 ml-starter-0.0.40/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.949558 ml-starter-0.0.40/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.949558 ml-starter-0.0.40/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25205 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16201 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.949558 ml-starter-0.0.40/ml/models/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/models/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41249 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/models/pretrained/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31800 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/models/pretrained/hubert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22211 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/models/pretrained/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60772 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/models/pretrained/sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.953559 ml-starter-0.0.40/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.953559 ml-starter-0.0.40/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.953559 ml-starter-0.0.40/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18456 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.953559 ml-starter-0.0.40/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.953559 ml-starter-0.0.40/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.957558 ml-starter-0.0.40/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.957558 ml-starter-0.0.40/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.957558 ml-starter-0.0.40/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.957558 ml-starter-0.0.40/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20655 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.957558 ml-starter-0.0.40/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/sl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.961558 ml-starter-0.0.40/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.961558 ml-starter-0.0.40/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/torch_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.961558 ml-starter-0.0.40/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-14 11:20:28.000000 ml-starter-0.0.40/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-05-14 11:20:28.000000 ml-starter-0.0.40/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 11:20:28.000000 ml-starter-0.0.40/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-14 11:20:28.000000 ml-starter-0.0.40/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-14 11:20:28.000000 ml-starter-0.0.40/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-14 11:20:16.000000 ml-starter-0.0.40/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-14 11:20:16.000000 ml-starter-0.0.40/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-14 11:20:16.000000 ml-starter-0.0.40/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-14 11:20:16.000000 ml-starter-0.0.40/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-14 11:20:28.961558 ml-starter-0.0.40/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-14 11:20:16.000000 ml-starter-0.0.40/setup.py
```

### Comparing `ml-starter-0.0.39/LICENSE` & `ml-starter-0.0.40/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/PKG-INFO` & `ml-starter-0.0.40/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.39
+Version: 0.0.40
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.39/README.md` & `ml-starter-0.0.40/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/api.py` & `ml-starter-0.0.40/ml/api.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/core/common_types.py` & `ml-starter-0.0.40/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/core/config.py` & `ml-starter-0.0.40/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/core/env.py` & `ml-starter-0.0.40/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/core/registry.py` & `ml-starter-0.0.40/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/core/state.py` & `ml-starter-0.0.40/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/launchers/base.py` & `ml-starter-0.0.40/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/launchers/mp.py` & `ml-starter-0.0.40/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/launchers/slurm.py` & `ml-starter-0.0.40/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/launchers/torchrun.py` & `ml-starter-0.0.40/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/loggers/base.py` & `ml-starter-0.0.40/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/loggers/meter.py` & `ml-starter-0.0.40/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/loggers/multi.py` & `ml-starter-0.0.40/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/loggers/stdout.py` & `ml-starter-0.0.40/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/loggers/tensorboard.py` & `ml-starter-0.0.40/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/lr_schedulers/base.py` & `ml-starter-0.0.40/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/lr_schedulers/constant.py` & `ml-starter-0.0.40/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.40/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.40/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/lr_schedulers/linear.py` & `ml-starter-0.0.40/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.40/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.40/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/models/activations.py` & `ml-starter-0.0.40/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/models/base.py` & `ml-starter-0.0.40/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/models/embeddings.py` & `ml-starter-0.0.40/ml/models/embeddings.py`

 * *Files 3% similar despite different names*

```diff
@@ -184,73 +184,74 @@
 @overload
 def get_positional_embeddings(
     max_tsz: int,
     embed_dim: int,
     kind: Literal["learned"],
     *,
     weight_init: InitializationType = "normal",
-    learnable: bool = True,
+    learnable: bool | None = None,
 ) -> LearnedPositionalEmbeddings:
     ...
 
 
 @overload
 def get_positional_embeddings(
     max_tsz: int,
     embed_dim: int,
     kind: Literal["sinusoidal"],
     *,
-    learnable: bool = True,
+    learnable: bool | None = None,
     base: int = 10_000,
 ) -> SinusoidalEmbeddings:
     ...
 
 
 @overload
 def get_positional_embeddings(
     max_tsz: int,
     embed_dim: int,
     kind: Literal["rotary"],
     *,
-    learnable: bool = False,
+    learnable: bool | None = None,
     base: int = 10_000,
 ) -> RotaryEmbeddings:
     ...
 
 
 @overload
 def get_positional_embeddings(
     max_tsz: int,
     embed_dim: int,
     kind: EmbeddingKind,
     *,
     weight_init: InitializationType = "normal",
-    learnable: bool = False,
+    learnable: bool | None = None,
     base: int = 10_000,
 ) -> IdentityPositionalEmbeddings | LearnedPositionalEmbeddings | SinusoidalEmbeddings | RotaryEmbeddings:
     ...
 
 
 def get_positional_embeddings(
     max_tsz: int,
     embed_dim: int,
     kind: EmbeddingKind,
     *,
     weight_init: InitializationType = "normal",
-    learnable: bool = False,
+    learnable: bool | None = None,
     base: int = 10_000,
 ) -> nn.Module:
     """Defines the common module for adding positional embeddings.
 
     Args:
         max_tsz: The maximum sequence length.
         embed_dim: The embedding dimension.
         kind: The type of embedding to use.
         weight_init: The weight initialization for learned embeddings.
-        learnable: Whether the embeddings are learnable.
+        learnable: Whether the embeddings are learnable; if not provided,
+            uses sensible defaults.
         base: The base for the sinusoidal embeddings.
 
     Returns:
         The positional embeddings module.
 
     Raises:
         ValueError: If an invalid embedding kind is supplied.
@@ -260,28 +261,28 @@
             return IdentityPositionalEmbeddings()
 
         case "learned":
             return LearnedPositionalEmbeddings(
                 max_tsz=max_tsz,
                 embed_dim=embed_dim,
                 weight_init=weight_init,
-                learnable=learnable,
+                learnable=True if learnable is None else learnable,
             )
 
         case "sinusoidal":
             return SinusoidalEmbeddings(
                 max_tsz=max_tsz,
                 embed_dim=embed_dim,
-                learnable=learnable,
+                learnable=False if learnable is None else learnable,
                 base=base,
             )
 
         case "rotary":
             return RotaryEmbeddings(
                 max_tsz=max_tsz,
                 embed_dim=embed_dim,
-                learnable=learnable,
+                learnable=False if learnable is None else learnable,
                 base=base,
             )
 
         case _:
             raise ValueError(f"Invalid embedding kind: {kind}")
```

### Comparing `ml-starter-0.0.39/ml/models/init.py` & `ml-starter-0.0.40/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/models/lora.py` & `ml-starter-0.0.40/ml/models/lora.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/models/norms.py` & `ml-starter-0.0.40/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/models/parallel.py` & `ml-starter-0.0.40/ml/models/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/models/pretrained/clip.py` & `ml-starter-0.0.40/ml/models/pretrained/clip.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/models/pretrained/hubert.py` & `ml-starter-0.0.40/ml/models/pretrained/hubert.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/models/pretrained/llama.py` & `ml-starter-0.0.40/ml/models/pretrained/llama.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/models/pretrained/sam.py` & `ml-starter-0.0.40/ml/models/pretrained/sam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/optimizers/adam.py` & `ml-starter-0.0.40/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/optimizers/adamw.py` & `ml-starter-0.0.40/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/optimizers/adan.py` & `ml-starter-0.0.40/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/optimizers/base.py` & `ml-starter-0.0.40/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/optimizers/sgd.py` & `ml-starter-0.0.40/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/optimizers/shampoo.py` & `ml-starter-0.0.40/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/scripts/cli.py` & `ml-starter-0.0.40/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/scripts/stage.py` & `ml-starter-0.0.40/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/scripts/train.py` & `ml-starter-0.0.40/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/tasks/base.py` & `ml-starter-0.0.40/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.40/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.40/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/tasks/datasets/collate.py` & `ml-starter-0.0.40/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.40/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.40/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.40/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.40/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.40/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/tasks/datasets/utils.py` & `ml-starter-0.0.40/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.40/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/tasks/environments/base.py` & `ml-starter-0.0.40/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/tasks/environments/utils.py` & `ml-starter-0.0.40/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/tasks/environments/worker.py` & `ml-starter-0.0.40/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/tasks/losses/reduce.py` & `ml-starter-0.0.40/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/tasks/rl/base.py` & `ml-starter-0.0.40/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/tasks/rl/replay.py` & `ml-starter-0.0.40/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/tasks/sl/base.py` & `ml-starter-0.0.40/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/trainers/base.py` & `ml-starter-0.0.40/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/trainers/mixins/compile.py` & `ml-starter-0.0.40/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.40/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.0.40/ml/trainers/mixins/data_parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.40/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.40/ml/trainers/mixins/grad_clipping.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,91 +17,59 @@
 
 Global norm-based clipping clips the norm of all gradients to a maximum
 value, by dividing all gradients by the total norm if the total norm is
 greater than some threshold.
 """
 
 from dataclasses import dataclass
-from typing import Any, Callable, TypeVar
+from typing import Any, TypeVar
 
-import torch
-from torch import Tensor, nn
+from torch import nn
 from torch.distributed.fsdp.fully_sharded_data_parallel import FullyShardedDataParallel as FSDP
 from torch.optim import Optimizer
 
 from ml.core.config import conf_field
 from ml.trainers.base import BaseTrainer, BaseTrainerConfig, ModelT, TaskT
 from ml.trainers.mixins.mixed_precision import (
     MixedPrecisionTrainerConfig,
     MixedPrecisionTrainerMixin,
 )
 
 
 @dataclass
 class GradientClipping:
     clip_grad_norm: float | None = conf_field(None, help="What to clip the gradient norm to")
-    norm_type: Any = conf_field(2, help="Type of norm to use")
     clip_grad_value: float | None = conf_field(None, help="What to clip the gradient value to")
-    clip_global_grad_norm: float | None = conf_field(None, help="What to clip global gradient norm to")
-    global_norm_type: Any = conf_field(2, help="Type of global norm to use")
-    log_grad: bool = conf_field(False, help="Whether to log the gradient norm")
+    norm_type: Any = conf_field(2, help="Type of norm to use")
 
 
 @dataclass
 class GradientClippingConfig(MixedPrecisionTrainerConfig, BaseTrainerConfig):
     grad_clipping: GradientClipping = conf_field(GradientClipping(), help="Gradient clipping configuration")
 
 
 GradientClippingConfigT = TypeVar("GradientClippingConfigT", bound=GradientClippingConfig)
 
 
-def get_clip_grad_func(clip_value: float) -> Callable[[Tensor], Tensor]:
-    def func(grad: Tensor) -> Tensor:
-        return grad.clamp(-clip_value, clip_value)
-
-    return func
-
-
-def get_clip_norm_func(clip_value: float, norm_type: Any) -> Callable[[Tensor], Tensor]:
-    def func(grad: Tensor) -> Tensor:
-        grad_norm = torch.norm(grad, p=norm_type)
-        return grad * (grad_norm.clamp_max(clip_value) / grad_norm)
-
-    return func
-
-
 class GradientClippingTrainerMixin(
     MixedPrecisionTrainerMixin[GradientClippingConfigT, ModelT, TaskT],
     BaseTrainer[GradientClippingConfigT, ModelT, TaskT],
 ):
     """Defines a trainer mixin for doing gradient clipping."""
 
-    def maybe_add_grad_clipping(self, model: nn.Module) -> None:
-        clip_value = self.config.grad_clipping.clip_grad_value
+    def clip_grads(self, model: nn.Module, optim: Optimizer) -> None:
         clip_norm = self.config.grad_clipping.clip_grad_norm
-        if clip_value is not None:
-            for p in model.parameters():
-                if p.requires_grad:
-                    p.register_hook(get_clip_grad_func(clip_value))
-        if clip_norm is not None:
-            for p in model.parameters():
-                if p.requires_grad:
-                    p.register_hook(get_clip_norm_func(clip_norm, self.config.grad_clipping.norm_type))
+        clip_value = self.config.grad_clipping.clip_grad_value
+        norm_type = self.config.grad_clipping.norm_type
 
-    def clip_grads(self, model: nn.Module, optim: Optimizer) -> None:
-        clip_norm = self.config.grad_clipping.clip_global_grad_norm
-        norm_type = self.config.grad_clipping.global_norm_type
         if clip_norm is not None:
             if isinstance(model, FSDP):
                 total_norm = model.clip_grad_norm_(clip_norm, norm_type)
+                self.logger.log_scalar("total_norm", total_norm.item(), namespace="optim")
             else:
                 self.unscale_mixed_precision(optim)
                 total_norm = nn.utils.clip_grad.clip_grad_norm_(model.parameters(), clip_norm, norm_type)
-            self.logger.log_scalar("total_norm", total_norm.item(), namespace="optim")
-            if self.config.grad_clipping.log_grad:
-                self.unscale_mixed_precision(optim)
-                total_grad = sum(
-                    param.grad.norm(self.config.grad_clipping.norm_type) ** 2
-                    for param in model.parameters()
-                    if param.grad is not None
-                )
-                self.logger.log_scalar("total_grad", total_grad.item(), namespace="optim")
+                self.logger.log_scalar("total_norm", total_norm.item(), namespace="optim")
+
+        if clip_value is not None:
+            self.unscale_mixed_precision(optim)
+            nn.utils.clip_grad.clip_grad_value_(model.parameters(), clip_value)
```

### Comparing `ml-starter-0.0.39/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.0.40/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.40/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.0.40/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.40/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.40/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/trainers/rl.py` & `ml-starter-0.0.40/ml/trainers/rl.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,16 +74,21 @@
         Raises:
             ValueError: If the task is not a reinforcement learning task
         """
         if not isinstance(task, ReinforcementLearningTask):
             raise ValueError(f"Expected task to be a ReinforcementLearningTask, got {type(task)}")
 
         self._init_environment()
-        model = self._compile_model(model)
-        task_model = self._get_task_model(task, model)
+
+        with Timer("compiling model", spinner=True):
+            model = self._compile_model(model)
+
+        with Timer("building task model", spinner=True):
+            task_model = self._get_task_model(task, model)
+
         optim, lr_sched = self._get_optim_and_lr_sched(model, optimizer, lr_scheduler)
         state = self._get_state(task, model, optim, lr_sched)
 
         def on_exit(signum: int, _: FrameType | None) -> None:
             sig = signal.Signals(signum)
             self.on_exit(sig, state, task, model, optim, lr_sched)
```

### Comparing `ml-starter-0.0.39/ml/trainers/sl.py` & `ml-starter-0.0.40/ml/trainers/sl.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,19 +102,20 @@
         Raises:
             ValueError: If the task is not a supervised learning task
         """
         if not isinstance(task, SupervisedLearningTask):
             raise ValueError(f"Expected task to be a SupervisedLearningTask, got {type(task)}")
 
         self._init_environment()
-        model = self._compile_model(model)
+
+        with Timer("compiling model", spinner=True):
+            model = self._compile_model(model)
 
         with Timer("building task model", spinner=True):
             task_model = self._get_task_model(task, model)
-            self.maybe_add_grad_clipping(task_model)
 
         optim, lr_sched = self._get_optim_and_lr_sched(task_model, optimizer, lr_scheduler)
         state = self._get_state(task, model, optim, lr_sched)
 
         def on_exit(signum: int, _: FrameType | None) -> None:
             sig = signal.Signals(signum)
             self.on_exit(sig, state, task, model, optim, lr_sched)
```

### Comparing `ml-starter-0.0.39/ml/trainers/vanilla.py` & `ml-starter-0.0.40/ml/trainers/vanilla.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/utils/argparse.py` & `ml-starter-0.0.40/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/utils/atomic.py` & `ml-starter-0.0.40/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/utils/augmentation.py` & `ml-starter-0.0.40/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/utils/caching.py` & `ml-starter-0.0.40/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/utils/checkpoint.py` & `ml-starter-0.0.40/ml/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/utils/cli.py` & `ml-starter-0.0.40/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/utils/colors.py` & `ml-starter-0.0.40/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/utils/config.py` & `ml-starter-0.0.40/ml/utils/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/utils/data.py` & `ml-starter-0.0.40/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/utils/datetime.py` & `ml-starter-0.0.40/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/utils/device/auto.py` & `ml-starter-0.0.40/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/utils/device/base.py` & `ml-starter-0.0.40/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/utils/device/cpu.py` & `ml-starter-0.0.40/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/utils/device/gpu.py` & `ml-starter-0.0.40/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/utils/device/metal.py` & `ml-starter-0.0.40/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/utils/distributed.py` & `ml-starter-0.0.40/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/utils/image.py` & `ml-starter-0.0.40/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/utils/large_models.py` & `ml-starter-0.0.40/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/utils/logging.py` & `ml-starter-0.0.40/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/utils/meter.py` & `ml-starter-0.0.40/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/utils/parallel.py` & `ml-starter-0.0.40/ml/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/utils/staging.py` & `ml-starter-0.0.40/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/utils/timer.py` & `ml-starter-0.0.40/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/utils/torch_distributed.py` & `ml-starter-0.0.40/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml/utils/video.py` & `ml-starter-0.0.40/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.0.40/ml_starter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.39
+Version: 0.0.40
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.39/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.40/ml_starter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/pyproject.toml` & `ml-starter-0.0.40/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.39/setup.py` & `ml-starter-0.0.40/setup.py`

 * *Files identical despite different names*

