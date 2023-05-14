# Comparing `tmp/ultralytics-8.0.98.tar.gz` & `tmp/ultralytics-8.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultralytics-8.0.98.tar", last modified: Wed May 10 23:16:51 2023, max compression
+gzip compressed data, was "ultralytics-8.0.99.tar", last modified: Fri May 12 16:35:37 2023, max compression
```

## Comparing `ultralytics-8.0.98.tar` & `ultralytics-8.0.99.tar`

### file list

```diff
@@ -1,194 +1,194 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.723256 ultralytics-8.0.98/
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-10 23:15:33.000000 ultralytics-8.0.98/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-10 23:15:33.000000 ultralytics-8.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-10 23:15:33.000000 ultralytics-8.0.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    25911 2023-05-10 23:16:51.723256 ultralytics-8.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24235 2023-05-10 23:15:33.000000 ultralytics-8.0.98/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    23225 2023-05-10 23:15:33.000000 ultralytics-8.0.98/README.zh-CN.md
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-10 23:15:33.000000 ultralytics-8.0.98/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-10 23:16:51.723256 ultralytics-8.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-10 23:15:33.000000 ultralytics-8.0.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.703256 ultralytics-8.0.98/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-10 23:15:33.000000 ultralytics-8.0.98/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-10 23:15:33.000000 ultralytics-8.0.98/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-05-10 23:15:33.000000 ultralytics-8.0.98/tests/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.703256 ultralytics-8.0.98/ultralytics/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.707256 ultralytics-8.0.98/ultralytics/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   137419 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/assets/bus.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    50427 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/assets/zidane.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.707256 ultralytics-8.0.98/ultralytics/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/Argoverse.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/GlobalWheat2020.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    42439 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/ImageNet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/Objects365.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/SKU-110K.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/VOC.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/VisDrone.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/coco-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/coco.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/coco128-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/coco128.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/coco8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/coco8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/coco8.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/xView.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.707256 ultralytics-8.0.98/ultralytics/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/hub/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/hub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.699256 ultralytics-8.0.98/ultralytics/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.707256 ultralytics-8.0.98/ultralytics/models/rt-detr/
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/models/rt-detr/rt-detr-l.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/models/rt-detr/rt-detr-x.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.707256 ultralytics-8.0.98/ultralytics/models/v3/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/models/v3/yolov3-spp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/models/v3/yolov3-tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/models/v3/yolov3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.707256 ultralytics-8.0.98/ultralytics/models/v5/
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/models/v5/yolov5-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/models/v5/yolov5.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.707256 ultralytics-8.0.98/ultralytics/models/v8/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/models/v8/yolov8-cls.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/models/v8/yolov8-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/models/v8/yolov8-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/models/v8/yolov8-pose-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/models/v8/yolov8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/models/v8/yolov8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/models/v8/yolov8.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.711256 ultralytics-8.0.98/ultralytics/nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24244 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/nn/autobackend.py
--rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/nn/autoshape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.711256 ultralytics-8.0.98/ultralytics/nn/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/nn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/nn/modules/block.py
--rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/nn/modules/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    17115 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/nn/modules/head.py
--rw-r--r--   0 runner    (1001) docker     (123)    16394 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/nn/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/nn/modules/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28327 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/nn/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.711256 ultralytics-8.0.98/ultralytics/tracker/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/tracker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.711256 ultralytics-8.0.98/ultralytics/tracker/cfg/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/tracker/cfg/botsort.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/tracker/cfg/bytetrack.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/tracker/track.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.711256 ultralytics-8.0.98/ultralytics/tracker/trackers/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/tracker/trackers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/tracker/trackers/basetrack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/tracker/trackers/bot_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/tracker/trackers/byte_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.711256 ultralytics-8.0.98/ultralytics/tracker/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/tracker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/tracker/utils/gmc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18420 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/tracker/utils/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/tracker/utils/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.711256 ultralytics-8.0.98/ultralytics/vit/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.711256 ultralytics-8.0.98/ultralytics/vit/rtdetr/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/rtdetr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/rtdetr/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/rtdetr/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/rtdetr/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.711256 ultralytics-8.0.98/ultralytics/vit/sam/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/sam/amg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/sam/autosize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/sam/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/sam/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.715256 ultralytics-8.0.98/ultralytics/vit/sam/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/sam/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/sam/modules/decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    22502 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/sam/modules/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/sam/modules/mask_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/sam/modules/prompt_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/sam/modules/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/sam/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/sam/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.715256 ultralytics-8.0.98/ultralytics/yolo/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.715256 ultralytics-8.0.98/ultralytics/yolo/cfg/
--rw-r--r--   0 runner    (1001) docker     (123)    17817 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/cfg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/cfg/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.715256 ultralytics-8.0.98/ultralytics/yolo/data/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/data/annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)    33512 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/data/augment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/data/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/data/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/data/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.715256 ultralytics-8.0.98/ultralytics/yolo/data/dataloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/data/dataloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/data/dataloaders/stream_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17646 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/data/dataloaders/v5augmentations.py
--rw-r--r--   0 runner    (1001) docker     (123)    51260 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/data/dataloaders/v5loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/data/dataset_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    23582 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.715256 ultralytics-8.0.98/ultralytics/yolo/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40265 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/engine/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21937 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/engine/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/engine/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    20634 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/engine/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    31310 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/engine/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11462 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/engine/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.719256 ultralytics-8.0.98/ultralytics/yolo/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    27780 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/autobatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.719256 ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/clearml.py
--rw-r--r--   0 runner    (1001) docker     (123)    13190 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/comet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/neptune.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/raytune.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/wb.py
--rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    41927 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    28191 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    24037 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/tal.py
--rw-r--r--   0 runner    (1001) docker     (123)    20153 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.719256 ultralytics-8.0.98/ultralytics/yolo/v8/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.719256 ultralytics-8.0.98/ultralytics/yolo/v8/classify/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/classify/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/classify/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/classify/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.719256 ultralytics-8.0.98/ultralytics/yolo/v8/detect/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/detect/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/detect/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    14486 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/detect/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.723256 ultralytics-8.0.98/ultralytics/yolo/v8/pose/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/pose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/pose/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/pose/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/pose/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.723256 ultralytics-8.0.98/ultralytics/yolo/v8/segment/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/segment/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/segment/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/segment/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.703256 ultralytics-8.0.98/ultralytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25911 2023-05-10 23:16:51.000000 ultralytics-8.0.98/ultralytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-10 23:16:51.000000 ultralytics-8.0.98/ultralytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 23:16:51.000000 ultralytics-8.0.98/ultralytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-10 23:16:51.000000 ultralytics-8.0.98/ultralytics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-10 23:16:51.000000 ultralytics-8.0.98/ultralytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 23:16:51.000000 ultralytics-8.0.98/ultralytics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.899440 ultralytics-8.0.99/
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-12 16:33:52.000000 ultralytics-8.0.99/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-12 16:33:52.000000 ultralytics-8.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-12 16:33:52.000000 ultralytics-8.0.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    25911 2023-05-12 16:35:37.899440 ultralytics-8.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24235 2023-05-12 16:33:52.000000 ultralytics-8.0.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    23225 2023-05-12 16:33:52.000000 ultralytics-8.0.99/README.zh-CN.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-12 16:33:52.000000 ultralytics-8.0.99/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-12 16:35:37.899440 ultralytics-8.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-12 16:33:52.000000 ultralytics-8.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.875440 ultralytics-8.0.99/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-12 16:33:52.000000 ultralytics-8.0.99/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-12 16:33:52.000000 ultralytics-8.0.99/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-05-12 16:33:52.000000 ultralytics-8.0.99/tests/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.875440 ultralytics-8.0.99/ultralytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.875440 ultralytics-8.0.99/ultralytics/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   137419 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/assets/bus.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    50427 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/assets/zidane.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.879439 ultralytics-8.0.99/ultralytics/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/datasets/Argoverse.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/datasets/GlobalWheat2020.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    42439 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/datasets/ImageNet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/datasets/Objects365.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/datasets/SKU-110K.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/datasets/VOC.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/datasets/VisDrone.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/datasets/coco-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/datasets/coco.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/datasets/coco128-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/datasets/coco128.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/datasets/coco8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/datasets/coco8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/datasets/coco8.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/datasets/xView.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.879439 ultralytics-8.0.99/ultralytics/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/hub/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/hub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.871439 ultralytics-8.0.99/ultralytics/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.879439 ultralytics-8.0.99/ultralytics/models/rt-detr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/models/rt-detr/rt-detr-l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/models/rt-detr/rt-detr-x.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.879439 ultralytics-8.0.99/ultralytics/models/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/models/v3/yolov3-spp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/models/v3/yolov3-tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/models/v3/yolov3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.883440 ultralytics-8.0.99/ultralytics/models/v5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/models/v5/yolov5-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/models/v5/yolov5.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.883440 ultralytics-8.0.99/ultralytics/models/v8/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/models/v8/yolov8-cls.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/models/v8/yolov8-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/models/v8/yolov8-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/models/v8/yolov8-pose-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/models/v8/yolov8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/models/v8/yolov8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/models/v8/yolov8.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.883440 ultralytics-8.0.99/ultralytics/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24244 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/nn/autobackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/nn/autoshape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.883440 ultralytics-8.0.99/ultralytics/nn/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/nn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/nn/modules/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/nn/modules/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17115 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/nn/modules/head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16394 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/nn/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/nn/modules/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28327 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/nn/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.883440 ultralytics-8.0.99/ultralytics/tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/tracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.883440 ultralytics-8.0.99/ultralytics/tracker/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/tracker/cfg/botsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/tracker/cfg/bytetrack.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/tracker/track.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.883440 ultralytics-8.0.99/ultralytics/tracker/trackers/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/tracker/trackers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/tracker/trackers/basetrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/tracker/trackers/bot_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/tracker/trackers/byte_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.887440 ultralytics-8.0.99/ultralytics/tracker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/tracker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/tracker/utils/gmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18420 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/tracker/utils/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/tracker/utils/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.887440 ultralytics-8.0.99/ultralytics/vit/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/vit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.887440 ultralytics-8.0.99/ultralytics/vit/rtdetr/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/vit/rtdetr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/vit/rtdetr/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/vit/rtdetr/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/vit/rtdetr/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.887440 ultralytics-8.0.99/ultralytics/vit/sam/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/vit/sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/vit/sam/amg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/vit/sam/autosize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/vit/sam/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/vit/sam/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.887440 ultralytics-8.0.99/ultralytics/vit/sam/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/vit/sam/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/vit/sam/modules/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22502 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/vit/sam/modules/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/vit/sam/modules/mask_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/vit/sam/modules/prompt_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/vit/sam/modules/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/vit/sam/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/vit/sam/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.887440 ultralytics-8.0.99/ultralytics/yolo/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.887440 ultralytics-8.0.99/ultralytics/yolo/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)    17817 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/cfg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/cfg/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.891440 ultralytics-8.0.99/ultralytics/yolo/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/data/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33512 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/data/augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/data/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/data/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.891440 ultralytics-8.0.99/ultralytics/yolo/data/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/data/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/data/dataloaders/stream_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17646 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/data/dataloaders/v5augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51260 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/data/dataloaders/v5loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/data/dataset_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23582 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.891440 ultralytics-8.0.99/ultralytics/yolo/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40265 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/engine/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21937 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/engine/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/engine/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20634 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/engine/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32067 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/engine/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11462 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/engine/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.895440 ultralytics-8.0.99/ultralytics/yolo/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    27780 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/utils/autobatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/utils/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.895440 ultralytics-8.0.99/ultralytics/yolo/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/utils/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/utils/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/utils/callbacks/clearml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13190 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/utils/callbacks/comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/utils/callbacks/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/utils/callbacks/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/utils/callbacks/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/utils/callbacks/raytune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/utils/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/utils/callbacks/wb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/utils/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/utils/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41927 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28191 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/utils/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24037 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/utils/tal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20153 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/utils/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.895440 ultralytics-8.0.99/ultralytics/yolo/v8/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/v8/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.899440 ultralytics-8.0.99/ultralytics/yolo/v8/classify/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/v8/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/v8/classify/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/v8/classify/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/v8/classify/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.899440 ultralytics-8.0.99/ultralytics/yolo/v8/detect/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/v8/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/v8/detect/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/v8/detect/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14486 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/v8/detect/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.899440 ultralytics-8.0.99/ultralytics/yolo/v8/pose/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/v8/pose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/v8/pose/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/v8/pose/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/v8/pose/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.899440 ultralytics-8.0.99/ultralytics/yolo/v8/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/v8/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/v8/segment/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/v8/segment/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-05-12 16:33:52.000000 ultralytics-8.0.99/ultralytics/yolo/v8/segment/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:35:37.875440 ultralytics-8.0.99/ultralytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25911 2023-05-12 16:35:37.000000 ultralytics-8.0.99/ultralytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-12 16:35:37.000000 ultralytics-8.0.99/ultralytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 16:35:37.000000 ultralytics-8.0.99/ultralytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-12 16:35:37.000000 ultralytics-8.0.99/ultralytics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-12 16:35:37.000000 ultralytics-8.0.99/ultralytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-12 16:35:37.000000 ultralytics-8.0.99/ultralytics.egg-info/top_level.txt
```

### Comparing `ultralytics-8.0.98/CONTRIBUTING.md` & `ultralytics-8.0.99/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/LICENSE` & `ultralytics-8.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/PKG-INFO` & `ultralytics-8.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.0.98
+Version: 8.0.99
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Home-page: https://github.com/ultralytics/ultralytics
 Author: Ultralytics
 Author-email: hello@ultralytics.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.0.98 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ultralytics Version: 8.0.99 Summary: Ultralytics
 YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation,
 pose estimation and image classification. Home-page: https://github.com/
 ultralytics/ultralytics Author: Ultralytics Author-email: hello@ultralytics.com
 License: AGPL-3.0 Project-URL: Bug Reports, https://github.com/ultralytics/
 ultralytics/issues Project-URL: Funding, https://ultralytics.com Project-URL:
 Source, https://github.com/ultralytics/ultralytics Keywords: machine-
 learning,deep-
```

### Comparing `ultralytics-8.0.98/README.md` & `ultralytics-8.0.99/README.md`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/README.zh-CN.md` & `ultralytics-8.0.99/README.zh-CN.md`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/requirements.txt` & `ultralytics-8.0.99/requirements.txt`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/setup.cfg` & `ultralytics-8.0.99/setup.cfg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/setup.py` & `ultralytics-8.0.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,15 @@
             'check-manifest',
             'pytest',
             'pytest-cov',
             'coverage',
             'mkdocs-material',
             'mkdocstrings[python]',
             'mkdocs-redirects',  # for 301 redirects
-            'mkdocs-git-revision-date-localized-plugin',  # for created/updated dates
-            'mkdocs-ultralytics-plugin',  # for meta descriptions and images
+            'mkdocs-ultralytics-plugin',  # for meta descriptions and images, dates and authors
         ],
         'export': ['coremltools>=6.0', 'openvino-dev>=2022.3', 'tensorflowjs'],  # automatically installs tensorflow
     },
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
```

### Comparing `ultralytics-8.0.98/tests/test_cli.py` & `ultralytics-8.0.99/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/tests/test_engine.py` & `ultralytics-8.0.99/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/tests/test_python.py` & `ultralytics-8.0.99/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/assets/bus.jpg` & `ultralytics-8.0.99/ultralytics/assets/bus.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/assets/zidane.jpg` & `ultralytics-8.0.99/ultralytics/assets/zidane.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/datasets/Argoverse.yaml` & `ultralytics-8.0.99/ultralytics/datasets/Argoverse.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/datasets/GlobalWheat2020.yaml` & `ultralytics-8.0.99/ultralytics/datasets/GlobalWheat2020.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/datasets/ImageNet.yaml` & `ultralytics-8.0.99/ultralytics/datasets/ImageNet.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/datasets/Objects365.yaml` & `ultralytics-8.0.99/ultralytics/datasets/Objects365.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/datasets/SKU-110K.yaml` & `ultralytics-8.0.99/ultralytics/datasets/SKU-110K.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/datasets/VOC.yaml` & `ultralytics-8.0.99/ultralytics/datasets/VOC.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/datasets/VisDrone.yaml` & `ultralytics-8.0.99/ultralytics/datasets/VisDrone.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/datasets/coco-pose.yaml` & `ultralytics-8.0.99/ultralytics/datasets/coco-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/datasets/coco.yaml` & `ultralytics-8.0.99/ultralytics/datasets/coco.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/datasets/coco128-seg.yaml` & `ultralytics-8.0.99/ultralytics/datasets/coco128-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/datasets/coco128.yaml` & `ultralytics-8.0.99/ultralytics/datasets/coco128.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/datasets/coco8-pose.yaml` & `ultralytics-8.0.99/ultralytics/datasets/coco8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/datasets/coco8-seg.yaml` & `ultralytics-8.0.99/ultralytics/datasets/coco8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/datasets/coco8.yaml` & `ultralytics-8.0.99/ultralytics/datasets/coco8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/datasets/xView.yaml` & `ultralytics-8.0.99/ultralytics/datasets/xView.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/hub/__init__.py` & `ultralytics-8.0.99/ultralytics/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/hub/auth.py` & `ultralytics-8.0.99/ultralytics/hub/auth.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/hub/session.py` & `ultralytics-8.0.99/ultralytics/hub/session.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/hub/utils.py` & `ultralytics-8.0.99/ultralytics/hub/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/models/rt-detr/rt-detr-l.yaml` & `ultralytics-8.0.99/ultralytics/models/rt-detr/rt-detr-l.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/models/rt-detr/rt-detr-x.yaml` & `ultralytics-8.0.99/ultralytics/models/rt-detr/rt-detr-x.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/models/v3/yolov3-spp.yaml` & `ultralytics-8.0.99/ultralytics/models/v3/yolov3-spp.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/models/v3/yolov3-tiny.yaml` & `ultralytics-8.0.99/ultralytics/models/v3/yolov3-tiny.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/models/v3/yolov3.yaml` & `ultralytics-8.0.99/ultralytics/models/v3/yolov3.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/models/v5/yolov5-p6.yaml` & `ultralytics-8.0.99/ultralytics/models/v5/yolov5-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/models/v5/yolov5.yaml` & `ultralytics-8.0.99/ultralytics/models/v5/yolov5.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/models/v8/yolov8-cls.yaml` & `ultralytics-8.0.99/ultralytics/models/v8/yolov8-cls.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/models/v8/yolov8-p2.yaml` & `ultralytics-8.0.99/ultralytics/models/v8/yolov8-p2.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/models/v8/yolov8-p6.yaml` & `ultralytics-8.0.99/ultralytics/models/v8/yolov8-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/models/v8/yolov8-pose-p6.yaml` & `ultralytics-8.0.99/ultralytics/models/v8/yolov8-pose-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/models/v8/yolov8-pose.yaml` & `ultralytics-8.0.99/ultralytics/models/v8/yolov8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/models/v8/yolov8-seg.yaml` & `ultralytics-8.0.99/ultralytics/models/v8/yolov8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/models/v8/yolov8.yaml` & `ultralytics-8.0.99/ultralytics/models/v8/yolov8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/nn/autobackend.py` & `ultralytics-8.0.99/ultralytics/nn/autobackend.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/nn/autoshape.py` & `ultralytics-8.0.99/ultralytics/nn/autoshape.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/nn/modules/__init__.py` & `ultralytics-8.0.99/ultralytics/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/nn/modules/block.py` & `ultralytics-8.0.99/ultralytics/nn/modules/block.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/nn/modules/conv.py` & `ultralytics-8.0.99/ultralytics/nn/modules/conv.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/nn/modules/head.py` & `ultralytics-8.0.99/ultralytics/nn/modules/head.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/nn/modules/transformer.py` & `ultralytics-8.0.99/ultralytics/nn/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/nn/modules/utils.py` & `ultralytics-8.0.99/ultralytics/nn/modules/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/nn/tasks.py` & `ultralytics-8.0.99/ultralytics/nn/tasks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/tracker/cfg/botsort.yaml` & `ultralytics-8.0.99/ultralytics/tracker/cfg/botsort.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/tracker/cfg/bytetrack.yaml` & `ultralytics-8.0.99/ultralytics/tracker/cfg/bytetrack.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/tracker/track.py` & `ultralytics-8.0.99/ultralytics/tracker/track.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/tracker/trackers/basetrack.py` & `ultralytics-8.0.99/ultralytics/tracker/trackers/basetrack.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/tracker/trackers/bot_sort.py` & `ultralytics-8.0.99/ultralytics/tracker/trackers/bot_sort.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/tracker/trackers/byte_tracker.py` & `ultralytics-8.0.99/ultralytics/tracker/trackers/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/tracker/utils/gmc.py` & `ultralytics-8.0.99/ultralytics/tracker/utils/gmc.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/tracker/utils/kalman_filter.py` & `ultralytics-8.0.99/ultralytics/tracker/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/tracker/utils/matching.py` & `ultralytics-8.0.99/ultralytics/tracker/utils/matching.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/vit/rtdetr/model.py` & `ultralytics-8.0.99/ultralytics/vit/rtdetr/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from pathlib import Path
 
 from ultralytics.nn.tasks import DetectionModel, attempt_load_one_weight, yaml_model_load
 from ultralytics.yolo.cfg import get_cfg
 from ultralytics.yolo.engine.exporter import Exporter
 from ultralytics.yolo.utils import DEFAULT_CFG, DEFAULT_CFG_DICT
 from ultralytics.yolo.utils.checks import check_imgsz
+from ultralytics.yolo.utils.torch_utils import model_info
 
 from ...yolo.utils.torch_utils import smart_inference_mode
 from .predict import RTDETRPredictor
 from .val import RTDETRValidator
 
 
 class RTDETR:
@@ -80,14 +81,18 @@
         args = get_cfg(cfg=DEFAULT_CFG, overrides=overrides)
         args.imgsz = check_imgsz(args.imgsz, max_dim=1)
         validator = RTDETRValidator(args=args)
         validator(model=self.model)
         self.metrics = validator.metrics
         return validator.metrics
 
+    def info(self, verbose=True):
+        """Get model info"""
+        return model_info(self.model, verbose=verbose)
+
     @smart_inference_mode()
     def export(self, **kwargs):
         """
         Export model.
 
         Args:
             **kwargs : Any other args accepted by the predictors. To see all args check 'configuration' section in docs
```

### Comparing `ultralytics-8.0.98/ultralytics/vit/rtdetr/predict.py` & `ultralytics-8.0.99/ultralytics/vit/rtdetr/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/vit/rtdetr/val.py` & `ultralytics-8.0.99/ultralytics/vit/rtdetr/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/vit/sam/amg.py` & `ultralytics-8.0.99/ultralytics/vit/sam/amg.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/vit/sam/autosize.py` & `ultralytics-8.0.99/ultralytics/vit/sam/autosize.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/vit/sam/build.py` & `ultralytics-8.0.99/ultralytics/vit/sam/build.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/vit/sam/model.py` & `ultralytics-8.0.99/ultralytics/vit/sam/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/vit/sam/modules/decoders.py` & `ultralytics-8.0.99/ultralytics/vit/sam/modules/decoders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/vit/sam/modules/encoders.py` & `ultralytics-8.0.99/ultralytics/vit/sam/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/vit/sam/modules/mask_generator.py` & `ultralytics-8.0.99/ultralytics/vit/sam/modules/mask_generator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/vit/sam/modules/prompt_predictor.py` & `ultralytics-8.0.99/ultralytics/vit/sam/modules/prompt_predictor.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/vit/sam/modules/sam.py` & `ultralytics-8.0.99/ultralytics/vit/sam/modules/sam.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/vit/sam/modules/transformer.py` & `ultralytics-8.0.99/ultralytics/vit/sam/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/vit/sam/predict.py` & `ultralytics-8.0.99/ultralytics/vit/sam/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/cfg/__init__.py` & `ultralytics-8.0.99/ultralytics/yolo/cfg/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/cfg/default.yaml` & `ultralytics-8.0.99/ultralytics/yolo/cfg/default.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/data/annotator.py` & `ultralytics-8.0.99/ultralytics/yolo/data/annotator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/data/augment.py` & `ultralytics-8.0.99/ultralytics/yolo/data/augment.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/data/base.py` & `ultralytics-8.0.99/ultralytics/yolo/data/base.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/data/build.py` & `ultralytics-8.0.99/ultralytics/yolo/data/build.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/data/converter.py` & `ultralytics-8.0.99/ultralytics/yolo/data/converter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/data/dataloaders/stream_loaders.py` & `ultralytics-8.0.99/ultralytics/yolo/data/dataloaders/stream_loaders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/data/dataloaders/v5augmentations.py` & `ultralytics-8.0.99/ultralytics/yolo/data/dataloaders/v5augmentations.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/data/dataloaders/v5loader.py` & `ultralytics-8.0.99/ultralytics/yolo/data/dataloaders/v5loader.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/data/dataset.py` & `ultralytics-8.0.99/ultralytics/yolo/data/dataset.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/data/dataset_wrappers.py` & `ultralytics-8.0.99/ultralytics/yolo/data/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/data/utils.py` & `ultralytics-8.0.99/ultralytics/yolo/data/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/engine/exporter.py` & `ultralytics-8.0.99/ultralytics/yolo/engine/exporter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/engine/model.py` & `ultralytics-8.0.99/ultralytics/yolo/engine/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/engine/predictor.py` & `ultralytics-8.0.99/ultralytics/yolo/engine/predictor.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/engine/results.py` & `ultralytics-8.0.99/ultralytics/yolo/engine/results.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/engine/trainer.py` & `ultralytics-8.0.99/ultralytics/yolo/engine/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,14 +186,25 @@
             except Exception as e:
                 raise e
             finally:
                 ddp_cleanup(self, str(file))
         else:
             self._do_train(world_size)
 
+    def _pre_caching_dataset(self):
+        """
+        Caching dataset before training to avoid NCCL timeout.
+        Must be done before DDP initialization.
+        See https://github.com/ultralytics/ultralytics/pull/2549 for details.
+        """
+        if RANK in (-1, 0):
+            LOGGER.info('Pre-caching dataset to avoid NCCL timeout')
+            self.get_dataloader(self.trainset, batch_size=1, rank=RANK, mode='train')
+            self.get_dataloader(self.testset, batch_size=1, rank=-1, mode='val')
+
     def _setup_ddp(self, world_size):
         """Initializes and sets the DistributedDataParallel parameters for training."""
         torch.cuda.set_device(RANK)
         self.device = torch.device('cuda', RANK)
         LOGGER.info(f'DDP settings: RANK {RANK}, WORLD_SIZE {world_size}, DEVICE {self.device}')
         dist.init_process_group('nccl' if dist.is_nccl_available() else 'gloo', rank=RANK, world_size=world_size)
 
@@ -259,14 +270,15 @@
         self.resume_training(ckpt)
         self.scheduler.last_epoch = self.start_epoch - 1  # do not move
         self.run_callbacks('on_pretrain_routine_end')
 
     def _do_train(self, world_size=1):
         """Train completed, evaluate and plot if specified by arguments."""
         if world_size > 1:
+            self._pre_caching_dataset()
             self._setup_ddp(world_size)
 
         self._setup_train(world_size)
 
         self.epoch_time = None
         self.epoch_time_start = time.time()
         self.train_time_start = time.time()
@@ -545,18 +557,23 @@
                     self.run_callbacks('on_fit_epoch_end')
 
     def check_resume(self):
         """Check if resume checkpoint exists and update arguments accordingly."""
         resume = self.args.resume
         if resume:
             try:
-                last = Path(
-                    check_file(resume) if isinstance(resume, (str,
-                                                              Path)) and Path(resume).exists() else get_latest_run())
-                self.args = get_cfg(attempt_load_weights(last).args)
+                exists = isinstance(resume, (str, Path)) and Path(resume).exists()
+                last = Path(check_file(resume) if exists else get_latest_run())
+
+                # Check that resume data YAML exists, otherwise strip to force re-download of dataset
+                ckpt_args = attempt_load_weights(last).args
+                if not Path(ckpt_args['data']).exists():
+                    ckpt_args['data'] = self.args.data
+
+                self.args = get_cfg(ckpt_args)
                 self.args.model, resume = str(last), True  # reinstate
             except Exception as e:
                 raise FileNotFoundError('Resume checkpoint not found. Please pass a valid checkpoint to resume from, '
                                         "i.e. 'yolo train resume model=path/to/last.pt'") from e
         self.resume = resume
 
     def resume_training(self, ckpt):
```

### Comparing `ultralytics-8.0.98/ultralytics/yolo/engine/validator.py` & `ultralytics-8.0.99/ultralytics/yolo/engine/validator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/utils/__init__.py` & `ultralytics-8.0.99/ultralytics/yolo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/utils/autobatch.py` & `ultralytics-8.0.99/ultralytics/yolo/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/utils/benchmarks.py` & `ultralytics-8.0.99/ultralytics/yolo/utils/benchmarks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/base.py` & `ultralytics-8.0.99/ultralytics/yolo/utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/clearml.py` & `ultralytics-8.0.99/ultralytics/yolo/utils/callbacks/clearml.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/comet.py` & `ultralytics-8.0.99/ultralytics/yolo/utils/callbacks/comet.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/hub.py` & `ultralytics-8.0.99/ultralytics/yolo/utils/callbacks/hub.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/mlflow.py` & `ultralytics-8.0.99/ultralytics/yolo/utils/callbacks/mlflow.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/neptune.py` & `ultralytics-8.0.99/ultralytics/yolo/utils/callbacks/neptune.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/tensorboard.py` & `ultralytics-8.0.99/ultralytics/yolo/utils/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/wb.py` & `ultralytics-8.0.99/ultralytics/yolo/utils/callbacks/wb.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/utils/checks.py` & `ultralytics-8.0.99/ultralytics/yolo/utils/checks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/utils/dist.py` & `ultralytics-8.0.99/ultralytics/yolo/utils/dist.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/utils/downloads.py` & `ultralytics-8.0.99/ultralytics/yolo/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/utils/files.py` & `ultralytics-8.0.99/ultralytics/yolo/utils/files.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/utils/instance.py` & `ultralytics-8.0.99/ultralytics/yolo/utils/instance.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/utils/loss.py` & `ultralytics-8.0.99/ultralytics/yolo/utils/loss.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/utils/metrics.py` & `ultralytics-8.0.99/ultralytics/yolo/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/utils/ops.py` & `ultralytics-8.0.99/ultralytics/yolo/utils/ops.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/utils/plotting.py` & `ultralytics-8.0.99/ultralytics/yolo/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/utils/tal.py` & `ultralytics-8.0.99/ultralytics/yolo/utils/tal.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/utils/torch_utils.py` & `ultralytics-8.0.99/ultralytics/yolo/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/utils/tuner.py` & `ultralytics-8.0.99/ultralytics/yolo/utils/tuner.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/v8/classify/predict.py` & `ultralytics-8.0.99/ultralytics/yolo/v8/classify/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/v8/classify/train.py` & `ultralytics-8.0.99/ultralytics/yolo/v8/classify/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/v8/classify/val.py` & `ultralytics-8.0.99/ultralytics/yolo/v8/classify/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/v8/detect/predict.py` & `ultralytics-8.0.99/ultralytics/yolo/v8/detect/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/v8/detect/train.py` & `ultralytics-8.0.99/ultralytics/yolo/v8/detect/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/v8/detect/val.py` & `ultralytics-8.0.99/ultralytics/yolo/v8/detect/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/v8/pose/predict.py` & `ultralytics-8.0.99/ultralytics/yolo/v8/pose/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/v8/pose/train.py` & `ultralytics-8.0.99/ultralytics/yolo/v8/pose/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/v8/pose/val.py` & `ultralytics-8.0.99/ultralytics/yolo/v8/pose/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/v8/segment/predict.py` & `ultralytics-8.0.99/ultralytics/yolo/v8/segment/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/v8/segment/train.py` & `ultralytics-8.0.99/ultralytics/yolo/v8/segment/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics/yolo/v8/segment/val.py` & `ultralytics-8.0.99/ultralytics/yolo/v8/segment/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.98/ultralytics.egg-info/PKG-INFO` & `ultralytics-8.0.99/ultralytics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.0.98
+Version: 8.0.99
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Home-page: https://github.com/ultralytics/ultralytics
 Author: Ultralytics
 Author-email: hello@ultralytics.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.0.98 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ultralytics Version: 8.0.99 Summary: Ultralytics
 YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation,
 pose estimation and image classification. Home-page: https://github.com/
 ultralytics/ultralytics Author: Ultralytics Author-email: hello@ultralytics.com
 License: AGPL-3.0 Project-URL: Bug Reports, https://github.com/ultralytics/
 ultralytics/issues Project-URL: Funding, https://ultralytics.com Project-URL:
 Source, https://github.com/ultralytics/ultralytics Keywords: machine-
 learning,deep-
```

### Comparing `ultralytics-8.0.98/ultralytics.egg-info/SOURCES.txt` & `ultralytics-8.0.99/ultralytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

