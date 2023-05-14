# Comparing `tmp/trojanzoo-1.1.1.tar.gz` & `tmp/trojanzoo-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trojanzoo-1.1.1.tar", last modified: Wed Jul 13 23:33:13 2022, max compression
+gzip compressed data, was "trojanzoo-2.0.0.tar", last modified: Sun May 14 09:58:21 2023, max compression
```

## Comparing `trojanzoo-1.1.1.tar` & `trojanzoo-2.0.0.tar`

### file list

```diff
@@ -1,345 +1,341 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.712250 trojanzoo-1.1.1/
--rw-r--r--   0 root         (0) root         (0)    35149 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      316 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9619 2022-07-13 23:33:13.712250 trojanzoo-1.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8708 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.672247 trojanzoo-1.1.1/docs/
--rw-r--r--   0 root         (0) root         (0)      855 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)      175 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.672247 trojanzoo-1.1.1/docs/source/
--rw-r--r--   0 root         (0) root         (0)     3968 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.672247 trojanzoo-1.1.1/docs/source/images/
--rw-r--r--   0 root         (0) root         (0)     4286 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/images/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.672247 trojanzoo-1.1.1/docs/source/images/logo/
--rw-r--r--   0 root         (0) root         (0)     8520 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/images/logo/trojanzoo-logo-dark.svg
--rw-r--r--   0 root         (0) root         (0)     5671 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/images/logo/trojanzoo-logo-icon.svg
--rw-r--r--   0 root         (0) root         (0)     7587 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/images/logo/trojanzoo-logo.svg
--rw-r--r--   0 root         (0) root         (0)   570067 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/images/screenshot.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.676247 trojanzoo-1.1.1/docs/source/images/trojanvision/
--rw-r--r--   0 root         (0) root         (0)    83160 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/images/trojanvision/center_cropped.png
--rw-r--r--   0 root         (0) root         (0)    16840 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/images/trojanvision/grad_cam.png
--rw-r--r--   0 root         (0) root         (0)    79679 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/images/trojanvision/grad_cam_impose.png
--rw-r--r--   0 root         (0) root         (0)    51879 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/images/trojanvision/saliency_map.png
--rw-r--r--   0 root         (0) root         (0)    92604 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/images/trojanvision/saliency_map_impose.png
--rw-r--r--   0 root         (0) root         (0)    68027 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/images/trojanzoo-logo-readme.svg
--rw-r--r--   0 root         (0) root         (0)      507 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.676247 trojanzoo-1.1.1/docs/source/trojanvision/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.676247 trojanzoo-1.1.1/docs/source/trojanvision/attacks/
--rw-r--r--   0 root         (0) root         (0)       93 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanvision/attacks/adv.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.676247 trojanzoo-1.1.1/docs/source/trojanvision/attacks/backdoor/
--rw-r--r--   0 root         (0) root         (0)      201 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanvision/attacks/backdoor/clean_label.rst
--rw-r--r--   0 root         (0) root         (0)      158 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanvision/attacks/backdoor/dynamic.rst
--rw-r--r--   0 root         (0) root         (0)      170 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanvision/attacks/backdoor/index.rst
--rw-r--r--   0 root         (0) root         (0)      303 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanvision/attacks/backdoor/normal.rst
--rw-r--r--   0 root         (0) root         (0)      337 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanvision/attacks/index.rst
--rw-r--r--   0 root         (0) root         (0)      136 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanvision/configs.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.676247 trojanzoo-1.1.1/docs/source/trojanvision/datasets/
--rw-r--r--   0 root         (0) root         (0)      317 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanvision/datasets/folder.rst
--rw-r--r--   0 root         (0) root         (0)      275 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanvision/datasets/index.rst
--rw-r--r--   0 root         (0) root         (0)      281 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanvision/datasets/normal.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.676247 trojanzoo-1.1.1/docs/source/trojanvision/defenses/
--rw-r--r--   0 root         (0) root         (0)       83 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanvision/defenses/adv.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.676247 trojanzoo-1.1.1/docs/source/trojanvision/defenses/backdoor/
--rw-r--r--   0 root         (0) root         (0)      334 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanvision/defenses/backdoor/attack_agnostic.rst
--rw-r--r--   0 root         (0) root         (0)      209 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanvision/defenses/backdoor/index.rst
--rw-r--r--   0 root         (0) root         (0)      198 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanvision/defenses/backdoor/input_filtering.rst
--rw-r--r--   0 root         (0) root         (0)      331 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanvision/defenses/backdoor/model_inspection.rst
--rw-r--r--   0 root         (0) root         (0)      242 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanvision/defenses/backdoor/training_filtering.rst
--rw-r--r--   0 root         (0) root         (0)      388 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanvision/defenses/index.rst
--rw-r--r--   0 root         (0) root         (0)      123 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanvision/environ.rst
--rw-r--r--   0 root         (0) root         (0)      206 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanvision/index.rst
--rw-r--r--   0 root         (0) root         (0)      174 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanvision/marks.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.680248 trojanzoo-1.1.1/docs/source/trojanvision/models/
--rw-r--r--   0 root         (0) root         (0)      283 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanvision/models/index.rst
--rw-r--r--   0 root         (0) root         (0)      274 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanvision/models/nas.rst
--rw-r--r--   0 root         (0) root         (0)      129 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanvision/models/others.rst
--rw-r--r--   0 root         (0) root         (0)      407 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanvision/models/torchvision.rst
--rw-r--r--   0 root         (0) root         (0)       77 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanvision/optim.rst
--rw-r--r--   0 root         (0) root         (0)      123 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanvision/trainer.rst
--rw-r--r--   0 root         (0) root         (0)       77 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanvision/utils.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.680248 trojanzoo-1.1.1/docs/source/trojanzoo/
--rw-r--r--   0 root         (0) root         (0)      172 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanzoo/attacks.rst
--rw-r--r--   0 root         (0) root         (0)      127 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanzoo/configs.rst
--rw-r--r--   0 root         (0) root         (0)      177 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanzoo/datasets.rst
--rw-r--r--   0 root         (0) root         (0)      177 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanzoo/defenses.rst
--rw-r--r--   0 root         (0) root         (0)      169 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanzoo/environ.rst
--rw-r--r--   0 root         (0) root         (0)      170 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanzoo/index.rst
--rw-r--r--   0 root         (0) root         (0)      285 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanzoo/models.rst
--rw-r--r--   0 root         (0) root         (0)      110 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanzoo/optim.rst
--rw-r--r--   0 root         (0) root         (0)      173 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanzoo/trainer.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.680248 trojanzoo-1.1.1/docs/source/trojanzoo/utils/
--rw-r--r--   0 root         (0) root         (0)      247 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanzoo/utils/data.rst
--rw-r--r--   0 root         (0) root         (0)      191 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanzoo/utils/fim.rst
--rw-r--r--   0 root         (0) root         (0)      329 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanzoo/utils/index.rst
--rw-r--r--   0 root         (0) root         (0)      213 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanzoo/utils/logger.rst
--rw-r--r--   0 root         (0) root         (0)      369 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanzoo/utils/model.rst
--rw-r--r--   0 root         (0) root         (0)      422 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanzoo/utils/module.rst
--rw-r--r--   0 root         (0) root         (0)      206 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanzoo/utils/tensor.rst
--rw-r--r--   0 root         (0) root         (0)      135 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/trojanzoo/utils/train.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.680248 trojanzoo-1.1.1/docs/source/tutorials/
--rw-r--r--   0 root         (0) root         (0)     1759 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/docs/source/tutorials/basic.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.684248 trojanzoo-1.1.1/examples/
--rw-r--r--   0 root         (0) root         (0)     1116 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/examples/adv_attack.py
--rw-r--r--   0 root         (0) root         (0)     1046 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/examples/adv_defense.py
--rw-r--r--   0 root         (0) root         (0)      955 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/examples/adv_validate.py
--rw-r--r--   0 root         (0) root         (0)     1169 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/examples/backdoor_attack.py
--rw-r--r--   0 root         (0) root         (0)     1345 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/examples/backdoor_defense.py
--rw-r--r--   0 root         (0) root         (0)      930 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/examples/backdoor_validate.py
--rw-r--r--   0 root         (0) root         (0)     1087 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/examples/heatmap.py
--rw-r--r--   0 root         (0) root         (0)      428 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/examples/test.py
--rw-r--r--   0 root         (0) root         (0)     1728 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/examples/train.py
--rw-r--r--   0 root         (0) root         (0)      749 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/examples/validate.py
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       99 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     1350 2022-07-13 23:33:13.712250 trojanzoo-1.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       93 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.684248 trojanzoo-1.1.1/trojanvision/
--rw-r--r--   0 root         (0) root         (0)      419 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.684248 trojanzoo-1.1.1/trojanvision/attacks/
--rw-r--r--   0 root         (0) root         (0)     3584 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/attacks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18671 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/attacks/abstract.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.684248 trojanzoo-1.1.1/trojanvision/attacks/adv/
--rw-r--r--   0 root         (0) root         (0)      161 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/attacks/adv/__init__.py
--rw-r--r--   0 root         (0) root         (0)       66 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/attacks/adv/pgd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.684248 trojanzoo-1.1.1/trojanvision/attacks/backdoor/
--rw-r--r--   0 root         (0) root         (0)      428 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/attacks/backdoor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.684248 trojanzoo-1.1.1/trojanvision/attacks/backdoor/clean_label/
--rw-r--r--   0 root         (0) root         (0)      382 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/attacks/backdoor/clean_label/__init__.py
--rw-r--r--   0 root         (0) root         (0)      748 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/attacks/backdoor/clean_label/clean_label.py
--rw-r--r--   0 root         (0) root         (0)    11700 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/attacks/backdoor/clean_label/invisible_poison.py
--rw-r--r--   0 root         (0) root         (0)    16863 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/attacks/backdoor/clean_label/label_consistent.py
--rw-r--r--   0 root         (0) root         (0)    26356 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/attacks/backdoor/clean_label/refool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.684248 trojanzoo-1.1.1/trojanvision/attacks/backdoor/dynamic/
--rw-r--r--   0 root         (0) root         (0)      248 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/attacks/backdoor/dynamic/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28578 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/attacks/backdoor/dynamic/input_aware_dynamic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.684248 trojanzoo-1.1.1/trojanvision/attacks/backdoor/normal/
--rw-r--r--   0 root         (0) root         (0)      474 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/attacks/backdoor/normal/__init__.py
--rw-r--r--   0 root         (0) root         (0)      734 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/attacks/backdoor/normal/badnet.py
--rw-r--r--   0 root         (0) root         (0)     3431 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/attacks/backdoor/normal/imc.py
--rw-r--r--   0 root         (0) root         (0)    10777 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/attacks/backdoor/normal/latent_backdoor.py
--rw-r--r--   0 root         (0) root         (0)    15353 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/attacks/backdoor/normal/trojannet.py
--rw-r--r--   0 root         (0) root         (0)    11063 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/attacks/backdoor/normal/trojannn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.684248 trojanzoo-1.1.1/trojanvision/attacks/backdoor/others/
--rw-r--r--   0 root         (0) root         (0)      192 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/attacks/backdoor/others/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1430 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/attacks/backdoor/others/unlearn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.688248 trojanzoo-1.1.1/trojanvision/attacks/poison/
--rw-r--r--   0 root         (0) root         (0)      373 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/attacks/poison/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8438 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/attacks/poison/imc_poison.py
--rw-r--r--   0 root         (0) root         (0)     7186 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/attacks/poison/poison_basic.py
--rw-r--r--   0 root         (0) root         (0)     4085 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/attacks/poison/poison_random.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.688248 trojanzoo-1.1.1/trojanvision/configs/
--rw-r--r--   0 root         (0) root         (0)     1057 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/configs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.688248 trojanzoo-1.1.1/trojanvision/configs/attack/
--rw-r--r--   0 root         (0) root         (0)       30 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/configs/attack/bypass_embed.yml
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/configs/attack/clean_label.yml
--rw-r--r--   0 root         (0) root         (0)       75 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/configs/attack/hidden_trigger.yml
--rw-r--r--   0 root         (0) root         (0)       21 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/configs/attack/pgd.yml
--rw-r--r--   0 root         (0) root         (0)       69 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/configs/attack/reflection_backdoor.yml
--rw-r--r--   0 root         (0) root         (0)      192 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/configs/dataset.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.688248 trojanzoo-1.1.1/trojanvision/configs/defense/
--rw-r--r--   0 root         (0) root         (0)       81 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/configs/defense/abs.yml
--rw-r--r--   0 root         (0) root         (0)      159 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/configs/defense/activation_clustering.yml
--rw-r--r--   0 root         (0) root         (0)       63 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/configs/defense/advmind.yml
--rw-r--r--   0 root         (0) root         (0)       18 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/configs/defense/fine_pruning.yml
--rw-r--r--   0 root         (0) root         (0)       46 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/configs/defense/image_transform.yml
--rw-r--r--   0 root         (0) root         (0)       49 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/configs/defense/neo.yml
--rw-r--r--   0 root         (0) root         (0)       75 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/configs/defense/neuron_inspect.yml
--rw-r--r--   0 root         (0) root         (0)      103 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/configs/defense/spectral_signature.yml
--rw-r--r--   0 root         (0) root         (0)      261 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/configs/model.yml
--rw-r--r--   0 root         (0) root         (0)      369 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/configs/trainer.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.668247 trojanzoo-1.1.1/trojanvision/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.688248 trojanzoo-1.1.1/trojanvision/data/cub200/
--rw-r--r--   0 root         (0) root         (0)   174592 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/data/cub200/test.txt
--rw-r--r--   0 root         (0) root         (0)   168954 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/data/cub200/train.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.688248 trojanzoo-1.1.1/trojanvision/data/cub200_2011/
--rw-r--r--   0 root         (0) root         (0)   100487 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/data/cub200_2011/image_class_labels.txt
--rw-r--r--   0 root         (0) root         (0)    83198 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/data/cub200_2011/train_test_split.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.692249 trojanzoo-1.1.1/trojanvision/data/isic2018/
--rw-r--r--   0 root         (0) root         (0)   410650 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/data/isic2018/train.csv
--rw-r--r--   0 root         (0) root         (0)     7948 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/data/isic2018/valid.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.692249 trojanzoo-1.1.1/trojanvision/data/refool/
--rw-r--r--   0 root         (0) root         (0)     8674 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/data/refool/insert_reflection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.692249 trojanzoo-1.1.1/trojanvision/data/sample_imagenet/
--rw-r--r--   0 root         (0) root         (0)      417 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/data/sample_imagenet/class_dict.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.692249 trojanzoo-1.1.1/trojanvision/datasets/
--rw-r--r--   0 root         (0) root         (0)     2911 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/datasets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.692249 trojanzoo-1.1.1/trojanvision/datasets/folder/
--rw-r--r--   0 root         (0) root         (0)      679 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/datasets/folder/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5558 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/datasets/folder/cub200.py
--rw-r--r--   0 root         (0) root         (0)     2021 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/datasets/folder/gtsrb.py
--rw-r--r--   0 root         (0) root         (0)     4384 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/datasets/folder/imagenet.py
--rw-r--r--   0 root         (0) root         (0)     2960 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/datasets/folder/isic.py
--rw-r--r--   0 root         (0) root         (0)     1658 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/datasets/folder/vggface2.py
--rw-r--r--   0 root         (0) root         (0)    14880 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/datasets/imagefolder.py
--rw-r--r--   0 root         (0) root         (0)    10846 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/datasets/imageset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.692249 trojanzoo-1.1.1/trojanvision/datasets/normal/
--rw-r--r--   0 root         (0) root         (0)      438 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/datasets/normal/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3163 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/datasets/normal/cifar.py
--rw-r--r--   0 root         (0) root         (0)     3314 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/datasets/normal/downsampled_imagenet.py
--rw-r--r--   0 root         (0) root         (0)     1367 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/datasets/normal/mnist.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.692249 trojanzoo-1.1.1/trojanvision/defenses/
--rw-r--r--   0 root         (0) root         (0)     1560 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/defenses/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23206 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/defenses/abstract.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.692249 trojanzoo-1.1.1/trojanvision/defenses/adv/
--rw-r--r--   0 root         (0) root         (0)      334 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/defenses/adv/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17940 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/defenses/adv/advmind.py
--rw-r--r--   0 root         (0) root         (0)     1451 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/defenses/adv/curvature.py
--rw-r--r--   0 root         (0) root         (0)     2603 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/defenses/adv/grad_train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.692249 trojanzoo-1.1.1/trojanvision/defenses/backdoor/
--rw-r--r--   0 root         (0) root         (0)      532 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/defenses/backdoor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.696249 trojanzoo-1.1.1/trojanvision/defenses/backdoor/attack_agnostic/
--rw-r--r--   0 root         (0) root         (0)      534 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/defenses/backdoor/attack_agnostic/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5981 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/defenses/backdoor/attack_agnostic/adv_train.py
--rw-r--r--   0 root         (0) root         (0)     4215 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/defenses/backdoor/attack_agnostic/fine_pruning.py
--rw-r--r--   0 root         (0) root         (0)     1397 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/defenses/backdoor/attack_agnostic/magnet.py
--rw-r--r--   0 root         (0) root         (0)      287 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/defenses/backdoor/attack_agnostic/randomized_smooth.py
--rw-r--r--   0 root         (0) root         (0)     1827 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/defenses/backdoor/attack_agnostic/recompress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.696249 trojanzoo-1.1.1/trojanvision/defenses/backdoor/input_filtering/
--rw-r--r--   0 root         (0) root         (0)      224 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/defenses/backdoor/input_filtering/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7720 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/defenses/backdoor/input_filtering/neo.py
--rw-r--r--   0 root         (0) root         (0)     3610 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/defenses/backdoor/input_filtering/strip.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.696249 trojanzoo-1.1.1/trojanvision/defenses/backdoor/model_inspection/
--rw-r--r--   0 root         (0) root         (0)      504 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/defenses/backdoor/model_inspection/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14370 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/defenses/backdoor/model_inspection/abs.py
--rw-r--r--   0 root         (0) root         (0)     6652 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/defenses/backdoor/model_inspection/deep_inspect.py
--rw-r--r--   0 root         (0) root         (0)     5908 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/defenses/backdoor/model_inspection/neural_cleanse.py
--rw-r--r--   0 root         (0) root         (0)     4596 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/defenses/backdoor/model_inspection/neuron_inspect.py
--rw-r--r--   0 root         (0) root         (0)     4018 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/defenses/backdoor/model_inspection/tabor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.696249 trojanzoo-1.1.1/trojanvision/defenses/backdoor/training_filtering/
--rw-r--r--   0 root         (0) root         (0)      387 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/defenses/backdoor/training_filtering/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10901 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/defenses/backdoor/training_filtering/activation_clustering.py
--rw-r--r--   0 root         (0) root         (0)     7870 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/defenses/backdoor/training_filtering/spectral_signature.py
--rw-r--r--   0 root         (0) root         (0)      581 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/environ.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.696249 trojanzoo-1.1.1/trojanvision/marks/
--rw-r--r--   0 root         (0) root         (0)    22252 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/marks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3602 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/marks/apple_black.png
--rw-r--r--   0 root         (0) root         (0)     3595 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/marks/apple_white.png
--rw-r--r--   0 root         (0) root         (0)      756 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/marks/square_black.png
--rw-r--r--   0 root         (0) root         (0)      675 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/marks/square_white.png
--rw-r--r--   0 root         (0) root         (0)     9850 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/marks/tag_black.png
--rw-r--r--   0 root         (0) root         (0)     9823 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/marks/tag_white.png
--rw-r--r--   0 root         (0) root         (0)    26522 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/marks/watermark_black.png
--rw-r--r--   0 root         (0) root         (0)    26281 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/marks/watermark_white.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.700249 trojanzoo-1.1.1/trojanvision/models/
--rw-r--r--   0 root         (0) root         (0)     4129 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30597 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/models/imagemodel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.700249 trojanzoo-1.1.1/trojanvision/models/nas/
--rw-r--r--   0 root         (0) root         (0)      524 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/models/nas/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20990 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/models/nas/darts.py
--rw-r--r--   0 root         (0) root         (0)     2708 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/models/nas/enas.py
--rw-r--r--   0 root         (0) root         (0)     3717 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/models/nas/lanet.py
--rw-r--r--   0 root         (0) root         (0)     6056 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/models/nas/natsbench.py
--rw-r--r--   0 root         (0) root         (0)     2178 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/models/nas/pnasnet.py
--rw-r--r--   0 root         (0) root         (0)     3494 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/models/nas/proxylessnas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.700249 trojanzoo-1.1.1/trojanvision/models/normal/
--rw-r--r--   0 root         (0) root         (0)      314 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/models/normal/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9448 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/models/normal/bit.py
--rw-r--r--   0 root         (0) root         (0)     3872 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/models/normal/dla.py
--rw-r--r--   0 root         (0) root         (0)     1955 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/models/normal/dpn.py
--rw-r--r--   0 root         (0) root         (0)     1065 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/models/normal/net.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.700249 trojanzoo-1.1.1/trojanvision/models/others/
--rw-r--r--   0 root         (0) root         (0)      196 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/models/others/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7219 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/models/others/magnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.700249 trojanzoo-1.1.1/trojanvision/models/torchvision/
--rw-r--r--   0 root         (0) root         (0)      724 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/models/torchvision/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2405 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/models/torchvision/alexnet.py
--rw-r--r--   0 root         (0) root         (0)     3365 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/models/torchvision/densenet.py
--rw-r--r--   0 root         (0) root         (0)     3147 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/models/torchvision/efficientnet.py
--rw-r--r--   0 root         (0) root         (0)     2873 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/models/torchvision/mnasnet.py
--rw-r--r--   0 root         (0) root         (0)     3525 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/models/torchvision/mobilenet.py
--rw-r--r--   0 root         (0) root         (0)     7460 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/models/torchvision/resnet.py
--rw-r--r--   0 root         (0) root         (0)     3884 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/models/torchvision/shufflenetv2.py
--rw-r--r--   0 root         (0) root         (0)     3270 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/models/torchvision/vgg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.700249 trojanzoo-1.1.1/trojanvision/optim/
--rw-r--r--   0 root         (0) root         (0)      110 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/optim/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13957 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/optim/pgd.py
--rw-r--r--   0 root         (0) root         (0)     4847 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/optim/uname.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.704249 trojanzoo-1.1.1/trojanvision/shortcut/
--rw-r--r--   0 root         (0) root         (0)       58 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/shortcut/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12411 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/shortcut/pgd.py
--rw-r--r--   0 root         (0) root         (0)     1141 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.704249 trojanzoo-1.1.1/trojanvision/utils/
--rw-r--r--   0 root         (0) root         (0)     2641 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.704249 trojanzoo-1.1.1/trojanvision/utils/autoaugment/
--rw-r--r--   0 root         (0) root         (0)      164 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/autoaugment/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60569 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/autoaugment/functional.py
--rw-r--r--   0 root         (0) root         (0)    12720 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/autoaugment/functional_pil.py
--rw-r--r--   0 root         (0) root         (0)    35805 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/autoaugment/functional_tensor.py
--rw-r--r--   0 root         (0) root         (0)    10101 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/autoaugment/operations.py
--rw-r--r--   0 root         (0) root         (0)     2804 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/autoaugment/policy.py
--rw-r--r--   0 root         (0) root         (0)     3584 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/autoaugment/wgan.py
--rw-r--r--   0 root         (0) root         (0)     9276 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.704249 trojanzoo-1.1.1/trojanvision/utils/datasets/
--rw-r--r--   0 root         (0) root         (0)      102 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5233 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/datasets/downsampled_imagenet.py
--rw-r--r--   0 root         (0) root         (0)     2202 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.704249 trojanzoo-1.1.1/trojanvision/utils/model_archs/
--rw-r--r--   0 root         (0) root         (0)      885 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/model_archs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8509 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/model_archs/bit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.708250 trojanzoo-1.1.1/trojanvision/utils/model_archs/darts/
--rw-r--r--   0 root         (0) root         (0)      131 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/model_archs/darts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4593 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/model_archs/darts/features.py
--rw-r--r--   0 root         (0) root         (0)    10884 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/model_archs/darts/genotypes.py
--rw-r--r--   0 root         (0) root         (0)     5945 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/model_archs/darts/operations.py
--rw-r--r--   0 root         (0) root         (0)     6067 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/model_archs/darts/search.py
--rw-r--r--   0 root         (0) root         (0)    11910 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/model_archs/darts/sgas.py
--rw-r--r--   0 root         (0) root         (0)    10085 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/model_archs/dla.py
--rw-r--r--   0 root         (0) root         (0)     8661 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/model_archs/dpn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.708250 trojanzoo-1.1.1/trojanvision/utils/model_archs/enas/
--rw-r--r--   0 root         (0) root         (0)      130 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/model_archs/enas/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3333 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/model_archs/enas/macro.py
--rw-r--r--   0 root         (0) root         (0)    14037 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/model_archs/enas/mutables.py
--rw-r--r--   0 root         (0) root         (0)     3400 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/model_archs/enas/ops.py
--rw-r--r--   0 root         (0) root         (0)     1549 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/model_archs/lanet.py
--rw-r--r--   0 root         (0) root         (0)     4285 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/model_archs/pnasnet.py
--rw-r--r--   0 root         (0) root         (0)     5806 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/model_archs/resnet_ap.py
--rw-r--r--   0 root         (0) root         (0)     1933 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/model_archs/resnet_s.py
--rw-r--r--   0 root         (0) root         (0)     2761 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/sgm.py
--rw-r--r--   0 root         (0) root         (0)    11211 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanvision/utils/transform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.708250 trojanzoo-1.1.1/trojanzoo/
--rw-r--r--   0 root         (0) root         (0)      399 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6739 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/attacks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.712250 trojanzoo-1.1.1/trojanzoo/configs/
--rw-r--r--   0 root         (0) root         (0)    10406 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/configs/__init__.py
--rw-r--r--   0 root         (0) root         (0)       27 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/configs/attack.yml
--rw-r--r--   0 root         (0) root         (0)      125 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/configs/dataset.yml
--rw-r--r--   0 root         (0) root         (0)       29 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/configs/defense.yml
--rw-r--r--   0 root         (0) root         (0)       40 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/configs/env.yml
--rw-r--r--   0 root         (0) root         (0)       48 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/configs/model.yml
--rw-r--r--   0 root         (0) root         (0)      146 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/configs/trainer.yml
--rw-r--r--   0 root         (0) root         (0)    22163 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/datasets.py
--rw-r--r--   0 root         (0) root         (0)     6064 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/defenses.py
--rw-r--r--   0 root         (0) root         (0)     7282 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/environ.py
--rw-r--r--   0 root         (0) root         (0)    65930 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/models.py
--rw-r--r--   0 root         (0) root         (0)    10800 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/optim.py
--rw-r--r--   0 root         (0) root         (0)    14367 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.712250 trojanzoo-1.1.1/trojanzoo/utils/
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7815 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/utils/data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.712250 trojanzoo-1.1.1/trojanzoo/utils/fim/
--rw-r--r--   0 root         (0) root         (0)      148 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/utils/fim/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12525 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/utils/fim/ekfac.py
--rw-r--r--   0 root         (0) root         (0)     3899 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/utils/fim/fim.py
--rw-r--r--   0 root         (0) root         (0)    15646 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/utils/fim/kfac.py
--rw-r--r--   0 root         (0) root         (0)     1491 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/utils/lock.py
--rw-r--r--   0 root         (0) root         (0)    14445 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/utils/logger.py
--rw-r--r--   0 root         (0) root         (0)     2258 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/utils/memory.py
--rw-r--r--   0 root         (0) root         (0)     1504 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/utils/metric.py
--rw-r--r--   0 root         (0) root         (0)    25201 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/utils/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.712250 trojanzoo-1.1.1/trojanzoo/utils/module/
--rw-r--r--   0 root         (0) root         (0)     1093 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/utils/module/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6231 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/utils/module/param.py
--rw-r--r--   0 root         (0) root         (0)     6545 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/utils/module/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.712250 trojanzoo-1.1.1/trojanzoo/utils/ntk/
--rw-r--r--   0 root         (0) root         (0)     1920 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/utils/ntk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3795 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/utils/output.py
--rw-r--r--   0 root         (0) root         (0)     3120 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/utils/tensor.py
--rw-r--r--   0 root         (0) root         (0)    13798 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/utils/train.py
--rw-r--r--   0 root         (0) root         (0)       46 2022-07-13 23:33:04.000000 trojanzoo-1.1.1/trojanzoo/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 23:33:13.708250 trojanzoo-1.1.1/trojanzoo.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9619 2022-07-13 23:33:13.000000 trojanzoo-1.1.1/trojanzoo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10823 2022-07-13 23:33:13.000000 trojanzoo-1.1.1/trojanzoo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-13 23:33:13.000000 trojanzoo-1.1.1/trojanzoo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-13 23:33:13.000000 trojanzoo-1.1.1/trojanzoo.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      158 2022-07-13 23:33:13.000000 trojanzoo-1.1.1/trojanzoo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-13 23:33:13.000000 trojanzoo-1.1.1/trojanzoo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.860679 trojanzoo-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      316 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9623 2023-05-14 09:58:21.860679 trojanzoo-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8712 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.820679 trojanzoo-2.0.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      855 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)      165 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.820679 trojanzoo-2.0.0/docs/source/
+-rw-r--r--   0 root         (0) root         (0)     4002 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.820679 trojanzoo-2.0.0/docs/source/images/
+-rw-r--r--   0 root         (0) root         (0)     4286 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/images/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.820679 trojanzoo-2.0.0/docs/source/images/logo/
+-rw-r--r--   0 root         (0) root         (0)     8520 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/images/logo/trojanzoo-logo-dark.svg
+-rw-r--r--   0 root         (0) root         (0)     5671 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/images/logo/trojanzoo-logo-icon.svg
+-rw-r--r--   0 root         (0) root         (0)     7587 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/images/logo/trojanzoo-logo.svg
+-rw-r--r--   0 root         (0) root         (0)   570067 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/images/screenshot.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.824679 trojanzoo-2.0.0/docs/source/images/trojanvision/
+-rw-r--r--   0 root         (0) root         (0)    83160 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/images/trojanvision/center_cropped.png
+-rw-r--r--   0 root         (0) root         (0)    16840 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/images/trojanvision/grad_cam.png
+-rw-r--r--   0 root         (0) root         (0)    79679 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/images/trojanvision/grad_cam_impose.png
+-rw-r--r--   0 root         (0) root         (0)    51879 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/images/trojanvision/saliency_map.png
+-rw-r--r--   0 root         (0) root         (0)    92604 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/images/trojanvision/saliency_map_impose.png
+-rw-r--r--   0 root         (0) root         (0)    68027 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/images/trojanzoo-logo-readme.svg
+-rw-r--r--   0 root         (0) root         (0)      507 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.824679 trojanzoo-2.0.0/docs/source/trojanvision/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.824679 trojanzoo-2.0.0/docs/source/trojanvision/attacks/
+-rw-r--r--   0 root         (0) root         (0)       93 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/attacks/adv.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.824679 trojanzoo-2.0.0/docs/source/trojanvision/attacks/backdoor/
+-rw-r--r--   0 root         (0) root         (0)      201 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/attacks/backdoor/clean_label.rst
+-rw-r--r--   0 root         (0) root         (0)      158 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/attacks/backdoor/dynamic.rst
+-rw-r--r--   0 root         (0) root         (0)      170 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/attacks/backdoor/index.rst
+-rw-r--r--   0 root         (0) root         (0)      303 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/attacks/backdoor/normal.rst
+-rw-r--r--   0 root         (0) root         (0)      337 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/attacks/index.rst
+-rw-r--r--   0 root         (0) root         (0)      136 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/configs.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.824679 trojanzoo-2.0.0/docs/source/trojanvision/datasets/
+-rw-r--r--   0 root         (0) root         (0)      317 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/datasets/folder.rst
+-rw-r--r--   0 root         (0) root         (0)      275 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/datasets/index.rst
+-rw-r--r--   0 root         (0) root         (0)      316 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/datasets/normal.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.824679 trojanzoo-2.0.0/docs/source/trojanvision/defenses/
+-rw-r--r--   0 root         (0) root         (0)       83 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/defenses/adv.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.828679 trojanzoo-2.0.0/docs/source/trojanvision/defenses/backdoor/
+-rw-r--r--   0 root         (0) root         (0)      334 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/defenses/backdoor/attack_agnostic.rst
+-rw-r--r--   0 root         (0) root         (0)      209 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/defenses/backdoor/index.rst
+-rw-r--r--   0 root         (0) root         (0)      198 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/defenses/backdoor/input_filtering.rst
+-rw-r--r--   0 root         (0) root         (0)      331 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/defenses/backdoor/model_inspection.rst
+-rw-r--r--   0 root         (0) root         (0)      242 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/defenses/backdoor/training_filtering.rst
+-rw-r--r--   0 root         (0) root         (0)      388 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/defenses/index.rst
+-rw-r--r--   0 root         (0) root         (0)      123 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/environ.rst
+-rw-r--r--   0 root         (0) root         (0)      206 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/index.rst
+-rw-r--r--   0 root         (0) root         (0)      174 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/marks.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.828679 trojanzoo-2.0.0/docs/source/trojanvision/models/
+-rw-r--r--   0 root         (0) root         (0)      283 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/models/index.rst
+-rw-r--r--   0 root         (0) root         (0)      274 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/models/nas.rst
+-rw-r--r--   0 root         (0) root         (0)      129 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/models/others.rst
+-rw-r--r--   0 root         (0) root         (0)      407 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/models/torchvision.rst
+-rw-r--r--   0 root         (0) root         (0)       77 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/optim.rst
+-rw-r--r--   0 root         (0) root         (0)      123 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/trainer.rst
+-rw-r--r--   0 root         (0) root         (0)       77 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanvision/utils.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.828679 trojanzoo-2.0.0/docs/source/trojanzoo/
+-rw-r--r--   0 root         (0) root         (0)      172 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/attacks.rst
+-rw-r--r--   0 root         (0) root         (0)      127 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/configs.rst
+-rw-r--r--   0 root         (0) root         (0)      177 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/datasets.rst
+-rw-r--r--   0 root         (0) root         (0)      177 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/defenses.rst
+-rw-r--r--   0 root         (0) root         (0)      169 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/environ.rst
+-rw-r--r--   0 root         (0) root         (0)      170 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/index.rst
+-rw-r--r--   0 root         (0) root         (0)      285 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/models.rst
+-rw-r--r--   0 root         (0) root         (0)      110 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/optim.rst
+-rw-r--r--   0 root         (0) root         (0)      173 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/trainer.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.828679 trojanzoo-2.0.0/docs/source/trojanzoo/utils/
+-rw-r--r--   0 root         (0) root         (0)      247 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/utils/data.rst
+-rw-r--r--   0 root         (0) root         (0)      191 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/utils/fim.rst
+-rw-r--r--   0 root         (0) root         (0)      329 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/utils/index.rst
+-rw-r--r--   0 root         (0) root         (0)      213 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/utils/logger.rst
+-rw-r--r--   0 root         (0) root         (0)      369 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/utils/model.rst
+-rw-r--r--   0 root         (0) root         (0)      422 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/utils/module.rst
+-rw-r--r--   0 root         (0) root         (0)      206 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/utils/tensor.rst
+-rw-r--r--   0 root         (0) root         (0)      135 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/trojanzoo/utils/train.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.828679 trojanzoo-2.0.0/docs/source/tutorials/
+-rw-r--r--   0 root         (0) root         (0)     1759 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/docs/source/tutorials/basic.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.832679 trojanzoo-2.0.0/examples/
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/examples/adv_attack.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/examples/adv_defense.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/examples/adv_validate.py
+-rw-r--r--   0 root         (0) root         (0)     1252 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/examples/backdoor_attack.py
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/examples/backdoor_defense.py
+-rw-r--r--   0 root         (0) root         (0)      944 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/examples/backdoor_validate.py
+-rw-r--r--   0 root         (0) root         (0)     1013 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/examples/heatmap.py
+-rw-r--r--   0 root         (0) root         (0)      428 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/examples/test.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/examples/train.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/examples/validate.py
+-rw-r--r--   0 root         (0) root         (0)      106 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       98 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-05-14 09:58:21.860679 trojanzoo-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       93 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.832679 trojanzoo-2.0.0/trojanvision/
+-rw-r--r--   0 root         (0) root         (0)      419 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.832679 trojanzoo-2.0.0/trojanvision/attacks/
+-rw-r--r--   0 root         (0) root         (0)     3584 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18456 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/abstract.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.832679 trojanzoo-2.0.0/trojanvision/attacks/adv/
+-rw-r--r--   0 root         (0) root         (0)      161 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/adv/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       66 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/adv/pgd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.832679 trojanzoo-2.0.0/trojanvision/attacks/backdoor/
+-rw-r--r--   0 root         (0) root         (0)      428 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.832679 trojanzoo-2.0.0/trojanvision/attacks/backdoor/clean_label/
+-rw-r--r--   0 root         (0) root         (0)      382 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/clean_label/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      748 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/clean_label/clean_label.py
+-rw-r--r--   0 root         (0) root         (0)    11700 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/clean_label/invisible_poison.py
+-rw-r--r--   0 root         (0) root         (0)    16740 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/clean_label/label_consistent.py
+-rw-r--r--   0 root         (0) root         (0)    26368 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/clean_label/refool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.832679 trojanzoo-2.0.0/trojanvision/attacks/backdoor/dynamic/
+-rw-r--r--   0 root         (0) root         (0)      248 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/dynamic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30304 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/dynamic/input_aware_dynamic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.832679 trojanzoo-2.0.0/trojanvision/attacks/backdoor/normal/
+-rw-r--r--   0 root         (0) root         (0)      474 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/normal/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      734 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/normal/badnet.py
+-rw-r--r--   0 root         (0) root         (0)     3431 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/normal/imc.py
+-rw-r--r--   0 root         (0) root         (0)    10777 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/normal/latent_backdoor.py
+-rw-r--r--   0 root         (0) root         (0)    15353 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/normal/trojannet.py
+-rw-r--r--   0 root         (0) root         (0)    11063 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/normal/trojannn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.836679 trojanzoo-2.0.0/trojanvision/attacks/backdoor/others/
+-rw-r--r--   0 root         (0) root         (0)      192 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/others/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/backdoor/others/unlearn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.836679 trojanzoo-2.0.0/trojanvision/attacks/poison/
+-rw-r--r--   0 root         (0) root         (0)      373 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/poison/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8430 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/poison/imc_poison.py
+-rw-r--r--   0 root         (0) root         (0)     7186 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/poison/poison_basic.py
+-rw-r--r--   0 root         (0) root         (0)     4085 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/attacks/poison/poison_random.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.836679 trojanzoo-2.0.0/trojanvision/configs/
+-rw-r--r--   0 root         (0) root         (0)     1057 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.836679 trojanzoo-2.0.0/trojanvision/configs/attack/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/attack/bypass_embed.yml
+-rw-r--r--   0 root         (0) root         (0)       91 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/attack/clean_label.yml
+-rw-r--r--   0 root         (0) root         (0)       75 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/attack/hidden_trigger.yml
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/attack/pgd.yml
+-rw-r--r--   0 root         (0) root         (0)       69 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/attack/reflection_backdoor.yml
+-rw-r--r--   0 root         (0) root         (0)      192 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/dataset.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.836679 trojanzoo-2.0.0/trojanvision/configs/defense/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/defense/abs.yml
+-rw-r--r--   0 root         (0) root         (0)      159 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/defense/activation_clustering.yml
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/defense/advmind.yml
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/defense/fine_pruning.yml
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/defense/image_transform.yml
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/defense/neo.yml
+-rw-r--r--   0 root         (0) root         (0)       75 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/defense/neuron_inspect.yml
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/defense/spectral_signature.yml
+-rw-r--r--   0 root         (0) root         (0)      261 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/model.yml
+-rw-r--r--   0 root         (0) root         (0)      369 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/configs/trainer.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.816679 trojanzoo-2.0.0/trojanvision/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.836679 trojanzoo-2.0.0/trojanvision/data/cub200/
+-rw-r--r--   0 root         (0) root         (0)   174592 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/data/cub200/test.txt
+-rw-r--r--   0 root         (0) root         (0)   168954 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/data/cub200/train.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.840679 trojanzoo-2.0.0/trojanvision/data/cub200_2011/
+-rw-r--r--   0 root         (0) root         (0)   682287 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/data/cub200_2011/images.txt
+-rw-r--r--   0 root         (0) root         (0)    83198 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/data/cub200_2011/train_test_split.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.840679 trojanzoo-2.0.0/trojanvision/data/isic2018/
+-rw-r--r--   0 root         (0) root         (0)   410650 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/data/isic2018/train.csv
+-rw-r--r--   0 root         (0) root         (0)     7948 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/data/isic2018/valid.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.840679 trojanzoo-2.0.0/trojanvision/data/refool/
+-rw-r--r--   0 root         (0) root         (0)     8680 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/data/refool/insert_reflection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.840679 trojanzoo-2.0.0/trojanvision/data/sample_imagenet/
+-rw-r--r--   0 root         (0) root         (0)      417 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/data/sample_imagenet/class_dict.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.840679 trojanzoo-2.0.0/trojanvision/data/stl10/
+-rw-r--r--   0 root         (0) root         (0)   100000 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/data/stl10/unlabeled_y.bin
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.840679 trojanzoo-2.0.0/trojanvision/datasets/
+-rw-r--r--   0 root         (0) root         (0)     2911 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.840679 trojanzoo-2.0.0/trojanvision/datasets/folder/
+-rw-r--r--   0 root         (0) root         (0)      679 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/folder/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5558 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/folder/cub200.py
+-rw-r--r--   0 root         (0) root         (0)     2021 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/folder/gtsrb.py
+-rw-r--r--   0 root         (0) root         (0)     4814 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/folder/imagenet.py
+-rw-r--r--   0 root         (0) root         (0)     2960 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/folder/isic.py
+-rw-r--r--   0 root         (0) root         (0)     1655 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/folder/vggface2.py
+-rw-r--r--   0 root         (0) root         (0)    14991 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/imagefolder.py
+-rw-r--r--   0 root         (0) root         (0)    10615 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/imageset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.840679 trojanzoo-2.0.0/trojanvision/datasets/normal/
+-rw-r--r--   0 root         (0) root         (0)      592 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/normal/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1262 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/normal/celeba.py
+-rw-r--r--   0 root         (0) root         (0)     3163 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/normal/cifar.py
+-rw-r--r--   0 root         (0) root         (0)     4314 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/normal/downsampled_imagenet.py
+-rw-r--r--   0 root         (0) root         (0)     1367 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/normal/mnist.py
+-rw-r--r--   0 root         (0) root         (0)     4725 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/datasets/normal/stl10.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.840679 trojanzoo-2.0.0/trojanvision/defenses/
+-rw-r--r--   0 root         (0) root         (0)     1560 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23436 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/abstract.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.844679 trojanzoo-2.0.0/trojanvision/defenses/adv/
+-rw-r--r--   0 root         (0) root         (0)      334 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/adv/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17940 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/adv/advmind.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/adv/curvature.py
+-rw-r--r--   0 root         (0) root         (0)     2603 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/adv/grad_train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.844679 trojanzoo-2.0.0/trojanvision/defenses/backdoor/
+-rw-r--r--   0 root         (0) root         (0)      532 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.844679 trojanzoo-2.0.0/trojanvision/defenses/backdoor/attack_agnostic/
+-rw-r--r--   0 root         (0) root         (0)      534 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/attack_agnostic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5981 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/attack_agnostic/adv_train.py
+-rw-r--r--   0 root         (0) root         (0)     4215 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/attack_agnostic/fine_pruning.py
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/attack_agnostic/magnet.py
+-rw-r--r--   0 root         (0) root         (0)      287 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/attack_agnostic/randomized_smooth.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/attack_agnostic/recompress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.844679 trojanzoo-2.0.0/trojanvision/defenses/backdoor/input_filtering/
+-rw-r--r--   0 root         (0) root         (0)      224 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/input_filtering/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7720 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/input_filtering/neo.py
+-rw-r--r--   0 root         (0) root         (0)     3610 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/input_filtering/strip.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.844679 trojanzoo-2.0.0/trojanvision/defenses/backdoor/model_inspection/
+-rw-r--r--   0 root         (0) root         (0)      504 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/model_inspection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14370 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/model_inspection/abs.py
+-rw-r--r--   0 root         (0) root         (0)     6652 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/model_inspection/deep_inspect.py
+-rw-r--r--   0 root         (0) root         (0)     5908 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/model_inspection/neural_cleanse.py
+-rw-r--r--   0 root         (0) root         (0)     4596 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/model_inspection/neuron_inspect.py
+-rw-r--r--   0 root         (0) root         (0)     4018 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/model_inspection/tabor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.844679 trojanzoo-2.0.0/trojanvision/defenses/backdoor/training_filtering/
+-rw-r--r--   0 root         (0) root         (0)      387 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/training_filtering/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10901 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/training_filtering/activation_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     7870 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/defenses/backdoor/training_filtering/spectral_signature.py
+-rw-r--r--   0 root         (0) root         (0)      567 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/environ.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.848679 trojanzoo-2.0.0/trojanvision/marks/
+-rw-r--r--   0 root         (0) root         (0)    22268 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/marks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3602 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/marks/apple_black.png
+-rw-r--r--   0 root         (0) root         (0)     3595 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/marks/apple_white.png
+-rw-r--r--   0 root         (0) root         (0)      756 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/marks/square_black.png
+-rw-r--r--   0 root         (0) root         (0)      675 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/marks/square_white.png
+-rw-r--r--   0 root         (0) root         (0)     9850 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/marks/tag_black.png
+-rw-r--r--   0 root         (0) root         (0)     9823 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/marks/tag_white.png
+-rw-r--r--   0 root         (0) root         (0)    26522 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/marks/watermark_black.png
+-rw-r--r--   0 root         (0) root         (0)    26281 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/marks/watermark_white.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.848679 trojanzoo-2.0.0/trojanvision/models/
+-rw-r--r--   0 root         (0) root         (0)     4128 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29817 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/imagemodel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.848679 trojanzoo-2.0.0/trojanvision/models/nas/
+-rw-r--r--   0 root         (0) root         (0)      524 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/nas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20990 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/nas/darts.py
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/nas/enas.py
+-rw-r--r--   0 root         (0) root         (0)     3726 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/nas/lanet.py
+-rw-r--r--   0 root         (0) root         (0)     8069 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/nas/natsbench.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/nas/pnasnet.py
+-rw-r--r--   0 root         (0) root         (0)     3494 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/nas/proxylessnas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.848679 trojanzoo-2.0.0/trojanvision/models/normal/
+-rw-r--r--   0 root         (0) root         (0)      314 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/normal/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9448 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/normal/bit.py
+-rw-r--r--   0 root         (0) root         (0)     3928 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/normal/dla.py
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/normal/dpn.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/normal/net.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.848679 trojanzoo-2.0.0/trojanvision/models/others/
+-rw-r--r--   0 root         (0) root         (0)      196 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/others/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7219 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/others/magnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.848679 trojanzoo-2.0.0/trojanvision/models/torchvision/
+-rw-r--r--   0 root         (0) root         (0)      724 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/torchvision/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2423 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/torchvision/alexnet.py
+-rw-r--r--   0 root         (0) root         (0)     3648 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/torchvision/densenet.py
+-rw-r--r--   0 root         (0) root         (0)     4174 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/torchvision/efficientnet.py
+-rw-r--r--   0 root         (0) root         (0)     2727 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/torchvision/mnasnet.py
+-rw-r--r--   0 root         (0) root         (0)     3530 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/torchvision/mobilenet.py
+-rw-r--r--   0 root         (0) root         (0)     8284 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/torchvision/resnet.py
+-rw-r--r--   0 root         (0) root         (0)     4247 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/torchvision/shufflenetv2.py
+-rw-r--r--   0 root         (0) root         (0)     3699 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/models/torchvision/vgg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.848679 trojanzoo-2.0.0/trojanvision/shortcut/
+-rw-r--r--   0 root         (0) root         (0)       58 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/shortcut/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13302 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/shortcut/pgd.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.852679 trojanzoo-2.0.0/trojanvision/utils/
+-rw-r--r--   0 root         (0) root         (0)     2641 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9275 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.852679 trojanzoo-2.0.0/trojanvision/utils/datasets/
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6102 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/datasets/downsampled_imagenet.py
+-rw-r--r--   0 root         (0) root         (0)     2202 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.852679 trojanzoo-2.0.0/trojanvision/utils/model_archs/
+-rw-r--r--   0 root         (0) root         (0)      885 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8509 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/bit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.852679 trojanzoo-2.0.0/trojanvision/utils/model_archs/darts/
+-rw-r--r--   0 root         (0) root         (0)      131 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/darts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4593 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/darts/features.py
+-rw-r--r--   0 root         (0) root         (0)    10884 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/darts/genotypes.py
+-rw-r--r--   0 root         (0) root         (0)     5945 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/darts/operations.py
+-rw-r--r--   0 root         (0) root         (0)     6067 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/darts/search.py
+-rw-r--r--   0 root         (0) root         (0)    11910 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/darts/sgas.py
+-rw-r--r--   0 root         (0) root         (0)    10085 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/dla.py
+-rw-r--r--   0 root         (0) root         (0)     8661 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/dpn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.852679 trojanzoo-2.0.0/trojanvision/utils/model_archs/enas/
+-rw-r--r--   0 root         (0) root         (0)      130 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/enas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3333 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/enas/macro.py
+-rw-r--r--   0 root         (0) root         (0)    14031 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/enas/mutables.py
+-rw-r--r--   0 root         (0) root         (0)     3400 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/enas/ops.py
+-rw-r--r--   0 root         (0) root         (0)     1549 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/lanet.py
+-rw-r--r--   0 root         (0) root         (0)     4285 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/pnasnet.py
+-rw-r--r--   0 root         (0) root         (0)     5806 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/resnet_ap.py
+-rw-r--r--   0 root         (0) root         (0)     1933 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/model_archs/resnet_s.py
+-rw-r--r--   0 root         (0) root         (0)     2761 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/sgm.py
+-rw-r--r--   0 root         (0) root         (0)    11205 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanvision/utils/transform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.852679 trojanzoo-2.0.0/trojanzoo/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6739 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/attacks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.856679 trojanzoo-2.0.0/trojanzoo/configs/
+-rw-r--r--   0 root         (0) root         (0)    10382 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/configs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/configs/attack.yml
+-rw-r--r--   0 root         (0) root         (0)      125 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/configs/dataset.yml
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/configs/defense.yml
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/configs/env.yml
+-rw-r--r--   0 root         (0) root         (0)       48 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/configs/model.yml
+-rw-r--r--   0 root         (0) root         (0)      146 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/configs/trainer.yml
+-rw-r--r--   0 root         (0) root         (0)    22356 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/datasets.py
+-rw-r--r--   0 root         (0) root         (0)     6064 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/defenses.py
+-rw-r--r--   0 root         (0) root         (0)     7468 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/environ.py
+-rw-r--r--   0 root         (0) root         (0)    66195 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.856679 trojanzoo-2.0.0/trojanzoo/optim/
+-rw-r--r--   0 root         (0) root         (0)      134 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/optim/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10815 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/optim/optimizer.py
+-rw-r--r--   0 root         (0) root         (0)    13659 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/optim/pgd.py
+-rw-r--r--   0 root         (0) root         (0)     4831 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/optim/uname.py
+-rw-r--r--   0 root         (0) root         (0)    14367 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.856679 trojanzoo-2.0.0/trojanzoo/utils/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7818 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.856679 trojanzoo-2.0.0/trojanzoo/utils/fim/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/fim/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12525 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/fim/ekfac.py
+-rw-r--r--   0 root         (0) root         (0)     3897 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/fim/fim.py
+-rw-r--r--   0 root         (0) root         (0)    15646 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/fim/kfac.py
+-rw-r--r--   0 root         (0) root         (0)     1491 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/lock.py
+-rw-r--r--   0 root         (0) root         (0)    14626 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/logger.py
+-rw-r--r--   0 root         (0) root         (0)     2258 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/memory.py
+-rw-r--r--   0 root         (0) root         (0)     1576 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/metric.py
+-rw-r--r--   0 root         (0) root         (0)    25201 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.860679 trojanzoo-2.0.0/trojanzoo/utils/module/
+-rw-r--r--   0 root         (0) root         (0)     1093 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/module/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6231 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/module/param.py
+-rw-r--r--   0 root         (0) root         (0)     6545 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/module/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.860679 trojanzoo-2.0.0/trojanzoo/utils/ntk/
+-rw-r--r--   0 root         (0) root         (0)     1918 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/ntk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3795 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/output.py
+-rw-r--r--   0 root         (0) root         (0)     3120 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/tensor.py
+-rw-r--r--   0 root         (0) root         (0)    13800 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/utils/train.py
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-14 09:58:13.000000 trojanzoo-2.0.0/trojanzoo/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:58:21.856679 trojanzoo-2.0.0/trojanzoo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9623 2023-05-14 09:58:21.000000 trojanzoo-2.0.0/trojanzoo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10615 2023-05-14 09:58:21.000000 trojanzoo-2.0.0/trojanzoo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 09:58:21.000000 trojanzoo-2.0.0/trojanzoo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 09:58:21.000000 trojanzoo-2.0.0/trojanzoo.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      160 2023-05-14 09:58:21.000000 trojanzoo-2.0.0/trojanzoo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-14 09:58:21.000000 trojanzoo-2.0.0/trojanzoo.egg-info/top_level.txt
```

### Comparing `trojanzoo-1.1.1/LICENSE` & `trojanzoo-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/PKG-INFO` & `trojanzoo-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trojanzoo
-Version: 1.1.1
+Version: 2.0.0
 Summary: a universal pytorch platform to conduct security researches
 Home-page: https://github.com/ain-soph/trojanzoo
 Author: Ren Pang
 Author-email: rbp5354@psu.edu
 License: GPL-3
 Keywords: pytorch,image classification,backdoor attack/defense
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.3
@@ -30,15 +30,15 @@
 [![docs](https://github.com/ain-soph/trojanzoo/workflows/docs/badge.svg)](https://ain-soph.github.io/trojanzoo/)
 
 [![release](https://img.shields.io/github/v/release/ain-soph/trojanzoo)](https://github.com/ain-soph/trojanzoo/releases)
 [![pypi](https://img.shields.io/pypi/v/trojanzoo)](https://pypi.org/project/trojanzoo/)
 [![docker](https://img.shields.io/pypi/v/trojanzoo?label=docker)](https://hub.docker.com/r/local0state/trojanzoo)
 <!-- [![conda](https://img.shields.io/pypi/v/trojanzoo?label=conda)](https://anaconda.org/anaconda/trojanzoo) -->
 
-> **NOTE:** TrojanZoo requires `python>=3.10`, `pytorch>=1.11` and `torchvision>=0.12`, which must be installed manually. Recommend to use `conda` to install.
+> **NOTE:** TrojanZoo requires `python>=3.10`, `pytorch>=1.12.1` and `torchvision>=0.13.1`, which must be installed manually. Recommend to use `conda` to install.
 
 This is the code implementation (pytorch) for our paper in EuroS&P 2022:  
 [TrojanZoo: Towards Unified, Holistic, and Practical Evaluation of Neural Backdoors](https://arxiv.org/abs/2012.09302)
 
 TrojanZoo provides a universal pytorch platform to conduct security researches (especially backdoor attacks/defenses) of image classification in deep learning. It is composed of two packages: `trojanzoo` and `trojanvision`. `trojanzoo` contains abstract classes and utilities, while `trojanvision` contains abstract and concrete ones for image classification task. 
 
 > Note: This repository is also maintained to cover the implementation of
```

### Comparing `trojanzoo-1.1.1/README.md` & `trojanzoo-2.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [![docs](https://github.com/ain-soph/trojanzoo/workflows/docs/badge.svg)](https://ain-soph.github.io/trojanzoo/)
 
 [![release](https://img.shields.io/github/v/release/ain-soph/trojanzoo)](https://github.com/ain-soph/trojanzoo/releases)
 [![pypi](https://img.shields.io/pypi/v/trojanzoo)](https://pypi.org/project/trojanzoo/)
 [![docker](https://img.shields.io/pypi/v/trojanzoo?label=docker)](https://hub.docker.com/r/local0state/trojanzoo)
 <!-- [![conda](https://img.shields.io/pypi/v/trojanzoo?label=conda)](https://anaconda.org/anaconda/trojanzoo) -->
 
-> **NOTE:** TrojanZoo requires `python>=3.10`, `pytorch>=1.11` and `torchvision>=0.12`, which must be installed manually. Recommend to use `conda` to install.
+> **NOTE:** TrojanZoo requires `python>=3.10`, `pytorch>=1.12.1` and `torchvision>=0.13.1`, which must be installed manually. Recommend to use `conda` to install.
 
 This is the code implementation (pytorch) for our paper in EuroS&P 2022:  
 [TrojanZoo: Towards Unified, Holistic, and Practical Evaluation of Neural Backdoors](https://arxiv.org/abs/2012.09302)
 
 TrojanZoo provides a universal pytorch platform to conduct security researches (especially backdoor attacks/defenses) of image classification in deep learning. It is composed of two packages: `trojanzoo` and `trojanvision`. `trojanzoo` contains abstract classes and utilities, while `trojanvision` contains abstract and concrete ones for image classification task. 
 
 > Note: This repository is also maintained to cover the implementation of
```

### Comparing `trojanzoo-1.1.1/docs/make.bat` & `trojanzoo-2.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/docs/source/conf.py` & `trojanzoo-2.0.0/docs/source/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import trojanzoo as package  # noqa
 
 pkg_name = package.__name__
 pkg_file = package.__file__
 pkg_version = str(package.__version__)
 pkg_location = path.dirname(path.dirname(pkg_file))
 
-autoapi_dirs = ['../../trojanzoo']
+# autoapi_dirs = ['../../trojanzoo']
 
 # -- General configuration ------------------------------------------------
 
 project = 'TrojanZoo'
 author = 'ain-soph'
 copyright = f'2021, {author}'
 
@@ -53,23 +53,24 @@
     'logo_dark': 'images/logo/trojanzoo-logo-dark.svg',
     'logo_icon': 'images/logo/trojanzoo-logo-icon.svg',
 }
 
 # -- Extension configuration ----------------------------------------------
 
 extensions = [
-    # 'sphinx.ext.autodoc',
+    'sphinx.ext.autodoc',
     'sphinx.ext.autosectionlabel',
     'sphinx.ext.githubpages',
     'sphinx.ext.intersphinx',
     'sphinx.ext.linkcode',  # viewcode
     'sphinx.ext.napoleon',
     'sphinxcontrib.katex',
+    'sphinxcontrib.jquery',
     'sphinx_copybutton',
-    'autoapi.extension',
+    # 'autoapi.extension',
 ]
 
 
 def linkcode_resolve(domain, info):
     return linkcode_helper(
         domain, info,
         prefix=pkg_location,
@@ -87,35 +88,35 @@
     'sklearn': ('https://scikit-learn.org/stable/', None),
     'torch': ('https://pytorch.org/docs/stable/', None),
     'torchvision': ('https://pytorch.org/vision/stable/', None),
 }
 
 # -- General default configuration ----------------------------------------
 
-needs_sphinx = '4.0.2'
+needs_sphinx = '7.0.0'
 templates_path = ['_templates']
 source_suffix = '.rst'  # ['.rst', '.md']
 root_doc = 'index'
 
 release = pkg_version
 version = release if release.find('a') == -1 else release[:release.find('a')]
 
-language = None
+language = 'en'
 exclude_patterns = []
 
 # -- General default extension configuration ------------------------------
 
 # autodoc options
 autodoc_docstring_signature = True
 autodoc_inherit_docstrings = False
 autodoc_preserve_defaults = True
 autodoc_typehints = 'none'
 
-autoapi_type = 'python'
-autoapi_generate_api_docs = False
+# autoapi_type = 'python'
+# autoapi_generate_api_docs = False
 
 # autosectionlabel options
 # autosectionlabel throws warnings if section names are duplicated.
 # The following tells autosectionlabel to not throw a warning for
 # duplicated section names that are in different documents.
 autosectionlabel_prefix_document = True
```

### Comparing `trojanzoo-1.1.1/docs/source/images/favicon.ico` & `trojanzoo-2.0.0/docs/source/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/docs/source/images/logo/trojanzoo-logo-dark.svg` & `trojanzoo-2.0.0/docs/source/images/logo/trojanzoo-logo-dark.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/docs/source/images/logo/trojanzoo-logo-icon.svg` & `trojanzoo-2.0.0/docs/source/images/logo/trojanzoo-logo-icon.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/docs/source/images/logo/trojanzoo-logo.svg` & `trojanzoo-2.0.0/docs/source/images/logo/trojanzoo-logo.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/docs/source/images/screenshot.png` & `trojanzoo-2.0.0/docs/source/images/screenshot.png`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/docs/source/images/trojanvision/center_cropped.png` & `trojanzoo-2.0.0/docs/source/images/trojanvision/center_cropped.png`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/docs/source/images/trojanvision/grad_cam.png` & `trojanzoo-2.0.0/docs/source/images/trojanvision/grad_cam.png`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/docs/source/images/trojanvision/grad_cam_impose.png` & `trojanzoo-2.0.0/docs/source/images/trojanvision/grad_cam_impose.png`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/docs/source/images/trojanvision/saliency_map.png` & `trojanzoo-2.0.0/docs/source/images/trojanvision/saliency_map.png`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/docs/source/images/trojanvision/saliency_map_impose.png` & `trojanzoo-2.0.0/docs/source/images/trojanvision/saliency_map_impose.png`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/docs/source/images/trojanzoo-logo-readme.svg` & `trojanzoo-2.0.0/docs/source/images/trojanzoo-logo-readme.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/docs/source/tutorials/basic.rst` & `trojanzoo-2.0.0/docs/source/tutorials/basic.rst`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/examples/adv_attack.py` & `trojanzoo-2.0.0/examples/adv_attack.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 #!/usr/bin/env python3
 
-# CUDA_VISIBLE_DEVICES=1 python examples/adv_attack.py --verbose 1 --color --attack pgd --dataset cifar10 --model resnet18_comp --pretrained --stop_threshold 0.0 --target_idx 1 --require_class --grad_method nes --valid_batch_size 200
+r"""
+CUDA_VISIBLE_DEVICES=1 python examples/adv_attack.py --verbose 1 --color --attack pgd --dataset cifar10 --model resnet18_comp --pretrained --stop_threshold 0.0 --target_idx 1 --require_class --grad_method nes --valid_batch_size 200
+"""  # noqa: E501
 
 import trojanvision
 import argparse
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
     trojanvision.environ.add_argument(parser)
     trojanvision.datasets.add_argument(parser)
     trojanvision.models.add_argument(parser)
     trojanvision.trainer.add_argument(parser)
     trojanvision.attacks.add_argument(parser)
-    kwargs = parser.parse_args().__dict__
+    kwargs = vars(parser.parse_args())
 
     env = trojanvision.environ.create(**kwargs)
     dataset = trojanvision.datasets.create(**kwargs)
     model = trojanvision.models.create(dataset=dataset, **kwargs)
     trainer = trojanvision.trainer.create(dataset=dataset, model=model, **kwargs)
     attack = trojanvision.attacks.create(dataset=dataset, model=model, **kwargs)
```

### Comparing `trojanzoo-1.1.1/examples/adv_defense.py` & `trojanzoo-2.0.0/examples/adv_defense.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     parser = argparse.ArgumentParser()
     trojanvision.environ.add_argument(parser)
     trojanvision.datasets.add_argument(parser)
     trojanvision.models.add_argument(parser)
     trojanvision.trainer.add_argument(parser)
     trojanvision.attacks.add_argument(parser)
     trojanvision.defenses.add_argument(parser)
-    kwargs = parser.parse_args().__dict__
+    kwargs = vars(parser.parse_args())
 
     env = trojanvision.environ.create(**kwargs)
     dataset = trojanvision.datasets.create(**kwargs)
     model = trojanvision.models.create(dataset=dataset, **kwargs)
     trainer = trojanvision.trainer.create(dataset=dataset, model=model, **kwargs)
     attack = trojanvision.attacks.create(dataset=dataset, model=model, **kwargs)
     defense = trojanvision.defenses.create(dataset=dataset, model=model, attack=attack, **kwargs)
```

### Comparing `trojanzoo-1.1.1/examples/adv_validate.py` & `trojanzoo-2.0.0/examples/adv_validate.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
     trojanvision.environ.add_argument(parser)
     trojanvision.datasets.add_argument(parser)
     trojanvision.models.add_argument(parser)
     trojanvision.trainer.add_argument(parser)
     trojanvision.attacks.add_argument(parser)
-    kwargs = parser.parse_args().__dict__
+    kwargs = vars(parser.parse_args())
 
     env = trojanvision.environ.create(**kwargs)
     dataset = trojanvision.datasets.create(**kwargs)
     model = trojanvision.models.create(dataset=dataset, **kwargs)
     trainer = trojanvision.trainer.create(dataset=dataset, model=model, **kwargs)
     attack: PoisonRandom = trojanvision.attacks.create(dataset=dataset, model=model, **kwargs)
```

### Comparing `trojanzoo-1.1.1/examples/backdoor_attack.py` & `trojanzoo-2.0.0/examples/backdoor_attack.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 #!/usr/bin/env python3
 
-# CUDA_VISIBLE_DEVICES=0 python ./examples/backdoor_attack.py --color --verbose 1 --attack badnet --pretrained --validate_interval 1 --epochs 50 --lr 1e-2
+r"""
+CUDA_VISIBLE_DEVICES=0 python ./examples/backdoor_attack.py --color --verbose 1 --attack badnet --pretrained --validate_interval 1 --epochs 50 --lr 1e-2
+"""  # noqa: E501
 
 import trojanvision
 import argparse
 
+from trojanvision.attacks import BackdoorAttack
+
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
     trojanvision.environ.add_argument(parser)
     trojanvision.datasets.add_argument(parser)
     trojanvision.models.add_argument(parser)
     trojanvision.trainer.add_argument(parser)
     trojanvision.marks.add_argument(parser)
     trojanvision.attacks.add_argument(parser)
-    kwargs = parser.parse_args().__dict__
+    kwargs = vars(parser.parse_args())
 
     env = trojanvision.environ.create(**kwargs)
     dataset = trojanvision.datasets.create(**kwargs)
     model = trojanvision.models.create(dataset=dataset, **kwargs)
     trainer = trojanvision.trainer.create(dataset=dataset, model=model, **kwargs)
     mark = trojanvision.marks.create(dataset=dataset, **kwargs)
-    attack = trojanvision.attacks.create(dataset=dataset, model=model, mark=mark, **kwargs)
+    attack: BackdoorAttack = trojanvision.attacks.create(dataset=dataset, model=model, mark=mark, **kwargs)
 
     if env['verbose']:
         trojanvision.summary(env=env, dataset=dataset, model=model, mark=mark, trainer=trainer, attack=attack)
     attack.attack(**trainer)
```

### Comparing `trojanzoo-1.1.1/examples/backdoor_defense.py` & `trojanzoo-2.0.0/examples/backdoor_validate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 #!/usr/bin/env python3
 
-# CUDA_VISIBLE_DEVICES=0 python ./examples/backdoor_defense.py --color --verbose 1 --attack badnet --defense neural_cleanse --validate_interval 1 --epochs 50 --lr 1e-2
-
 import trojanvision
 import argparse
 
+from trojanvision.attacks import BackdoorAttack
+
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
     trojanvision.environ.add_argument(parser)
     trojanvision.datasets.add_argument(parser)
     trojanvision.models.add_argument(parser)
-    trojanvision.trainer.add_argument(parser)
     trojanvision.marks.add_argument(parser)
     trojanvision.attacks.add_argument(parser)
-    trojanvision.defenses.add_argument(parser)
-    kwargs = parser.parse_args().__dict__
+    kwargs = vars(parser.parse_args())
 
     env = trojanvision.environ.create(**kwargs)
     dataset = trojanvision.datasets.create(**kwargs)
     model = trojanvision.models.create(dataset=dataset, **kwargs)
-    trainer = trojanvision.trainer.create(dataset=dataset, model=model, **kwargs)
     mark = trojanvision.marks.create(dataset=dataset, **kwargs)
-    attack = trojanvision.attacks.create(dataset=dataset, model=model, mark=mark, **kwargs)
-    defense = trojanvision.defenses.create(dataset=dataset, model=model, attack=attack, **kwargs)
+    attack: BackdoorAttack = trojanvision.attacks.create(dataset=dataset, model=model, mark=mark, **kwargs)
 
     if env['verbose']:
-        trojanvision.summary(env=env, dataset=dataset, model=model, mark=mark, trainer=trainer, attack=attack, defense=defense)
-    defense.detect(**trainer)
+        trojanvision.summary(env=env, dataset=dataset, model=model, mark=mark, attack=attack)
+    attack.load()
+    attack.validate_fn()
```

### Comparing `trojanzoo-1.1.1/examples/backdoor_validate.py` & `trojanzoo-2.0.0/examples/backdoor_defense.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 #!/usr/bin/env python3
 
+r"""
+CUDA_VISIBLE_DEVICES=0 python ./examples/backdoor_defense.py --color --verbose 1 --attack badnet --defense neural_cleanse --validate_interval 1 --epochs 50 --lr 1e-2
+"""  # noqa: E501
+
 import trojanvision
-from trojanvision.attacks import BadNet
 import argparse
 
+from trojanvision.attacks import BackdoorAttack
+from trojanvision.defenses import BackdoorDefense
+
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
     trojanvision.environ.add_argument(parser)
     trojanvision.datasets.add_argument(parser)
     trojanvision.models.add_argument(parser)
+    trojanvision.trainer.add_argument(parser)
     trojanvision.marks.add_argument(parser)
     trojanvision.attacks.add_argument(parser)
-    kwargs = parser.parse_args().__dict__
+    trojanvision.defenses.add_argument(parser)
+    kwargs = vars(parser.parse_args())
 
     env = trojanvision.environ.create(**kwargs)
     dataset = trojanvision.datasets.create(**kwargs)
     model = trojanvision.models.create(dataset=dataset, **kwargs)
+    trainer = trojanvision.trainer.create(dataset=dataset, model=model, **kwargs)
     mark = trojanvision.marks.create(dataset=dataset, **kwargs)
-    attack: BadNet = trojanvision.attacks.create(dataset=dataset, model=model, mark=mark, **kwargs)
+    attack: BackdoorAttack = trojanvision.attacks.create(dataset=dataset, model=model, mark=mark, **kwargs)
+    defense: BackdoorDefense = trojanvision.defenses.create(dataset=dataset, model=model, attack=attack, **kwargs)
 
     if env['verbose']:
-        trojanvision.summary(env=env, dataset=dataset, model=model, mark=mark, attack=attack)
-    attack.load()
-    attack.validate_fn()
+        trojanvision.summary(env=env, dataset=dataset, model=model, mark=mark, trainer=trainer, attack=attack, defense=defense)
+    defense.detect(**trainer)
```

### Comparing `trojanzoo-1.1.1/examples/heatmap.py` & `trojanzoo-2.0.0/examples/heatmap.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 #!/usr/bin/env python3
 
 import trojanvision
 from trojanvision.utils import superimpose
-import torchvision.transforms.functional as F
+
+import torchvision
 import argparse
 import os
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
     trojanvision.environ.add_argument(parser)
     trojanvision.datasets.add_argument(parser)
     trojanvision.models.add_argument(parser)
-    kwargs = parser.parse_args().__dict__
+    kwargs = vars(parser.parse_args())
 
     env = trojanvision.environ.create(**kwargs)
     dataset = trojanvision.datasets.create(**kwargs)
     model = trojanvision.models.create(dataset=dataset, **kwargs)
 
     if not os.path.exists('./result'):
         os.makedirs('./result')
 
     if env['verbose']:
         trojanvision.summary(env=env, dataset=dataset, model=model)
     for data in dataset.loader['valid']:
         _input, _label = model.get_data(data)
         heatmap = model.get_heatmap(_input, _label, method='saliency_map')
         heatmap = superimpose(heatmap, _input, alpha=0.5)
-        for i, map in enumerate(heatmap):
-            F.to_pil_image(heatmap[i]).save(f'./result/heatmap_{i}.jpg')
+        torchvision.utils.save_image(heatmap, './result/heatmap.jpg')
         break
```

### Comparing `trojanzoo-1.1.1/examples/train.py` & `trojanzoo-2.0.0/examples/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 r"""
-CUDA_VISIBLE_DEVICES=0 python examples/train.py --verbose 1 --color --epochs 200 --batch_size 96 --cutout --grad_clip 5.0 --lr 0.025 --lr_scheduler
+CUDA_VISIBLE_DEVICES=0 python examples/train.py --verbose 1 --color --epochs 200 --batch_size 96 --cutout --lr 0.025 --lr_scheduler
 
 # adv train pgd
 CUDA_VISIBLE_DEVICES=0 python examples/train.py --verbose 1 --color --adv_train --adv_train_random_init --validate_interval 1 --epochs 15 --lr 0.1 --lr_scheduler
 
 # adv train fgsm
 CUDA_VISIBLE_DEVICES=0 python examples/train.py --verbose 1 --color --adv_train --adv_train_random_init --adv_train_iter 1 --adv_train_alpha 0.0392156862745 --adv_train_eval_iter 7 --adv_train_eval_alpha 0.0078431372549 --validate_interval 1 --epochs 15 --lr 0.1 --lr_scheduler
 
@@ -18,15 +18,15 @@
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
     trojanvision.environ.add_argument(parser)
     trojanvision.datasets.add_argument(parser)
     trojanvision.models.add_argument(parser)
     trojanvision.trainer.add_argument(parser)
-    kwargs = parser.parse_args().__dict__
+    kwargs = vars(parser.parse_args())
 
     env = trojanvision.environ.create(**kwargs)
     dataset = trojanvision.datasets.create(**kwargs)
     model = trojanvision.models.create(dataset=dataset, **kwargs)
     trainer = trojanvision.trainer.create(dataset=dataset, model=model, **kwargs)
 
     if env['verbose']:
```

### Comparing `trojanzoo-1.1.1/examples/validate.py` & `trojanzoo-2.0.0/examples/validate.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import argparse
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
     trojanvision.environ.add_argument(parser)
     trojanvision.datasets.add_argument(parser)
     trojanvision.models.add_argument(parser)
-    kwargs = parser.parse_args().__dict__
+    kwargs = vars(parser.parse_args())
 
     env = trojanvision.environ.create(**kwargs)
     dataset = trojanvision.datasets.create(**kwargs)
     model = trojanvision.models.create(dataset=dataset, **kwargs)
 
     if env['verbose']:
         trojanvision.summary(env=env, dataset=dataset, model=model)
```

### Comparing `trojanzoo-1.1.1/setup.cfg` & `trojanzoo-2.0.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 	image classification
 	backdoor attack/defense
 
 [options]
 zip_safe = False
 packages = find:
 install_requires = 
-	torch>=1.11
-	torchvision>=0.12
-	numpy>=1.20.3
+	torch>=1.12.1
+	torchvision>=0.13.1
+	numpy>=1.22
 	matplotlib>=3.4.2
 	scikit-image>=0.19.2
 	scikit-learn>=0.24.0
 	scipy>=1.5.4
 	pyyaml>=5.3.1
 	pandas>=1.1.5
 	tqdm>=4.54.1
```

### Comparing `trojanzoo-1.1.1/trojanvision/attacks/__init__.py` & `trojanzoo-2.0.0/trojanvision/attacks/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/attacks/abstract.py` & `trojanzoo-2.0.0/trojanvision/attacks/abstract.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,37 +104,34 @@
             case 'dataset':
                 self.poison_num = int(len(self.dataset.loader['train'].dataset) * self.poison_ratio)
                 self.poison_set = self.get_poison_dataset()
             case _:
                 self.poison_set = None
 
     def attack(self, epochs: int, **kwargs):
+        kwargs['validate_fn'] = kwargs.get('validate_fn', self.validate_fn)
+        kwargs['save_fn'] = kwargs.get('save_fn', self.save)
         match self.train_mode:
             case 'batch':
                 loader = self.dataset.get_dataloader(
                     'train', batch_size=self.dataset.batch_size + int(self.poison_num))
                 return self.model._train(epochs, loader_train=loader,
-                                         validate_fn=self.validate_fn,
                                          get_data_fn=self.get_data,
-                                         save_fn=self.save, **kwargs)
+                                         **kwargs)
             case 'dataset':
                 mix_dataset = torch.utils.data.ConcatDataset([self.dataset.loader['train'].dataset,
                                                               self.poison_set])
                 loader = self.dataset.get_dataloader('train', dataset=mix_dataset)
-                return self.model._train(epochs, loader_train=loader,
-                                         validate_fn=self.validate_fn,
-                                         save_fn=self.save, **kwargs)
+                return self.model._train(epochs, loader_train=loader, **kwargs)
             case 'loss':
                 if 'loss_fn' in kwargs.keys():
                     kwargs['loss_fn'] = functools.partial(self.loss_weighted, loss_fn=kwargs['loss_fn'])
                 else:
                     kwargs['loss_fn'] = self.loss_weighted
-                return self.model._train(epochs,
-                                         validate_fn=self.validate_fn,
-                                         save_fn=self.save, **kwargs)
+                return self.model._train(epochs, **kwargs)
             case _:
                 raise NotImplementedError(f'{self.train_mode=}')
 
     def get_poison_dataset(self, poison_label: bool = True,
                            poison_num: int = None,
                            seed: int = None
                            ) -> torch.utils.data.Dataset:
```

### Comparing `trojanzoo-1.1.1/trojanvision/attacks/backdoor/clean_label/clean_label.py` & `trojanzoo-2.0.0/trojanvision/attacks/backdoor/clean_label/clean_label.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/attacks/backdoor/clean_label/invisible_poison.py` & `trojanzoo-2.0.0/trojanvision/attacks/backdoor/clean_label/invisible_poison.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/attacks/backdoor/clean_label/label_consistent.py` & `trojanzoo-2.0.0/trojanvision/attacks/backdoor/clean_label/label_consistent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 from ...abstract import BackdoorAttack
 from trojanzoo.utils.model import init_weights
 from trojanvision.attacks.adv import PGD    # TODO: Need to check whether this will cause ImportError
-from trojanvision.optim import PGDoptimizer
-from trojanvision.environ import env
+from trojanzoo.environ import env
+from trojanzoo.optim import PGD as PGDoptimizer
 from trojanzoo.utils.data import TensorListDataset, dataset_to_tensor, sample_batch
 
 import torch
 import torch.nn as nn
 import torch.optim as optim
 
 import argparse
@@ -25,15 +25,15 @@
 
     Clean Label Backdoor Attack is described in detail in the paper `Clean Label Backdoor Attack`_ by Alexander Turner.
 
     The main idea is to perturb the poisoned samples
     in order to render learning the salient characteristic of the input more difficult,
     causing the model rely more heavily on the backdoor pattern in order to successfully introduce backdoor.
 
-    Utilize the adversarial examples and GAB generated data,
+    Utilize the adversarial examples and GAN generated data,
     the resulted poisoned inputs appear to be consistent with their label
     and thus seem benign even upon human inspection.
 
     The authors haven't posted `original source code`_.
 
     Args:
         poison_generation_method (str): the chosen method to generate poisoned sample. Default: 'pgd'.
@@ -172,18 +172,16 @@
                         source_encode = self.wgan.get_encode_value(source_chunk).detach()
                         target_encode = self.wgan.get_encode_value(target_chunk).detach()
                         # noise = torch.randn_like(source_encode)
                         # source_img = self.wgan.G(source_encode)
                         # target_img = self.wgan.G(target_encode)
                         # if not os.path.exists('./imgs'):
                         #     os.makedirs('./imgs')
-                        # for i in range(len(source_img)):
-                        #     F.to_pil_image(source_img[i]).save(f'./imgs/source_{i}.png')
-                        # for i in range(len(target_img)):
-                        #     F.to_pil_image(target_img[i]).save(f'./imgs/target_{i}.png')
+                        # torchvision.utils.save_image(source_img, './imgs/source.png')
+                        # torchvision.utils.save_image(target_img, './imgs/target.png')
                         # exit()
                         interpolation_encode = source_encode * self.tau + target_encode * (1 - self.tau)
                         poison_imgs = self.wgan.G(interpolation_encode).detach()
                         poison_imgs = self.add_mark(poison_imgs)
 
                         poison_imgs = poison_imgs.cpu()
                         x_list.append(poison_imgs)
```

### Comparing `trojanzoo-1.1.1/trojanvision/attacks/backdoor/clean_label/refool.py` & `trojanzoo-2.0.0/trojanvision/attacks/backdoor/clean_label/refool.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,15 @@
         If :attr:`mark_alpha` ``<0``, use mean of :attr:`x`
         and :attr:`self.mark.mark` as their weights.
         """
         mark_alpha = kwargs.get('mark_alpha', self.mark.mark_alpha)
         if mark_alpha < 0:
             x_weight: float = x.mean().item()
             mark_weight: float = self.mark.mark[:-1].mean().item()
-            alpha = x_weight / (x_weight + mark_weight)
+            alpha = mark_weight / (x_weight + mark_weight)
             kwargs['mark_alpha'] = alpha
         return super().add_mark(x, **kwargs)
 
     def attack(self, epochs: int, optimizer: torch.optim.Optimizer, **kwargs):
         model_dict = copy.deepcopy(self.model.state_dict())
         W = torch.ones(len(self.reflect_imgs))
         refool_optimizer = torch.optim.SGD(optimizer.param_groups[0]['params'],
@@ -372,15 +372,15 @@
                 logger.update(ssim=ssim)
                 if 0.7 < ssim < 0.85:
                     logger.update(reflect_num=1)
                     candidates.add(i)
                     filename = os.path.basename(reflect_paths[i])
                     bytes_io = io.BytesIO()
                     format = os.path.splitext(filename)[1][1:].lower().replace('jpg', 'jpeg')
-                    F.to_pil_image(reflection_layer).save(bytes_io, format=format)
+                    torchvision.utils.save_image(reflection_layer, bytes_io, format=format)
                     bytes_data = bytes_io.getvalue()
                     tarinfo = tarfile.TarInfo(name=filename)
                     tarinfo.size = len(bytes_data)
                     tf.addfile(tarinfo, io.BytesIO(bytes_data))
                     break
         if len(candidates) == num_attack:
             break
```

### Comparing `trojanzoo-1.1.1/trojanvision/attacks/backdoor/dynamic/input_aware_dynamic.py` & `trojanzoo-2.0.0/trojanvision/attacks/backdoor/dynamic/input_aware_dynamic.py`

 * *Files 9% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     def __init__(self, train_mask_epochs: int = 25,
                  lambda_div: float = 1.0, lambda_norm: float = 100.0,
                  mask_density: float = 0.032,
                  cross_percent: float = 0.1,
                  natural: bool = False,
                  poison_percent: float = 0.1, **kwargs):
         super().__init__(poison_percent=poison_percent, **kwargs)
-        self.param_list['input_aware_dynamic'] = ['train_mask_epochs',
+        self.param_list['input_aware_dynamic'] = ['train_mask_epochs', 'natural',
                                                   'lambda_div', 'lambda_norm',
                                                   'mask_density', 'cross_percent']
 
         self.train_mask_epochs = train_mask_epochs
         self.lambda_div = lambda_div
         self.lambda_norm = lambda_norm
         self.mask_density = mask_density
@@ -272,15 +272,19 @@
         if self.clean_acc - clean_acc > threshold:
             asr = 0.0
         return asr, clean_acc
 
     def attack(self, epochs: int, optimizer: torch.optim.Optimizer,
                lr_scheduler: torch.optim.lr_scheduler._LRScheduler = None,
                validate_interval: int = 1, save: bool = False,
+               validate_fn: Callable[..., tuple[float, float]] = None,
+               writer=None, main_tag: str = 'train', tag: str = '',
                verbose: bool = True, **kwargs):
+        validate_fn = validate_fn or self.validate_fn
+        start_epoch: int = 0
         if verbose:
             print('train mask generator')
         self.mark_generator.requires_grad_(False)
         self.mask_generator.requires_grad_()
         self.model.requires_grad_(False)
         self.train_mask_generator(verbose=verbose)
         if verbose:
@@ -299,16 +303,17 @@
         mark_scheduler = torch.optim.lr_scheduler.CosineAnnealingLR(
             mark_optimizer, T_max=epochs)
         loader = self.dataset.loader['train']
         dataset = loader.dataset
         logger = MetricLogger()
         logger.create_meters(loss=None, div=None, ce=None)
 
+        best_validate_result = (0.0, float('inf'))
         if validate_interval != 0:
-            best_validate_result = self.validate_fn(verbose=verbose)
+            best_validate_result = validate_fn(writer=writer, tag=tag, _epoch=start_epoch, verbose=verbose, **kwargs)
             best_asr = best_validate_result[0]
         for _epoch in range(epochs):
             _epoch += 1
             idx = torch.randperm(len(dataset))
             pos = 0
             logger.reset()
             if not self.natural:
@@ -346,59 +351,80 @@
                     cross_int += 1
                 x = _input[trigger_int:trigger_int + cross_int]
                 x2 = _input2[trigger_int:trigger_int + cross_int]
                 cross_mark, cross_mask = self.get_mark(x2), self.get_mask(x2)
                 cross_input = x + cross_mask * (cross_mark - x)
                 final_input[trigger_int:trigger_int + cross_int] = cross_input
 
-                # div loss
-                if len(trigger_input) <= len(cross_input):
-                    length = len(trigger_input)
-                    cross_input = cross_input[:length]
-                    cross_mark = cross_mark[:length]
-                    cross_mask = cross_mask[:length]
-                else:
-                    length = len(cross_input)
-                    trigger_input = trigger_input[:length]
-                    trigger_mark = trigger_mark[:length]
-                    trigger_mask = trigger_mask[:length]
-                input_dist: torch.Tensor = (trigger_input - cross_input).flatten(1).norm(p=2, dim=1)
-                mark_dist: torch.Tensor = (trigger_mark - cross_mark).flatten(1).norm(p=2, dim=1) + 1e-5
-
                 loss_ce = self.model.loss(final_input, final_label)
-                loss_div = input_dist.div(mark_dist).mean()
+                loss = loss_ce
+                # div loss
+                loss_div = torch.zeros_like(loss_ce)
+                if len(trigger_input) > 0 and len(cross_input) > 0:
+                    if len(trigger_input) <= len(cross_input):
+                        length = len(trigger_input)
+                        cross_input = cross_input[:length]
+                        cross_mark = cross_mark[:length]
+                        cross_mask = cross_mask[:length]
+                    else:
+                        length = len(cross_input)
+                        trigger_input = trigger_input[:length]
+                        trigger_mark = trigger_mark[:length]
+                        trigger_mask = trigger_mask[:length]
+                    input_dist: torch.Tensor = (trigger_input - cross_input).flatten(1).norm(p=2, dim=1)
+                    mark_dist: torch.Tensor = (trigger_mark - cross_mark).flatten(1).norm(p=2, dim=1) + 1e-5
+                    loss_div = input_dist.div(mark_dist).mean().nan_to_num(0.0)
+                    loss = loss_ce + self.lambda_div * loss_div
 
-                loss = loss_ce + self.lambda_div * loss_div
                 loss.backward()
                 if not self.natural:
                     optimizer.step()
                 mark_optimizer.step()
                 logger.update(n=batch_size, loss=loss.item(), div=loss_div.item(), ce=loss_ce.item())
             if not self.natural and lr_scheduler:
                 lr_scheduler.step()
             mark_scheduler.step()
             if not self.natural:
                 self.model.eval()
             self.mark_generator.eval()
+            if writer is not None:
+                from torch.utils.tensorboard import SummaryWriter
+                assert isinstance(writer, SummaryWriter)
+                writer.add_scalars(main_tag='Loss/' + main_tag,
+                                   tag_scalar_dict={tag: loss},
+                                   global_step=_epoch + start_epoch)
+                # writer.add_scalars(main_tag='Acc/' + main_tag,
+                #                 tag_scalar_dict={tag: acc},
+                #                 global_step=_epoch + start_epoch)
             if validate_interval != 0 and (_epoch % validate_interval == 0 or _epoch == epochs):
-                validate_result = self.validate_fn(verbose=verbose)
+                validate_result = validate_fn(writer=writer, tag=tag, _epoch=_epoch + start_epoch,
+                                              verbose=verbose, **kwargs)
                 cur_asr = validate_result[0]
                 if cur_asr >= best_asr:
                     best_validate_result = validate_result
                     best_asr = cur_asr
                     if save:
                         self.save()
         if not self.natural:
             optimizer.zero_grad()
         mark_optimizer.zero_grad()
         self.mark_generator.requires_grad_(False)
         self.mask_generator.requires_grad_(False)
         self.model.requires_grad_(False)
         return best_validate_result
 
+    def get_filename(self, target_class: int = None, **kwargs) -> str:
+        r"""Get filenames for current attack settings."""
+        if target_class is None:
+            target_class = self.target_class
+        _file = 'tar{target:d}'.format(target=target_class)
+        _file = 'tar{target:d} poison{poison:.2f} cross{cross:.2f}'.format(
+            target=target_class, poison=self.poison_percent, cross=self.cross_percent)
+        return _file
+
     def save(self, filename: str = None, **kwargs):
         r"""Save attack results to files."""
         filename = filename or self.get_filename(**kwargs)
         file_path = os.path.join(self.folder_path, filename)
         torch.save(self.mask_generator.state_dict(), file_path + '_mask.pth')
         torch.save(self.mark_generator.state_dict(), file_path + '_mark.pth')
         self.model.save(file_path + '.pth')
@@ -539,18 +565,19 @@
             down_seq.add_module(f'bn{3*i+2}', nn.BatchNorm2d(down_channel_list[i + 1], momentum=0.05))
             down_seq.add_module(f'relu{3*i+2}', nn.ReLU(inplace=True))
             down_seq.add_module(f'maxpool{3*i+3}', nn.MaxPool2d(kernel_size=2))
         middle_seq.add_module('conv', conv3x3(num_channels[-1], num_channels[-1]))
         middle_seq.add_module('bn', nn.BatchNorm2d(num_channels[-1], momentum=0.05))
         middle_seq.add_module('relu', nn.ReLU(inplace=True))
         for i in range(len(num_channels)):
-            up_seq.add_module(f'upsample{3*i+1}', nn.Upsample(scale_factor=2.0))
+            up_seq.add_module(f'upsample{3*i+1}', nn.Upsample(scale_factor=2.0, mode='bilinear'))
             up_seq.add_module(f'conv{3*i+2}', conv3x3(up_channel_list[i], up_channel_list[i]))
             up_seq.add_module(f'bn{3*i+2}', nn.BatchNorm2d(up_channel_list[i], momentum=0.05))
             up_seq.add_module(f'relu{3*i+2}', nn.ReLU(inplace=True))
             up_seq.add_module(f'conv{3*i+3}', conv3x3(up_channel_list[i], up_channel_list[i + 1]))
             up_seq.add_module(f'bn{3*i+3}', nn.BatchNorm2d(up_channel_list[i + 1], momentum=0.05))
-            up_seq.add_module(f'relu{3*i+3}', nn.ReLU(inplace=True))
+            if i != len(num_channels) - 1:
+                up_seq.add_module(f'relu{3*i+3}', nn.ReLU(inplace=True))
         seq.add_module('down', down_seq)
         seq.add_module('middle', middle_seq)
         seq.add_module('up', up_seq)
         return seq
```

### Comparing `trojanzoo-1.1.1/trojanvision/attacks/backdoor/normal/badnet.py` & `trojanzoo-2.0.0/trojanvision/attacks/backdoor/normal/badnet.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/attacks/backdoor/normal/imc.py` & `trojanzoo-2.0.0/trojanvision/attacks/backdoor/normal/imc.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/attacks/backdoor/normal/latent_backdoor.py` & `trojanzoo-2.0.0/trojanvision/attacks/backdoor/normal/latent_backdoor.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/attacks/backdoor/normal/trojannet.py` & `trojanzoo-2.0.0/trojanvision/attacks/backdoor/normal/trojannet.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/attacks/backdoor/normal/trojannn.py` & `trojanzoo-2.0.0/trojanvision/attacks/backdoor/normal/trojannn.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/attacks/backdoor/others/unlearn.py` & `trojanzoo-2.0.0/trojanvision/attacks/backdoor/others/unlearn.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/attacks/poison/imc_poison.py` & `trojanzoo-2.0.0/trojanvision/attacks/poison/imc_poison.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 
 from .poison_basic import PoisonBasic
 from trojanvision.attacks import PGD
-from trojanvision.optim import PGDoptimizer
 from trojanvision.models import MagNet
+from trojanzoo.optim import PGD as PGDoptimizer
 
 import torch
 import numpy as np
 import os
 from scipy.stats import ks_2samp
 import argparse
 
@@ -65,22 +65,22 @@
             pgd_eps = 2.0 / 255
         pgd_checker = PGD(pgd_alpha=pgd_alpha, pgd_eps=pgd_eps, iteration=8,
                           dataset=self.dataset, model=self.model, target_idx=self.target_idx, stop_threshold=0.95)
         easy = 0
         difficult = 0
         normal = 0
         loader = self.dataset.get_dataloader(mode='valid', batch_size=1)
-        if 'curvature' in self.__dict__.keys():
+        if 'curvature' in vars(self).keys():
             benign_curvature = self.curvature.benign_measure()
             tgt_curvature_list = []
             org_curvature_list = []
         if self.randomized_smooth:
             org_conf_list = []
             tgt_conf_list = []
-        if 'magnet' in self.__dict__.keys():
+        if 'magnet' in vars(self).keys():
             org_magnet_list = []
             tgt_magnet_list = []
         for data in loader:
             print(easy, normal, difficult)
             if normal >= 100:
                 break
             self.model.load()
@@ -110,15 +110,15 @@
             print(f'[{total+1} / 100]\n'
                   f'target confidence: {np.mean(target_conf_list)}({np.std(target_conf_list)})\n'
                   f'target accuracy: {np.mean(target_acc_list)}({np.std(target_acc_list)})\n'
                   f'clean accuracy Drop: {np.mean(clean_acc_list)}({np.std(clean_acc_list)})\n'
                   f'PGD Norm: {np.mean(pgd_norm_list)}({np.std(pgd_norm_list)})\n\n\n')
             org_conf = self.model.get_target_prob(_input=trigger_input, target=_label)
             tgt_conf = self.model.get_target_prob(_input=trigger_input, target=target_label)
-            if 'curvature' in self.__dict__.keys():
+            if 'curvature' in vars(self).keys():
                 org_curvature_list.extend(self.curvature.measure(trigger_input, _label).detach().cpu().tolist())
                 tgt_curvature_list.extend(self.curvature.measure(trigger_input, target_label).detach().cpu().tolist())
                 print('Curvature:')
                 print(f'    org_curvature: {ks_2samp(org_curvature_list, benign_curvature)}')    # type: ignore
                 print(f'    tgt_curvature: {ks_2samp(tgt_curvature_list, benign_curvature)}')    # type: ignore
                 print()
             if self.randomized_smooth:
@@ -128,15 +128,15 @@
                 tgt_decrease = (tgt_new - tgt_conf).clamp(min=0.0)
                 org_conf_list.extend(org_increase.detach().cpu().tolist())
                 tgt_conf_list.extend(tgt_decrease.detach().cpu().tolist())
                 print('Randomized Smooth:')
                 print(f'    org_confidence: {np.mean(org_conf_list)}')
                 print(f'    tgt_confidence: {np.mean(tgt_conf_list)}')
                 print()
-            if 'magnet' in self.__dict__.keys():
+            if 'magnet' in vars(self).keys():
                 trigger_input = self.magnet(trigger_input)
                 org_new = self.model.get_target_prob(_input=trigger_input, target=_label)
                 tgt_new = self.model.get_target_prob(_input=trigger_input, target=target_label)
                 org_increase = (org_new - org_conf).clamp(min=0.0)
                 tgt_decrease = (tgt_conf - tgt_new).clamp(min=0.0)
                 org_magnet_list.extend(org_increase.detach().cpu().tolist())
                 tgt_magnet_list.extend(tgt_decrease.detach().cpu().tolist())
```

### Comparing `trojanzoo-1.1.1/trojanvision/attacks/poison/poison_basic.py` & `trojanzoo-2.0.0/trojanvision/attacks/poison/poison_basic.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/attacks/poison/poison_random.py` & `trojanzoo-2.0.0/trojanvision/attacks/poison/poison_random.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/configs/__init__.py` & `trojanzoo-2.0.0/trojanvision/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/data/cub200/test.txt` & `trojanzoo-2.0.0/trojanvision/data/cub200/test.txt`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/data/cub200/train.txt` & `trojanzoo-2.0.0/trojanvision/data/cub200/train.txt`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/data/cub200_2011/train_test_split.txt` & `trojanzoo-2.0.0/trojanvision/data/cub200_2011/train_test_split.txt`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/data/isic2018/train.csv` & `trojanzoo-2.0.0/trojanvision/data/isic2018/train.csv`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/data/isic2018/valid.csv` & `trojanzoo-2.0.0/trojanvision/data/isic2018/valid.csv`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/data/refool/insert_reflection.py` & `trojanzoo-2.0.0/trojanvision/data/refool/insert_reflection.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     return tensor.unsqueeze(0) if tensor.dim() == 2 else tensor
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('--voc_root', default='~/voc')
     parser.add_argument('--tar_path', default='~/reflection.tar')
-    kwargs = parser.parse_args().__dict__
+    kwargs = vars(parser.parse_args())
     voc_root: str = kwargs['voc_root']
     tar_path: str = kwargs['tar_path']
 
     print('get image paths')
     datasets = [torchvision.datasets.VOCDetection(voc_root, year=year, image_set=image_set,
                                                   download=True) for year, image_set in sets]
     background_paths = get_img_paths(datasets, positive_class=background_class, negative_class=reflect_class)
@@ -166,15 +166,15 @@
                 logger.update(ssim=ssim)
                 if 0.7 < ssim < 0.85:
                     logger.update(reflect_num=1)
                     candidates.add(i)
                     filename = os.path.basename(reflect_paths[i])
                     bytes_io = io.BytesIO()
                     format = os.path.splitext(filename)[1][1:].lower().replace('jpg', 'jpeg')
-                    F.to_pil_image(reflection_layer).save(bytes_io, format=format)
+                    torchvision.utils.save_image(reflection_layer, bytes_io, format=format)
                     bytes_data = bytes_io.getvalue()
                     tarinfo = tarfile.TarInfo(name=filename)
                     tarinfo.size = len(bytes_data)
                     tf.addfile(tarinfo, io.BytesIO(bytes_data))
                     break
     tf.close()
```

### Comparing `trojanzoo-1.1.1/trojanvision/datasets/__init__.py` & `trojanzoo-2.0.0/trojanvision/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/datasets/folder/__init__.py` & `trojanzoo-2.0.0/trojanvision/datasets/folder/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/datasets/folder/cub200.py` & `trojanzoo-2.0.0/trojanvision/datasets/folder/cub200.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/datasets/folder/gtsrb.py` & `trojanzoo-2.0.0/trojanvision/datasets/folder/gtsrb.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/datasets/folder/imagenet.py` & `trojanzoo-2.0.0/trojanvision/datasets/folder/imagenet.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 from trojanvision.datasets.imagefolder import ImageFolder
-from trojanzoo.utils.module import Module
+import trojanvision
 
 from torchvision import datasets
 import os
 import json
 
 from trojanvision import __file__ as root_file
 root_dir = os.path.dirname(root_file)
@@ -83,25 +83,33 @@
 
     def _get_org_dataset(self, mode: str, data_format: str = None,
                          **kwargs) -> datasets.DatasetFolder:
         data_format = data_format or self.data_format
         split = 'val' if mode == 'valid' else mode
         return datasets.ImageNet(root=self.folder_path, split=split, **kwargs)
 
+    def get_class_names(self) -> list[str]:
+        if hasattr(self, 'class_names'):
+            return getattr(self, 'class_names')
+        dataset: datasets.ImageNet = self.get_org_dataset('train')
+        classes: list[tuple[str, ...]] = dataset.classes
+        return [clss[0] for clss in classes]
+
 
 class Sample_ImageNet(ImageNet):
 
     name: str = 'sample_imagenet'
     num_classes = 10
     url = {}
     org_folder_name = {}
 
+    def _get_org_dataset(self, mode: str, data_format: str = None,
+                         **kwargs) -> datasets.DatasetFolder:
+        return super(ImageNet, self)._get_org_dataset(mode, data_format=data_format, **kwargs)
+
     def initialize_folder(self):
-        _dict = Module(self.__dict__)
-        _dict.__delattr__('folder_path')
-        imagenet = ImageNet(**_dict)
-        class_dict: dict = {}
+        imagenet: ImageNet = trojanvision.datasets.create('imagenet')
         json_path = os.path.normpath(os.path.join(
             root_dir, 'data', 'sample_imagenet', 'class_dict.json'))
         with open(json_path, 'r', encoding='utf-8') as f:
             class_dict: dict = json.load(f)
         imagenet.sample(child_name=self.name, class_dict=class_dict)
```

### Comparing `trojanzoo-1.1.1/trojanvision/datasets/folder/isic.py` & `trojanzoo-2.0.0/trojanvision/datasets/folder/isic.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/datasets/folder/vggface2.py` & `trojanzoo-2.0.0/trojanvision/datasets/folder/vggface2.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,11 +36,11 @@
 
     name: str = 'sample_vggface2'
     num_classes = 20
     url = {}
     org_folder_name = {}
 
     def initialize_folder(self):
-        _dict = Module(self.__dict__)
+        _dict = Module(vars(self))
         _dict.__delattr__('folder_path')
         vggface2 = VGGface2(**_dict)
         vggface2.sample(child_name=self.name, sample_num=self.num_classes)
```

### Comparing `trojanzoo-1.1.1/trojanvision/datasets/imagefolder.py` & `trojanzoo-2.0.0/trojanvision/datasets/imagefolder.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,16 +76,15 @@
                  memory: bool = False, **kwargs):
         self.data_format: str = data_format
         self.memory: bool = memory
         super().__init__(**kwargs)
         self.param_list['imagefolder'] = ['data_format', 'memory', 'org_folder_name',
                                           'url']
         self.class_names = self.get_class_names()
-        if self.num_classes is None:
-            self.num_classes = len(self.class_to_idx)
+        self.num_classes = self.num_classes or len(self.class_names)
 
     def initialize(self, *args, **kwargs):
         r"""You could use this method to transform across different :attr:`data_format`."""
         if self.data_format == 'folder' or \
                 not self.check_files(data_format='folder'):
             self.initialize_folder(*args, **kwargs)
         if self.data_format == 'zip':
@@ -164,21 +163,20 @@
                 kwargs['memory'] = self.memory
         return DatasetClass(root=root, **kwargs)
 
     def get_class_names(self) -> list[str]:
         if hasattr(self, 'class_names'):
             return getattr(self, 'class_names')
         dataset: datasets.ImageFolder = self.get_org_dataset('train')
-        idx_to_class = {i: name for name, i in dataset.class_to_idx.items()}
-        return [idx_to_class[i] for i in range(len(idx_to_class.keys()))]
+        return dataset.classes
 
     def sample(self, child_name: str = None,
                class_dict: dict[str, list[str]] = None,
                sample_num: int = None,
-               method='zip'):
+               method='folder'):
         r"""Sample a subset image folder dataset.
 
         Args:
             child_name (str): Name of child subset.
                 Defaults to ``'{self.name}_sample{sample_num}'``
             class_dict (dict[str, list[str]] | None):
                 Map from new class name to list of old class names.
@@ -186,15 +184,15 @@
                 random sample a subset (1 to 1).
                 Defaults to ``None``.
             sample_num (int | None):
                 The number of subset classes to sample
                 if :attr:`class_dict` is ``None``.
                 Defaults to ``None``.
             method (str): :attr:`data_format` of new subset to save.
-                Defaults to ``'.zip'``.
+                Defaults to ``'folder'``.
         """
         if sample_num is None:
             assert class_dict
             sample_num = len(class_dict)
         if child_name is None and sample_num is not None:
             child_name = f'{self.name}_sample{sample_num:d}'
         src_path = self.folder_path
@@ -250,68 +248,69 @@
                 src2dst_dict[class_name] = class_name
         else:
             src2dst_dict = {src_class: dst_class
                             for src_class, dst_list in class_dict.items()
                             for dst_class in dst_list}
         src_class_list = src2dst_dict.keys()
         print(src2dst_dict)
-        if method == 'zip':
-            for mode in mode_list:
-                print('{purple}mode: {0}{reset}'.format(mode, **ansi))
-                assert mode in ['train', 'valid', 'test']
-                dst_zip_path = os.path.join(dst_path,
-                                            f'{child_name}_{mode}_store.zip')
-                dst_zip = zipfile.ZipFile(dst_zip_path, 'w',
-                                          compression=zipfile.ZIP_STORED)
-                src_zip_path = os.path.join(src_path,
-                                            f'{self.name}_{mode}_store.zip')
-                src_zip = zipfile.ZipFile(src_zip_path, 'r',
-                                          compression=zipfile.ZIP_STORED)
-                _list = src_zip.namelist()
-                if env['tqdm']:
-                    _list = tqdm(_list, leave=False)
-                for filename in _list:
-                    if filename[-1] == '/':
-                        continue
-                    dirname, basename = os.path.split(filename)
-                    mode_check, src_class = os.path.split(dirname)
-                    if mode_check == mode and src_class in src_class_list:
-                        print(filename)
-                        dst_class = src2dst_dict[src_class]
-                        dst_zip.writestr(f'{mode}/{dst_class}/{basename}',
-                                         src_zip.read(filename))
-                src_zip.close()
-                dst_zip.close()
-        elif method == 'folder':
-            len_i = len(class_dict.keys())
-            for mode in mode_list:
-                print('{purple}{0}{reset}'.format(mode, **ansi))
-                assert mode in ['train', 'valid', 'test']
-                for i, dst_class in enumerate(class_dict.keys()):
-                    if not os.path.exists(_path := os.path.join(dst_path,
-                                                                mode,
-                                                                dst_class)):
-                        os.makedirs(_path)
-                    prints('{blue_light}{0}{reset}'.format(dst_class, **ansi),
-                           indent=10)
-                    class_list = class_dict[dst_class]
-                    len_j = len(class_list)
-                    for j, src_class in enumerate(class_list):
-                        _list = os.listdir(os.path.join(src_path,
-                                                        mode,
-                                                        src_class))
-                        prints(output_iter(i + 1, len_i),
-                               output_iter(j + 1, len_j),
-                               f'dst: {dst_class:15s}    '
-                               f'src: {src_class:15s}    '
-                               f'image_num: {len(_list):>8d}',
+        match method:
+            case 'zip':
+                for mode in mode_list:
+                    print('{purple}mode: {0}{reset}'.format(mode, **ansi))
+                    assert mode in ['train', 'valid', 'test']
+                    dst_zip_path = os.path.join(dst_path,
+                                                f'{child_name}_{mode}_store.zip')
+                    dst_zip = zipfile.ZipFile(dst_zip_path, 'w',
+                                              compression=zipfile.ZIP_STORED)
+                    src_zip_path = os.path.join(src_path,
+                                                f'{self.name}_{mode}_store.zip')
+                    src_zip = zipfile.ZipFile(src_zip_path, 'r',
+                                              compression=zipfile.ZIP_STORED)
+                    _list = src_zip.namelist()
+                    if env['tqdm']:
+                        _list = tqdm(_list, leave=False)
+                    for filename in _list:
+                        if filename[-1] == '/':
+                            continue
+                        dirname, basename = os.path.split(filename)
+                        mode_check, src_class = os.path.split(dirname)
+                        if mode_check == mode and src_class in src_class_list:
+                            print(filename)
+                            dst_class = src2dst_dict[src_class]
+                            dst_zip.writestr(f'{mode}/{dst_class}/{basename}',
+                                             src_zip.read(filename))
+                    src_zip.close()
+                    dst_zip.close()
+            case 'folder':
+                len_i = len(class_dict.keys())
+                for mode in mode_list:
+                    print('{purple}{0}{reset}'.format(mode, **ansi))
+                    assert mode in ['train', 'valid', 'test']
+                    for i, dst_class in enumerate(class_dict.keys()):
+                        if not os.path.exists(_path := os.path.join(dst_path,
+                                                                    mode,
+                                                                    dst_class)):
+                            os.makedirs(_path)
+                        prints('{blue_light}{0}{reset}'.format(dst_class, **ansi),
                                indent=10)
-                        if env['tqdm']:
-                            _list = tqdm(_list, leave=False)
-                        for _file in _list:
-                            src_file_path = os.path.join(src_path, mode,
-                                                         src_class, _file)
-                            dst_file_path = os.path.join(dst_path, mode,
-                                                         dst_class, _file)
-                            shutil.copyfile(src_file_path, dst_file_path)
-                        if env['tqdm']:
-                            print('{upline}{clear_line}'.format(**ansi))
+                        class_list = class_dict[dst_class]
+                        len_j = len(class_list)
+                        for j, src_class in enumerate(class_list):
+                            _list = os.listdir(os.path.join(src_path,
+                                                            mode,
+                                                            src_class))
+                            prints(output_iter(i + 1, len_i),
+                                   output_iter(j + 1, len_j),
+                                   f'dst: {dst_class:15s}    '
+                                   f'src: {src_class:15s}    '
+                                   f'image_num: {len(_list):>8d}',
+                                   indent=10)
+                            if env['tqdm']:
+                                _list = tqdm(_list, leave=False)
+                            for _file in _list:
+                                src_file_path = os.path.join(src_path, mode,
+                                                             src_class, _file)
+                                dst_file_path = os.path.join(dst_path, mode,
+                                                             dst_class, _file)
+                                shutil.copyfile(src_file_path, dst_file_path)
+                            if env['tqdm']:
+                                print('{upline}{clear_line}'.format(**ansi))
```

### Comparing `trojanzoo-1.1.1/trojanvision/datasets/imageset.py` & `trojanzoo-2.0.0/trojanvision/datasets/imageset.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,17 +32,14 @@
         For users, please use :func:`create` instead, which is more user-friendly.
 
     Args:
         norm_par (dict[str, list[float]]):
             Data normalization parameters of ``'mean'`` and ``'std'``
             (e.g., ``{'mean': [0.5, 0.4, 0.6], 'std': [0.2, 0.3, 0.1]}``).
             Defaults to ``None``.
-        default_model (str): Default model for the dataset.
-            Usually stored in the config.
-            Defaults to ``'resnet18_comp'``.
         normalize (bool): Whether to use :any:`torchvision.transforms.Normalize`
             in dataset transform. Otherwise, use it as model preprocess layer.
         transform (str): The dataset transform type.
 
             * ``None |'none'`` (:any:`torchvision.transforms.PILToTensor`
               and :any:`torchvision.transforms.ConvertImageDtype`)
             * ``'bit'`` (transform used in BiT network)
@@ -112,15 +109,14 @@
         group.add_argument('--cutmix', action='store_true', help='use cutmix')
         group.add_argument('--cutmix_alpha', type=float, help='cutmix alpha (default: 0.0)')
         group.add_argument('--cutout', action='store_true', help='use cutout')
         group.add_argument('--cutout_length', type=int, help='cutout length')
         return group
 
     def __init__(self, norm_par: dict[str, list[float]] = None,
-                 default_model: str = 'resnet18_comp',
                  normalize: bool = False, transform: str = None,
                  auto_augment: bool = False,
                  mixup: bool = False, mixup_alpha: float = 0.0,
                  cutmix: bool = False, cutmix_alpha: float = 0.0,
                  cutout: bool = False, cutout_length: int = None,
                  **kwargs):
         self.norm_par: dict[str, list[float]] = norm_par
@@ -143,15 +139,15 @@
             mixupcutmix = mixup_transforms[0] if len(mixup_transforms) == 1 \
                 else transforms.RandomChoice(mixup_transforms)
 
             def collate_fn(batch: Iterable[torch.Tensor]) -> Iterable[torch.Tensor]:
                 return mixupcutmix(*default_collate(batch))  # noqa: E731
             self.collate_fn = collate_fn
 
-        super().__init__(default_model=default_model, **kwargs)
+        super().__init__(**kwargs)
         self.param_list['imageset'] = ['data_shape', 'norm_par',
                                        'normalize', 'transform',
                                        'auto_augment']
         if cutout:
             self.param_list['imageset'].append('cutout_length')
 
         if mixup:
```

### Comparing `trojanzoo-1.1.1/trojanvision/datasets/normal/cifar.py` & `trojanzoo-2.0.0/trojanvision/datasets/normal/cifar.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/datasets/normal/downsampled_imagenet.py` & `trojanzoo-2.0.0/trojanvision/datasets/normal/downsampled_imagenet.py`

 * *Files 19% similar despite different names*

```diff
@@ -64,21 +64,46 @@
     It inherits :class:`trojanvision.datasets.ImageSet`.
 
     See Also:
         * paper: `A Downsampled Variant of ImageNet as an Alternative to the CIFAR datasets`_
         * website: https://patrykchrabaszcz.github.io/Imagenet32/
 
     Attributes:
-        name (str): ``'imagenet32'``
+        name (str): ``'imagenet64'``
         num_classes (int): Flexible (passed by command line argument, no larger than 1000).
         data_shape (list[int]): ``[3, 32, 32]``
 
     .. _A Downsampled Variant of ImageNet as an Alternative to the CIFAR datasets:
         https://arxiv.org/abs/1707.08819
     """
     name = 'imagenet32'
     data_shape = [3, 32, 32]
 
     def _get_org_dataset(self, mode: str, **kwargs):
         assert mode in ['train', 'valid']
         return di.ImageNet32(root=self.folder_path, train=(mode == 'train'),
                              num_classes=self.num_classes if self.num_classes < 1000 else None, **kwargs)
+
+
+class ImageNet64(DownsampledImageNet):
+    r"""ImageNet64 dataset introduced by Patryk Chrabaszcz in 2017.
+    It inherits :class:`trojanvision.datasets.ImageSet`.
+
+    See Also:
+        * paper: `A Downsampled Variant of ImageNet as an Alternative to the CIFAR datasets`_
+        * website: https://patrykchrabaszcz.github.io/Imagenet32/
+
+    Attributes:
+        name (str): ``'imagenet32'``
+        num_classes (int): Flexible (passed by command line argument, no larger than 1000).
+        data_shape (list[int]): ``[3, 64, 64]``
+
+    .. _A Downsampled Variant of ImageNet as an Alternative to the CIFAR datasets:
+        https://arxiv.org/abs/1707.08819
+    """
+    name = 'imagenet64'
+    data_shape = [3, 64, 64]
+
+    def _get_org_dataset(self, mode: str, **kwargs):
+        assert mode in ['train', 'valid']
+        return di.ImageNet64(root=self.folder_path, train=(mode == 'train'),
+                             num_classes=self.num_classes if self.num_classes < 1000 else None, **kwargs)
```

### Comparing `trojanzoo-1.1.1/trojanvision/datasets/normal/mnist.py` & `trojanzoo-2.0.0/trojanvision/datasets/normal/mnist.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/defenses/__init__.py` & `trojanzoo-2.0.0/trojanvision/defenses/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/defenses/abstract.py` & `trojanzoo-2.0.0/trojanvision/defenses/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,15 @@
         tn, fp, fn, tp = metrics.confusion_matrix(y_true, y_pred).ravel()
         print()
         print(f'{tn=:d} {fp=:d} {fn=:d} {tp=:d}')
         print(f'f1_score        : {metrics.f1_score(y_true, y_pred):8.3f}')
         print(f'precision_score : {metrics.precision_score(y_true, y_pred):8.3f}')
         print(f'recall_score    : {metrics.recall_score(y_true, y_pred):8.3f}')
         print(f'accuracy_score  : {metrics.accuracy_score(y_true, y_pred):8.3f}')
+        print(f'roc_auc_score  : {metrics.roc_auc_score(y_true, y_pred):8.3f}')
 
     def get_test_data(self) -> tuple[torch.Tensor, torch.Tensor]:
         r"""Get test data.
 
         Returns:
             (torch.Tensor, torch.Tensor):
                 Input and label tensors
@@ -377,16 +378,19 @@
         """
         mark_list: list[torch.Tensor] = []
         loss_list: list[float] = []
         asr_list: list[float] = []
         # todo: parallel to avoid for loop
         file_path = os.path.normpath(os.path.join(
             self.folder_path, self.get_filename() + '.npz'))
+
+        org_target_class = self.attack.target_class
         for label in range(self.model.num_classes):
             print('Class: ', output_iter(label, self.model.num_classes))
+            self.attack.target_class = label
             mark, loss = self.optimize_mark(label, verbose=verbose, **kwargs)
             if verbose:
                 asr, _ = self.attack.validate_fn(indent=4)
                 if not self.mark_random_pos:
                     select_num = self.attack.mark.mark_height * self.attack.mark.mark_width
                     overlap = mask_jaccard(self.attack.mark.get_mask(),
                                            self.real_mask,
@@ -397,14 +401,15 @@
                                               keep_org=False, poison_label=True,
                                               verbose=False)
             mark_list.append(mark)
             loss_list.append(loss)
             asr_list.append(asr)
             np.savez(file_path, mark_list=np.stack([mark.detach().cpu().numpy() for mark in mark_list]),
                      loss_list=np.array(loss_list))
+        self.attack.target_class = org_target_class
         print()
         print('Defense results saved at: ' + file_path)
         mark_list_tensor = torch.stack(mark_list)
         return mark_list_tensor, loss_list, asr_list
 
     def loss(self, _input: torch.Tensor, _label: torch.Tensor, target: int,
              trigger_output: None | torch.Tensor = None,
```

### Comparing `trojanzoo-1.1.1/trojanvision/defenses/adv/advmind.py` & `trojanzoo-2.0.0/trojanvision/defenses/adv/advmind.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/defenses/adv/curvature.py` & `trojanzoo-2.0.0/trojanvision/defenses/adv/curvature.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/defenses/adv/grad_train.py` & `trojanzoo-2.0.0/trojanvision/defenses/adv/grad_train.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/defenses/backdoor/__init__.py` & `trojanzoo-2.0.0/trojanvision/defenses/backdoor/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/defenses/backdoor/attack_agnostic/__init__.py` & `trojanzoo-2.0.0/trojanvision/defenses/backdoor/attack_agnostic/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/defenses/backdoor/attack_agnostic/adv_train.py` & `trojanzoo-2.0.0/trojanvision/defenses/backdoor/attack_agnostic/adv_train.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/defenses/backdoor/attack_agnostic/fine_pruning.py` & `trojanzoo-2.0.0/trojanvision/defenses/backdoor/attack_agnostic/fine_pruning.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/defenses/backdoor/attack_agnostic/magnet.py` & `trojanzoo-2.0.0/trojanvision/defenses/backdoor/attack_agnostic/magnet.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/defenses/backdoor/attack_agnostic/recompress.py` & `trojanzoo-2.0.0/trojanvision/defenses/backdoor/attack_agnostic/recompress.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/defenses/backdoor/input_filtering/neo.py` & `trojanzoo-2.0.0/trojanvision/defenses/backdoor/input_filtering/neo.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/defenses/backdoor/input_filtering/strip.py` & `trojanzoo-2.0.0/trojanvision/defenses/backdoor/input_filtering/strip.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/defenses/backdoor/model_inspection/abs.py` & `trojanzoo-2.0.0/trojanvision/defenses/backdoor/model_inspection/abs.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/defenses/backdoor/model_inspection/deep_inspect.py` & `trojanzoo-2.0.0/trojanvision/defenses/backdoor/model_inspection/deep_inspect.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/defenses/backdoor/model_inspection/neural_cleanse.py` & `trojanzoo-2.0.0/trojanvision/defenses/backdoor/model_inspection/neural_cleanse.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/defenses/backdoor/model_inspection/neuron_inspect.py` & `trojanzoo-2.0.0/trojanvision/defenses/backdoor/model_inspection/neuron_inspect.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/defenses/backdoor/model_inspection/tabor.py` & `trojanzoo-2.0.0/trojanvision/defenses/backdoor/model_inspection/tabor.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/defenses/backdoor/training_filtering/activation_clustering.py` & `trojanzoo-2.0.0/trojanvision/defenses/backdoor/training_filtering/activation_clustering.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/defenses/backdoor/training_filtering/spectral_signature.py` & `trojanzoo-2.0.0/trojanvision/defenses/backdoor/training_filtering/spectral_signature.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/environ.py` & `trojanzoo-2.0.0/trojanvision/environ.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 from trojanvision.configs import config
 from trojanzoo.environ import add_argument, env  # noqa: F401
 import trojanzoo.environ
 
 from trojanvision.configs import Config
 
 
-def create(*args, config: Config = config, **kwargs) -> trojanzoo.environ.Env:
-    return trojanzoo.environ.create(*args, config=config, **kwargs)
+def create(config: Config = config, **kwargs) -> trojanzoo.environ.Env:
+    return trojanzoo.environ.create(config=config, **kwargs)
 
 
 create()
```

### Comparing `trojanzoo-1.1.1/trojanvision/marks/__init__.py` & `trojanzoo-2.0.0/trojanvision/marks/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,15 +372,16 @@
                 It's ignored when alpha channel in watermark image.
                 Defaults to ``'auto'``.
             already_processed (bool):
                 If ``True``, will just load :attr:`mark_img` as :attr:`self.mark`.
                 Defaults to ``False``.
 
         Returns:
-            torch.Tensor: Watermark tensor ranging in ``[0, 1]``
+            torch.Tensor:
+                Watermark tensor ranging in ``[0, 1]``
                 with shape ``(channel + 1, height, width)`` with alpha channel.
         """
         if isinstance(mark_img, str):
             if mark_img.endswith('.npy'):
                 mark_img = np.load(mark_img)
             else:
                 if not os.path.isfile(mark_img) and \
```

### Comparing `trojanzoo-1.1.1/trojanvision/marks/apple_black.png` & `trojanzoo-2.0.0/trojanvision/marks/apple_black.png`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/marks/apple_white.png` & `trojanzoo-2.0.0/trojanvision/marks/apple_white.png`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/marks/square_black.png` & `trojanzoo-2.0.0/trojanvision/marks/square_black.png`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/marks/square_white.png` & `trojanzoo-2.0.0/trojanvision/marks/square_white.png`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/marks/tag_black.png` & `trojanzoo-2.0.0/trojanvision/marks/tag_black.png`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/marks/tag_white.png` & `trojanzoo-2.0.0/trojanvision/marks/tag_white.png`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/marks/watermark_black.png` & `trojanzoo-2.0.0/trojanvision/marks/watermark_black.png`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/marks/watermark_white.png` & `trojanzoo-2.0.0/trojanvision/marks/watermark_white.png`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/models/__init__.py` & `trojanzoo-2.0.0/trojanvision/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,9 +99,9 @@
 
     See Also:
         :func:`trojanzoo.models.output_available_models()`
     """
     return trojanzoo.models.output_available_models(class_dict=class_dict, indent=indent)
 
 
-def get_available_models(class_dict: dict[str, type[ImageModel]] = class_dict) -> dict[str, list[str]]:
+def get_available_models(class_dict: dict[str, type[ImageModel]] = class_dict) -> dict[str, set[str]]:
     return trojanzoo.models.get_available_models(class_dict=class_dict)
```

### Comparing `trojanzoo-1.1.1/trojanvision/models/imagemodel.py` & `trojanzoo-2.0.0/trojanvision/models/imagemodel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python3
 
 from trojanvision.shortcut.pgd import PGD
 from trojanvision.datasets import ImageSet
 from trojanvision.utils import apply_cmap
 from trojanvision.utils.sgm import register_hook
 from trojanzoo.models import _Model, Model
-from trojanzoo.environ import env
 from trojanzoo.utils.fim import KFAC, EKFAC
 from trojanzoo.utils.tensor import add_noise
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.utils.hooks import RemovableHandle
@@ -208,14 +207,15 @@
                  adv_train: str = None, adv_train_random_init: bool = False, adv_train_eval_random_init: bool = None,
                  adv_train_iter: int = 7, adv_train_alpha: float = 2 / 255, adv_train_eps: float = 8 / 255,
                  adv_train_eval_iter: int = None, adv_train_eval_alpha: float = None, adv_train_eval_eps: float = None,
                  adv_train_trades_beta: float = 6.0,
                  norm_layer: str = 'bn', sgm: bool = False, sgm_gamma: float = 1.0,
                  norm_par: dict[str, list[float]] = None, suffix: str = None,
                  modify_first_layer_channel: bool = True, **kwargs):
+        self.norm_par = norm_par
         name = self.get_name(name, layer=layer)
         if norm_par is None and isinstance(dataset, ImageSet):
             norm_par = None if dataset.normalize else dataset.norm_par
         if 'num_classes' not in kwargs.keys() and dataset is None:
             kwargs['num_classes'] = 1000
         if adv_train is not None and suffix is None:
             suffix = f'_at-{adv_train}'
@@ -255,31 +255,18 @@
             if 'suffix' not in self.param_list['model']:
                 self.param_list['model'].append('suffix')
             self.param_list['adv_train'] = ['adv_train', 'adv_train_random_init', 'adv_train_eval_random_init',
                                             'adv_train_iter', 'adv_train_alpha', 'adv_train_eps',
                                             'adv_train_eval_iter', 'adv_train_eval_alpha', 'adv_train_eval_eps']
             if adv_train == 'trades':
                 self.param_list['adv_train'].append('adv_train_trades_beta')
-            clip_min, clip_max = 0.0, 1.0
-            if norm_par is None and isinstance(dataset, ImageSet):
-                if dataset.normalize and dataset.norm_par is not None:
-                    mean = torch.tensor(dataset.norm_par['mean'],
-                                        device=env['device']).view(-1, 1, 1)
-                    std = torch.tensor(dataset.norm_par['std'],
-                                       device=env['device']).view(-1, 1, 1)
-                    clip_min, clip_max = -mean / std, (1 - mean) / std
-                    self.adv_train_eval_alpha /= std
-                    self.adv_train_eval_eps /= std
-                    self.adv_train_alpha /= std
-                    self.adv_train_eps /= std
             self.pgd = PGD(pgd_alpha=self.adv_train_eval_alpha, pgd_eps=self.adv_train_eval_eps,
                            iteration=self.adv_train_eval_iter, stop_threshold=None,
                            target_idx=0,
                            random_init=self.adv_train_eval_random_init,
-                           clip_min=clip_min, clip_max=clip_max,
                            model=self, dataset=self.dataset)
         self._model: _ImageModel
         self.dataset: ImageSet
         self.sgm_remove: list[RemovableHandle]
 
     def trades_loss_fn(self, _input: torch.Tensor, org_prob: torch.Tensor, **kwargs) -> torch.Tensor:
         return -F.kl_div(self(_input, **kwargs).log_softmax(1), org_prob,
@@ -347,16 +334,16 @@
 
         :Example:
             .. code-block:: python
                 :emphasize-lines: 30-32
 
                 import trojanvision
                 from trojanvision.utils import superimpose
+                import torchvision
                 import torchvision.transforms as transforms
-                import torchvision.transforms.functional as F
                 import PIL.Image as Image
                 import os
                 import wget
 
                 env = trojanvision.environ.create(device='cpu')
                 model = trojanvision.models.create(
                     'resnet152', data_shape=[3, 224, 224], official=True,
@@ -383,19 +370,19 @@
                 saliency_map = model.get_heatmap(_input, label,
                                                  method='saliency_map')[:, :3]
                 grad_cam_impose = (grad_cam * 0.4 + _input)
                 saliency_map_impose = (saliency_map * 0.4 + _input)
                 grad_cam_impose = grad_cam_impose.div(grad_cam_impose.max())
                 saliency_map_impose = saliency_map_impose.div(saliency_map_impose.max())
 
-                F.to_pil_image(_input).save('./center_cropped.png')
-                F.to_pil_image(grad_cam).save('./grad_cam.png')
-                F.to_pil_image(saliency_map).save('./saliency_map.png')
-                F.to_pil_image(grad_cam_impose).save('./grad_cam_impose.png')
-                F.to_pil_image(saliency_map_impose).save('./saliency_map_impose.png')
+                torchvision.utils.save_image(_input, './center_cropped.png')
+                torchvision.utils.save_image(grad_cam, './grad_cam.png')
+                torchvision.utils.save_image(saliency_map, './saliency_map.png')
+                torchvision.utils.save_image(grad_cam_impose, './grad_cam_impose.png')
+                torchvision.utils.save_image(saliency_map_impose, './saliency_map_impose.png')
 
             ``label=386  conf=77.74%``
 
             .. table::
                 :align: left
                 :widths: 80, 160, 160
```

### Comparing `trojanzoo-1.1.1/trojanvision/models/nas/__init__.py` & `trojanzoo-2.0.0/trojanvision/models/nas/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/models/nas/darts.py` & `trojanzoo-2.0.0/trojanvision/models/nas/darts.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 class DARTS(ImageModel):
     r"""DARTS-like models used in Neural Architecture Search.
 
     :Available model names:
 
         .. code-block:: python3
 
-            ['darts']
+            {'darts'}
 
     See Also:
         * paper: `DARTS\: Differentiable Architecture Search`_
         * code: https://github.com/quark0/darts
 
     Args:
         supernet (bool): Whether to use supernet (mixed operations).
@@ -116,15 +116,15 @@
 
     Note:
         The implementation of DARTS model is in ``trojanvision.utils.model_archs.darts``
 
     .. _DARTS\: Differentiable Architecture Search:
         https://arxiv.org/abs/1806.09055
     """
-    available_models = ['darts']
+    available_models = {'darts'}
 
     @classmethod
     def add_argument(cls, group: argparse._ArgumentGroup):
         super().add_argument(group)
         group.add_argument('--supernet', action='store_true', help='whether to use supernet')
         group.add_argument('--model_arch', help='genotype name (default: "darts")')
         group.add_argument('--layers', type=int, help='total number of layers (default: 20)')
```

### Comparing `trojanzoo-1.1.1/trojanvision/models/nas/enas.py` & `trojanzoo-2.0.0/trojanvision/models/nas/enas.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,25 +47,25 @@
     Warning:
         It is highly recommended to use :class:`trojanvision.models.DARTS` with ``model_arch='enas'`` instead.
 
     :Available model names:
 
         .. code-block:: python3
 
-            ['enas']
+            {'enas'}
 
     See Also:
         * paper: `Efficient Neural Architecture Search via Parameter Sharing`_
         * official code (tensorflow): https://github.com/melodyguan/enas
         * NNI code (pytorch): https://github.com/microsoft/nni
 
     .. _Efficient Neural Architecture Search via Parameter Sharing:
         https://arxiv.org/abs/1802.03268
     """
-    available_models = ['enas']
+    available_models = {'enas'}
 
     def __init__(self, name: str = 'enas', model: type[_ENAS] = _ENAS, folder_path: str = None, **kwargs):
         import sys
         from trojanvision.utils.model_archs.enas import __file__ as file_path
         sys.path.append(os.path.dirname(file_path))
         _model = torch.load(os.path.join(folder_path, 'enas_macro.pt'))  # generated by nni library
         super().__init__(name=name, model=model, _model=_model, folder_path=folder_path, **kwargs)
```

### Comparing `trojanzoo-1.1.1/trojanvision/models/nas/lanet.py` & `trojanzoo-2.0.0/trojanvision/models/nas/lanet.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,25 +24,25 @@
     r"""LaNet proposed by Linnan Wang from Facebook in TPAMI 2021.
     It inherits :class:`trojanvision.models.DARTS`.
 
     :Available model names:
 
         .. code-block:: python3
 
-            ['lanet']
+            {'lanet'}
 
     See Also:
         * paper: `Sample-Efficient Neural Architecture Search by Learning Action Space`_
         * code: https://github.com/facebookresearch/LaMCTS
 
     .. _Sample-Efficient Neural Architecture Search by Learning Action Space:
         https://arxiv.org/abs/1906.06832
     """
-    available_models = ['lanet']
-    model_urls = {'cifar10': '1bZsEoG-sroVyYR4F_2ozGLA5W50CT84P', }
+    available_models = {'lanet'}
+    model_urls = {'cifar10': '1bZsEoG-sroVyYR4F_2ozGLA5W50CT84P', }  # TODO
 
     def __init__(self, name: str = 'lanet', layers: int = 24, init_channels: int = 128,
                  arch: list[int] = cifar_arch, model: type[_DARTS] = _DARTS,
                  supernet: bool = False, **kwargs):
         genotype = None
         if not supernet:
             genotype = translator(gen_code_from_list(arch))
@@ -73,15 +73,15 @@
             _dict = _dict['model_state_dict']
         new_dict: OrderedDict[str, torch.Tensor] = self.state_dict()
         old_keys = list(_dict.keys())
         new_keys = list(new_dict.keys())
         new2old: dict[str, str] = {}
         i = 0
         j = 0
-        while(i < len(new_keys) and j < len(old_keys)):
+        while (i < len(new_keys) and j < len(old_keys)):
             if 'auxiliary_head' not in new_keys[i] and 'auxiliary_head' in old_keys[j]:
                 j += 1
                 continue
             new2old[new_keys[i]] = old_keys[j]
             i += 1
             j += 1
         for i, key in enumerate(new_keys):
```

### Comparing `trojanzoo-1.1.1/trojanvision/models/nas/natsbench.py` & `trojanzoo-2.0.0/trojanvision/models/nas/natsbench.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,39 +10,84 @@
 from collections import OrderedDict
 
 import argparse
 from typing import Any
 from collections.abc import Callable
 
 
+class DARTSCells(nn.ModuleList):
+    def __init__(self, cells: nn.ModuleList, alphas: nn.Parameter):
+        super().__init__(cells)
+        self.alphas = alphas
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        alphas = self.alphas.softmax(dim=-1)
+        for cell in self:
+            if 'search' in cell.__class__.__name__.lower():
+                x = cell(x, alphas)
+            else:
+                x = cell(x)
+        return x
+
+    def arch_str(self) -> str:
+        genotypes = []
+        for i in range(1, self[0].max_nodes):
+            xlist = []
+            for j in range(i):
+                node_str = "{:}<-{:}".format(i, j)
+                with torch.no_grad():
+                    weights = self.alphas[self[0].edge2index[node_str]]
+                    op_name = self[0].op_names[weights.argmax().item()]
+                xlist.append((op_name, j))
+            genotypes.append(tuple(xlist))
+        from xautodl.models.cell_searchs.genotypes import Structure   # type: ignore
+        return Structure(genotypes).tostr()
+
+
 class _NATSbench(_ImageModel):
 
     def __init__(self, network: nn.Module = None, **kwargs):
         super().__init__(**kwargs)
         self.load_model(network)
 
     def load_model(self, network: nn.Module):
-        self.features = nn.Sequential(OrderedDict([
-            ('stem', getattr(network, 'stem')),
-            ('cells', nn.Sequential(*getattr(network, 'cells'))),
-            ('lastact', getattr(network, 'lastact')),
-        ]))
+        if 'darts' in network.__class__.__name__.lower():
+            self.features = nn.Sequential(OrderedDict([
+                ('stem', getattr(network, 'stem')),
+                ('cells', DARTSCells(network.cells, network.arch_parameters)),
+                ('lastact', getattr(network, 'lastact')),
+            ]))
+        else:
+            self.features = nn.Sequential(OrderedDict([
+                ('stem', getattr(network, 'stem')),
+                ('cells', nn.Sequential(*getattr(network, 'cells'))),
+                ('lastact', getattr(network, 'lastact')),
+            ]))
         self.classifier = nn.Sequential(OrderedDict([
             ('fc', getattr(network, 'classifier'))
         ]))
 
+    def arch_parameters(self) -> list[torch.Tensor]:
+        return [self.features.cells.alphas]
+
+    def arch_str(self) -> str:
+        if isinstance(self.features.cells, DARTSCells):
+            return self.features.cells.arch_str()
+        else:
+            raise TypeError(f'Cells are not DARTSCells but {type(self.features.cells)}')
+
 
 class NATSbench(ImageModel):
     r"""NATS-Bench proposed by Xuanyi Dong from University of Technology Sydney.
 
     :Available model names:
 
         .. code-block:: python3
 
-            ['nats_bench']
+            {'nats_bench'}
 
     Note:
         There are prerequisites to use the benchmark:
 
         * ``pip install nats_bench``.
         * ``git clone https://github.com/D-X-Y/AutoDL-Projects.git`` and ``pip install .``
         * Extract ``NATS-tss-v1_0-3ffb9-full`` to :attr:`nats_path`.
@@ -59,15 +104,15 @@
         model_index (int): :attr:`model_index` passed to
             ``api.get_net_config()``.
             Ranging from ``0 -- 15624``.
             Defaults to ``0``.
         model_seed (int): :attr:`model_seed` passed to
             ``api.get_net_param()``.
             Choose from ``[777, 888, 999]``.
-            Defaults to ``999``.
+            Defaults to ``777``.
         hp (int): Training epochs.
             :attr:`hp` passed to ``api.get_net_param()``.
             Choose from ``[12, 200]``.
             Defaults to ``200``.
         nats_path (str): NATS benchmark file path.
             It should be set as format like
             ``'**/NATS-tss-v1_0-3ffb9-full'``
@@ -75,44 +120,44 @@
             Choose from ``['tss', 'sss']``.
         dataset_name (str): Dataset name.
             Choose from ``['cifar10', 'cifar10-valid', 'cifar100', 'imagenet16-120']``.
 
     .. _NATS-Bench\: Benchmarking NAS Algorithms for Architecture Topology and Size:
         https://arxiv.org/abs/2009.00437
     """
-    available_models = ['nats_bench']
+    available_models = {'nats_bench'}
 
     @classmethod
     def add_argument(cls, group: argparse._ArgumentGroup):
         super().add_argument(group)
         group.add_argument('--model_index', type=int)
         group.add_argument('--model_seed', type=int)
         group.add_argument('--hp', type=int)
         group.add_argument('--nats_path')
         group.add_argument('--search_space')
         return group
 
     def __init__(self, name: str = 'nats_bench', model: type[_NATSbench] = _NATSbench,
-                 model_index: int = 0, model_seed: int = 999, hp: int = 200,
+                 model_index: int = 0, model_seed: int = 777, hp: int = 200,
                  dataset: ImageSet | None = None, dataset_name: str | None = None,
                  nats_path: str | None = None,
                  search_space: str = 'tss', **kwargs):
         try:
             # pip install nats_bench
             from nats_bench import create   # type: ignore
             from xautodl.models import get_cell_based_tiny_net   # type: ignore
         except ImportError:
             raise ImportError('You need to install nats_bench and auto-dl library')
 
         if isinstance(dataset, ImageSet):
             kwargs['dataset'] = dataset
             if dataset_name is None:
                 dataset_name = dataset.name
-                if dataset_name == 'imagenet16':
-                    dataset_name = f'imagenet16-{dataset.num_classes:d}'
+            if dataset_name == 'imagenet16':
+                dataset_name = f'imagenet16-{dataset.num_classes:d}'
         assert dataset_name is not None
         dataset_name = dataset_name.replace('imagenet16', 'ImageNet16')
         self.dataset_name = dataset_name
 
         self.model_index = model_index
         self.model_seed = model_seed
         self.hp = hp
@@ -120,17 +165,24 @@
         self.nats_path = nats_path
 
         self.api = create(nats_path, search_space, fast_mode=True, verbose=False)
         config: dict[str, Any] = self.api.get_net_config(model_index, dataset_name)
         self.get_cell_based_tiny_net: Callable[..., nn.Module] = get_cell_based_tiny_net
         network = self.get_cell_based_tiny_net(config)
         super().__init__(name=name, model=model, network=network, **kwargs)
-        self.param_list['nats_bench'] = ['model_index', 'model_seed', 'hp', 'search_space', 'nats_path']
+        self.param_list['nats_bench'] = ['arch_str', 'model_index', 'model_seed', 'hp', 'search_space', 'nats_path']
         self._model: _NATSbench
 
+    @property
+    def arch_str(self) -> str:
+        if isinstance(self._model.features.cells, DARTSCells):
+            return self._model.arch_str()
+        config = self.api.get_net_config(self.model_index, self.dataset_name)
+        return config['arch_str']
+
     def get_official_weights(self, model_index: int | None = None,
                              model_seed: int | None = None,
                              hp: int | None = None,
                              **kwargs) -> OrderedDict[str, torch.Tensor]:
         model_index = model_index if model_index is not None else self.model_index
         model_seed = model_seed if model_seed is not None else self.model_seed
         hp = hp if hp is not None else self.hp
```

### Comparing `trojanzoo-1.1.1/trojanvision/models/nas/pnasnet.py` & `trojanzoo-2.0.0/trojanvision/models/nas/pnasnet.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,24 +37,24 @@
         It might be better to reimplement according to tensorflow codes:
         https://github.com/tensorflow/models/blob/master/research/slim/nets/nasnet/pnasnet.py
 
     :Available model names:
 
         .. code-block:: python3
 
-            ['pnasnet', 'pnasnet_a', 'pnasnet_b']
+            {'pnasnet', 'pnasnet_a', 'pnasnet_b'}
 
     See Also:
         * paper: `Progressive Neural Architecture Search`_
         * code: https://github.com/kuangliu/pytorch-cifar/blob/master/models/pnasnet.py
 
     .. _Progressive Neural Architecture Search:
         https://arxiv.org/abs/1712.00559
     """
-    available_models = ['pnasnet', 'pnasnet_a', 'pnasnet_b']
+    available_models = {'pnasnet', 'pnasnet_a', 'pnasnet_b'}
 
     def __init__(self, name: str = 'pnasnet', layer: str = '_b',
                  model: type[_PNASNet] = _PNASNet, **kwargs):
         super().__init__(name=name, layer=layer, model=model, **kwargs)
 
     @classmethod
     def get_name(cls, name: str, layer: str = '') -> str:
```

### Comparing `trojanzoo-1.1.1/trojanvision/models/nas/proxylessnas.py` & `trojanzoo-2.0.0/trojanvision/models/nas/proxylessnas.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,29 +32,29 @@
 class ProxylessNAS(ImageModel):
     r"""ProxylessNAS proposed by Han Cai from MIT in ICLR 2019.
 
     :Available model names:
 
         .. code-block:: python3
 
-            ['proxylessnas']
+            {'proxylessnas'}
 
     See Also:
         * paper: `ProxylessNAS\: Direct Neural Architecture Search on Target Task and Hardware`_
         * code: https://github.com/MIT-HAN-LAB/ProxylessNAS
 
     Args:
         target_platform (str): Target platform to load using :any:`torch.hub.load`.
             Choose from ``['proxyless_cpu', 'proxyless_gpu', 'proxyless_mobile', 'proxyless_mobile_14', 'proxyless_cifar']``
             Defaults to ``'proxyless_cifar'``.
 
     .. _ProxylessNAS\: Direct Neural Architecture Search on Target Task and Hardware:
         https://arxiv.org/abs/1812.00332
     """  # noqa: E501
-    available_models = ['proxylessnas']
+    available_models = {'proxylessnas'}
 
     @classmethod
     def add_argument(cls, group: argparse._ArgumentGroup):
         super().add_argument(group)
         group.add_argument('--target_platform')
         return group
```

### Comparing `trojanzoo-1.1.1/trojanvision/models/normal/bit.py` & `trojanzoo-2.0.0/trojanvision/models/normal/bit.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,25 +49,25 @@
 class BiT(ImageModel):
     r"""Big Transfer (ResNetv2) proposed by Alexander Kolesnikov from Google in ECCV 2020.
 
     :Available model names:
 
         .. code-block:: python3
 
-            ['bit', 'bit_comp', 'bit_official',
+            {'bit', 'bit_comp', 'bit_official',
              'bit-m-r50x1', 'bit-m-r50x3', 'bit-m-r101x1', 'bit-m-r101x3', 'bit-m-r152x2', 'bit-m-r152x4',
              'bit-s-r50x1', 'bit-s-r50x3', 'bit-s-r101x1', 'bit-s-r101x3', 'bit-s-r152x2', 'bit-s-r152x4',
              'bit-m-r50x1_comp', 'bit-m-r50x3_comp', 'bit-m-r101x1_comp',
              'bit-m-r101x3_comp', 'bit-m-r152x2_comp', 'bit-m-r152x4_comp',
              'bit-s-r50x1_comp', 'bit-s-r50x3_comp', 'bit-s-r101x1_comp',
              'bit-s-r101x3_comp', 'bit-s-r152x2_comp', 'bit-s-r152x4_comp',
              'bit-m-r50x1_official', 'bit-m-r50x3_official', 'bit-m-r101x1_official',
              'bit-m-r101x3_official', 'bit-m-r152x2_official', 'bit-m-r152x4_official',
              'bit-s-r50x1_official', 'bit-s-r50x3_official', 'bit-s-r101x1_official',
-             'bit-s-r101x3_official', 'bit-s-r152x2_official', 'bit-s-r152x4_official']
+             'bit-s-r101x3_official', 'bit-s-r152x2_official', 'bit-s-r152x4_official'}
 
     See Also:
         * paper: `Big Transfer (BiT)\: General Visual Representation Learning`_
         * code: https://github.com/google-research/big_transfer
 
     Note:
         ``_comp`` reduces the first convolutional layer
@@ -77,25 +77,25 @@
         and removes following ``norm0, relu0, pool0``
         (``pool0`` is :any:`torch.nn.MaxPool2d`)
         before block layers.
 
     .. _Big Transfer (BiT)\: General Visual Representation Learning:
         https://arxiv.org/abs/1912.11370
     """
-    available_models = ['bit', 'bit_comp', 'bit_official',
+    available_models = {'bit', 'bit_comp', 'bit_official',
                         'bit-m-r50x1', 'bit-m-r50x3', 'bit-m-r101x1', 'bit-m-r101x3', 'bit-m-r152x2', 'bit-m-r152x4',
                         'bit-s-r50x1', 'bit-s-r50x3', 'bit-s-r101x1', 'bit-s-r101x3', 'bit-s-r152x2', 'bit-s-r152x4',
                         'bit-m-r50x1_comp', 'bit-m-r50x3_comp', 'bit-m-r101x1_comp',
                         'bit-m-r101x3_comp', 'bit-m-r152x2_comp', 'bit-m-r152x4_comp',
                         'bit-s-r50x1_comp', 'bit-s-r50x3_comp', 'bit-s-r101x1_comp',
                         'bit-s-r101x3_comp', 'bit-s-r152x2_comp', 'bit-s-r152x4_comp',
                         'bit-m-r50x1_official', 'bit-m-r50x3_official', 'bit-m-r101x1_official',
                         'bit-m-r101x3_official', 'bit-m-r152x2_official', 'bit-m-r152x4_official',
                         'bit-s-r50x1_official', 'bit-s-r50x3_official', 'bit-s-r101x1_official',
-                        'bit-s-r101x3_official', 'bit-s-r152x2_official', 'bit-s-r152x4_official']
+                        'bit-s-r101x3_official', 'bit-s-r152x2_official', 'bit-s-r152x4_official'}
 
     def __init__(self, name: str = 'bit',
                  pretrained_dataset: str = 'm', layer: int = 50, width_factor: int = 1,
                  model: type[_BiT] = _BiT, norm_par: dict[str, list[float]] = None,
                  official: bool = False, **kwargs):
         name = self.parse_name(name, pretrained_dataset, layer, width_factor)
         if official and norm_par is None:
```

### Comparing `trojanzoo-1.1.1/trojanvision/models/normal/dla.py` & `trojanzoo-2.0.0/trojanvision/models/normal/dla.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,31 +5,14 @@
 
 import torch.nn as nn
 
 import torch
 from collections import OrderedDict
 from collections.abc import Callable
 
-urls = {
-    'dla34': 'http://dl.yf.io/dla/models/imagenet/dla34-ba72cf86.pth',
-    'dla46_c': 'http://dl.yf.io/dla/models/imagenet/dla46_c-2bfd52c3.pth',
-    'dla46x_c': 'http://dl.yf.io/dla/models/imagenet/dla46x_c-d761bae7.pth',
-    'dla60x_c': 'http://dl.yf.io/dla/models/imagenet/dla60x_c-b870c45c.pth',
-    'dla60': 'http://dl.yf.io/dla/models/imagenet/dla60-24839fc4.pth',
-    'dla60x': 'http://dl.yf.io/dla/models/imagenet/dla60x-d15cacda.pth',
-    'dla102': 'http://dl.yf.io/dla/models/imagenet/dla102-d94d9790.pth',
-    'dla102x': 'http://dl.yf.io/dla/models/imagenet/dla102x-ad62be81.pth',
-    'dla102x2': 'http://dl.yf.io/dla/models/imagenet/dla102x2-262837b6.pth',
-    'dla169': 'http://dl.yf.io/dla/models/imagenet/dla169-0914e092.pth',
-    # 'dla60_res2net':
-    #     'https://github.com/rwightman/pytorch-image-models/releases/download/v0.1-res2net/res2net_dla60_4s-d88db7f9.pth',
-    # 'dla60_res2next':
-    #     'https://github.com/rwightman/pytorch-image-models/releases/download/v0.1-res2net/res2next_dla60_4s-d327927b.pth',
-}
-
 
 class _DLA(_ImageModel):
 
     def __init__(self, name: str = 'dla', **kwargs):
         super().__init__(**kwargs)
         ModelClass: Callable[..., dla.DLA] = getattr(dla, name.replace('_comp', ''))
         if 'comp' in name:
@@ -41,33 +24,48 @@
         else:
             _model = ModelClass(num_classes=self.num_classes)
         self.features = _model.features
         self.classifier = _model.classifier
 
 
 class DLA(ImageModel):
-    available_models = ['dla', 'dla_comp',
+    available_models = {'dla', 'dla_comp',
                         'dla34', 'dla46_c', 'dla46x_c', 'dla60x_c', 'dla60', 'dla60x',
                         'dla102', 'dla102x', 'dla102x2', 'dla169',
                         'dla34_comp', 'dla46_c_comp', 'dla46x_c_comp', 'dla60x_c_comp', 'dla60_comp', 'dla60x_comp',
-                        'dla102_comp', 'dla102x_comp', 'dla102x2_comp', 'dla169_comp']
-    model_urls = urls
+                        'dla102_comp', 'dla102x_comp', 'dla102x2_comp', 'dla169_comp'}
+    model_urls = {  # TODO
+        'dla34': 'http://dl.yf.io/dla/models/imagenet/dla34-ba72cf86.pth',
+        'dla46_c': 'http://dl.yf.io/dla/models/imagenet/dla46_c-2bfd52c3.pth',
+        'dla46x_c': 'http://dl.yf.io/dla/models/imagenet/dla46x_c-d761bae7.pth',
+        'dla60x_c': 'http://dl.yf.io/dla/models/imagenet/dla60x_c-b870c45c.pth',
+        'dla60': 'http://dl.yf.io/dla/models/imagenet/dla60-24839fc4.pth',
+        'dla60x': 'http://dl.yf.io/dla/models/imagenet/dla60x-d15cacda.pth',
+        'dla102': 'http://dl.yf.io/dla/models/imagenet/dla102-d94d9790.pth',
+        'dla102x': 'http://dl.yf.io/dla/models/imagenet/dla102x-ad62be81.pth',
+        'dla102x2': 'http://dl.yf.io/dla/models/imagenet/dla102x2-262837b6.pth',
+        'dla169': 'http://dl.yf.io/dla/models/imagenet/dla169-0914e092.pth',
+        # 'dla60_res2net':
+        #     'https://github.com/rwightman/pytorch-image-models/releases/download/v0.1-res2net/res2net_dla60_4s-d88db7f9.pth',
+        # 'dla60_res2next':
+        #     'https://github.com/rwightman/pytorch-image-models/releases/download/v0.1-res2net/res2next_dla60_4s-d327927b.pth',
+    }
 
     def __init__(self, name: str = 'dla', layer: int = 34, model: type[_DLA] = _DLA, **kwargs):
         super().__init__(name=name, layer=layer, model=model, **kwargs)
 
     def get_official_weights(self, **kwargs) -> OrderedDict[str, torch.Tensor]:
         old_dict = super().get_official_weights(**kwargs)
         new_dict: OrderedDict[str, torch.Tensor] = self.state_dict()
         old_keys = list(old_dict.keys())
         new_keys = list(new_dict.keys())
         new2old: dict[str, str] = {}
         i = 0
         j = 0
-        while(i < len(new_keys) and j < len(old_keys)):
+        while (i < len(new_keys) and j < len(old_keys)):
             if 'num_batches_tracked' in new_keys[i]:
                 i += 1
                 continue
             if 'project' not in new_keys[i] and 'project' in old_keys[j]:
                 j += 1
                 continue
             # print(f'{new_keys[i]:60} {old_keys[j]}')
```

### Comparing `trojanzoo-1.1.1/trojanvision/models/normal/dpn.py` & `trojanzoo-2.0.0/trojanvision/models/normal/dpn.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,14 @@
         self.features = nn.Sequential(OrderedDict(module_list))
         self.classifier = nn.Sequential(OrderedDict([
             ('fc', _model.fc)
         ]))
 
 
 class DPN(ImageModel):
-    available_models = ['dpn', 'dpn_comp',
+    available_models = {'dpn', 'dpn_comp',
                         'dpn68', 'dpn92', 'dpn98', 'dpn131', 'dpn107',
-                        'dpn68_comp', 'dpn92_comp', 'dpn98_comp', 'dpn131_comp', 'dpn107_comp']
+                        'dpn68_comp', 'dpn92_comp', 'dpn98_comp', 'dpn131_comp', 'dpn107_comp'}
 
     def __init__(self, name: str = 'dpn', layer: int = 92,
                  model: type[_DPN] = _DPN, **kwargs):
         super().__init__(name=name, layer=layer, model=model, **kwargs)
```

### Comparing `trojanzoo-1.1.1/trojanvision/models/normal/net.py` & `trojanzoo-2.0.0/trojanvision/models/normal/net.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,11 +25,11 @@
             ('relu1', nn.ReLU(True)),
             ('dropout2', nn.Dropout(0.5)),
             ('fc2', nn.Linear(128, self.num_classes)),
         ]))
 
 
 class Net(ImageModel):
-    available_models = ['net']
+    available_models = {'net'}
 
     def __init__(self, name: str = 'net', model: type[_Net] = _Net, **kwargs):
         super().__init__(name=name, model=model, **kwargs)
```

### Comparing `trojanzoo-1.1.1/trojanvision/models/others/magnet.py` & `trojanzoo-2.0.0/trojanvision/models/others/magnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     r"""MagNet proposed by Dongyu Meng from Shanghai Tech University in CCS 2017.
     It is an autoencoder for input images to defend against adversarial attacks.
 
     :Available model names:
 
         .. code-block:: python3
 
-            ['magnet']
+            {'magnet'}
 
     See Also:
         * paper: `MagNet\: a Two-Pronged Defense against Adversarial Examples`_
 
     Args:
         structure (list[int | str]): The MagNet model structure.
             Defaults to
@@ -100,15 +100,15 @@
             and ``'relu'`` for 3-channel images.
         v_noise (float): The std of random Gaussian noise added to training data.
             Defaults to ``0.1``.
 
     .. _MagNet\: a Two-Pronged Defense against Adversarial Examples:
         https://arxiv.org/abs/1705.09064
     """
-    available_models = ['magnet']
+    available_models = {'magnet'}
 
     def __init__(self, name: str = 'magnet',
                  dataset: ImageSet = None, model: type = _MagNet,
                  structure: list = None, activation: str = None,
                  v_noise: float = 0.1, **kwargs):
         self.v_noise: float = v_noise
         if structure is None:
```

### Comparing `trojanzoo-1.1.1/trojanvision/models/torchvision/__init__.py` & `trojanzoo-2.0.0/trojanvision/models/torchvision/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/models/torchvision/alexnet.py` & `trojanzoo-2.0.0/trojanvision/models/torchvision/alexnet.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 from trojanvision.models.imagemodel import _ImageModel, ImageModel
 
 import torch.nn as nn
 import torchvision.models
-from torchvision.models.alexnet import model_urls as urls
+from torchvision.models.alexnet import AlexNet_Weights
 
 
 class _AlexNet(_ImageModel):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         _model = torchvision.models.alexnet(num_classes=self.num_classes)
         self.features = _model.features
@@ -21,15 +21,15 @@
 class AlexNet(ImageModel):
     r"""AlexNet proposed by Alex Krizhevsky from Google in 2014.
 
     :Available model names:
 
         .. code-block:: python3
 
-            ['alexnet']
+            {'alexnet'}
 
     See Also:
         * torchvision: :any:`torchvision.models.alexnet`
         * paper: `One weird trick for parallelizing convolutional neural networks`_
 
     .. code-block:: python3
 
@@ -61,13 +61,13 @@
             nn.ReLU(inplace=True),
             nn.Linear(4096, num_classes),
         )
 
     .. _One weird trick for parallelizing convolutional neural networks:
         https://arxiv.org/abs/1404.5997
     """
-    available_models = ['alexnet']
-    model_urls = urls
+    available_models = {'alexnet'}
+    weights = {'alexnet': AlexNet_Weights}
 
     def __init__(self, name: str = 'alexnet',
                  model: type[_AlexNet] = _AlexNet, **kwargs):
         super().__init__(name=name, model=model, **kwargs)
```

### Comparing `trojanzoo-1.1.1/trojanvision/models/torchvision/densenet.py` & `trojanzoo-2.0.0/trojanvision/models/torchvision/densenet.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python3
 
 from trojanvision.models.imagemodel import _ImageModel, ImageModel
 
 import torch
 import torch.nn as nn
 import torchvision.models
-from torchvision.models.densenet import model_urls as urls
+from torchvision.models.densenet import (DenseNet121_Weights, DenseNet161_Weights,
+                                         DenseNet169_Weights, DenseNet201_Weights)
 import re
 from collections import OrderedDict
 
 from collections.abc import Callable
 
 
 class _DenseNet(_ImageModel):
@@ -35,17 +36,17 @@
 class DenseNet(ImageModel):
     r"""DenseNet proposed by Gao Huang from Cornell University in CVPR 2017.
 
     :Available model names:
 
         .. code-block:: python3
 
-            ['densenet', 'densenet_comp',
+            {'densenet', 'densenet_comp',
              'densenet121', 'densenet169', 'densenet201', 'densenet161',
-             'densenet121_comp', 'densenet169_comp', 'densenet201_comp', 'densenet161_comp']
+             'densenet121_comp', 'densenet169_comp', 'densenet201_comp', 'densenet161_comp'}
 
     See Also:
         * torchvision: :any:`torchvision.models.densenet121`
         * paper: `Densely Connected Convolutional Networks`_
 
     Note:
         ``_comp`` reduces the first convolutional layer
@@ -55,18 +56,23 @@
         and removes following ``norm0, relu0, pool0``
         (``pool0`` is :any:`torch.nn.MaxPool2d`)
         before block layers.
 
     .. _Densely Connected Convolutional Networks:
         https://arxiv.org/abs/1608.06993
     """
-    available_models = ['densenet', 'densenet_comp',
+    available_models = {'densenet', 'densenet_comp',
                         'densenet121', 'densenet169', 'densenet201', 'densenet161',
-                        'densenet121_comp', 'densenet169_comp', 'densenet201_comp', 'densenet161_comp']
-    model_urls = urls
+                        'densenet121_comp', 'densenet169_comp', 'densenet201_comp', 'densenet161_comp'}
+    weights = {
+        'densenet121': DenseNet121_Weights,
+        'densenet161': DenseNet161_Weights,
+        'densenet169': DenseNet169_Weights,
+        'densenet201': DenseNet201_Weights,
+    }
 
     def __init__(self, name: str = 'densenet', layer: int = 121,
                  model: type[_DenseNet] = _DenseNet, **kwargs):
         super().__init__(name=name, layer=layer, model=model, **kwargs)
 
     def get_official_weights(self, **kwargs) -> OrderedDict[str, torch.Tensor]:
         _dict = super().get_official_weights(**kwargs)
```

### Comparing `trojanzoo-1.1.1/trojanvision/models/torchvision/mnasnet.py` & `trojanzoo-2.0.0/trojanvision/models/torchvision/mnasnet.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,17 @@
 #!/usr/bin/env python3
 from trojanvision.models.imagemodel import _ImageModel, ImageModel
 
 import torchvision.models
-from torchvision.models._utils import _ModelURLs
+from torchvision.models.mnasnet import MNASNet0_5_Weights, MNASNet0_75_Weights, MNASNet1_0_Weights, MNASNet1_3_Weights
 import re
 
 import torch
 from collections import OrderedDict
 
-urls = _ModelURLs(
-    {
-        "mnasnet0_5": "https://download.pytorch.org/models/mnasnet0.5_top1_67.823-3ffadce67e.pth",
-        "mnasnet0_75": "https://download.pytorch.org/models/mnasnet0_75-7090bc5f.pth",
-        "mnasnet1_0": "https://download.pytorch.org/models/mnasnet1.0_top1_73.512-f206786ef8.pth",
-        "mnasnet1_3": "https://download.pytorch.org/models/mnasnet1_3-a4c69d6f.pth",
-    }
-)
-
 
 class _MNASNet(_ImageModel):
 
     def __init__(self, mnas_alpha: float, **kwargs):
         super().__init__(**kwargs)
         _model = torchvision.models.MNASNet(mnas_alpha, num_classes=self.num_classes)
         self.features = _model.layers
@@ -32,25 +23,30 @@
 class MNASNet(ImageModel):
     r"""MNASNet proposed by Mingxing Tan from Google in CVPR 2019.
 
     :Available model names:
 
         .. code-block:: python3
 
-            ['mnasnet', 'mnasnet0_5', 'mnasnet0_75', 'mnasnet1_0', 'mnasnet1_3']
+            {'mnasnet', 'mnasnet0_5', 'mnasnet0_75', 'mnasnet1_0', 'mnasnet1_3'}
 
     See Also:
         * torchvision: :any:`torchvision.models.mnasnet0_5`
         * paper: `MnasNet\: Platform-Aware Neural Architecture Search for Mobile`_
 
     .. _MnasNet\: Platform-Aware Neural Architecture Search for Mobile:
         https://arxiv.org/abs/1807.11626
     """
-    available_models = ['mnasnet', 'mnasnet0_5', 'mnasnet0_75', 'mnasnet1_0', 'mnasnet1_3']
-    model_urls = urls
+    available_models = {'mnasnet', 'mnasnet0_5', 'mnasnet0_75', 'mnasnet1_0', 'mnasnet1_3'}
+    weights = {
+        'mnasnet0_5': MNASNet0_5_Weights,
+        'mnasnet0_75': MNASNet0_75_Weights,
+        'mnasnet1_0': MNASNet1_0_Weights,
+        'mnasnet1_3': MNASNet1_3_Weights,
+    }
 
     def __init__(self, name: str = 'mnasnet', mnas_alpha: float = 1.0,
                  model: type[_MNASNet] = _MNASNet, **kwargs):
         name, self.mnas_alpha = self.parse_name(name, mnas_alpha)
         super().__init__(name=name, mnas_alpha=self.mnas_alpha, model=model, **kwargs)
 
     @staticmethod
@@ -60,15 +56,15 @@
         if len(name_list) > 1:
             assert len(name_list) == 2
             mnas_alpha = float(name_list[1].replace('_', '.'))
         mnas_alpha_str = f'{mnas_alpha:.2f}'.removesuffix('0')
         return f'{name}{mnas_alpha_str}'.replace('.', '_'), mnas_alpha
 
     def get_official_weights(self, **kwargs) -> OrderedDict[str, torch.Tensor]:
-        url = self.model_urls[self.parse_name('mnasnet', self.mnas_alpha)[0]]
-        _dict = super().get_official_weights(url=url)
+        weights = getattr(self.weights, self.parse_name('mnasnet', self.mnas_alpha)[0])
+        _dict = super().get_official_weights(weights=weights)
         new_dict = OrderedDict()
         for key, value in _dict.items():
             if key.startswith('layers.'):
                 key = 'features.' + key[7:]
             new_dict[key] = value
         return new_dict
```

### Comparing `trojanzoo-1.1.1/trojanvision/models/torchvision/mobilenet.py` & `trojanzoo-2.0.0/trojanvision/models/torchvision/mobilenet.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 from trojanvision.models.imagemodel import _ImageModel, ImageModel
 
 import torch.nn as nn
 import torchvision.models
+from torchvision.models.mobilenet import MobileNet_V2_Weights, MobileNet_V3_Small_Weights, MobileNet_V3_Large_Weights
 
 
 cifar10_inverted_residual_setting = [
     # t, c, n, s
     [1, 16, 1, 1],
     [6, 24, 2, 1],    # Stride 2 -> 1 for CIFAR-10
     [6, 32, 3, 2],
@@ -17,14 +18,15 @@
 ]
 
 
 class _MobileNet(_ImageModel):
     def __init__(self, name: str = 'mobilenet_v2', **kwargs):
         try:
             sub_type: str = name[10:]
+            # TODO
             assert sub_type in ['v2', 'v2_comp', 'v3_small', 'v3_large', 'v3_small_comp', 'v3_large_comp'], f'{name=}'
         except Exception:
             raise AssertionError(f'model name should be in {MobileNet.available_models}')
         super().__init__(**kwargs)
         if 'v2' in sub_type:
             inverted_residual_setting = cifar10_inverted_residual_setting if 'comp' in sub_type else None
             _model = torchvision.models.mobilenet.mobilenet_v2(num_classes=self.num_classes,
@@ -68,18 +70,18 @@
         and set first conv layer ``stride=1``.
 
     .. _MobileNetV2\: Inverted Residuals and Linear Bottlenecks:
         https://arxiv.org/abs/1801.04381
     .. _Searching for MobileNetV3:
         https://arxiv.org/abs/1905.02244
     """
-    available_models = ['mobilenet_v2', 'mobilenet_v3_large', 'mobilenet_v3_small',
-                        'mobilenet_v2_comp', 'mobilenet_v3_large_comp', 'mobilenet_v3_small_comp']
+    available_models = {'mobilenet_v2', 'mobilenet_v3_large', 'mobilenet_v3_small',
+                        'mobilenet_v2_comp', 'mobilenet_v3_large_comp', 'mobilenet_v3_small_comp'}
 
-    model_urls = {
-        'mobilenet_v2': 'https://download.pytorch.org/models/mobilenet_v2-b0353104.pth',
-        'mobilenet_v3_large': 'https://download.pytorch.org/models/mobilenet_v3_large-8738ca79.pth',
-        'mobilenet_v3_small': 'https://download.pytorch.org/models/mobilenet_v3_small-047dcff4.pth',
+    weights = {
+        'mobilenet_v2': MobileNet_V2_Weights,
+        'mobilenet_v3_small': MobileNet_V3_Small_Weights,
+        'mobilenet_v3_large': MobileNet_V3_Large_Weights,
     }
 
     def __init__(self, name: str = 'mobilenet_v2', model: type[_MobileNet] = _MobileNet, **kwargs):
         super().__init__(name=name, model=model, **kwargs)
```

### Comparing `trojanzoo-1.1.1/trojanvision/models/torchvision/resnet.py` & `trojanzoo-2.0.0/trojanvision/models/torchvision/resnet.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 from trojanvision.models.imagemodel import _ImageModel, ImageModel
 from trojanvision.datasets import ImageSet
 import trojanvision.utils.model_archs.resnet_ap as resnet_ap
 
 import torch
 import torch.nn as nn
 import torchvision.models
-from torchvision.models.resnet import model_urls as urls
+from torchvision.models.resnet import (ResNet18_Weights, ResNet34_Weights, ResNet50_Weights,
+                                       ResNet101_Weights, ResNet152_Weights,
+                                       ResNeXt50_32X4D_Weights, ResNeXt101_32X8D_Weights, ResNeXt101_64X4D_Weights,
+                                       Wide_ResNet50_2_Weights, Wide_ResNet101_2_Weights)
 from torchvision.models.resnet import conv3x3
 from collections import OrderedDict
 
 
 class _ResNet(_ImageModel):
 
     def __init__(self, name: str = 'resnet18', dataset: ImageSet = None,
@@ -69,24 +72,24 @@
 class ResNet(ImageModel):
     r"""ResNet model series including ResNet, ResNext and WideResNet.
 
     :Available model names:
 
         .. code-block:: python3
 
-            ['resnet', 'resnet_comp', 'resnet_s',
+            {'resnet', 'resnet_comp', 'resnet_s',
              'resnet18', 'resnet34', 'resnet50', 'resnet101', 'resnet152',
              'resnet18_comp', 'resnet34_comp', 'resnet50_comp', 'resnet101_comp', 'resnet152_comp',
              'resnext50_32x4d', 'resnext101_32x8d',
              'resnext50_32x4d_comp', 'resnext101_32x8d_comp',
              'wide_resnet50_2', 'wide_resnet101_2',
              'wide_resnet50_2_comp', 'wide_resnet101_2_comp',
 
              'resnet18_s', 'resnet34_s', 'resnet50_s', 'resnet101_s', 'resnet152_s',
-             'resnet18_ap_comp']
+             'resnet18_ap_comp'}
 
     See Also:
         * ResNet:
 
           - torchvision: :any:`torchvision.models.resnet18`
           - paper: `Deep Residual Learning for Image Recognition`_
         * ResNext:
@@ -125,25 +128,36 @@
     .. _Wide Residual Networks:
         https://arxiv.org/abs/1605.07146
     .. _Gradient Episodic Memory for Continual Learning:
         https://arxiv.org/abs/1706.08840
     .. _Dataset Condensation with Gradient Matching:
         https://arxiv.org/abs/2006.05929
     """
-    available_models = ['resnet', 'resnet_comp', 'resnet_s',
+    available_models = {'resnet', 'resnet_comp', 'resnet_s',
                         'resnet18', 'resnet34', 'resnet50', 'resnet101', 'resnet152',
                         'resnet18_comp', 'resnet34_comp', 'resnet50_comp', 'resnet101_comp', 'resnet152_comp',
-                        'resnext50_32x4d', 'resnext101_32x8d',
-                        'resnext50_32x4d_comp', 'resnext101_32x8d_comp',
+                        'resnext50_32x4d', 'resnext101_32x8d', 'resnext101_64x4d',
+                        'resnext50_32x4d_comp', 'resnext101_32x8d_comp', 'resnext101_64x4d_comp',
                         'wide_resnet50_2', 'wide_resnet101_2',
                         'wide_resnet50_2_comp', 'wide_resnet101_2_comp',
 
                         'resnet18_s', 'resnet34_s', 'resnet50_s', 'resnet101_s', 'resnet152_s',
-                        'resnet18_ap_comp']
-    model_urls = urls
+                        'resnet18_ap_comp'}
+    weights = {
+        'resnet18': ResNet18_Weights,
+        'resnet34': ResNet34_Weights,
+        'resnet50': ResNet50_Weights,
+        'resnet101': ResNet101_Weights,
+        'resnet152': ResNet152_Weights,
+        'resnext50_32x4d': ResNeXt50_32X4D_Weights,
+        'resnext101_32x8d': ResNeXt101_32X8D_Weights,
+        'resnext101_64x4d': ResNeXt101_64X4D_Weights,
+        'wide_resnet50_2': Wide_ResNet50_2_Weights,
+        'wide_resnet101_2': Wide_ResNet101_2_Weights,
+    }
 
     def __init__(self, name: str = 'resnet', layer: int = 18,
                  model: type[_ResNet] = _ResNet,
                  **kwargs):
         super().__init__(name=name, layer=layer, model=model, **kwargs)
 
     def get_official_weights(self, **kwargs) -> OrderedDict[str, torch.Tensor]:
```

### Comparing `trojanzoo-1.1.1/trojanvision/models/torchvision/shufflenetv2.py` & `trojanzoo-2.0.0/trojanvision/models/torchvision/shufflenetv2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python3
 
 from trojanvision.models.imagemodel import _ImageModel, ImageModel
 
 import torch
 import torch.nn as nn
 import torchvision.models
-from torchvision.models.shufflenetv2 import model_urls as urls
+from torchvision.models.shufflenetv2 import (ShuffleNet_V2_X0_5_Weights, ShuffleNet_V2_X1_0_Weights,
+                                             ShuffleNet_V2_X1_5_Weights, ShuffleNet_V2_X2_0_Weights)
 from collections import OrderedDict
 from collections.abc import Callable
 
 
 class _ShuffleNetV2(_ImageModel):
     def __init__(self, name: str = 'shufflenetv2_x1_0', **kwargs):
         try:
@@ -45,19 +46,19 @@
 class ShuffleNetV2(ImageModel):
     r"""ShuffleNet v2 proposed by Ningning Ma from Megvii in ECCV 2018.
 
     :Available model names:
 
         .. code-block:: python3
 
-            ['shufflenetv2', 'shufflenetv2_comp',
+            {'shufflenetv2', 'shufflenetv2_comp',
              'shufflenetv2_x0_5', 'shufflenetv2_x1_0',
              'shufflenetv2_x1_5', 'shufflenetv2_x2_0',
              'shufflenetv2_x0_5_comp', 'shufflenetv2_x1_0_comp',
-             'shufflenetv2_x1_5_comp', 'shufflenetv2_x2_0_comp', ]
+             'shufflenetv2_x1_5_comp', 'shufflenetv2_x2_0_comp'}
 
     See Also:
         * torchvision: :any:`torchvision.models.shufflenet_v2_x0_5`
         * paper: `ShuffleNet V2\: Practical Guidelines for Efficient CNN Architecture Design`_
 
     Note:
         ``_comp`` reduces the first convolutional layer
@@ -65,21 +66,26 @@
 
         to ``kernel_size=3, stride=1, padding=1``,
         and removes the ``maxpool`` layer before block layers.
 
     .. _ShuffleNet V2\: Practical Guidelines for Efficient CNN Architecture Design:
         https://arxiv.org/abs/1807.11164
     """
-    available_models = ['shufflenetv2', 'shufflenetv2_comp',
+    available_models = {'shufflenetv2', 'shufflenetv2_comp',
                         'shufflenetv2_x0_5', 'shufflenetv2_x1_0',
                         'shufflenetv2_x1_5', 'shufflenetv2_x2_0',
                         'shufflenetv2_x0_5_comp', 'shufflenetv2_x1_0_comp',
-                        'shufflenetv2_x1_5_comp', 'shufflenetv2_x2_0_comp', ]
+                        'shufflenetv2_x1_5_comp', 'shufflenetv2_x2_0_comp'}
 
-    model_urls = urls
+    weights = {
+        'shufflenetv2_x0_5': ShuffleNet_V2_X0_5_Weights,
+        'shufflenetv2_x1_0': ShuffleNet_V2_X1_0_Weights,
+        'shufflenetv2_x1_5': ShuffleNet_V2_X1_5_Weights,
+        'shufflenetv2_x2_0': ShuffleNet_V2_X2_0_Weights,
+    }
 
     def __init__(self, name: str = 'shufflenetv2', layer: str = '_x0_5',
                  model: type[_ShuffleNetV2] = _ShuffleNetV2, **kwargs):
         super().__init__(name=name, layer=layer, model=model, **kwargs)
 
     @classmethod
     def get_name(cls, name: str, layer: str = '') -> str:
```

### Comparing `trojanzoo-1.1.1/trojanvision/models/torchvision/vgg.py` & `trojanzoo-2.0.0/trojanvision/models/torchvision/vgg.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 from trojanvision.models.imagemodel import _ImageModel, ImageModel
 
 import torch.nn as nn
 import torchvision.models
-from torchvision.models.vgg import model_urls as urls
-
+from torchvision.models.vgg import (VGG11_Weights, VGG11_BN_Weights, VGG13_Weights, VGG13_BN_Weights,
+                                    VGG16_Weights, VGG16_BN_Weights, VGG19_Weights, VGG19_BN_Weights)
 from collections.abc import Callable
 
 
 class _VGG(_ImageModel):
 
     def __init__(self, name: str = 'vgg', dropout: float = 0.5, **kwargs):
         if 'num_features' not in kwargs.keys() and ('_comp' or '_s' in name):
@@ -38,40 +38,49 @@
 class VGG(ImageModel):
     r"""VGG model proposed by Karen Simonyan from University of Oxford in ICLR 2015.
 
     :Available model names:
 
         .. code-block:: python3
 
-            ['vgg', 'vgg_bn', 'vgg_comp', 'vgg_bn_comp', 'vgg_s', 'vgg_bn_s',
+            {'vgg', 'vgg_bn', 'vgg_comp', 'vgg_bn_comp', 'vgg_s', 'vgg_bn_s',
              'vgg11', 'vgg13', 'vgg16', 'vgg19',
              'vgg11_bn', 'vgg13_bn', 'vgg16_bn', 'vgg19_bn',
              'vgg11_comp', 'vgg13_comp', 'vgg16_comp', 'vgg19_comp',
              'vgg11_bn_comp', 'vgg13_bn_comp', 'vgg16_bn_comp', 'vgg19_bn_comp'
              'vgg11_s', 'vgg13_s', 'vgg16_s', 'vgg19_s',
-             'vgg11_bn_s', 'vgg13_bn_s', 'vgg16_bn_s', 'vgg19_bn_s']
+             'vgg11_bn_s', 'vgg13_bn_s', 'vgg16_bn_s', 'vgg19_bn_s'}
 
     See Also:
         * torchvision: :any:`torchvision.models.vgg11`
         * paper: `Very Deep Convolutional Networks for Large-Scale Image Recognition`_
 
     Note:
         * ``_comp`` sets :any:`torch.nn.AdaptiveAvgPool2d` from ``(7, 7)`` to ``(1, 1)``,
           update the intermediate feature dimension from 4096 to 512 in ``self.classifier``.
         * ``_s`` further makes ``self.classifier`` only one single linear layer based on ``_comp``.
 
     .. _Very Deep Convolutional Networks for Large-Scale Image Recognition:
         https://arxiv.org/abs/1409.1556
     """
-    available_models = ['vgg', 'vgg_bn', 'vgg_comp', 'vgg_bn_comp', 'vgg_s', 'vgg_bn_s',
+    available_models = {'vgg', 'vgg_bn', 'vgg_comp', 'vgg_bn_comp', 'vgg_s', 'vgg_bn_s',
                         'vgg11', 'vgg13', 'vgg16', 'vgg19',
                         'vgg11_bn', 'vgg13_bn', 'vgg16_bn', 'vgg19_bn',
                         'vgg11_comp', 'vgg13_comp', 'vgg16_comp', 'vgg19_comp',
                         'vgg11_bn_comp', 'vgg13_bn_comp', 'vgg16_bn_comp', 'vgg19_bn_comp'
                         'vgg11_s', 'vgg13_s', 'vgg16_s', 'vgg19_s',
-                        'vgg11_bn_s', 'vgg13_bn_s', 'vgg16_bn_s', 'vgg19_bn_s']
+                        'vgg11_bn_s', 'vgg13_bn_s', 'vgg16_bn_s', 'vgg19_bn_s'}
 
-    model_urls = urls
+    weights = {
+        'vgg11': VGG11_Weights,
+        'vgg11_bn': VGG11_BN_Weights,
+        'vgg13': VGG13_Weights,
+        'vgg13_bn': VGG13_BN_Weights,
+        'vgg16': VGG16_Weights,
+        'vgg16_bn': VGG16_BN_Weights,
+        'vgg19': VGG19_Weights,
+        'vgg19_bn': VGG19_BN_Weights,
+    }
 
     def __init__(self, name: str = 'vgg', layer: int = 13,
                  model: type[_VGG] = _VGG, **kwargs):
         super().__init__(name=name, layer=layer, model=model, **kwargs)
```

### Comparing `trojanzoo-1.1.1/trojanvision/optim/pgd.py` & `trojanzoo-2.0.0/trojanzoo/optim/pgd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-import trojanzoo.optim
+from .optimizer import Optimizer
 
 from trojanzoo.utils.output import prints
 from trojanzoo.utils.tensor import add_noise
 from trojanzoo.environ import env
 
 import torch
 import torch.autograd
@@ -12,33 +12,26 @@
 from collections.abc import Callable
 from typing import Iterable
 
 
 def init_noise(noise_shape: Iterable[int], pgd_eps: float | torch.Tensor,
                random_init: bool = False, device: None | str | torch.device = None) -> torch.Tensor:
     device = device or env['device']
-    noise: torch.Tensor = torch.zeros(noise_shape, dtype=torch.float, device=device)
     if random_init:
-        if isinstance(pgd_eps, torch.Tensor) and pgd_eps.shape[0] != 1:
-            assert all([size == 1 for size in pgd_eps.shape[1:]])
-            for i in range(pgd_eps.shape[0]):
-                data = noise[i, :, :] if noise.dim() == 3 else noise[:, i, :, :]
-                data.uniform_(-pgd_eps[i].item(), pgd_eps[i].item())
-        else:
-            pgd_eps = float(pgd_eps)
-            noise.uniform_(-pgd_eps, pgd_eps)
-    return noise
+        return pgd_eps * torch.rand(*noise_shape, device=device).mul(2).sub(1)
+    else:
+        return torch.zeros(noise_shape, device=device)
 
 
 def valid_noise(adv_input: torch.Tensor, org_input: torch.Tensor, universal: bool = False) -> torch.Tensor:
     result = (adv_input - org_input).detach()
     return result.mode(dim=0)[0] if universal else result
 
 
-class PGDoptimizer(trojanzoo.optim.Optimizer):
+class PGD(Optimizer):
     r"""Projected Gradient Descent.
     Args:
         pgd_alpha (float): learning rate :math:`\pgd_alpha`. Default: :math:`\frac{3}{255}`.
         pgd_eps (float): the perturbation threshold :math:`\pgd_eps` in input space. Default: :math:`\frac{8}{255}`.
 
         norm (int): :math:`L_p` norm passed to :func:`torch.norm`. Default: ``float(inf)``.
         universal (bool): All inputs in the batch share the same noise. Default: ``False``.
@@ -57,17 +50,14 @@
                  clip_min: float | torch.Tensor = 0.0,
                  clip_max: float | torch.Tensor = 1.0,
                  grad_method: str = 'white', query_num: int = 100, sigma: float = 1e-3,
                  hess_b: int = 100, hess_p: int = 1, hess_lambda: float = 1, **kwargs):
         super().__init__(iteration=iteration, **kwargs)
         self.param_list['pgd'] = ['pgd_alpha', 'pgd_eps', 'random_init', 'norm', 'universal']
 
-        pgd_alpha = pgd_alpha if pgd_alpha <= 1.0 else pgd_alpha / 255
-        pgd_eps = pgd_eps if pgd_eps <= 1.0 else pgd_eps / 255
-
         self.pgd_alpha = pgd_alpha
         self.pgd_eps = pgd_eps
         self.random_init = random_init
 
         self.norm = norm
         self.universal = universal
 
@@ -154,15 +144,15 @@
                          clip_max: None | float | torch.Tensor = None,
                          **kwargs) -> torch.Tensor:
         adv_input = add_noise_fn(x=adv_input, noise=noise, universal=self.universal,
                                  clip_min=clip_min, clip_max=clip_max)
         noise.copy_(self.valid_noise(adv_input, org_input))
         return adv_input
 
-    @torch.no_grad()
+    # @torch.no_grad()
     def output_info(self, org_input: torch.Tensor, noise: torch.Tensor, *args,
                     loss_fn: Callable[[torch.Tensor], torch.Tensor] = None,
                     loss_kwargs: dict[str, torch.Tensor] = {},
                     **kwargs):
         super().output_info(*args, **kwargs)
         loss = float(loss_fn(org_input + noise, **loss_kwargs))
         norm = noise.norm(p=self.norm)
@@ -207,30 +197,33 @@
         grad = torch.autograd.grad(loss, x)[0]
         x.requires_grad_(False)
         return grad
 
     def blackbox_grad(self, f: Callable[[torch.Tensor], torch.Tensor], x: torch.Tensor,
                       query_num: int = None, sigma: float = None,
                       loss_kwargs: dict[str, torch.Tensor] = {}) -> torch.Tensor:
-        seq = self.gen_seq(x, query_num=query_num, sigma=sigma)
-        grad = self.calc_seq(f, seq, loss_kwargs=loss_kwargs)
+        query_num = query_num or self.query_num
+        sigma = sigma or self.sigma
+        scale = torch.as_tensor(self.clip_max - self.clip_min, device=x.device)
+        sigma_tensor = sigma * scale
+
+        seq = self.gen_seq(x, query_num=query_num, sigma=sigma_tensor)
+        grad = self.calc_seq(f, seq, sigma=sigma_tensor, loss_kwargs=loss_kwargs)
         return grad
 
-    # x: (N, C, H, W)
-    # return: (query_num+1, N, C, H, W)
-    def gen_seq(self, x: torch.Tensor, query_num: int = None, sigma: float = None) -> torch.Tensor:
-        query_num = query_num if query_num is not None else self.query_num
-        sigma = sigma if sigma is not None else self.sigma
+    # x: (*)
+    # return: (query_num+1, *)
+    def gen_seq(self, x: torch.Tensor, query_num: int, sigma: torch.Tensor) -> torch.Tensor:
         shape = list(x.shape)
         shape.insert(0, query_num)
         if self.grad_method == 'nes':
             shape[0] = shape[0] // 2
         noise = sigma * torch.normal(mean=0.0, std=1.0, size=shape, device=x.device)
 
-        zeros = torch.zeros_like(x.unsqueeze(0))
+        zeros = torch.zeros_like(x).unsqueeze(0)
         seq = [zeros]
         match self.grad_method:
             case 'nes':
                 seq.extend([noise, -noise])
                 if query_num % 2 == 1:
                     seq.append(zeros)
             case 'sgd':
@@ -239,41 +232,43 @@
                 raise NotImplementedError(self.grad_method)
                 noise = (self.hess @ noise.view(-1, 1)).view(x.shape)
                 seq.append(noise)
             case 'zoo':
                 raise NotImplementedError(self.grad_method)
             case _:
                 raise ValueError(f'{self.grad_method=}')
-        seq = torch.cat(seq).add(x)  # (query_num+1, N, C, H, W)
+        seq = torch.cat(seq).add(x)  # (query_num+1, *)
         return seq
 
     @torch.no_grad()
-    def calc_seq(self, f: Callable[[torch.Tensor], torch.Tensor], seq: torch.Tensor,
+    def calc_seq(self, f: Callable[..., torch.Tensor], seq: torch.Tensor,
+                 sigma: torch.Tensor,
                  loss_kwargs: dict[str, torch.Tensor] = {}) -> torch.Tensor:
-        X = seq[0]  # (N, C, H, W)
-        seq = seq[1:]  # (query_num, N, C, H, W)
-        noise = seq.sub(X)
+        X = seq[0]  # (N, *)
+        noise = seq[1:].sub(X)  # (query_num, N, *)
         temp_list: list[torch.Tensor] = []
-        for sub_seq in seq:
-            temp_list.append(f(sub_seq, reduction='none', **loss_kwargs))   # (query_num, N)
-        g = torch.stack(temp_list)[..., None, None, None].mul(noise).sum(dim=0)  # (N, C, H, W)
+        for element in seq[1:]:
+            temp_list.append(f(element, reduction='none', **loss_kwargs))
+        stack_result = torch.stack(temp_list)   # (query_num, N)
+        shape = list(stack_result.size()) + [1]*(noise.dim-stack_result.dim)  # (query_num, N, [1]*[*])
+        g = stack_result.view(shape).mul(noise).sum(dim=0)  # (N, *)
         if self.grad_method in ['sgd', 'hess']:
-            g -= f(X) * noise.sum(dim=0)
-        g /= len(seq) * self.sigma * self.sigma
+            g -= f(X, reduction='none', **loss_kwargs).view(shape[1:]) * noise.sum(dim=0)
+        g /= (len(seq) - 1) * sigma.square()
         return g
 
     @staticmethod
     @torch.no_grad()
     def calc_hess(f: Callable[[torch.Tensor], torch.Tensor], X: torch.Tensor,
-                  sigma: float, hess_b: int, hess_lambda: float = 1) -> torch.Tensor:
+                  sigma: torch.Tensor, hess_b: int, hess_lambda: float = 1) -> torch.Tensor:
         length = X.numel()
         hess: torch.Tensor = torch.zeros(length, length, device=X.device)
         for i in range(hess_b):
             noise = torch.normal(mean=0.0, std=1.0, size=X.shape, device=X.device)
             X1 = X + sigma * noise
             X2 = X - sigma * noise
             hess += abs(f(X1) + f(X2) - 2 * f(X)) * \
                 (noise.view(-1, 1) @ noise.view(1, -1))
-        hess /= (2 * hess_b * sigma * sigma)
+        hess /= (2 * hess_b * sigma.square())
         hess += hess_lambda * torch.eye(length, device=X.device)
         result = hess.cholesky_inverse()
         return result
```

### Comparing `trojanzoo-1.1.1/trojanvision/optim/uname.py` & `trojanzoo-2.0.0/trojanzoo/optim/uname.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 #!/usr/bin/env python3
 
 # todo: Need a better name
 
-import trojanzoo.optim
+from .optimizer import Optimizer
 
 from trojanzoo.utils.output import prints
 from trojanzoo.utils.tensor import atan_func, tanh_func
 
 import torch
 import torch.optim
-from torch.optim import Optimizer
 from torch.optim.lr_scheduler import CosineAnnealingLR
 from collections.abc import Callable
 from typing import Any
 
 
-class Uname(trojanzoo.optim.Optimizer):
+class Uname(Optimizer):
     r"""This class transforms input (tanh, atan or sigmoid) and then apply standard torch.optim.Optimizer
     """
 
     name: str = 'uname'
 
-    def __init__(self, OptimType: str | type[Optimizer], optim_kwargs: dict[str, Any] = {},
+    def __init__(self, OptimType: str | type[torch.optim.Optimizer], optim_kwargs: dict[str, Any] = {},
                  lr_scheduler: bool = False,
                  input_transform: str | Callable[[torch.Tensor], torch.Tensor] = lambda x: x, **kwargs):
         super().__init__(**kwargs)
         self.param_list['uname'] = ['OptimType', 'optim_kwargs', 'lr_scheduler', 'input_transform']
         if isinstance(OptimType, str):
             OptimType = getattr(torch.optim, OptimType)
-        self.OptimType: type[Optimizer] = OptimType
+        self.OptimType: type[torch.optim.Optimizer] = OptimType
         self.optim_kwargs: dict = optim_kwargs
         self.lr_scheduler: bool = lr_scheduler
         self.input_transform: Callable[[torch.Tensor], torch.Tensor] = input_transform
 
     def optimize(self, unbound_params: list[torch.Tensor],
                  iteration: int = None, loss_fn: Callable[[torch.Tensor], torch.Tensor] = None,
                  output: int | list[str] = None, **kwargs) -> tuple[list[torch.Tensor], int]:
```

### Comparing `trojanzoo-1.1.1/trojanvision/shortcut/pgd.py` & `trojanzoo-2.0.0/trojanvision/shortcut/pgd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 #!/usr/bin/env python3
 
-from trojanvision.optim import PGDoptimizer
+from trojanvision.environ import env
 from trojanzoo.attacks import Attack
+from trojanzoo.optim import PGD as PGDoptimizer
 from trojanzoo.utils.output import prints, ansi
 from trojanzoo.utils.logger import SmoothedValue
 
+from trojanvision.datasets import ImageSet
 import torch
 import argparse
 from collections.abc import Callable
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
-    from trojanvision.datasets import ImageSet
     from trojanvision.models import ImageModel
 
 
-def get_func_key(func: Callable[..., torch.Tensor]) -> str:
-    keys = func.__code__.co_varnames
-    valid_keys = [key for key in keys if 'target' in key or 'label' in key or 'y' in key or 'Y' in key]
-    assert len(valid_keys) == 1, keys
-    return valid_keys[0]
-
-
 class PGD(Attack, PGDoptimizer):
     r"""PGD Adversarial Attack.
 
     Args:
         pgd_alpha (float): learning rate :math:`\alpha`. Default: :math:`\frac{3}{255}`.
         pgd_eps (float): the perturbation threshold :math:`\epsilon` in input space. Default: :math:`\frac{8}{255}`.
     """
@@ -33,15 +27,15 @@
 
     @classmethod
     def add_argument(cls, group: argparse._ArgumentGroup):
         super().add_argument(group)
         group.add_argument('--pgd_alpha', type=float, help='PGD learning rate per step, defaults to 2.0/255')
         group.add_argument('--pgd_eps', type=float, help='Projection norm constraint, defaults to 8.0/255')
         group.add_argument('--iteration', type=int, help='Attack Iteration, defaults to 7')
-        group.add_argument('--stop_threshold', type=float, help='early stop confidence, defaults to 0.99')
+        group.add_argument('--stop_threshold', type=float, help='early stop confidence, defaults to 0.99 (defined in config)')
         group.add_argument('--target_class', type=int, help='Do not set it if using target_idx')
         group.add_argument('--target_idx', type=int,
                            help='Target label order in original classification, defaults to -1 '
                            '(0 for untargeted attack, 1 for most possible class, -1 for most unpossible class)')
         group.add_argument('--test_num', type=int, help='total number of test examples for PGD, defaults to 1000.')
         group.add_argument('--num_restart', type=int,
                            help='number of random init for PGD, defaults to 0 (without random initialization).')
@@ -53,22 +47,42 @@
         group.add_argument('--query_num', type=int,
                            help='query numbers for black box gradient estimation, defaults to 100.')
         group.add_argument('--sigma', type=float,
                            help='gaussian sampling std for black box gradient estimation, defaults to 1e-3')
         return group
 
     def __init__(self, target_class: int = None, target_idx: int = -1, test_num: int = 1000, num_restart: int = 0,
-                 require_class: bool = False, **kwargs):
+                 require_class: bool = False,
+                 dataset: ImageSet = None, model: 'ImageModel' = None,
+                 pgd_alpha: float | torch.Tensor = 2.0 / 255,
+                 pgd_eps: float | torch.Tensor = 8.0 / 255,
+                 clip_min: float | torch.Tensor = 0.0,
+                 clip_max: float | torch.Tensor = 1.0,
+                 **kwargs):
         self.target_class = target_class
         self.target_idx = target_idx
         self.test_num = test_num
         self.num_restart = num_restart
         self.require_class = require_class
-        kwargs.update(random_init=bool(num_restart))
-        super().__init__(**kwargs)
+        if num_restart > 0:
+            kwargs.update(random_init=True)
+
+        if model.norm_par is None and isinstance(dataset, ImageSet):
+            if dataset.normalize and dataset.norm_par is not None:
+                mean = torch.tensor(dataset.norm_par['mean'],
+                                    device=env['device']).view(-1, 1, 1)
+                std = torch.tensor(dataset.norm_par['std'],
+                                   device=env['device']).view(-1, 1, 1)
+                clip_min = (clip_min - mean) / std
+                clip_max = (clip_max - mean) / std
+                pgd_alpha = pgd_alpha / std
+                pgd_eps = pgd_eps / std
+        super().__init__(dataset=dataset, model=model,
+                         pgd_alpha=pgd_alpha, pgd_eps=pgd_eps,
+                         clip_min=clip_min, clip_max=clip_max, **kwargs)
         self.param_list['pgd_attack'] = ['target_class', 'target_idx', 'test_num', 'num_restart', 'require_class']
         self.dataset: ImageSet
         self.model: 'ImageModel'
 
     def attack(self, verbose: int = 1, **kwargs) -> tuple[float, float]:
         validset = self.dataset.get_dataset('valid')
         testset, _ = self.dataset.split_dataset(validset, percent=0.3)
@@ -211,15 +225,15 @@
             result = ~result
         if require_class:
             _class = self.model.get_class(adv_input[current_idx])
             class_result = _class == target[current_idx]
             if untarget_condition:
                 class_result = ~class_result
             result = result.bitwise_and(class_result)
-        return result
+        return result.detach().cpu()
 
     @torch.no_grad()
     def output_info(self, org_input: torch.Tensor, noise: torch.Tensor, target: torch.Tensor,
                     loss_fn: Callable[[torch.Tensor], torch.Tensor] = None, **kwargs):
         super().output_info(org_input=org_input, noise=noise, loss_fn=loss_fn, **kwargs)
         # prints('Original class     : ', _label, indent=self.indent)
         # prints('Original confidence: ', _confidence, indent=self.indent)
```

### Comparing `trojanzoo-1.1.1/trojanvision/trainer.py` & `trojanzoo-2.0.0/trojanvision/trainer.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/utils/__init__.py` & `trojanzoo-2.0.0/trojanvision/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/utils/dataset.py` & `trojanzoo-2.0.0/trojanvision/utils/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             try:
                 import accimage  # type: ignore
                 return accimage.Image(f)
             except IOError:
                 pass   # fall through to PIL
         return Image.open(f).convert('RGB')
 
-    def _find_classes(self, *args, **kwargs) -> tuple[list[str], dict[str, int]]:
+    def find_classes(self, *args, **kwargs) -> tuple[list[str], dict[str, int]]:
         r"""Finds the class folders in a dataset.
 
         Args:
             dir (str): Root directory path.
 
         Returns:
             tuple: (classes, class_to_idx) where classes are relative to (dir), and class_to_idx is a dictionary.
```

### Comparing `trojanzoo-1.1.1/trojanvision/utils/datasets/downsampled_imagenet.py` & `trojanzoo-2.0.0/trojanvision/utils/datasets/downsampled_imagenet.py`

 * *Files 12% similar despite different names*

```diff
@@ -133,7 +133,26 @@
         ['train_data_batch_8', '46583e44f926baaeacbf8c333dc6110f'],
         ['train_data_batch_9', '7c82c36ce028b457204f1080d1793669'],
         ['train_data_batch_10', '14e3a6ce19d584ba97208a1d9f551e63'],
     ]
     test_list = [
         ['val_data', '4836a1eec28cd4476eb017126cd0f059'],
     ]
+
+
+class ImageNet64(DownsampledImageNet):
+    data_shape: list[int] = [3, 64, 64]
+    train_list = [
+        ['train_data_batch_1', '7d78180ed6d675199904d73e97363aa3'],
+        ['train_data_batch_2', '62979cbd524679ea440f2eb998cf70ed'],
+        ['train_data_batch_3', '022d13e31ebf76e3a3b4995f59d5898b'],
+        ['train_data_batch_4', 'b595889ec25e147ac6a807e55fa0a5a0'],
+        ['train_data_batch_5', 'd0ca147cd803ad8ad2ea89a82838ff61'],
+        ['train_data_batch_6', '559bdb1c5dc35865d698de7e96067db5'],
+        ['train_data_batch_7', '9799a53adf03a4f99599822ac8ee65ad'],
+        ['train_data_batch_8', '97c910a5c1807fb7ff08f5722c1a6cb8'],
+        ['train_data_batch_9', 'fc1ef2b2a8667a72a046e165413ef006'],
+        ['train_data_batch_10', 'b31fa3cd87885f6161c6e12cb6fd6030'],
+    ]
+    test_list = [
+        ['val_data', '68a29f115231937c359924d8af1b0922'],
+    ]
```

### Comparing `trojanzoo-1.1.1/trojanvision/utils/model.py` & `trojanzoo-2.0.0/trojanvision/utils/model.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/utils/model_archs/__init__.py` & `trojanzoo-2.0.0/trojanvision/utils/model_archs/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/utils/model_archs/bit.py` & `trojanzoo-2.0.0/trojanvision/utils/model_archs/bit.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/utils/model_archs/darts/features.py` & `trojanzoo-2.0.0/trojanvision/utils/model_archs/darts/features.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/utils/model_archs/darts/genotypes.py` & `trojanzoo-2.0.0/trojanvision/utils/model_archs/darts/genotypes.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/utils/model_archs/darts/operations.py` & `trojanzoo-2.0.0/trojanvision/utils/model_archs/darts/operations.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/utils/model_archs/darts/search.py` & `trojanzoo-2.0.0/trojanvision/utils/model_archs/darts/search.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/utils/model_archs/darts/sgas.py` & `trojanzoo-2.0.0/trojanvision/utils/model_archs/darts/sgas.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/utils/model_archs/dla.py` & `trojanzoo-2.0.0/trojanvision/utils/model_archs/dla.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/utils/model_archs/dpn.py` & `trojanzoo-2.0.0/trojanvision/utils/model_archs/dpn.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/utils/model_archs/enas/macro.py` & `trojanzoo-2.0.0/trojanvision/utils/model_archs/enas/macro.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/utils/model_archs/enas/mutables.py` & `trojanzoo-2.0.0/trojanvision/utils/model_archs/enas/mutables.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,18 +62,18 @@
         raise NotImplementedError("Deep copy doesn't work for mutables.")
 
     def __call__(self, *args, **kwargs):
         self._check_built()
         return super().__call__(*args, **kwargs)
 
     def set_mutator(self, mutator):
-        if "mutator" in self.__dict__:
+        if "mutator" in vars(self):
             raise RuntimeError("`set_mutator` is called more than once. Did you parse the search space multiple times? "
                                "Or did you apply multiple fixed architectures?")
-        self.__dict__["mutator"] = mutator
+        vars(self)["mutator"] = mutator
 
     @property
     def key(self):
         """
         Read-only property of key.
         """
         return self._key
```

### Comparing `trojanzoo-1.1.1/trojanvision/utils/model_archs/enas/ops.py` & `trojanzoo-2.0.0/trojanvision/utils/model_archs/enas/ops.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/utils/model_archs/lanet.py` & `trojanzoo-2.0.0/trojanvision/utils/model_archs/lanet.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/utils/model_archs/pnasnet.py` & `trojanzoo-2.0.0/trojanvision/utils/model_archs/pnasnet.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/utils/model_archs/resnet_ap.py` & `trojanzoo-2.0.0/trojanvision/utils/model_archs/resnet_ap.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/utils/model_archs/resnet_s.py` & `trojanzoo-2.0.0/trojanvision/utils/model_archs/resnet_s.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/utils/sgm.py` & `trojanzoo-2.0.0/trojanvision/utils/sgm.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanvision/utils/transform.py` & `trojanzoo-2.0.0/trojanvision/utils/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     def __repr__(self) -> str:
         s = self.__class__.__name__ + "("
         s += "num_classes={num_classes}"
         s += ", p={p}"
         s += ", alpha={alpha}"
         s += ", inplace={inplace}"
         s += ")"
-        return s.format(**self.__dict__)
+        return s.format(**vars(self))
 
 
 class RandomCutmix(nn.Module):
     """Randomly apply Cutmix to the provided batch and targets.
     The class implements the data augmentations as described in the paper
     `"CutMix: Regularization Strategy to Train Strong Classifiers with Localizable Features"
     <https://arxiv.org/abs/1905.04899>`_.
@@ -188,15 +188,15 @@
     def __repr__(self) -> str:
         s = self.__class__.__name__ + "("
         s += "num_classes={num_classes}"
         s += ", p={p}"
         s += ", alpha={alpha}"
         s += ", inplace={inplace}"
         s += ")"
-        return s.format(**self.__dict__)
+        return s.format(**vars(self))
 
 
 def cutout(img: torch.Tensor, length: int | tuple[int, int] | torch.Tensor,
            fill_values: float | torch.Tensor = 0.0) -> torch.Tensor:
     if isinstance(length, int):
         length = (length, length)
     h, w = img.size(-2), img.size(-1)
```

### Comparing `trojanzoo-1.1.1/trojanzoo/attacks.py` & `trojanzoo-2.0.0/trojanzoo/attacks.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanzoo/configs/__init__.py` & `trojanzoo-2.0.0/trojanzoo/configs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,19 +198,19 @@
                     if ext in ['.yml', '.yaml', 'json']:
                         _dict.update(Config.load_config(file_path))
             return _dict
         elif os.path.isfile(path):
             name, ext = os.path.splitext(os.path.split(path)[1])
             if ext in ['.yml', 'yaml', 'json']:
                 with open(path, 'r', encoding='utf-8') as f:
-                    _dict: dict[str, Any | dict[str, Any]] = {}
                     if ext == 'json':
                         _dict = json.load(f.read())
                     else:
                         _dict = yaml.load(f.read(), Loader=yaml.FullLoader)
+                    _dict = _dict or {}
                     return Module(**{name: Config.organize_config_file(_dict)})
             else:
                 return Module()
         else:
             raise Exception(f'unknown: {path}')
 
     @staticmethod
```

### Comparing `trojanzoo-1.1.1/trojanzoo/datasets.py` & `trojanzoo-2.0.0/trojanzoo/datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     Note:
         This is the implementation of dataset.
         For users, please use :func:`create` instead, which is more user-friendly.
 
     Args:
         batch_size (int): Batch size of training set
             (negative number means batch size for each gpu).
+            Defaults to ``100``.
         valid_batch_size (int): Batch size of validation set.
             Defaults to ``100``.
         folder_path (str): Folder path to store dataset.
             Defaults to ``None``.
 
             Note:
                 :attr:`folder_path` is usually
@@ -61,14 +62,15 @@
 
     Attributes:
         name (str): Dataset Name. (need overriding)
         loader(dict[str, ~torch.utils.data.DataLoader]):
             | Preset dataloader for users at dataset initialization.
             | It contains ``'train'`` and ``'valid'`` loaders.
         batch_size (int): Batch size of training set (always positive).
+            Defaults to ``100``.
         valid_batch_size (int): Batch size of validation set.
             Defaults to ``100``.
         num_classes (int): Number of classes. (need overriding)
         folder_path (str): Folder path to store dataset.
             Defaults to ``None``.
 
         data_type (str): Data type (e.g., ``'image'``). (need overriding)
@@ -116,27 +118,27 @@
                            'torch.utils.data.DataLoader (default: 4)')
         group.add_argument('--download', action='store_true',
                            help='download dataset if not exist by calling '
                            'self.initialize()')
         group.add_argument('--data_dir', help='directory to contain datasets')
         return group
 
-    def __init__(self, batch_size: int = None,
+    def __init__(self, batch_size: int = 100,
                  valid_batch_size: int = 100,
                  folder_path: str = None, download: bool = False,
                  split_ratio: float = 0.8, num_workers: int = 4,
                  loss_weights: bool | np.ndarray | torch.Tensor = False,
                  **kwargs):
         super().__init__(**kwargs)
         self.param_list['dataset'] = ['num_classes', 'batch_size', 'valid_batch_size',
                                       'folder_path', 'num_workers', ]
         if not self.valid_set:
             self.param_list['dataset'].append('split_ratio')
         self.__batch_size = batch_size
-        self.valid_batch_size = valid_batch_size
+        self.__valid_batch_size = valid_batch_size
         self.split_ratio = split_ratio
         self.num_workers = num_workers
         self.collate_fn: Callable[[Iterable[torch.Tensor]], Iterable[torch.Tensor]] = None
         # ----------------------------------------------- #
 
         if folder_path is not None:
             folder_path = os.path.normpath(folder_path)
@@ -169,14 +171,19 @@
         self.loss_weights: None | torch.Tensor = loss_weights
 
     @functools.cached_property
     def batch_size(self):
         return self.__batch_size if self.__batch_size >= 0 else \
             -self.__batch_size * max(1, env['num_gpus'])
 
+    @functools.cached_property
+    def valid_batch_size(self):
+        return self.__valid_batch_size if self.__valid_batch_size >= 0 else \
+            -self.__valid_batch_size * max(1, env['num_gpus'])
+
     # TODO: should it be abstractmethod?
     def initialize(self, *args, **kwargs):
         r"""Initialize the dataset (download and extract) if it's not prepared yet
         (need overriding).
         """
         raise NotImplementedError()
 
@@ -397,20 +404,18 @@
                 if :attr:`dataset` is not provided.
 
         Returns:
             torch.utils.data.DataLoader: The pytorch dataloader.
         """
         if batch_size is None:
             match mode:
-                case 'train':
-                    batch_size = self.batch_size
                 case 'valid':
                     batch_size = self.valid_batch_size
                 case _:
-                    raise ValueError(f'{mode=}')
+                    batch_size = self.batch_size
         if shuffle is None:
             shuffle = (mode == 'train')
         if num_workers is None:
             num_workers = self.num_workers
         if dataset is None:
             dataset = self.get_dataset(mode=mode, **kwargs)
         pin_memory = pin_memory and env['num_gpus']
```

### Comparing `trojanzoo-1.1.1/trojanzoo/defenses.py` & `trojanzoo-2.0.0/trojanzoo/defenses.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanzoo/environ.py` & `trojanzoo-2.0.0/trojanzoo/environ.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,22 @@
         group.add_argument('--tqdm', action='store_true',
                            help='show tqdm progress bar')
         return group
 
     def __init__(self, *args, device: str = 'auto', **kwargs):
         super().__init__(*args, device=device, **kwargs)
 
+    def set_seed(self, seed: int = None):
+        if seed is None:
+            seed = self['seed']
+        random.seed(seed)
+        np.random.seed(seed)
+        torch.manual_seed(seed)
+        torch.cuda.manual_seed_all(seed)
+
 
 env = Env(default=None)
 
 
 def add_argument(parser: argparse.ArgumentParser) -> argparse._ArgumentGroup:
     r"""
     | Add environ arguments to argument parser.
@@ -114,15 +122,15 @@
     env.add_argument(group)
     return group
 
 
 def create(cmd_config_path: str = None, dataset_name: str = None, dataset: str = None,
            seed: int = None, data_seed: int = None, cudnn_benchmark: bool = None,
            config: Config = config,
-           cache_threshold: float = None, verbose: int = 0,
+           cache_threshold: float = None, verbose: int = None,
            color: bool = None, device: str | int | torch.device = None, tqdm: bool = None,
            **kwargs) -> Env:
     r"""
     | Load :attr:`env` values from config and command line.
 
     Args:
         dataset_name (str): The dataset name.
@@ -135,31 +143,30 @@
         config (Config): The default parameter config.
         **kwargs: The keyword arguments in keys of
             ``['optim_args', 'train_args', 'writer_args']``.
 
     Returns:
         Env: The :attr:`env` instance.
     """
+    if verbose is None:
+        verbose = 0
     other_kwargs = {'data_seed': data_seed, 'cache_threshold': cache_threshold,
                     'verbose': verbose, 'color': color, 'device': device, 'tqdm': tqdm}
     config.cmd_config_path = cmd_config_path
     dataset_name = get_name(
         name=dataset_name, module=dataset, arg_list=['-d', '--dataset'])
     dataset_name = dataset_name if dataset_name is not None \
         else config.full_config['dataset']['default_dataset']
     result = config.get_config(dataset_name=dataset_name)[
         'env'].update(other_kwargs)
     env.clear().update(**result)
     ansi.switch(env['color'])
     if seed is None and 'seed' in env.keys():
         seed = env['seed']
-    random.seed(seed)
-    np.random.seed(seed)
-    torch.manual_seed(seed)
-    torch.cuda.manual_seed_all(seed)
+    env.set_seed(seed)
 
     num_gpus: int = torch.cuda.device_count()
     device: str | int | torch.device = result['device']
     if device is None:
         device = 'auto'
     match device:
         case torch.device():
```

### Comparing `trojanzoo-1.1.1/trojanzoo/models.py` & `trojanzoo-2.0.0/trojanzoo/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from typing import TYPE_CHECKING
 # TODO: python 3.10
 from typing import Generator, Iterator, Mapping
 from trojanzoo.configs import Config    # TODO: python 3.10
 from trojanzoo.utils.model import ExponentialMovingAverage
 from torch.optim.optimizer import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler
+from torchvision.models._api import WeightsEnum
 import argparse
 from collections.abc import Callable
 if TYPE_CHECKING:
     import torch.utils.data
 
 __all__ = ['_Model', 'Model',
            'add_argument', 'create',
@@ -204,16 +205,16 @@
         randomized_smooth (bool): Whether to use randomized smoothing.
             Defaults to ``False``.
         rs_sigma (float): Randomized smoothing sampling std :math:`\sigma`.
             Defaults to ``0.01``.
         rs_n (int): Randomized smoothing sampling number. Defaults to ``100``.
 
     Attributes:
-        available_models (list[str]): The list of available model names.
-        model_urls (dict[str, str]): The links to official pretrained model weights.
+        available_models (set[str]): The list of available model names.
+        weights (~torchvision.models._api.WeightsEnum): The pretrained weights to use.
 
         name (str): Name of model.
         suffix (str):
             | Suffix of local model weights file (e.g., ``'_adv_train'``).
               Defaults to empty string ``''``.
             | The location of local pretrained weights is
               ``'{folder_path}/{self.name}{self.suffix}.pth'``
@@ -238,16 +239,16 @@
         criterion_noreduction (~collections.abc.Callable):
             The criterion used to calculate :meth:`loss()`
             when ``reduction='none'``.
         softmax (torch.nn.Module): :any:`torch.nn.Softmax` ``(dim=1)``.
             Used in :meth:`get_prob()`.
     """
 
-    available_models: list[str] = []
-    model_urls: dict[str, str] = []
+    available_models: set[str] = set()
+    weights: dict[str, WeightsEnum] = None
 
     @staticmethod
     def add_argument(group: argparse._ArgumentGroup) -> argparse._ArgumentGroup:
         r"""Add model arguments to argument parser group.
         View source to see specific arguments.
 
         Note:
@@ -930,38 +931,42 @@
         _dict: OrderedDict[str, torch.Tensor] = module.state_dict(
             prefix=component)
         torch.save(_dict, file_path, **kwargs)
         if verbose:
             prints(
                 f'Model {self.name} saved at: {file_path}', indent=indent)
 
-    def get_official_weights(self, url: str = None,
+    def get_official_weights(self, weights: WeightsEnum | None = None,
+                             progress: bool = True,
                              map_location: str | Callable | torch.device | dict = 'cpu',
                              **kwargs) -> OrderedDict[str, torch.Tensor]:
-        r"""Get official model weights from :attr:`url`.
+        r"""Get official model weights from :attr:`weights`.
 
         Args:
-            url (str | None): The link to model weights.
-                Defaults to :attr:`self.model_urls[self.name]`.
+            weights (~torchvision.models._api.WeightsEnum | None):
+                The pretrained weights to use.
+                Defaults to :attr:`self.weights[self.name]`.
             map_location (str | ~torch.torch.device | dict):
                 Passed to :any:`torch.hub.load_state_dict_from_url`.
                 Defaults to ``'cpu'``.
             **kwargs: Keyword arguments passed to
                 :any:`torch.hub.load_state_dict_from_url`.
 
         Returns:
             OrderedDict[str, torch.Tensor]: The model weights OrderedDict.
         """
-        url = self.model_urls[self.name] if url is None else url
-        print('get official model weights from: ', url)
-        return torch.hub.load_state_dict_from_url(url, map_location=map_location, **kwargs)
+        if weights is None:
+            weights = getattr(self.weights, self.name)
+        return weights.get_state_dict(progress=progress, check_hash=True,
+                                      map_location=map_location, **kwargs)
 
     # ---------------------Train and Validate--------------------- #
     # TODO: annotation and remove those arguments to be *args, **kwargs
     def _train(self, epochs: int, optimizer: Optimizer,
+               module: nn.Module = None, num_classes: int = None,
                lr_scheduler: _LRScheduler = None,
                lr_warmup_epochs: int = 0,
                model_ema: ExponentialMovingAverage = None,
                model_ema_steps: int = 32,
                grad_clip: float = None, pre_conditioner: None | KFAC | EKFAC = None,
                print_prefix: str = 'Train', start_epoch: int = 0, resume: int = 0,
                validate_interval: int = 10, save: bool = False, amp: bool = False,
@@ -975,29 +980,30 @@
                validate_fn: Callable[..., tuple[float, float]] = None,
                save_fn: Callable[..., None] = None, file_path: str = None,
                folder_path: str = None, suffix: str = None,
                writer=None, main_tag: str = 'train', tag: str = '',
                accuracy_fn: Callable[..., list[float]] = None,
                verbose: bool = True, indent: int = 0, **kwargs):
         r"""Train the model"""
-        loader_train = loader_train if loader_train is not None \
-            else self.dataset.loader['train']
+        module = module or self._model
+        num_classes = num_classes or self.num_classes
+        loader_train = loader_train or self.dataset.loader['train']
         get_data_fn = get_data_fn if callable(get_data_fn) else self.get_data
         loss_fn = loss_fn if callable(loss_fn) else self.loss
         validate_fn = validate_fn if callable(validate_fn) else self._validate
         save_fn = save_fn if callable(save_fn) else self.save
         accuracy_fn = accuracy_fn if callable(accuracy_fn) else self.accuracy
         kwargs['forward_fn'] = kwargs.get('forward_fn', self.__call__)
         # if not callable(iter_fn) and hasattr(self, 'iter_fn'):
         #     iter_fn = getattr(self, 'iter_fn')
         if not callable(epoch_fn) and hasattr(self, 'epoch_fn'):
             epoch_fn = getattr(self, 'epoch_fn')
         if not callable(after_loss_fn) and hasattr(self, 'after_loss_fn'):
             after_loss_fn = getattr(self, 'after_loss_fn')
-        return train(module=self._model, num_classes=self.num_classes,
+        return train(module=module, num_classes=num_classes,
                      epochs=epochs, optimizer=optimizer, lr_scheduler=lr_scheduler,
                      lr_warmup_epochs=lr_warmup_epochs,
                      model_ema=model_ema, model_ema_steps=model_ema_steps,
                      grad_clip=grad_clip, pre_conditioner=pre_conditioner,
                      print_prefix=print_prefix, start_epoch=start_epoch,
                      resume=resume, validate_interval=validate_interval,
                      save=save, amp=amp,
@@ -1023,16 +1029,16 @@
                   accuracy_fn: Callable[..., list[float]] = None,
                   **kwargs) -> tuple[float, float]:
         r"""Evaluate the model.
 
         Returns:
             (float, float): Accuracy and loss.
         """
-        module = self._model if module is None else module
-        num_classes = self.num_classes if num_classes is None else num_classes
+        module = module or self._model
+        num_classes = num_classes or self.num_classes
         loader = loader or self.dataset.loader['valid']
         get_data_fn = get_data_fn or self.get_data
         loss_fn = loss_fn or self.loss
         accuracy_fn = accuracy_fn if callable(accuracy_fn) else self.accuracy
         kwargs['forward_fn'] = kwargs.get('forward_fn', self.__call__)
         return validate(module=module, num_classes=num_classes, loader=loader,
                         print_prefix=print_prefix,
@@ -1490,15 +1496,15 @@
     for k in sorted(names_dict.keys()):
         prints('{yellow}{k}{reset}'.format(k=k, **ansi), indent=indent)
         prints(names_dict[k], indent=indent + 10)
         print()
 
 
 def get_available_models(class_dict: dict[str, type[Model]] = {}
-                         ) -> dict[str, list[str]]:
+                         ) -> dict[str, set[str]]:
     return {k: v.available_models for k, v in class_dict.items()}
 
 
 def get_model_class(name: str, class_dict: dict[str, type[Model]] = {}) -> str:
     correct_name: str = None
     for class_name in class_dict.keys():
         if class_name in name.lower() and \
```

### Comparing `trojanzoo-1.1.1/trojanzoo/optim.py` & `trojanzoo-2.0.0/trojanzoo/optim/optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
             current_loss_kwargs = {k: v[current_idx]
                                    for k, v in loss_kwargs.items()}
             loss_values = loss_fn(
                 adv_input[current_idx], **current_loss_kwargs)
         assert loss_values.dim() == 1
         if adv_input[current_idx] is not None:
             assert len(loss_values) == len(current_idx)
-        return loss_values < stop_threshold
+        return loss_values.detach().cpu() < stop_threshold
 
     def output_info(self, *args, mode: str = 'start',
                     _iter: int = 0, iteration: int = 0,
                     output: Iterable[str] = None, indent: int = None,
                     **kwargs):
         r"""Output information.
```

### Comparing `trojanzoo-1.1.1/trojanzoo/trainer.py` & `trojanzoo-2.0.0/trojanzoo/trainer.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanzoo/utils/data.py` & `trojanzoo-2.0.0/trojanzoo/utils/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
         >>> dataset = TensorListDataset(data, targets)
         >>> subset = get_class_subset(dataset, class_list=[2, 3])
         >>> len(subset)
         2
     """
     class_list = [class_list] if isinstance(class_list, int) else class_list
     indices = np.arange(len(dataset))
-    if isinstance(dataset, Subset):
+    while isinstance(dataset, Subset):
         idx = np.array(dataset.indices)
         indices = idx[indices]
         dataset = dataset.dataset
     _, targets = dataset_to_tensor(dataset=dataset)
     idx_bool = np.isin(targets.numpy(), class_list)
     idx = np.arange(len(dataset))[idx_bool]
     idx = np.intersect1d(idx, indices)
```

### Comparing `trojanzoo-1.1.1/trojanzoo/utils/fim/ekfac.py` & `trojanzoo-2.0.0/trojanzoo/utils/fim/ekfac.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanzoo/utils/fim/fim.py` & `trojanzoo-2.0.0/trojanzoo/utils/fim/fim.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 import torch
 import torch.nn as nn
-from torch.nn.utils import _stateless
+from torch.nn.utils import stateless
 
 from typing import Iterable
 
 
 def fim_diag(module: nn.Module, _input: torch.Tensor,
              parameters: Iterable[nn.Parameter] = None
              ) -> list[torch.Tensor]:
@@ -77,15 +77,15 @@
     keys, values = zip(*parameters.items())
 
     with torch.no_grad():
         _output: torch.Tensor = module(_input)  # (N, C)
         prob = _output.softmax(dim=1).unsqueeze(-1).unsqueeze(-1)  # (N, C, 1, 1)
 
     def func(*params: torch.Tensor):
-        _output: torch.Tensor = _stateless.functional_call(
+        _output: torch.Tensor = stateless.functional_call(
             module, {n: p for n, p in zip(keys, params)}, _input)
         return _output.log_softmax(dim=1)  # (N, C)
     jac: tuple[torch.Tensor] = torch.autograd.functional.jacobian(
         func, values)
     jac = (j.flatten(2) for j in jac)   # (N, C, D)
 
     fim_list: list[torch.Tensor] = []
```

### Comparing `trojanzoo-1.1.1/trojanzoo/utils/fim/kfac.py` & `trojanzoo-2.0.0/trojanzoo/utils/fim/kfac.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanzoo/utils/lock.py` & `trojanzoo-2.0.0/trojanzoo/utils/lock.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanzoo/utils/logger.py` & `trojanzoo-2.0.0/trojanzoo/utils/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -302,29 +302,30 @@
         if strip:
             _str = _str.rstrip()
         return _str
 
     def __getattr__(self, attr: str) -> float:
         if attr in self.meters:
             return self.meters[attr]
-        if attr in self.__dict__:   # TODO: use hasattr
-            return self.__dict__[attr]
+        if attr in vars(self):   # TODO: use hasattr
+            return vars(self)[attr]
         raise AttributeError("'{}' object has no attribute '{}'".format(
             type(self).__name__, attr))
 
     def __str__(self) -> str:
         return self.get_str(**self.meters)
 
     def synchronize_between_processes(self):
         for meter in self.meters.values():
             meter.synchronize_between_processes()
 
     def log_every(self, iterable: Iterable[_T], header: str = '',
                   tqdm: bool = None, tqdm_header: str = 'Iter',
-                  indent: int = None) -> Generator[_T, None, None]:
+                  indent: int = None, verbose: int = None
+                  ) -> Generator[_T, None, None]:
         r"""Wrap an :class:`collections.abc.Iterable` with formatted outputs.
 
         * Middle Output:
           ``{tqdm_header}: [ current / total ] str(self) {memory} {iter_time} {data_time} {time}<{remaining}``
         * Final Output
           ``{header} str(self) {memory} {iter_time} {data_time} {total_time}``
 
@@ -335,20 +336,24 @@
             tqdm (bool): Whether to use tqdm to show iteration information.
                 Defaults to ``self.tqdm``.
             tqdm_header (str): The header string for middle output.
                 Defaults to ``'Iter'``.
             indent (int): The space indent for the entire string.
                 if ``None``, use ``self.indent``.
                 Defaults to ``None``.
+            verbose (int): The verbose level of output information.
+                Defaults to ``env[verbose]``
 
         :Example:
             .. seealso:: :func:`trojanzoo.utils.train.train()`
         """
         tqdm = tqdm if tqdm is not None else self.tqdm
         indent = indent if indent is not None else self.indent
+        if verbose is None:
+            verbose = env['verbose']
         iterator = iterable
         if len(header) != 0:
             header = header.ljust(30 + get_ansi_len(header))
         if tqdm:
             length = len(str(len(iterable)))
             pattern: str = ('{tqdm_header}: {blue_light}'
                             '[ {red}{{n_fmt:>{length}}}{blue_light} '
@@ -373,29 +378,29 @@
             cur_iter_time = time.time() - end
             self.iter_time.update(cur_iter_time)
             if torch.cuda.is_available():
                 cur_memory = torch.cuda.max_memory_allocated() / MB
                 self.memory.update(cur_memory)
             if tqdm:
                 _dict = {k: v for k, v in self.meters.items()}
-                if env['verbose'] > 2 and torch.cuda.is_available():
+                if verbose > 2 and torch.cuda.is_available():
                     _dict.update(memory=f'{cur_memory:.0f} MB')
-                if env['verbose'] > 1:
+                if verbose > 1:
                     _dict.update(iter=f'{cur_iter_time:.3f} s',
                                  data=f'{cur_data_time:.3f} s')
                 iterator.set_description_str(self.get_str(**_dict, strip=False))
             end = time.time()
         self.synchronize_between_processes()
         total_time = time.time() - start_time
         total_time_str = tqdm_class.format_interval(total_time)
 
         _dict = {k: v for k, v in self.meters.items()}
-        if env['verbose'] > 2 and torch.cuda.is_available():
+        if verbose > 2 and torch.cuda.is_available():
             _dict.update(memory=f'{str(self.memory)} MB')
-        if env['verbose'] > 1:
+        if verbose > 1:
             _dict.update(iter=f'{str(self.iter_time)} s',
                          data=f'{str(self.data_time)} s')
         _dict.update(time=total_time_str)
         prints(self.delimiter.join([header, self.get_str(**_dict)]),
                indent=indent)
 
 
@@ -424,8 +429,8 @@
         self.val = val
         self.sum += val * n
         self.count += n
         self.avg = self.sum / self.count
 
     def __str__(self):
         fmtstr = '{name} {val' + self.fmt + '} ({avg' + self.fmt + '})'
-        return fmtstr.format(**self.__dict__)
+        return fmtstr.format(**vars(self))
```

### Comparing `trojanzoo-1.1.1/trojanzoo/utils/memory.py` & `trojanzoo-2.0.0/trojanzoo/utils/memory.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanzoo/utils/metric.py` & `trojanzoo-2.0.0/trojanzoo/utils/metric.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,10 +32,11 @@
 
 
 def mask_jaccard(mask: torch.Tensor, real_mask: torch.Tensor,
                  select_num: int = 9) -> float:
     mask = mask.float()
     real_mask = real_mask.float()
     detect_mask = mask > mask.flatten().topk(select_num)[0][-1]
+    real_mask = real_mask > real_mask.flatten().topk(select_num)[0][-1]
     sum_temp = detect_mask.int() + real_mask.int()
     overlap = (sum_temp == 2).sum().float() / (sum_temp >= 1).sum().float()
     return float(overlap)
```

### Comparing `trojanzoo-1.1.1/trojanzoo/utils/model.py` & `trojanzoo-2.0.0/trojanzoo/utils/model.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanzoo/utils/module/__init__.py` & `trojanzoo-2.0.0/trojanzoo/utils/module/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanzoo/utils/module/param.py` & `trojanzoo-2.0.0/trojanzoo/utils/module/param.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
             regard it as the default value.
         **kwargs: Keyword arguments that compose a dict.
             All keys will be merged together.
 
     Attributes:
         _marker (str): The marker of the class,
             which is shown in ``str(self)``.
-            Defaults to ``'M'``.
+            Defaults to ``'P'``.
         default (Any): The default value of unknown keys.
     """
     _marker = 'P'
 
     def update(self, *args: dict[_KT, _VT], **kwargs: _VT):
         if len(kwargs) == 0 and len(args) == 1 and \
                 not isinstance(args[0], (dict, Module)):
```

### Comparing `trojanzoo-1.1.1/trojanzoo/utils/module/process.py` & `trojanzoo-2.0.0/trojanzoo/utils/module/process.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanzoo/utils/ntk/__init__.py` & `trojanzoo-2.0.0/trojanzoo/utils/ntk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 # https://pytorch.org/functorch/nightly/notebooks/neural_tangent_kernels.html
 
 import torch
 import torch.nn as nn
-from torch.nn.utils import _stateless
+from torch.nn.utils import stateless
 
 import functools
 
 from typing import Iterable
 
 
 def empirical_ntk(module: nn.Module, input1: torch.Tensor, input2: torch.Tensor,
@@ -32,15 +32,15 @@
             param, torch.nn.Parameter) else param]: param
             for param in parameters}
     if parameters is None:
         parameters = dict(module.named_parameters())
     names, values = zip(*parameters.items())
 
     def func(*params: torch.Tensor, _input: torch.Tensor = None):
-        _output: torch.Tensor = _stateless.functional_call(
+        _output: torch.Tensor = stateless.functional_call(
             module, {n: p for n, p in zip(names, params)}, _input)
         return _output  # (N, C)
 
     jac1: tuple[torch.Tensor] = torch.autograd.functional.jacobian(
         functools.partial(func, _input=input1), values)
     jac2: tuple[torch.Tensor] = torch.autograd.functional.jacobian(
         functools.partial(func, _input=input2), values)
```

### Comparing `trojanzoo-1.1.1/trojanzoo/utils/output.py` & `trojanzoo-2.0.0/trojanzoo/utils/output.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanzoo/utils/tensor.py` & `trojanzoo-2.0.0/trojanzoo/utils/tensor.py`

 * *Files identical despite different names*

### Comparing `trojanzoo-1.1.1/trojanzoo/utils/train.py` & `trojanzoo-2.0.0/trojanzoo/utils/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         amp = False
     if amp:
         scaler = torch.cuda.amp.GradScaler()
     best_validate_result = (0.0, float('inf'))
     if validate_interval != 0:
         best_validate_result = validate_fn(loader=loader_valid, get_data_fn=get_data_fn,
                                            forward_fn=forward_fn, loss_fn=loss_fn,
-                                           writer=None, tag=tag, _epoch=start_epoch,
+                                           writer=writer, tag=tag, _epoch=start_epoch,
                                            verbose=verbose, indent=indent, **kwargs)
         best_acc = best_validate_result[0]
 
     params: list[nn.Parameter] = []
     for param_group in optimizer.param_groups:
         params.extend(param_group['params'])
     len_loader_train = len(loader_train)
```

### Comparing `trojanzoo-1.1.1/trojanzoo.egg-info/PKG-INFO` & `trojanzoo-2.0.0/trojanzoo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trojanzoo
-Version: 1.1.1
+Version: 2.0.0
 Summary: a universal pytorch platform to conduct security researches
 Home-page: https://github.com/ain-soph/trojanzoo
 Author: Ren Pang
 Author-email: rbp5354@psu.edu
 License: GPL-3
 Keywords: pytorch,image classification,backdoor attack/defense
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.3
@@ -30,15 +30,15 @@
 [![docs](https://github.com/ain-soph/trojanzoo/workflows/docs/badge.svg)](https://ain-soph.github.io/trojanzoo/)
 
 [![release](https://img.shields.io/github/v/release/ain-soph/trojanzoo)](https://github.com/ain-soph/trojanzoo/releases)
 [![pypi](https://img.shields.io/pypi/v/trojanzoo)](https://pypi.org/project/trojanzoo/)
 [![docker](https://img.shields.io/pypi/v/trojanzoo?label=docker)](https://hub.docker.com/r/local0state/trojanzoo)
 <!-- [![conda](https://img.shields.io/pypi/v/trojanzoo?label=conda)](https://anaconda.org/anaconda/trojanzoo) -->
 
-> **NOTE:** TrojanZoo requires `python>=3.10`, `pytorch>=1.11` and `torchvision>=0.12`, which must be installed manually. Recommend to use `conda` to install.
+> **NOTE:** TrojanZoo requires `python>=3.10`, `pytorch>=1.12.1` and `torchvision>=0.13.1`, which must be installed manually. Recommend to use `conda` to install.
 
 This is the code implementation (pytorch) for our paper in EuroS&P 2022:  
 [TrojanZoo: Towards Unified, Holistic, and Practical Evaluation of Neural Backdoors](https://arxiv.org/abs/2012.09302)
 
 TrojanZoo provides a universal pytorch platform to conduct security researches (especially backdoor attacks/defenses) of image classification in deep learning. It is composed of two packages: `trojanzoo` and `trojanvision`. `trojanzoo` contains abstract classes and utilities, while `trojanvision` contains abstract and concrete ones for image classification task. 
 
 > Note: This repository is also maintained to cover the implementation of
```

### Comparing `trojanzoo-1.1.1/trojanzoo.egg-info/SOURCES.txt` & `trojanzoo-2.0.0/trojanzoo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -117,33 +117,36 @@
 trojanvision/configs/defense/fine_pruning.yml
 trojanvision/configs/defense/image_transform.yml
 trojanvision/configs/defense/neo.yml
 trojanvision/configs/defense/neuron_inspect.yml
 trojanvision/configs/defense/spectral_signature.yml
 trojanvision/data/cub200/test.txt
 trojanvision/data/cub200/train.txt
-trojanvision/data/cub200_2011/image_class_labels.txt
+trojanvision/data/cub200_2011/images.txt
 trojanvision/data/cub200_2011/train_test_split.txt
 trojanvision/data/isic2018/train.csv
 trojanvision/data/isic2018/valid.csv
 trojanvision/data/refool/insert_reflection.py
 trojanvision/data/sample_imagenet/class_dict.json
+trojanvision/data/stl10/unlabeled_y.bin
 trojanvision/datasets/__init__.py
 trojanvision/datasets/imagefolder.py
 trojanvision/datasets/imageset.py
 trojanvision/datasets/folder/__init__.py
 trojanvision/datasets/folder/cub200.py
 trojanvision/datasets/folder/gtsrb.py
 trojanvision/datasets/folder/imagenet.py
 trojanvision/datasets/folder/isic.py
 trojanvision/datasets/folder/vggface2.py
 trojanvision/datasets/normal/__init__.py
+trojanvision/datasets/normal/celeba.py
 trojanvision/datasets/normal/cifar.py
 trojanvision/datasets/normal/downsampled_imagenet.py
 trojanvision/datasets/normal/mnist.py
+trojanvision/datasets/normal/stl10.py
 trojanvision/defenses/__init__.py
 trojanvision/defenses/abstract.py
 trojanvision/defenses/adv/__init__.py
 trojanvision/defenses/adv/advmind.py
 trojanvision/defenses/adv/curvature.py
 trojanvision/defenses/adv/grad_train.py
 trojanvision/defenses/backdoor/__init__.py
@@ -195,31 +198,21 @@
 trojanvision/models/torchvision/densenet.py
 trojanvision/models/torchvision/efficientnet.py
 trojanvision/models/torchvision/mnasnet.py
 trojanvision/models/torchvision/mobilenet.py
 trojanvision/models/torchvision/resnet.py
 trojanvision/models/torchvision/shufflenetv2.py
 trojanvision/models/torchvision/vgg.py
-trojanvision/optim/__init__.py
-trojanvision/optim/pgd.py
-trojanvision/optim/uname.py
 trojanvision/shortcut/__init__.py
 trojanvision/shortcut/pgd.py
 trojanvision/utils/__init__.py
 trojanvision/utils/dataset.py
 trojanvision/utils/model.py
 trojanvision/utils/sgm.py
 trojanvision/utils/transform.py
-trojanvision/utils/autoaugment/__init__.py
-trojanvision/utils/autoaugment/functional.py
-trojanvision/utils/autoaugment/functional_pil.py
-trojanvision/utils/autoaugment/functional_tensor.py
-trojanvision/utils/autoaugment/operations.py
-trojanvision/utils/autoaugment/policy.py
-trojanvision/utils/autoaugment/wgan.py
 trojanvision/utils/datasets/__init__.py
 trojanvision/utils/datasets/downsampled_imagenet.py
 trojanvision/utils/model_archs/__init__.py
 trojanvision/utils/model_archs/bit.py
 trojanvision/utils/model_archs/dla.py
 trojanvision/utils/model_archs/dpn.py
 trojanvision/utils/model_archs/lanet.py
@@ -238,15 +231,14 @@
 trojanvision/utils/model_archs/enas/ops.py
 trojanzoo/__init__.py
 trojanzoo/attacks.py
 trojanzoo/datasets.py
 trojanzoo/defenses.py
 trojanzoo/environ.py
 trojanzoo/models.py
-trojanzoo/optim.py
 trojanzoo/trainer.py
 trojanzoo/version.py
 trojanzoo.egg-info/PKG-INFO
 trojanzoo.egg-info/SOURCES.txt
 trojanzoo.egg-info/dependency_links.txt
 trojanzoo.egg-info/not-zip-safe
 trojanzoo.egg-info/requires.txt
@@ -254,14 +246,18 @@
 trojanzoo/configs/__init__.py
 trojanzoo/configs/attack.yml
 trojanzoo/configs/dataset.yml
 trojanzoo/configs/defense.yml
 trojanzoo/configs/env.yml
 trojanzoo/configs/model.yml
 trojanzoo/configs/trainer.yml
+trojanzoo/optim/__init__.py
+trojanzoo/optim/optimizer.py
+trojanzoo/optim/pgd.py
+trojanzoo/optim/uname.py
 trojanzoo/utils/__init__.py
 trojanzoo/utils/data.py
 trojanzoo/utils/lock.py
 trojanzoo/utils/logger.py
 trojanzoo/utils/memory.py
 trojanzoo/utils/metric.py
 trojanzoo/utils/model.py
```

