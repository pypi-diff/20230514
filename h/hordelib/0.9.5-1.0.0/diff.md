# Comparing `tmp/hordelib-0.9.5.tar.gz` & `tmp/hordelib-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hordelib-0.9.5.tar", last modified: Thu Apr 20 22:16:34 2023, max compression
+gzip compressed data, was "hordelib-1.0.0.tar", last modified: Sun May 14 14:25:47 2023, max compression
```

## Comparing `hordelib-0.9.5.tar` & `hordelib-1.0.0.tar`

### file list

```diff
@@ -1,892 +1,922 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.031641 hordelib-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-20 22:16:18.000000 hordelib-0.9.5/.changelog
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-20 22:16:18.000000 hordelib-0.9.5/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.911638 hordelib-0.9.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.927638 hordelib-0.9.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-20 22:16:18.000000 hordelib-0.9.5/.github/workflows/maintests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-20 22:16:18.000000 hordelib-0.9.5/.github/workflows/prtests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-20 22:16:18.000000 hordelib-0.9.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-04-20 22:16:18.000000 hordelib-0.9.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    23940 2023-04-20 22:16:23.000000 hordelib-0.9.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-20 22:16:18.000000 hordelib-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-20 22:16:18.000000 hordelib-0.9.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    50204 2023-04-20 22:16:34.031641 hordelib-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-04-20 22:16:18.000000 hordelib-0.9.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-20 22:16:18.000000 hordelib-0.9.5/build_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.927638 hordelib-0.9.5/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_controlnet_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_facefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_img2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_img2img_hires.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_img2img_inpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_img2img_inpaint_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_img2img_outpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_inpainting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_memory_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_stress_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_txt2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_txt2img_hires.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-20 22:16:18.000000 hordelib-0.9.5/examples/run_upscale.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.927638 hordelib-0.9.5/hordelib/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.931638 hordelib-0.9.5/hordelib/_comfyui/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.931638 hordelib-0.9.5/hordelib/_comfyui/comfy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.931638 hordelib-0.9.5/hordelib/_comfyui/comfy/cldm/
--rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/cldm/cldm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/cli_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/clip_vision.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/clip_vision_config_h.json
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/clip_vision_config_vitl.json
--rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/diffusers_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.931638 hordelib-0.9.5/hordelib/_comfyui/comfy/extra_samplers/
--rw-r--r--   0 runner    (1001) docker     (123)    38450 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/extra_samplers/uni_pc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.931638 hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/external.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/gns.py
--rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.935639 hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/models/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/models/image_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    26723 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    13168 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.939638 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.939638 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/data/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.939638 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/autoencoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.939638 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21367 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/ddim.py
--rw-r--r--   0 runner    (1001) docker     (123)    89269 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/ddpm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.943639 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66501 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/dpm_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/plms.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/sampling_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.943639 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/
--rw-r--r--   0 runner    (1001) docker     (123)    21572 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.943639 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37813 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    31860 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/openaimodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/upscaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.943639 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/distributions/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/ema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.943639 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/encoders/kornia_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/encoders/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/encoders/noise_aug_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.947639 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25198 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan.py
--rw-r--r--   0 runner    (1001) docker     (123)    22341 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan_light.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.947639 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/
--rw-r--r--   0 runner    (1001) docker     (123)   441072 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/test.png
--rw-r--r--   0 runner    (1001) docker     (123)    29024 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.947639 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.947639 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/dpt_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/sub_quadratic_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/tomesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    13187 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/model_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    23539 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/sd.py
--rw-r--r--   0 runner    (1001) docker     (123)    13673 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/sd1_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/sd1_clip_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.947639 hordelib-0.9.5/hordelib/_comfyui/comfy/sd1_tokenizer/
--rw-r--r--   0 runner    (1001) docker     (123)   524619 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/sd1_tokenizer/merges.txt
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/sd1_tokenizer/special_tokens_map.json
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/sd1_tokenizer/tokenizer_config.json
--rw-r--r--   0 runner    (1001) docker     (123)  1059962 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/sd1_tokenizer/vocab.json
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/sd2_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/sd2_clip_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.951639 hordelib-0.9.5/hordelib/_comfyui/comfy/t2i_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/t2i_adapter/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.951639 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.951639 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.955639 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/
--rw-r--r--   0 runner    (1001) docker     (123)    44849 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/HAT.py
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-ESRGAN
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-HAT
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-RealESRGAN
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SPSR
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwiftSRGAN
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-Swin2SR
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwinIR
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-lama
--rw-r--r--   0 runner    (1001) docker     (123)    17696 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-mat
--rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LaMa.py
--rw-r--r--   0 runner    (1001) docker     (123)    52744 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/MAT.py
--rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/RRDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SPSR.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SRVGG.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwiftSRGAN.py
--rw-r--r--   0 runner    (1001) docker     (123)    51124 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/Swin2SR.py
--rw-r--r--   0 runner    (1001) docker     (123)    42740 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwinIR.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13485 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.955639 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/
--rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-GFPGAN
--rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-RestoreFormer
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-codeformer
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/arcface_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    26761 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/codeformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/fused_act.py
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpgan_bilinear_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    19869 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_clean_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    24279 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/restoreformer_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    28520 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    23283 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_bilinear_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    16146 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_clean_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/upfirdn2d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.955639 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/
--rw-r--r--   0 runner    (1001) docker     (123)    25609 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.955639 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/model_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/nodes_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/nodes_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfy_extras/nodes_upscale_model.py
--rw-r--r--   0 runner    (1001) docker     (123)   118577 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/comfyui_screenshot.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.955639 hordelib-0.9.5/hordelib/_comfyui/custom_nodes/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/custom_nodes/example_node.py.example
--rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/extra_model_paths.yaml.example
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/folder_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.955639 hordelib-0.9.5/hordelib/_comfyui/input/
--rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/input/example.png
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.915638 hordelib-0.9.5/hordelib/_comfyui/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.955639 hordelib-0.9.5/hordelib/_comfyui/models/checkpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/checkpoints/put_checkpoints_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.955639 hordelib-0.9.5/hordelib/_comfyui/models/clip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/clip/put_clip_or_text_encoder_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.955639 hordelib-0.9.5/hordelib/_comfyui/models/clip_vision/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/clip_vision/put_clip_vision_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.959639 hordelib-0.9.5/hordelib/_comfyui/models/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/configs/anything_v3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/configs/v1-inference.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2_fp16.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/configs/v1-inference_fp16.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/configs/v1-inpainting-inference.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/configs/v2-inference-v.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/configs/v2-inference-v_fp32.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/configs/v2-inference.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/configs/v2-inference_fp32.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/configs/v2-inpainting-inference.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.959639 hordelib-0.9.5/hordelib/_comfyui/models/controlnet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/controlnet/put_controlnets_and_t2i_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.959639 hordelib-0.9.5/hordelib/_comfyui/models/diffusers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/diffusers/put_diffusers_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.959639 hordelib-0.9.5/hordelib/_comfyui/models/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/embeddings/put_embeddings_or_textual_inversion_concepts_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.959639 hordelib-0.9.5/hordelib/_comfyui/models/loras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/loras/put_loras_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.959639 hordelib-0.9.5/hordelib/_comfyui/models/style_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/style_models/put_t2i_style_model_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.959639 hordelib-0.9.5/hordelib/_comfyui/models/upscale_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/upscale_models/put_esrgan_and_other_upscale_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.959639 hordelib-0.9.5/hordelib/_comfyui/models/vae/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/models/vae/put_vae_here
--rw-r--r--   0 runner    (1001) docker     (123)    43981 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.959639 hordelib-0.9.5/hordelib/_comfyui/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    12637 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/notebooks/comfyui_colab.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.959639 hordelib-0.9.5/hordelib/_comfyui/output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/output/_output_images_will_be_put_here
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.959639 hordelib-0.9.5/hordelib/_comfyui/script_examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/script_examples/basic_api_example.py
--rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.959639 hordelib-0.9.5/hordelib/_comfyui/web/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.959639 hordelib-0.9.5/hordelib/_comfyui/web/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.959639 hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/
--rw-r--r--   0 runner    (1001) docker     (123)    14641 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/colorPalette.js
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/contextMenuFilter.js
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/dynamicPrompts.js
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/keybinds.js
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/nodeTemplates.js
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/noteNode.js
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/rerouteNode.js
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/slotDefaults.js
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/snapToGrid.js
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/uploadImage.js
--rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/widgetInputs.js
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/extensions/logging.js.example
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/jsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.963639 hordelib-0.9.5/hordelib/_comfyui/web/lib/
--rw-r--r--   0 runner    (1001) docker     (123)   482237 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/lib/litegraph.core.js
--rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/lib/litegraph.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.963639 hordelib-0.9.5/hordelib/_comfyui/web/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/scripts/api.js
--rw-r--r--   0 runner    (1001) docker     (123)    31674 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/scripts/app.js
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/scripts/defaultGraph.js
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/scripts/pnginfo.js
--rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/scripts/ui.js
--rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/scripts/widgets.js
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.963639 hordelib-0.9.5/hordelib/_comfyui/web/types/
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/types/comfy.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)    52898 2023-04-20 22:16:26.000000 hordelib-0.9.5/hordelib/_comfyui/web/types/litegraph.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-20 22:16:33.000000 hordelib-0.9.5/hordelib/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.963639 hordelib-0.9.5/hordelib/blip/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/blip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/blip/caption.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.963639 hordelib-0.9.5/hordelib/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/cache/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.963639 hordelib-0.9.5/hordelib/clip/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/clip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/clip/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/clip/coca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/clip/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    11991 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/clip/interrogate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.963639 hordelib-0.9.5/hordelib/clip/ranking_lists/
--rw-r--r--   0 runner    (1001) docker     (123)    80572 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/clip/ranking_lists/artists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/clip/ranking_lists/flavors.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/clip/ranking_lists/mediums.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/clip/ranking_lists/movements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/clip/ranking_lists/sites.txt
--rw-r--r--   0 runner    (1001) docker     (123)    22260 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/clip/ranking_lists/tags.txt
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/clip/ranking_lists/techniques.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/clip/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    19562 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/comfy_horde.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/config_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13844 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/horde.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/initialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22045 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/install_comfy.patch
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/install_comfy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.967639 hordelib-0.9.5/hordelib/model_database/
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_database/aitemplate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_database/blip.json
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_database/clip.json
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_database/codeformer.json
--rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_database/controlnet.json
--rw-r--r--   0 runner    (1001) docker     (123)   218801 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_database/db.json
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_database/db_dep.json
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_database/db_embeds.json
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_database/diffusers.json
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_database/esrgan.json
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_database/gfpgan.json
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_database/med_config.json
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_database/safety_checker.json
--rw-r--r--   0 runner    (1001) docker     (123)   243306 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_database/stable_diffusion.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.967639 hordelib-0.9.5/hordelib/model_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32017 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_manager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_manager/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_manager/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_manager/codeformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_manager/compvis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_manager/controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_manager/diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_manager/esrgan.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_manager/gfpgan.py
--rw-r--r--   0 runner    (1001) docker     (123)    14356 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_manager/hyper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/model_manager/safety_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.967639 hordelib-0.9.5/hordelib/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.971639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    12874 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.971639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/binary/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.971639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/canny/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/canny/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.971639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/color/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.971639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/hed/
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/install.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.971639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.971639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    22985 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.971639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.971639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py
--rw-r--r--   0 runner    (1001) docker     (123)    28960 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.971639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.975639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.975639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.975639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.975639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.975639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/
--rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)    24104 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.975639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.975639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.975639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.975639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20432 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.975639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.919638 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.975639 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.979640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.983640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.983640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_160k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_20k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_40k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_80k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.919638 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.983640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.983640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.983640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.983640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.987640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)    15999 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/swish.py
--rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.987640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22125 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)    26048 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.987640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.987640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41996 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.987640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.991640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    25196 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py
--rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.991640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/deprecated.json
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.995640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15624 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py
--rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.995640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.999640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    20867 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    25157 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.999640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/closure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py
--rw-r--r--   0 runner    (1001) docker     (123)    22532 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/iter_timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.999640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    21317 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.003640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.003640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26305 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.003640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.003640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.003640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19217 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.923638 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.003640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.007640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.007640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13100 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.007640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.007640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/base_pixel_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.007640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.007640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.007640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)    31035 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.007640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.011640 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py
--rw-r--r--   0 runner    (1001) docker     (123)    24415 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py
--rw-r--r--   0 runner    (1001) docker     (123)    18353 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    18518 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18169 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.015641 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.015641 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.015641 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.015641 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.015641 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.015641 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.015641 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.019641 hordelib-0.9.5/hordelib/nodes/facerestore/
--rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.019641 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.019641 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/align_trans.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.019641 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/retinaface/
--rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py
--rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.019641 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.019641 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.019641 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/autoanchor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/extract_ckpt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.019641 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/parsing/bisenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/parsing/parsenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/parsing/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.019641 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23302 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/utils/face_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/facerestore/facelib/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/node_clip_similarities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/node_controlnet_model_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/node_image_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/node_image_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/node_model_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/nodes/node_upscale_model_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.023641 hordelib-0.9.5/hordelib/pipeline_designs/
--rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/pipeline_designs/pipeline_controlnet.json
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/pipeline_designs/pipeline_controlnet_annotator.json
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/pipeline_designs/pipeline_image_facefix.json
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/pipeline_designs/pipeline_image_upscale.json
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/pipeline_designs/pipeline_stable_diffusion.json
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json
--rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.023641 hordelib-0.9.5/hordelib/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/pipelines/pipeline_controlnet.json
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/pipelines/pipeline_controlnet_annotator.json
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/pipelines/pipeline_image_facefix.json
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/pipelines/pipeline_image_upscale.json
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/pipelines/pipeline_stable_diffusion.json
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/pipelines/pipeline_stable_diffusion_paint.json
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/run_comfyui.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/shared_model_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.023641 hordelib-0.9.5/hordelib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.023641 hordelib-0.9.5/hordelib/utils/blip/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/utils/blip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/utils/blip/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)    41378 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/utils/blip/med.py
--rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/utils/blip/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/utils/cast.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/utils/ioredirect.py
--rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-20 22:16:18.000000 hordelib-0.9.5/hordelib/utils/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:33.927638 hordelib-0.9.5/hordelib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    50204 2023-04-20 22:16:33.000000 hordelib-0.9.5/hordelib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    49489 2023-04-20 22:16:33.000000 hordelib-0.9.5/hordelib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 22:16:33.000000 hordelib-0.9.5/hordelib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-20 22:16:33.000000 hordelib-0.9.5/hordelib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-20 22:16:33.000000 hordelib-0.9.5/hordelib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.027641 hordelib-0.9.5/images/
--rw-r--r--   0 runner    (1001) docker     (123)    71522 2023-04-20 22:16:18.000000 hordelib-0.9.5/images/test_annotator.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    36815 2023-04-20 22:16:18.000000 hordelib-0.9.5/images/test_db0.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   538159 2023-04-20 22:16:18.000000 hordelib-0.9.5/images/test_facefix.png
--rw-r--r--   0 runner    (1001) docker     (123)  1474994 2023-04-20 22:16:18.000000 hordelib-0.9.5/images/test_inpaint.png
--rw-r--r--   0 runner    (1001) docker     (123)   411844 2023-04-20 22:16:18.000000 hordelib-0.9.5/images/test_inpaint_alpha.png
--rw-r--r--   0 runner    (1001) docker     (123)    11886 2023-04-20 22:16:18.000000 hordelib-0.9.5/images/test_inpaint_mask.png
--rw-r--r--   0 runner    (1001) docker     (123)   407128 2023-04-20 22:16:18.000000 hordelib-0.9.5/images/test_inpaint_original.png
--rw-r--r--   0 runner    (1001) docker     (123)  1467500 2023-04-20 22:16:18.000000 hordelib-0.9.5/images/test_outpaint.png
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-20 22:16:26.000000 hordelib-0.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-20 22:16:18.000000 hordelib-0.9.5/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-20 22:16:26.000000 hordelib-0.9.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 22:16:34.031641 hordelib-0.9.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.031641 hordelib-0.9.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/make_index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:16:34.031641 hordelib-0.9.5/tests/model_managers/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/model_managers/test_comvis.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/model_managers/test_diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/model_managers/test_safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/test_blip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/test_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/test_comfy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/test_horde_controlnet_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/test_horde_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/test_horde_inference_controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/test_horde_inference_img2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/test_horde_inference_painting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/test_horde_pp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/test_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/test_initialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/test_safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/test_shared_model_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-20 22:16:18.000000 hordelib-0.9.5/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-20 22:16:18.000000 hordelib-0.9.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.622115 hordelib-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-14 14:25:28.000000 hordelib-1.0.0/.changelog
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-14 14:25:28.000000 hordelib-1.0.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.498118 hordelib-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.526117 hordelib-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-14 14:25:28.000000 hordelib-1.0.0/.github/workflows/maintests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-14 14:25:28.000000 hordelib-1.0.0/.github/workflows/prtests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-14 14:25:28.000000 hordelib-1.0.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-14 14:25:28.000000 hordelib-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    37984 2023-05-14 14:25:36.000000 hordelib-1.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-14 14:25:28.000000 hordelib-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-14 14:25:28.000000 hordelib-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    50821 2023-05-14 14:25:47.622115 hordelib-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-05-14 14:25:28.000000 hordelib-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-14 14:25:28.000000 hordelib-1.0.0/build_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.526117 hordelib-1.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-05-14 14:25:28.000000 hordelib-1.0.0/examples/kudos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-14 14:25:28.000000 hordelib-1.0.0/examples/make_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-14 14:25:28.000000 hordelib-1.0.0/examples/make_index_all_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-14 14:25:28.000000 hordelib-1.0.0/examples/run_all_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-14 14:25:28.000000 hordelib-1.0.0/examples/run_all_stress_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-14 14:25:28.000000 hordelib-1.0.0/examples/run_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-14 14:25:28.000000 hordelib-1.0.0/examples/run_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-14 14:25:28.000000 hordelib-1.0.0/examples/run_controlnet_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-14 14:25:28.000000 hordelib-1.0.0/examples/run_facefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-14 14:25:28.000000 hordelib-1.0.0/examples/run_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-14 14:25:28.000000 hordelib-1.0.0/examples/run_img2img_hires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-14 14:25:28.000000 hordelib-1.0.0/examples/run_img2img_inpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-14 14:25:28.000000 hordelib-1.0.0/examples/run_img2img_inpaint_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-14 14:25:28.000000 hordelib-1.0.0/examples/run_img2img_outpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-14 14:25:28.000000 hordelib-1.0.0/examples/run_inpainting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-05-14 14:25:28.000000 hordelib-1.0.0/examples/run_kudos_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-05-14 14:25:28.000000 hordelib-1.0.0/examples/run_memory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-05-14 14:25:28.000000 hordelib-1.0.0/examples/run_stress_test_cnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-14 14:25:28.000000 hordelib-1.0.0/examples/run_stress_test_cnet_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-05-14 14:25:28.000000 hordelib-1.0.0/examples/run_stress_test_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-14 14:25:28.000000 hordelib-1.0.0/examples/run_stress_test_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-05-14 14:25:28.000000 hordelib-1.0.0/examples/run_stress_test_mixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-05-14 14:25:28.000000 hordelib-1.0.0/examples/run_stress_test_pp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-14 14:25:28.000000 hordelib-1.0.0/examples/run_stress_test_txt2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-14 14:25:28.000000 hordelib-1.0.0/examples/run_stress_test_txt2img_hiresfix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-14 14:25:28.000000 hordelib-1.0.0/examples/run_txt2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-14 14:25:28.000000 hordelib-1.0.0/examples/run_txt2img_hires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-14 14:25:28.000000 hordelib-1.0.0/examples/run_txt2img_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-14 14:25:28.000000 hordelib-1.0.0/examples/run_upscale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.530117 hordelib-1.0.0/hordelib/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.530117 hordelib-1.0.0/hordelib/_comfyui/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-14 14:25:39.000000 hordelib-1.0.0/hordelib/_comfyui/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-14 14:25:39.000000 hordelib-1.0.0/hordelib/_comfyui/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.534117 hordelib-1.0.0/hordelib/_comfyui/comfy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.534117 hordelib-1.0.0/hordelib/_comfyui/comfy/cldm/
+-rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/cldm/cldm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/cli_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-14 14:25:39.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/clip_vision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-14 14:25:39.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/clip_vision_config_h.json
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-14 14:25:39.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/clip_vision_config_vitl.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-05-14 14:25:39.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/diffusers_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.534117 hordelib-1.0.0/hordelib/_comfyui/comfy/extra_samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)    38450 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/extra_samplers/uni_pc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/gligen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.534117 hordelib-1.0.0/hordelib/_comfyui/comfy/k_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-05-14 14:25:39.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/k_diffusion/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-14 14:25:39.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/k_diffusion/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-14 14:25:39.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/k_diffusion/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-05-14 14:25:39.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/k_diffusion/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-14 14:25:39.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/k_diffusion/gns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-05-14 14:25:39.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/k_diffusion/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.534117 hordelib-1.0.0/hordelib/_comfyui/comfy/k_diffusion/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-14 14:25:39.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/k_diffusion/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-05-14 14:25:39.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/k_diffusion/models/image_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27584 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/k_diffusion/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13168 2023-05-14 14:25:39.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/k_diffusion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.534117 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.534117 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:39.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-14 14:25:39.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/data/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.534117 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/models/autoencoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.534117 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/models/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:39.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/models/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21367 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/models/diffusion/ddim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89269 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/models/diffusion/ddpm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.538117 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-14 14:25:39.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66501 2023-05-14 14:25:39.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/dpm_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/models/diffusion/plms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/models/diffusion/sampling_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.538117 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)    21885 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.538117 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37813 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31910 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/openaimodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/upscaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.538117 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/distributions/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/ema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.538117 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/encoders/kornia_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/encoders/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/encoders/noise_aug_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.538117 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25198 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22341 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan_light.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.538117 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)   441072 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29024 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.538117 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/midas/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.542117 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/dpt_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/midas/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/sub_quadratic_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/tomesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14175 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/model_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25875 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41290 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/sd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13673 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/sd1_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/sd1_clip_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.542117 hordelib-1.0.0/hordelib/_comfyui/comfy/sd1_tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (123)   524619 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/sd1_tokenizer/merges.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/sd1_tokenizer/special_tokens_map.json
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/sd1_tokenizer/tokenizer_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1059962 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/sd1_tokenizer/vocab.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/sd2_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/sd2_clip_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.542117 hordelib-1.0.0/hordelib/_comfyui/comfy/t2i_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/t2i_adapter/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.542117 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.542117 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.546117 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/
+-rw-r--r--   0 runner    (1001) docker     (123)    44849 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/HAT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-ESRGAN
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-HAT
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-RealESRGAN
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SPSR
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwiftSRGAN
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-Swin2SR
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwinIR
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-lama
+-rw-r--r--   0 runner    (1001) docker     (123)    17696 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-mat
+-rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LaMa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52744 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/MAT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/RRDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SPSR.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SRVGG.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwiftSRGAN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51124 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/Swin2SR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42740 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwinIR.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13485 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.546117 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/
+-rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-GFPGAN
+-rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-RestoreFormer
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-codeformer
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/arcface_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26761 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/codeformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/fused_act.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpgan_bilinear_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19869 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_clean_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24279 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/restoreformer_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28520 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23283 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_bilinear_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16146 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_clean_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/upfirdn2d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.546117 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/
+-rw-r--r--   0 runner    (1001) docker     (123)    25609 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.550117 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/model_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/nodes_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/nodes_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfy_extras/nodes_upscale_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118577 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/comfyui_screenshot.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.550117 hordelib-1.0.0/hordelib/_comfyui/custom_nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/custom_nodes/example_node.py.example
+-rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/extra_model_paths.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/extra_model_paths.yaml.example
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/folder_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.550117 hordelib-1.0.0/hordelib/_comfyui/input/
+-rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/input/example.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.510117 hordelib-1.0.0/hordelib/_comfyui/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.550117 hordelib-1.0.0/hordelib/_comfyui/models/checkpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/models/checkpoints/put_checkpoints_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.550117 hordelib-1.0.0/hordelib/_comfyui/models/clip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/models/clip/put_clip_or_text_encoder_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.550117 hordelib-1.0.0/hordelib/_comfyui/models/clip_vision/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/models/clip_vision/put_clip_vision_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.550117 hordelib-1.0.0/hordelib/_comfyui/models/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/models/configs/anything_v3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/models/configs/v1-inference.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2_fp16.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/models/configs/v1-inference_fp16.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/models/configs/v1-inpainting-inference.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/models/configs/v2-inference-v.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/models/configs/v2-inference-v_fp32.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/models/configs/v2-inference.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/models/configs/v2-inference_fp32.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/models/configs/v2-inpainting-inference.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.550117 hordelib-1.0.0/hordelib/_comfyui/models/controlnet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/models/controlnet/put_controlnets_and_t2i_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.550117 hordelib-1.0.0/hordelib/_comfyui/models/diffusers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/models/diffusers/put_diffusers_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.550117 hordelib-1.0.0/hordelib/_comfyui/models/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/models/embeddings/put_embeddings_or_textual_inversion_concepts_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.550117 hordelib-1.0.0/hordelib/_comfyui/models/gligen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/models/gligen/put_gligen_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.550117 hordelib-1.0.0/hordelib/_comfyui/models/loras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/models/loras/put_loras_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.550117 hordelib-1.0.0/hordelib/_comfyui/models/style_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/models/style_models/put_t2i_style_model_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.550117 hordelib-1.0.0/hordelib/_comfyui/models/upscale_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/models/upscale_models/put_esrgan_and_other_upscale_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.550117 hordelib-1.0.0/hordelib/_comfyui/models/vae/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/models/vae/put_vae_here
+-rw-r--r--   0 runner    (1001) docker     (123)    48078 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.550117 hordelib-1.0.0/hordelib/_comfyui/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/notebooks/comfyui_colab.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.550117 hordelib-1.0.0/hordelib/_comfyui/output/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/output/_output_images_will_be_put_here
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.550117 hordelib-1.0.0/hordelib/_comfyui/script_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/script_examples/basic_api_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.550117 hordelib-1.0.0/hordelib/_comfyui/web/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.550117 hordelib-1.0.0/hordelib/_comfyui/web/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.554117 hordelib-1.0.0/hordelib/_comfyui/web/extensions/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    14641 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/web/extensions/core/colorPalette.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/web/extensions/core/contextMenuFilter.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/web/extensions/core/dynamicPrompts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/web/extensions/core/editAttention.js
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/web/extensions/core/keybinds.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/web/extensions/core/nodeTemplates.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/web/extensions/core/noteNode.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/web/extensions/core/rerouteNode.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/web/extensions/core/slotDefaults.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/web/extensions/core/snapToGrid.js
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/web/extensions/core/uploadImage.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/web/extensions/core/widgetInputs.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/web/extensions/logging.js.example
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/web/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/web/jsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.554117 hordelib-1.0.0/hordelib/_comfyui/web/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)   482237 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/web/lib/litegraph.core.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/web/lib/litegraph.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.554117 hordelib-1.0.0/hordelib/_comfyui/web/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/web/scripts/api.js
+-rw-r--r--   0 runner    (1001) docker     (123)    31674 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/web/scripts/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/web/scripts/defaultGraph.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/web/scripts/pnginfo.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/web/scripts/ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/web/scripts/widgets.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/web/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.554117 hordelib-1.0.0/hordelib/_comfyui/web/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/web/types/comfy.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    52898 2023-05-14 14:25:40.000000 hordelib-1.0.0/hordelib/_comfyui/web/types/litegraph.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-14 14:25:47.000000 hordelib-1.0.0/hordelib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.554117 hordelib-1.0.0/hordelib/blip/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/blip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/blip/caption.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.554117 hordelib-1.0.0/hordelib/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/cache/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.558117 hordelib-1.0.0/hordelib/clip/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/clip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/clip/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/clip/coca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/clip/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/clip/interrogate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.558117 hordelib-1.0.0/hordelib/clip/ranking_lists/
+-rw-r--r--   0 runner    (1001) docker     (123)    80572 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/clip/ranking_lists/artists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/clip/ranking_lists/flavors.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/clip/ranking_lists/mediums.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/clip/ranking_lists/movements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/clip/ranking_lists/sites.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    22260 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/clip/ranking_lists/tags.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/clip/ranking_lists/techniques.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/clip/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21161 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/comfy_horde.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/config_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19874 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/horde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/initialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44802 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/install_comfy.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/install_comfy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.558117 hordelib-1.0.0/hordelib/model_database/
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/model_database/aitemplate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/model_database/blip.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/model_database/clip.json
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/model_database/codeformer.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/model_database/controlnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)   218801 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/model_database/db.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/model_database/db_dep.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/model_database/db_embeds.json
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/model_database/diffusers.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/model_database/esrgan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/model_database/gfpgan.json
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/model_database/med_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/model_database/safety_checker.json
+-rw-r--r--   0 runner    (1001) docker     (123)   256036 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/model_database/stable_diffusion.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.562116 hordelib-1.0.0/hordelib/model_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/model_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36755 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/model_manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/model_manager/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/model_manager/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/model_manager/codeformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/model_manager/compvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/model_manager/controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/model_manager/diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/model_manager/esrgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/model_manager/gfpgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15847 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/model_manager/hyper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/model_manager/safety_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.562116 hordelib-1.0.0/hordelib/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.562116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13015 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.562116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/binary/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.562116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/canny/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/canny/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.562116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/color/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.562116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/hed/
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.562116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.562116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22985 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.562116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.566116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28960 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.566116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.566116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.566116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.566116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.566116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.566116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24104 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.566116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.566116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.570116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.570116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20432 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.570116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.518117 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.570116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.570116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.574116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.574116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_160k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_40k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_80k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.518117 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.574116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.574116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.574116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.574116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.578116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15999 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/swish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.578116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22125 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25256 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.578116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.578116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41996 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.582116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.582116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25196 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.582116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/deprecated.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.586116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15624 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.586116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.590116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20867 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25157 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.590116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/closure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22532 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/iter_timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.594116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21317 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.594116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.594116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25975 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.594116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.594116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.594116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19217 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.522117 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.598116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.598116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.598116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13100 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.598116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.598116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/base_pixel_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.598116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.598116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14268 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.598116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31035 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.602116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.602116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24415 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18353 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18518 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18169 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.606116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.606116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.606116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.606116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.606116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.606116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.606116 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.606116 hordelib-1.0.0/hordelib/nodes/facerestore/
+-rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.610116 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.610116 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/align_trans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.610116 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/retinaface/
+-rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.610116 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.610116 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.610116 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/autoanchor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/extract_ckpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.610116 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/parsing/bisenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/parsing/parsenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/parsing/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.610116 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23302 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/utils/face_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/facerestore/facelib/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/node_clip_similarities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/node_controlnet_model_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/node_image_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/node_image_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/node_model_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/nodes/node_upscale_model_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.614116 hordelib-1.0.0/hordelib/pipeline_designs/
+-rw-r--r--   0 runner    (1001) docker     (123)    15440 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/pipeline_designs/pipeline_controlnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/pipeline_designs/pipeline_controlnet_annotator.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17729 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/pipeline_designs/pipeline_controlnet_hires_fix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/pipeline_designs/pipeline_image_facefix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/pipeline_designs/pipeline_image_upscale.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/pipeline_designs/pipeline_stable_diffusion.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.614116 hordelib-1.0.0/hordelib/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/pipelines/pipeline_controlnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/pipelines/pipeline_controlnet_annotator.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/pipelines/pipeline_controlnet_hires_fix.json
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/pipelines/pipeline_image_facefix.json
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/pipelines/pipeline_image_upscale.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/pipelines/pipeline_stable_diffusion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/pipelines/pipeline_stable_diffusion_paint.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/preload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/shared_model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13850 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.614116 hordelib-1.0.0/hordelib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.614116 hordelib-1.0.0/hordelib/utils/blip/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/utils/blip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/utils/blip/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41378 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/utils/blip/med.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/utils/blip/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/utils/cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/utils/dynamicprompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/utils/gpuinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/utils/ioredirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-14 14:25:28.000000 hordelib-1.0.0/hordelib/utils/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.530117 hordelib-1.0.0/hordelib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    50821 2023-05-14 14:25:47.000000 hordelib-1.0.0/hordelib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    50459 2023-05-14 14:25:47.000000 hordelib-1.0.0/hordelib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 14:25:47.000000 hordelib-1.0.0/hordelib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-14 14:25:47.000000 hordelib-1.0.0/hordelib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-14 14:25:47.000000 hordelib-1.0.0/hordelib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.618116 hordelib-1.0.0/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    71522 2023-05-14 14:25:28.000000 hordelib-1.0.0/images/test_annotator.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    36815 2023-05-14 14:25:28.000000 hordelib-1.0.0/images/test_db0.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   538159 2023-05-14 14:25:28.000000 hordelib-1.0.0/images/test_facefix.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1474994 2023-05-14 14:25:28.000000 hordelib-1.0.0/images/test_inpaint.png
+-rw-r--r--   0 runner    (1001) docker     (123)   411844 2023-05-14 14:25:28.000000 hordelib-1.0.0/images/test_inpaint_alpha.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11886 2023-05-14 14:25:28.000000 hordelib-1.0.0/images/test_inpaint_mask.png
+-rw-r--r--   0 runner    (1001) docker     (123)   407128 2023-05-14 14:25:28.000000 hordelib-1.0.0/images/test_inpaint_original.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1467500 2023-05-14 14:25:28.000000 hordelib-1.0.0/images/test_outpaint.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-14 14:25:40.000000 hordelib-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-14 14:25:28.000000 hordelib-1.0.0/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-14 14:25:40.000000 hordelib-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 14:25:47.622115 hordelib-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.622115 hordelib-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-14 14:25:28.000000 hordelib-1.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.622115 hordelib-1.0.0/tests/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-14 14:25:28.000000 hordelib-1.0.0/tests/meta/test_build_helper_import_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:25:47.622115 hordelib-1.0.0/tests/model_managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-14 14:25:28.000000 hordelib-1.0.0/tests/model_managers/test_annotators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-14 14:25:28.000000 hordelib-1.0.0/tests/model_managers/test_comvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-14 14:25:28.000000 hordelib-1.0.0/tests/model_managers/test_diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-14 14:25:28.000000 hordelib-1.0.0/tests/model_managers/test_safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-14 14:25:28.000000 hordelib-1.0.0/tests/test_blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-14 14:25:28.000000 hordelib-1.0.0/tests/test_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-05-14 14:25:28.000000 hordelib-1.0.0/tests/test_comfy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-14 14:25:28.000000 hordelib-1.0.0/tests/test_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-14 14:25:28.000000 hordelib-1.0.0/tests/test_dynamic_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-14 14:25:28.000000 hordelib-1.0.0/tests/test_horde_controlnet_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-05-14 14:25:28.000000 hordelib-1.0.0/tests/test_horde_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-14 14:25:28.000000 hordelib-1.0.0/tests/test_horde_inference_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-05-14 14:25:28.000000 hordelib-1.0.0/tests/test_horde_inference_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-14 14:25:28.000000 hordelib-1.0.0/tests/test_horde_inference_painting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-05-14 14:25:28.000000 hordelib-1.0.0/tests/test_horde_pp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-14 14:25:28.000000 hordelib-1.0.0/tests/test_horde_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-14 14:25:28.000000 hordelib-1.0.0/tests/test_image_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-05-14 14:25:28.000000 hordelib-1.0.0/tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-14 14:25:28.000000 hordelib-1.0.0/tests/test_initialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-14 14:25:28.000000 hordelib-1.0.0/tests/test_safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-05-14 14:25:28.000000 hordelib-1.0.0/tests/test_shared_model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-14 14:25:28.000000 hordelib-1.0.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-14 14:25:28.000000 hordelib-1.0.0/tox.ini
```

### Comparing `hordelib-0.9.5/.changelog` & `hordelib-1.0.0/.changelog`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/.github/workflows/maintests.yml` & `hordelib-1.0.0/.github/workflows/maintests.yml`

 * *Files 17% similar despite different names*

```diff
@@ -24,23 +24,29 @@
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
       - name: Install tox and any other packages
-        run: pip install --upgrade -r requirements.dev.txt
-      - name: Run lint/format check
+        run: | 
+          python -m pip install --upgrade pip
+          pip install --upgrade -r requirements.dev.txt
+      - name: Run format check
+        run: tox -e format
+      - name: Run lint check
         run: tox -e lint-weak-check
-      - name: Run tox
+      - name: Check build_helper.py hordelib imports have no breaking dependency changes
+        run: tox -e test-build-helper
+      - name: Build unit test environment, confirm CUDA is available on host
+        run: tox -e tests -- -k test_cuda
+      - name: Run unit tests
         run: tox -e tests
-      - name: Run a direct run test
-        run: python -m examples.run_upscale
       - name: Create CI webpage of results
-        run: python -m tests.make_index
+        run: python -m examples.make_index
       - name: Upload to S3
         uses: shallwefootball/s3-upload-action@master
         id: S3
         with:
           aws_key_id: ${{secrets.S3_BUILD_ARTIFACTS_ACCESS_KEY_ID}}
           aws_secret_access_key: ${{secrets.S3_BUILD_ARTIFACTS_SECRET_ACCESS_KEY}}
           aws_bucket: hordelib
```

### Comparing `hordelib-0.9.5/.github/workflows/prtests.yml` & `hordelib-1.0.0/.github/workflows/prtests.yml`

 * *Files 9% similar despite different names*

```diff
@@ -29,23 +29,29 @@
         with:
           ref: ${{ github.event.pull_request.head.sha }}
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
       - name: Install tox and any other packages
-        run: pip install --upgrade -r requirements.dev.txt
-      - name: Run lint/format check
+        run: | 
+          python -m pip install --upgrade pip
+          pip install --upgrade -r requirements.dev.txt
+      - name: Run format check
+        run: tox -e format
+      - name: Run lint check
         run: tox -e lint-weak-check
-      - name: Run tox
+      - name: Check build_helper.py hordelib imports have no breaking dependency changes
+        run: tox -e test-build-helper
+      - name: Build unit test environment, confirm CUDA is available on host
+        run: tox -e tests -- -k test_cuda
+      - name: Run unit tests
         run: tox -e tests
-      - name: Run a direct run test
-        run: python -m examples.run_upscale
       - name: Create CI webpage of results
-        run: python -m tests.make_index
+        run: python -m examples.make_index
       - name: Upload to S3
         uses: shallwefootball/s3-upload-action@master
         id: S3
         with:
           aws_key_id: ${{secrets.S3_BUILD_ARTIFACTS_ACCESS_KEY_ID}}
           aws_secret_access_key: ${{secrets.S3_BUILD_ARTIFACTS_SECRET_ACCESS_KEY}}
           aws_bucket: hordelib
```

### Comparing `hordelib-0.9.5/.github/workflows/release.yml` & `hordelib-1.0.0/.github/workflows/release.yml`

 * *Files 7% similar despite different names*

```diff
@@ -33,23 +33,27 @@
     # Pass the version number in an env var to the below steps
     - name: Set build version env var
       run: echo "SETUPTOOLS_SCM_PRETEND_VERSION=${{ steps.release.outputs.version }}" >> $GITHUB_ENV
 
     # We need python...
     - name: "🐍 Set up Python 3.10"
       if: ${{ steps.release.outputs.version != '' }}
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v4
       with:
         python-version: "3.10"
 
     # Install build deps
+    # NOTE If any hordelib imports used by build_helper.py are changed, or the specific modules
+    # imported from hordelib depend on a package not included here, this will fail.
+    # See `build_helper.py` and `tests\meta\test_build_helper_import_check.py` for more information.
     - name: "🛠 Install pypa/build"
       if: ${{ steps.release.outputs.version != '' }}
-      run: >-
-        python -m pip install build typing-extensions loguru --user
+      run: |
+        python -m pip install --upgrade pip
+        python -m pip install build psutil typing-extensions loguru --user
 
     - name: "✏️ Install changelog dependencies"
       if: ${{ steps.release.outputs.version != '' }}
       uses: actions/setup-node@v3
 
     - name: "✏️ Generate release changelog"
       if: ${{ steps.release.outputs.version != '' }}
```

### Comparing `hordelib-0.9.5/.gitignore` & `hordelib-1.0.0/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -133,30 +133,35 @@
 
 # Cython debug symbols
 cython_debug/
 
 # Local
 test-image.png
 hordelib/ComfyUI
-hordelib/_comfyui
+hordelib/model_database
 ComfyUI
 model.ckpt
 coverage.lcov
 images/pip*.png
 images/test.png
 images/hor*.png
 images/hor*.webp
 images/pip*.webp
 images/test.webp
 images/run_*
+images/all_models
+profiles/
 images/perftest
 images/stresstest
+images/longprompts
+longprompts.zip
 comfy-prompt*.json
 images/index.html
 hordelib/_comfyui
 _version.py
 _comfyui
+tmp/
 
 .vscode
 *.ckpt
 *.pth
 .gitignore
```

### Comparing `hordelib-0.9.5/CHANGELOG.md` & `hordelib-1.0.0/CHANGELOG.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,277 @@
 ## hordelib Changelog
 
+# [v1.0.0](https://github.com/jug-dev/hordelib/compare/v0.19.15...v1.0.0)
+
+14 May 2023
+
+- feat: release v1.0.0 [`#246`](https://github.com/jug-dev/hordelib/pull/246) (Jug)
+
+## [v0.19.15](https://github.com/jug-dev/hordelib/compare/v0.19.14...v0.19.15)
+
+14 May 2023
+
+- chore: prep for v1.0.0 [`#245`](https://github.com/jug-dev/hordelib/pull/245) (Jug)
+
+## [v0.19.14](https://github.com/jug-dev/hordelib/compare/v0.19.13...v0.19.14)
+
+14 May 2023
+
+- fix: better memory management [`#239`](https://github.com/jug-dev/hordelib/pull/239) (Jug)
+- fix: remove some pointless dependencies like libcario [`#240`](https://github.com/jug-dev/hordelib/pull/240) (Jug)
+- Revert "fix: pin timm version to 0.6.13" [`407bee9`](https://github.com/jug-dev/hordelib/commit/407bee9deb997147c8b78a30f04df5171e28aa7b)  (Jug)
+- feat: adds code to generate all models test page [`6c8d882`](https://github.com/jug-dev/hordelib/commit/6c8d88253f820ae03e19a80492554905f90bb5ed)  (Jug)
+- doc: update readme with all models link [`f34bcce`](https://github.com/jug-dev/hordelib/commit/f34bcce43c4cd1b8de7125c5f435f333f3ec227e)  (Jug)
+
+## [v0.19.13](https://github.com/jug-dev/hordelib/compare/v0.19.12...v0.19.13)
+
+13 May 2023
+
+- fix: better memory management [`#243`](https://github.com/jug-dev/hordelib/pull/243) (Jug)
+
+## [v0.19.12](https://github.com/jug-dev/hordelib/compare/v0.19.11...v0.19.12)
+
+13 May 2023
+
+- fix: remove some pointless dependencies like libcario [`#240`](https://github.com/jug-dev/hordelib/pull/240) (Jug)
+
+## [v0.19.11](https://github.com/jug-dev/hordelib/compare/v0.19.10...v0.19.11)
+
+13 May 2023
+
+- fix: pin timm library to v0.6.12 [`ae2e8b0`](https://github.com/jug-dev/hordelib/commit/ae2e8b0d7764b6e1076c4443a378f5275d1c6066)  (Jug)
+
+## [v0.19.10](https://github.com/jug-dev/hordelib/compare/v0.19.9...v0.19.10)
+
+12 May 2023
+
+- fix: check underlying model before warm loading from cache [`#236`](https://github.com/jug-dev/hordelib/pull/236) (tazlin)
+- test: add sampler tests [`#233`](https://github.com/jug-dev/hordelib/pull/233) (Jug)
+- feat: build a payload to inference time prediction model [`#231`](https://github.com/jug-dev/hordelib/pull/231) (Jug)
+- fix: pin timm version to 0.6.13 [`bc4f862`](https://github.com/jug-dev/hordelib/commit/bc4f862d0416d2905a660b7492f9229d9ffca5c4)  (Jug)
+- test: add 10 step sampler tests [`363cbc2`](https://github.com/jug-dev/hordelib/commit/363cbc2ae5ed50c38a87f437c4afd38f6a309f7c)  (Jug)
+- fix: fix kudos model validation [`e103518`](https://github.com/jug-dev/hordelib/commit/e1035183701a8fb7a3f8c06db45e25fa8f5c41b5)  (Jug)
+
+## [v0.19.9](https://github.com/jug-dev/hordelib/compare/v0.19.8...v0.19.9)
+
+8 May 2023
+
+- fix: handle image / mask size mismatch [`#229`](https://github.com/jug-dev/hordelib/pull/229) (Jug)
+
+## [v0.19.8](https://github.com/jug-dev/hordelib/compare/v0.19.7...v0.19.8)
+
+7 May 2023
+
+- fix: faster startup with many models cached [`#224`](https://github.com/jug-dev/hordelib/pull/224) (Jug)
+- fix: cuts 25+ seconds from load time [`f1a453c`](https://github.com/jug-dev/hordelib/commit/f1a453c3fb1a40863ef79a9456ff2dfe06aeea5e)  (tazlin)
+- fix: updates kudos test [`2102588`](https://github.com/jug-dev/hordelib/commit/210258860612ffcf623ec2841979a1850904c8b8)  (Jug)
+- hack: disable optimizations for n_iter &gt; 1 [`89c4aac`](https://github.com/jug-dev/hordelib/commit/89c4aac1a2839336a00a57d8b50eb51f06678c27)  (tazlin)
+
+## [v0.19.7](https://github.com/jug-dev/hordelib/compare/v0.19.6...v0.19.7)
+
+3 May 2023
+
+- fix: remove ether real from exclude list [`92b5794`](https://github.com/jug-dev/hordelib/commit/92b5794f68947a51b94433f7a3b8fa38bec8745a)  (tazlin)
+
+## [v0.19.6](https://github.com/jug-dev/hordelib/compare/v0.19.5...v0.19.6)
+
+3 May 2023
+
+- feat: get model db from legacy model reference repo [`b3dd5a4`](https://github.com/jug-dev/hordelib/commit/b3dd5a4ed122170f514e986187cfe10764779fc1)  (tazlin)
+- fix: the disaster with linking [`1de6e06`](https://github.com/jug-dev/hordelib/commit/1de6e061441ad0b19e29eb1eff29093c9a8847fe)  (tazlin)
+- feat: add a model exclusion list to `consts.py` [`b7e8b46`](https://github.com/jug-dev/hordelib/commit/b7e8b4682feb5bd8712d11b8369038b22cfe5c24)  (tazlin)
+
+## [v0.19.5](https://github.com/jug-dev/hordelib/compare/v0.19.4...v0.19.5)
+
+1 May 2023
+
+- fix: remove Ether Real model due to bad hash [`a671924`](https://github.com/jug-dev/hordelib/commit/a671924d00431b507a00ebbe97e3affe24084a38)  (Jug)
+- ci: try upgrading pip before tests [`68cbd9d`](https://github.com/jug-dev/hordelib/commit/68cbd9df1e8f46741f3e652a38aacdafff199d27)  (Jug)
+
+## [v0.19.4](https://github.com/jug-dev/hordelib/compare/v0.19.3...v0.19.4)
+
+1 May 2023
+
+- fix: update to latest model database [`2f037cf`](https://github.com/jug-dev/hordelib/commit/2f037cf2bbd64b6cc784bfa8c1b57138b3a29941)  (Jug)
+- fix: fix some model download links [`4e6743c`](https://github.com/jug-dev/hordelib/commit/4e6743c57d5026ef7f9b7d94b32f950fd4b6ad0c)  (Jug)
+- ci: change tests to abort after first failure [`d80613c`](https://github.com/jug-dev/hordelib/commit/d80613cc35a86d5b299cb70f70607e19785672a3)  (Jug)
+
+## [v0.19.3](https://github.com/jug-dev/hordelib/compare/v0.19.2...v0.19.3)
+
+1 May 2023
+
+- ci: update some bits of the release ci [`1add1db`](https://github.com/jug-dev/hordelib/commit/1add1db011ed43d23cda10ac46709a2c7cf83fda)  (Jug)
+
+## [v0.19.2](https://github.com/jug-dev/hordelib/compare/v0.19.1...v0.19.2)
+
+1 May 2023
+
+## [v0.19.1](https://github.com/jug-dev/hordelib/compare/v0.19.0...v0.19.1)
+
+1 May 2023
+
+- docs: update readme [`646a419`](https://github.com/jug-dev/hordelib/commit/646a419bef63c48bfb970efbd25781bd748c8b8e)  (Jug)
+
+## [v0.19.0](https://github.com/jug-dev/hordelib/compare/v0.18.0...v0.19.0)
+
+1 May 2023
+
+## [v0.18.0](https://github.com/jug-dev/hordelib/compare/v0.17.0...v0.18.0)
+
+1 May 2023
+
+- feat: use less vram with large images (tiled vae decode) [`#207`](https://github.com/jug-dev/hordelib/pull/207) (Jug)
+- fix: suppress some clip debug [`9849955`](https://github.com/jug-dev/hordelib/commit/98499553b367bb8c9fad3ab2c66a1d557cbb539b)  (Jug)
+
+## [v0.17.0](https://github.com/jug-dev/hordelib/compare/v0.16.4...v0.17.0)
+
+1 May 2023
+
+- feat: minor performance tweaking [`#205`](https://github.com/jug-dev/hordelib/pull/205) (Jug)
+- feat: update model database [`a80846e`](https://github.com/jug-dev/hordelib/commit/a80846e2f7b791f496bd3042e968b8b67ddbb7bf)  (Jug)
+- fix: adds ersgan upscaler, SHA check now case insensitive [`1d82e30`](https://github.com/jug-dev/hordelib/commit/1d82e30aac4ce3207a034b184e7a7406b3206962)  (tazlin)
+- docs: update readme [`26c3b62`](https://github.com/jug-dev/hordelib/commit/26c3b6268e5f8041a193a9967605d0843cee6884)  (Jug)
+
+## [v0.16.4](https://github.com/jug-dev/hordelib/compare/v0.16.3...v0.16.4)
+
+30 April 2023
+
+- fix: support the latest model database format [`a986d06`](https://github.com/jug-dev/hordelib/commit/a986d0699edf3d299a0c8b9b8b75382fcebb1e39)  (Jug)
+
+## [v0.16.3](https://github.com/jug-dev/hordelib/compare/v0.16.2...v0.16.3)
+
+29 April 2023
+
+- style: stable_diffusion.json whitespace [`d5dbd95`](https://github.com/jug-dev/hordelib/commit/d5dbd95ff1267ddb47c633ef13e0bece8a5044c3)  (tazlin)
+- fix: update civitai links out of date, adds two safetensors [`70a675e`](https://github.com/jug-dev/hordelib/commit/70a675e8d7cc5a930664d2b94be3d97b6b995246)  (tazlin)
+- fix: don't allow dynamic prompts to interfere with the random seed. [`5643490`](https://github.com/jug-dev/hordelib/commit/5643490d8fea6070074232b6623ef6c6f98b21e5)  (Jug)
+
+## [v0.16.2](https://github.com/jug-dev/hordelib/compare/v0.16.1...v0.16.2)
+
+29 April 2023
+
+- fix: ensure we manage ram when loading models from cache [`516f001`](https://github.com/jug-dev/hordelib/commit/516f001383f27c9d2e9b56dff42164213a8d0b96)  (Jug)
+
+## [v0.16.1](https://github.com/jug-dev/hordelib/compare/v0.16.0...v0.16.1)
+
+29 April 2023
+
+- fix: disk cache model load optimisation [`#198`](https://github.com/jug-dev/hordelib/pull/198) (Jug)
+
+## [v0.16.0](https://github.com/jug-dev/hordelib/compare/v0.15.3...v0.16.0)
+
+29 April 2023
+
+- feat: automatic resource management [`#186`](https://github.com/jug-dev/hordelib/pull/186) (Jug)
+
+## [v0.15.3](https://github.com/jug-dev/hordelib/compare/v0.15.2...v0.15.3)
+
+29 April 2023
+
+- fix: removed extraoneous clip debug messages [`#194`](https://github.com/jug-dev/hordelib/pull/194) (Divided by Zer0)
+- feat: add torch and xformers versions to benchmark [`559f198`](https://github.com/jug-dev/hordelib/commit/559f1989e2ec3b42c95ee0e2947bf248f01a92f5)  (Jug)
+- fix: exclude `build/` folder from linting [`5f38c3f`](https://github.com/jug-dev/hordelib/commit/5f38c3feecacb7e6a12af598b4a42bee8c00f43a)  (tazlin)
+
+## [v0.15.2](https://github.com/jug-dev/hordelib/compare/v0.15.1...v0.15.2)
+
+29 April 2023
+
+- fix: validate denoising parameter bounds [`df1a369`](https://github.com/jug-dev/hordelib/commit/df1a369b612e7e960844ed5da7aee54fce42895e)  (Jug)
+- fix: facefix didn't work on dev versions of torch [`7cc212b`](https://github.com/jug-dev/hordelib/commit/7cc212b4fb7bc174307e2d8de960042628d06cef)  (Jug)
+- build: bump to xformers 0.0.19 [`1c0eb4a`](https://github.com/jug-dev/hordelib/commit/1c0eb4a094a5f88c2bcc3e61155141d743fdf92d)  (Jug)
+
+## [v0.15.1](https://github.com/jug-dev/hordelib/compare/v0.15.0...v0.15.1)
+
+27 April 2023
+
+- fix: disable controlnet on low vram gpus in benchmark [`#191`](https://github.com/jug-dev/hordelib/pull/191) (Jug)
+- fix: rectify txt2img highres denoising [`fd20e69`](https://github.com/jug-dev/hordelib/commit/fd20e691af566048df3032d42485dbc374101e51)  (Jug)
+
+## [v0.15.0](https://github.com/jug-dev/hordelib/compare/v0.14.2...v0.15.0)
+
+27 April 2023
+
+- fix: remove unused file [`410923c`](https://github.com/jug-dev/hordelib/commit/410923cfb6880321c6532a7049a7f90aaefd95f4)  (Jug)
+- tests: new test for cuda [`4288273`](https://github.com/jug-dev/hordelib/commit/4288273590cc7681ced9d104e1b7caa45276c21e)  (db0)
+- fix: auto fix if width/height not divisible by 64 [`f89f889`](https://github.com/jug-dev/hordelib/commit/f89f889122bf3656c9c3706146863118c60bff9a)  (Jug)
+
+## [v0.14.2](https://github.com/jug-dev/hordelib/compare/v0.14.1...v0.14.2)
+
+27 April 2023
+
+- fix: image sizing bugs with hires fix and controlnet [`ad0d6a9`](https://github.com/jug-dev/hordelib/commit/ad0d6a9551c5b3766c4c19bc08b994bf7e3589dc)  (Jug)
+- fix: benchmark on linux [`48de047`](https://github.com/jug-dev/hordelib/commit/48de0477261b5b7f5c01789658a15b161d7796c2)  (Jug)
+
+## [v0.14.1](https://github.com/jug-dev/hordelib/compare/v0.14.0...v0.14.1)
+
+24 April 2023
+
+- fix: use denoising as controlnet strength (compatibility hack) [`#183`](https://github.com/jug-dev/hordelib/pull/183) (Jug)
+
+## [v0.14.0](https://github.com/jug-dev/hordelib/compare/v0.13.0...v0.14.0)
+
+24 April 2023
+
+- feat: encode prompt pipeline in raw output image metadata [`#181`](https://github.com/jug-dev/hordelib/pull/181) (Jug)
+- feat: add OS and VRAM to benchmark [`95fa03d`](https://github.com/jug-dev/hordelib/commit/95fa03da94f0940248b09743de91a94732a9118a)  (Jug)
+- fix: lint fixes [`c87f3b0`](https://github.com/jug-dev/hordelib/commit/c87f3b02ada9c7ee927636c1ebd1485c48891279)  (Jug)
+
+## [v0.13.0](https://github.com/jug-dev/hordelib/compare/v0.12.1...v0.13.0)
+
+24 April 2023
+
+- feat: adds a hordelib benchmark test [`#179`](https://github.com/jug-dev/hordelib/pull/179) (Jug)
+
+## [v0.12.1](https://github.com/jug-dev/hordelib/compare/v0.12.0...v0.12.1)
+
+24 April 2023
+
+- fix: unload local models correctly [`d75ffb9`](https://github.com/jug-dev/hordelib/commit/d75ffb91985025a71cb5960d260df178f3dfd269)  (Jug)
+- fix: Clearer logging message for annotator check/download [`131d07f`](https://github.com/jug-dev/hordelib/commit/131d07fcc5142c28caaf451a440cd5d336ba1e3e)  (tazlin)
+- fix: pidinet annotator being downloaded to wrong location [`8b40b16`](https://github.com/jug-dev/hordelib/commit/8b40b169a5a69c1cbc01f3eca201eb959918c096)  (tazlin)
+
+## [v0.12.0](https://github.com/jug-dev/hordelib/compare/v0.11.1...v0.12.0)
+
+24 April 2023
+
+- fix: model loaded/unloading stress test fixes [`#175`](https://github.com/jug-dev/hordelib/pull/175) (Jug)
+- feat: add support for controlnet hires fix [`#173`](https://github.com/jug-dev/hordelib/pull/173) (Jug)
+- fix: implicitly load local models [`#174`](https://github.com/jug-dev/hordelib/pull/174) (Jug)
+
+## [v0.11.1](https://github.com/jug-dev/hordelib/compare/v0.11.0...v0.11.1)
+
+23 April 2023
+
+- fix: parameter handling improvements [`#170`](https://github.com/jug-dev/hordelib/pull/170) (Jug)
+
+## [v0.11.0](https://github.com/jug-dev/hordelib/compare/v0.10.1...v0.11.0)
+
+23 April 2023
+
+- feat: add control_strength parameter for cnet strength [`#167`](https://github.com/jug-dev/hordelib/pull/167) (Jug)
+- feat: add support for local models including safetensors [`#166`](https://github.com/jug-dev/hordelib/pull/166) (Jug)
+- feat: upgrade to latest comfyui backend [`#165`](https://github.com/jug-dev/hordelib/pull/165) (Jug)
+
+## [v0.10.1](https://github.com/jug-dev/hordelib/compare/v0.10.0...v0.10.1)
+
+22 April 2023
+
+- fix: img2img passes 5 thread stress test [`#163`](https://github.com/jug-dev/hordelib/pull/163) (Jug)
+- fix: unknown samplers and cnets changed to warnings [`c98c74b`](https://github.com/jug-dev/hordelib/commit/c98c74ba497555770b8a685bd8fbc356216fce90)  (Jug)
+
+## [v0.10.0](https://github.com/jug-dev/hordelib/compare/v0.9.5...v0.10.0)
+
+22 April 2023
+
+- feat: add dynamic prompt support [`#161`](https://github.com/jug-dev/hordelib/pull/161) (Jug)
+- fix: stability fixes [`#159`](https://github.com/jug-dev/hordelib/pull/159) (Jug)
+- fix: Moves ControlNet Annotators to `AIWORKER_CACHE_HOME` [`e0a7db7`](https://github.com/jug-dev/hordelib/commit/e0a7db7e89dc91016dd5abba2e94ccf3767c65d3)  (tazlin)
+- refactor: cleans up the preload annotators functions [`6b8f9c4`](https://github.com/jug-dev/hordelib/commit/6b8f9c453ef38af3439a6bf6ca2b99de649fc6c6)  (tazlin)
+- feat: Preload controlnet annotators [`6d16515`](https://github.com/jug-dev/hordelib/commit/6d1651535915022cac8e7d218ca4d5081d1d2241)  (tazlin)
+
 ## [v0.9.5](https://github.com/jug-dev/hordelib/compare/v0.9.4...v0.9.5)
 
 20 April 2023
 
 - build: fix missing dependency in pypi build [`01169be`](https://github.com/jug-dev/hordelib/commit/01169beb575c0a0577eebc00210ca98d14eeff42)  (Jug)
 
 ## [v0.9.4](https://github.com/jug-dev/hordelib/compare/v0.9.3...v0.9.4)
```

### Comparing `hordelib-0.9.5/LICENSE` & `hordelib-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/PKG-INFO` & `hordelib-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hordelib
-Version: 0.9.5
+Version: 1.0.0
 Summary: A thin wrapper around ComfyUI to allow use by AI Horde.
 Author-email: Jug <jugdev@proton.me>, db0 <mail@dbzer0.com>, tazlin <tazlin.on.github@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -682,21 +682,22 @@
 [![PyPI Version][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 ![GitHub license][license-url]
 
 [![Build][build-image]][build-url]
 [![Test Images][main-test-image]][main-test-url]
 [![Test Images][pr-test-image]][pr-test-url]
+[![All Models][all-model-images]][all-model-url]
 [![Release Changelog][changelog-image]][changelog-url]
 
-`hordelib` is a thin wrapper around [ComfyUI](https://github.com/comfyanonymous/ComfyUI) primarily to enable the [AI Horde](https://aihorde.net/) to run inference pipelines designed visually in the ComfyUI GUI.
+`hordelib` is a wrapper around [ComfyUI](https://github.com/comfyanonymous/ComfyUI) primarily to enable the [AI Horde](https://aihorde.net/) to run inference pipelines designed visually in the ComfyUI GUI.
 
 The developers of `hordelib` can be found in the AI Horde Discord server: [https://discord.gg/3DxrhksKzn](https://discord.gg/3DxrhksKzn)
 
-NOTE: This project is in development and is not yet in use by Stable Horde.
+`hordelib` has been the default inference backend library of the [AI Horde](https://aihorde.net/) since `hordelib` v1.0.0.
 
 ## Purpose
 
 The goal here is to be able to design inference pipelines in the excellent ComfyUI, and then call those inference pipelines programmatically. Whilst providing features that maintain compatibility with the existing horde implementation.
 
 ## Installation
 
@@ -830,15 +831,26 @@
 `hordelib/pipelines/`
 Contains the above pipeline JSON files converted to the format required by the backend pipeline processor. These are converted from the web app, see _Converting ComfyUI pipelines_ below.
 
 `hordelib/nodes/` These are the custom ComfyUI nodes we use for `hordelib` specific processing.
 
 ### Running ComfyUI Web Application
 
-`tox -e comfyui`
+In this example we install the dependencies in the OS default environment. When using the git version of `hordelib`, from the project root:
+
+`pip install -r requirements.txt --extra-index-url https://download.pytorch.org/whl/cu118 --upgrade`
+
+Ensure ComfyUI is installed and patched, one way is running the tests:
+
+`tox`
+
+From then on to run ComfyUI:
+
+`cd ComfyUI`
+`python main.py`
 
 Then open a browser at: http://127.0.0.1:8188/
 
 ### Designing ComfyUI Pipelines
 
 Use the standard ComfyUI web app. Use the "title" attribute to name the nodes, these names become parameter names in the `hordelib`. For example, a KSampler with the "title" of "sampler2" would become a parameter `sampler2.seed`, `sampler2.cfg`, etc. Load the pipeline `hordelib/pipeline_designs/pipeline_stable_diffusion.json` in the ComfyUI web app for an example.
 
@@ -867,15 +879,15 @@
 
 ### Standalone "clean" environment test from Pypi
 
 Here's an example:
 
 Start in a new empty directory. Create requirements.txt:
 ```
---extra-index-url https://download.pytorch.org/whl/cu117
+--extra-index-url https://download.pytorch.org/whl/cu118
 hordelib
 ```
 
 Create the directory `images/` and copy the `test_db0.jpg` into it.
 
 Copy `run_controlnet.py` from the `hordelib/tests/` directory.
 
@@ -926,14 +938,16 @@
 
 [pypi-image]: https://badge.fury.io/py/hordelib.svg?branch=main&kill_cache=1
 [pypi-url]: https://badge.fury.io/py/hordelib
 [downloads-image]: https://pepy.tech/badge/hordelib
 [downloads-url]: https://pepy.tech/project/hordelib
 [license-url]: https://img.shields.io/github/license/jug-dev/hordelib
 [build-image]: https://github.com/jug-dev/hordelib/actions/workflows/maintests.yml/badge.svg?branch=main
+[all-model-images]: https://badgen.net/badge/all-models/images/blue?icon=awesome
 [build-url]: http://hordelib.s3-website-eu-west-1.amazonaws.com/
 [main-test-image]: https://badgen.net/badge/main/latest-images/blue?icon=awesome
 [main-test-url]: http://hordelib.s3-website-eu-west-1.amazonaws.com/
 [pr-test-image]: https://badgen.net/badge/develop/latest-images/blue?icon=awesome
 [pr-test-url]: http://hordelib.s3-website-eu-west-1.amazonaws.com/unstable
+[all-model-url]: http://hordelib.s3-website-eu-west-1.amazonaws.com/all_models/
 [changelog-image]: https://img.shields.io/badge/Release-Changelog-yellow
 [changelog-url]: https://github.com/jug-dev/hordelib/blob/releases/CHANGELOG.md
```

### Comparing `hordelib-0.9.5/README.md` & `hordelib-1.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 [![PyPI Version][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 ![GitHub license][license-url]
 
 [![Build][build-image]][build-url]
 [![Test Images][main-test-image]][main-test-url]
 [![Test Images][pr-test-image]][pr-test-url]
+[![All Models][all-model-images]][all-model-url]
 [![Release Changelog][changelog-image]][changelog-url]
 
-`hordelib` is a thin wrapper around [ComfyUI](https://github.com/comfyanonymous/ComfyUI) primarily to enable the [AI Horde](https://aihorde.net/) to run inference pipelines designed visually in the ComfyUI GUI.
+`hordelib` is a wrapper around [ComfyUI](https://github.com/comfyanonymous/ComfyUI) primarily to enable the [AI Horde](https://aihorde.net/) to run inference pipelines designed visually in the ComfyUI GUI.
 
 The developers of `hordelib` can be found in the AI Horde Discord server: [https://discord.gg/3DxrhksKzn](https://discord.gg/3DxrhksKzn)
 
-NOTE: This project is in development and is not yet in use by Stable Horde.
+`hordelib` has been the default inference backend library of the [AI Horde](https://aihorde.net/) since `hordelib` v1.0.0.
 
 ## Purpose
 
 The goal here is to be able to design inference pipelines in the excellent ComfyUI, and then call those inference pipelines programmatically. Whilst providing features that maintain compatibility with the existing horde implementation.
 
 ## Installation
 
@@ -151,15 +152,26 @@
 `hordelib/pipelines/`
 Contains the above pipeline JSON files converted to the format required by the backend pipeline processor. These are converted from the web app, see _Converting ComfyUI pipelines_ below.
 
 `hordelib/nodes/` These are the custom ComfyUI nodes we use for `hordelib` specific processing.
 
 ### Running ComfyUI Web Application
 
-`tox -e comfyui`
+In this example we install the dependencies in the OS default environment. When using the git version of `hordelib`, from the project root:
+
+`pip install -r requirements.txt --extra-index-url https://download.pytorch.org/whl/cu118 --upgrade`
+
+Ensure ComfyUI is installed and patched, one way is running the tests:
+
+`tox`
+
+From then on to run ComfyUI:
+
+`cd ComfyUI`
+`python main.py`
 
 Then open a browser at: http://127.0.0.1:8188/
 
 ### Designing ComfyUI Pipelines
 
 Use the standard ComfyUI web app. Use the "title" attribute to name the nodes, these names become parameter names in the `hordelib`. For example, a KSampler with the "title" of "sampler2" would become a parameter `sampler2.seed`, `sampler2.cfg`, etc. Load the pipeline `hordelib/pipeline_designs/pipeline_stable_diffusion.json` in the ComfyUI web app for an example.
 
@@ -188,15 +200,15 @@
 
 ### Standalone "clean" environment test from Pypi
 
 Here's an example:
 
 Start in a new empty directory. Create requirements.txt:
 ```
---extra-index-url https://download.pytorch.org/whl/cu117
+--extra-index-url https://download.pytorch.org/whl/cu118
 hordelib
 ```
 
 Create the directory `images/` and copy the `test_db0.jpg` into it.
 
 Copy `run_controlnet.py` from the `hordelib/tests/` directory.
 
@@ -247,14 +259,16 @@
 
 [pypi-image]: https://badge.fury.io/py/hordelib.svg?branch=main&kill_cache=1
 [pypi-url]: https://badge.fury.io/py/hordelib
 [downloads-image]: https://pepy.tech/badge/hordelib
 [downloads-url]: https://pepy.tech/project/hordelib
 [license-url]: https://img.shields.io/github/license/jug-dev/hordelib
 [build-image]: https://github.com/jug-dev/hordelib/actions/workflows/maintests.yml/badge.svg?branch=main
+[all-model-images]: https://badgen.net/badge/all-models/images/blue?icon=awesome
 [build-url]: http://hordelib.s3-website-eu-west-1.amazonaws.com/
 [main-test-image]: https://badgen.net/badge/main/latest-images/blue?icon=awesome
 [main-test-url]: http://hordelib.s3-website-eu-west-1.amazonaws.com/
 [pr-test-image]: https://badgen.net/badge/develop/latest-images/blue?icon=awesome
 [pr-test-url]: http://hordelib.s3-website-eu-west-1.amazonaws.com/unstable
+[all-model-url]: http://hordelib.s3-website-eu-west-1.amazonaws.com/all_models/
 [changelog-image]: https://img.shields.io/badge/Release-Changelog-yellow
 [changelog-url]: https://github.com/jug-dev/hordelib/blob/releases/CHANGELOG.md
```

### Comparing `hordelib-0.9.5/build_helper.py` & `hordelib-1.0.0/build_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # build_helper.py
 # This is just a build helper script to build the pypi package.
 import argparse
 import os
 import shutil
 import subprocess
 
+# NOTE The following imports should *exactly* match those in `tests/meta/test_build_helper.py`
+# If `tests/meta/test_build_helper.py`, fails, include the imports missing in `release.yaml`.
+# and update [testenv:test-build-helper] in `tox.ini`.
 from hordelib import install_comfy
 from hordelib.consts import COMFYUI_VERSION
 
 
 def run(command):
     result = subprocess.run(command, shell=True, text=True)
     if result.returncode:
```

### Comparing `hordelib-0.9.5/examples/run_clip.py` & `hordelib-1.0.0/examples/run_clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/examples/run_controlnet.py` & `hordelib-1.0.0/examples/run_controlnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/examples/run_controlnet_annotator.py` & `hordelib-1.0.0/examples/run_controlnet_annotator.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/examples/run_facefix.py` & `hordelib-1.0.0/examples/run_facefix.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/examples/run_img2img.py` & `hordelib-1.0.0/examples/run_img2img.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/examples/run_img2img_hires.py` & `hordelib-1.0.0/examples/run_img2img_hires.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/examples/run_img2img_inpaint.py` & `hordelib-1.0.0/examples/run_img2img_inpaint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/examples/run_img2img_inpaint_mask.py` & `hordelib-1.0.0/examples/run_img2img_inpaint_mask.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/examples/run_img2img_outpaint.py` & `hordelib-1.0.0/examples/run_img2img_outpaint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/examples/run_inpainting.py` & `hordelib-1.0.0/examples/run_inpainting.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/examples/run_stress_test.py` & `hordelib-1.0.0/examples/run_stress_test_mixed.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,210 +1,224 @@
 # This tests running hordelib standalone, as an external caller would use it.
-# Call with: python -m test.run_stress_test
+# Call with: python -m test.run_stress_test_cnet
 # You need all the deps in whatever environment you are running this.
+import os
+import random
+import sys
+import threading
 import time
 
+from loguru import logger
+from PIL import Image
+
 if __name__ != "__main__":
     exit(0)
-import random
-
-random.seed(999)
 
 import hordelib
 
 hordelib.initialise(setup_logging=False)
+from hordelib.horde import HordeLib
+from hordelib.shared_model_manager import SharedModelManager
 
-import threading
+random.seed(999)
 
-from loguru import logger
-from PIL import Image
+if len(sys.argv) > 2:
+    print(f"Usage: {sys.argv[0]} [<iterations>]")
+    sys.exit(1)
+if len(sys.argv) == 2:
+    try:
+        ITERATIONS = int(sys.argv[1])
+    except ValueError:
+        print("Please provide an integer as the argument.")
+        sys.exit(1)
+else:
+    ITERATIONS = 50
 
-from hordelib.horde import HordeLib
-from hordelib.shared_model_manager import SharedModelManager
+logger.warning(f"Running for {ITERATIONS} iterations: {sys.argv}")
+
+out_dir = f"images/stresstest/{os.path.splitext(os.path.basename(sys.argv[0]))[0]}"
+os.makedirs(out_dir, exist_ok=True)
 
 generate = HordeLib()
-SharedModelManager.loadModelManagers(compvis=True, controlnet=True)
-SharedModelManager.manager.load("Deliberate")
-SharedModelManager.manager.load("Anything Diffusion")
-SharedModelManager.manager.load("Realistic Vision")
-SharedModelManager.manager.load("Papercutcraft")
+SharedModelManager.loadModelManagers(compvis=True, controlnet=True, codeformer=True, esrgan=True, gfpgan=True)
 
-models = ["Deliberate", "Anything Diffusion", "Realistic Vision", "Papercutcraft"]
-cnets = ["openpose", "canny", "fakescribbes", "hed", "depth"]
+models = ["Deliberate", "Anything Diffusion", "Realistic Vision", "URPM"]
+cnets = ["canny", "hed", "fakescribbles", "depth", "normal", "hough"]
+SAMPLERS_MAP = {
+    "k_euler": "euler",
+    "k_euler_a": "euler_ancestral",
+    "k_heun": "heun",
+    "k_dpm_2": "dpm_2",
+    "k_dpm_2_a": "dpm_2_ancestral",
+    "k_lms": "lms",
+    "k_dpm_fast": "dpm_fast",
+    "k_dpm_adaptive": "dpm_adaptive",
+    "k_dpmpp_2s_a": "dpmpp_2s_ancestral",
+    "k_dpmpp_sde": "dpmpp_sde",
+    "k_dpmpp_2m": "dpmpp_2m",
+    "ddim": "ddim",
+    "uni_pc": "uni_pc",
+    "uni_pc_bh2": "uni_pc_bh2",
+    "plms": "euler",
+}
+pp_models = [
+    "CodeFormers",
+    "GFPGAN",
+]
+pp_models_upscale = [
+    "RealESRGAN_x4plus",
+    "RealESRGAN_x2plus",
+    "NMKD_Siax",
+    "RealESRGAN_x4plus_anime_6B",
+    "4x_AnimeSharp",
+]
+
+for model in models:
+    SharedModelManager.manager.load(model)
+for model in pp_models:
+    SharedModelManager.manager.load(model)
+for model in pp_models_upscale:
+    SharedModelManager.manager.load(model)
 
 start_time = time.time()
 
-ITERATIONS = 1
-CONTROL_NET = True
-
 mutex = threading.Lock()
 count = 0
 
 
 def inc():
     with mutex:
         global count
         count += 1
+        return count
 
 
-def generate_images():
+def generate_images_cnet():
+    i = inc()
+    logger.info(f"Thread {threading.current_thread().ident} starting iteration {i}")
+    cnet_type = random.choice(cnets)
+    model = random.choice(models)
+    sampler = random.choice(list(SAMPLERS_MAP.keys()))
     data = {
-        "sampler_name": "k_dpmpp_2m",
+        "sampler_name": sampler,
         "cfg_scale": 7.5,
         "denoising_strength": 1.0,
         "seed": random.randint(1, 1000000000),
         "height": 512,
         "width": 512,
-        "karras": random.random() < 0.5,
+        "karras": True,
         "tiling": False,
         "hires_fix": False,
         "clip_skip": 1,
-        "control_type": None,
+        "control_type": cnet_type,
         "image_is_control": False,
-        "return_control_map": False,
-        "prompt": "an ancient llamia monster",
-        "ddim_steps": 25,
-        "n_iter": 1,
-        "model": random.choice(models),
-    }
-    horde = HordeLib()
-    pil_image = horde.basic_inference(data)
-    inc()
-
-
-def generate_images_portrait():
-    data = {
-        "sampler_name": "k_dpmpp_2m",
-        "cfg_scale": 7.5,
-        "denoising_strength": 1.0,
-        "seed": random.randint(1, 1000000000),
-        "height": 512,
-        "width": 768,
-        "karras": random.random() < 0.5,
-        "tiling": False,
-        "hires_fix": False,
-        "clip_skip": 1,
-        "control_type": None,
-        "image_is_control": False,
-        "return_control_map": False,
-        "prompt": "an ancient llamia monster",
+        "return_control_map": random.random() < 0.1,
+        "prompt": "a man walking in the snow",
         "ddim_steps": 25,
         "n_iter": 1,
-        "model": random.choice(models),
+        "model": model,
+        "source_image": Image.open("images/test_db0.jpg"),
+        "source_processing": "img2img",
     }
     horde = HordeLib()
     pil_image = horde.basic_inference(data)
-    inc()
+    pil_image.save(
+        f"{out_dir}/cnet_{model}_{sampler}_{cnet_type}_{threading.current_thread().ident}_{i}.webp",
+        quality=80,
+    )
 
 
-def generate_images_hires_fix():
+def generate_images_txt2img():
+    i = inc()
+    logger.info(f"Thread {threading.current_thread().ident} starting iteration {i}")
+    model = random.choice(models)
+    sampler = random.choice(list(SAMPLERS_MAP.keys()))
     data = {
-        "sampler_name": "k_dpmpp_2m",
+        "sampler_name": sampler,
         "cfg_scale": 7.5,
         "denoising_strength": 1.0,
         "seed": random.randint(1, 1000000000),
-        "height": 768,
-        "width": 768,
+        "height": random.choice([512, 768]),
+        "width": random.choice([512, 768]),
         "karras": random.random() < 0.5,
         "tiling": False,
-        "hires_fix": True,
+        "hires_fix": random.random() < 0.5,
         "clip_skip": 1,
         "control_type": None,
         "image_is_control": False,
         "return_control_map": False,
-        "prompt": "an ancient llamia monster",
+        "prompt": "a man walking in the snow",
         "ddim_steps": 25,
         "n_iter": 1,
-        "model": random.choice(models),
+        "model": model,
+        "source_image": None,
+        "source_processing": "txt2img",
     }
     horde = HordeLib()
     pil_image = horde.basic_inference(data)
-    inc()
+    pil_image.save(
+        f"{out_dir}/cnet_{model}_{sampler}_{threading.current_thread().ident}_{i}.webp",
+        quality=80,
+    )
 
 
-def generate_images_cnet():
-    if not CONTROL_NET:
-        return
+def generate_images_pp():
+    i = inc()
+    logger.info(f"Thread {threading.current_thread().ident} starting iteration {i}")
+    model = random.choice(pp_models)
     data = {
-        "sampler_name": "k_dpmpp_2m",
-        "cfg_scale": 7.5,
-        "denoising_strength": 1.0,
-        "seed": random.randint(1, 1000000000),
-        "height": 512,
-        "width": 768,
-        "karras": random.random() < 0.5,
-        "tiling": False,
-        "hires_fix": False,
-        "clip_skip": 1,
-        "control_type": random.choice(cnets),
-        "image_is_control": False,
-        "return_control_map": False,
-        "prompt": "a man walking in the snow",
-        "ddim_steps": 25,
-        "n_iter": 1,
-        "model": random.choice(models),
-        "source_image": Image.open("images/test_db0.jpg"),
-        "source_processing": "img2img",
+        "model": model,
+        "source_image": Image.open("images/test_facefix.png"),
     }
-    horde = HordeLib()
-    pil_image = horde.basic_inference(data)
-    inc()
+    pil_image = generate.image_facefix(data)
+    pil_image.save(
+        f"{out_dir}/pp_{model}_{threading.current_thread().ident}_{i}.webp",
+        quality=80,
+    )
 
 
-def generate_images_img2img():
+def generate_images_pp_upscale():
+    i = inc()
+    logger.info(f"Thread {threading.current_thread().ident} starting iteration {i}")
+    model = random.choice(pp_models_upscale)
     data = {
-        "sampler_name": "k_dpmpp_2m",
-        "cfg_scale": 7.5,
-        "denoising_strength": 0.4,
-        "seed": random.randint(1, 1000000000),
-        "height": 768,
-        "width": 512,
-        "karras": random.random() < 0.5,
-        "tiling": False,
-        "hires_fix": False,
-        "clip_skip": 1,
-        "control_type": None,
-        "image_is_control": False,
-        "return_control_map": False,
-        "prompt": "a dinosaur",
-        "ddim_steps": 25,
-        "n_iter": 1,
-        "model": random.choice(models),
+        "model": model,
         "source_image": Image.open("images/test_db0.jpg"),
-        "source_processing": "img2img",
     }
-    horde = HordeLib()
-    pil_image = horde.basic_inference(data)
-    inc()
+    pil_image = generate.image_upscale(data)
+    pil_image.save(
+        f"{out_dir}/pp_{model}_{threading.current_thread().ident}_{i}.webp",
+        quality=80,
+    )
 
 
 def run_iterations():
     for i in range(ITERATIONS):
-        generate_images()
-        generate_images_portrait()
-        generate_images_cnet()
-        generate_images_img2img()
-        generate_images_hires_fix()
+        funcs = [
+            generate_images_pp_upscale,
+            generate_images_pp,
+            generate_images_txt2img,
+            generate_images_txt2img,
+            generate_images_txt2img,
+            generate_images_txt2img,
+            generate_images_cnet,
+        ]
+        random.choice(funcs)()
 
 
 def main():
     global count
     count = 0
     threads = [
         threading.Thread(daemon=True, target=run_iterations),
         threading.Thread(daemon=True, target=run_iterations),
         threading.Thread(daemon=True, target=run_iterations),
+        threading.Thread(daemon=True, target=run_iterations),
+        threading.Thread(daemon=True, target=run_iterations),
     ]
     [x.start() for x in threads]
     [x.join() for x in threads if x]
 
-    expected_iterations = (ITERATIONS * 5) * len(threads)
     logger.warning(f"Test took {round(time.time() - start_time)} seconds ({count} generations)")
-    if expected_iterations != count:
-        logger.error("Test did not finsihed all iterations")
 
 
 main()
-
-# 275 seconds, 3 threads, 5 iterations, 5 tests = 3.6 seconds per gen
-# 311 seconds, 3 threads, 5 iterations, 5 tests, 1 at a time (mutex locked) = 4.14
-# 265 seconds, 3 threads, 5 iterations, 5 tests, sampler_mutex = 3.5 seconds per gen
```

### Comparing `hordelib-0.9.5/examples/run_txt2img.py` & `hordelib-1.0.0/examples/run_txt2img.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/examples/run_txt2img_hires.py` & `hordelib-1.0.0/examples/run_txt2img_hires.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/examples/run_upscale.py` & `hordelib-1.0.0/examples/run_upscale.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/LICENSE` & `hordelib-1.0.0/hordelib/_comfyui/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/README.md` & `hordelib-1.0.0/hordelib/_comfyui/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 - Saving/Loading workflows as Json files.
 - Nodes interface can be used to create complex workflows like one for [Hires fix](https://comfyanonymous.github.io/ComfyUI_examples/2_pass_txt2img/) or much more advanced ones.
 - [Area Composition](https://comfyanonymous.github.io/ComfyUI_examples/area_composition/)
 - [Inpainting](https://comfyanonymous.github.io/ComfyUI_examples/inpaint/) with both regular and inpainting models.
 - [ControlNet and T2I-Adapter](https://comfyanonymous.github.io/ComfyUI_examples/controlnet/)
 - [Upscale Models (ESRGAN, ESRGAN variants, SwinIR, Swin2SR, etc...)](https://comfyanonymous.github.io/ComfyUI_examples/upscale_models/)
 - [unCLIP Models](https://comfyanonymous.github.io/ComfyUI_examples/unclip/)
+- [GLIGEN](https://comfyanonymous.github.io/ComfyUI_examples/gligen/)
 - Starts up very fast.
 - Works fully offline: will never download anything.
 - [Config file](extra_model_paths.yaml.example) to set the search paths for models.
 
 Workflow examples can be found on the [Examples page](https://comfyanonymous.github.io/ComfyUI_examples/)
 
 ## Shortcuts
@@ -79,15 +80,15 @@
 
 Put your SD checkpoints (the huge ckpt/safetensors files) in: models/checkpoints
 
 Put your VAE in: models/vae
 
 At the time of writing this pytorch has issues with python versions higher than 3.10 so make sure your python/pip versions are 3.10.
 
-### AMD (Linux only)
+### AMD GPUs (Linux only)
 AMD users can install rocm and pytorch with pip if you don't have it already installed, this is the command to install the stable version:
 
 ```pip install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/rocm5.4.2```
 
 
 ### NVIDIA
```

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/cldm/cldm.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/cldm/cldm.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/cli_args.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/cli_args.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/clip_vision.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/clip_vision.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/diffusers_convert.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/diffusers_convert.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/extra_samplers/uni_pc.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/extra_samplers/uni_pc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/augmentation.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/k_diffusion/augmentation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/config.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/k_diffusion/config.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/evaluation.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/k_diffusion/evaluation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/external.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/k_diffusion/external.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/gns.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/k_diffusion/gns.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/layers.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/k_diffusion/layers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/models/image_v1.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/k_diffusion/models/image_v1.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/sampling.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/k_diffusion/sampling.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import torch
 from torch import nn
 from torchdiffeq import odeint
 import torchsde
 from tqdm.auto import trange, tqdm
 
 from . import utils
+from loguru import logger
+import threading
 
 
 def append_zero(x):
     return torch.cat([x, x.new_zeros([1])])
 
 
 def get_sigmas_karras(n, sigma_min, sigma_max, rho=7., device='cpu'):
@@ -580,28 +582,40 @@
             x = x + noise_sampler(sigma_fn(t), sigma_fn(t_next)) * s_noise * su
     return x
 
 
 @torch.no_grad()
 def sample_dpmpp_2m(model, x, sigmas, extra_args=None, callback=None, disable=None):
     """DPM-Solver++(2M)."""
+    # logger.warning(f"Starting DPM-Solver++(2M) on model {id(model):x}")
     extra_args = {} if extra_args is None else extra_args
     s_in = x.new_ones([x.shape[0]])
     sigma_fn = lambda t: t.neg().exp()
     t_fn = lambda sigma: sigma.log().neg()
     old_denoised = None
 
+    # logger.warning(f"Starting iterations of DPM-Solver++(2M) on model {id(model):x}")
     for i in trange(len(sigmas) - 1, disable=disable):
+        # logger.warning(f"Starting iterations {i} on model {id(model):x}")
+        # logger.warning(f"denoise = {id(model):x}({id(x):x}, {id(sigmas):x} * {id(s_in)}, {id(extra_args)})")
         denoised = model(x, sigmas[i] * s_in, **extra_args)
+        # logger.warning(f"  denoised on model {id(model):x}")
         if callback is not None:
             callback({'x': x, 'i': i, 'sigma': sigmas[i], 'sigma_hat': sigmas[i], 'denoised': denoised})
+        # logger.warning(f"  step 1 {id(model):x}")
         t, t_next = t_fn(sigmas[i]), t_fn(sigmas[i + 1])
+        # logger.warning(f"  step 2 {id(model):x}")
         h = t_next - t
+        # logger.warning(f"  step 3 {id(model):x}")
         if old_denoised is None or sigmas[i + 1] == 0:
+            # logger.warning(f"  step 3a {id(model):x}")
             x = (sigma_fn(t_next) / sigma_fn(t)) * x - (-h).expm1() * denoised
         else:
+            # logger.warning(f"  step 3b {id(model):x}")
             h_last = t - t_fn(sigmas[i - 1])
             r = h_last / h
             denoised_d = (1 + 1 / (2 * r)) * denoised - (1 / (2 * r)) * old_denoised
             x = (sigma_fn(t_next) / sigma_fn(t)) * x - (-h).expm1() * denoised_d
+        # logger.warning(f"  step 4 end iteration {id(model):x}")
         old_denoised = denoised
+    # logger.warning(f"Done DPM-Solver++(2M) on model {id(model):x}")
     return x
```

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/k_diffusion/utils.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/k_diffusion/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/data/util.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/data/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/autoencoder.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/models/autoencoder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/ddim.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/models/diffusion/ddim.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/ddpm.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/models/diffusion/ddpm.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/dpm_solver.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/dpm_solver.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/sampler.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/sampler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/plms.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/models/diffusion/plms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/models/diffusion/sampling_util.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/models/diffusion/sampling_util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/attention.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/attention.py`

 * *Files 4% similar despite different names*

```diff
@@ -451,31 +451,24 @@
         q = self.to_q(x)
         context = default(context, x)
         k = self.to_k(context)
         v = self.to_v(context)
 
         b, _, _ = q.shape
         q, k, v = map(
-            lambda t: t.unsqueeze(3)
-            .reshape(b, t.shape[1], self.heads, self.dim_head)
-            .permute(0, 2, 1, 3)
-            .reshape(b * self.heads, t.shape[1], self.dim_head)
-            .contiguous(),
+            lambda t: t.view(b, -1, self.heads, self.dim_head).transpose(1, 2),
             (q, k, v),
         )
 
         out = torch.nn.functional.scaled_dot_product_attention(q, k, v, attn_mask=None, dropout_p=0.0, is_causal=False)
 
         if exists(mask):
             raise NotImplementedError
         out = (
-            out.unsqueeze(0)
-            .reshape(b, self.heads, out.shape[1], self.dim_head)
-            .permute(0, 2, 1, 3)
-            .reshape(b, out.shape[1], self.heads * self.dim_head)
+            out.transpose(1, 2).reshape(b, -1, self.heads * self.dim_head)
         )
 
         return self.to_out(out)
 
 if model_management.xformers_enabled():
     print("Using xformers cross attention")
     CrossAttention = MemoryEfficientCrossAttention
@@ -506,27 +499,43 @@
         self.norm3 = nn.LayerNorm(dim)
         self.checkpoint = checkpoint
 
     def forward(self, x, context=None, transformer_options={}):
         return checkpoint(self._forward, (x, context, transformer_options), self.parameters(), self.checkpoint)
 
     def _forward(self, x, context=None, transformer_options={}):
+        current_index = None
+        if "current_index" in transformer_options:
+            current_index = transformer_options["current_index"]
+        if "patches" in transformer_options:
+            transformer_patches = transformer_options["patches"]
+        else:
+            transformer_patches = {}
+
         n = self.norm1(x)
         if "tomesd" in transformer_options:
             m, u = tomesd.get_functions(x, transformer_options["tomesd"]["ratio"], transformer_options["original_shape"])
             n = u(self.attn1(m(n), context=context if self.disable_self_attn else None))
         else:
             n = self.attn1(n, context=context if self.disable_self_attn else None)
 
         x += n
+        if "middle_patch" in transformer_patches:
+            patch = transformer_patches["middle_patch"]
+            for p in patch:
+                x = p(current_index, x)
+
         n = self.norm2(x)
         n = self.attn2(n, context=context)
 
         x += n
         x = self.ff(self.norm3(x)) + x
+
+        if current_index is not None:
+            transformer_options["current_index"] += 1
         return x
 
 
 class SpatialTransformer(nn.Module):
     """
     Transformer block for image-like data.
     First, project the input (aka embedding)
```

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/model.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/openaimodel.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/openaimodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -778,14 +778,16 @@
         :param x: an [N x C x ...] Tensor of inputs.
         :param timesteps: a 1-D batch of timesteps.
         :param context: conditioning plugged in via crossattn
         :param y: an [N] Tensor of labels, if class-conditional.
         :return: an [N x C x ...] Tensor of outputs.
         """
         transformer_options["original_shape"] = list(x.shape)
+        transformer_options["current_index"] = 0
+
         assert (y is not None) == (
             self.num_classes is not None
         ), "must specify y if and only if the model is class-conditional"
         hs = []
         t_emb = timestep_embedding(timesteps, self.model_channels, repeat_only=False)
         emb = self.time_embed(t_emb)
```

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/upscaling.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/upscaling.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/util.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/distributions/distributions.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/distributions/distributions.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/ema.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/ema.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/encoders/kornia_functions.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/encoders/kornia_functions.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/encoders/modules.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/encoders/modules.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/encoders/noise_aug_modules.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/encoders/noise_aug_modules.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan_light.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan_light.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/test.png` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/test.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils_image.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils_image.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/api.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/midas/api.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/blocks.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/dpt_depth.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net_custom.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/transforms.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/vit.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/midas/utils.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/midas/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/sub_quadratic_attention.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/sub_quadratic_attention.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/modules/tomesd.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/modules/tomesd.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/ldm/util.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/ldm/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/model_management.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/model_management.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import psutil
 from enum import Enum
 from cli_args import args
 import threading
 from loguru import logger
+from contextlib import nullcontext
 
 class VRAMState(Enum):
     CPU = 0
     NO_VRAM = 1
     LOW_VRAM = 2
     NORMAL_VRAM = 3
     HIGH_VRAM = 4
@@ -28,21 +29,14 @@
         import intel_extension_for_pytorch as ipex
         if torch.xpu.is_available():
             xpu_available = True
             total_vram = torch.xpu.get_device_properties(torch.xpu.current_device()).total_memory / (1024 * 1024)
     except:
         total_vram = torch.cuda.mem_get_info(torch.cuda.current_device())[1] / (1024 * 1024)
     total_ram = psutil.virtual_memory().total / (1024 * 1024)
-    if not args.normalvram and not args.cpu:
-        if total_vram <= 4096:
-            print("Trying to enable lowvram mode because your GPU seems to have 4GB or less. If you don't want this use: --normalvram")
-            set_vram_to = VRAMState.LOW_VRAM
-        elif total_vram > total_ram * 1.1 and total_vram > 14336:
-            print("Enabling highvram mode because your GPU has more vram than your computer has ram. If you don't want this use: --normalvram")
-            vram_state = VRAMState.HIGH_VRAM
 except:
     pass
 
 try:
     OOM_EXCEPTION = torch.cuda.OutOfMemoryError
 except:
     OOM_EXCEPTION = Exception
@@ -57,18 +51,18 @@
         import xformers.ops
         XFORMERS_IS_AVAILABLE = True
         try:
             XFORMERS_VERSION = xformers.version.__version__
             print("xformers version:", XFORMERS_VERSION)
             if XFORMERS_VERSION.startswith("0.0.18"):
                 print()
-                print("WARNING: This version of xformers has a major bug where you will get black images when generating high resolution images.")
-                print("Please downgrade or upgrade xformers to a different version.")
-                print()
-                XFORMERS_ENABLED_VAE = False
+                # print("WARNING: This version of xformers has a major bug where you will get black images when generating high resolution images.")
+                # print("Please downgrade or upgrade xformers to a different version.")
+                # print()
+                # XFORMERS_ENABLED_VAE = False
         except:
             pass
     except:
         XFORMERS_IS_AVAILABLE = False
 
 ENABLE_PYTORCH_ATTENTION = args.use_pytorch_cross_attention
 if ENABLE_PYTORCH_ATTENTION:
@@ -108,23 +102,27 @@
         vram_state = VRAMState.MPS
 except:
     pass
 
 if args.cpu:
     vram_state = VRAMState.CPU
 
-print(f"Set vram state to: {vram_state.name}")
+# print(f"Set vram state to: {vram_state.name}")
 
 
 class ModelManager:
     _instance = None
     _initialised = False
-    _mutex = threading.RLock()
+    _load_mutex = threading.RLock()
+    _property_mutex = threading.RLock()
     sampler_mutex = threading.RLock()
-    system_reserved_vram_mb = 6 * 1024
+    vae_mutex = threading.RLock()
+
+    _property_mutex = nullcontext()
+
     user_reserved_vram_mb = 0
 
     # We are a singleton
     def __new__(cls):
         if cls._instance is None:
             cls._instance = super().__new__(cls)
         return cls._instance
@@ -135,122 +133,150 @@
             self.models_in_use = []
             self.current_loaded_models = []
             self.current_gpu_controlnets = []
             self.models_accelerated = []
             self.__class__._initialised = True    
 
     def set_user_reserved_vram(self, vram_mb):
-        with self._mutex:
+        with self._property_mutex:
             self.user_reserved_vram_mb = vram_mb
 
     def get_models_on_gpu(self):
-        with self._mutex:
+        with self._property_mutex:
             return self.current_loaded_models[:]
 
-    def model_in_use(self, model):
-        with self._mutex:
+    def set_model_in_use(self, model):
+        with self._property_mutex:
+            self.models_in_use.append(model)
+
+    def is_model_in_use(self, model):
+        with self._property_mutex:
             return model in self.models_in_use
 
     def unload_model(self, model):
         global vram_state
-        with self._mutex:
+        with self._property_mutex:
             if model not in self.current_loaded_models:
                 logger.debug("Skip GPU unload as not on the GPU")
                 return
 
             if model in self.models_in_use:
                 logger.debug("Not unloaded model as it is in use right now")
                 return
 
             if model in self.models_accelerated:
                 accelerate.hooks.remove_hook_from_submodules(model.model)
                 self.models_accelerated.remove(model)
 
-            # Unload to RAM
-            model.model.cpu()
-            model.unpatch_model()
             self.current_loaded_models.remove(model)
 
+        # Unload to RAM
+        model.model.cpu()
+        model.unpatch_model()
+        return True
+
     def done_with_model(self, model):
-        with self._mutex:
+        with self._property_mutex:
             if model in self.models_in_use:
                 self.models_in_use.remove(model)
 
+    def have_free_vram(self):
+        freemem = round(get_free_memory(get_torch_device()) / (1024 * 1024))
+        logger.debug(f"Free VRAM is: {freemem}MB ({len(self.current_loaded_models)} models loaded on GPU)")
+        return freemem > self.user_reserved_vram_mb
+
     def load_model_gpu(self, model):
         global vram_state
-
-        with self._mutex:
+        
+        with self._load_mutex:
+            #logger.warning(f"load_model_gpu( {id(model):x} )")
 
             # Don't run out of vram
             if self.current_loaded_models:
-                freemem = round(get_free_memory(get_torch_device()) / (1024 * 1024))
-                logger.debug(f"Free VRAM is: {freemem}MB ({len(self.current_loaded_models)} models loaded on GPU)")
-                if freemem < (self.system_reserved_vram_mb + self.user_reserved_vram_mb):
-                    # release the least used model
-                    self.unload_model(self.current_loaded_models[-1])
+                if not self.have_free_vram():
+                    # Release the first least used model that we can
+                    for release_model in reversed(self.current_loaded_models):
+                        if self.unload_model(release_model):
+                            break
                     freemem = round(get_free_memory(get_torch_device()) / (1024 * 1024))
                     logger.debug(f"Unloaded a model, free VRAM is now: {freemem}MB ({len(self.current_loaded_models)} models loaded on GPU)")
 
             if model in self.current_loaded_models:
                 # Move this model to the top of the list
                 self.current_loaded_models.insert(0, self.current_loaded_models.pop(self.current_loaded_models.index(model)))
+                #logger.warning(f"Model {id(model):x} already on GPU so not loading")
                 return model
             
             try:
+                #logger.warning(f"Patching model {id(model):x}")
                 real_model = model.patch_model()
             except Exception as e:
+                logger.error("Patching failed")
                 model.unpatch_model()
                 raise e
             
+            #logger.warning(f"Adding model to current_loaded_models {id(model):x}")
             self.current_loaded_models.insert(0, model)
 
             if vram_state == VRAMState.CPU:
                 pass
             elif vram_state == VRAMState.MPS:
                 mps_device = torch.device("mps")
                 real_model.to(mps_device)
             elif vram_state == VRAMState.NORMAL_VRAM or vram_state == VRAMState.HIGH_VRAM:
                 if model in self.models_accelerated:
+                    #logger.warning(f"removing model from accelerated list {id(model):x}")
                     self.models_accelerated.remove(model)
+                #logger.warning(f"Moving model {id(model):x} / {id(real_model):x} to device {get_torch_device()}")
                 real_model.to(get_torch_device())
+                #logger.warning(f"Done moving model {id(model):x} / {id(real_model):x} to device {get_torch_device()}")
             else:
                 if vram_state == VRAMState.NO_VRAM:
                     device_map = accelerate.infer_auto_device_map(real_model, max_memory={0: "256MiB", "cpu": "16GiB"})
                 elif vram_state == VRAMState.LOW_VRAM:
                     device_map = accelerate.infer_auto_device_map(real_model, max_memory={0: "{}MiB".format(total_vram_available_mb), "cpu": "16GiB"})
 
                 accelerate.dispatch_model(real_model, device_map=device_map, main_device=get_torch_device())
                 self.models_accelerated.append(model)
             return model
 
-    def load_controlnet_gpu(self, models):        
-        global vram_state
-        with self._mutex:
+    def load_controlnet_gpu(self, control_models):
+        with self._load_mutex:
+            global vram_state
             if vram_state == VRAMState.CPU:
                 return
 
             if vram_state == VRAMState.LOW_VRAM or vram_state == VRAMState.NO_VRAM:
                 #don't load controlnets like this if low vram because they will be loaded right before running and unloaded right after
                 return
 
+            models = []
+            for m in control_models:
+                models += m.get_models()
+
             device = get_torch_device()
             for m in models:
                 if m not in self.current_gpu_controlnets:
+                    #logger.warning(f"Loaded controlnet {id(m):x} to GPU")
                     self.current_gpu_controlnets.append(m.to(device))
 
-    def unload_controlnet_gpu(self, models):        
-        global vram_state
-        with self._mutex:
+    def unload_controlnet_gpu(self, control_models):
+        with self._load_mutex:
+            global vram_state
             if vram_state == VRAMState.CPU:
                 return
 
             if vram_state == VRAMState.LOW_VRAM or vram_state == VRAMState.NO_VRAM:
                 #don't load controlnets like this if low vram because they will be loaded right before running and unloaded right after
                 return
 
+            models = []
+            for m in control_models:
+                models += m.get_models()
+
             for m in models:
                 if m in self.current_gpu_controlnets:
                     m.cpu()
                     self.current_gpu_controlnets.remove(m)
                     del m
 
 model_manager = ModelManager()
@@ -324,14 +350,16 @@
 
     if torch_free_too:
         return (mem_free_total, mem_free_torch)
     else:
         return mem_free_total
 
 def maximum_batch_area():
+    return 0
+    # See https://github.com/jug-dev/hordelib/issues/225
     global vram_state
     if vram_state == VRAMState.NO_VRAM:
         return 0
 
     memory_free = get_free_memory() / (1024 * 1024)
     area = ((memory_free - 1024) * 0.9) / (0.6)
     return int(max(area, 0))
```

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/samplers.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/samplers.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,46 +2,31 @@
 from .k_diffusion import external as k_diffusion_external
 from .extra_samplers import uni_pc
 import torch
 import contextlib
 from comfy import model_management
 from .ldm.models.diffusion.ddim import DDIMSampler
 from .ldm.modules.diffusionmodules.util import make_ddim_timesteps
-
-class CFGDenoiser(torch.nn.Module):
-    def __init__(self, model):
-        super().__init__()
-        self.inner_model = model
-
-    def forward(self, x, sigma, uncond, cond, cond_scale):
-        if len(uncond[0]) == len(cond[0]) and x.shape[0] * x.shape[2] * x.shape[3] < (96 * 96): #TODO check memory instead
-            x_in = torch.cat([x] * 2)
-            sigma_in = torch.cat([sigma] * 2)
-            cond_in = torch.cat([uncond, cond])
-            uncond, cond = self.inner_model(x_in, sigma_in, cond=cond_in).chunk(2)
-        else:
-            cond = self.inner_model(x, sigma, cond=cond)
-            uncond = self.inner_model(x, sigma, cond=uncond)
-        return uncond + (cond - uncond) * cond_scale
-
+from loguru import logger
+import threading
 
 #The main sampling function shared by all the samplers
 #Returns predicted noise
 def sampling_function(model_function, x, timestep, uncond, cond, cond_scale, cond_concat=None, model_options={}):
         def get_area_and_mult(cond, x_in, cond_concat_in, timestep_in):
             area = (x_in.shape[2], x_in.shape[3], 0, 0)
             strength = 1.0
             if 'area' in cond[1]:
                 area = cond[1]['area']
             if 'strength' in cond[1]:
                 strength = cond[1]['strength']
 
             adm_cond = None
-            if 'adm' in cond[1]:
-                adm_cond = cond[1]['adm']
+            if 'adm_encoded' in cond[1]:
+                adm_cond = cond[1]['adm_encoded']
 
             input_x = x_in[:,:,area[2]:area[0] + area[2],area[3]:area[1] + area[3]]
             mult = torch.ones_like(input_x) * strength
 
             rr = 8
             if area[2] != 0:
                 for t in range(rr):
@@ -66,15 +51,29 @@
 
             if adm_cond is not None:
                 conditionning['c_adm'] = adm_cond
 
             control = None
             if 'control' in cond[1]:
                 control = cond[1]['control']
-            return (input_x, mult, conditionning, area, control)
+
+            patches = None
+            if 'gligen' in cond[1]:
+                gligen = cond[1]['gligen']
+                patches = {}
+                gligen_type = gligen[0]
+                gligen_model = gligen[1]
+                if gligen_type == "position":
+                    gligen_patch = gligen_model.set_position(input_x.shape, gligen[2], input_x.device)
+                else:
+                    gligen_patch = gligen_model.set_empty(input_x.shape, input_x.device)
+
+                patches['middle_patch'] = [gligen_patch]
+
+            return (input_x, mult, conditionning, area, control, patches)
 
         def cond_equal_size(c1, c2):
             if c1 is c2:
                 return True
             if c1.keys() != c2.keys():
                 return False
             if 'c_crossattn' in c1:
@@ -87,20 +86,29 @@
                 if c1['c_adm'].shape != c2['c_adm'].shape:
                     return False
             return True
 
         def can_concat_cond(c1, c2):
             if c1[0].shape != c2[0].shape:
                 return False
+
+            #control
             if (c1[4] is None) != (c2[4] is None):
                 return False
             if c1[4] is not None:
                 if c1[4] is not c2[4]:
                     return False
 
+            #patches
+            if (c1[5] is None) != (c2[5] is None):
+                return False
+            if (c1[5] is not None):
+                if c1[5] is not c2[5]:
+                    return False
+
             return cond_equal_size(c1[2], c2[2])
 
         def cond_cat(c_list):
             c_crossattn = []
             c_concat = []
             c_adm = []
             for x in c_list:
@@ -116,106 +124,136 @@
             if len(c_concat) > 0:
                 out['c_concat'] = [torch.cat(c_concat)]
             if len(c_adm) > 0:
                 out['c_adm'] = torch.cat(c_adm)
             return out
 
         def calc_cond_uncond_batch(model_function, cond, uncond, x_in, timestep, max_total_area, cond_concat_in, model_options):
+            # #logger.warning("calc_cond_uncond_batch()")
             out_cond = torch.zeros_like(x_in)
             out_count = torch.ones_like(x_in)/100000.0
 
             out_uncond = torch.zeros_like(x_in)
             out_uncond_count = torch.ones_like(x_in)/100000.0
 
             COND = 0
             UNCOND = 1
 
             to_run = []
+            # #logger.warning("calc_cond_uncond_batch() 1")
             for x in cond:
                 p = get_area_and_mult(x, x_in, cond_concat_in, timestep)
                 if p is None:
                     continue
 
                 to_run += [(p, COND)]
+            #logger.warning("calc_cond_uncond_batch() 2")
             for x in uncond:
                 p = get_area_and_mult(x, x_in, cond_concat_in, timestep)
                 if p is None:
                     continue
 
                 to_run += [(p, UNCOND)]
 
+            #logger.warning("calc_cond_uncond_batch() 3")
             while len(to_run) > 0:
                 first = to_run[0]
                 first_shape = first[0][0].shape
                 to_batch_temp = []
                 for x in range(len(to_run)):
                     if can_concat_cond(to_run[x][0], first[0]):
                         to_batch_temp += [x]
 
+                #logger.warning("calc_cond_uncond_batch() 3a")
                 to_batch_temp.reverse()
                 to_batch = to_batch_temp[:1]
 
+                #logger.warning("calc_cond_uncond_batch() 3b")
                 for i in range(1, len(to_batch_temp) + 1):
                     batch_amount = to_batch_temp[:len(to_batch_temp)//i]
                     if (len(batch_amount) * first_shape[0] * first_shape[2] * first_shape[3] < max_total_area):
                         to_batch = batch_amount
                         break
 
+                #logger.warning("calc_cond_uncond_batch() 3c")
                 input_x = []
                 mult = []
                 c = []
                 cond_or_uncond = []
                 area = []
                 control = None
+                patches = None
                 for x in to_batch:
                     o = to_run.pop(x)
                     p = o[0]
                     input_x += [p[0]]
                     mult += [p[1]]
                     c += [p[2]]
                     area += [p[3]]
                     cond_or_uncond += [o[1]]
                     control = p[4]
+                    patches = p[5]
 
                 batch_chunks = len(cond_or_uncond)
                 input_x = torch.cat(input_x)
                 c = cond_cat(c)
                 timestep_ = torch.cat([timestep] * batch_chunks)
 
                 if control is not None:
                     c['control'] = control.get_control(input_x, timestep_, c['c_crossattn'], len(cond_or_uncond))
 
+                transformer_options = {}
                 if 'transformer_options' in model_options:
-                    c['transformer_options'] = model_options['transformer_options']
+                    transformer_options = model_options['transformer_options'].copy()
 
+                if patches is not None:
+                    transformer_options["patches"] = patches
+
+                c['transformer_options'] = transformer_options
+
+                model_management.model_manager.sampler_mutex.acquire()
                 output = model_function(input_x, timestep_, cond=c).chunk(batch_chunks)
+                #logger.warning(f"{threading.current_thread().ident}: calc_cond_uncond_batch() 3d del")
                 del input_x
+                model_management.model_manager.sampler_mutex.release()
 
-                model_management.throw_exception_if_processing_interrupted()
-
+                #logger.warning(f"{threading.current_thread().ident}: calc_cond_uncond_batch() 3d(comfy)")
+                # model_management.throw_exception_if_processing_interrupted()
+                
+                #logger.warning("calc_cond_uncond_batch() 3f")
                 for o in range(batch_chunks):
                     if cond_or_uncond[o] == COND:
                         out_cond[:,:,area[o][2]:area[o][0] + area[o][2],area[o][3]:area[o][1] + area[o][3]] += output[o] * mult[o]
                         out_count[:,:,area[o][2]:area[o][0] + area[o][2],area[o][3]:area[o][1] + area[o][3]] += mult[o]
                     else:
                         out_uncond[:,:,area[o][2]:area[o][0] + area[o][2],area[o][3]:area[o][1] + area[o][3]] += output[o] * mult[o]
                         out_uncond_count[:,:,area[o][2]:area[o][0] + area[o][2],area[o][3]:area[o][1] + area[o][3]] += mult[o]
+                #logger.warning("calc_cond_uncond_batch() 3g")
                 del mult
+                #logger.warning("calc_cond_uncond_batch() 3h")
+
 
+            #logger.warning("calc_cond_uncond_batch() 4")
             out_cond /= out_count
             del out_count
+            #logger.warning("calc_cond_uncond_batch() 5")
             out_uncond /= out_uncond_count
             del out_uncond_count
+            #logger.warning("calc_cond_uncond_batch() 6")
 
             return out_cond, out_uncond
 
-
+        #logger.warning("Entering main shared sampling function")
         max_total_area = model_management.maximum_batch_area()
+        #logger.warning("Entering main shared sampling function 2")
         cond, uncond = calc_cond_uncond_batch(model_function, cond, uncond, x, timestep, max_total_area, cond_concat, model_options)
-        return uncond + (cond - uncond) * cond_scale
+        if "sampler_cfg_function" in model_options:
+            return model_options["sampler_cfg_function"](cond, uncond, cond_scale)
+        else:
+            return uncond + (cond - uncond) * cond_scale
 
 
 class CompVisVDenoiser(k_diffusion_external.DiscreteVDDPMDenoiser):
     def __init__(self, model, quantize=False, device='cpu'):
         super().__init__(model, model.alphas_cumprod, quantize=quantize)
 
     def get_v(self, x, t, cond, **kwargs):
@@ -302,50 +340,50 @@
         return
     if 'area' in smallest[1]:
         if smallest[1]['area'] == c_area:
             return
     n = c[1].copy()
     conds += [[smallest[0], n]]
 
-
-def apply_control_net_to_equal_area(conds, uncond):
+def apply_empty_x_to_equal_area(conds, uncond, name, uncond_fill_func):
     cond_cnets = []
     cond_other = []
     uncond_cnets = []
     uncond_other = []
     for t in range(len(conds)):
         x = conds[t]
         if 'area' not in x[1]:
-            if 'control' in x[1] and x[1]['control'] is not None:
-                cond_cnets.append(x[1]['control'])
+            if name in x[1] and x[1][name] is not None:
+                cond_cnets.append(x[1][name])
             else:
                 cond_other.append((x, t))
     for t in range(len(uncond)):
         x = uncond[t]
         if 'area' not in x[1]:
-            if 'control' in x[1] and x[1]['control'] is not None:
-                uncond_cnets.append(x[1]['control'])
+            if name in x[1] and x[1][name] is not None:
+                uncond_cnets.append(x[1][name])
             else:
                 uncond_other.append((x, t))
 
     if len(uncond_cnets) > 0:
         return
 
     for x in range(len(cond_cnets)):
         temp = uncond_other[x % len(uncond_other)]
         o = temp[0]
-        if 'control' in o[1] and o[1]['control'] is not None:
+        if name in o[1] and o[1][name] is not None:
             n = o[1].copy()
-            n['control'] = cond_cnets[x]
+            n[name] = uncond_fill_func(cond_cnets, x)
             uncond += [[o[0], n]]
         else:
             n = o[1].copy()
-            n['control'] = cond_cnets[x]
+            n[name] = uncond_fill_func(cond_cnets, x)
             uncond[temp[1]] = [o[0], n]
 
+
 def encode_adm(noise_augmentor, conds, batch_size, device):
     for t in range(len(conds)):
         x = conds[t]
         if 'adm' in x[1]:
             adm_inputs = []
             weights = []
             noise_aug = []
@@ -367,18 +405,19 @@
                 noise_augment = 0.05
                 noise_level = round((noise_augmentor.max_noise_level - 1) * noise_augment)
                 c_adm, noise_level_emb = noise_augmentor(adm_out[:, :noise_augmentor.time_embed.dim], noise_level=torch.tensor([noise_level], device=device))
                 adm_out = torch.cat((c_adm, noise_level_emb), 1)
         else:
             adm_out = torch.zeros((1, noise_augmentor.time_embed.dim * 2), device=device)
         x[1] = x[1].copy()
-        x[1]["adm"] = torch.cat([adm_out] * batch_size)
+        x[1]["adm_encoded"] = torch.cat([adm_out] * batch_size)
 
     return conds
 
+
 class KSampler:
     SCHEDULERS = ["karras", "normal", "simple", "ddim_uniform"]
     SAMPLERS = ["euler", "euler_ancestral", "heun", "dpm_2", "dpm_2_ancestral",
                 "lms", "dpm_fast", "dpm_adaptive", "dpmpp_2s_ancestral", "dpmpp_sde",
                 "dpmpp_2m", "ddim", "uni_pc", "uni_pc_bh2"]
 
     def __init__(self, model, steps, device, sampler=None, scheduler=None, denoise=None, model_options={}):
@@ -436,44 +475,50 @@
             self.sigmas = sigmas[-(steps + 1):]
 
 
     def sample(self, noise, positive, negative, cfg, latent_image=None, start_step=None, last_step=None, force_full_denoise=False, denoise_mask=None):
         sigmas = self.sigmas
         sigma_min = self.sigma_min
 
+        #logger.warning("sampler step 1")
         if last_step is not None and last_step < (len(sigmas) - 1):
             sigma_min = sigmas[last_step]
             sigmas = sigmas[:last_step + 1]
             if force_full_denoise:
                 sigmas[-1] = 0
 
+        #logger.warning("sampler step 2")
         if start_step is not None:
             if start_step < (len(sigmas) - 1):
                 sigmas = sigmas[start_step:]
             else:
                 if latent_image is not None:
                     return latent_image
                 else:
                     return torch.zeros_like(noise)
 
+        #logger.warning("sampler step 3")
         positive = positive[:]
         negative = negative[:]
         #make sure each cond area has an opposite one with the same area
         for c in positive:
             create_cond_with_same_area_if_none(negative, c)
         for c in negative:
             create_cond_with_same_area_if_none(positive, c)
 
-        apply_control_net_to_equal_area(positive, negative)
+        apply_empty_x_to_equal_area(positive, negative, 'control', lambda cond_cnets, x: cond_cnets[x])
+        apply_empty_x_to_equal_area(positive, negative, 'gligen', lambda cond_cnets, x: cond_cnets[x])
 
+        #logger.warning("sampler step 5")
         if self.model.model.diffusion_model.dtype == torch.float16:
             precision_scope = torch.autocast
         else:
             precision_scope = contextlib.nullcontext
 
+        #logger.warning("sampler step 6")
         if hasattr(self.model, 'noise_augmentor'): #unclip
             positive = encode_adm(self.model.noise_augmentor, positive, noise.shape[0], self.device)
             negative = encode_adm(self.model.noise_augmentor, negative, noise.shape[0], self.device)
 
         extra_args = {"cond":positive, "uncond":negative, "cond_scale": cfg, "model_options": self.model_options}
 
         cond_concat = None
@@ -493,56 +538,61 @@
             extra_args["cond_concat"] = cond_concat
 
         if sigmas[0] != self.sigmas[0] or (self.denoise is not None and self.denoise < 1.0):
             max_denoise = False
         else:
             max_denoise = True
 
-        with model_management.model_manager.sampler_mutex:
-            with precision_scope(model_management.get_autocast_device(self.device)):
-                if self.sampler == "uni_pc":
-                    samples = uni_pc.sample_unipc(self.model_wrap, noise, latent_image, sigmas, sampling_function=sampling_function, max_denoise=max_denoise, extra_args=extra_args, noise_mask=denoise_mask)
-                elif self.sampler == "uni_pc_bh2":
-                    samples = uni_pc.sample_unipc(self.model_wrap, noise, latent_image, sigmas, sampling_function=sampling_function, max_denoise=max_denoise, extra_args=extra_args, noise_mask=denoise_mask, variant='bh2')
-                elif self.sampler == "ddim":
-                    timesteps = []
-                    for s in range(sigmas.shape[0]):
-                        timesteps.insert(0, self.model_wrap.sigma_to_t(sigmas[s]))
-                    noise_mask = None
-                    if denoise_mask is not None:
-                        noise_mask = 1.0 - denoise_mask
-                    sampler = DDIMSampler(self.model, device=self.device)
-                    sampler.make_schedule_timesteps(ddim_timesteps=timesteps, verbose=False)
-                    z_enc = sampler.stochastic_encode(latent_image, torch.tensor([len(timesteps) - 1] * noise.shape[0]).to(self.device), noise=noise, max_denoise=max_denoise)
-                    samples, _ = sampler.sample_custom(ddim_timesteps=timesteps,
-                                                        conditioning=positive,
-                                                        batch_size=noise.shape[0],
-                                                        shape=noise.shape[1:],
-                                                        verbose=False,
-                                                        unconditional_guidance_scale=cfg,
-                                                        unconditional_conditioning=negative,
-                                                        eta=0.0,
-                                                        x_T=z_enc,
-                                                        x0=latent_image,
-                                                        denoise_function=sampling_function,
-                                                        extra_args=extra_args,
-                                                        mask=noise_mask,
-                                                        to_zero=sigmas[-1]==0,
-                                                        end_step=sigmas.shape[0] - 1)
+        #logger.warning("sampler step 7")
+        with precision_scope(model_management.get_autocast_device(self.device)):
+            #logger.warning("sampler step 7a")
+            if self.sampler == "uni_pc":
+                samples = uni_pc.sample_unipc(self.model_wrap, noise, latent_image, sigmas, sampling_function=sampling_function, max_denoise=max_denoise, extra_args=extra_args, noise_mask=denoise_mask)
+            elif self.sampler == "uni_pc_bh2":
+                samples = uni_pc.sample_unipc(self.model_wrap, noise, latent_image, sigmas, sampling_function=sampling_function, max_denoise=max_denoise, extra_args=extra_args, noise_mask=denoise_mask, variant='bh2')
+            elif self.sampler == "ddim":
+                timesteps = []
+                for s in range(sigmas.shape[0]):
+                    timesteps.insert(0, self.model_wrap.sigma_to_t(sigmas[s]))
+                noise_mask = None
+                if denoise_mask is not None:
+                    noise_mask = 1.0 - denoise_mask
+                sampler = DDIMSampler(self.model, device=self.device)
+                sampler.make_schedule_timesteps(ddim_timesteps=timesteps, verbose=False)
+                z_enc = sampler.stochastic_encode(latent_image, torch.tensor([len(timesteps) - 1] * noise.shape[0]).to(self.device), noise=noise, max_denoise=max_denoise)
+                samples, _ = sampler.sample_custom(ddim_timesteps=timesteps,
+                                                    conditioning=positive,
+                                                    batch_size=noise.shape[0],
+                                                    shape=noise.shape[1:],
+                                                    verbose=False,
+                                                    unconditional_guidance_scale=cfg,
+                                                    unconditional_conditioning=negative,
+                                                    eta=0.0,
+                                                    x_T=z_enc,
+                                                    x0=latent_image,
+                                                    denoise_function=sampling_function,
+                                                    extra_args=extra_args,
+                                                    mask=noise_mask,
+                                                    to_zero=sigmas[-1]==0,
+                                                    end_step=sigmas.shape[0] - 1)
+
+            else:
+                #logger.warning("sampler step 7b")
+                extra_args["denoise_mask"] = denoise_mask
+                self.model_k.latent_image = latent_image
+                self.model_k.noise = noise
 
+                noise = noise * sigmas[0]
+
+                if latent_image is not None:
+                    noise += latent_image
+                if self.sampler == "dpm_fast":
+                    #logger.warning("sampler sample_dpm_fast")
+                    samples = k_diffusion_sampling.sample_dpm_fast(self.model_k, noise, sigma_min, sigmas[0], self.steps, extra_args=extra_args)
+                elif self.sampler == "dpm_adaptive":
+                    #logger.warning("sampler sample_dpm_adaptive")
+                    samples = k_diffusion_sampling.sample_dpm_adaptive(self.model_k, noise, sigma_min, sigmas[0], extra_args=extra_args)
                 else:
-                    extra_args["denoise_mask"] = denoise_mask
-                    self.model_k.latent_image = latent_image
-                    self.model_k.noise = noise
-
-                    noise = noise * sigmas[0]
-
-                    if latent_image is not None:
-                        noise += latent_image
-                    if self.sampler == "dpm_fast":
-                        samples = k_diffusion_sampling.sample_dpm_fast(self.model_k, noise, sigma_min, sigmas[0], self.steps, extra_args=extra_args)
-                    elif self.sampler == "dpm_adaptive":
-                        samples = k_diffusion_sampling.sample_dpm_adaptive(self.model_k, noise, sigma_min, sigmas[0], extra_args=extra_args)
-                    else:
-                        samples = getattr(k_diffusion_sampling, "sample_{}".format(self.sampler))(self.model_k, noise, sigmas, extra_args=extra_args)
+                    #logger.warning("sampler: "+"sample_{}".format(self.sampler))
+                    samples = getattr(k_diffusion_sampling, "sample_{}".format(self.sampler))(self.model_k, noise, sigmas, extra_args=extra_args)
 
         return samples.to(torch.float32)
```

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/sd.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/sd.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 from .ldm.models.autoencoder import AutoencoderKL
 import yaml
 from .cldm import cldm
 from .t2i_adapter import adapter
 
 from . import utils
 from . import clip_vision
+from loguru import logger
+import threading
+from . import gligen
 
 def load_model_weights(model, sd, verbose=False, load_state_dict_to=[]):
     m, u = model.load_state_dict(sd, strict=False)
 
     k = list(sd.keys())
     for x in k:
         # print(x)
@@ -247,14 +250,17 @@
         n.patches = self.patches[:]
         n.model_options = copy.deepcopy(self.model_options)
         return n
 
     def set_model_tomesd(self, ratio):
         self.model_options["transformer_options"]["tomesd"] = {"ratio": ratio}
 
+    def set_model_sampler_cfg_function(self, sampler_cfg_function):
+        self.model_options["sampler_cfg_function"] = sampler_cfg_function
+
     def model_dtype(self):
         return self.model.diffusion_model.dtype
 
     def add_patches(self, patches, strength=1.0):
         p = {}
         model_sd = self.model.state_dict()
         for k in patches:
@@ -262,14 +268,15 @@
                 p[k] = patches[k]
         self.patches += [(strength, p)]
         return p.keys()
 
     def patch_model(self):
         model_sd = self.model.state_dict()
         for p in self.patches:
+            #logger.warning(f"Patching model {id(self):x} {len(self.patches)} patches")
             for k in p[1]:
                 v = p[1][k]
                 key = k
                 if key not in model_sd:
                     print("could not patch. key doesn't exist in model:", k)
                     continue
 
@@ -372,24 +379,28 @@
 
     def clip_layer(self, layer_idx):
         self.layer_idx = layer_idx
 
     def tokenize(self, text, return_word_ids=False):
         return self.tokenizer.tokenize_with_weights(text, return_word_ids)
 
-    def encode_from_tokens(self, tokens):
+    def encode_from_tokens(self, tokens, return_pooled=False):
         if self.layer_idx is not None:
             self.cond_stage_model.clip_layer(self.layer_idx)
         try:
             self.patcher.patch_model()
             cond = self.cond_stage_model.encode_token_weights(tokens)
             self.patcher.unpatch_model()
         except Exception as e:
             self.patcher.unpatch_model()
             raise e
+        if return_pooled:
+            eos_token_index = max(range(len(tokens[0])), key=tokens[0].__getitem__)
+            pooled = cond[:, eos_token_index]
+            return cond, pooled
         return cond
 
     def encode(self, text):
         tokens = self.tokenize(text)
         return self.encode_from_tokens(tokens)
 
 class VAE:
@@ -412,56 +423,80 @@
             (utils.tiled_scale(samples, decode_fn, tile_x // 2, tile_y * 2, overlap, upscale_amount = 8) +
             utils.tiled_scale(samples, decode_fn, tile_x * 2, tile_y // 2, overlap, upscale_amount = 8) +
              utils.tiled_scale(samples, decode_fn, tile_x, tile_y, overlap, upscale_amount = 8))
             / 3.0) / 2.0, min=0.0, max=1.0)
         return output
 
     def decode(self, samples_in):
-        self.first_stage_model = self.first_stage_model.to(self.device)
-        try:
-            free_memory = model_management.get_free_memory(self.device)
-            batch_number = int((free_memory * 0.7) / (2562 * samples_in.shape[2] * samples_in.shape[3] * 64))
-            batch_number = max(1, batch_number)
-
-            pixel_samples = torch.empty((samples_in.shape[0], 3, round(samples_in.shape[2] * 8), round(samples_in.shape[3] * 8)), device="cpu")
-            for x in range(0, samples_in.shape[0], batch_number):
-                samples = samples_in[x:x+batch_number].to(self.device)
-                pixel_samples[x:x+batch_number] = torch.clamp((self.first_stage_model.decode(1. / self.scale_factor * samples) + 1.0) / 2.0, min=0.0, max=1.0).cpu()
-        except model_management.OOM_EXCEPTION as e:
-            print("Warning: Ran out of memory when regular VAE decoding, retrying with tiled VAE decoding.")
-            pixel_samples = self.decode_tiled_(samples_in)
-
-        self.first_stage_model = self.first_stage_model.cpu()
-        pixel_samples = pixel_samples.cpu().movedim(1,-1)
-        return pixel_samples
+        with model_management.model_manager.vae_mutex:
+            tid = threading.current_thread().ident
+            #logger.warning(f"VAE.decode({tid}) would unload model")
+            # model_management.unload_model()
+
+            #logger.warning(f"VAE.decode({tid}) first_stage_model to device {self.device}")
+            self.first_stage_model = self.first_stage_model.to(self.device)
+            try:
+                #logger.warning(f"VAE.decode({tid}) get free memory")
+                free_memory = model_management.get_free_memory(self.device)
+                batch_number = int((free_memory * 0.7) / (2562 * samples_in.shape[2] * samples_in.shape[3] * 64))
+                batch_number = max(1, batch_number)
+                #logger.warning(f"VAE.decode({tid}) {batch_number} batches")
+
+                #logger.warning(f"VAE.decode({tid}) torch.empty")
+                pixel_samples = torch.empty((samples_in.shape[0], 3, round(samples_in.shape[2] * 8), round(samples_in.shape[3] * 8)), device="cpu")
+                #logger.warning(f"VAE.decode({tid}) starting iterations")
+                for x in range(0, samples_in.shape[0], batch_number):
+                    samples = samples_in[x:x+batch_number].to(self.device)
+                    #logger.warning(f"VAE.decode({tid}) got samples")
+                    pixel_samples[x:x+batch_number] = torch.clamp((self.first_stage_model.decode(1. / self.scale_factor * samples) + 1.0) / 2.0, min=0.0, max=1.0).cpu()
+                    #logger.warning(f"VAE.decode({tid}) clamped")
+            except model_management.OOM_EXCEPTION as e:
+                print("Warning: Ran out of memory when regular VAE decoding, retrying with tiled VAE decoding.")
+                pixel_samples = self.decode_tiled_(samples_in)
+
+            #logger.warning(f"VAE.decode({tid}) moving to cpu")
+            self.first_stage_model = self.first_stage_model.cpu()
+            #logger.warning(f"VAE.decode({tid}) calculating pixels")
+            pixel_samples = pixel_samples.cpu().movedim(1,-1)
+            #logger.warning(f"VAE.decode({tid}) returning")
+            return pixel_samples
 
     def decode_tiled(self, samples, tile_x=64, tile_y=64, overlap = 16):
-        self.first_stage_model = self.first_stage_model.to(self.device)
-        output = self.decode_tiled_(samples, tile_x, tile_y, overlap)
-        self.first_stage_model = self.first_stage_model.cpu()
-        return output.movedim(1,-1)
+        with model_management.model_manager.vae_mutex:
+            #logger.warning("VAE.decode_tiled() would unload model")
+            # model_management.unload_model()
+            self.first_stage_model = self.first_stage_model.to(self.device)
+            output = self.decode_tiled_(samples, tile_x, tile_y, overlap)
+            self.first_stage_model = self.first_stage_model.cpu()
+            return output.movedim(1,-1)
 
     def encode(self, pixel_samples):
-        self.first_stage_model = self.first_stage_model.to(self.device)
-        pixel_samples = pixel_samples.movedim(-1,1).to(self.device)
-        samples = self.first_stage_model.encode(2. * pixel_samples - 1.).sample() * self.scale_factor
-        self.first_stage_model = self.first_stage_model.cpu()
-        samples = samples.cpu()
-        return samples
+        #logger.warning("VAE.encode() would unload model")
+        # model_management.unload_model()
+        with model_management.model_manager.vae_mutex:
+            self.first_stage_model = self.first_stage_model.to(self.device)
+            pixel_samples = pixel_samples.movedim(-1,1).to(self.device)
+            samples = self.first_stage_model.encode(2. * pixel_samples - 1.).sample() * self.scale_factor
+            self.first_stage_model = self.first_stage_model.cpu()
+            samples = samples.cpu()
+            return samples
 
     def encode_tiled(self, pixel_samples, tile_x=512, tile_y=512, overlap = 64):
-        self.first_stage_model = self.first_stage_model.to(self.device)
-        pixel_samples = pixel_samples.movedim(-1,1).to(self.device)
-        samples = utils.tiled_scale(pixel_samples, lambda a: self.first_stage_model.encode(2. * a - 1.).sample() * self.scale_factor, tile_x, tile_y, overlap, upscale_amount = (1/8), out_channels=4)
-        samples += utils.tiled_scale(pixel_samples, lambda a: self.first_stage_model.encode(2. * a - 1.).sample() * self.scale_factor, tile_x * 2, tile_y // 2, overlap, upscale_amount = (1/8), out_channels=4)
-        samples += utils.tiled_scale(pixel_samples, lambda a: self.first_stage_model.encode(2. * a - 1.).sample() * self.scale_factor, tile_x // 2, tile_y * 2, overlap, upscale_amount = (1/8), out_channels=4)
-        samples /= 3.0
-        self.first_stage_model = self.first_stage_model.cpu()
-        samples = samples.cpu()
-        return samples
+        #logger.warning("VAE.decode() would unload model")
+        # model_management.unload_model()
+        with model_management.model_manager.vae_mutex:
+            self.first_stage_model = self.first_stage_model.to(self.device)
+            pixel_samples = pixel_samples.movedim(-1,1).to(self.device)
+            samples = utils.tiled_scale(pixel_samples, lambda a: self.first_stage_model.encode(2. * a - 1.).sample() * self.scale_factor, tile_x, tile_y, overlap, upscale_amount = (1/8), out_channels=4)
+            samples += utils.tiled_scale(pixel_samples, lambda a: self.first_stage_model.encode(2. * a - 1.).sample() * self.scale_factor, tile_x * 2, tile_y // 2, overlap, upscale_amount = (1/8), out_channels=4)
+            samples += utils.tiled_scale(pixel_samples, lambda a: self.first_stage_model.encode(2. * a - 1.).sample() * self.scale_factor, tile_x // 2, tile_y * 2, overlap, upscale_amount = (1/8), out_channels=4)
+            samples /= 3.0
+            self.first_stage_model = self.first_stage_model.cpu()
+            samples = samples.cpu()
+            return samples
 
 def resize_image_to(tensor, target_latent_tensor, batched_number):
     tensor = utils.common_upscale(tensor, target_latent_tensor.shape[3] * 8, target_latent_tensor.shape[2] * 8, 'nearest-exact', "center")
     target_batch_size = target_latent_tensor.shape[0]
 
     current_batch_size = tensor.shape[0]
     print(current_batch_size, target_batch_size)
@@ -554,31 +589,29 @@
 
     def copy(self):
         c = ControlNet(self.control_model)
         c.cond_hint_original = self.cond_hint_original
         c.strength = self.strength
         return c
 
-    def get_control_models(self):
+    def get_models(self):
         out = []
         if self.previous_controlnet is not None:
-            out += self.previous_controlnet.get_control_models()
+            out += self.previous_controlnet.get_models()
         out.append(self.control_model)
         return out
 
 _controlnet_models = {}
-_mutex = threading.Lock()
 
 def load_controlnet(ckpt_path, model=None):
-    with _mutex:
-        if ckpt_path in _controlnet_models:
-            controlnet_data = copy.deepcopy(_controlnet_models.get(ckpt_path))
-        else:
-            controlnet_data = utils.load_torch_file(ckpt_path)
-            _controlnet_models[ckpt_path] = copy.deepcopy(controlnet_data)
+    if ckpt_path in _controlnet_models:
+        controlnet_data = copy.deepcopy(_controlnet_models.get(ckpt_path))
+    else:
+        controlnet_data = utils.load_torch_file(ckpt_path)
+        _controlnet_models[ckpt_path] = copy.deepcopy(controlnet_data)
 
     pth_key = 'control_model.input_blocks.1.1.transformer_blocks.0.attn2.to_k.weight'
     pth = False
     sd2 = False
     key = 'input_blocks.1.1.transformer_blocks.0.attn2.to_k.weight'
     if pth_key in controlnet_data:
         pth = True
@@ -631,14 +664,15 @@
                                         legacy=False,
                                         use_fp16=use_fp16)
     if pth:
         if 'difference' in controlnet_data:
             if model is not None:
                 m = model.patch_model()
                 model_sd = m.state_dict()
+                #logger.warning(f"Modifying model {id(model):x} with controlnet {id(controlnet_data):x}")
                 for x in controlnet_data:
                     c_m = "control_model."
                     if x.startswith(c_m):
                         sd_key = "model.diffusion_model.{}".format(x[len(c_m):])
                         if sd_key in model_sd:
                             cd = controlnet_data[x]
                             cd += model_sd[sd_key].type(cd.dtype).to(cd.device)
@@ -736,18 +770,18 @@
     def cleanup(self):
         if self.previous_controlnet is not None:
             self.previous_controlnet.cleanup()
         if self.cond_hint is not None:
             del self.cond_hint
             self.cond_hint = None
 
-    def get_control_models(self):
+    def get_models(self):
         out = []
         if self.previous_controlnet is not None:
-            out += self.previous_controlnet.get_control_models()
+            out += self.previous_controlnet.get_models()
         return out
 
 def load_t2i_adapter(t2i_data):
     keys = t2i_data.keys()
     if "body.0.in_conv.weight" in keys:
         cin = t2i_data['body.0.in_conv.weight'].shape[1]
         model_ad = adapter.Adapter_light(cin=cin, channels=[320, 640, 1280, 1280], nums_rb=4)
@@ -786,14 +820,21 @@
         config['target'] = 'ldm.modules.encoders.modules.FrozenOpenCLIPEmbedder'
     else:
         config['target'] = 'ldm.modules.encoders.modules.FrozenCLIPEmbedder'
     clip = CLIP(config=config, embedding_directory=embedding_directory)
     clip.load_from_state_dict(clip_data)
     return clip
 
+def load_gligen(ckpt_path):
+    data = utils.load_torch_file(ckpt_path)
+    model = gligen.load_gligen(data)
+    if model_management.should_use_fp16():
+        model = model.half()
+    return model
+
 def load_checkpoint(config_path, ckpt_path, output_vae=True, output_clip=True, embedding_directory=None):
     with open(config_path, 'r') as stream:
         config = yaml.safe_load(stream)
     model_config_params = config['model']['params']
     clip_config = model_config_params['cond_stage_config']
     scale_factor = model_config_params['scale_factor']
     vae_config = model_config_params['first_stage_config']
```

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/sd1_clip.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/sd1_clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/sd1_clip_config.json` & `hordelib-1.0.0/hordelib/_comfyui/comfy/sd1_clip_config.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/sd1_tokenizer/merges.txt` & `hordelib-1.0.0/hordelib/_comfyui/comfy/sd1_tokenizer/merges.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/sd1_tokenizer/tokenizer_config.json` & `hordelib-1.0.0/hordelib/_comfyui/comfy/sd1_tokenizer/tokenizer_config.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/sd1_tokenizer/vocab.json` & `hordelib-1.0.0/hordelib/_comfyui/comfy/sd1_tokenizer/vocab.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/sd2_clip.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/sd2_clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/sd2_clip_config.json` & `hordelib-1.0.0/hordelib/_comfyui/comfy/sd2_clip_config.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/t2i_adapter/adapter.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/t2i_adapter/adapter.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy/utils.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/HAT.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/HAT.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-ESRGAN` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-ESRGAN`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-HAT` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-HAT`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-RealESRGAN` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-RealESRGAN`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SPSR` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SPSR`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwiftSRGAN` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwiftSRGAN`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-Swin2SR` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-Swin2SR`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwinIR` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwinIR`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-lama` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-lama`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-mat` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-mat`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LaMa.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LaMa.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/MAT.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/MAT.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/RRDB.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/RRDB.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SPSR.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SPSR.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SRVGG.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SRVGG.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwiftSRGAN.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwiftSRGAN.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/Swin2SR.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/Swin2SR.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwinIR.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwinIR.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/block.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/block.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-GFPGAN` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-GFPGAN`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-RestoreFormer` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-RestoreFormer`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-codeformer` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-codeformer`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/arcface_arch.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/arcface_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/codeformer.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/codeformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/fused_act.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/fused_act.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpgan_bilinear_arch.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpgan_bilinear_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_arch.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_clean_arch.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_clean_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/restoreformer_arch.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/restoreformer_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_arch.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_bilinear_arch.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_bilinear_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_clean_arch.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_clean_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/upfirdn2d.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/utils.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/LICENSE` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/drop.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/drop.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/helpers.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/helpers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/weight_init.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/weight_init.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/model_loading.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/model_loading.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/chainner_models/types.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/chainner_models/types.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/nodes_mask.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/nodes_mask.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/nodes_post_processing.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/nodes_post_processing.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfy_extras/nodes_upscale_model.py` & `hordelib-1.0.0/hordelib/_comfyui/comfy_extras/nodes_upscale_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 from comfy_extras.chainner_models import model_loading
 from comfy import model_management
 import torch
 import comfy.utils
 import folder_paths
+import threading
 
 class UpscaleModelLoader:
     @classmethod
     def INPUT_TYPES(s):
         return {"required": { "model_name": (folder_paths.get_filename_list("upscale_models"), ),
                              }}
     RETURN_TYPES = ("UPSCALE_MODEL",)
@@ -19,30 +20,32 @@
         model_path = folder_paths.get_full_path("upscale_models", model_name)
         sd = comfy.utils.load_torch_file(model_path)
         out = model_loading.load_state_dict(sd).eval()
         return (out, )
 
 
 class ImageUpscaleWithModel:
+    _mutex = threading.Lock()
     @classmethod
     def INPUT_TYPES(s):
         return {"required": { "upscale_model": ("UPSCALE_MODEL",),
                               "image": ("IMAGE",),
                               }}
     RETURN_TYPES = ("IMAGE",)
     FUNCTION = "upscale"
 
     CATEGORY = "image/upscaling"
 
     def upscale(self, upscale_model, image):
-        device = model_management.get_torch_device()
-        upscale_model.to(device)
-        in_img = image.movedim(-1,-3).to(device)
-        s = comfy.utils.tiled_scale(in_img, lambda a: upscale_model(a), tile_x=128 + 64, tile_y=128 + 64, overlap = 8, upscale_amount=upscale_model.scale)
-        upscale_model.cpu()
-        s = torch.clamp(s.movedim(-3,-1), min=0, max=1.0)
-        return (s,)
+        with ImageUpscaleWithModel._mutex:
+            device = model_management.get_torch_device()
+            upscale_model.to(device)
+            in_img = image.movedim(-1,-3).to(device)
+            s = comfy.utils.tiled_scale(in_img, lambda a: upscale_model(a), tile_x=128 + 64, tile_y=128 + 64, overlap = 8, upscale_amount=upscale_model.scale)
+            upscale_model.cpu()
+            s = torch.clamp(s.movedim(-3,-1), min=0, max=1.0)
+            return (s,)
 
 NODE_CLASS_MAPPINGS = {
     "UpscaleModelLoader": UpscaleModelLoader,
     "ImageUpscaleWithModel": ImageUpscaleWithModel
 }
```

### Comparing `hordelib-0.9.5/hordelib/_comfyui/comfyui_screenshot.png` & `hordelib-1.0.0/hordelib/_comfyui/comfyui_screenshot.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/custom_nodes/example_node.py.example` & `hordelib-1.0.0/hordelib/_comfyui/custom_nodes/example_node.py.example`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/execution.py` & `hordelib-1.0.0/hordelib/_comfyui/execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,16 +200,16 @@
                 for x in executed:
                     self.old_prompt[x] = copy.deepcopy(prompt[x])
             finally:
                 self.server.last_node_id = None
                 if self.server.client_id is not None:
                     self.server.send_sync("executing", { "node": None }, self.server.client_id)
 
-        gc.collect()
-        comfy.model_management.soft_empty_cache()
+        # gc.collect()
+        # comfy.model_management.soft_empty_cache()
 
 
 def validate_inputs(prompt, item):
     unique_id = item
     inputs = prompt[unique_id]['inputs']
     class_type = prompt[unique_id]['class_type']
     obj_class = nodes.NODE_CLASS_MAPPINGS[class_type]
```

### Comparing `hordelib-0.9.5/hordelib/_comfyui/extra_model_paths.yaml.example` & `hordelib-1.0.0/hordelib/_comfyui/extra_model_paths.yaml.example`

 * *Files 21% similar despite different names*

```diff
@@ -14,10 +14,11 @@
                   models/SwinIR
     embeddings: embeddings
     controlnet: models/ControlNet
 
 #other_ui:
 #    base_path: path/to/ui
 #    checkpoints: models/checkpoints
+#    gligen: models/gligen
 #    custom_nodes: path/custom_nodes
```

### Comparing `hordelib-0.9.5/hordelib/_comfyui/folder_paths.py` & `hordelib-1.0.0/hordelib/_comfyui/folder_paths.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 folder_names_and_paths["clip"] = ([os.path.join(models_dir, "clip")], supported_pt_extensions)
 folder_names_and_paths["clip_vision"] = ([os.path.join(models_dir, "clip_vision")], supported_pt_extensions)
 folder_names_and_paths["style_models"] = ([os.path.join(models_dir, "style_models")], supported_pt_extensions)
 folder_names_and_paths["embeddings"] = ([os.path.join(models_dir, "embeddings")], supported_pt_extensions)
 folder_names_and_paths["diffusers"] = ([os.path.join(models_dir, "diffusers")], ["folder"])
 
 folder_names_and_paths["controlnet"] = ([os.path.join(models_dir, "controlnet"), os.path.join(models_dir, "t2i_adapter")], supported_pt_extensions)
+folder_names_and_paths["gligen"] = ([os.path.join(models_dir, "gligen")], supported_pt_extensions)
+
 folder_names_and_paths["upscale_models"] = ([os.path.join(models_dir, "upscale_models")], supported_pt_extensions)
 
 folder_names_and_paths["custom_nodes"] = ([os.path.join(base_path, "custom_nodes")], [])
 
 
 output_directory = os.path.join(os.path.dirname(os.path.realpath(__file__)), "output")
 temp_directory = os.path.join(os.path.dirname(os.path.realpath(__file__)), "temp")
```

### Comparing `hordelib-0.9.5/hordelib/_comfyui/input/example.png` & `hordelib-1.0.0/hordelib/_comfyui/input/example.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/main.py` & `hordelib-1.0.0/hordelib/_comfyui/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,15 +86,14 @@
         load_extra_path_config(extra_model_paths_config_path)
 
     if args.extra_model_paths_config:
         for config_path in itertools.chain(*args.extra_model_paths_config):
             load_extra_path_config(config_path)
 
     init_custom_nodes()
-    load_custom_nodes(os.getenv("AIWORKER_CUSTOM_NODES"))
     server.add_routes()
     hijack_progress(server)
 
     threading.Thread(target=prompt_worker, daemon=True, args=(q,server,)).start()
 
     address = args.listen
```

### Comparing `hordelib-0.9.5/hordelib/_comfyui/models/configs/anything_v3.yaml` & `hordelib-1.0.0/hordelib/_comfyui/models/configs/anything_v3.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/models/configs/v1-inference.yaml` & `hordelib-1.0.0/hordelib/_comfyui/models/configs/v1-inference.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2.yaml` & `hordelib-1.0.0/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2_fp16.yaml` & `hordelib-1.0.0/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2_fp16.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/models/configs/v1-inference_fp16.yaml` & `hordelib-1.0.0/hordelib/_comfyui/models/configs/v1-inference_fp16.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/models/configs/v1-inpainting-inference.yaml` & `hordelib-1.0.0/hordelib/_comfyui/models/configs/v1-inpainting-inference.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/models/configs/v2-inference-v.yaml` & `hordelib-1.0.0/hordelib/_comfyui/models/configs/v2-inference-v.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/models/configs/v2-inference-v_fp32.yaml` & `hordelib-1.0.0/hordelib/_comfyui/models/configs/v2-inference-v_fp32.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/models/configs/v2-inference.yaml` & `hordelib-1.0.0/hordelib/_comfyui/models/configs/v2-inference.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/models/configs/v2-inference_fp32.yaml` & `hordelib-1.0.0/hordelib/_comfyui/models/configs/v2-inference_fp32.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/models/configs/v2-inpainting-inference.yaml` & `hordelib-1.0.0/hordelib/_comfyui/models/configs/v2-inpainting-inference.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/nodes.py` & `hordelib-1.0.0/hordelib/_comfyui/nodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,19 @@
 import comfy.clip_vision
 
 import comfy.model_management
 import importlib
 
 import folder_paths
 
+import pickle
+import time
+from loguru import logger
+import threading
+
 def before_node_execution():
     comfy.model_management.throw_exception_if_processing_interrupted()
 
 def interrupt_processing(value=True):
     comfy.model_management.interrupt_current_processing(value)
 
 MAX_RESOLUTION=8192
@@ -486,14 +491,59 @@
                 o["adm"] = o["adm"][:] + [x]
             else:
                 o["adm"] = [x]
             n = [t[0], o]
             c.append(n)
         return (c, )
 
+class GLIGENLoader:
+    @classmethod
+    def INPUT_TYPES(s):
+        return {"required": { "gligen_name": (folder_paths.get_filename_list("gligen"), )}}
+
+    RETURN_TYPES = ("GLIGEN",)
+    FUNCTION = "load_gligen"
+
+    CATEGORY = "loaders"
+
+    def load_gligen(self, gligen_name):
+        gligen_path = folder_paths.get_full_path("gligen", gligen_name)
+        gligen = comfy.sd.load_gligen(gligen_path)
+        return (gligen,)
+
+class GLIGENTextBoxApply:
+    @classmethod
+    def INPUT_TYPES(s):
+        return {"required": {"conditioning_to": ("CONDITIONING", ),
+                              "clip": ("CLIP", ),
+                              "gligen_textbox_model": ("GLIGEN", ),
+                              "text": ("STRING", {"multiline": True}),
+                              "width": ("INT", {"default": 64, "min": 8, "max": MAX_RESOLUTION, "step": 8}),
+                              "height": ("INT", {"default": 64, "min": 8, "max": MAX_RESOLUTION, "step": 8}),
+                              "x": ("INT", {"default": 0, "min": 0, "max": MAX_RESOLUTION, "step": 8}),
+                              "y": ("INT", {"default": 0, "min": 0, "max": MAX_RESOLUTION, "step": 8}),
+                             }}
+    RETURN_TYPES = ("CONDITIONING",)
+    FUNCTION = "append"
+
+    CATEGORY = "conditioning/gligen"
+
+    def append(self, conditioning_to, clip, gligen_textbox_model, text, width, height, x, y):
+        c = []
+        cond, cond_pooled = clip.encode_from_tokens(clip.tokenize(text), return_pooled=True)
+        for t in conditioning_to:
+            n = [t[0], t[1].copy()]
+            position_params = [(cond_pooled, height // 8, width // 8, y // 8, x // 8)]
+            prev = []
+            if "gligen" in n[1]:
+                prev = n[1]['gligen'][2]
+
+            n[1]['gligen'] = ("position", gligen_textbox_model, prev + position_params)
+            c.append(n)
+        return (c, )
 
 class EmptyLatentImage:
     def __init__(self, device="cpu"):
         self.device = device
 
     @classmethod
     def INPUT_TYPES(s):
@@ -506,14 +556,32 @@
     CATEGORY = "latent"
 
     def generate(self, width, height, batch_size=1):
         latent = torch.zeros([batch_size, 4, height // 8, width // 8])
         return ({"samples":latent}, )
 
 
+class LatentFromBatch:
+    @classmethod
+    def INPUT_TYPES(s):
+        return {"required": { "samples": ("LATENT",),
+                              "batch_index": ("INT", {"default": 0, "min": 0, "max": 63}),
+                              }}
+    RETURN_TYPES = ("LATENT",)
+    FUNCTION = "rotate"
+
+    CATEGORY = "latent"
+
+    def rotate(self, samples, batch_index):
+        s = samples.copy()
+        s_in = samples["samples"]
+        batch_index = min(s_in.shape[0] - 1, batch_index)
+        s["samples"] = s_in[batch_index:batch_index + 1].clone()
+        s["batch_index"] = batch_index
+        return (s,)
 
 class LatentUpscale:
     upscale_methods = ["nearest-exact", "bilinear", "area"]
     crop_methods = ["disabled", "center"]
 
     @classmethod
     def INPUT_TYPES(s):
@@ -672,82 +740,107 @@
     CATEGORY = "latent/inpaint"
 
     def set_mask(self, samples, mask):
         s = samples.copy()
         s["noise_mask"] = mask
         return (s,)
 
-
 def common_ksampler(model, seed, steps, cfg, sampler_name, scheduler, positive, negative, latent, denoise=1.0, disable_noise=False, start_step=None, last_step=None, force_full_denoise=False):
     latent_image = latent["samples"]
     noise_mask = None
     device = comfy.model_management.get_torch_device()
 
     if disable_noise:
         noise = torch.zeros(latent_image.size(), dtype=latent_image.dtype, layout=latent_image.layout, device="cpu")
     else:
-        noise = torch.randn(latent_image.size(), dtype=latent_image.dtype, layout=latent_image.layout, generator=torch.manual_seed(seed), device="cpu")
+        batch_index = 0
+        if "batch_index" in latent:
+            batch_index = latent["batch_index"]
+
+        generator = torch.manual_seed(seed)
+        for i in range(batch_index):
+            noise = torch.randn([1] + list(latent_image.size())[1:], dtype=latent_image.dtype, layout=latent_image.layout, generator=generator, device="cpu")
+        noise = torch.randn(latent_image.size(), dtype=latent_image.dtype, layout=latent_image.layout, generator=generator, device="cpu")
 
     if "noise_mask" in latent:
         noise_mask = latent['noise_mask']
         noise_mask = torch.nn.functional.interpolate(noise_mask[None,None,], size=(noise.shape[2], noise.shape[3]), mode="bilinear")
         noise_mask = noise_mask.round()
         noise_mask = torch.cat([noise_mask] * noise.shape[1], dim=1)
         noise_mask = torch.cat([noise_mask] * noise.shape[0])
         noise_mask = noise_mask.to(device)
 
-    real_model = None
-    comfy.model_management.model_manager.model_in_use(model)
-    comfy.model_management.model_manager.load_model_gpu(model)
-    real_model = model.model
-
-    noise = noise.to(device)
-    latent_image = latent_image.to(device)
-
-    positive_copy = []
-    negative_copy = []
-
-    control_nets = []
-    for p in positive:
-        t = p[0]
-        if t.shape[0] < noise.shape[0]:
-            t = torch.cat([t] * noise.shape[0])
-        t = t.to(device)
-        if 'control' in p[1]:
-            control_nets += [p[1]['control']]
-        positive_copy += [[t] + p[1:]]
-    for n in negative:
-        t = n[0]
-        if t.shape[0] < noise.shape[0]:
-            t = torch.cat([t] * noise.shape[0])
-        t = t.to(device)
-        if 'control' in n[1]:
-            control_nets += [n[1]['control']]
-        negative_copy += [[t] + n[1:]]
-
-    control_net_models = []
-    for x in control_nets:
-        control_net_models += x.get_control_models()
-    comfy.model_management.model_manager.load_controlnet_gpu(control_net_models)
-
-    if sampler_name in comfy.samplers.KSampler.SAMPLERS:
-        sampler = comfy.samplers.KSampler(real_model, steps=steps, device=device, sampler=sampler_name, scheduler=scheduler, denoise=denoise, model_options=model.model_options)
-    else:
-        #other samplers
-        pass
+    comfy.model_management.model_manager.set_model_in_use(model)
+    try:
+        comfy.model_management.model_manager.load_model_gpu(model)
+        real_model = model.model
+
+        #logger.warning(f"Moving noise {id(noise):x} to device {device}")
+        noise = noise.to(device)
+        #logger.warning(f"Moving latest image {id(latent_image):x} to device {device}")
+        latent_image = latent_image.to(device)
+
+        positive_copy = []
+        negative_copy = []
+
+        #logger.warning(f"Assembling control nets")
+        control_nets = []
+        def get_models(cond):
+            models = []
+            for c in cond:
+                if 'control' in c[1]:
+                    models += [c[1]['control']]
+                if 'gligen' in c[1]:
+                    models += [c[1]['gligen'][1]]
+            return models
+
+        for p in positive:
+            t = p[0]
+            if t.shape[0] < noise.shape[0]:
+                t = torch.cat([t] * noise.shape[0])
+            t = t.to(device)
+            positive_copy += [[t] + p[1:]]
+        for n in negative:
+            t = n[0]
+            if t.shape[0] < noise.shape[0]:
+                t = torch.cat([t] * noise.shape[0])
+            t = t.to(device)
+            negative_copy += [[t] + n[1:]]
+
+        models = get_models(positive) + get_models(negative)
+        if models:
+            comfy.model_management.model_manager.load_controlnet_gpu(models)
+            comfy.model_management.model_manager.sampler_mutex.acquire()
+
+        if sampler_name in comfy.samplers.KSampler.SAMPLERS:
+            #logger.warning(f"Creating KSampler for real model {id(real_model):x}")
+            sampler = comfy.samplers.KSampler(real_model, steps=steps, device=device, sampler=sampler_name, scheduler=scheduler, denoise=denoise, model_options=model.model_options)
+        else:
+            #other samplers
+            pass
 
-    samples = sampler.sample(noise, positive_copy, negative_copy, cfg=cfg, latent_image=latent_image, start_step=start_step, last_step=last_step, force_full_denoise=force_full_denoise, denoise_mask=noise_mask)
-    samples = samples.cpu()
-    comfy.model_management.model_manager.unload_controlnet_gpu(control_net_models)
-    for c in control_nets:
-        c.cleanup()
-
-    out = latent.copy()
-    out["samples"] = samples
-    comfy.model_management.model_manager.done_with_model(model)
+        #logger.warning(f"Sampling")
+        samples = sampler.sample(noise, positive_copy, negative_copy, cfg=cfg, latent_image=latent_image, start_step=start_step, last_step=last_step, force_full_denoise=force_full_denoise, denoise_mask=noise_mask)
+        #logger.warning("Done sampling")
+        samples = samples.cpu()
+
+        #logger.warning("Moved samples to cpu")
+        if models:
+            # XXX force unload models for controlnet
+            #logger.warning("Forcing GPU unload of controlnet models")
+            comfy.model_management.model_manager.unload_controlnet_gpu(models)
+            comfy.model_management.model_manager.unload_model(model)
+            comfy.model_management.model_manager.sampler_mutex.release()
+            for m in models:
+                m.cleanup()
+
+        out = latent.copy()
+        out["samples"] = samples
+    finally:
+        comfy.model_management.model_manager.done_with_model(model)
     return (out, )
 
 class KSampler:
     @classmethod
     def INPUT_TYPES(s):
         return {"required":
                     {"model": ("MODEL",),
@@ -902,14 +995,15 @@
     CATEGORY = "image"
 
     RETURN_TYPES = ("IMAGE", "MASK")
     FUNCTION = "load_image"
     def load_image(self, image):
         input_dir = folder_paths.get_input_directory()
         image_path = os.path.join(input_dir, image)
+        #logger.warning(f"Loading image {image_path}")
         i = Image.open(image_path)
         image = i.convert("RGB")
         image = np.array(image).astype(np.float32) / 255.0
         image = torch.from_numpy(image)[None,]
         if 'A' in i.getbands():
             mask = np.array(i.getchannel('A')).astype(np.float32) / 255.0
             mask = 1. - torch.from_numpy(mask)
@@ -1072,14 +1166,15 @@
     "CLIPSetLastLayer": CLIPSetLastLayer,
     "VAEDecode": VAEDecode,
     "VAEEncode": VAEEncode,
     "VAEEncodeForInpaint": VAEEncodeForInpaint,
     "VAELoader": VAELoader,
     "EmptyLatentImage": EmptyLatentImage,
     "LatentUpscale": LatentUpscale,
+    "LatentFromBatch": LatentFromBatch,
     "SaveImage": SaveImage,
     "PreviewImage": PreviewImage,
     "LoadImage": LoadImage,
     "LoadImageMask": LoadImageMask,
     "ImageScale": ImageScale,
     "ImageInvert": ImageInvert,
     "ImagePadForOutpaint": ImagePadForOutpaint,
@@ -1101,14 +1196,17 @@
     "DiffControlNetLoader": DiffControlNetLoader,
     "StyleModelLoader": StyleModelLoader,
     "CLIPVisionLoader": CLIPVisionLoader,
     "VAEDecodeTiled": VAEDecodeTiled,
     "VAEEncodeTiled": VAEEncodeTiled,
     "TomePatchModel": TomePatchModel,
     "unCLIPCheckpointLoader": unCLIPCheckpointLoader,
+    "GLIGENLoader": GLIGENLoader,
+    "GLIGENTextBoxApply": GLIGENTextBoxApply,
+
     "CheckpointLoader": CheckpointLoader,
     "DiffusersLoader": DiffusersLoader,
 }
 
 NODE_DISPLAY_NAME_MAPPINGS = {
     # Sampling
     "KSampler": "KSampler",
```

### Comparing `hordelib-0.9.5/hordelib/_comfyui/notebooks/comfyui_colab.ipynb` & `hordelib-1.0.0/hordelib/_comfyui/notebooks/comfyui_colab.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999035493827161%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(70, '\\n'), (71, '\\n'), (72, '# GLIGEN\\n'), (73, '#!wget "*

 * *            '-c '*

 * *            'https://huggingface.co/comfyanonymous/GLIGEN_pruned_safetensors/resolve/main/gligen_sd14_textbox_pruned_fp16.safetensors '*

 * *            "-P ./models/gligen/\\n'), (74, '\\n')]}}}"}*

```diff
@@ -134,14 +134,19 @@
                 "#!wget -c https://huggingface.co/comfyanonymous/ControlNet-v1-1_fp16_safetensors/resolve/main/control_v11p_sd15s2_lineart_anime_fp16.safetensors -P ./models/controlnet/\n",
                 "#!wget -c https://huggingface.co/comfyanonymous/ControlNet-v1-1_fp16_safetensors/resolve/main/control_v11u_sd15_tile_fp16.safetensors -P ./models/controlnet/\n",
                 "\n",
                 "\n",
                 "# Controlnet Preprocessor nodes by Fannovel16\n",
                 "#!cd custom_nodes && git clone https://github.com/Fannovel16/comfy_controlnet_preprocessors; cd comfy_controlnet_preprocessors && python install.py\n",
                 "\n",
+                "\n",
+                "# GLIGEN\n",
+                "#!wget -c https://huggingface.co/comfyanonymous/GLIGEN_pruned_safetensors/resolve/main/gligen_sd14_textbox_pruned_fp16.safetensors -P ./models/gligen/\n",
+                "\n",
+                "\n",
                 "# ESRGAN upscale model\n",
                 "#!wget -c https://huggingface.co/sberbank-ai/Real-ESRGAN/resolve/main/RealESRGAN_x2.pth -P ./models/upscale_models/\n",
                 "#!wget -c https://huggingface.co/sberbank-ai/Real-ESRGAN/resolve/main/RealESRGAN_x4.pth -P ./models/upscale_models/\n",
                 "\n",
                 "\n"
             ]
         },
```

### Comparing `hordelib-0.9.5/hordelib/_comfyui/script_examples/basic_api_example.py` & `hordelib-1.0.0/hordelib/_comfyui/script_examples/basic_api_example.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/server.py` & `hordelib-1.0.0/hordelib/_comfyui/server.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/colorPalette.js` & `hordelib-1.0.0/hordelib/_comfyui/web/extensions/core/colorPalette.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/contextMenuFilter.js` & `hordelib-1.0.0/hordelib/_comfyui/web/extensions/core/contextMenuFilter.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/dynamicPrompts.js` & `hordelib-1.0.0/hordelib/_comfyui/web/extensions/core/dynamicPrompts.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js` & `hordelib-1.0.0/hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/keybinds.js` & `hordelib-1.0.0/hordelib/_comfyui/web/extensions/core/keybinds.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -3,28 +3,28 @@
 } from "/scripts/app.js";
 
 const id = "Comfy.Keybinds";
 app.registerExtension({
     name: id,
     init() {
         const keybindListener = function(event) {
-            const target = event.composedPath()[0];
-
-            if (target.tagName === "INPUT" || target.tagName === "TEXTAREA") {
-                return;
-            }
-
             const modifierPressed = event.ctrlKey || event.metaKey;
 
             // Queue prompt using ctrl or command + enter
             if (modifierPressed && (event.key === "Enter" || event.keyCode === 13 || event.keyCode === 10)) {
                 app.queuePrompt(event.shiftKey ? -1 : 0);
                 return;
             }
 
+            const target = event.composedPath()[0];
+
+            if (target.tagName === "INPUT" || target.tagName === "TEXTAREA") {
+                return;
+            }
+
             const modifierKeyIdMap = {
                 "s": "#comfy-save-button",
                 83: "#comfy-save-button",
                 "o": "#comfy-file-input",
                 79: "#comfy-file-input",
                 "Backspace": "#comfy-clear-button",
                 8: "#comfy-clear-button",
```

### Comparing `hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/nodeTemplates.js` & `hordelib-1.0.0/hordelib/_comfyui/web/extensions/core/nodeTemplates.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/noteNode.js` & `hordelib-1.0.0/hordelib/_comfyui/web/extensions/core/noteNode.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/rerouteNode.js` & `hordelib-1.0.0/hordelib/_comfyui/web/extensions/core/rerouteNode.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js` & `hordelib-1.0.0/hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/snapToGrid.js` & `hordelib-1.0.0/hordelib/_comfyui/web/extensions/core/snapToGrid.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -7,15 +7,15 @@
 app.registerExtension({
     name: "Comfy.SnapToGrid",
     init() {
         // Add setting to control grid size
         app.ui.settings.addSetting({
             id: "Comfy.SnapToGrid.GridSize",
             name: "Grid Size",
-            type: "number",
+            type: "slider",
             attrs: {
                 min: 1,
                 max: 500,
             },
             tooltip: "When dragging and resizing nodes while holding shift they will be aligned to the grid, this controls the size of that grid.",
             defaultValue: LiteGraph.CANVAS_GRID_SIZE,
             onChange(value) {
```

### Comparing `hordelib-0.9.5/hordelib/_comfyui/web/extensions/core/widgetInputs.js` & `hordelib-1.0.0/hordelib/_comfyui/web/extensions/core/widgetInputs.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/web/extensions/logging.js.example` & `hordelib-1.0.0/hordelib/_comfyui/web/extensions/logging.js.example`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/web/index.html` & `hordelib-1.0.0/hordelib/_comfyui/web/index.html`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/web/lib/litegraph.core.js` & `hordelib-1.0.0/hordelib/_comfyui/web/lib/litegraph.core.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/web/lib/litegraph.css` & `hordelib-1.0.0/hordelib/_comfyui/web/lib/litegraph.css`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/web/scripts/api.js` & `hordelib-1.0.0/hordelib/_comfyui/web/scripts/api.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/web/scripts/app.js` & `hordelib-1.0.0/hordelib/_comfyui/web/scripts/app.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/web/scripts/defaultGraph.js` & `hordelib-1.0.0/hordelib/_comfyui/web/scripts/defaultGraph.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/web/scripts/pnginfo.js` & `hordelib-1.0.0/hordelib/_comfyui/web/scripts/pnginfo.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/web/scripts/ui.js` & `hordelib-1.0.0/hordelib/_comfyui/web/scripts/ui.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -290,14 +290,40 @@
                                             setter(e.target.value);
                                         },
                                         ...attrs
                                     }),
                                 ]),
                             ]);
                             break;
+                        case "slider":
+                            element = $el("div", [
+                                $el("label", {
+                                    textContent: name
+                                }, [
+                                    $el("input", {
+                                        type: "range",
+                                        value,
+                                        oninput: (e) => {
+                                            setter(e.target.value);
+                                            e.target.nextElementSibling.value = e.target.value;
+                                        },
+                                        ...attrs
+                                    }),
+                                    $el("input", {
+                                        type: "number",
+                                        value,
+                                        oninput: (e) => {
+                                            setter(e.target.value);
+                                            e.target.previousElementSibling.value = e.target.value;
+                                        },
+                                        ...attrs
+                                    }),
+                                ]),
+                            ]);
+                            break;
                         default:
                             console.warn("Unsupported setting type, defaulting to text");
                             element = $el("div", [
                                 $el("label", {
                                     textContent: name || id
                                 }, [
                                     $el("input", {
```

### Comparing `hordelib-0.9.5/hordelib/_comfyui/web/scripts/widgets.js` & `hordelib-1.0.0/hordelib/_comfyui/web/scripts/widgets.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/web/style.css` & `hordelib-1.0.0/hordelib/_comfyui/web/style.css`

 * *Files 6% similar despite different names*

```diff
@@ -213,14 +213,22 @@
 .comfy-modal.comfy-manage-templates {
 	text-align: center;
 	font-family: sans-serif;
 	color: var(--descrip-text);
 	z-index: 99;
 }
 
+.comfy-modal.comfy-settings input[type="range"] {
+	vertical-align: middle;
+}
+
+.comfy-modal.comfy-settings input[type="range"] + input[type="number"] {
+	width: 3.5em;
+}
+
 .comfy-modal input,
 .comfy-modal select {
 	color: var(--input-text);
 	background-color: var(--comfy-input-bg);
 	border-radius: 8px;
 	border-color: var(--border-color);
 	border-style: solid;
```

### Comparing `hordelib-0.9.5/hordelib/_comfyui/web/types/comfy.d.ts` & `hordelib-1.0.0/hordelib/_comfyui/web/types/comfy.d.ts`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/_comfyui/web/types/litegraph.d.ts` & `hordelib-1.0.0/hordelib/_comfyui/web/types/litegraph.d.ts`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/blip/caption.py` & `hordelib-1.0.0/hordelib/blip/caption.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/cache/cache.py` & `hordelib-1.0.0/hordelib/cache/cache.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/clip/bulk.py` & `hordelib-1.0.0/hordelib/clip/bulk.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/clip/coca.py` & `hordelib-1.0.0/hordelib/clip/coca.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/clip/image.py` & `hordelib-1.0.0/hordelib/clip/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,18 +102,19 @@
             image_hash = hashlib.sha256(pil_image.tobytes()).hexdigest()
         else:
             file_hash = None
             image_hash = hashlib.sha256(pil_image.tobytes()).hexdigest()
         if not skip_cache:
             cached = self.cache.get(pil_hash=image_hash)
             if cached:
-                logger.debug(f"Image {image_hash} already in cache")
+                # logger.debug(f"Image {image_hash} already in cache")
                 return image_hash
         else:
-            logger.debug(f"Skipping cache for image {image_hash}")
-        logger.debug(f"Embedding image {image_hash}")
+            pass
+            # logger.debug(f"Skipping cache for image {image_hash}")
+        # logger.debug(f"Embedding image {image_hash}")
         with torch.no_grad():
             preprocess_image = self.model["preprocess"](pil_image).unsqueeze(0).to(self.model["device"])
         image_features = self.model["model"].encode_image(preprocess_image).float()
         self._save(image_features, image_hash)
         self.cache.add_sqlite_row(file=filename, hash=file_hash, pil_hash=image_hash)
         return image_hash
```

### Comparing `hordelib-0.9.5/hordelib/clip/interrogate.py` & `hordelib-1.0.0/hordelib/clip/interrogate.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,31 +42,32 @@
         """
         :param key: Key to use for embed_lists
         :param text_array: List of text to embed
         :param individual: Whether to store each text embed individually or as a concatenated tensor
         If individual is True, self.embed_lists[key] will be a dict with text as key and embed as value.
         If individual is False, self.embed_lists[key] will be a tensor of all text embeds concatenated.
         """
-        logger.debug(f"key: {key}, text_array: {text_array}, individual: {individual}")
+        # logger.debug(f"key: {key}, text_array: {text_array}, individual: {individual}")
         cached = True
         for text in text_array:
             text_hash = hashlib.sha256(text.encode("utf-8")).hexdigest()
             if self.cache.get(file_hash=text_hash) is None:
                 cached = False
-                logger.debug(f"{text} not cached")
+                # logger.debug(f"{text} not cached")
                 break
         if not cached:
-            logger.debug(f"Embedding {key}...")
+            # logger.debug(f"Embedding {key}...")
             text_embed = TextEmbed(self.model_info, self.cache)
             for text in text_array:
-                logger.debug(f"Embedding {text}")
+                # logger.debug(f"Embedding {text}")
                 text_embed(text)
         else:
-            logger.debug(f"{key} embeds already cached")
-        logger.debug(f"Loading {key} embeds")
+            pass
+            # logger.debug(f"{key} embeds already cached")
+        # logger.debug(f"Loading {key} embeds")
         if individual:
             self.embed_lists[key] = {}
             for text in text_array:
                 text_hash = hashlib.sha256(text.encode("utf-8")).hexdigest()
                 filename = f"{self.cache.cache_dir}/{text_hash}.npy"
                 logger.debug(
                     f"text: {text}, text_hash: {text_hash}, filename: {filename}",
@@ -142,17 +143,17 @@
         :param image_features: Image features to compare to text features
         :param text_array: List of text to compare to image
         :param key: Key to use for embed_lists
         :param device: Device to run on
         :return: dict of {text: similarity}
         """
         if key not in self.embed_lists:
-            logger.debug(f"Loading {key} embeds")
+            # logger.debug(f"Loading {key} embeds")
             self.load(key, text_array, individual=True, device=device)
-        logger.debug(f"{len(text_array)} text_array: {text_array}")
+        # logger.debug(f"{len(text_array)} text_array: {text_array}")
         similarity = {}
         for text in text_array:
             text_features = self.embed_lists[key][text].to(device)
             similarity[text] = round(
                 self._similarity(image_features, text_features)[0][0].item(),
                 4,
             )
@@ -246,45 +247,45 @@
             for k in text_array:
                 results[k] = self.similarity(
                     image_features,
                     text_array[k],
                     k,
                     self.model_info["device"],
                 )
-                logger.debug(f"{k}: {results[k]}")
+                # logger.debug(f"{k}: {results[k]}")
             return results
         if rank and not similarity:
             results = {}
             for k in text_array:
                 results[k] = self.rank(
                     image_features,
                     text_array[k],
                     k,
                     self.model_info["device"],
                     top_count,
                 )
-                logger.debug(f"{k}: {results[k]}")
+                # logger.debug(f"{k}: {results[k]}")
             return results
         else:
             similarity = {}
             for k in text_array:
                 similarity[k] = self.similarity(
                     image_features,
                     text_array[k],
                     k,
                     self.model_info["device"],
                 )
-                logger.debug(f"{k}: {similarity[k]}")
+                # logger.debug(f"{k}: {similarity[k]}")
             rank = {}
             for k in text_array:
                 rank[k] = self.rank(
                     image_features,
                     text_array[k],
                     k,
                     self.model_info["device"],
                     top_count,
                 )
-                logger.debug(f"{k}: {rank[k]}")
+                # logger.debug(f"{k}: {rank[k]}")
             return {
                 "similarity": similarity,
                 "rank": rank,
             }
```

### Comparing `hordelib-0.9.5/hordelib/clip/ranking_lists/artists.txt` & `hordelib-1.0.0/hordelib/clip/ranking_lists/artists.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/clip/ranking_lists/flavors.txt` & `hordelib-1.0.0/hordelib/clip/ranking_lists/flavors.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/clip/ranking_lists/mediums.txt` & `hordelib-1.0.0/hordelib/clip/ranking_lists/mediums.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/clip/ranking_lists/movements.txt` & `hordelib-1.0.0/hordelib/clip/ranking_lists/movements.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/clip/ranking_lists/tags.txt` & `hordelib-1.0.0/hordelib/clip/ranking_lists/tags.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/clip/ranking_lists/techniques.txt` & `hordelib-1.0.0/hordelib/clip/ranking_lists/techniques.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/clip/text.py` & `hordelib-1.0.0/hordelib/clip/text.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/comfy_horde.py` & `hordelib-1.0.0/hordelib/comfy_horde.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,77 +28,103 @@
 from execution import nodes as _comfy_nodes
 from execution import PromptExecutor as _comfy_PromptExecutor
 from folder_paths import folder_names_and_paths as _comfy_folder_paths
 from comfy.sd import load_checkpoint_guess_config as __comfy_load_checkpoint_guess_config
 from comfy.sd import load_controlnet as __comfy_load_controlnet
 from comfy.model_management import model_manager as _comfy_model_manager
 from comfy.model_management import get_torch_device as __comfy_get_torch_device
+from comfy.model_management import get_free_memory as __comfy_get_free_memory
 from comfy.utils import load_torch_file as __comfy_load_torch_file
 from comfy_extras.chainner_models import model_loading as _comfy_model_loading
 
 # isort: on
 
 __models_to_release = {}
-_controlnet_mutex = threading.Lock()
-_facefix_mutex = threading.Lock()
+__model_load_mutex = threading.Lock()
 
 
 def cleanup():
-    with _comfy_model_manager.sampler_mutex:
+    locked = _comfy_model_manager.sampler_mutex.acquire(timeout=0)
+    if locked:
         # Do we have any models waiting to be released?
         if not __models_to_release:
+            _comfy_model_manager.sampler_mutex.release()
             return
 
         # Can we release any of them?
         for model_name, model_data in __models_to_release.copy().items():
             if is_model_in_use(model_data["model"]):
                 # We're in the middle of using it, nothing we can do
                 continue
             # Unload the model from the GPU
+            logger.debug(f"Unloading {model_name} from GPU")
             unload_model_from_gpu(model_data["model"])
             # Free ram
             if "model" in model_data:
                 del model_data["model"]
             if "clip" in model_data:
                 del model_data["clip"]
             if "vae" in model_data:
                 del model_data["vae"]
             if "clipVisionModel" in model_data:
                 del model_data["clipVisionModel"]
             del model_data
-            del __models_to_release[model_name]
+            with __model_load_mutex:
+                del __models_to_release[model_name]
             gc.collect()
+            logger.debug(f"Removal of model {model_name} completed")
+
+        _comfy_model_manager.sampler_mutex.release()
 
 
 def remove_model_from_memory(model_name, model_data):
-    with _comfy_model_manager.sampler_mutex:
+    logger.debug(f"Comfy_Horde received request to unload {model_name}")
+    with __model_load_mutex:
         if model_name not in __models_to_release:
+            logger.debug(f"Model {model_name} queued for GPU/RAM unload")
             __models_to_release[model_name] = model_data
 
 
 def get_models_on_gpu():
     return _comfy_model_manager.get_models_on_gpu()
 
 
 def get_torch_device():
     return __comfy_get_torch_device()
 
 
+def get_torch_free_vram_mb():
+    return round(__comfy_get_free_memory() / (1024 * 1024))
+
+
 def unload_model_from_gpu(model):
-    _comfy_model_manager.unload_model(model)
+    _comfy_model_manager.load_model_gpu(model)
+    garbage_collect()
+
+
+def garbage_collect():
     gc.collect()
     if not torch.cuda.is_available():
         return None
     if torch.version.cuda:
         torch.cuda.empty_cache()
         torch.cuda.ipc_collect()
 
 
+def load_model_to_gpu(model):
+    # Don't bother if there isn't any space
+    if not _comfy_model_manager.have_free_vram():
+        return
+    # Load the model to the GPU. This would normally be done just before
+    # the model is used for sampling, the caller must want more free ram.
+    return _comfy_model_manager.load_model_gpu(model)
+
+
 def is_model_in_use(model):
-    return _comfy_model_manager.model_in_use(model)
+    return _comfy_model_manager.is_model_in_use(model)
 
 
 def load_torch_file(filename):
     result = __comfy_load_torch_file(filename)
     return result
 
 
@@ -181,18 +207,39 @@
         "sampler.steps": (1, 500),
         "empty_latent_image.batch_size": (1, 500),
         "clip_skip.stop_at_clip_layer": (-10, -1),
         "latent_upscale.width": (64, 8192),
         "latent_upscale.height": (64, 8192),
     }
 
+    # Approximate number of seconds to force garbage collection
+    GC_TIME = 30
+
+    _property_mutex = threading.Lock()
+
+    # We maintain one "client_id" per thread
+    @property
+    def client_id(self):
+        with Comfy_Horde._property_mutex:
+            tid = threading.current_thread().ident
+            return self._client_id.get(tid)
+
+    @client_id.setter
+    def client_id(self, client_id):
+        with Comfy_Horde._property_mutex:
+            tid = threading.current_thread().ident
+            self._client_id[tid] = client_id
+
     def __init__(self) -> None:
-        self.client_id = None  # used for receiving comfyUI async events
+        self._client_id = {}
         self.pipelines = {}
-        self.exit_time = 0
+        self._exit_time = 0
+        self._callers = 0
+        self._gc_timer = time.time()
+        self._counter_mutex = threading.Lock()
         # Set custom node path
         _comfy_folder_paths["custom_nodes"] = ([os.path.join(get_hordelib_path(), "nodes")], [])
         # Load our pipelines
         self._load_pipelines()
 
         stdio = OutputCollector()
         with contextlib.redirect_stdout(stdio):
@@ -391,15 +438,15 @@
     def run_pipeline(self, pipeline_name: str, params: dict) -> dict | None:
         # Sanity
         if pipeline_name not in self.pipelines:
             logger.error(f"Unknown inference pipeline: {pipeline_name}")
             return None
 
         # Update user settings
-        _comfy_model_manager.set_user_reserved_vram(UserSettings.vram_to_leave_free_mb)
+        _comfy_model_manager.set_user_reserved_vram(UserSettings.get_vram_to_leave_free_mb())
 
         logger.info(f"Running pipeline {pipeline_name}")
 
         # Grab a copy of the pipeline
         pipeline = copy.deepcopy(self.pipelines[pipeline_name])
 
         # Inject our model manager if required
@@ -407,24 +454,21 @@
 
         if "model_loader.model_manager" not in params:
             logger.debug("Injecting model manager")
             params["model_loader.model_manager"] = SharedModelManager
 
         # If we have a source image, use that rather than noise (i.e. img2img)
         # XXX This probably shouldn't be here. But for the moment, it works.
-        if "image_loader.image" in params:
+        if params.get("image_loader.image"):
             self.reconnect_input(pipeline, "sampler.latent_image", "vae_encode")
 
         # XXX This shouldn't be here either, but it's not clear to me yet where the
         # XXX correct place for dynamic connection of nodes is. Need to do a few more
         # XXX pipelines to see.
-        mutex = None
-        if "control_type" in params:
-            # FIXME Only allow one controlnet job at a time
-            mutex = _controlnet_mutex
+        if params.get("control_type"):
             # Inject control net model manager
             if "controlnet_model_loader.model_manager" not in params:
                 logger.debug("Injecting controlnet model manager")
                 params["controlnet_model_loader.model_manager"] = SharedModelManager
             # Connect to the correct pre-processor node
             if params.get("return_control_map", False):
                 # Connect annotator to output image directly
@@ -453,51 +497,56 @@
         # This is useful for dumping the entire pipeline to the terminal when
         # developing and debugging new pipelines. A badly structured pipeline
         # file just results in a cryptic error from comfy
         pretty_pipeline = pformat(pipeline)
         if False:  # This isn't here Tazlin :)
             logger.error(pretty_pipeline)
 
-        # Last minute mutex setup
-        if pipeline_name == "image_facefix":
-            mutex = _facefix_mutex
-
         # The client_id parameter here is just so we receive comfy callbacks for debugging.
         # We pretend we are a web client and want async callbacks.
         stdio = OutputCollector()
         with contextlib.redirect_stdout(stdio), contextlib.redirect_stderr(stdio):
-            if mutex:
-                with mutex:
-                    inference.execute(pipeline, extra_data={"client_id": random.randint(0, sys.maxsize)})
-            else:
-                inference.execute(pipeline, extra_data={"client_id": random.randint(0, sys.maxsize)})
+            inference.execute(pipeline, extra_data={"client_id": random.randint(0, sys.maxsize)})
 
         stdio.replay()
 
         # Check if there are any resource to clean up
         cleanup()
+        if time.time() - self._gc_timer > Comfy_Horde.GC_TIME:
+            self._gc_timer = time.time()
+            garbage_collect()
 
         return inference.outputs
 
     # Run a pipeline that returns an image in pixel space
     def run_image_pipeline(self, pipeline_name: str, params: dict) -> list[dict] | None:
         # From the horde point of view, let us assume the output we are interested in
         # is always in a HordeImageOutput node named "output_image". This is an array of
         # dicts of the form:
         # [ {
         #     "imagedata": <BytesIO>,
         #     "type": "PNG"
         #   },
         # ]
         # See node_image_output.py
-        if self.exit_time:
-            idle_time = time.time() - self.exit_time
+
+        # If no callers for a while, announce it
+        if self._callers == 0 and self._exit_time:
+            idle_time = time.time() - self._exit_time
             if idle_time > 1:
                 logger.warning(f"No job ran for {round(idle_time, 3)} seconds")
 
+        # We have just been entered
+        with self._counter_mutex:
+            self._callers += 1
+
         result = self.run_pipeline(pipeline_name, params)
-        self.exit_time = time.time()
+
+        # We are being exited
+        with self._counter_mutex:
+            self._exit_time = time.time()
+            self._callers -= 1
 
         if result:
             return result["output_image"]["images"]
 
         return None
```

### Comparing `hordelib-0.9.5/hordelib/config_path.py` & `hordelib-1.0.0/hordelib/config_path.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/consts.py` & `hordelib-1.0.0/hordelib/consts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 # consts.py
 import os
 from enum import Enum, auto
 
 from hordelib.config_path import get_hordelib_path
 
-COMFYUI_VERSION = "74fc7b772656a59b344508480632d9d45f9127de"
+COMFYUI_VERSION = "6908f9c94992b32fbb96be0f6cd8c5b362d72a77"
 """The exact version of ComfyUI version to load."""
 
 REMOTE_MODEL_DB = "https://raw.githubusercontent.com/db0/AI-Horde-image-model-reference/main/"
 """The default base endpoint where to find model databases. See MODEL_DB_NAMES for valid database names."""
 
 RELEASE_VERSION = os.path.exists(os.path.join(get_hordelib_path(), "_version.py"))
 """A flag for if this is a pypi release or a git dev mode"""
 
 
 class HordeSupportedBackends(Enum):
     ComfyUI = auto()
 
 
+# Models Excluded from hordelib (for now) # FIXME
+# this could easily be a json file on the AI-Horde-image-model-reference repo
+EXCLUDED_MODEL_NAMES = ["pix2pix", "anything_v4_inpainting", "dreamlike_diffusion_inpainting"]
+
+
 class MODEL_CATEGORY_NAMES(str, Enum):
     """Look up str enum for the categories of models (compvis, controlnet, clip, etc...)."""
 
     blip = "blip"
     clip = "clip"
     codeformer = "codeformer"
     compvis = "compvis"
```

### Comparing `hordelib-0.9.5/hordelib/initialisation.py` & `hordelib-1.0.0/hordelib/initialisation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,47 @@
 # initialisation.py
 # Initialise hordelib.
+import os
+import shutil
 import sys
 
 from loguru import logger
 
 from hordelib import install_comfy
 from hordelib.config_path import get_hordelib_path, set_system_path
 from hordelib.consts import (
     COMFYUI_VERSION,
     DEFAULT_MODEL_MANAGERS,
     MODEL_CATEGORY_NAMES,
     RELEASE_VERSION,
 )
 from hordelib.utils.logger import HordeLog
 
+_is_initialised = False
+
 
 def initialise(
-    model_managers_to_load: dict[MODEL_CATEGORY_NAMES, bool] = DEFAULT_MODEL_MANAGERS,
+    # model_managers_to_load: dict[MODEL_CATEGORY_NAMES, bool] = DEFAULT_MODEL_MANAGERS,
+    *,
     setup_logging=True,
-):
+    clear_logs=False,
+    debug_logging=False,
+):  # XXX # TODO Do we need `model_managers_to_load`?
+
+    global _is_initialised
+
+    # Wipe existing logs if requested
+    if clear_logs and os.path.exists("./logs"):
+        shutil.rmtree("./logs")
+
     # Setup logging if requested
-    HordeLog.initialise(setup_logging)
+    HordeLog.initialise(setup_logging=setup_logging)
+    if debug_logging:
+        HordeLog.set_logger_verbosity(5)
+        HordeLog.quiesce_logger(0)
 
     # If developer mode, don't permit some things
     if not RELEASE_VERSION and " " in get_hordelib_path():
         # Our runtime patching can't handle this
         raise Exception(
             "Do not run this project in developer mode from a path that " "contains spaces in directory names.",
         )
@@ -41,7 +58,13 @@
 
     # Initialise model manager
     from hordelib.shared_model_manager import SharedModelManager
 
     SharedModelManager()
 
     sys.argv = sys_arg_bkp
+
+    _is_initialised = True
+
+
+def is_initialised():
+    return _is_initialised
```

### Comparing `hordelib-0.9.5/hordelib/install_comfy.py` & `hordelib-1.0.0/hordelib/install_comfy.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 import subprocess
 
 from loguru import logger
 
 from hordelib.config_path import get_comfyui_path, get_hordelib_path
 from hordelib.consts import RELEASE_VERSION
 
+CUSTOM_NODE_YAML = """
+hordelib:
+    base_path: ../
+    custom_nodes: hordelib/nodes
+"""
+
 
 class Installer:
     """Handles the installation of ComfyUI."""
 
     @classmethod
     def get_commit_hash(cls) -> str:
         if RELEASE_VERSION:
@@ -144,7 +150,12 @@
             cls.remove_local_comfyui_changes()
             # Try to apply the patch
             logger.info(f"Applying patch {patchfile}")
             result = cls._run_get_result(f"git apply {patchfile}", get_comfyui_path())
             logger.debug(f"{result}")
             if result.returncode:
                 logger.error(f"Could not apply patch {patchfile}")
+
+        # Drop in custom node config
+        config_file = os.path.join(get_comfyui_path(), "extra_model_paths.yaml")
+        with open(config_file, "wt") as outfile:
+            outfile.write(CUSTOM_NODE_YAML)
```

### Comparing `hordelib-0.9.5/hordelib/model_database/aitemplate.json` & `hordelib-1.0.0/hordelib/model_database/aitemplate.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/model_database/blip.json` & `hordelib-1.0.0/hordelib/model_database/blip.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/model_database/clip.json` & `hordelib-1.0.0/hordelib/model_database/clip.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/model_database/controlnet.json` & `hordelib-1.0.0/hordelib/model_database/controlnet.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/model_database/db.json` & `hordelib-1.0.0/hordelib/model_database/db.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/model_database/db_dep.json` & `hordelib-1.0.0/hordelib/model_database/db_dep.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/model_database/db_embeds.json` & `hordelib-1.0.0/hordelib/model_database/db_embeds.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/model_database/diffusers.json` & `hordelib-1.0.0/hordelib/model_database/diffusers.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/model_database/esrgan.json` & `hordelib-1.0.0/hordelib/model_database/esrgan.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'4x_NMKD_Superscale_SP'": "OrderedDict([('name', '4x_NMKD_Superscale_SP'), ('type', 'esrgan'), "*

 * *                            "('description', 'Realistic, multipurpose upscaler'), ('version', "*

 * *                            "'1.0.0'), ('style', 'generalist'), ('config', OrderedDict([('files', "*

 * *                            "[OrderedDict([('path', '4x_NMKD-Superscale-SP_178000_G.pth'), "*

 * *                            "('sha256sum', "*

 * *                            "'1d1b0078fe71446e0469d8d4df59e96baa80d83cda600d682 […]*

```diff
@@ -18,14 +18,37 @@
         },
         "description": "Specialised anime upscaler",
         "name": "4x_AnimeSharp",
         "style": "anime",
         "type": "esrgan",
         "version": "0.1.0"
     },
+    "4x_NMKD_Superscale_SP": {
+        "available": false,
+        "config": {
+            "download": [
+                {
+                    "file_name": "4x_NMKD-Superscale-SP_178000_G.pth",
+                    "file_path": "",
+                    "file_url": "https://nmkd.de/shared/ESRGAN/Models/Realistic%2C%20Multipurpose/4x_NMKD-Superscale-SP_178000_G.pth"
+                }
+            ],
+            "files": [
+                {
+                    "path": "4x_NMKD-Superscale-SP_178000_G.pth",
+                    "sha256sum": "1d1b0078fe71446e0469d8d4df59e96baa80d83cda600d68237d655830821bcc"
+                }
+            ]
+        },
+        "description": "Realistic, multipurpose upscaler",
+        "name": "4x_NMKD_Superscale_SP",
+        "style": "generalist",
+        "type": "esrgan",
+        "version": "1.0.0"
+    },
     "NMKD_Siax": {
         "available": false,
         "config": {
             "download": [
                 {
                     "file_name": "NMKD_Siax.pth",
                     "file_path": "",
```

### Comparing `hordelib-0.9.5/hordelib/model_database/gfpgan.json` & `hordelib-1.0.0/hordelib/model_database/gfpgan.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/model_database/safety_checker.json` & `hordelib-1.0.0/hordelib/model_database/safety_checker.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/model_database/stable_diffusion.json` & `hordelib-1.0.0/hordelib/model_database/stable_diffusion.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9467714211957633%*

 * *Differences: {'"Elldreth\'s Lucid Mix"': "{'config': {'download': {0: {'file_url': "*

 * *                            "'https://civitai.com/api/download/models/1450?type=Model&format=PickleTensor&size=full&fp=fp16'}}}}",*

 * * '"Healy\'s Anime Blend"': "{'config': {'download': {0: {'file_url': "*

 * *                           "'https://huggingface.co/BlancOfficial/Healy_AnimeBlend/resolve/main/healySAnimeBlend_17.ckpt'}}}}",*

 * * "'526Mix-Animated'": "OrderedDict([('name', '526Mix-Animated'), ('baseline', 'stable diffusion "*

 * *             […]*

```diff
@@ -30,14 +30,48 @@
             "https://raw.githubusercontent.com/db0/AI-Horde-image-model-reference/main/showcase/3dkx/01_airic.webp",
             "https://raw.githubusercontent.com/db0/AI-Horde-image-model-reference/main/showcase/3dkx/02_gigachad.webp"
         ],
         "style": "artistic",
         "type": "ckpt",
         "version": "1.1"
     },
+    "526Mix-Animated": {
+        "available": false,
+        "baseline": "stable diffusion 1",
+        "config": {
+            "download": [
+                {
+                    "file_name": "526mixAnimated.safetensors",
+                    "file_path": "",
+                    "file_url": "https://civitai.com/api/download/models/42086?type=Model&format=SafeTensor&size=pruned&fp=fp16"
+                }
+            ],
+            "files": [
+                {
+                    "path": "526mixAnimated.safetensors",
+                    "sha256sum": "5c0b94405672bff73bb16fc9f2b4335695021494de16ddb1709ea7ee0f2e1b74"
+                },
+                {
+                    "path": "v1-inference.yaml"
+                }
+            ]
+        },
+        "description": "The goal of this model was to anchor 526Mix's whimsical and artistic personality into anime. 526Mix can do a pretty cool anime style (and other 2D styles), but it can be a bit unreliable at times. This simple mix increases the reliability, depth, and nuance in 526Mix's anime and anime-esque capabilities.",
+        "download_all": false,
+        "homepage": "https://civitai.com/models/35893/526mix-animated",
+        "name": "526Mix-Animated",
+        "nsfw": true,
+        "style": "anime",
+        "tags": [
+            "anime",
+            "character"
+        ],
+        "type": "ckpt",
+        "version": "1.0"
+    },
     "A to Zovya RPG": {
         "available": false,
         "baseline": "stable diffusion 2",
         "config": {
             "download": [
                 {
                     "file_name": "A-to-z_zovya_rpg.ckpt",
@@ -553,14 +587,49 @@
         "style": "artistic",
         "trigger": [
             "asim style"
         ],
         "type": "ckpt",
         "version": "1.0"
     },
+    "Aurora": {
+        "available": false,
+        "baseline": "stable diffusion 1",
+        "config": {
+            "download": [
+                {
+                    "file_name": "aurora.safetensors",
+                    "file_path": "",
+                    "file_url": "https://civitai.com/api/download/models/45601?type=Model&format=SafeTensor&size=full&fp=fp16"
+                }
+            ],
+            "files": [
+                {
+                    "path": "aurora.safetensors",
+                    "sha256sum": "1b5f8211ec04926035ac81033518c802db9964e93630ab4698b6365b9811c7eb"
+                },
+                {
+                    "path": "v1-inference.yaml"
+                }
+            ]
+        },
+        "description": "Aurora is a Stable Diffusion model, similar to its predecessor Kenshi, with the goal of capturing my own feelings towards the anime styles I desire.The name Aurora, which means 'dawn' in Latin, represents the idea of a new beginning and a fresh start.",
+        "download_all": false,
+        "homepage": "https://civitai.com/models/40199/aurora",
+        "name": "Aurora",
+        "nsfw": false,
+        "style": "anime",
+        "trigger": [
+            "sle",
+            "mksks style",
+            "detailed background"
+        ],
+        "type": "ckpt",
+        "version": "1.0"
+    },
     "BPModel": {
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
                     "file_name": "BPModel.ckpt",
@@ -625,14 +694,44 @@
         "style": "other",
         "trigger": [
             "BalloonArt"
         ],
         "type": "ckpt",
         "version": "1.0"
     },
+    "Beautiful Realistic Asians": {
+        "available": false,
+        "baseline": "stable diffusion 1",
+        "config": {
+            "download": [
+                {
+                    "file_name": "braBeautifulRealistic.safetensors",
+                    "file_path": "",
+                    "file_url": "https://civitai.com/api/download/models/51395?type=Model&format=SafeTensor&size=full&fp=fp32"
+                }
+            ],
+            "files": [
+                {
+                    "path": "braBeautifulRealistic.safetensors",
+                    "sha256sum": "9c03252bea886e921a10f6b5f61b2d60565c32d02bbbb40cb59944c0218c5e90"
+                },
+                {
+                    "path": "v1-inference.yaml"
+                }
+            ]
+        },
+        "description": "Trained on countless pictures of Beautiful Asian women. (some nsfw images included)",
+        "download_all": false,
+        "homepage": "https://civitai.com/models/25494/brabeautiful-realistic-asians-v3",
+        "name": "Beautiful Realistic Asians",
+        "nsfw": true,
+        "style": "realistic",
+        "type": "ckpt",
+        "version": "4.0"
+    },
     "Borderlands": {
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
                     "file_name": "borderlands.ckpt",
@@ -701,23 +800,53 @@
         "style": "artistic",
         "trigger": [
             "art by bubblydubbly"
         ],
         "type": "ckpt",
         "version": "1"
     },
+    "CamelliaMix 2.5D": {
+        "available": false,
+        "baseline": "stable diffusion 1",
+        "config": {
+            "download": [
+                {
+                    "file_name": "camelliamix25D.safetensors",
+                    "file_path": "",
+                    "file_url": "https://civitai.com/api/download/models/48859?type=Model&format=SafeTensor&size=pruned&fp=fp16"
+                }
+            ],
+            "files": [
+                {
+                    "path": "camelliamix25D.safetensors",
+                    "sha256sum": "ed4f26c284bc9baaeee63f10ad823486bcc0dd6fcc03c9472fd8c44e508889a1"
+                },
+                {
+                    "path": "v1-inference.yaml"
+                }
+            ]
+        },
+        "description": "Semi-realistic model, Camellia Mix 2.5D V2",
+        "download_all": false,
+        "homepage": "https://civitai.com/models/44219",
+        "name": "CamelliaMix 2.5D",
+        "nsfw": false,
+        "style": "anime",
+        "type": "ckpt",
+        "version": "2.0"
+    },
     "Char": {
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
                     "file_name": "Char.ckpt",
                     "file_path": "",
-                    "file_url": "https://civitai.com/api/download/models/24806?type=Pruned%20Model&format=PickleTensor"
+                    "file_url": "https://civitai.com/api/download/models/24806?type=Pruned%20Model&format=PickleTensor&size=pruned&fp=fp16"
                 }
             ],
             "files": [
                 {
                     "md5sum": "bc457a17eca7b57c0d7fa11489a5dab8",
                     "path": "Char.ckpt",
                     "sha256sum": "20fd9992efbb5dab68d054932d228865a1bc11965a285e84f82cef667ad6e3c7"
@@ -782,15 +911,15 @@
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
                     "file_name": "CDLandscapeMix.ckpt",
                     "file_path": "",
-                    "file_url": "https://civitai.com/api/download/models/7304?type=Model&format=PickleTensor"
+                    "file_url": "https://civitai.com/api/download/models/7304?type=Model&format=PickleTensor&size=full&fp=fp16"
                 }
             ],
             "files": [
                 {
                     "md5sum": "73eae68e9dfae23c10d4aab2df183390",
                     "path": "CDLandscapeMix.ckpt",
                     "sha256sum": "469820821518540111673d6ba590cf2010ea4bc4a758e47fcf2b1ae23408b016"
@@ -992,15 +1121,15 @@
         "available": false,
         "baseline": "stable diffusion 2",
         "config": {
             "download": [
                 {
                     "file_name": "coloringbook.ckpt",
                     "file_path": "",
-                    "file_url": "https://civitai.com/api/download/models/5978?type=Model&format=PickleTensor"
+                    "file_url": "https://civitai.com/api/download/models/5978?type=Model&format=PickleTensor&size=full&fp=fp16"
                 }
             ],
             "files": [
                 {
                     "md5sum": "853cb408368331239034be64811095d1",
                     "path": "coloringbook.ckpt",
                     "sha256sum": "ee10b26e6cd95370fdbd5f3a93684dc70ad67d505d9e21cc364552a7ca37a152"
@@ -1067,15 +1196,15 @@
         "available": false,
         "baseline": "stable diffusion 2",
         "config": {
             "download": [
                 {
                     "file_name": "ConceptSheet.ckpt",
                     "file_path": "",
-                    "file_url": "https://civitai.com/api/download/models/5635?type=Model&format=PickleTensor"
+                    "file_url": "https://civitai.com/api/download/models/5635?type=Model&format=PickleTensor&size=full&fp=fp16"
                 }
             ],
             "files": [
                 {
                     "md5sum": "4164e3765e41fc65d283360a1f406a51",
                     "path": "ConceptSheet.ckpt",
                     "sha256sum": "a938d435404da008edcb1a562cdf4f52363ac71fd7a7582839cc3cb068710ad2"
@@ -1480,14 +1609,47 @@
         "style": "other",
         "trigger": [
             "dnditem"
         ],
         "type": "ckpt",
         "version": "1.0"
     },
+    "DnD Map Generator": {
+        "available": false,
+        "baseline": "stable diffusion 1",
+        "config": {
+            "download": [
+                {
+                    "file_name": "dndMapGenerator.safetensors",
+                    "file_path": "",
+                    "file_url": "https://civitai.com/api/download/models/19517?type=Model&format=SafeTensor&size=full&fp=fp16"
+                }
+            ],
+            "files": [
+                {
+                    "path": "dndMapGenerator.safetensors",
+                    "sha256sum": "535d3a621d9ce06392cc554ac0d5ba1f0e68974a52902bf0c1f22eccf516ff28"
+                },
+                {
+                    "path": "v1-inference.yaml"
+                }
+            ]
+        },
+        "description": "This model is trained on various D&D Battlemaps. Use the negative prompt: 'grid' to improve some maps, or use the gridless version. Try to experiment with the CFG scale, 10 can create some amazing results but to each their own.",
+        "download_all": false,
+        "homepage": "https://civitai.com/models/5012/dnd-map-generator",
+        "name": "DnD Map Generator",
+        "nsfw": false,
+        "style": "other",
+        "trigger": [
+            "2d dnd battlemap"
+        ],
+        "type": "ckpt",
+        "version": "3.0"
+    },
     "Double Exposure Diffusion": {
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
                     "file_name": "dublex-diffusion.ckpt",
@@ -1525,15 +1687,15 @@
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
                     "file_name": "DreamLikeSamKuvshinov.ckpt",
                     "file_path": "",
-                    "file_url": "https://civitai.com/api/download/models/1642"
+                    "file_url": "https://civitai.com/api/download/models/1642?type=Model&format=PickleTensor&size=full&fp=fp16"
                 }
             ],
             "files": [
                 {
                     "md5sum": "0e836fa9fe4ed5a91ec1251513358ea8",
                     "path": "DreamLikeSamKuvshinov.ckpt",
                     "sha256sum": "d43a0899eb8be52939b612189e6e93d99722888fd74999baae214cfb78192188"
@@ -1805,14 +1967,45 @@
         "homepage": "https://civitai.com/models/11718/dungeons-n-waifus",
         "name": "Dungeons n Waifus",
         "nsfw": false,
         "style": "artistic",
         "type": "ckpt",
         "version": "1.0"
     },
+    "Edge Of Realism": {
+        "available": false,
+        "baseline": "stable diffusion 1",
+        "config": {
+            "download": [
+                {
+                    "file_name": "edgeOfRealism.safetensors",
+                    "file_path": "",
+                    "file_url": "https://civitai.com/api/download/models/51913?type=Model&format=SafeTensor&size=pruned&fp=fp16"
+                }
+            ],
+            "files": [
+                {
+                    "md5sum": "bda9e9b98d88c27f9256623147523d64",
+                    "path": "edgeOfRealism.safetensors",
+                    "sha256sum": "7f6146b8a9ad2a92b739954c1d5ef34e26fb0b65eef2d70ffd128e6046a3d0ab"
+                },
+                {
+                    "path": "v1-inference.yaml"
+                }
+            ]
+        },
+        "description": "A spin off from Level4. Built to produce high quality photos. Sometimes photos will come out as uncanny as they are on the edge of realism.",
+        "download_all": false,
+        "homepage": "https://civitai.com/models/21813/edge-of-realism",
+        "name": "Edge Of Realism",
+        "nsfw": true,
+        "style": "realistic",
+        "type": "ckpt",
+        "version": "2"
+    },
     "Eimis Anime Diffusion": {
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
                     "file_name": "eimis_anime-diffusion.ckpt",
@@ -1888,15 +2081,15 @@
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
                     "file_name": "Elldreths_Lucid_Mix.ckpt",
                     "file_path": "",
-                    "file_url": "https://civitai.com/api/download/models/1450?type=Model&format=PickleTensor"
+                    "file_url": "https://civitai.com/api/download/models/1450?type=Model&format=PickleTensor&size=full&fp=fp16"
                 }
             ],
             "files": [
                 {
                     "md5sum": "b2b73886b8d3cc040aea991f264acb56",
                     "path": "Elldreths_Lucid_Mix.ckpt",
                     "sha256sum": "d0cf7cf924c6a6f42eabed6729b8d6df3ef66ba2b4c35cb3d7e2f54a5d878166"
@@ -1922,15 +2115,15 @@
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
                     "file_name": "Elldreths_Retro_Mix.ckpt",
                     "file_path": "",
-                    "file_url": "https://civitai.com/api/download/models/1575?type=Model&format=PickleTensor"
+                    "file_url": "https://civitai.com/api/download/models/1575?type=Model&format=PickleTensor&size=full&fp=fp16"
                 }
             ],
             "files": [
                 {
                     "md5sum": "613d7ac32ac59db04e5209605d9e79c1",
                     "path": "Elldreths_Retro_Mix.ckpt",
                     "sha256sum": "8c6da97f03576dde964f3e508ef5595a28f0898dcdb275f1601d410e1c8adc03"
@@ -1962,15 +2155,15 @@
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
                     "file_name": "EpicDiffusion.ckpt",
                     "file_path": "",
-                    "file_url": "https://civitai.com/api/download/models/5677?type=Model&format=PickleTensor"
+                    "file_url": "https://civitai.com/api/download/models/5677?type=Model&format=PickleTensor&size=full&fp=fp16"
                 }
             ],
             "files": [
                 {
                     "md5sum": "db7bad70b29fa7ed613d30ced9e5f26a",
                     "path": "EpicDiffusion.ckpt",
                     "sha256sum": "ee6266109f4060b9bf134bf670ea75e663ec356352db6140b86828917340b162"
@@ -2467,15 +2660,15 @@
         "available": false,
         "baseline": "stable diffusion 2",
         "config": {
             "download": [
                 {
                     "file_name": "graphic-art.ckpt",
                     "file_path": "",
-                    "file_url": "https://civitai.com/api/download/models/9297?type=Model&format=PickleTensor"
+                    "file_url": "https://civitai.com/api/download/models/9297?type=Model&format=PickleTensor&size=full&fp=fp16"
                 }
             ],
             "files": [
                 {
                     "md5sum": "fe23f60ebb26bc8d2dfda9ed9363ce49",
                     "path": "graphic-art.ckpt",
                     "sha256sum": "72adf3e51f689cdc54cf0672a74a7a281d9f38e05bd6b2e730ea962c3a4014fa"
@@ -2493,14 +2686,47 @@
         "showcases": [
             "https://raw.githubusercontent.com/db0/AI-Horde-image-model-reference/main/showcase/graphic_art/01_graphicart.webp"
         ],
         "style": "other",
         "type": "ckpt",
         "version": "beta"
     },
+    "GuFeng": {
+        "available": false,
+        "baseline": "stable diffusion 1",
+        "config": {
+            "download": [
+                {
+                    "file_name": "GuFeng.safetensors",
+                    "file_path": "",
+                    "file_url": "https://civitai.com/api/download/models/42796?type=Model&format=SafeTensor&size=full&fp=fp16"
+                }
+            ],
+            "files": [
+                {
+                    "path": "GuFeng.safetensors",
+                    "sha256sum": "1f4fd502679cdbddb168f36ca11de3787097497eeb0e4f85bd1102618178e332"
+                },
+                {
+                    "path": "v1-inference.yaml"
+                }
+            ]
+        },
+        "description": "This is a model of ancient Chinese style, and it also belongs to the model series with ink and water orientation",
+        "download_all": false,
+        "homepage": "https://civitai.com/models/12903/gufeng",
+        "name": "GuFeng",
+        "nsfw": false,
+        "style": "anime",
+        "tags": [
+            "anime"
+        ],
+        "type": "ckpt",
+        "version": "2.0"
+    },
     "GuoFeng": {
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
                     "file_name": "GuoFeng.ckpt",
@@ -2670,15 +2896,15 @@
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
                     "file_name": "Healys.ckpt",
                     "file_path": "",
-                    "file_url": "https://civitai.com/api/download/models/1498"
+                    "file_url": "https://huggingface.co/BlancOfficial/Healy_AnimeBlend/resolve/main/healySAnimeBlend_17.ckpt"
                 }
             ],
             "files": [
                 {
                     "md5sum": "416566bada0313f4504857dcdbe530c6",
                     "path": "Healys.ckpt",
                     "sha256sum": "8416edf88cf48cc59c6cd36aece35acd4ae465aea934b7ff1e29b3f1049e2161"
@@ -2764,25 +2990,25 @@
                     "md5sum": "f9319c292efb474e950a5e2c5897fb56",
                     "path": "Illuminati.ckpt",
                     "sha256sum": "1cd89acd67160b32dee7e61125d8c1f0221370bf18ba021c93b7a75b2af36856"
                 },
                 {
                     "path": "v2-inference-v.yaml"
                 }
-            ],
-            "showcases": [
-                "https://raw.githubusercontent.com/db0/AI-Horde-image-model-reference/main/showcase/illuminati/001_muted001.webp",
-                "https://raw.githubusercontent.com/db0/AI-Horde-image-model-reference/main/showcase/illuminati/002_blank.webp"
             ]
         },
         "description": "Illuminati Diffusion is a latent text-to-image diffusion model that has been conditioned on high aesthetic synthetic images through fine-tuning. It was trained on 82,000 images locally with a single 3090ti, taking over 100 hours.",
         "download_all": false,
         "homepage": "https://civitai.com/models/11193",
         "name": "Illuminati Diffusion",
         "nsfw": false,
+        "showcases": [
+            "https://raw.githubusercontent.com/db0/AI-Horde-image-model-reference/main/showcase/illuminati/001_muted001.webp",
+            "https://raw.githubusercontent.com/db0/AI-Horde-image-model-reference/main/showcase/illuminati/002_blank.webp"
+        ],
         "style": "generalist",
         "type": "ckpt",
         "version": "1.1"
     },
     "Inkpunk Diffusion": {
         "available": false,
         "baseline": "stable diffusion 1",
@@ -2884,14 +3110,48 @@
         "homepage": "https://civitai.com/models/10720/jim-eidomode",
         "name": "Jim Eidomode",
         "nsfw": false,
         "style": "artistic",
         "type": "ckpt",
         "version": "1.0"
     },
+    "JoMad Diffusion": {
+        "available": false,
+        "baseline": "stable diffusion 1",
+        "config": {
+            "download": [
+                {
+                    "file_name": "jomadDiffusion.ckpt",
+                    "file_path": "",
+                    "file_url": "https://civitai.com/api/download/models/1286?type=Model&format=PickleTensor&size=full&fp=fp16"
+                }
+            ],
+            "files": [
+                {
+                    "md5sum": "43aa66b9ef9b799b155cd5d905d6ef88",
+                    "path": "jomadDiffusion.ckpt",
+                    "sha256sum": "bfdb1bc07f86a37363bdf04b778e0d528d28f25d2b78becc66f5b725452e4e62"
+                },
+                {
+                    "path": "v1-inference.yaml"
+                }
+            ]
+        },
+        "description": "SD 1.5 model trained on a sample of Joe Madureiras artwork, this model was combined with another anime style model to create the blend uploaded here.",
+        "download_all": false,
+        "homepage": "https://civitai.com/models/1223/jomad-diffusion",
+        "name": "JoMad Diffusion",
+        "nsfw": false,
+        "style": "anime",
+        "trigger": [
+            "style of joemadureira"
+        ],
+        "type": "ckpt",
+        "version": "1.0"
+    },
     "Kenshi": {
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
                     "file_name": "Kenshi.ckpt",
@@ -3067,15 +3327,15 @@
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
                     "file_name": "liberty.ckpt",
                     "file_path": "",
-                    "file_url": "https://civitai.com/api/download/models/6908?type=Model&format=PickleTensor"
+                    "file_url": "https://civitai.com/api/download/models/6908?type=Model&format=PickleTensor&size=full&fp=fp16"
                 }
             ],
             "files": [
                 {
                     "md5sum": "bde75d7ae88cc7896c1cdfd2f5bd9ea7",
                     "path": "liberty.ckpt",
                     "sha256sum": "b59a47e81c6b110dc02b8141928b44f2396928469f999f9228bc0920eb89de10"
@@ -3093,14 +3353,44 @@
         "showcases": [
             "https://raw.githubusercontent.com/db0/AI-Horde-image-model-reference/main/showcase/liberty/01_liberty.webp"
         ],
         "style": "realistic",
         "type": "ckpt",
         "version": "1.0"
     },
+    "Lyriel": {
+        "available": false,
+        "baseline": "stable diffusion 1",
+        "config": {
+            "download": [
+                {
+                    "file_name": "lyriel.safetensors",
+                    "file_path": "",
+                    "file_url": "https://civitai.com/api/download/models/50127?type=Model&format=SafeTensor&size=full&fp=fp16"
+                }
+            ],
+            "files": [
+                {
+                    "path": "lyriel.safetensors",
+                    "sha256sum": "4d91c4c2174557c2211ba32c54798b19a14c74d84f937d904a481f9b42a9e2ad"
+                },
+                {
+                    "path": "v1-inference.yaml"
+                }
+            ]
+        },
+        "description": "This model is generally designed for portraits and full-length anime style photos. Fantastic landscapes are quite decent. And it doesn't require kilometer-long queries to get a high-quality result.",
+        "download_all": false,
+        "homepage": "https://civitai.com/models/22922/lyriel",
+        "name": "Lyriel",
+        "nsfw": true,
+        "style": "artistic",
+        "type": "ckpt",
+        "version": "1.5"
+    },
     "Marvel Diffusion": {
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
                     "file_name": "marvel-diffusion.ckpt",
@@ -3498,15 +3788,15 @@
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
                     "file_name": "moedel.ckpt",
                     "file_path": "",
-                    "file_url": "https://civitai.com/api/download/models/2410?type=Model&format=PickleTensor"
+                    "file_url": "https://civitai.com/api/download/models/2410?type=Model&format=PickleTensor&size=full&fp=fp16"
                 }
             ],
             "files": [
                 {
                     "md5sum": "63132423ae711d87c813bf0f0442b154",
                     "path": "moedel.ckpt",
                     "sha256sum": "b2c2e471f84ad2581238719c7f49a2a6e5e87960fdaf2828696e7af8cae00f5d"
@@ -3532,15 +3822,15 @@
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
                     "file_name": "MoistMix.ckpt",
                     "file_path": "",
-                    "file_url": "https://civitai.com/api/download/models/5955?type=Model&format=PickleTensor"
+                    "file_url": "https://civitai.com/api/download/models/5955?type=Model&format=PickleTensor&size=full&fp=fp16"
                 }
             ],
             "files": [
                 {
                     "md5sum": "fe58cff02ec3c355d9d3abe925a775d5",
                     "path": "MoistMix.ckpt",
                     "sha256sum": "a01de4dd971acbf013363b202cac71dc4db7d7cfa36ca63b99d662dd89c520c6"
@@ -3589,14 +3879,45 @@
         "homepage": "https://civitai.com/models/8067/movie-diffusion-v12",
         "name": "Movie Diffusion",
         "nsfw": false,
         "style": "realistic",
         "type": "ckpt",
         "version": "1.2"
     },
+    "Neurogen": {
+        "available": false,
+        "baseline": "stable diffusion 1",
+        "config": {
+            "download": [
+                {
+                    "file_name": "neurogen.safetensors",
+                    "file_path": "",
+                    "file_url": "https://civitai.com/api/download/models/29681?type=Pruned%20Model&format=SafeTensor&size=pruned&fp=fp16"
+                }
+            ],
+            "files": [
+                {
+                    "md5sum": "95ce431e83ae9d8488e9989b39a14724",
+                    "path": "neurogen.safetensors",
+                    "sha256sum": "7ce537a0b7cca96f6862dda000b0d4054b8b996ae5859ddb2c196211447f99fc"
+                },
+                {
+                    "path": "v1-inference.yaml"
+                }
+            ]
+        },
+        "description": "This model gives a very good detail of skin and textures. Great for close-up photorealistic portraits as well as various characters and models.",
+        "download_all": false,
+        "homepage": "https://civitai.com/models/21616/neurogen-v11",
+        "name": "Neurogen",
+        "nsfw": true,
+        "style": "realistic",
+        "type": "ckpt",
+        "version": "1.1"
+    },
     "NeverEnding Dream": {
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
                     "file_name": "NED.ckpt",
@@ -3708,15 +4029,15 @@
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
                     "file_name": "OrbAI.ckpt",
                     "file_path": "",
-                    "file_url": "https://civitai.com/api/download/models/16595?type=Model&format=PickleTensor"
+                    "file_url": "https://civitai.com/api/download/models/16595?type=Model&format=PickleTensor&size=full&fp=fp16"
                 }
             ],
             "files": [
                 {
                     "md5sum": "1ed0a5f6efea5347e42d848a974c5829",
                     "path": "OrbAI.ckpt",
                     "sha256sum": "47563c68cf1aff6cd970dbeb4db0233f706ce264e8f8eb168d5f7aceeea8d549"
@@ -3742,15 +4063,15 @@
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
                     "file_name": "PFG.ckpt",
                     "file_path": "",
-                    "file_url": "https://civitai.com/api/download/models/1291"
+                    "file_url": "https://civitai.com/api/download/models/1291?type=Model&format=PickleTensor&size=full&fp=fp16"
                 }
             ],
             "files": [
                 {
                     "md5sum": "07dc65f652bb400af4d03b0bf6a41b95",
                     "path": "PFG.ckpt",
                     "sha256sum": "5a369d04a05862bdf83acb86fa9aa4ea65c9bcc4102badc01821e851f34cc1d7"
@@ -3810,15 +4131,15 @@
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
                     "file_name": "PPP.ckpt",
                     "file_path": "",
-                    "file_url": "https://civitai.com/api/download/models/1304"
+                    "file_url": "https://civitai.com/api/download/models/1304?type=Model&format=PickleTensor&size=full&fp=fp16"
                 }
             ],
             "files": [
                 {
                     "md5sum": "0e9012fab5382c7c3e9f3365e474835e",
                     "path": "PPP.ckpt",
                     "sha256sum": "40c6475ecb9aacee74f19a92a43d36b4485f16dda90acbdff79801e9c1798bb4"
@@ -3843,15 +4164,15 @@
         "available": false,
         "baseline": "stable diffusion 2",
         "config": {
             "download": [
                 {
                     "file_name": "PRMJ.ckpt",
                     "file_path": "",
-                    "file_url": "https://civitai.com/api/download/models/7592?type=Model&format=PickleTensor"
+                    "file_url": "https://civitai.com/api/download/models/7592?type=Model&format=PickleTensor&size=full&fp=fp16"
                 }
             ],
             "files": [
                 {
                     "md5sum": "44cd3e53b653288bab002c55200a3d6e",
                     "path": "PRMJ.ckpt",
                     "sha256sum": "e40298941c61102383e4839649c47610fd7fe58d0e052b041767d6a321d8f83a"
@@ -4275,15 +4596,15 @@
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
                     "file_name": "Protogen_Anime.ckpt",
                     "file_path": "",
-                    "file_url": "https://civitai.com/api/download/models/4007?type=Pruned%20Model&format=PickleTensor"
+                    "file_url": "https://civitai.com/api/download/models/4007?type=Pruned%20Model&format=PickleTensor&size=pruned&fp=fp16"
                 }
             ],
             "files": [
                 {
                     "md5sum": "4f2220296e0409c75f5752df05f843ca",
                     "path": "Protogen_Anime.ckpt",
                     "sha256sum": "eea02a02bfa43a929306f4daddad7698d7163055ed35ead53e4302c941c87b76"
@@ -4343,15 +4664,15 @@
         "available": false,
         "baseline": "stable diffusion 2",
         "config": {
             "download": [
                 {
                     "file_name": "pulp_vectorart.ckpt",
                     "file_path": "",
-                    "file_url": "https://civitai.com/api/download/models/5859?type=Model&format=PickleTensor"
+                    "file_url": "https://civitai.com/api/download/models/5859?type=Model&format=PickleTensor&size=full&fp=fp16"
                 }
             ],
             "files": [
                 {
                     "md5sum": "f3427844a139d5be2c4b4cec2e67b2f1",
                     "path": "pulp_vectorart.ckpt",
                     "sha256sum": "0c27deb0c848bc97330d17c6916f651ccc2bf154905d1e29f9dcdfc6d12ee1c5"
@@ -4515,15 +4836,15 @@
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
                     "file_name": "rainbowpatch.ckpt",
                     "file_path": "",
-                    "file_url": "https://civitai.com/api/download/models/6432?type=Model&format=PickleTensor"
+                    "file_url": "https://civitai.com/api/download/models/6432?type=Model&format=PickleTensor&size=full&fp=fp16"
                 }
             ],
             "files": [
                 {
                     "md5sum": "b082ad98aeedcd28b9164162a1ccf3e1",
                     "path": "rainbowpatch.ckpt",
                     "sha256sum": "d9d11a9ff2584632d40fd7b51821c4711ed98582937edbf0d96558ac09f97755"
@@ -4661,15 +4982,15 @@
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
                     "file_name": "RealisticVision.ckpt",
                     "file_path": "",
-                    "file_url": "https://civitai.com/api/download/models/6987?type=Model&format=PickleTensor"
+                    "file_url": "https://civitai.com/api/download/models/6987?type=Model&format=PickleTensor&size=full&fp=fp16"
                 }
             ],
             "files": [
                 {
                     "md5sum": "8c41f9f090e4c924b2a05cf21608e6c0",
                     "path": "RealisticVision.ckpt",
                     "sha256sum": "77e392958a6b2ce335fe6ed0cb8ebb9f5cfb48706bfde9c28d4721f4ce65619e"
@@ -4730,45 +5051,44 @@
     },
     "Rev Animated": {
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
-                    "file_name": "Rev-animated.ckpt",
+                    "file_name": "Rev-animated.safetensors",
                     "file_path": "",
-                    "file_url": "https://huggingface.co/Airic/mirrors/resolve/main/RevAnimated_v11_inclVAE.ckpt"
+                    "file_url": "https://civitai.com/api/download/models/46846?type=Model&format=SafeTensor&size=full&fp=fp32"
                 }
             ],
             "files": [
                 {
-                    "md5sum": "67fb60349b3b2fc98a7b7c6fa1d02e4a",
-                    "path": "Rev-animated.ckpt",
-                    "sha256sum": "669b5c04f0ac98b225b2e8d53259748fdf07ef7a8d7e6ea7b6359783ced855e2"
+                    "path": "Rev-animated.safetensors",
+                    "sha256sum": "4199bcdd147e11328d5f3560301d5a7ab4ac7eeefbf49dc3eb663cb3e772b9ac"
                 },
                 {
                     "path": "v1-inference.yaml"
                 }
             ]
         },
         "description": "This model is mainly intended for Portraits and Full Body Anime-like pictures. Fantasy landscapes are decent.",
         "download_all": false,
-        "homepage": "https://civitai.com/models/7371/rev-animated",
+        "homepage": "https://civitai.com/models/7371?modelVersionId=46846",
         "name": "Rev Animated",
         "nsfw": true,
         "showcases": [
             "https://raw.githubusercontent.com/db0/AI-Horde-image-model-reference/main/showcase/rev_animated/001_muted.webp"
         ],
         "style": "anime",
         "tags": [
             "anime",
             "character"
         ],
         "type": "ckpt",
-        "version": "1.1"
+        "version": "1.2.2"
     },
     "Robo-Diffusion": {
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
@@ -4937,15 +5257,15 @@
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
                     "file_name": "seek-art-mega.ckpt",
                     "file_path": "",
-                    "file_url": "https://civitai.com/api/download/models/22808?type=Model&format=PickleTensor"
+                    "file_url": "https://civitai.com/api/download/models/22808?type=Model&format=PickleTensor&size=full&fp=fp16"
                 }
             ],
             "files": [
                 {
                     "md5sum": "a1ae126a2a57f47115082ada5f527cc5",
                     "path": "seek-art-mega.ckpt",
                     "sha256sum": "5600db52c98225fcd410e43c2995c7ec2aaa34dd4dc94cad59ecddf240dbaf23"
@@ -5258,15 +5578,15 @@
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
                     "file_name": "Synthpunk.ckpt",
                     "file_path": "",
-                    "file_url": "https://civitai.com/api/download/models/1144?format=PickleTensor"
+                    "file_url": "https://civitai.com/api/download/models/1144?type=Model&format=PickleTensor&size=pruned&fp=fp16"
                 }
             ],
             "files": [
                 {
                     "md5sum": "96b9822c6c38b156eb9b958748699164",
                     "path": "Synthpunk.ckpt",
                     "sha256sum": "dc4c67171e2eb64b1a79da7fde1cb3fcbef65364b12c8f5e30a0141fd8c88233"
@@ -5289,15 +5609,15 @@
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
                     "file_name": "t-shirt_diffusion.ckpt",
                     "file_path": "",
-                    "file_url": "https://civitai.com/api/download/models/5365?type=Model&format=PickleTensor"
+                    "file_url": "https://civitai.com/api/download/models/5365?type=Model&format=PickleTensor&size=full&fp=fp16"
                 }
             ],
             "files": [
                 {
                     "md5sum": "37e58d85c8b0815f61526afa1c5d98e4",
                     "path": "t-shirt_diffusion.ckpt",
                     "sha256sum": "a7832ba06828551744094e7a80225bae233f0aac1cf579dff764b3d0e845da8e"
@@ -5326,15 +5646,15 @@
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
                     "file_name": "tshirt-print-designs.ckpt",
                     "file_path": "",
-                    "file_url": "https://civitai.com/api/download/models/6098?type=Model&format=PickleTensor"
+                    "file_url": "https://civitai.com/api/download/models/6098?type=Model&format=PickleTensor&size=full&fp=fp16"
                 }
             ],
             "files": [
                 {
                     "md5sum": "d1f51ba806e29742df8adbf35169bd2c",
                     "path": "tshirt-print-designs.ckpt",
                     "sha256sum": "d7686e58ab3cd745515bcf6489a5bec812458b002482f5d3b955c393be95c4a7"
@@ -5509,15 +5829,15 @@
         "available": false,
         "baseline": "stable diffusion 1",
         "config": {
             "download": [
                 {
                     "file_name": "URPM.ckpt",
                     "file_path": "",
-                    "file_url": "https://civitai.com/api/download/models/15640?type=Pruned%20Model&format=PickleTensor"
+                    "file_url": "https://civitai.com/api/download/models/15640?type=Pruned%20Model&format=PickleTensor&size=pruned&fp=fp16"
                 }
             ],
             "files": [
                 {
                     "md5sum": "15aa3ca9ab7ae6de04424bcafb556cc4",
                     "path": "URPM.ckpt",
                     "sha256sum": "ce9f23b04771e636b37b7d52ff0d0f20f176f170af1ebbe9203d2b3e4a88522e"
@@ -5732,15 +6052,15 @@
         "available": false,
         "baseline": "stable diffusion 2",
         "config": {
             "download": [
                 {
                     "file_name": "vector_art.ckpt",
                     "file_path": "",
-                    "file_url": "https://civitai.com/api/download/models/5265?type=Model&format=PickleTensor"
+                    "file_url": "https://civitai.com/api/download/models/5265?type=Model&format=PickleTensor&size=full&fp=fp16"
                 }
             ],
             "files": [
                 {
                     "md5sum": "218567e0a45db9139337c888a40285f1",
                     "path": "vector_art.ckpt",
                     "sha256sum": "360d741263d05dd2fc3efe42c057a6e1faf84b30e634934fac5febfcd632f5d6"
```

### Comparing `hordelib-0.9.5/hordelib/model_manager/base.py` & `hordelib-1.0.0/hordelib/model_manager/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,38 @@
-import gc
 import hashlib
 import importlib.resources as importlib_resources
 import json
 import os
 import shutil
 import threading
 import time
 import typing
 import zipfile
 from abc import ABC, abstractmethod
+from contextlib import nullcontext
 from pathlib import Path
 from typing import Any
 from uuid import uuid4
 
 import git
 import psutil
 import requests
 import torch
 from loguru import logger
 from tqdm import tqdm
 from transformers import logging
 
 from hordelib.cache import get_cache_directory
-from hordelib.comfy_horde import get_models_on_gpu, remove_model_from_memory
+from hordelib.comfy_horde import (
+    cleanup,
+    get_models_on_gpu,
+    get_torch_free_vram_mb,
+    load_model_to_gpu,
+    remove_model_from_memory,
+)
 from hordelib.comfy_horde import get_torch_device as _get_torch_device
 from hordelib.config_path import get_hordelib_path
 from hordelib.consts import REMOTE_MODEL_DB
 from hordelib.settings import UserSettings
 
 logging.set_verbosity_error()
 
@@ -43,29 +49,34 @@
     models_db_path: Path
     cuda_available: bool
     cuda_devices: list
     recommended_gpu: list
     download_reference: bool
     remote_db: str
     _mutex = threading.RLock()
+    _disk_write_mutex = threading.Lock()
 
     def get_torch_device(self):
         return _get_torch_device()
 
     def get_loaded_models(self):
         return self._loaded_models.copy()
 
     def add_loaded_model(self, model_name, model_data):
         with self._mutex:
             self._loaded_models[model_name] = model_data
 
     def remove_loaded_model(self, model_name):
+        logger.debug(f"Received request to remove loaded model {model_name}")
         with self._mutex:
             if model_name in self._loaded_models:
+                logger.debug(f"Removing loaded model {model_name}")
                 del self._loaded_models[model_name]
+            else:
+                logger.debug(f"Could not find loaded model {model_name}")
 
     def __init__(
         self,
         *,
         models_db_name: str,  # XXX Remove default
         modelFolder: str | None = None,
         download_reference: bool = False,
@@ -96,14 +107,15 @@
         )
 
         self.cuda_available = torch.cuda.is_available()  # XXX Remove?
         self.cuda_devices, self.recommended_gpu = self.get_cuda_devices()  # XXX Remove?
         self.remote_db = f"{REMOTE_MODEL_DB}{self.models_db_name}.json"
         self.download_reference = download_reference
         self.loadModelDatabase()
+        self.load_disk_cached_models()
 
     def loadModelDatabase(self, list_models=False):
         if self.model_reference:
             logger.info(
                 (
                     "Model reference was already loaded."
                     f" Got {len(self.model_reference)} models for {self.models_db_name}."
@@ -142,14 +154,25 @@
         logger.info(
             f"Got {len(self.available_models)} available models for {self.models_db_name}.",
         )
         if list_models:
             for model in self.available_models:
                 logger.info(model)
 
+    def load_disk_cached_models(self):
+        """Assume we've already loaded any disk cached models"""
+        if not self.can_cache_on_disk():
+            return
+        for model_name in self.available_models:
+            if self.have_model_cache(model_name):
+                self.add_loaded_model(model_name, self.load_from_disk_cache(model_name))
+
+    def load_from_disk_cache(self, model_name):
+        return False
+
     def download_model_reference(self):
         try:
             logger.init("Model Reference", status="Downloading")
             response = requests.get(self.remote_db)
             logger.init_ok("Model Reference", status="OK")
             models = response.json()
             return models
@@ -164,79 +187,137 @@
     def _modelref_to_name(self, modelref):
         with self._mutex:
             for name, data in self.get_loaded_models().items():
                 if modelref and data["model"] is modelref:
                     return name
             return None
 
-    def ensure_memory_available(self):
-        # Can this type of model be cached?
-        if not self.can_cache_on_disk():
-            return
+    def get_free_ram_mb(self):
+        return int(psutil.virtual_memory().available / (1024 * 1024))
+
+    def ensure_ram_available(self):
         with self._mutex:
             # If we have less than the minimum RAM free, free some up
-            freemem = round(psutil.virtual_memory().available / (1024 * 1024))
-            logger.debug(f"Free RAM is: {freemem} MB, ({len(self.get_loaded_models())} models loaded in RAM)")
-            if freemem > UserSettings.ram_to_leave_free_mb + 4096:
-                return
-            logger.debug("Not enough free RAM attempting to free some")
-            # Grab a list of models (ModelPatcher) that are loaded on the gpu
-            # These are actually returned with the least important at the bottom of the list
-            busy_models = get_models_on_gpu()
-            # Try to find one we have in ram that isn't on the gpu
-            idle_model = None
-            for ram_model_name, ram_model_data in self.get_loaded_models().items():
-                if type(ram_model_data["model"]) is not str and ram_model_data["model"] not in busy_models:
-                    idle_model = ram_model_name
-                    break
-            # If we didn't have one hanging around in ram not on the gpu
-            # pick the least used gpu model
-            if not idle_model and busy_models:
-                idle_model = self._modelref_to_name(busy_models[-1])
-
-            if idle_model:
-                logger.debug(f"Moving model {idle_model} to disk to free up RAM")
-                self.move_to_disk_cache(idle_model)
-            else:
-                # Nothing else to release
-                logger.debug("Could not find a model to free RAM")
+            # Although, perhaps we have plenty of available vram, in which case we
+            # can consider moving something from ram to vram.
+            attempts = 2  # if ram isn't being released yet, no point keep trying
+            while (
+                self.get_free_ram_mb() < UserSettings.get_ram_to_leave_free_mb()
+                and attempts
+                and len(self.get_loaded_models()) > 0
+            ):
+                logger.debug(
+                    f"Free RAM is: {self.get_free_ram_mb()} MB, "
+                    f"({len(self.get_loaded_models())} models loaded in RAM)",
+                )
+                logger.debug("Not enough free RAM attempting to free some")
+                # Grab a list of models (ModelPatcher) that are loaded on the gpu
+                # These are actually returned with the least important at the bottom of the list
+                busy_models = get_models_on_gpu()
+                # Try to find one we have in ram that isn't on the gpu
+                idle_model = None
+                idle_model_data = None
+                for ram_model_name, ram_model_data in self.get_loaded_models().items():
+                    if type(ram_model_data["model"]) is not str and ram_model_data["model"] not in busy_models:
+                        idle_model = ram_model_name
+                        idle_model_data = ram_model_data
+                        break
+
+                # Should we move to vram rather than disk cache or free completely?
+                # First try to determine the headroom we have on vram and ram even though that requires
+                # that we brave entry into Tazlin's UserSettings trap...
+                vram_headroom = get_torch_free_vram_mb() - UserSettings.get_vram_to_leave_free_mb()
+                ram_headroom = self.get_free_ram_mb() - UserSettings.get_ram_to_leave_free_mb()
+                # Don't try this unless we have 1500MB head room at least
+                if vram_headroom > ram_headroom and vram_headroom > 1500:
+                    logger.debug("More free VRAM than RAM, consider RAM->VRAM migration")
+                    if self.can_move_to_vram() and idle_model and load_model_to_gpu(idle_model_data["model"]):
+                        return
+                    # We failed to move a model to vram, continue with plan A
+
+                # If we didn't have one hanging around in ram not on the gpu
+                # pick the least used gpu model
+                if not idle_model and busy_models:
+                    idle_model = self._modelref_to_name(busy_models[-1])
+
+                if idle_model:
+                    # Can this type of model be cached?
+                    if self.can_cache_on_disk():
+                        logger.debug(f"Moving model {idle_model} to disk to free up RAM")
+                        self.move_to_disk_cache(idle_model)
+                        # Try to release ram right now
+                        cleanup()
+                    elif self.can_auto_unload():
+                        # Unload the model to free ram
+                        self.unload_model(idle_model)
+                        # Try to release ram right now
+                        cleanup()
+                else:
+                    # Nothing else to release
+                    logger.debug("Could not find a model to free RAM")
+
+                # Try again if we must
+                attempts -= 1
 
     # @abstractmethod # TODO
     def move_to_disk_cache(self, model_name):
         pass
 
+    # @abstractmethod # TODO
+    def move_from_disk_cache(self, model_name, model, clip, vae):
+        pass
+
+    # @abstractmethod # TODO
     def can_cache_on_disk(self):
         """Can this of type model be cached on disk?"""
         return False
 
+    # @abstractmethod # TODO
+    def can_auto_unload(self):
+        """Can/should we ever auto unload this model to release memory resources.
+
+        Not a great idea with something like the safety checker.
+        """
+        return False
+
+    # @abstractmethod # TODO
+    def can_move_to_vram(self):
+        """Can we move this model directly to the GPU to save ram?
+
+        XXX This is realistically only possible with compvis right now
+        """
+        return False
+
     def load(
         self,
         model_name: str,
         *,
         half_precision: bool = True,
         gpu_id: int | None = 0,
         cpu_only: bool = False,
         **kwargs,
     ):  # XXX # FIXME
         with self._mutex:
-            self.ensure_memory_available()
-            if model_name not in self.model_reference:
+            self.ensure_ram_available()
+            local = self.is_local_model(model_name)
+            if not local and model_name not in self.model_reference:
                 logger.error(f"{model_name} not found")
                 return False
-            if model_name not in self.available_models:
-                logger.error(f"{model_name} not available")
+            if not local and model_name not in self.available_models:
+                logger.init_warn(f"{model_name} may need to be downloaded, checking...", status="Loading")
                 download_succeeded = self.download_model(model_name)
                 if not download_succeeded:
                     logger.init_err(f"{model_name} failed to download", status="Error")
                     return False
                 logger.init_ok(f"{model_name}", status="Downloaded")
             if model_name not in self.get_loaded_models():
-                model_validated = self.validate_model(model_name)
-                if not model_validated:
-                    return False
+                if not local:
+                    model_validated = self.validate_model(model_name)
+                    if not model_validated:
+                        return False
                 logger.init(f"{model_name}", status="Loading")
 
                 tic = time.time()
                 logger.init(f"{model_name}", status="Loading")
 
                 try:
                     self.add_loaded_model(
@@ -259,17 +340,24 @@
 
                 logger.init_ok(f"{model_name}: {round(toc-tic,2)} seconds", status="Loaded")
                 return True
             return None
 
     def getFullModelPath(self, model_name: str):
         """Returns the fully qualified filename for the specified model."""
-        ckpt_path = self.get_model_files(model_name)[0]["path"]  # XXX Rework?
+        if not self.is_local_model(model_name):
+            ckpt_path = self.get_model_files(model_name)[0]["path"]  # XXX Rework?
+        else:
+            ckpt_path = model_name
+
         return f"{self.modelFolderPath}/{ckpt_path}"
 
+    def is_local_model(self, model_name):
+        return False
+
     @abstractmethod
     def modelToRam(
         self,
         *,
         model_name: str,
         half_precision: bool = True,
         gpu_id: int | None = None,
@@ -293,15 +381,15 @@
         return self.model_reference.get(model_name)
 
     def get_model_files(self, model_name: str):
         """
         :param model_name: Name of the model
         Returns the files for a model
         """
-        return self.model_reference[model_name]["config"]["files"]
+        return self.model_reference.get(model_name, {}).get("config", {}).get("files", [])
 
     def get_model_download(self, model_name: str):
         """
         :param model_name: Name of the model
         Returns the download details for a model
         """
         return self.model_reference[model_name]["config"]["download"]
@@ -364,20 +452,30 @@
         """
         :param model_name: Name of the model
         Issue a request to unload a model, completely remove it, free all resources, forget it exists.
         This may not be possible right now, as it may be being used, so we actually issue a request for it to
         be unloaded at the earliest opportunity.
         """
         with self._mutex:
+            logger.debug(f"Model Manager received unload model {model_name} request (mutex locked)")
             if model_name in self._loaded_models:
-                self.free_model_resources(model_name)
+                # If this model is not in ram, just on disk cache don't try to free memory resources
+                model_data = self._loaded_models[model_name].get("model")
+                if not isinstance(model_data, str):
+                    logger.debug(f"{model_name} is on loaded models list, trying free resources")
+                    self.free_model_resources(model_name)
                 self.remove_loaded_model(model_name)
+                logger.debug("Model Manager done with model unload request (mutex released)")
                 return True
+            else:
+                logger.debug(f"Model {model_name} is not in loaded models list so can't unload")
+        logger.debug(f"Model manager done with unload request for model {model_name}")
 
     def free_model_resources(self, model_name: str):
+        logger.debug(f"Received request to free model memory resources for {model_name}")
         with self._mutex:
             remove_model_from_memory(model_name, self.get_loaded_model(model_name))
 
     def unload_all_models(self):
         """
         Unloads all models
         """
@@ -508,18 +606,19 @@
         Returns True if the file is valid, False otherwise
         """
         full_path = f"{self.modelFolderPath}/{file_details['path']}"
 
         # Default to sha256 hashes
         if "sha256sum" in file_details:
             logger.debug(f"Getting sha256sum of {full_path}")
-            sha256_file_hash = self.get_file_sha256_hash(full_path)
+            sha256_file_hash = self.get_file_sha256_hash(full_path).lower()
+            expected_hash = file_details["sha256sum"].lower()
             logger.debug(f"sha256sum: {sha256_file_hash}")
-            logger.debug(f"Expected: {file_details['sha256sum']}")
-            return file_details["sha256sum"] == sha256_file_hash
+            logger.debug(f"Expected: {expected_hash}")
+            return expected_hash == sha256_file_hash
 
         # If sha256 is not available, fall back to md5
         if "md5sum" in file_details:
             logger.debug(f"Getting md5sum of {full_path}")
             md5_file_hash = self.get_file_md5sum_hash(full_path)
             logger.debug(f"md5sum: {md5_file_hash}")
             logger.debug(f"Expected: {file_details['md5sum']}")
@@ -716,15 +815,15 @@
         """
         # XXX this has no fall back and always returns true
         for model in self.get_filtered_model_names(download_all=True):
             if not self.check_model_available(model):
                 logger.init(f"{model}", status="Downloading")  # logger.init
                 self.download_model(model)
             else:
-                logger.init(f"{model} is already downloaded.")
+                logger.init(f"{model} is already downloaded.", status="Skipped")
         return True
 
     def check_model_available(self, model_name: str) -> bool:
         """
         :param model_name: Name of the model
         Checks if the model is available.
         Returns True if the model is available, False otherwise.
```

### Comparing `hordelib-0.9.5/hordelib/model_manager/blip.py` & `hordelib-1.0.0/hordelib/model_manager/blip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/model_manager/clip.py` & `hordelib-1.0.0/hordelib/model_manager/clip.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             self.add_loaded_models(model_name, loaded_model_info)
         else:
             logger.error(
                 f"Unknown model type: {self.model_reference[model_name]['type']}",
             )
             return {}  # XXX # FIXME
         if not loaded_model_info:
-            logger.init_error(f"Failed to load {model_name}", status="Error")
+            logger.init_err(f"Failed to load {model_name}", status="Error")
             return {}  # XXX # FIXME
 
         logger.init_ok(f"Loading {model_name}", status="Success")  # logger.init_ok
         toc = time.time()
         logger.init_ok(
             f"Loading {model_name}: Took {toc-tic} seconds",
             status="Success",
```

### Comparing `hordelib-0.9.5/hordelib/model_manager/codeformer.py` & `hordelib-1.0.0/hordelib/model_manager/diffusers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,25 @@
-import time
 import typing
 
-from loguru import logger
 from typing_extensions import override
 
-from hordelib import comfy_horde
+from hordelib.comfy_horde import horde_load_checkpoint
 from hordelib.consts import MODEL_CATEGORY_NAMES, MODEL_DB_NAMES
 from hordelib.model_manager.base import BaseModelManager
 
 
-class CodeFormerModelManager(BaseModelManager):
+class DiffusersModelManager(BaseModelManager):
     def __init__(self, download_reference=False):
         super().__init__(
-            models_db_name=MODEL_DB_NAMES[MODEL_CATEGORY_NAMES.codeformer],
+            models_db_name=MODEL_DB_NAMES[MODEL_CATEGORY_NAMES.diffusers],
             download_reference=download_reference,
         )
 
     @override
     def modelToRam(
         self,
         model_name: str,
         **kwargs,
     ) -> dict[str, typing.Any]:
-        model_path = self.getFullModelPath(model_name)
-        sd = comfy_horde.load_torch_file(model_path)
-        out = comfy_horde.load_state_dict(sd).eval()
-
-        # FIXME This is a hack to force the model to the GPU which shouldn't be here
-        # FIXME but is here as our facefix plugin is a bit dodgy
-        return {"model": out.to(self.get_torch_device())}
+        return horde_load_checkpoint(
+            ckpt_path=self.getFullModelPath(model_name),
+        )
```

### Comparing `hordelib-0.9.5/hordelib/model_manager/compvis.py` & `hordelib-1.0.0/hordelib/model_manager/compvis.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import copy
 import os
 import pickle
 import typing
 
+from loguru import logger
 from typing_extensions import override
 
+from hordelib import UserSettings
 from hordelib.comfy_horde import horde_load_checkpoint
 from hordelib.consts import MODEL_CATEGORY_NAMES, MODEL_DB_NAMES, MODEL_FOLDER_NAMES
 from hordelib.model_manager.base import BaseModelManager
 
 
 class CompVisModelManager(BaseModelManager):
     def __init__(
@@ -19,63 +21,108 @@
         super().__init__(
             modelFolder=MODEL_FOLDER_NAMES[MODEL_CATEGORY_NAMES.compvis],
             models_db_name=MODEL_DB_NAMES[MODEL_CATEGORY_NAMES.compvis],
             download_reference=download_reference,
         )
 
     @override
+    def is_local_model(self, model_name):
+        parts = os.path.splitext(model_name.lower())
+        if parts[-1] in [".safetensors", ".ckpt"]:
+            return True
+        return False
+
+    @override
     def modelToRam(
         self,
         model_name: str,
         **kwargs,
     ) -> dict[str, typing.Any]:
-
         embeddings_path = os.getenv("HORDE_MODEL_DIR_EMBEDDINGS", "./")
 
+        if not kwargs.get("local", False):
+            ckpt_path = self.getFullModelPath(model_name)
+        else:
+            ckpt_path = os.path.join(self.modelFolderPath, model_name)
         return horde_load_checkpoint(
-            ckpt_path=self.getFullModelPath(model_name),
+            ckpt_path=ckpt_path,
             embeddings_path=embeddings_path,
         )
 
     def can_cache_on_disk(self):
         """Can this of type model be cached on disk?"""
+        if UserSettings.disable_disk_cache.active:
+            return False
+        return True
+
+    def can_auto_unload(self):
+        # Allow compvis models to be auto unloaded
+        return True
+
+    def can_move_to_vram(self):
+        # Allow moving directly to vram to save ram
         return True
 
     def get_model_cache_filename(self, model_name):
         cache_dir = os.getenv("AIWORKER_TEMP_DIR", "./tmp")
         # Create cache directory if it doesn't already exist
         if not os.path.isdir(cache_dir):
             os.makedirs(cache_dir, exist_ok=True)
         cache_file = os.path.join(cache_dir, model_name)
         return f"{cache_file}.hordelib.cache"
 
     def have_model_cache(self, model_name):
         model_filename = self.getFullModelPath(model_name)
         cache_file = self.get_model_cache_filename(model_name)
         if os.path.exists(cache_file):
+            if not self.validate_model(model_name):
+                # The model is invalid, so delete the cache file because that's almost certainly no good either
+                # This should only happen if the model was updated on disk manually, or the model reference changed
+                logger.error(f"The model {model_name} is invalid, deleting the cache file.")
+                os.remove(path=cache_file)
+                return False
             # We have a cache file but only consider it valid if it's up to date
             model_timestamp = os.path.getmtime(model_filename)
             cache_timestamp = os.path.getmtime(cache_file)
             if model_timestamp <= cache_timestamp:
                 return True
         return False
 
+    def load_from_disk_cache(self, model_name):
+        filename = self.get_model_cache_filename(model_name)
+        logger.info(f"Model {model_name} warm loaded from disk cache")
+        return {
+            "model": filename,
+            "clip": filename,
+            "vae": filename,
+            "clipVisionModel": None,
+        }
+
     def move_to_disk_cache(self, model_name):
         with self._mutex:
             cache_file = self.get_model_cache_filename(model_name)
             # Serialise our objects
             model_data = copy.copy(self.get_loaded_model(model_name))
             components = ["model", "vae", "clip"]
             if not self.have_model_cache(model_name):
-                with open(cache_file, "wb") as cache:
-                    for component in components:
-                        pickle.dump(
-                            self.get_loaded_model(model_name)[component],
-                            cache,
-                            protocol=pickle.HIGHEST_PROTOCOL,
-                        )
+                # Only do one sequential write at a time
+                with self._disk_write_mutex:
+                    with open(cache_file, "wb") as cache:
+                        for component in components:
+                            pickle.dump(
+                                self.get_loaded_model(model_name)[component],
+                                cache,
+                                protocol=pickle.HIGHEST_PROTOCOL,
+                            )
             for component in components:
                 model_data[component] = cache_file
             # Remove from vram/ram
             self.free_model_resources(model_name)
             # Point the model to the cache
             self.add_loaded_model(model_name, model_data)
+
+    def move_from_disk_cache(self, model_name, model, clip, vae):
+        self.ensure_ram_available()
+        with self._mutex:
+            self._loaded_models[model_name]["model"] = model
+            self._loaded_models[model_name]["clip"] = clip
+            self._loaded_models[model_name]["vae"] = vae
```

### Comparing `hordelib-0.9.5/hordelib/model_manager/controlnet.py` & `hordelib-1.0.0/hordelib/model_manager/controlnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/model_manager/diffusers.py` & `hordelib-1.0.0/hordelib/model_manager/codeformer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import typing
 
 from typing_extensions import override
 
-from hordelib.comfy_horde import horde_load_checkpoint
+from hordelib import comfy_horde
 from hordelib.consts import MODEL_CATEGORY_NAMES, MODEL_DB_NAMES
 from hordelib.model_manager.base import BaseModelManager
 
-# from nataili.util.voodoo import push_diffusers_pipeline_to_plasma
 
-
-class DiffusersModelManager(BaseModelManager):
+class CodeFormerModelManager(BaseModelManager):
     def __init__(self, download_reference=False):
         super().__init__(
-            models_db_name=MODEL_DB_NAMES[MODEL_CATEGORY_NAMES.diffusers],
+            models_db_name=MODEL_DB_NAMES[MODEL_CATEGORY_NAMES.codeformer],
             download_reference=download_reference,
         )
 
     @override
     def modelToRam(
         self,
         model_name: str,
         **kwargs,
     ) -> dict[str, typing.Any]:
-        return horde_load_checkpoint(
-            ckpt_path=self.getFullModelPath(model_name),
-        )
+        model_path = self.getFullModelPath(model_name)
+        sd = comfy_horde.load_torch_file(model_path)
+        out = comfy_horde.load_state_dict(sd).eval()
+        return {"model": out}
```

### Comparing `hordelib-0.9.5/hordelib/model_manager/esrgan.py` & `hordelib-1.0.0/hordelib/model_manager/esrgan.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import typing
 
 from typing_extensions import override
 
 from hordelib import comfy_horde
 from hordelib.consts import MODEL_CATEGORY_NAMES, MODEL_DB_NAMES
 from hordelib.model_manager.base import BaseModelManager
@@ -11,14 +12,21 @@
     def __init__(self, download_reference=False):
         super().__init__(
             models_db_name=MODEL_DB_NAMES[MODEL_CATEGORY_NAMES.esrgan],
             download_reference=download_reference,
         )
 
     @override
+    def is_local_model(self, model_name):
+        parts = os.path.splitext(model_name.lower())
+        if parts[-1] in [".pth"]:
+            return True
+        return False
+
+    @override
     def modelToRam(
         self,
         model_name: str,
         **kwargs,
     ) -> dict[str, typing.Any]:
         model_path = self.getFullModelPath(model_name)
         sd = comfy_horde.load_torch_file(model_path)
```

### Comparing `hordelib-0.9.5/hordelib/model_manager/gfpgan.py` & `hordelib-1.0.0/hordelib/model_manager/gfpgan.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import typing
 
 from typing_extensions import override
 
 from hordelib import comfy_horde
 from hordelib.consts import MODEL_CATEGORY_NAMES, MODEL_DB_NAMES
 from hordelib.model_manager.base import BaseModelManager
@@ -11,14 +12,21 @@
     def __init__(self, download_reference=False):
         super().__init__(
             models_db_name=MODEL_DB_NAMES[MODEL_CATEGORY_NAMES.gfpgan],
             download_reference=download_reference,
         )
 
     @override
+    def is_local_model(self, model_name):
+        parts = os.path.splitext(model_name.lower())
+        if parts[-1] in [".pth"]:
+            return True
+        return False
+
+    @override
     def modelToRam(
         self,
         model_name: str,
         **kwargs,
     ) -> dict[str, typing.Any]:
         model_path = self.getFullModelPath(model_name)
         sd = comfy_horde.load_torch_file(model_path)
```

### Comparing `hordelib-0.9.5/hordelib/model_manager/hyper.py` & `hordelib-1.0.0/hordelib/model_manager/hyper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """Home for the controller class ModelManager, and related meta information."""
+import copy
+import threading
+
 import torch
 from loguru import logger
 
-from hordelib.consts import MODEL_CATEGORY_NAMES
+from hordelib.consts import EXCLUDED_MODEL_NAMES, MODEL_CATEGORY_NAMES
 
 # from hordelib.model_manager.aitemplate import AITemplateModelManager
 from hordelib.model_manager.base import BaseModelManager
 from hordelib.model_manager.blip import BlipModelManager
 from hordelib.model_manager.clip import ClipModelManager
 from hordelib.model_manager.codeformer import CodeFormerModelManager
 from hordelib.model_manager.compvis import CompVisModelManager
 from hordelib.model_manager.controlnet import ControlNetModelManager
 from hordelib.model_manager.diffusers import DiffusersModelManager
 from hordelib.model_manager.esrgan import EsrganModelManager
 from hordelib.model_manager.gfpgan import GfpganModelManager
 from hordelib.model_manager.safety_checker import SafetyCheckerModelManager
 
-# from worker.util.voodoo import initialise_voodoo
-
-
 MODEL_MANAGERS_TYPE_LOOKUP: dict[MODEL_CATEGORY_NAMES, type[BaseModelManager]] = {
     # ModelCategoryNames.aitemplate: AITemplateModelManager,
     MODEL_CATEGORY_NAMES.blip: BlipModelManager,
     MODEL_CATEGORY_NAMES.clip: ClipModelManager,
     MODEL_CATEGORY_NAMES.codeformer: CodeFormerModelManager,
     MODEL_CATEGORY_NAMES.compvis: CompVisModelManager,
     MODEL_CATEGORY_NAMES.controlnet: ControlNetModelManager,
@@ -98,18 +98,27 @@
 
         return _active_model_managers
 
     def __init__(
         self,
     ):
         """Create a new instance of model manager."""
-        # logger.initialise_voodoo()
         self.cuda_available = torch.cuda.is_available()
         """DEPRECATED: Use `torch.cuda.is_available()` instead."""
 
+        # We use this to serialise disk reads as no point in
+        # doing more than one at a time as this will slow down the sequential read op.
+        self.disk_read_mutex = threading.Lock()
+
+    def get_model_copy(self, model_name, model_component=None):
+        if not model_component:
+            return copy.deepcopy(self.loaded_models[model_name])
+        else:
+            return copy.deepcopy(self.loaded_models[model_name][model_component])
+
     def init_model_managers(
         self,
         # aitemplate: bool = False, # XXX
         blip: bool = False,
         clip: bool = False,
         codeformer: bool = False,
         compvis: bool = False,
@@ -234,17 +243,33 @@
         Returns:
             bool | None: The result of the unloading. If `None`, the model was not found.
         """
         for model_manager_type in MODEL_MANAGERS_TYPE_LOOKUP:
             model_manager: BaseModelManager = getattr(self, model_manager_type)
             if model_manager is None:
                 continue
-            if model_name not in model_manager.model_reference:
+            if model_name in model_manager.model_reference or model_manager.is_local_model(model_name):
+                return model_manager.unload_model(model_name)
+        return None
+
+    def move_from_disk_cache(self, model_name, model, clip, vae):
+        """Moves the given model back into ram.
+
+        Args:
+            model_name (str): The model name to remove.
+            model (model): the model data
+            clip (clip): the clip model data
+            var (var): the var model data
+        """
+        for model_manager_type in MODEL_MANAGERS_TYPE_LOOKUP:
+            model_manager: BaseModelManager = getattr(self, model_manager_type)
+            if model_manager is None:
                 continue
-            return model_manager.unload_model(model_name)
+            if model_name in model_manager.model_reference or model_manager.is_local_model(model_name):
+                return model_manager.move_from_disk_cache(model_name, model, clip, vae)
         return None
 
     def get_loaded_models_names(self) -> list:
         """DEPRECATED: Use property self.loaded_models. Returns a list of all the currently loaded models.
 
         Returns:
             list: All currently loaded models.
@@ -295,48 +320,54 @@
         """Asserts minimum amount of RAM is available. Unloads models if necessary."""
         for model_manager_type in MODEL_MANAGERS_TYPE_LOOKUP:
             if specific_type and specific_type != model_manager_type:
                 continue
             model_manager: BaseModelManager = getattr(self, model_manager_type)
             if model_manager is None:
                 continue
-            model_manager.ensure_memory_available()
+            model_manager.ensure_ram_available()
         return
 
     def load(
         self,
         model_name: str,
         half_precision: bool = True,
         gpu_id: int = 0,
         cpu_only: bool = False,
-        voodoo: bool = False,
+        local: bool = False,
     ) -> bool | None:
         """_summary_
 
         Args:
             model_name (str): Name of the model to load. See available_models for
             a list of available models.
             half_precision (bool, optional): If the model should be loaded in half precision.
             Defaults to True.
             gpu_id (int, optional): The id of the gpu to use. Defaults to 0.
             cpu_only (bool, optional): If should be loaded on the cpu.
             If True, half_precision will be set to False. Defaults to False.
-            voodoo (bool, optional): (compvis only) Voodoo ray. Defaults to False.
+            local (bool): model_name is a local filesystem filename of a model to load
 
         Returns:
             bool | None: The success of the load. If `None`, the model was not found.
         """
+        if model_name in EXCLUDED_MODEL_NAMES:
+            logger.init_warn(
+                f"{model_name} is excluded from loading at this time. If this is unexpected, let us know on discord.",
+                status="Skipping",
+            )
+            return False
+
         if not self.cuda_available:
             cpu_only = True
 
         for model_manager in self.active_model_managers:
-            if model_name in model_manager.model_reference:
+            if model_name in model_manager.model_reference or model_manager.is_local_model(model_name):
                 return model_manager.load(
                     model_name=model_name,
                     half_precision=half_precision,
                     gpu_id=gpu_id,
                     cpu_only=cpu_only,
-                    voodoo=voodoo,
                 )
 
         logger.error(f"{model_name} not found")
         return None
```

### Comparing `hordelib-0.9.5/hordelib/model_manager/safety_checker.py` & `hordelib-1.0.0/hordelib/model_manager/safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/README.md` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/README.md`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 from . import canny, hed, midas, mlsd, openpose, uniformer, leres, mp_pose_hand, color, binary, pidinet, mp_face_mesh
 from .util import HWC3, resize_image
 import torch
 import numpy as np
 import cv2
+import threading
 
 def img_np_to_tensor(img_np_list):
     out_list = []
     for img_np in img_np_list:
         out_list.append(torch.from_numpy(img_np.astype(np.float32) / 255.0))
     return torch.stack(out_list)
 def img_tensor_to_np(img_tensor):
     img_tensor = img_tensor.clone()
     img_tensor = img_tensor * 255.0
     mask_list = [x.squeeze().numpy().astype(np.uint8) for x in torch.split(img_tensor, 1)]
     return mask_list
     #Thanks ChatGPT
 
+_mutex = threading.Lock()
+
 def common_annotator_call(annotator_callback, tensor_image, *args):
-    tensor_image_list = img_tensor_to_np(tensor_image)
-    out_list = []
-    out_info_list = []
-    for tensor_image in tensor_image_list:
-        call_result = annotator_callback(resize_image(HWC3(tensor_image)), *args)
-        H, W, C = tensor_image.shape
+    with _mutex:
+        tensor_image_list = img_tensor_to_np(tensor_image)
+        out_list = []
+        out_info_list = []
+        for tensor_image in tensor_image_list:
+            call_result = annotator_callback(resize_image(HWC3(tensor_image)), *args)
+            H, W, C = tensor_image.shape
+            if type(annotator_callback) is openpose.OpenposeDetector:
+                out_list.append(cv2.resize(HWC3(call_result[0]), (W, H), interpolation=cv2.INTER_AREA))
+                out_info_list.append(call_result[1])
+            elif type(annotator_callback) is midas.MidasDetector:
+                out_list.append(cv2.resize(HWC3(call_result[0]), (W, H), interpolation=cv2.INTER_AREA))
+                out_info_list.append(cv2.resize(HWC3(call_result[1]), (W, H), interpolation=cv2.INTER_AREA))
+            else:
+                out_list.append(cv2.resize(HWC3(call_result), (W, H), interpolation=cv2.INTER_AREA))
         if type(annotator_callback) is openpose.OpenposeDetector:
-            out_list.append(cv2.resize(HWC3(call_result[0]), (W, H), interpolation=cv2.INTER_AREA))
-            out_info_list.append(call_result[1])
+            return (out_list, out_info_list)
         elif type(annotator_callback) is midas.MidasDetector:
-            out_list.append(cv2.resize(HWC3(call_result[0]), (W, H), interpolation=cv2.INTER_AREA))
-            out_info_list.append(cv2.resize(HWC3(call_result[1]), (W, H), interpolation=cv2.INTER_AREA))
+            return (out_list, out_info_list)
         else:
-            out_list.append(cv2.resize(HWC3(call_result), (W, H), interpolation=cv2.INTER_AREA))
-    if type(annotator_callback) is openpose.OpenposeDetector:
-        return (out_list, out_info_list)
-    elif type(annotator_callback) is midas.MidasDetector:
-        return (out_list, out_info_list)
-    else:
-        return out_list
+            return out_list
 
 
 class Canny_Edge_Preprocessor:
     @classmethod
     def INPUT_TYPES(s):
         return {"required": { "image": ("IMAGE", ) ,
                               "low_threshold": ("INT", {"default": 100, "min": 0, "max": 255, "step": 1}),
```

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,119 +1,136 @@
 import numpy as np
 import cv2
 import os
 import torch
 from einops import rearrange
-from comfy_controlnet_preprocessors.util import annotator_ckpts_path
+
+import builtins
 import model_management
 
 
 class Network(torch.nn.Module):
     def __init__(self, model_path):
         super().__init__()
 
         self.netVggOne = torch.nn.Sequential(
             torch.nn.Conv2d(in_channels=3, out_channels=64, kernel_size=3, stride=1, padding=1),
             torch.nn.ReLU(inplace=False),
             torch.nn.Conv2d(in_channels=64, out_channels=64, kernel_size=3, stride=1, padding=1),
-            torch.nn.ReLU(inplace=False)
+            torch.nn.ReLU(inplace=False),
         )
 
         self.netVggTwo = torch.nn.Sequential(
             torch.nn.MaxPool2d(kernel_size=2, stride=2),
             torch.nn.Conv2d(in_channels=64, out_channels=128, kernel_size=3, stride=1, padding=1),
             torch.nn.ReLU(inplace=False),
             torch.nn.Conv2d(in_channels=128, out_channels=128, kernel_size=3, stride=1, padding=1),
-            torch.nn.ReLU(inplace=False)
+            torch.nn.ReLU(inplace=False),
         )
 
         self.netVggThr = torch.nn.Sequential(
             torch.nn.MaxPool2d(kernel_size=2, stride=2),
             torch.nn.Conv2d(in_channels=128, out_channels=256, kernel_size=3, stride=1, padding=1),
             torch.nn.ReLU(inplace=False),
             torch.nn.Conv2d(in_channels=256, out_channels=256, kernel_size=3, stride=1, padding=1),
             torch.nn.ReLU(inplace=False),
             torch.nn.Conv2d(in_channels=256, out_channels=256, kernel_size=3, stride=1, padding=1),
-            torch.nn.ReLU(inplace=False)
+            torch.nn.ReLU(inplace=False),
         )
 
         self.netVggFou = torch.nn.Sequential(
             torch.nn.MaxPool2d(kernel_size=2, stride=2),
             torch.nn.Conv2d(in_channels=256, out_channels=512, kernel_size=3, stride=1, padding=1),
             torch.nn.ReLU(inplace=False),
             torch.nn.Conv2d(in_channels=512, out_channels=512, kernel_size=3, stride=1, padding=1),
             torch.nn.ReLU(inplace=False),
             torch.nn.Conv2d(in_channels=512, out_channels=512, kernel_size=3, stride=1, padding=1),
-            torch.nn.ReLU(inplace=False)
+            torch.nn.ReLU(inplace=False),
         )
 
         self.netVggFiv = torch.nn.Sequential(
             torch.nn.MaxPool2d(kernel_size=2, stride=2),
             torch.nn.Conv2d(in_channels=512, out_channels=512, kernel_size=3, stride=1, padding=1),
             torch.nn.ReLU(inplace=False),
             torch.nn.Conv2d(in_channels=512, out_channels=512, kernel_size=3, stride=1, padding=1),
             torch.nn.ReLU(inplace=False),
             torch.nn.Conv2d(in_channels=512, out_channels=512, kernel_size=3, stride=1, padding=1),
-            torch.nn.ReLU(inplace=False)
+            torch.nn.ReLU(inplace=False),
         )
 
         self.netScoreOne = torch.nn.Conv2d(in_channels=64, out_channels=1, kernel_size=1, stride=1, padding=0)
         self.netScoreTwo = torch.nn.Conv2d(in_channels=128, out_channels=1, kernel_size=1, stride=1, padding=0)
         self.netScoreThr = torch.nn.Conv2d(in_channels=256, out_channels=1, kernel_size=1, stride=1, padding=0)
         self.netScoreFou = torch.nn.Conv2d(in_channels=512, out_channels=1, kernel_size=1, stride=1, padding=0)
         self.netScoreFiv = torch.nn.Conv2d(in_channels=512, out_channels=1, kernel_size=1, stride=1, padding=0)
 
         self.netCombine = torch.nn.Sequential(
-            torch.nn.Conv2d(in_channels=5, out_channels=1, kernel_size=1, stride=1, padding=0),
-            torch.nn.Sigmoid()
+            torch.nn.Conv2d(in_channels=5, out_channels=1, kernel_size=1, stride=1, padding=0), torch.nn.Sigmoid()
         )
 
-        self.load_state_dict({strKey.replace('module', 'net'): tenWeight for strKey, tenWeight in torch.load(model_path).items()})
+        self.load_state_dict(
+            {strKey.replace("module", "net"): tenWeight for strKey, tenWeight in torch.load(model_path).items()}
+        )
 
     def forward(self, tenInput):
         tenInput = tenInput * 255.0
-        tenInput = tenInput - torch.tensor(data=[104.00698793, 116.66876762, 122.67891434], dtype=tenInput.dtype, device=tenInput.device).view(1, 3, 1, 1)
+        tenInput = tenInput - torch.tensor(
+            data=[104.00698793, 116.66876762, 122.67891434], dtype=tenInput.dtype, device=tenInput.device
+        ).view(1, 3, 1, 1)
 
         tenVggOne = self.netVggOne(tenInput)
         tenVggTwo = self.netVggTwo(tenVggOne)
         tenVggThr = self.netVggThr(tenVggTwo)
         tenVggFou = self.netVggFou(tenVggThr)
         tenVggFiv = self.netVggFiv(tenVggFou)
 
         tenScoreOne = self.netScoreOne(tenVggOne)
         tenScoreTwo = self.netScoreTwo(tenVggTwo)
         tenScoreThr = self.netScoreThr(tenVggThr)
         tenScoreFou = self.netScoreFou(tenVggFou)
         tenScoreFiv = self.netScoreFiv(tenVggFiv)
 
-        tenScoreOne = torch.nn.functional.interpolate(input=tenScoreOne, size=(tenInput.shape[2], tenInput.shape[3]), mode='bilinear', align_corners=False)
-        tenScoreTwo = torch.nn.functional.interpolate(input=tenScoreTwo, size=(tenInput.shape[2], tenInput.shape[3]), mode='bilinear', align_corners=False)
-        tenScoreThr = torch.nn.functional.interpolate(input=tenScoreThr, size=(tenInput.shape[2], tenInput.shape[3]), mode='bilinear', align_corners=False)
-        tenScoreFou = torch.nn.functional.interpolate(input=tenScoreFou, size=(tenInput.shape[2], tenInput.shape[3]), mode='bilinear', align_corners=False)
-        tenScoreFiv = torch.nn.functional.interpolate(input=tenScoreFiv, size=(tenInput.shape[2], tenInput.shape[3]), mode='bilinear', align_corners=False)
+        tenScoreOne = torch.nn.functional.interpolate(
+            input=tenScoreOne, size=(tenInput.shape[2], tenInput.shape[3]), mode="bilinear", align_corners=False
+        )
+        tenScoreTwo = torch.nn.functional.interpolate(
+            input=tenScoreTwo, size=(tenInput.shape[2], tenInput.shape[3]), mode="bilinear", align_corners=False
+        )
+        tenScoreThr = torch.nn.functional.interpolate(
+            input=tenScoreThr, size=(tenInput.shape[2], tenInput.shape[3]), mode="bilinear", align_corners=False
+        )
+        tenScoreFou = torch.nn.functional.interpolate(
+            input=tenScoreFou, size=(tenInput.shape[2], tenInput.shape[3]), mode="bilinear", align_corners=False
+        )
+        tenScoreFiv = torch.nn.functional.interpolate(
+            input=tenScoreFiv, size=(tenInput.shape[2], tenInput.shape[3]), mode="bilinear", align_corners=False
+        )
 
-        return self.netCombine(torch.cat([ tenScoreOne, tenScoreTwo, tenScoreThr, tenScoreFou, tenScoreFiv ], 1))
+        return self.netCombine(torch.cat([tenScoreOne, tenScoreTwo, tenScoreThr, tenScoreFou, tenScoreFiv], 1))
 
 
 class HEDdetector:
     def __init__(self):
-        remote_model_path = "https://huggingface.co/lllyasviel/ControlNet/resolve/main/annotator/ckpts/network-bsds500.pth"
-        modelpath = os.path.join(annotator_ckpts_path, "network-bsds500.pth")
+        remote_model_path = (
+            "https://huggingface.co/lllyasviel/ControlNet/resolve/main/annotator/ckpts/network-bsds500.pth"
+        )
+        modelpath = os.path.join(builtins.annotator_ckpts_path, "network-bsds500.pth")
         if not os.path.exists(modelpath):
             from comfy_controlnet_preprocessors.util import load_file_from_url
-            load_file_from_url(remote_model_path, model_dir=annotator_ckpts_path)
+
+            load_file_from_url(remote_model_path, model_dir=builtins.annotator_ckpts_path)
         self.netNetwork = Network(modelpath).to(model_management.get_torch_device()).eval()
 
     def __call__(self, input_image):
         assert input_image.ndim == 3
         input_image = input_image[:, :, ::-1].copy()
         with torch.no_grad():
             image_hed = torch.from_numpy(input_image).float().to(model_management.get_torch_device())
             image_hed = image_hed / 255.0
-            image_hed = rearrange(image_hed, 'h w c -> 1 c h w')
+            image_hed = rearrange(image_hed, "h w c -> 1 c h w")
             edge = self.netNetwork(image_hed)[0]
             edge = (edge.cpu().numpy() * 255.0).clip(0, 255).astype(np.uint8)
             return edge[0]
 
 
 def nms(x, t, s):
     x = cv2.GaussianBlur(x.astype(np.float32), (0, 0), s)
```

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,107 +1,115 @@
 import cv2
 import numpy as np
 import torch
 import os
-#from modules import devices, shared
+
+# from modules import devices, shared
 from torchvision.transforms import transforms
 
 # AdelaiDepth/LeReS imports
 from .leres.depthmap import estimateleres, estimateboost
 from .leres.multi_depth_model_woauxi import RelDepthModel
 from .leres.net_tools import strip_prefix_if_present
 
 # pix2pix/merge net imports
-#from .pix2pix.options.test_options import TestOptions
-#from .pix2pix.models.pix2pix4depth_model import Pix2Pix4DepthModel
+# from .pix2pix.options.test_options import TestOptions
+# from .pix2pix.models.pix2pix4depth_model import Pix2Pix4DepthModel
+
+import builtins
 
-from comfy_controlnet_preprocessors.util import annotator_ckpts_path
-base_model_path = annotator_ckpts_path
 old_modeldir = os.path.dirname(os.path.realpath(__file__))
 import model_management
 
-remote_model_path_leres = "https://cloudstor.aarnet.edu.au/plus/s/lTIJF4vrvHCAI31/download"
+# remote_model_path_leres = "https://cloudstor.aarnet.edu.au/plus/s/lTIJF4vrvHCAI31/download"
+remote_model_path_leres = (
+    "https://huggingface.co/lllyasviel/Annotators/resolve/1e70a29f5d06c27d37988d2c6c43f6fd21fdb2d1/res101.pth"
+)
 remote_model_path_pix2pix = "https://sfu.ca/~yagiz/CVPR21/latest_net_G.pth"
 
 model = None
 pix2pixmodel = None
 
+
 def unload_leres_model():
     global model, pix2pixmodel
     if model is not None:
         model = model.cpu()
     if pix2pixmodel is not None:
-        pix2pixmodel = pix2pixmodel.unload_network('G')
+        pix2pixmodel = pix2pixmodel.unload_network("G")
+
 
 def download_model_if_not_existed():
-    model_path = os.path.join(base_model_path, "res101.pth")
-    #old_model_path = os.path.join(old_modeldir, "res101.pth")
-    
-    #if os.path.exists(old_model_path):
+    model_path = os.path.join(builtins.annotator_ckpts_path, "res101.pth")
+    # old_model_path = os.path.join(old_modeldir, "res101.pth")
+
+    # if os.path.exists(old_model_path):
     #    model_path = old_model_path
     if not os.path.exists(model_path):
         from comfy_controlnet_preprocessors.util import load_file_from_url
-        load_file_from_url(remote_model_path_leres, model_dir=base_model_path)
-        os.rename(os.path.join(base_model_path, 'download'), model_path)
+
+        load_file_from_url(remote_model_path_leres, model_dir=builtins.annotator_ckpts_path)
+        os.rename(os.path.join(builtins.annotator_ckpts_path, "res101.pth"), model_path)
     return model_path
 
+
 def apply_leres(input_image, thr_a, thr_b):
     global model, pix2pixmodel
-    #boost = shared.opts.data.get("control_net_monocular_depth_optim", False)
-    boost = False #Too lazy to implement this to ComfyUI
+    # boost = shared.opts.data.get("control_net_monocular_depth_optim", False)
+    boost = False  # Too lazy to implement this to ComfyUI
     if model is None:
         model_path = download_model_if_not_existed()
         checkpoint = torch.load(model_path, map_location=torch.device(model_management.get_torch_device()))
-        model = RelDepthModel(backbone='resnext101').to(model_management.get_torch_device())
-        model.load_state_dict(strip_prefix_if_present(checkpoint['depth_model'], "module."), strict=True)
+        model = RelDepthModel(backbone="resnext101").to(model_management.get_torch_device())
+        model.load_state_dict(strip_prefix_if_present(checkpoint["depth_model"], "module."), strict=True)
         del checkpoint
 
     """ if boost and pix2pixmodel is None:
-        pix2pixmodel_path = os.path.join(base_model_path, "latest_net_G.pth")
+        pix2pixmodel_path = os.path.join(builtins.annotator_ckpts_path, "latest_net_G.pth")
         if not os.path.exists(pix2pixmodel_path):
             from comfy_controlnet_preprocessors.util import load_file_from_url
-            load_file_from_url(remote_model_path_pix2pix, model_dir=base_model_path)
+            load_file_from_url(remote_model_path_pix2pix, model_dir=builtins.annotator_ckpts_path)
 
         opt = TestOptions().parse()
         if not torch.cuda.is_available():
             opt.gpu_ids = [] # cpu mode
         pix2pixmodel = Pix2Pix4DepthModel(opt)
-        pix2pixmodel.save_dir = base_model_path
+        pix2pixmodel.save_dir = builtins.annotator_ckpts_path
         pix2pixmodel.load_networks('latest')
         pix2pixmodel.eval() """
-    
-    #if devices.get_device_for("controlnet").type != 'mps':
-        #model = model.to(devices.get_device_for("controlnet"))
+
+    # if devices.get_device_for("controlnet").type != 'mps':
+    # model = model.to(devices.get_device_for("controlnet"))
 
     assert input_image.ndim == 3
     height, width, dim = input_image.shape
 
     with torch.no_grad():
 
         if boost:
             depth = estimateboost(input_image, model, 0, pix2pixmodel, max(width, height))
         else:
             depth = estimateleres(input_image, model, width, height)
 
-        numbytes=2
+        numbytes = 2
         depth_min = depth.min()
         depth_max = depth.max()
-        max_val = (2**(8*numbytes))-1
+        max_val = (2 ** (8 * numbytes)) - 1
 
         # check output before normalizing and mapping to 16 bit
         if depth_max - depth_min > np.finfo("float").eps:
             out = max_val * (depth - depth_min) / (depth_max - depth_min)
         else:
             out = np.zeros(depth.shape)
-        
+
         # single channel, 16 bit image
         depth_image = out.astype("uint16")
 
         # convert to uint8
-        depth_image = cv2.convertScaleAbs(depth_image, alpha=(255.0/65535.0))
+        depth_image = cv2.convertScaleAbs(depth_image, alpha=(255.0 / 65535.0))
 
         # remove near
         if thr_a != 0:
             thr_a = thr_a * 255
             depth_image = cv2.threshold(depth_image, thr_a, 255, cv2.THRESH_TOZERO)[1]
 
         # invert image
```

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 import torch.nn as nn
 from torchvision.transforms import Compose
 
 from .midas.dpt_depth import DPTDepthModel
 from .midas.midas_net import MidasNet
 from .midas.midas_net_custom import MidasNet_small
 from .midas.transforms import Resize, NormalizeImage, PrepareForNet
-from comfy_controlnet_preprocessors.util import annotator_ckpts_path
+import builtins
 
 
 ISL_PATHS = {
-    "dpt_large": os.path.join(annotator_ckpts_path, "dpt_large-midas-2f21e586.pt"),
-    "dpt_hybrid": os.path.join(annotator_ckpts_path, "dpt_hybrid-midas-501f0c75.pt"),
+    "dpt_large": "dpt_large-midas-2f21e586.pt",
+    "dpt_hybrid": "dpt_hybrid-midas-501f0c75.pt",
     "midas_v21": "",
     "midas_v21_small": "",
 }
 
-remote_model_path = "https://huggingface.co/lllyasviel/ControlNet/resolve/main/annotator/ckpts/dpt_hybrid-midas-501f0c75.pt"
+remote_model_path = (
+    "https://huggingface.co/lllyasviel/ControlNet/resolve/main/annotator/ckpts/dpt_hybrid-midas-501f0c75.pt"
+)
 
 
 def disabled_train(self, mode=True):
     """Overwrite model.train with this function to make sure train/eval mode
     does not change anymore."""
     return self
 
@@ -73,55 +75,58 @@
 
     return transform
 
 
 def load_model(model_type):
     # https://github.com/isl-org/MiDaS/blob/master/run.py
     # load network
-    model_path = ISL_PATHS[model_type]
+    model_path = os.path.join(builtins.annotator_ckpts_path, ISL_PATHS[model_type])
     if model_type == "dpt_large":  # DPT-Large
         model = DPTDepthModel(
             path=model_path,
             backbone="vitl16_384",
             non_negative=True,
         )
         net_w, net_h = 384, 384
         resize_mode = "minimal"
         normalization = NormalizeImage(mean=[0.5, 0.5, 0.5], std=[0.5, 0.5, 0.5])
 
     elif model_type == "dpt_hybrid":  # DPT-Hybrid
         if not os.path.exists(model_path):
             from comfy_controlnet_preprocessors.util import load_file_from_url
-            load_file_from_url(remote_model_path, model_dir=annotator_ckpts_path)
+
+            load_file_from_url(remote_model_path, model_dir=builtins.annotator_ckpts_path)
 
         model = DPTDepthModel(
             path=model_path,
             backbone="vitb_rn50_384",
             non_negative=True,
         )
         net_w, net_h = 384, 384
         resize_mode = "minimal"
         normalization = NormalizeImage(mean=[0.5, 0.5, 0.5], std=[0.5, 0.5, 0.5])
 
     elif model_type == "midas_v21":
         model = MidasNet(model_path, non_negative=True)
         net_w, net_h = 384, 384
         resize_mode = "upper_bound"
-        normalization = NormalizeImage(
-            mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225]
-        )
+        normalization = NormalizeImage(mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225])
 
     elif model_type == "midas_v21_small":
-        model = MidasNet_small(model_path, features=64, backbone="efficientnet_lite3", exportable=True,
-                               non_negative=True, blocks={'expand': True})
+        model = MidasNet_small(
+            model_path,
+            features=64,
+            backbone="efficientnet_lite3",
+            exportable=True,
+            non_negative=True,
+            blocks={"expand": True},
+        )
         net_w, net_h = 256, 256
         resize_mode = "upper_bound"
-        normalization = NormalizeImage(
-            mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225]
-        )
+        normalization = NormalizeImage(mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225])
 
     else:
         print(f"model_type '{model_type}' not implemented, use: --model_type large")
         assert False
 
     transform = Compose(
         [
@@ -139,31 +144,26 @@
         ]
     )
 
     return model.eval(), transform
 
 
 class MiDaSInference(nn.Module):
-    MODEL_TYPES_TORCH_HUB = [
-        "DPT_Large",
-        "DPT_Hybrid",
-        "MiDaS_small"
-    ]
+    MODEL_TYPES_TORCH_HUB = ["DPT_Large", "DPT_Hybrid", "MiDaS_small"]
     MODEL_TYPES_ISL = [
         "dpt_large",
         "dpt_hybrid",
         "midas_v21",
         "midas_v21_small",
     ]
 
     def __init__(self, model_type):
         super().__init__()
-        assert (model_type in self.MODEL_TYPES_ISL)
+        assert model_type in self.MODEL_TYPES_ISL
         model, _ = load_model(model_type)
         self.model = model
         self.model.train = disabled_train
 
     def forward(self, x):
         with torch.no_grad():
             prediction = self.model(x)
         return prediction
-
```

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 import os
 
 from einops import rearrange
 from .models.mbv2_mlsd_tiny import MobileV2_MLSD_Tiny
 from .models.mbv2_mlsd_large import MobileV2_MLSD_Large
 from .utils import pred_lines
 
-from comfy_controlnet_preprocessors.util import annotator_ckpts_path
+import builtins
 import model_management
 
 
 remote_model_path = "https://huggingface.co/lllyasviel/ControlNet/resolve/main/annotator/ckpts/mlsd_large_512_fp32.pth"
 
 
 class MLSDdetector:
     def __init__(self):
-        model_path = os.path.join(annotator_ckpts_path, "mlsd_large_512_fp32.pth")
+        model_path = os.path.join(builtins.annotator_ckpts_path, "mlsd_large_512_fp32.pth")
         if not os.path.exists(model_path):
             from comfy_controlnet_preprocessors.util import load_file_from_url
-            load_file_from_url(remote_model_path, model_dir=annotator_ckpts_path)
+
+            load_file_from_url(remote_model_path, model_dir=builtins.annotator_ckpts_path)
         model = MobileV2_MLSD_Large()
         model.load_state_dict(torch.load(model_path), strict=True)
         self.model = model.to(model_management.get_torch_device()).eval()
 
     def __call__(self, input_image, thr_v, thr_d):
         assert input_image.ndim == 3
         img = input_image
```

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 import os
-os.environ["KMP_DUPLICATE_LIB_OK"]="TRUE"
+
+os.environ["KMP_DUPLICATE_LIB_OK"] = "TRUE"
 
 import torch
 import numpy as np
 from . import util
 from .body import Body
 from .hand import Hand
-from comfy_controlnet_preprocessors.util import annotator_ckpts_path
+import builtins
 
 
 body_model_path = "https://huggingface.co/lllyasviel/ControlNet/resolve/main/annotator/ckpts/body_pose_model.pth"
 hand_model_path = "https://huggingface.co/lllyasviel/ControlNet/resolve/main/annotator/ckpts/hand_pose_model.pth"
 
 
 class OpenposeDetector:
     def __init__(self):
-        body_modelpath = os.path.join(annotator_ckpts_path, "body_pose_model.pth")
-        hand_modelpath = os.path.join(annotator_ckpts_path, "hand_pose_model.pth")
+        body_modelpath = os.path.join(builtins.annotator_ckpts_path, "body_pose_model.pth")
+        hand_modelpath = os.path.join(builtins.annotator_ckpts_path, "hand_pose_model.pth")
 
         if not os.path.exists(hand_modelpath):
             from comfy_controlnet_preprocessors.util import load_file_from_url
-            load_file_from_url(body_model_path, model_dir=annotator_ckpts_path)
-            load_file_from_url(hand_model_path, model_dir=annotator_ckpts_path)
+
+            load_file_from_url(body_model_path, model_dir=builtins.annotator_ckpts_path)
+            load_file_from_url(hand_model_path, model_dir=builtins.annotator_ckpts_path)
 
         self.body_estimation = Body(body_modelpath)
         self.hand_estimation = Hand(hand_modelpath)
 
     def __call__(self, oriImg, hand=False):
         oriImg = oriImg[:, :, ::-1].copy()
         with torch.no_grad():
             candidate, subset = self.body_estimation(oriImg)
             canvas = np.zeros_like(oriImg)
             canvas = util.draw_bodypose(canvas, candidate, subset)
             if hand:
                 hands_list = util.handDetect(candidate, subset, oriImg)
                 all_hand_peaks = []
                 for x, y, w, is_left in hands_list:
-                    peaks = self.hand_estimation(oriImg[y:y+w, x:x+w, :])
+                    peaks = self.hand_estimation(oriImg[y : y + w, x : x + w, :])
                     peaks[:, 0] = np.where(peaks[:, 0] == 0, peaks[:, 0], peaks[:, 0] + x)
                     peaks[:, 1] = np.where(peaks[:, 1] == 0, peaks[:, 1], peaks[:, 1] + y)
                     all_hand_peaks.append(peaks)
                 canvas = util.draw_handpose(canvas, all_hand_peaks)
             return canvas, dict(candidate=candidate.tolist(), subset=subset.tolist())
```

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import cv2
 import numpy as np
 import math
 import time
 from scipy.ndimage.filters import gaussian_filter
-import matplotlib.pyplot as plt
-import matplotlib
 import torch
 from torchvision import transforms
 
 from . import util
 from .model import bodypose_model
 import model_management
 
@@ -203,17 +201,7 @@
             if subset[i][-1] < 4 or subset[i][-2] / subset[i][-1] < 0.4:
                 deleteIdx.append(i)
         subset = np.delete(subset, deleteIdx, axis=0)
 
         # subset: n*20 array, 0-17 is the index in candidate, 18 is the total score, 19 is the total parts
         # candidate: x, y, score, id
         return candidate, subset
-
-if __name__ == "__main__":
-    body_estimation = Body('../model/body_pose_model.pth')
-
-    test_image = '../images/ski.jpg'
-    oriImg = cv2.imread(test_image)  # B,G,R order
-    candidate, subset = body_estimation(oriImg)
-    canvas = util.draw_bodypose(oriImg, candidate, subset)
-    plt.imshow(canvas[:, :, [2, 1, 0]])
-    plt.show()
```

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import cv2
 import json
 import numpy as np
 import math
 import time
 from scipy.ndimage.filters import gaussian_filter
-import matplotlib.pyplot as plt
-import matplotlib
 import torch
 from skimage.measure import label
 import model_management
 
 from .model import handpose_model
 from . import util
 
@@ -67,18 +65,7 @@
             max_index = np.argmax([np.sum(map_ori[label_img == i]) for i in range(1, label_numbers + 1)]) + 1
             label_img[label_img != max_index] = 0
             map_ori[label_img == 0] = 0
 
             y, x = util.npmax(map_ori)
             all_peaks.append([x, y])
         return np.array(all_peaks)
-
-if __name__ == "__main__":
-    hand_estimation = Hand('../model/hand_pose_model.pth')
-
-    # test_image = '../images/hand.jpg'
-    test_image = '../images/hand.jpg'
-    oriImg = cv2.imread(test_image)  # B,G,R order
-    peaks = hand_estimation(oriImg)
-    canvas = util.draw_handpose(oriImg, peaks, True)
-    cv2.imshow('', canvas)
-    cv2.waitKey(0)
```

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 import numpy as np
-import matplotlib
 import cv2
+import colorsys
 
 
 def padRightDownCorner(img, stride, padValue):
     h = img.shape[0]
     w = img.shape[1]
 
     pad = 4 * [None]
@@ -76,15 +76,15 @@
              [10, 11], [11, 12], [0, 13], [13, 14], [14, 15], [15, 16], [0, 17], [17, 18], [18, 19], [19, 20]]
 
     for peaks in all_hand_peaks:
         for ie, e in enumerate(edges):
             if np.sum(np.all(peaks[e], axis=1)==0)==0:
                 x1, y1 = peaks[e[0]]
                 x2, y2 = peaks[e[1]]
-                cv2.line(canvas, (x1, y1), (x2, y2), matplotlib.colors.hsv_to_rgb([ie/float(len(edges)), 1.0, 1.0])*255, thickness=2)
+                cv2.line(canvas, (x1, y1), (x2, y2), colorsys.hsv_to_rgb([ie/float(len(edges)), 1.0, 1.0])*255, thickness=2)
 
         for i, keyponit in enumerate(peaks):
             x, y = keyponit
             cv2.circle(canvas, (x, y), 4, (0, 0, 255), thickness=-1)
             if show_number:
                 cv2.putText(canvas, str(i), (x, y), cv2.FONT_HERSHEY_SIMPLEX, 0.3, (0, 0, 0), lineType=cv2.LINE_AA)
     return canvas
```

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 import os
 import torch
 import numpy as np
 from einops import rearrange
 from .model import pidinet
-from comfy_controlnet_preprocessors.util import annotator_ckpts_path, load_state_dict, load_file_from_url
+from comfy_controlnet_preprocessors.util import load_state_dict, load_file_from_url
+import builtins
 import model_management
 
 netNetwork = None
 remote_model_path = "https://huggingface.co/TencentARC/T2I-Adapter/resolve/main/third-party-models/table5_pidinet.pth"
-modeldir = os.path.join(annotator_ckpts_path, "pidinet")
+modeldir = "pidinet"
+
 
 def download_if_not_existed():
-    modelpath = os.path.join(modeldir, "table5_pidinet.pth")
+    modelpath = os.path.join(builtins.annotator_ckpts_path, modeldir, "table5_pidinet.pth")
     if not os.path.exists(modelpath):
-        load_file_from_url(remote_model_path, model_dir=modeldir)
+        load_file_from_url(remote_model_path, model_dir=modelpath)
     return modelpath
 
+
 def apply_pidinet(input_image):
     global netNetwork
     if netNetwork is None:
         netNetwork = pidinet()
         ckp = load_state_dict(download_if_not_existed())
-        netNetwork.load_state_dict({k.replace('module.',''):v for k, v in ckp.items()})
-        
+        netNetwork.load_state_dict({k.replace("module.", ""): v for k, v in ckp.items()})
+
     netNetwork = netNetwork.to(model_management.get_torch_device())
     netNetwork.eval()
     assert input_image.ndim == 3
     input_image = input_image[:, :, ::-1].copy()
     with torch.no_grad():
         image_pidi = torch.from_numpy(input_image).float().to(model_management.get_torch_device())
         image_pidi = image_pidi / 255.0
-        image_pidi = rearrange(image_pidi, 'h w c -> 1 c h w')
+        image_pidi = rearrange(image_pidi, "h w c -> 1 c h w")
         edge = netNetwork(image_pidi)[-1]
-        edge = edge>0.5
+        edge = edge > 0.5
         edge = (edge * 255.0).clip(0, 255).cpu().numpy().astype(np.uint8)
-        
-    return edge[0][0] 
+
+    return edge[0][0]
```

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import os
 
 from comfy_controlnet_preprocessors.uniformer.mmseg.apis import init_segmentor, inference_segmentor, show_result_pyplot
 from comfy_controlnet_preprocessors.uniformer.mmseg.core.evaluation import get_palette
-from comfy_controlnet_preprocessors.util import annotator_ckpts_path
+import builtins
+
 import model_management
 
 
 checkpoint_file = "https://huggingface.co/lllyasviel/ControlNet/resolve/main/annotator/ckpts/upernet_global_small.pth"
 
 
 class UniformerDetector:
     def __init__(self):
-        modelpath = os.path.join(annotator_ckpts_path, "upernet_global_small.pth")
+        modelpath = os.path.join(builtins.annotator_ckpts_path, "upernet_global_small.pth")
         if not os.path.exists(modelpath):
             from comfy_controlnet_preprocessors.util import load_file_from_url
-            load_file_from_url(checkpoint_file, model_dir=annotator_ckpts_path)
+
+            load_file_from_url(checkpoint_file, model_dir=builtins.annotator_ckpts_path)
         config_file = os.path.join(os.path.dirname(__file__), "exp", "upernet_global_small", "config.py")
         self.model = init_segmentor(config_file, modelpath).to(model_management.get_torch_device())
 
     def __call__(self, img):
         result = inference_segmentor(self.model, img)
-        res_img = show_result_pyplot(self.model, img, result, get_palette('ade'), opacity=1)
+        res_img = show_result_pyplot(self.model, img, result, get_palette("ade"), opacity=1)
         return res_img
```

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (c) OpenMMLab. All rights reserved.
+import sys
 from ..runner import Sequential
 from ..utils import Registry, build_from_cfg
 
 
 def build_model_from_cfg(cfg, registry, default_args=None):
     """Build a PyTorch model from config dict(s). Different from
     ``build_from_cfg``, if cfg is a list, a ``nn.Sequential`` will be built.
@@ -15,16 +16,14 @@
         default_args (dict, optional): Default arguments to build the module.
             Defaults to None.
 
     Returns:
         nn.Module: A built nn module.
     """
     if isinstance(cfg, list):
-        modules = [
-            build_from_cfg(cfg_, registry, default_args) for cfg_ in cfg
-        ]
+        modules = [build_from_cfg(cfg_, registry, default_args) for cfg_ in cfg]
         return Sequential(*modules)
     else:
         return build_from_cfg(cfg, registry, default_args)
 
 
-MODELS = Registry('model', build_func=build_model_from_cfg)
+MODELS = Registry("model", sys.modules[__name__], build_func=build_model_from_cfg)
```

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,169 +1,155 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import copy
 import math
+import sys
 import warnings
 
 import numpy as np
 import torch
 import torch.nn as nn
 from torch import Tensor
 
 from comfy_controlnet_preprocessors.uniformer.mmcv.utils import Registry, build_from_cfg, get_logger, print_log
 
-INITIALIZERS = Registry('initializer')
+INITIALIZERS = Registry("initializer", sys.modules[__name__])
 
 
 def update_init_info(module, init_info):
     """Update the `_params_init_info` in the module if the value of parameters
     are changed.
 
     Args:
         module (obj:`nn.Module`): The module of PyTorch with a user-defined
             attribute `_params_init_info` which records the initialization
             information.
         init_info (str): The string that describes the initialization.
     """
-    assert hasattr(
-        module,
-        '_params_init_info'), f'Can not find `_params_init_info` in {module}'
+    assert hasattr(module, "_params_init_info"), f"Can not find `_params_init_info` in {module}"
     for name, param in module.named_parameters():
-
         assert param in module._params_init_info, (
-            f'Find a new :obj:`Parameter` '
-            f'named `{name}` during executing the '
-            f'`init_weights` of '
-            f'`{module.__class__.__name__}`. '
-            f'Please do not add or '
-            f'replace parameters during executing '
-            f'the `init_weights`. ')
+            f"Find a new :obj:`Parameter` "
+            f"named `{name}` during executing the "
+            f"`init_weights` of "
+            f"`{module.__class__.__name__}`. "
+            f"Please do not add or "
+            f"replace parameters during executing "
+            f"the `init_weights`. "
+        )
 
         # The parameter has been changed during executing the
         # `init_weights` of module
         mean_value = param.data.mean()
-        if module._params_init_info[param]['tmp_mean_value'] != mean_value:
-            module._params_init_info[param]['init_info'] = init_info
-            module._params_init_info[param]['tmp_mean_value'] = mean_value
+        if module._params_init_info[param]["tmp_mean_value"] != mean_value:
+            module._params_init_info[param]["init_info"] = init_info
+            module._params_init_info[param]["tmp_mean_value"] = mean_value
 
 
 def constant_init(module, val, bias=0):
-    if hasattr(module, 'weight') and module.weight is not None:
+    if hasattr(module, "weight") and module.weight is not None:
         nn.init.constant_(module.weight, val)
-    if hasattr(module, 'bias') and module.bias is not None:
+    if hasattr(module, "bias") and module.bias is not None:
         nn.init.constant_(module.bias, bias)
 
 
-def xavier_init(module, gain=1, bias=0, distribution='normal'):
-    assert distribution in ['uniform', 'normal']
-    if hasattr(module, 'weight') and module.weight is not None:
-        if distribution == 'uniform':
+def xavier_init(module, gain=1, bias=0, distribution="normal"):
+    assert distribution in ["uniform", "normal"]
+    if hasattr(module, "weight") and module.weight is not None:
+        if distribution == "uniform":
             nn.init.xavier_uniform_(module.weight, gain=gain)
         else:
             nn.init.xavier_normal_(module.weight, gain=gain)
-    if hasattr(module, 'bias') and module.bias is not None:
+    if hasattr(module, "bias") and module.bias is not None:
         nn.init.constant_(module.bias, bias)
 
 
 def normal_init(module, mean=0, std=1, bias=0):
-    if hasattr(module, 'weight') and module.weight is not None:
+    if hasattr(module, "weight") and module.weight is not None:
         nn.init.normal_(module.weight, mean, std)
-    if hasattr(module, 'bias') and module.bias is not None:
+    if hasattr(module, "bias") and module.bias is not None:
         nn.init.constant_(module.bias, bias)
 
 
-def trunc_normal_init(module: nn.Module,
-                      mean: float = 0,
-                      std: float = 1,
-                      a: float = -2,
-                      b: float = 2,
-                      bias: float = 0) -> None:
-    if hasattr(module, 'weight') and module.weight is not None:
+def trunc_normal_init(
+    module: nn.Module, mean: float = 0, std: float = 1, a: float = -2, b: float = 2, bias: float = 0
+) -> None:
+    if hasattr(module, "weight") and module.weight is not None:
         trunc_normal_(module.weight, mean, std, a, b)  # type: ignore
-    if hasattr(module, 'bias') and module.bias is not None:
+    if hasattr(module, "bias") and module.bias is not None:
         nn.init.constant_(module.bias, bias)  # type: ignore
 
 
 def uniform_init(module, a=0, b=1, bias=0):
-    if hasattr(module, 'weight') and module.weight is not None:
+    if hasattr(module, "weight") and module.weight is not None:
         nn.init.uniform_(module.weight, a, b)
-    if hasattr(module, 'bias') and module.bias is not None:
+    if hasattr(module, "bias") and module.bias is not None:
         nn.init.constant_(module.bias, bias)
 
 
-def kaiming_init(module,
-                 a=0,
-                 mode='fan_out',
-                 nonlinearity='relu',
-                 bias=0,
-                 distribution='normal'):
-    assert distribution in ['uniform', 'normal']
-    if hasattr(module, 'weight') and module.weight is not None:
-        if distribution == 'uniform':
-            nn.init.kaiming_uniform_(
-                module.weight, a=a, mode=mode, nonlinearity=nonlinearity)
+def kaiming_init(module, a=0, mode="fan_out", nonlinearity="relu", bias=0, distribution="normal"):
+    assert distribution in ["uniform", "normal"]
+    if hasattr(module, "weight") and module.weight is not None:
+        if distribution == "uniform":
+            nn.init.kaiming_uniform_(module.weight, a=a, mode=mode, nonlinearity=nonlinearity)
         else:
-            nn.init.kaiming_normal_(
-                module.weight, a=a, mode=mode, nonlinearity=nonlinearity)
-    if hasattr(module, 'bias') and module.bias is not None:
+            nn.init.kaiming_normal_(module.weight, a=a, mode=mode, nonlinearity=nonlinearity)
+    if hasattr(module, "bias") and module.bias is not None:
         nn.init.constant_(module.bias, bias)
 
 
 def caffe2_xavier_init(module, bias=0):
     # `XavierFill` in Caffe2 corresponds to `kaiming_uniform_` in PyTorch
     # Acknowledgment to FAIR's internal code
-    kaiming_init(
-        module,
-        a=1,
-        mode='fan_in',
-        nonlinearity='leaky_relu',
-        bias=bias,
-        distribution='uniform')
+    kaiming_init(module, a=1, mode="fan_in", nonlinearity="leaky_relu", bias=bias, distribution="uniform")
 
 
 def bias_init_with_prob(prior_prob):
     """initialize conv/fc bias value according to a given probability value."""
     bias_init = float(-np.log((1 - prior_prob) / prior_prob))
     return bias_init
 
 
 def _get_bases_name(m):
     return [b.__name__ for b in m.__class__.__bases__]
 
 
 class BaseInit(object):
-
     def __init__(self, *, bias=0, bias_prob=None, layer=None):
         self.wholemodule = False
         if not isinstance(bias, (int, float)):
-            raise TypeError(f'bias must be a number, but got a {type(bias)}')
+            raise TypeError(f"bias must be a number, but got a {type(bias)}")
 
         if bias_prob is not None:
             if not isinstance(bias_prob, float):
-                raise TypeError(f'bias_prob type must be float, \
-                    but got {type(bias_prob)}')
+                raise TypeError(
+                    f"bias_prob type must be float, \
+                    but got {type(bias_prob)}"
+                )
 
         if layer is not None:
             if not isinstance(layer, (str, list)):
-                raise TypeError(f'layer must be a str or a list of str, \
-                    but got a {type(layer)}')
+                raise TypeError(
+                    f"layer must be a str or a list of str, \
+                    but got a {type(layer)}"
+                )
         else:
             layer = []
 
         if bias_prob is not None:
             self.bias = bias_init_with_prob(bias_prob)
         else:
             self.bias = bias
         self.layer = [layer] if isinstance(layer, str) else layer
 
     def _get_init_info(self):
-        info = f'{self.__class__.__name__}, bias={self.bias}'
+        info = f"{self.__class__.__name__}, bias={self.bias}"
         return info
 
 
-@INITIALIZERS.register_module(name='Constant')
+@INITIALIZERS.register_module(name="Constant")
 class ConstantInit(BaseInit):
     """Initialize module parameters with constant values.
 
     Args:
         val (int | float): the value to fill the weights in the module with
         bias (int | float): the value to fill the bias. Defaults to 0.
         bias_prob (float, optional): the probability for bias initialization.
@@ -173,34 +159,33 @@
     """
 
     def __init__(self, val, **kwargs):
         super().__init__(**kwargs)
         self.val = val
 
     def __call__(self, module):
-
         def init(m):
             if self.wholemodule:
                 constant_init(m, self.val, self.bias)
             else:
                 layername = m.__class__.__name__
                 basesname = _get_bases_name(m)
                 if len(set(self.layer) & set([layername] + basesname)):
                     constant_init(m, self.val, self.bias)
 
         module.apply(init)
-        if hasattr(module, '_params_init_info'):
+        if hasattr(module, "_params_init_info"):
             update_init_info(module, init_info=self._get_init_info())
 
     def _get_init_info(self):
-        info = f'{self.__class__.__name__}: val={self.val}, bias={self.bias}'
+        info = f"{self.__class__.__name__}: val={self.val}, bias={self.bias}"
         return info
 
 
-@INITIALIZERS.register_module(name='Xavier')
+@INITIALIZERS.register_module(name="Xavier")
 class XavierInit(BaseInit):
     r"""Initialize module parameters with values according to the method
     described in `Understanding the difficulty of training deep feedforward
     neural networks - Glorot, X. & Bengio, Y. (2010).
     <http://proceedings.mlr.press/v9/glorot10a/glorot10a.pdf>`_
 
     Args:
@@ -210,41 +195,39 @@
             Defaults to None.
         distribution (str): distribution either be ``'normal'``
             or ``'uniform'``. Defaults to ``'normal'``.
         layer (str | list[str], optional): the layer will be initialized.
             Defaults to None.
     """
 
-    def __init__(self, gain=1, distribution='normal', **kwargs):
+    def __init__(self, gain=1, distribution="normal", **kwargs):
         super().__init__(**kwargs)
         self.gain = gain
         self.distribution = distribution
 
     def __call__(self, module):
-
         def init(m):
             if self.wholemodule:
                 xavier_init(m, self.gain, self.bias, self.distribution)
             else:
                 layername = m.__class__.__name__
                 basesname = _get_bases_name(m)
                 if len(set(self.layer) & set([layername] + basesname)):
                     xavier_init(m, self.gain, self.bias, self.distribution)
 
         module.apply(init)
-        if hasattr(module, '_params_init_info'):
+        if hasattr(module, "_params_init_info"):
             update_init_info(module, init_info=self._get_init_info())
 
     def _get_init_info(self):
-        info = f'{self.__class__.__name__}: gain={self.gain}, ' \
-               f'distribution={self.distribution}, bias={self.bias}'
+        info = f"{self.__class__.__name__}: gain={self.gain}, " f"distribution={self.distribution}, bias={self.bias}"
         return info
 
 
-@INITIALIZERS.register_module(name='Normal')
+@INITIALIZERS.register_module(name="Normal")
 class NormalInit(BaseInit):
     r"""Initialize module parameters with the values drawn from the normal
     distribution :math:`\mathcal{N}(\text{mean}, \text{std}^2)`.
 
     Args:
         mean (int | float):the mean of the normal distribution. Defaults to 0.
         std (int | float): the standard deviation of the normal distribution.
@@ -259,35 +242,33 @@
 
     def __init__(self, mean=0, std=1, **kwargs):
         super().__init__(**kwargs)
         self.mean = mean
         self.std = std
 
     def __call__(self, module):
-
         def init(m):
             if self.wholemodule:
                 normal_init(m, self.mean, self.std, self.bias)
             else:
                 layername = m.__class__.__name__
                 basesname = _get_bases_name(m)
                 if len(set(self.layer) & set([layername] + basesname)):
                     normal_init(m, self.mean, self.std, self.bias)
 
         module.apply(init)
-        if hasattr(module, '_params_init_info'):
+        if hasattr(module, "_params_init_info"):
             update_init_info(module, init_info=self._get_init_info())
 
     def _get_init_info(self):
-        info = f'{self.__class__.__name__}: mean={self.mean},' \
-               f' std={self.std}, bias={self.bias}'
+        info = f"{self.__class__.__name__}: mean={self.mean}," f" std={self.std}, bias={self.bias}"
         return info
 
 
-@INITIALIZERS.register_module(name='TruncNormal')
+@INITIALIZERS.register_module(name="TruncNormal")
 class TruncNormalInit(BaseInit):
     r"""Initialize module parameters with the values drawn from the normal
     distribution :math:`\mathcal{N}(\text{mean}, \text{std}^2)` with values
     outside :math:`[a, b]`.
 
     Args:
         mean (float): the mean of the normal distribution. Defaults to 0.
@@ -299,50 +280,44 @@
         bias_prob (float, optional): the probability for bias initialization.
             Defaults to None.
         layer (str | list[str], optional): the layer will be initialized.
             Defaults to None.
 
     """
 
-    def __init__(self,
-                 mean: float = 0,
-                 std: float = 1,
-                 a: float = -2,
-                 b: float = 2,
-                 **kwargs) -> None:
+    def __init__(self, mean: float = 0, std: float = 1, a: float = -2, b: float = 2, **kwargs) -> None:
         super().__init__(**kwargs)
         self.mean = mean
         self.std = std
         self.a = a
         self.b = b
 
     def __call__(self, module: nn.Module) -> None:
-
         def init(m):
             if self.wholemodule:
-                trunc_normal_init(m, self.mean, self.std, self.a, self.b,
-                                  self.bias)
+                trunc_normal_init(m, self.mean, self.std, self.a, self.b, self.bias)
             else:
                 layername = m.__class__.__name__
                 basesname = _get_bases_name(m)
                 if len(set(self.layer) & set([layername] + basesname)):
-                    trunc_normal_init(m, self.mean, self.std, self.a, self.b,
-                                      self.bias)
+                    trunc_normal_init(m, self.mean, self.std, self.a, self.b, self.bias)
 
         module.apply(init)
-        if hasattr(module, '_params_init_info'):
+        if hasattr(module, "_params_init_info"):
             update_init_info(module, init_info=self._get_init_info())
 
     def _get_init_info(self):
-        info = f'{self.__class__.__name__}: a={self.a}, b={self.b},' \
-               f' mean={self.mean}, std={self.std}, bias={self.bias}'
+        info = (
+            f"{self.__class__.__name__}: a={self.a}, b={self.b},"
+            f" mean={self.mean}, std={self.std}, bias={self.bias}"
+        )
         return info
 
 
-@INITIALIZERS.register_module(name='Uniform')
+@INITIALIZERS.register_module(name="Uniform")
 class UniformInit(BaseInit):
     r"""Initialize module parameters with values drawn from the uniform
     distribution :math:`\mathcal{U}(a, b)`.
 
     Args:
         a (int | float): the lower bound of the uniform distribution.
             Defaults to 0.
@@ -357,35 +332,33 @@
 
     def __init__(self, a=0, b=1, **kwargs):
         super().__init__(**kwargs)
         self.a = a
         self.b = b
 
     def __call__(self, module):
-
         def init(m):
             if self.wholemodule:
                 uniform_init(m, self.a, self.b, self.bias)
             else:
                 layername = m.__class__.__name__
                 basesname = _get_bases_name(m)
                 if len(set(self.layer) & set([layername] + basesname)):
                     uniform_init(m, self.a, self.b, self.bias)
 
         module.apply(init)
-        if hasattr(module, '_params_init_info'):
+        if hasattr(module, "_params_init_info"):
             update_init_info(module, init_info=self._get_init_info())
 
     def _get_init_info(self):
-        info = f'{self.__class__.__name__}: a={self.a},' \
-               f' b={self.b}, bias={self.bias}'
+        info = f"{self.__class__.__name__}: a={self.a}," f" b={self.b}, bias={self.bias}"
         return info
 
 
-@INITIALIZERS.register_module(name='Kaiming')
+@INITIALIZERS.register_module(name="Kaiming")
 class KaimingInit(BaseInit):
     r"""Initialize module parameters with the values according to the method
     described in `Delving deep into rectifiers: Surpassing human-level
     performance on ImageNet classification - He, K. et al. (2015).
     <https://www.cv-foundation.org/openaccess/content_iccv_2015/
     papers/He_Delving_Deep_into_ICCV_2015_paper.pdf>`_
 
@@ -404,67 +377,56 @@
             Defaults to None.
         distribution (str): distribution either be ``'normal'`` or
             ``'uniform'``. Defaults to ``'normal'``.
         layer (str | list[str], optional): the layer will be initialized.
             Defaults to None.
     """
 
-    def __init__(self,
-                 a=0,
-                 mode='fan_out',
-                 nonlinearity='relu',
-                 distribution='normal',
-                 **kwargs):
+    def __init__(self, a=0, mode="fan_out", nonlinearity="relu", distribution="normal", **kwargs):
         super().__init__(**kwargs)
         self.a = a
         self.mode = mode
         self.nonlinearity = nonlinearity
         self.distribution = distribution
 
     def __call__(self, module):
-
         def init(m):
             if self.wholemodule:
-                kaiming_init(m, self.a, self.mode, self.nonlinearity,
-                             self.bias, self.distribution)
+                kaiming_init(m, self.a, self.mode, self.nonlinearity, self.bias, self.distribution)
             else:
                 layername = m.__class__.__name__
                 basesname = _get_bases_name(m)
                 if len(set(self.layer) & set([layername] + basesname)):
-                    kaiming_init(m, self.a, self.mode, self.nonlinearity,
-                                 self.bias, self.distribution)
+                    kaiming_init(m, self.a, self.mode, self.nonlinearity, self.bias, self.distribution)
 
         module.apply(init)
-        if hasattr(module, '_params_init_info'):
+        if hasattr(module, "_params_init_info"):
             update_init_info(module, init_info=self._get_init_info())
 
     def _get_init_info(self):
-        info = f'{self.__class__.__name__}: a={self.a}, mode={self.mode}, ' \
-               f'nonlinearity={self.nonlinearity}, ' \
-               f'distribution ={self.distribution}, bias={self.bias}'
+        info = (
+            f"{self.__class__.__name__}: a={self.a}, mode={self.mode}, "
+            f"nonlinearity={self.nonlinearity}, "
+            f"distribution ={self.distribution}, bias={self.bias}"
+        )
         return info
 
 
-@INITIALIZERS.register_module(name='Caffe2Xavier')
+@INITIALIZERS.register_module(name="Caffe2Xavier")
 class Caffe2XavierInit(KaimingInit):
     # `XavierFill` in Caffe2 corresponds to `kaiming_uniform_` in PyTorch
     # Acknowledgment to FAIR's internal code
     def __init__(self, **kwargs):
-        super().__init__(
-            a=1,
-            mode='fan_in',
-            nonlinearity='leaky_relu',
-            distribution='uniform',
-            **kwargs)
+        super().__init__(a=1, mode="fan_in", nonlinearity="leaky_relu", distribution="uniform", **kwargs)
 
     def __call__(self, module):
         super().__call__(module)
 
 
-@INITIALIZERS.register_module(name='Pretrained')
+@INITIALIZERS.register_module(name="Pretrained")
 class PretrainedInit(object):
     """Initialize module by loading a pretrained model.
 
     Args:
         checkpoint (str): the checkpoint file of the pretrained model should
             be load.
         prefix (str, optional): the prefix of a sub-module in the pretrained
@@ -477,78 +439,72 @@
 
     def __init__(self, checkpoint, prefix=None, map_location=None):
         self.checkpoint = checkpoint
         self.prefix = prefix
         self.map_location = map_location
 
     def __call__(self, module):
-        from comfy_controlnet_preprocessors.uniformer.mmcv.runner import (_load_checkpoint_with_prefix, load_checkpoint,
-                                 load_state_dict)
-        logger = get_logger('mmcv')
+        from comfy_controlnet_preprocessors.uniformer.mmcv.runner import (
+            _load_checkpoint_with_prefix,
+            load_checkpoint,
+            load_state_dict,
+        )
+
+        logger = get_logger("mmcv")
         if self.prefix is None:
-            print_log(f'load model from: {self.checkpoint}', logger=logger)
-            load_checkpoint(
-                module,
-                self.checkpoint,
-                map_location=self.map_location,
-                strict=False,
-                logger=logger)
+            print_log(f"load model from: {self.checkpoint}", logger=logger)
+            load_checkpoint(module, self.checkpoint, map_location=self.map_location, strict=False, logger=logger)
         else:
-            print_log(
-                f'load {self.prefix} in model from: {self.checkpoint}',
-                logger=logger)
-            state_dict = _load_checkpoint_with_prefix(
-                self.prefix, self.checkpoint, map_location=self.map_location)
+            print_log(f"load {self.prefix} in model from: {self.checkpoint}", logger=logger)
+            state_dict = _load_checkpoint_with_prefix(self.prefix, self.checkpoint, map_location=self.map_location)
             load_state_dict(module, state_dict, strict=False, logger=logger)
 
-        if hasattr(module, '_params_init_info'):
+        if hasattr(module, "_params_init_info"):
             update_init_info(module, init_info=self._get_init_info())
 
     def _get_init_info(self):
-        info = f'{self.__class__.__name__}: load from {self.checkpoint}'
+        info = f"{self.__class__.__name__}: load from {self.checkpoint}"
         return info
 
 
 def _initialize(module, cfg, wholemodule=False):
     func = build_from_cfg(cfg, INITIALIZERS)
     # wholemodule flag is for override mode, there is no layer key in override
     # and initializer will give init values for the whole module with the name
     # in override.
     func.wholemodule = wholemodule
     func(module)
 
 
 def _initialize_override(module, override, cfg):
     if not isinstance(override, (dict, list)):
-        raise TypeError(f'override must be a dict or a list of dict, \
-                but got {type(override)}')
+        raise TypeError(
+            f"override must be a dict or a list of dict, \
+                but got {type(override)}"
+        )
 
     override = [override] if isinstance(override, dict) else override
 
     for override_ in override:
-
         cp_override = copy.deepcopy(override_)
-        name = cp_override.pop('name', None)
+        name = cp_override.pop("name", None)
         if name is None:
-            raise ValueError('`override` must contain the key "name",'
-                             f'but got {cp_override}')
+            raise ValueError('`override` must contain the key "name",' f"but got {cp_override}")
         # if override only has name key, it means use args in init_cfg
         if not cp_override:
             cp_override.update(cfg)
         # if override has name key and other args except type key, it will
         # raise error
-        elif 'type' not in cp_override.keys():
-            raise ValueError(
-                f'`override` need "type" key, but got {cp_override}')
+        elif "type" not in cp_override.keys():
+            raise ValueError(f'`override` need "type" key, but got {cp_override}')
 
         if hasattr(module, name):
             _initialize(getattr(module, name), cp_override, wholemodule=True)
         else:
-            raise RuntimeError(f'module did not have attribute {name}, '
-                               f'but init_cfg is {cp_override}.')
+            raise RuntimeError(f"module did not have attribute {name}, " f"but init_cfg is {cp_override}.")
 
 
 def initialize(module, init_cfg):
     """Initialize a module.
 
     Args:
         module (``torch.nn.Module``): the module will be initialized.
@@ -592,52 +548,54 @@
         >>> url = 'http://download.openmmlab.com/mmdetection/v2.0/retinanet/'\
         >>>     'retinanet_r50_fpn_1x_coco/'\
         >>>     'retinanet_r50_fpn_1x_coco_20200130-c2398f9e.pth'
         >>> init_cfg = dict(type='Pretrained',
                 checkpoint=url, prefix='backbone.')
     """
     if not isinstance(init_cfg, (dict, list)):
-        raise TypeError(f'init_cfg must be a dict or a list of dict, \
-                but got {type(init_cfg)}')
+        raise TypeError(
+            f"init_cfg must be a dict or a list of dict, \
+                but got {type(init_cfg)}"
+        )
 
     if isinstance(init_cfg, dict):
         init_cfg = [init_cfg]
 
     for cfg in init_cfg:
         # should deeply copy the original config because cfg may be used by
         # other modules, e.g., one init_cfg shared by multiple bottleneck
         # blocks, the expected cfg will be changed after pop and will change
         # the initialization behavior of other modules
         cp_cfg = copy.deepcopy(cfg)
-        override = cp_cfg.pop('override', None)
+        override = cp_cfg.pop("override", None)
         _initialize(module, cp_cfg)
 
         if override is not None:
-            cp_cfg.pop('layer', None)
+            cp_cfg.pop("layer", None)
             _initialize_override(module, override, cp_cfg)
         else:
             # All attributes in module have same initialization.
             pass
 
 
-def _no_grad_trunc_normal_(tensor: Tensor, mean: float, std: float, a: float,
-                           b: float) -> Tensor:
+def _no_grad_trunc_normal_(tensor: Tensor, mean: float, std: float, a: float, b: float) -> Tensor:
     # Method based on
     # https://people.sc.fsu.edu/~jburkardt/presentations/truncated_normal.pdf
     # Modified from
     # https://github.com/pytorch/pytorch/blob/master/torch/nn/init.py
     def norm_cdf(x):
         # Computes standard normal cumulative distribution function
-        return (1. + math.erf(x / math.sqrt(2.))) / 2.
+        return (1.0 + math.erf(x / math.sqrt(2.0))) / 2.0
 
     if (mean < a - 2 * std) or (mean > b + 2 * std):
         warnings.warn(
-            'mean is more than 2 std from [a, b] in nn.init.trunc_normal_. '
-            'The distribution of values may be incorrect.',
-            stacklevel=2)
+            "mean is more than 2 std from [a, b] in nn.init.trunc_normal_. "
+            "The distribution of values may be incorrect.",
+            stacklevel=2,
+        )
 
     with torch.no_grad():
         # Values are generated by using a truncated uniform distribution and
         # then using the inverse CDF for the normal distribution.
         # Get upper and lower cdf values
         lower = norm_cdf((a - mean) / std)
         upper = norm_cdf((b - mean) / std)
@@ -647,27 +605,23 @@
         tensor.uniform_(2 * lower - 1, 2 * upper - 1)
 
         # Use inverse cdf transform for normal distribution to get truncated
         # standard normal
         tensor.erfinv_()
 
         # Transform to proper mean, std
-        tensor.mul_(std * math.sqrt(2.))
+        tensor.mul_(std * math.sqrt(2.0))
         tensor.add_(mean)
 
         # Clamp to ensure it's in the proper range
         tensor.clamp_(min=a, max=b)
         return tensor
 
 
-def trunc_normal_(tensor: Tensor,
-                  mean: float = 0.,
-                  std: float = 1.,
-                  a: float = -2.,
-                  b: float = 2.) -> Tensor:
+def trunc_normal_(tensor: Tensor, mean: float = 0.0, std: float = 1.0, a: float = -2.0, b: float = 2.0) -> Tensor:
     r"""Fills the input Tensor with values drawn from a truncated
     normal distribution. The values are effectively drawn from the
     normal distribution :math:`\mathcal{N}(\text{mean}, \text{std}^2)`
     with values outside :math:`[a, b]` redrawn until they are within
     the bounds. The method used for generating the random values works
     best when :math:`a \leq \text{mean} \leq b`.
```

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,27 @@
-# Copyright (c) OpenMMLab. All rights reserved.
+# Copyright (c) OpenMMLab. All rights reserved.\
+import sys
 from comfy_controlnet_preprocessors.uniformer.mmcv.utils import Registry, is_method_overridden
 
-HOOKS = Registry('hook')
+HOOKS = Registry("hook", sys.modules[__name__])
 
 
 class Hook:
-    stages = ('before_run', 'before_train_epoch', 'before_train_iter',
-              'after_train_iter', 'after_train_epoch', 'before_val_epoch',
-              'before_val_iter', 'after_val_iter', 'after_val_epoch',
-              'after_run')
+    stages = (
+        "before_run",
+        "before_train_epoch",
+        "before_train_iter",
+        "after_train_iter",
+        "after_train_epoch",
+        "before_val_epoch",
+        "before_val_iter",
+        "after_val_iter",
+        "after_val_epoch",
+        "after_run",
+    )
 
     def before_run(self, runner):
         pass
 
     def after_run(self, runner):
         pass
 
@@ -75,18 +84,18 @@
         for stage in Hook.stages:
             if is_method_overridden(stage, Hook, self):
                 trigger_stages.add(stage)
 
         # some methods will be triggered in multi stages
         # use this dict to map method to stages.
         method_stages_map = {
-            'before_epoch': ['before_train_epoch', 'before_val_epoch'],
-            'after_epoch': ['after_train_epoch', 'after_val_epoch'],
-            'before_iter': ['before_train_iter', 'before_val_iter'],
-            'after_iter': ['after_train_iter', 'after_val_iter'],
+            "before_epoch": ["before_train_epoch", "before_val_epoch"],
+            "after_epoch": ["after_train_epoch", "after_val_epoch"],
+            "before_iter": ["before_train_iter", "before_val_iter"],
+            "after_iter": ["after_train_iter", "after_val_iter"],
         }
 
         for method, map_stages in method_stages_map.items():
             if is_method_overridden(method, Hook, self):
                 trigger_stages.update(map_stages)
 
         return [stage for stage in Hook.stages if stage in trigger_stages]
```

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import uuid
 import warnings
 from argparse import Action, ArgumentParser
 from collections import abc
 from importlib import import_module
 
 from addict import Dict
-from yapf.yapflib.yapf_api import FormatCode
 
 from .misc import import_modules_from_strings
 from .path import check_file_exist
 
 if platform.system() == 'Windows':
     import regex as re
 else:
@@ -484,20 +483,14 @@
             r += '\n'.join(s)
             if use_mapping:
                 r += '}'
             return r
 
         cfg_dict = self._cfg_dict.to_dict()
         text = _format_dict(cfg_dict, outest_level=True)
-        # copied from setup.cfg
-        yapf_style = dict(
-            based_on_style='pep8',
-            blank_line_before_nested_class_or_def=True,
-            split_before_expression_after_opening_paren=True)
-        text, _ = FormatCode(text, style_config=yapf_style, verify=True)
 
         return text
 
     def __repr__(self):
         return f'Config (path: {self.filename}): {self._cfg_dict.__repr__()}'
 
     def __len__(self):
```

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,57 +14,51 @@
         registry (:obj:`Registry`): The registry to search the type from.
         default_args (dict, optional): Default initialization arguments.
 
     Returns:
         object: The constructed object.
     """
     if not isinstance(cfg, dict):
-        raise TypeError(f'cfg must be a dict, but got {type(cfg)}')
-    if 'type' not in cfg:
-        if default_args is None or 'type' not in default_args:
-            raise KeyError(
-                '`cfg` or `default_args` must contain the key "type", '
-                f'but got {cfg}\n{default_args}')
+        raise TypeError(f"cfg must be a dict, but got {type(cfg)}")
+    if "type" not in cfg:
+        if default_args is None or "type" not in default_args:
+            raise KeyError('`cfg` or `default_args` must contain the key "type", ' f"but got {cfg}\n{default_args}")
     if not isinstance(registry, Registry):
-        raise TypeError('registry must be an mmcv.Registry object, '
-                        f'but got {type(registry)}')
+        raise TypeError("registry must be an mmcv.Registry object, " f"but got {type(registry)}")
     if not (isinstance(default_args, dict) or default_args is None):
-        raise TypeError('default_args must be a dict or None, '
-                        f'but got {type(default_args)}')
+        raise TypeError("default_args must be a dict or None, " f"but got {type(default_args)}")
 
     args = cfg.copy()
 
     if default_args is not None:
         for name, value in default_args.items():
             args.setdefault(name, value)
 
-    obj_type = args.pop('type')
+    obj_type = args.pop("type")
     if isinstance(obj_type, str):
         obj_cls = registry.get(obj_type)
         if obj_cls is None:
-            raise KeyError(
-                f'{obj_type} is not in the {registry.name} registry')
+            raise KeyError(f"{obj_type} is not in the {registry.name} registry")
     elif inspect.isclass(obj_type):
         obj_cls = obj_type
     else:
-        raise TypeError(
-            f'type must be a str or valid type, but got {type(obj_type)}')
+        raise TypeError(f"type must be a str or valid type, but got {type(obj_type)}")
     try:
         return obj_cls(**args)
     except Exception as e:
         # Normal TypeError does not print class name.
-        raise type(e)(f'{obj_cls.__name__}: {e}')
+        raise type(e)(f"{obj_cls.__name__}: {e}")
 
 
 class Registry:
     """A registry to map strings to classes.
 
     Registered object could be built from registry.
     Example:
-        >>> MODELS = Registry('models')
+        >>> MODELS = Registry('models', sys.modules[__name__])
         >>> @MODELS.register_module()
         >>> class ResNet:
         >>>     pass
         >>> resnet = MODELS.build(dict(type='ResNet'))
 
     Please refer to
     https://mmcv.readthedocs.io/en/latest/understand_mmcv/registry.html for
@@ -81,19 +75,20 @@
             children registry could be built from parent. Default: None.
         scope (str, optional): The scope of registry. It is the key to search
             for children registry. If not specified, scope will be the name of
             the package where class is defined, e.g. mmdet, mmcls, mmseg.
             Default: None.
     """
 
-    def __init__(self, name, build_func=None, parent=None, scope=None):
+    def __init__(self, name, calling_module, build_func=None, parent=None):
         self._name = name
         self._module_dict = dict()
         self._children = dict()
-        self._scope = self.infer_scope() if scope is None else scope
+        # self._scope = self.infer_scope()  # if scope is None else scope
+        self._scope = calling_module.__name__.split(".")[0]
 
         # self.build_func will be set with the following priority:
         # 1. build_func
         # 2. parent.build_func
         # 3. build_from_cfg
         if build_func is None:
             if parent is not None:
@@ -112,41 +107,39 @@
     def __len__(self):
         return len(self._module_dict)
 
     def __contains__(self, key):
         return self.get(key) is not None
 
     def __repr__(self):
-        format_str = self.__class__.__name__ + \
-                     f'(name={self._name}, ' \
-                     f'items={self._module_dict})'
+        format_str = self.__class__.__name__ + f"(name={self._name}, " f"items={self._module_dict})"
         return format_str
 
     @staticmethod
     def infer_scope():
         """Infer the scope of registry.
 
         The name of the package where registry is defined will be returned.
 
         Example:
             # in mmdet/models/backbone/resnet.py
-            >>> MODELS = Registry('models')
+            >>> MODELS = Registry('models', sys.modules[__name__])
             >>> @MODELS.register_module()
             >>> class ResNet:
             >>>     pass
             The scope of ``ResNet`` will be ``mmdet``.
 
 
         Returns:
             scope (str): The inferred scope name.
         """
         # inspect.stack() trace where this function is called, the index-2
         # indicates the frame where `infer_scope()` is called
         filename = inspect.getmodule(inspect.stack()[2][0]).__name__
-        split_filename = filename.split('.')
+        split_filename = filename.split(".")
         return split_filename[0]
 
     @staticmethod
     def split_scope_key(key):
         """Split scope and key.
 
         The first scope will be split from key.
@@ -157,17 +150,17 @@
             >>> Registry.split_scope_key('ResNet')
             None, 'ResNet'
 
         Return:
             scope (str, None): The first scope.
             key (str): The remaining key.
         """
-        split_index = key.find('.')
+        split_index = key.find(".")
         if split_index != -1:
-            return key[:split_index], key[split_index + 1:]
+            return key[:split_index], key[split_index + 1 :]
         else:
             return None, key
 
     @property
     def name(self):
         return self._name
 
@@ -214,102 +207,98 @@
     def _add_children(self, registry):
         """Add children for a registry.
 
         The ``registry`` will be added as children based on its scope.
         The parent registry could build objects from children registry.
 
         Example:
-            >>> models = Registry('models')
-            >>> mmdet_models = Registry('models', parent=models)
+            >>> models = Registry('models', sys.modules[__name__])
+            >>> mmdet_models = Registry('models', sys.modules[__name__], parent=models)
             >>> @mmdet_models.register_module()
             >>> class ResNet:
             >>>     pass
             >>> resnet = models.build(dict(type='mmdet.ResNet'))
         """
 
         assert isinstance(registry, Registry)
         assert registry.scope is not None
-        assert registry.scope not in self.children, \
-            f'scope {registry.scope} exists in {self.name} registry'
+        assert registry.scope not in self.children, f"scope {registry.scope} exists in {self.name} registry"
         self.children[registry.scope] = registry
 
     def _register_module(self, module_class, module_name=None, force=False):
         if not inspect.isclass(module_class):
-            raise TypeError('module must be a class, '
-                            f'but got {type(module_class)}')
+            raise TypeError("module must be a class, " f"but got {type(module_class)}")
 
         if module_name is None:
             module_name = module_class.__name__
         if isinstance(module_name, str):
             module_name = [module_name]
         for name in module_name:
             if not force and name in self._module_dict:
-                raise KeyError(f'{name} is already registered '
-                               f'in {self.name}')
+                raise KeyError(f"{name} is already registered " f"in {self.name}")
             self._module_dict[name] = module_class
 
     def deprecated_register_module(self, cls=None, force=False):
         warnings.warn(
-            'The old API of register_module(module, force=False) '
-            'is deprecated and will be removed, please use the new API '
-            'register_module(name=None, force=False, module=None) instead.')
+            "The old API of register_module(module, force=False) "
+            "is deprecated and will be removed, please use the new API "
+            "register_module(name=None, force=False, module=None) instead."
+        )
         if cls is None:
             return partial(self.deprecated_register_module, force=force)
         self._register_module(cls, force=force)
         return cls
 
     def register_module(self, name=None, force=False, module=None):
         """Register a module.
 
         A record will be added to `self._module_dict`, whose key is the class
         name or the specified name, and value is the class itself.
         It can be used as a decorator or a normal function.
 
         Example:
-            >>> backbones = Registry('backbone')
+            >>> backbones = Registry('backbone', sys.modules[__name__])
             >>> @backbones.register_module()
             >>> class ResNet:
             >>>     pass
 
-            >>> backbones = Registry('backbone')
+            >>> backbones = Registry('backbone', sys.modules[__name__])
             >>> @backbones.register_module(name='mnet')
             >>> class MobileNet:
             >>>     pass
 
-            >>> backbones = Registry('backbone')
+            >>> backbones = Registry('backbone', sys.modules[__name__])
             >>> class ResNet:
             >>>     pass
             >>> backbones.register_module(ResNet)
 
         Args:
             name (str | None): The module name to be registered. If not
                 specified, the class name will be used.
             force (bool, optional): Whether to override an existing class with
                 the same name. Default: False.
             module (type): Module class to be registered.
         """
         if not isinstance(force, bool):
-            raise TypeError(f'force must be a boolean, but got {type(force)}')
+            raise TypeError(f"force must be a boolean, but got {type(force)}")
         # NOTE: This is a walkaround to be compatible with the old api,
         # while it may introduce unexpected bugs.
         if isinstance(name, type):
             return self.deprecated_register_module(name, force=force)
 
         # raise the error ahead of time
         if not (name is None or isinstance(name, str) or is_seq_of(name, str)):
             raise TypeError(
-                'name must be either of None, an instance of str or a sequence'
-                f'  of str, but got {type(name)}')
+                "name must be either of None, an instance of str or a sequence" f"  of str, but got {type(name)}"
+            )
 
         # use it as a normal method: x.register_module(module=SomeClass)
         if module is not None:
-            self._register_module(
-                module_class=module, module_name=name, force=force)
+            self._register_module(module_class=module, module_name=name, force=force)
             return module
 
         # use it as a decorator: @x.register_module()
         def _register(cls):
-            self._register_module(
-                module_class=cls, module_name=name, force=force)
+            self._register_module(module_class=cls, module_name=name, force=force)
             return cls
 
         return _register
```

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import matplotlib.pyplot as plt
 import comfy_controlnet_preprocessors.uniformer.mmcv as mmcv
 import torch
 from comfy_controlnet_preprocessors.uniformer.mmcv.parallel import collate, scatter
 from comfy_controlnet_preprocessors.uniformer.mmcv.runner import load_checkpoint
 
 from comfy_controlnet_preprocessors.uniformer.mmseg.datasets.pipelines import Compose
 from comfy_controlnet_preprocessors.uniformer.mmseg.models import build_segmentor
```

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 import copy
 import platform
 import random
 from functools import partial
+import sys
 
 import numpy as np
 from comfy_controlnet_preprocessors.uniformer.mmcv.parallel import collate
 from comfy_controlnet_preprocessors.uniformer.mmcv.runner import get_dist_info
 from comfy_controlnet_preprocessors.uniformer.mmcv.utils import Registry, build_from_cfg
 from comfy_controlnet_preprocessors.uniformer.mmcv.utils.parrots_wrapper import DataLoader, PoolDataLoader
 from torch.utils.data import DistributedSampler
 
-if platform.system() != 'Windows':
+if platform.system() != "Windows":
     # https://github.com/pytorch/pytorch/issues/973
     import resource
+
     rlimit = resource.getrlimit(resource.RLIMIT_NOFILE)
     hard_limit = rlimit[1]
     soft_limit = min(4096, hard_limit)
     resource.setrlimit(resource.RLIMIT_NOFILE, (soft_limit, hard_limit))
 
-DATASETS = Registry('dataset')
-PIPELINES = Registry('pipeline')
+DATASETS = Registry("dataset", sys.modules[__name__])
+PIPELINES = Registry("pipeline", sys.modules[__name__])
 
 
 def _concat_dataset(cfg, default_args=None):
     """Build :obj:`ConcatDataset by."""
     from .dataset_wrappers import ConcatDataset
-    img_dir = cfg['img_dir']
-    ann_dir = cfg.get('ann_dir', None)
-    split = cfg.get('split', None)
+
+    img_dir = cfg["img_dir"]
+    ann_dir = cfg.get("ann_dir", None)
+    split = cfg.get("split", None)
     num_img_dir = len(img_dir) if isinstance(img_dir, (list, tuple)) else 1
     if ann_dir is not None:
         num_ann_dir = len(ann_dir) if isinstance(ann_dir, (list, tuple)) else 1
     else:
         num_ann_dir = 0
     if split is not None:
         num_split = len(split) if isinstance(split, (list, tuple)) else 1
@@ -44,52 +47,53 @@
         assert num_split == num_ann_dir or num_ann_dir <= 1
     num_dset = max(num_split, num_img_dir)
 
     datasets = []
     for i in range(num_dset):
         data_cfg = copy.deepcopy(cfg)
         if isinstance(img_dir, (list, tuple)):
-            data_cfg['img_dir'] = img_dir[i]
+            data_cfg["img_dir"] = img_dir[i]
         if isinstance(ann_dir, (list, tuple)):
-            data_cfg['ann_dir'] = ann_dir[i]
+            data_cfg["ann_dir"] = ann_dir[i]
         if isinstance(split, (list, tuple)):
-            data_cfg['split'] = split[i]
+            data_cfg["split"] = split[i]
         datasets.append(build_dataset(data_cfg, default_args))
 
     return ConcatDataset(datasets)
 
 
 def build_dataset(cfg, default_args=None):
     """Build datasets."""
     from .dataset_wrappers import ConcatDataset, RepeatDataset
+
     if isinstance(cfg, (list, tuple)):
         dataset = ConcatDataset([build_dataset(c, default_args) for c in cfg])
-    elif cfg['type'] == 'RepeatDataset':
-        dataset = RepeatDataset(
-            build_dataset(cfg['dataset'], default_args), cfg['times'])
-    elif isinstance(cfg.get('img_dir'), (list, tuple)) or isinstance(
-            cfg.get('split', None), (list, tuple)):
+    elif cfg["type"] == "RepeatDataset":
+        dataset = RepeatDataset(build_dataset(cfg["dataset"], default_args), cfg["times"])
+    elif isinstance(cfg.get("img_dir"), (list, tuple)) or isinstance(cfg.get("split", None), (list, tuple)):
         dataset = _concat_dataset(cfg, default_args)
     else:
         dataset = build_from_cfg(cfg, DATASETS, default_args)
 
     return dataset
 
 
-def build_dataloader(dataset,
-                     samples_per_gpu,
-                     workers_per_gpu,
-                     num_gpus=1,
-                     dist=True,
-                     shuffle=True,
-                     seed=None,
-                     drop_last=False,
-                     pin_memory=True,
-                     dataloader_type='PoolDataLoader',
-                     **kwargs):
+def build_dataloader(
+    dataset,
+    samples_per_gpu,
+    workers_per_gpu,
+    num_gpus=1,
+    dist=True,
+    shuffle=True,
+    seed=None,
+    drop_last=False,
+    pin_memory=True,
+    dataloader_type="PoolDataLoader",
+    **kwargs,
+):
     """Build PyTorch DataLoader.
 
     In distributed training, each GPU/process has a dataloader.
     In non-distributed training, there is only one dataloader for all GPUs.
 
     Args:
         dataset (Dataset): A PyTorch dataset.
@@ -110,48 +114,44 @@
         kwargs: any keyword argument to be used to initialize DataLoader
 
     Returns:
         DataLoader: A PyTorch dataloader.
     """
     rank, world_size = get_dist_info()
     if dist:
-        sampler = DistributedSampler(
-            dataset, world_size, rank, shuffle=shuffle)
+        sampler = DistributedSampler(dataset, world_size, rank, shuffle=shuffle)
         shuffle = False
         batch_size = samples_per_gpu
         num_workers = workers_per_gpu
     else:
         sampler = None
         batch_size = num_gpus * samples_per_gpu
         num_workers = num_gpus * workers_per_gpu
 
-    init_fn = partial(
-        worker_init_fn, num_workers=num_workers, rank=rank,
-        seed=seed) if seed is not None else None
-
-    assert dataloader_type in (
-        'DataLoader',
-        'PoolDataLoader'), f'unsupported dataloader {dataloader_type}'
+    init_fn = partial(worker_init_fn, num_workers=num_workers, rank=rank, seed=seed) if seed is not None else None
+
+    assert dataloader_type in ("DataLoader", "PoolDataLoader"), f"unsupported dataloader {dataloader_type}"
 
-    if dataloader_type == 'PoolDataLoader':
+    if dataloader_type == "PoolDataLoader":
         dataloader = PoolDataLoader
-    elif dataloader_type == 'DataLoader':
+    elif dataloader_type == "DataLoader":
         dataloader = DataLoader
 
     data_loader = dataloader(
         dataset,
         batch_size=batch_size,
         sampler=sampler,
         num_workers=num_workers,
         collate_fn=partial(collate, samples_per_gpu=samples_per_gpu),
         pin_memory=pin_memory,
         shuffle=shuffle,
         worker_init_fn=init_fn,
         drop_last=drop_last,
-        **kwargs)
+        **kwargs,
+    )
 
     return data_loader
 
 
 def worker_init_fn(worker_id, num_workers, rank, seed):
     """Worker init func for dataloader.
```

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import os.path as osp
 from collections import OrderedDict
 from functools import reduce
 
 import comfy_controlnet_preprocessors.uniformer.mmcv as mmcv
 import numpy as np
 from comfy_controlnet_preprocessors.uniformer.mmcv.utils import print_log
-from prettytable import PrettyTable
 from torch.utils.data import Dataset
 
 from comfy_controlnet_preprocessors.uniformer.mmseg.core import eval_metrics
 from comfy_controlnet_preprocessors.uniformer.mmseg.utils import get_root_logger
 from .builder import DATASETS
 from .pipelines import Compose
 
@@ -359,31 +358,14 @@
         ret_metrics_class = OrderedDict({
             ret_metric: np.round(ret_metric_value * 100, 2)
             for ret_metric, ret_metric_value in ret_metrics.items()
         })
         ret_metrics_class.update({'Class': class_names})
         ret_metrics_class.move_to_end('Class', last=False)
 
-        # for logger
-        class_table_data = PrettyTable()
-        for key, val in ret_metrics_class.items():
-            class_table_data.add_column(key, val)
-
-        summary_table_data = PrettyTable()
-        for key, val in ret_metrics_summary.items():
-            if key == 'aAcc':
-                summary_table_data.add_column(key, [val])
-            else:
-                summary_table_data.add_column('m' + key, [val])
-
-        print_log('per class results:', logger)
-        print_log('\n' + class_table_data.get_string(), logger=logger)
-        print_log('Summary:', logger)
-        print_log('\n' + summary_table_data.get_string(), logger=logger)
-
         # each metric dict
         for key, value in ret_metrics_summary.items():
             if key == 'aAcc':
                 eval_results[key] = value / 100.0
             else:
                 eval_results['m' + key] = value / 100.0
```

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+import sys
 import warnings
 
 from comfy_controlnet_preprocessors.uniformer.mmcv.cnn import MODELS as MMCV_MODELS
 from comfy_controlnet_preprocessors.uniformer.mmcv.utils import Registry
 
-MODELS = Registry('models', parent=MMCV_MODELS)
+MODELS = Registry("models", sys.modules[__name__], parent=MMCV_MODELS)
 
 BACKBONES = MODELS
 NECKS = MODELS
 HEADS = MODELS
 LOSSES = MODELS
 SEGMENTORS = MODELS
 
@@ -31,16 +32,13 @@
     """Build loss."""
     return LOSSES.build(cfg)
 
 
 def build_segmentor(cfg, train_cfg=None, test_cfg=None):
     """Build segmentor."""
     if train_cfg is not None or test_cfg is not None:
-        warnings.warn(
-            'train_cfg and test_cfg is deprecated, '
-            'please specify them in model', UserWarning)
-    assert cfg.get('train_cfg') is None or train_cfg is None, \
-        'train_cfg specified in both outer field and model field '
-    assert cfg.get('test_cfg') is None or test_cfg is None, \
-        'test_cfg specified in both outer field and model field '
-    return SEGMENTORS.build(
-        cfg, default_args=dict(train_cfg=train_cfg, test_cfg=test_cfg))
+        warnings.warn("train_cfg and test_cfg is deprecated, " "please specify them in model", UserWarning)
+    assert (
+        cfg.get("train_cfg") is None or train_cfg is None
+    ), "train_cfg specified in both outer field and model field "
+    assert cfg.get("test_cfg") is None or test_cfg is None, "test_cfg specified in both outer field and model field "
+    return SEGMENTORS.build(cfg, default_args=dict(train_cfg=train_cfg, test_cfg=test_cfg))
```

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/comfy_controlnet_preprocessors/util.py` & `hordelib-1.0.0/hordelib/nodes/comfy_controlnet_preprocessors/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 import math
 import requests
 from torch.hub import download_url_to_file, get_dir
 from tqdm import tqdm
 from urllib.parse import urlparse
 import torch
 
+import builtins
 
-annotator_ckpts_path = os.path.join(os.path.dirname(__file__), "ckpts")
+builtins.annotator_ckpts_path = os.path.join(os.path.dirname(__file__), "ckpts")
 
 
 def HWC3(x):
     assert x.dtype == np.uint8
     if x.ndim == 2:
         x = x[:, :, None]
     assert x.ndim == 3
```

### Comparing `hordelib-0.9.5/hordelib/nodes/facerestore/__init__.py` & `hordelib-1.0.0/hordelib/nodes/facerestore/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,15 +130,19 @@
     RETURN_TYPES = ("IMAGE",)
 
     FUNCTION = "restore_face"
 
     CATEGORY = "facerestore"
 
     def restore_face(self, upscale_model, image, facedetection):
+        # logger.warning(f"mutex:{id(FaceRestoreWithModel._mutex):x} Facerestore with upscale_model {id(upscale_model):x} and detection model {id(facedetection):x} and image {id(image):x}")
         with FaceRestoreWithModel._mutex:
+
+            # facedetection = copy.deepcopy(facedetection)
+
             device = model_management.get_torch_device()
             upscale_model.to(device)
             face_helper = FaceRestoreHelper(
                 1,
                 face_size=512,
                 crop_ratio=(1, 1),
                 det_model=facedetection,
@@ -151,23 +155,23 @@
 
             image_np = image_np[:, :, ::-1]
 
             original_resolution = image_np.shape[0:2]
 
             if upscale_model is None or face_helper is None:
                 return image
-
+        
             face_helper.clean_all()
             face_helper.read_image(image_np)
             face_helper.get_face_landmarks_5(
                 only_center_face=False, resize=640, eye_dist_threshold=5
             )
             face_helper.align_warp_face()
-
             restored_face = None
+
             for idx, cropped_face in enumerate(face_helper.cropped_faces):
                 cropped_face_t = img2tensor(
                     cropped_face / 255.0, bgr2rgb=True, float32=True
                 )
                 normalize(cropped_face_t, (0.5, 0.5, 0.5), (0.5, 0.5, 0.5), inplace=True)
                 cropped_face_t = cropped_face_t.unsqueeze(0).to(device)
```

### Comparing `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/__init__.py` & `hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/align_trans.py` & `hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/align_trans.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py` & `hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py` & `hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py` & `hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py` & `hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py` & `hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,19 +13,22 @@
 from facerestore.facelib.detection.yolov5face.utils.general import (
     check_img_size,
     non_max_suppression_face,
     scale_coords,
     scale_coords_landmarks,
 )
 
-IS_HIGH_VERSION = tuple(map(int, torch.__version__.split("+")[0].split("."))) >= (
-    1,
-    9,
-    0,
-)
+
+def is_high_version():
+    from packaging import version
+    try:
+        torch_v = version.parse(torch.__version__)
+        return torch_v > version.parse("1.9.0")
+    except Exception:
+        return True
 
 
 def isListempty(inList):
     if isinstance(inList, list):  # Is a list
         return all(map(isListempty, inList))
     return False  # Not a list
 
@@ -144,15 +147,15 @@
         # Pass input images through face detector
         images = imgs if isinstance(imgs, list) else [imgs]
         images = [cv2.cvtColor(img, cv2.COLOR_BGR2RGB) for img in images]
         origimgs = copy.deepcopy(images)
 
         images = self._preprocess(images)
 
-        if IS_HIGH_VERSION:
+        if is_high_version():
             with torch.inference_mode():  # for pytorch>=1.9
                 pred = self.detector(images)[0]
         else:
             with torch.no_grad():  # for pytorch<1.9
                 pred = self.detector(images)[0]
 
         bboxes, points = self._postprocess(
```

### Comparing `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py` & `hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py` & `hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py` & `hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml` & `hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml` & `hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py` & `hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py` & `hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py` & `hordelib-1.0.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/parsing/__init__.py` & `hordelib-1.0.0/hordelib/nodes/facerestore/facelib/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/parsing/bisenet.py` & `hordelib-1.0.0/hordelib/nodes/facerestore/facelib/parsing/bisenet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/parsing/parsenet.py` & `hordelib-1.0.0/hordelib/nodes/facerestore/facelib/parsing/parsenet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/parsing/resnet.py` & `hordelib-1.0.0/hordelib/nodes/facerestore/facelib/parsing/resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py` & `hordelib-1.0.0/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/utils/face_utils.py` & `hordelib-1.0.0/hordelib/nodes/facerestore/facelib/utils/face_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/facerestore/facelib/utils/misc.py` & `hordelib-1.0.0/hordelib/nodes/facerestore/facelib/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/node_clip_similarities.py` & `hordelib-1.0.0/hordelib/nodes/node_clip_similarities.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/node_image_loader.py` & `hordelib-1.0.0/hordelib/nodes/node_image_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/nodes/node_image_output.py` & `hordelib-1.0.0/hordelib/nodes/node_image_output.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,28 +21,32 @@
     RETURN_TYPES = ()
     FUNCTION = "get_image"
 
     OUTPUT_NODE = True
 
     CATEGORY = "image"
 
+    def _json_hack(self, obj):
+        if hasattr(obj, "__class__"):
+            return f"{obj.__class__.__name__} instance"
+        return f"Object of type {type(obj).__name__}"
+
     def get_image(self, images, prompt=None, extra_pnginfo=None):
         results = []
         for image in images:
             # Create a PNG
             i = 255.0 * image.cpu().numpy()
             img = Image.fromarray(np.clip(i, 0, 255).astype(np.uint8))
             metadata = PngInfo()
             # Save the full pipeline and variables into the PNG metadata
-            # FIXME we don't have a model manager JSON serialiser
-            # if prompt is not None:
-            #     metadata.add_text("prompt", json.dumps(prompt))
-            # if extra_pnginfo is not None:
-            #     for x in extra_pnginfo:
-            #         metadata.add_text(x, json.dumps(extra_pnginfo[x]))
+            if prompt is not None:
+                metadata.add_text("prompt", json.dumps(prompt, default=self._json_hack))
+            if extra_pnginfo is not None:
+                for x in extra_pnginfo:
+                    metadata.add_text(x, json.dumps(extra_pnginfo[x], default=self._json_hack))
 
             byte_stream = BytesIO()
             img.save(byte_stream, format="PNG", pnginfo=metadata, compress_level=4)
             byte_stream.seek(0)
 
             results.append({"imagedata": byte_stream, "type": "PNG"})
```

### Comparing `hordelib-0.9.5/hordelib/nodes/node_model_loader.py` & `hordelib-1.0.0/hordelib/nodes/node_model_loader.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # node_model_loader.py
 # Simple proof of concept custom node to load models.
 
 import contextlib
 import os
 import pickle
+import time
 
 from loguru import logger
 
 
 class HordeCheckpointLoader:
     @classmethod
     def INPUT_TYPES(s):
@@ -41,21 +42,28 @@
 
         model = loaded_models[model_name]["model"]
         clip = loaded_models[model_name]["clip"]
         vae = loaded_models[model_name]["vae"]
 
         # If we got strings, not objects, it's a cache reference, load the cache
         if type(model) is str:
-            logger.info("Loading model data from disk cache")
+            start_time = time.time()
+            logger.info(f"Loading from disk cache model {model_name}")
             model_cache = model
             try:
-                with open(model, "rb") as cache:
-                    model = pickle.load(cache)
-                    vae = pickle.load(cache)
-                    clip = pickle.load(cache)
+                with model_manager.manager.disk_read_mutex:
+                    with open(model, "rb") as cache:
+                        model = pickle.load(cache)
+                        vae = pickle.load(cache)
+                        clip = pickle.load(cache)
+                # Record this model as being in ram again
+                model_manager.manager.move_from_disk_cache(model_name, model, clip, vae)
+                logger.info(
+                    f"Loaded model {model_name} from disk cache in {round(time.time() - start_time, 1)} seconds",
+                )
             except (pickle.PickleError, EOFError):
                 # Most likely corrupt cache file, remove the file
                 with contextlib.suppress(OSError):
                     os.remove(model)  # ... at least try to remove it
 
                 raise Exception(f"Model cache file {model_cache} was corrupt. It has been removed.")
```

### Comparing `hordelib-0.9.5/hordelib/nodes/node_upscale_model_loader.py` & `hordelib-1.0.0/hordelib/nodes/node_upscale_model_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/pipeline_designs/pipeline_controlnet.json` & `hordelib-1.0.0/hordelib/pipeline_designs/pipeline_controlnet.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8424146068932075%*

 * *Differences: {"'last_link_id'": '99',*

 * * "'last_node_id'": '49',*

 * * "'links'": '{18: {insert: [(0, 96), (3, 49)], delete: [3, 0]}, 19: {insert: [(0, 97), (3, 49)], '*

 * *            'delete: [3, 0]}, 21: {insert: [(0, 99), (1, 34)], delete: [1, 0]}, insert: [(20, [98, '*

 * *            "49, 0, 9, 0, 'IMAGE'])], delete: [22, 2]}",*

 * * "'nodes'": "{1: {'order': 13}, 2: {'order': 14}, 3: {'order': 15, 'inputs': {2: {'link': 99}}}, "*

 * *            "4: {'order': 12}, 5: {'order': 18, 'inputs': {0: {'link': 98}}}, 6: {'order': 1}, 7: "*

 * *       […]*

```diff
@@ -1,13 +1,13 @@
 {
     "config": {},
     "extra": {},
     "groups": [],
-    "last_link_id": 95,
-    "last_node_id": 48,
+    "last_link_id": 99,
+    "last_node_id": 49,
     "links": [
         [
             2,
             5,
             0,
             3,
             3,
@@ -18,22 +18,14 @@
             7,
             0,
             3,
             2,
             "CONDITIONING"
         ],
         [
-            9,
-            8,
-            0,
-            9,
-            0,
-            "IMAGE"
-        ],
-        [
             40,
             23,
             0,
             3,
             1,
             "CONDITIONING"
         ],
@@ -154,44 +146,44 @@
             47,
             1,
             24,
             0,
             "CLIP"
         ],
         [
-            83,
+            96,
             47,
             2,
-            8,
+            49,
             1,
             "VAE"
         ],
         [
-            91,
+            97,
             3,
             0,
-            8,
+            49,
             0,
             "LATENT"
         ],
         [
-            94,
-            41,
+            98,
+            49,
+            0,
+            9,
             0,
-            23,
-            2,
             "IMAGE"
         ],
         [
-            95,
-            45,
-            0,
-            41,
+            99,
+            34,
             0,
-            "*"
+            23,
+            2,
+            "IMAGE"
         ]
     ],
     "nodes": [
         {
             "flags": {},
             "id": 5,
             "mode": 0,
@@ -232,15 +224,15 @@
                 {
                     "link": 81,
                     "name": "clip",
                     "type": "CLIP"
                 }
             ],
             "mode": 0,
-            "order": 4,
+            "order": 13,
             "outputs": [
                 {
                     "links": [
                         6
                     ],
                     "name": "CONDITIONING",
                     "slot_index": 0,
@@ -271,15 +263,15 @@
                 {
                     "link": 82,
                     "name": "clip",
                     "type": "CLIP"
                 }
             ],
             "mode": 0,
-            "order": 5,
+            "order": 14,
             "outputs": [
                 {
                     "links": [
                         77
                     ],
                     "name": "CONDITIONING",
                     "slot_index": 0,
@@ -301,161 +293,34 @@
             "type": "CLIPTextEncode",
             "widgets_values": [
                 "a man walking in the snow\n\n\n"
             ]
         },
         {
             "flags": {},
-            "id": 41,
-            "inputs": [
-                {
-                    "link": 95,
-                    "name": "",
-                    "type": "*"
-                }
-            ],
-            "mode": 0,
-            "order": 15,
-            "outputs": [
-                {
-                    "links": [
-                        94
-                    ],
-                    "name": "IMAGE",
-                    "slot_index": 0,
-                    "type": "IMAGE"
-                }
-            ],
-            "pos": [
-                304,
-                77
-            ],
-            "properties": {
-                "horizontal": false,
-                "showOutputText": true
-            },
-            "size": [
-                82,
-                26
-            ],
-            "type": "Reroute"
-        },
-        {
-            "flags": {},
-            "id": 47,
-            "mode": 0,
-            "order": 1,
-            "outputs": [
-                {
-                    "links": [
-                        79,
-                        80
-                    ],
-                    "name": "MODEL",
-                    "slot_index": 0,
-                    "type": "MODEL"
-                },
-                {
-                    "links": [
-                        81,
-                        82
-                    ],
-                    "name": "CLIP",
-                    "slot_index": 1,
-                    "type": "CLIP"
-                },
-                {
-                    "links": [
-                        83
-                    ],
-                    "name": "VAE",
-                    "slot_index": 2,
-                    "type": "VAE"
-                }
-            ],
-            "pos": [
-                -71,
-                -471
-            ],
-            "properties": {
-                "Node name for S&R": "CheckpointLoaderSimple"
-            },
-            "size": {
-                "0": 315,
-                "1": 98
-            },
-            "title": "model_loader",
-            "type": "CheckpointLoaderSimple",
-            "widgets_values": [
-                "Deliberate.ckpt"
-            ]
-        },
-        {
-            "flags": {},
-            "id": 8,
-            "inputs": [
-                {
-                    "link": 91,
-                    "name": "samples",
-                    "type": "LATENT"
-                },
-                {
-                    "link": 83,
-                    "name": "vae",
-                    "type": "VAE"
-                }
-            ],
-            "mode": 0,
-            "order": 18,
-            "outputs": [
-                {
-                    "links": [
-                        9
-                    ],
-                    "name": "IMAGE",
-                    "slot_index": 0,
-                    "type": "IMAGE"
-                }
-            ],
-            "pos": [
-                1321,
-                -444
-            ],
-            "properties": {
-                "Node name for S&R": "VAEDecode"
-            },
-            "size": {
-                "0": 210,
-                "1": 46
-            },
-            "title": "vae_decode",
-            "type": "VAEDecode"
-        },
-        {
-            "flags": {},
             "id": 23,
             "inputs": [
                 {
                     "link": 77,
                     "name": "conditioning",
                     "type": "CONDITIONING"
                 },
                 {
                     "link": 47,
                     "name": "control_net",
                     "type": "CONTROL_NET"
                 },
                 {
-                    "link": 94,
+                    "link": 99,
                     "name": "image",
                     "type": "IMAGE"
                 }
             ],
             "mode": 0,
-            "order": 16,
+            "order": 15,
             "outputs": [
                 {
                     "links": [
                         40
                     ],
                     "name": "CONDITIONING",
                     "slot_index": 0,
@@ -486,15 +351,15 @@
                 {
                     "link": 80,
                     "name": "model",
                     "type": "MODEL"
                 }
             ],
             "mode": 0,
-            "order": 3,
+            "order": 12,
             "outputs": [
                 {
                     "links": [
                         47
                     ],
                     "name": "CONTROL_NET",
                     "slot_index": 0,
@@ -519,21 +384,21 @@
             ]
         },
         {
             "flags": {},
             "id": 9,
             "inputs": [
                 {
-                    "link": 9,
+                    "link": 98,
                     "name": "images",
                     "type": "IMAGE"
                 }
             ],
             "mode": 0,
-            "order": 19,
+            "order": 18,
             "pos": [
                 1528,
                 -270
             ],
             "properties": {},
             "size": {
                 "0": 542.196533203125,
@@ -545,15 +410,15 @@
                 "ComfyUI"
             ]
         },
         {
             "flags": {},
             "id": 20,
             "mode": 0,
-            "order": 2,
+            "order": 1,
             "outputs": [
                 {
                     "links": [
                         48,
                         52,
                         58,
                         61,
@@ -598,15 +463,15 @@
                 {
                     "link": 58,
                     "name": "image",
                     "type": "IMAGE"
                 }
             ],
             "mode": 0,
-            "order": 8,
+            "order": 5,
             "outputs": [
                 {
                     "links": [],
                     "name": "IMAGE",
                     "slot_index": 0,
                     "type": "IMAGE"
                 }
@@ -623,63 +488,24 @@
                 "1": 26
             },
             "title": "hed",
             "type": "HEDPreprocessor"
         },
         {
             "flags": {},
-            "id": 34,
-            "inputs": [
-                {
-                    "link": 48,
-                    "name": "image",
-                    "type": "IMAGE"
-                }
-            ],
-            "mode": 0,
-            "order": 6,
-            "outputs": [
-                {
-                    "links": [],
-                    "name": "IMAGE",
-                    "slot_index": 0,
-                    "type": "IMAGE"
-                }
-            ],
-            "pos": [
-                28,
-                380
-            ],
-            "properties": {
-                "Node name for S&R": "CannyEdgePreprocessor"
-            },
-            "size": {
-                "0": 210,
-                "1": 106
-            },
-            "title": "canny",
-            "type": "CannyEdgePreprocessor",
-            "widgets_values": [
-                100,
-                200,
-                "disable"
-            ]
-        },
-        {
-            "flags": {},
             "id": 37,
             "inputs": [
                 {
                     "link": 52,
                     "name": "image",
                     "type": "IMAGE"
                 }
             ],
             "mode": 0,
-            "order": 7,
+            "order": 4,
             "outputs": [
                 {
                     "links": [],
                     "name": "IMAGE",
                     "slot_index": 0,
                     "type": "IMAGE"
                 }
@@ -709,15 +535,15 @@
                 {
                     "link": 61,
                     "name": "image",
                     "type": "IMAGE"
                 }
             ],
             "mode": 0,
-            "order": 9,
+            "order": 6,
             "outputs": [
                 {
                     "links": [],
                     "name": "IMAGE",
                     "slot_index": 0,
                     "type": "IMAGE"
                 }
@@ -747,15 +573,15 @@
                 {
                     "link": 66,
                     "name": "image",
                     "type": "IMAGE"
                 }
             ],
             "mode": 0,
-            "order": 10,
+            "order": 7,
             "outputs": [
                 {
                     "links": [],
                     "name": "IMAGE",
                     "slot_index": 0,
                     "type": "IMAGE"
                 }
@@ -784,15 +610,15 @@
                 {
                     "link": 68,
                     "name": "image",
                     "type": "IMAGE"
                 }
             ],
             "mode": 0,
-            "order": 11,
+            "order": 8,
             "outputs": [
                 {
                     "links": [],
                     "name": "IMAGE",
                     "slot_index": 0,
                     "type": "IMAGE"
                 }
@@ -818,15 +644,15 @@
                 {
                     "link": 70,
                     "name": "image",
                     "type": "IMAGE"
                 }
             ],
             "mode": 0,
-            "order": 12,
+            "order": 9,
             "outputs": [
                 {
                     "links": [],
                     "name": "IMAGE",
                     "slot_index": 0,
                     "type": "IMAGE"
                 }
@@ -852,20 +678,18 @@
                 {
                     "link": 72,
                     "name": "image",
                     "type": "IMAGE"
                 }
             ],
             "mode": 0,
-            "order": 13,
+            "order": 10,
             "outputs": [
                 {
-                    "links": [
-                        95
-                    ],
+                    "links": [],
                     "name": "IMAGE",
                     "slot_index": 0,
                     "type": "IMAGE"
                 }
             ],
             "pos": [
                 39,
@@ -888,15 +712,15 @@
                 {
                     "link": 74,
                     "name": "image",
                     "type": "IMAGE"
                 }
             ],
             "mode": 0,
-            "order": 14,
+            "order": 11,
             "outputs": [
                 {
                     "links": [],
                     "name": "IMAGE",
                     "slot_index": 0,
                     "type": "IMAGE"
                 }
@@ -912,15 +736,65 @@
                 "0": 210,
                 "1": 82
             },
             "title": "mlsd",
             "type": "M-LSDPreprocessor",
             "widgets_values": [
                 0.15,
-                1.0
+                1
+            ]
+        },
+        {
+            "flags": {},
+            "id": 47,
+            "mode": 0,
+            "order": 2,
+            "outputs": [
+                {
+                    "links": [
+                        79,
+                        80
+                    ],
+                    "name": "MODEL",
+                    "slot_index": 0,
+                    "type": "MODEL"
+                },
+                {
+                    "links": [
+                        81,
+                        82
+                    ],
+                    "name": "CLIP",
+                    "slot_index": 1,
+                    "type": "CLIP"
+                },
+                {
+                    "links": [
+                        96
+                    ],
+                    "name": "VAE",
+                    "slot_index": 2,
+                    "type": "VAE"
+                }
+            ],
+            "pos": [
+                -71,
+                -471
+            ],
+            "properties": {
+                "Node name for S&R": "CheckpointLoaderSimple"
+            },
+            "size": {
+                "0": 315,
+                "1": 98
+            },
+            "title": "model_loader",
+            "type": "CheckpointLoaderSimple",
+            "widgets_values": [
+                "Deliberate.ckpt"
             ]
         },
         {
             "flags": {},
             "id": 3,
             "inputs": [
                 {
@@ -941,19 +815,19 @@
                 {
                     "link": 2,
                     "name": "latent_image",
                     "type": "LATENT"
                 }
             ],
             "mode": 0,
-            "order": 17,
+            "order": 16,
             "outputs": [
                 {
                     "links": [
-                        91
+                        97
                     ],
                     "name": "LATENT",
                     "slot_index": 0,
                     "type": "LATENT"
                 }
             ],
             "pos": [
@@ -967,18 +841,100 @@
                 "0": 315,
                 "1": 262
             },
             "title": "sampler",
             "type": "KSampler",
             "widgets_values": [
                 123456789,
-                false,
+                "fixed",
                 25,
                 7.5,
                 "dpmpp_2m",
                 "karras",
                 1
             ]
+        },
+        {
+            "flags": {},
+            "id": 49,
+            "inputs": [
+                {
+                    "link": 97,
+                    "name": "samples",
+                    "type": "LATENT"
+                },
+                {
+                    "link": 96,
+                    "name": "vae",
+                    "type": "VAE"
+                }
+            ],
+            "mode": 0,
+            "order": 17,
+            "outputs": [
+                {
+                    "links": [
+                        98
+                    ],
+                    "name": "IMAGE",
+                    "slot_index": 0,
+                    "type": "IMAGE"
+                }
+            ],
+            "pos": [
+                1314,
+                -538
+            ],
+            "properties": {
+                "Node name for S&R": "VAEDecodeTiled"
+            },
+            "size": {
+                "0": 210,
+                "1": 46
+            },
+            "title": "vae_decode",
+            "type": "VAEDecodeTiled"
+        },
+        {
+            "flags": {},
+            "id": 34,
+            "inputs": [
+                {
+                    "link": 48,
+                    "name": "image",
+                    "type": "IMAGE"
+                }
+            ],
+            "mode": 0,
+            "order": 3,
+            "outputs": [
+                {
+                    "links": [
+                        99
+                    ],
+                    "name": "IMAGE",
+                    "slot_index": 0,
+                    "type": "IMAGE"
+                }
+            ],
+            "pos": [
+                28,
+                380
+            ],
+            "properties": {
+                "Node name for S&R": "CannyEdgePreprocessor"
+            },
+            "size": {
+                "0": 210,
+                "1": 106
+            },
+            "title": "canny",
+            "type": "CannyEdgePreprocessor",
+            "widgets_values": [
+                100,
+                200,
+                "disable"
+            ]
         }
     ],
     "version": 0.4
 }
```

### Comparing `hordelib-0.9.5/hordelib/pipeline_designs/pipeline_controlnet_annotator.json` & `hordelib-1.0.0/hordelib/pipeline_designs/pipeline_controlnet_annotator.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/pipeline_designs/pipeline_image_facefix.json` & `hordelib-1.0.0/hordelib/pipeline_designs/pipeline_image_facefix.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/pipeline_designs/pipeline_image_upscale.json` & `hordelib-1.0.0/hordelib/pipeline_designs/pipeline_image_upscale.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/pipeline_designs/pipeline_stable_diffusion.json` & `hordelib-1.0.0/hordelib/pipeline_designs/pipeline_stable_diffusion.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8338593678259871%*

 * *Differences: {"'last_link_id'": '21',*

 * * "'last_node_id'": '14',*

 * * "'links'": "{insert: [(9, [19, 4, 2, 14, 1, 'VAE']), (10, [20, 3, 0, 14, 0, 'LATENT']), (11, [21, "*

 * *            "14, 0, 9, 0, 'IMAGE'])], delete: [5, 4, 3]}",*

 * * "'nodes'": "{3: {'inputs': {0: {'link': 21}}}, 6: {'id': 11, 'type': 'LoadImage', 'pos': [66, "*

 * *            "755], 'size': {'1': 102}, 'order': 1, 'outputs': {0: {'name': 'IMAGE', 'type': "*

 * *            "'IMAGE', 'links': [15]}, insert: [(1, OrderedDict([('name', 'MASK'), ('type', "*

 * *            "'MASK […]*

```diff
@@ -1,13 +1,13 @@
 {
     "config": {},
     "extra": {},
     "groups": [],
-    "last_link_id": 18,
-    "last_node_id": 13,
+    "last_link_id": 21,
+    "last_node_id": 14,
     "links": [
         [
             1,
             4,
             0,
             3,
             0,
@@ -26,38 +26,14 @@
             7,
             0,
             3,
             2,
             "CONDITIONING"
         ],
         [
-            7,
-            3,
-            0,
-            8,
-            0,
-            "LATENT"
-        ],
-        [
-            8,
-            4,
-            2,
-            8,
-            1,
-            "VAE"
-        ],
-        [
-            9,
-            8,
-            0,
-            9,
-            0,
-            "IMAGE"
-        ],
-        [
             11,
             10,
             0,
             6,
             0,
             "CLIP"
         ],
@@ -96,60 +72,43 @@
         [
             18,
             5,
             0,
             3,
             3,
             "LATENT"
+        ],
+        [
+            19,
+            4,
+            2,
+            14,
+            1,
+            "VAE"
+        ],
+        [
+            20,
+            3,
+            0,
+            14,
+            0,
+            "LATENT"
+        ],
+        [
+            21,
+            14,
+            0,
+            9,
+            0,
+            "IMAGE"
         ]
     ],
     "nodes": [
         {
             "flags": {},
-            "id": 8,
-            "inputs": [
-                {
-                    "link": 7,
-                    "name": "samples",
-                    "type": "LATENT"
-                },
-                {
-                    "link": 8,
-                    "name": "vae",
-                    "type": "VAE"
-                }
-            ],
-            "mode": 0,
-            "order": 8,
-            "outputs": [
-                {
-                    "links": [
-                        9
-                    ],
-                    "name": "IMAGE",
-                    "slot_index": 0,
-                    "type": "IMAGE"
-                }
-            ],
-            "pos": [
-                1384,
-                398
-            ],
-            "properties": {
-                "Node name for S&R": "VAEDecode"
-            },
-            "size": {
-                "0": 210,
-                "1": 46
-            },
-            "title": "vae_decode",
-            "type": "VAEDecode"
-        },
-        {
-            "flags": {},
             "id": 7,
             "inputs": [
                 {
                     "link": 13,
                     "name": "clip",
                     "slot_index": 0,
                     "type": "CLIP"
@@ -264,15 +223,15 @@
             ]
         },
         {
             "flags": {},
             "id": 9,
             "inputs": [
                 {
-                    "link": 9,
+                    "link": 21,
                     "name": "images",
                     "type": "IMAGE"
                 }
             ],
             "mode": 0,
             "order": 9,
             "pos": [
@@ -361,77 +320,55 @@
                 512,
                 512,
                 1
             ]
         },
         {
             "flags": {},
-            "id": 3,
-            "inputs": [
-                {
-                    "link": 1,
-                    "name": "model",
-                    "type": "MODEL"
-                },
-                {
-                    "link": 4,
-                    "name": "positive",
-                    "type": "CONDITIONING"
-                },
-                {
-                    "link": 6,
-                    "name": "negative",
-                    "type": "CONDITIONING"
-                },
-                {
-                    "link": 18,
-                    "name": "latent_image",
-                    "type": "LATENT"
-                }
-            ],
+            "id": 11,
             "mode": 0,
-            "order": 7,
+            "order": 1,
             "outputs": [
                 {
                     "links": [
-                        7
+                        15
                     ],
-                    "name": "LATENT",
+                    "name": "IMAGE",
                     "slot_index": 0,
-                    "type": "LATENT"
+                    "type": "IMAGE"
+                },
+                {
+                    "links": null,
+                    "name": "MASK",
+                    "type": "MASK"
                 }
             ],
             "pos": [
-                1019,
-                107
+                66,
+                755
             ],
             "properties": {
-                "Node name for S&R": "KSampler"
+                "Node name for S&R": "LoadImage"
             },
             "size": {
                 "0": 315,
-                "1": 262
+                "1": 102
             },
-            "title": "sampler",
-            "type": "KSampler",
+            "title": "image_loader",
+            "type": "LoadImage",
             "widgets_values": [
-                843159458049729,
-                true,
-                20,
-                8,
-                "euler",
-                "normal",
-                1
+                "example.png",
+                "image"
             ]
         },
         {
             "flags": {},
             "id": 4,
             "mode": 0,
-            "order": 1,
+            "order": 2,
             "outputs": [
                 {
                     "links": [
                         1
                     ],
                     "name": "MODEL",
                     "slot_index": 0,
@@ -443,16 +380,16 @@
                     ],
                     "name": "CLIP",
                     "slot_index": 1,
                     "type": "CLIP"
                 },
                 {
                     "links": [
-                        8,
-                        14
+                        14,
+                        19
                     ],
                     "name": "VAE",
                     "slot_index": 2,
                     "type": "VAE"
                 }
             ],
             "pos": [
@@ -470,46 +407,109 @@
             "type": "CheckpointLoaderSimple",
             "widgets_values": [
                 "Deliberate.ckpt"
             ]
         },
         {
             "flags": {},
-            "id": 11,
+            "id": 3,
+            "inputs": [
+                {
+                    "link": 1,
+                    "name": "model",
+                    "type": "MODEL"
+                },
+                {
+                    "link": 4,
+                    "name": "positive",
+                    "type": "CONDITIONING"
+                },
+                {
+                    "link": 6,
+                    "name": "negative",
+                    "type": "CONDITIONING"
+                },
+                {
+                    "link": 18,
+                    "name": "latent_image",
+                    "type": "LATENT"
+                }
+            ],
             "mode": 0,
-            "order": 2,
+            "order": 7,
             "outputs": [
                 {
                     "links": [
-                        15
+                        20
                     ],
-                    "name": "IMAGE",
+                    "name": "LATENT",
                     "slot_index": 0,
-                    "type": "IMAGE"
-                },
-                {
-                    "links": null,
-                    "name": "MASK",
-                    "type": "MASK"
+                    "type": "LATENT"
                 }
             ],
             "pos": [
-                66,
-                755
+                1019,
+                107
             ],
             "properties": {
-                "Node name for S&R": "LoadImage"
+                "Node name for S&R": "KSampler"
             },
             "size": {
                 "0": 315,
-                "1": 102
+                "1": 262
             },
-            "title": "image_loader",
-            "type": "LoadImage",
+            "title": "sampler",
+            "type": "KSampler",
             "widgets_values": [
-                "example.png",
-                "image"
+                62706718437716,
+                "randomize",
+                20,
+                8,
+                "euler",
+                "normal",
+                1
             ]
+        },
+        {
+            "flags": {},
+            "id": 14,
+            "inputs": [
+                {
+                    "link": 20,
+                    "name": "samples",
+                    "type": "LATENT"
+                },
+                {
+                    "link": 19,
+                    "name": "vae",
+                    "type": "VAE"
+                }
+            ],
+            "mode": 0,
+            "order": 8,
+            "outputs": [
+                {
+                    "links": [
+                        21
+                    ],
+                    "name": "IMAGE",
+                    "slot_index": 0,
+                    "type": "IMAGE"
+                }
+            ],
+            "pos": [
+                1370,
+                527
+            ],
+            "properties": {
+                "Node name for S&R": "VAEDecodeTiled"
+            },
+            "size": {
+                "0": 210,
+                "1": 46
+            },
+            "title": "vae_decode",
+            "type": "VAEDecodeTiled"
         }
     ],
     "version": 0.4
 }
```

### Comparing `hordelib-0.9.5/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json` & `hordelib-1.0.0/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8388301702304106%*

 * *Differences: {"'last_link_id'": '34',*

 * * "'last_node_id'": '21',*

 * * "'links'": "{insert: [(14, [32, 16, 2, 21, 1, 'VAE']), (15, [33, 11, 0, 21, 0, 'LATENT']), (16, "*

 * *            "[34, 21, 0, 12, 0, 'IMAGE'])], delete: [9, 7, 6]}",*

 * * "'nodes'": "{0: {'inputs': {0: {'link': 34}}}, 5: {'id': 18, 'type': 'LoadImage', 'pos': [261, "*

 * *            "934], 'size': {'1': 102}, 'outputs': {0: {'name': 'IMAGE', 'type': 'IMAGE', 'links': "*

 * *            "[27]}, 1: {'name': 'MASK', 'type': 'MASK', 'links': None, delete: ['slot_index']}, "*

 * *   […]*

```diff
@@ -39,16 +39,16 @@
                 1201,
                 352
             ],
             "color": "#3f789e",
             "title": "img2img"
         }
     ],
-    "last_link_id": 31,
-    "last_node_id": 20,
+    "last_link_id": 34,
+    "last_node_id": 21,
     "links": [
         [
             4,
             6,
             0,
             3,
             1,
@@ -91,46 +91,22 @@
             10,
             0,
             11,
             3,
             "LATENT"
         ],
         [
-            15,
-            11,
-            0,
-            13,
-            0,
-            "LATENT"
-        ],
-        [
-            17,
-            13,
-            0,
-            12,
-            0,
-            "IMAGE"
-        ],
-        [
             18,
             16,
             0,
             3,
             0,
             "MODEL"
         ],
         [
-            22,
-            16,
-            2,
-            13,
-            1,
-            "VAE"
-        ],
-        [
             23,
             16,
             0,
             11,
             0,
             "MODEL"
         ],
@@ -177,64 +153,47 @@
         [
             31,
             5,
             0,
             3,
             3,
             "LATENT"
+        ],
+        [
+            32,
+            16,
+            2,
+            21,
+            1,
+            "VAE"
+        ],
+        [
+            33,
+            11,
+            0,
+            21,
+            0,
+            "LATENT"
+        ],
+        [
+            34,
+            21,
+            0,
+            12,
+            0,
+            "IMAGE"
         ]
     ],
     "nodes": [
         {
             "flags": {},
-            "id": 13,
-            "inputs": [
-                {
-                    "link": 15,
-                    "name": "samples",
-                    "type": "LATENT"
-                },
-                {
-                    "link": 22,
-                    "name": "vae",
-                    "type": "VAE"
-                }
-            ],
-            "mode": 0,
-            "order": 10,
-            "outputs": [
-                {
-                    "links": [
-                        17
-                    ],
-                    "name": "IMAGE",
-                    "slot_index": 0,
-                    "type": "IMAGE"
-                }
-            ],
-            "pos": [
-                1961,
-                125
-            ],
-            "properties": {
-                "Node name for S&R": "VAEDecode"
-            },
-            "size": {
-                "0": 210,
-                "1": 46
-            },
-            "title": "vae_decoder",
-            "type": "VAEDecode"
-        },
-        {
-            "flags": {},
             "id": 12,
             "inputs": [
                 {
-                    "link": 17,
+                    "link": 34,
                     "name": "images",
                     "type": "IMAGE"
                 }
             ],
             "mode": 0,
             "order": 11,
             "pos": [
@@ -412,293 +371,334 @@
                 512,
                 512,
                 "disabled"
             ]
         },
         {
             "flags": {},
-            "id": 16,
+            "id": 18,
             "mode": 0,
             "order": 0,
             "outputs": [
                 {
                     "links": [
-                        18,
-                        23
+                        27
                     ],
-                    "name": "MODEL",
+                    "name": "IMAGE",
                     "slot_index": 0,
-                    "type": "MODEL"
-                },
-                {
-                    "links": [
-                        24
-                    ],
-                    "name": "CLIP",
-                    "slot_index": 1,
-                    "type": "CLIP"
+                    "type": "IMAGE"
                 },
                 {
-                    "links": [
-                        22,
-                        28
-                    ],
-                    "name": "VAE",
-                    "slot_index": 2,
-                    "type": "VAE"
+                    "links": null,
+                    "name": "MASK",
+                    "type": "MASK"
                 }
             ],
             "pos": [
-                -420,
-                334
+                261,
+                934
             ],
             "properties": {
-                "Node name for S&R": "CheckpointLoaderSimple"
+                "Node name for S&R": "LoadImage"
             },
             "size": {
                 "0": 315,
-                "1": 98
+                "1": 102
             },
-            "title": "model_loader",
-            "type": "CheckpointLoaderSimple",
+            "title": "image_loader",
+            "type": "LoadImage",
             "widgets_values": [
-                "Deliberate.ckpt"
+                "example.png",
+                "image"
             ]
         },
         {
             "flags": {},
-            "id": 18,
+            "id": 5,
             "mode": 0,
             "order": 1,
             "outputs": [
                 {
                     "links": [
-                        27
+                        31
                     ],
-                    "name": "IMAGE",
+                    "name": "LATENT",
                     "slot_index": 0,
-                    "type": "IMAGE"
-                },
-                {
-                    "links": null,
-                    "name": "MASK",
-                    "type": "MASK"
+                    "type": "LATENT"
                 }
             ],
             "pos": [
-                261,
-                934
+                473,
+                625
             ],
             "properties": {
-                "Node name for S&R": "LoadImage"
+                "Node name for S&R": "EmptyLatentImage"
             },
             "size": {
                 "0": 315,
-                "1": 102
+                "1": 106
             },
-            "title": "image_loader",
-            "type": "LoadImage",
+            "title": "empty_latent_image",
+            "type": "EmptyLatentImage",
             "widgets_values": [
-                "example.png",
-                "image"
+                256,
+                256,
+                1
             ]
         },
         {
             "flags": {},
-            "id": 11,
+            "id": 3,
             "inputs": [
                 {
-                    "link": 23,
+                    "link": 18,
                     "name": "model",
-                    "slot_index": 0,
                     "type": "MODEL"
                 },
                 {
-                    "link": 12,
+                    "link": 4,
                     "name": "positive",
-                    "slot_index": 1,
                     "type": "CONDITIONING"
                 },
                 {
-                    "link": 13,
+                    "link": 6,
                     "name": "negative",
-                    "slot_index": 2,
                     "type": "CONDITIONING"
                 },
                 {
-                    "link": 14,
+                    "link": 31,
                     "name": "latent_image",
-                    "slot_index": 3,
                     "type": "LATENT"
                 }
             ],
             "mode": 0,
-            "order": 9,
+            "order": 7,
             "outputs": [
                 {
                     "links": [
-                        15
+                        10
                     ],
                     "name": "LATENT",
                     "slot_index": 0,
                     "type": "LATENT"
                 }
             ],
             "pos": [
-                1585,
-                114
+                845,
+                172
             ],
             "properties": {
                 "Node name for S&R": "KSampler"
             },
             "size": {
                 "0": 315,
                 "1": 262
             },
-            "title": "upscale_sampler",
+            "title": "sampler",
             "type": "KSampler",
             "widgets_values": [
-                347776641452924,
-                true,
-                14,
+                458841867575267,
+                "randomize",
+                12,
                 8,
-                "dpmpp_2m",
-                "simple",
-                0.5
+                "dpmpp_sde",
+                "normal",
+                1
             ]
         },
         {
             "flags": {},
-            "id": 5,
+            "id": 19,
+            "inputs": [
+                {
+                    "link": 27,
+                    "name": "pixels",
+                    "type": "IMAGE"
+                },
+                {
+                    "link": 28,
+                    "name": "vae",
+                    "type": "VAE"
+                }
+            ],
+            "mode": 0,
+            "order": 4,
+            "outputs": [
+                {
+                    "links": [],
+                    "name": "LATENT",
+                    "slot_index": 0,
+                    "type": "LATENT"
+                }
+            ],
+            "pos": [
+                581,
+                799
+            ],
+            "properties": {
+                "Node name for S&R": "VAEEncode"
+            },
+            "size": {
+                "0": 210,
+                "1": 46
+            },
+            "title": "vae_encode",
+            "type": "VAEEncode"
+        },
+        {
+            "flags": {},
+            "id": 16,
             "mode": 0,
             "order": 2,
             "outputs": [
                 {
                     "links": [
-                        31
+                        18,
+                        23
                     ],
-                    "name": "LATENT",
+                    "name": "MODEL",
                     "slot_index": 0,
-                    "type": "LATENT"
+                    "type": "MODEL"
+                },
+                {
+                    "links": [
+                        24
+                    ],
+                    "name": "CLIP",
+                    "slot_index": 1,
+                    "type": "CLIP"
+                },
+                {
+                    "links": [
+                        28,
+                        32
+                    ],
+                    "name": "VAE",
+                    "slot_index": 2,
+                    "type": "VAE"
                 }
             ],
             "pos": [
-                473,
-                625
+                -420,
+                334
             ],
             "properties": {
-                "Node name for S&R": "EmptyLatentImage"
+                "Node name for S&R": "CheckpointLoaderSimple"
             },
             "size": {
                 "0": 315,
-                "1": 106
+                "1": 98
             },
-            "title": "empty_latent_image",
-            "type": "EmptyLatentImage",
+            "title": "model_loader",
+            "type": "CheckpointLoaderSimple",
             "widgets_values": [
-                256,
-                256,
-                1
+                "Deliberate.ckpt"
             ]
         },
         {
             "flags": {},
-            "id": 3,
+            "id": 11,
             "inputs": [
                 {
-                    "link": 18,
+                    "link": 23,
                     "name": "model",
+                    "slot_index": 0,
                     "type": "MODEL"
                 },
                 {
-                    "link": 4,
+                    "link": 12,
                     "name": "positive",
+                    "slot_index": 1,
                     "type": "CONDITIONING"
                 },
                 {
-                    "link": 6,
+                    "link": 13,
                     "name": "negative",
+                    "slot_index": 2,
                     "type": "CONDITIONING"
                 },
                 {
-                    "link": 31,
+                    "link": 14,
                     "name": "latent_image",
+                    "slot_index": 3,
                     "type": "LATENT"
                 }
             ],
             "mode": 0,
-            "order": 7,
+            "order": 9,
             "outputs": [
                 {
                     "links": [
-                        10
+                        33
                     ],
                     "name": "LATENT",
                     "slot_index": 0,
                     "type": "LATENT"
                 }
             ],
             "pos": [
-                845,
-                172
+                1585,
+                114
             ],
             "properties": {
                 "Node name for S&R": "KSampler"
             },
             "size": {
                 "0": 315,
                 "1": 262
             },
-            "title": "sampler",
+            "title": "upscale_sampler",
             "type": "KSampler",
             "widgets_values": [
-                1096039238624618,
-                true,
-                12,
+                65484213431324,
+                "randomize",
+                14,
                 8,
-                "dpmpp_sde",
-                "normal",
-                1
+                "dpmpp_2m",
+                "simple",
+                0.5
             ]
         },
         {
             "flags": {},
-            "id": 19,
+            "id": 21,
             "inputs": [
                 {
-                    "link": 27,
-                    "name": "pixels",
-                    "type": "IMAGE"
+                    "link": 33,
+                    "name": "samples",
+                    "type": "LATENT"
                 },
                 {
-                    "link": 28,
+                    "link": 32,
                     "name": "vae",
                     "type": "VAE"
                 }
             ],
             "mode": 0,
-            "order": 4,
+            "order": 10,
             "outputs": [
                 {
-                    "links": [],
-                    "name": "LATENT",
+                    "links": [
+                        34
+                    ],
+                    "name": "IMAGE",
                     "slot_index": 0,
-                    "type": "LATENT"
+                    "type": "IMAGE"
                 }
             ],
             "pos": [
-                581,
-                799
+                1963,
+                130
             ],
             "properties": {
-                "Node name for S&R": "VAEEncode"
+                "Node name for S&R": "VAEDecodeTiled"
             },
             "size": {
                 "0": 210,
                 "1": 46
             },
-            "title": "vae_encode",
-            "type": "VAEEncode"
+            "title": "vae_decode",
+            "type": "VAEDecodeTiled"
         }
     ],
     "version": 0.4
 }
```

### Comparing `hordelib-0.9.5/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json` & `hordelib-1.0.0/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8334772619662534%*

 * *Differences: {"'last_link_id'": '24',*

 * * "'last_node_id'": '15',*

 * * "'links'": "{insert: [(10, [22, 4, 2, 15, 1, 'VAE']), (11, [23, 3, 0, 15, 0, 'LATENT']), (12, "*

 * *            "[24, 15, 0, 9, 0, 'IMAGE'])], delete: [5, 4, 3]}",*

 * * "'nodes'": "{3: {'inputs': {0: {'link': 24}}}, 6: {'id': 14, 'type': 'VAEEncodeForInpaint', "*

 * *            "'pos': [515, 758], 'size': {'0': 210, '1': 66}, 'order': 4, 'inputs': {0: {'name': "*

 * *            "'pixels', 'type': 'IMAGE', 'link': 21}, 1: {'name': 'vae', 'type': 'VAE', 'link': "*

 * *            […]*

```diff
@@ -1,13 +1,13 @@
 {
     "config": {},
     "extra": {},
     "groups": [],
-    "last_link_id": 21,
-    "last_node_id": 14,
+    "last_link_id": 24,
+    "last_node_id": 15,
     "links": [
         [
             1,
             4,
             0,
             3,
             0,
@@ -26,38 +26,14 @@
             7,
             0,
             3,
             2,
             "CONDITIONING"
         ],
         [
-            7,
-            3,
-            0,
-            8,
-            0,
-            "LATENT"
-        ],
-        [
-            8,
-            4,
-            2,
-            8,
-            1,
-            "VAE"
-        ],
-        [
-            9,
-            8,
-            0,
-            9,
-            0,
-            "IMAGE"
-        ],
-        [
             11,
             10,
             0,
             6,
             0,
             "CLIP"
         ],
@@ -104,60 +80,43 @@
         [
             21,
             11,
             0,
             14,
             0,
             "IMAGE"
+        ],
+        [
+            22,
+            4,
+            2,
+            15,
+            1,
+            "VAE"
+        ],
+        [
+            23,
+            3,
+            0,
+            15,
+            0,
+            "LATENT"
+        ],
+        [
+            24,
+            15,
+            0,
+            9,
+            0,
+            "IMAGE"
         ]
     ],
     "nodes": [
         {
             "flags": {},
-            "id": 8,
-            "inputs": [
-                {
-                    "link": 7,
-                    "name": "samples",
-                    "type": "LATENT"
-                },
-                {
-                    "link": 8,
-                    "name": "vae",
-                    "type": "VAE"
-                }
-            ],
-            "mode": 0,
-            "order": 8,
-            "outputs": [
-                {
-                    "links": [
-                        9
-                    ],
-                    "name": "IMAGE",
-                    "slot_index": 0,
-                    "type": "IMAGE"
-                }
-            ],
-            "pos": [
-                1384,
-                398
-            ],
-            "properties": {
-                "Node name for S&R": "VAEDecode"
-            },
-            "size": {
-                "0": 210,
-                "1": 46
-            },
-            "title": "vae_decode",
-            "type": "VAEDecode"
-        },
-        {
-            "flags": {},
             "id": 7,
             "inputs": [
                 {
                     "link": 13,
                     "name": "clip",
                     "slot_index": 0,
                     "type": "CLIP"
@@ -272,15 +231,15 @@
             ]
         },
         {
             "flags": {},
             "id": 9,
             "inputs": [
                 {
-                    "link": 9,
+                    "link": 24,
                     "name": "images",
                     "type": "IMAGE"
                 }
             ],
             "mode": 0,
             "order": 9,
             "pos": [
@@ -330,77 +289,101 @@
                 512,
                 512,
                 1
             ]
         },
         {
             "flags": {},
-            "id": 3,
-            "inputs": [
+            "id": 11,
+            "mode": 0,
+            "order": 1,
+            "outputs": [
                 {
-                    "link": 1,
-                    "name": "model",
-                    "type": "MODEL"
+                    "links": [
+                        21
+                    ],
+                    "name": "IMAGE",
+                    "slot_index": 0,
+                    "type": "IMAGE"
                 },
                 {
-                    "link": 4,
-                    "name": "positive",
-                    "type": "CONDITIONING"
+                    "links": [
+                        19
+                    ],
+                    "name": "MASK",
+                    "slot_index": 1,
+                    "type": "MASK"
+                }
+            ],
+            "pos": [
+                66,
+                755
+            ],
+            "properties": {
+                "Node name for S&R": "LoadImage"
+            },
+            "size": {
+                "0": 315,
+                "1": 102
+            },
+            "title": "image_loader",
+            "type": "LoadImage",
+            "widgets_values": [
+                "example.png",
+                "image"
+            ]
+        },
+        {
+            "flags": {},
+            "id": 14,
+            "inputs": [
+                {
+                    "link": 21,
+                    "name": "pixels",
+                    "type": "IMAGE"
                 },
                 {
-                    "link": 6,
-                    "name": "negative",
-                    "type": "CONDITIONING"
+                    "link": 20,
+                    "name": "vae",
+                    "type": "VAE"
                 },
                 {
-                    "link": 18,
-                    "name": "latent_image",
-                    "type": "LATENT"
+                    "link": 19,
+                    "name": "mask",
+                    "type": "MASK"
                 }
             ],
             "mode": 0,
-            "order": 7,
+            "order": 4,
             "outputs": [
                 {
-                    "links": [
-                        7
-                    ],
+                    "links": null,
                     "name": "LATENT",
-                    "slot_index": 0,
                     "type": "LATENT"
                 }
             ],
             "pos": [
-                1019,
-                107
+                515,
+                758
             ],
             "properties": {
-                "Node name for S&R": "KSampler"
+                "Node name for S&R": "VAEEncodeForInpaint"
             },
             "size": {
-                "0": 315,
-                "1": 262
+                "0": 210,
+                "1": 66
             },
-            "title": "sampler",
-            "type": "KSampler",
-            "widgets_values": [
-                843159458049729,
-                true,
-                20,
-                8,
-                "euler",
-                "normal",
-                1
-            ]
+            "title": "vae_encode",
+            "type": "VAEEncodeForInpaint"
         },
         {
             "flags": {},
             "id": 4,
             "mode": 0,
-            "order": 1,
+            "order": 2,
             "outputs": [
                 {
                     "links": [
                         1
                     ],
                     "name": "MODEL",
                     "slot_index": 0,
@@ -412,16 +395,16 @@
                     ],
                     "name": "CLIP",
                     "slot_index": 1,
                     "type": "CLIP"
                 },
                 {
                     "links": [
-                        8,
-                        20
+                        20,
+                        22
                     ],
                     "name": "VAE",
                     "slot_index": 2,
                     "type": "VAE"
                 }
             ],
             "pos": [
@@ -439,92 +422,108 @@
             "type": "CheckpointLoaderSimple",
             "widgets_values": [
                 "Deliberate.ckpt"
             ]
         },
         {
             "flags": {},
-            "id": 11,
+            "id": 3,
+            "inputs": [
+                {
+                    "link": 1,
+                    "name": "model",
+                    "type": "MODEL"
+                },
+                {
+                    "link": 4,
+                    "name": "positive",
+                    "type": "CONDITIONING"
+                },
+                {
+                    "link": 6,
+                    "name": "negative",
+                    "type": "CONDITIONING"
+                },
+                {
+                    "link": 18,
+                    "name": "latent_image",
+                    "type": "LATENT"
+                }
+            ],
             "mode": 0,
-            "order": 2,
+            "order": 7,
             "outputs": [
                 {
                     "links": [
-                        21
+                        23
                     ],
-                    "name": "IMAGE",
+                    "name": "LATENT",
                     "slot_index": 0,
-                    "type": "IMAGE"
-                },
-                {
-                    "links": [
-                        19
-                    ],
-                    "name": "MASK",
-                    "slot_index": 1,
-                    "type": "MASK"
+                    "type": "LATENT"
                 }
             ],
             "pos": [
-                66,
-                755
+                1019,
+                107
             ],
             "properties": {
-                "Node name for S&R": "LoadImage"
+                "Node name for S&R": "KSampler"
             },
             "size": {
                 "0": 315,
-                "1": 102
+                "1": 262
             },
-            "title": "image_loader",
-            "type": "LoadImage",
+            "title": "sampler",
+            "type": "KSampler",
             "widgets_values": [
-                "example.png",
-                "image"
+                1042448765519873,
+                "randomize",
+                20,
+                8,
+                "euler",
+                "normal",
+                1
             ]
         },
         {
             "flags": {},
-            "id": 14,
+            "id": 15,
             "inputs": [
                 {
-                    "link": 21,
-                    "name": "pixels",
-                    "type": "IMAGE"
+                    "link": 23,
+                    "name": "samples",
+                    "type": "LATENT"
                 },
                 {
-                    "link": 20,
+                    "link": 22,
                     "name": "vae",
                     "type": "VAE"
-                },
-                {
-                    "link": 19,
-                    "name": "mask",
-                    "type": "MASK"
                 }
             ],
             "mode": 0,
-            "order": 4,
+            "order": 8,
             "outputs": [
                 {
-                    "links": null,
-                    "name": "LATENT",
-                    "type": "LATENT"
+                    "links": [
+                        24
+                    ],
+                    "name": "IMAGE",
+                    "slot_index": 0,
+                    "type": "IMAGE"
                 }
             ],
             "pos": [
-                515,
-                758
+                1370,
+                471
             ],
             "properties": {
-                "Node name for S&R": "VAEEncodeForInpaint"
+                "Node name for S&R": "VAEDecodeTiled"
             },
             "size": {
                 "0": 210,
-                "1": 66
+                "1": 46
             },
-            "title": "vae_encode",
-            "type": "VAEEncodeForInpaint"
+            "type": "VAEDecodeTiled"
         }
     ],
     "version": 0.4
 }
```

### Comparing `hordelib-0.9.5/hordelib/pipelines/pipeline_controlnet.json` & `hordelib-1.0.0/hordelib/pipelines/pipeline_controlnet.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8984375%*

 * *Differences: {"'23'": "{'inputs': {'image': {insert: [(0, '34')], delete: [0]}}}",*

 * * "'49'": "OrderedDict([('inputs', OrderedDict([('samples', ['3', 0]), ('vae', ['47', 2])])), "*

 * *         "('class_type', 'VAEDecodeTiled')])",*

 * * "'9'": "{'inputs': {'images': {insert: [(0, '49')], delete: [0]}}}",*

 * * 'delete': "['8']"}*

```diff
@@ -14,15 +14,15 @@
                 0
             ],
             "control_net": [
                 "33",
                 0
             ],
             "image": [
-                "45",
+                "34",
                 0
             ],
             "strength": 0.8500000000000003
         }
     },
     "24": {
         "class_type": "CLIPTextEncode",
@@ -150,28 +150,41 @@
                 0
             ]
         }
     },
     "46": {
         "class_type": "M-LSDPreprocessor",
         "inputs": {
-            "dist_threshold": 1.0,
+            "dist_threshold": 1,
             "image": [
                 "20",
                 0
             ],
             "score_threshold": 0.15
         }
     },
     "47": {
         "class_type": "CheckpointLoaderSimple",
         "inputs": {
             "ckpt_name": "Deliberate.ckpt"
         }
     },
+    "49": {
+        "class_type": "VAEDecodeTiled",
+        "inputs": {
+            "samples": [
+                "3",
+                0
+            ],
+            "vae": [
+                "47",
+                2
+            ]
+        }
+    },
     "5": {
         "class_type": "EmptyLatentImage",
         "inputs": {
             "batch_size": 1,
             "height": 512,
             "width": 512
         }
@@ -182,31 +195,18 @@
             "clip": [
                 "47",
                 1
             ],
             "text": ""
         }
     },
-    "8": {
-        "class_type": "VAEDecode",
-        "inputs": {
-            "samples": [
-                "3",
-                0
-            ],
-            "vae": [
-                "47",
-                2
-            ]
-        }
-    },
     "9": {
         "class_type": "SaveImage",
         "inputs": {
             "filename_prefix": "ComfyUI",
             "images": [
-                "8",
+                "49",
                 0
             ]
         }
     }
 }
```

### Comparing `hordelib-0.9.5/hordelib/pipelines/pipeline_controlnet_annotator.json` & `hordelib-1.0.0/hordelib/pipelines/pipeline_controlnet_annotator.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/pipelines/pipeline_image_facefix.json` & `hordelib-1.0.0/hordelib/pipelines/pipeline_image_facefix.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/pipelines/pipeline_image_upscale.json` & `hordelib-1.0.0/hordelib/pipelines/pipeline_image_upscale.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/pipelines/pipeline_stable_diffusion.json` & `hordelib-1.0.0/hordelib/pipelines/pipeline_stable_diffusion.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8157196969696969%*

 * *Differences: {"'14'": "OrderedDict([('inputs', OrderedDict([('samples', ['3', 0]), ('vae', ['4', 2])])), "*

 * *         "('class_type', 'VAEDecodeTiled')])",*

 * * "'3'": "{'inputs': {'seed': 843159458049729}}",*

 * * "'9'": "{'inputs': {'images': {insert: [(0, '14')], delete: [0]}}}",*

 * * 'delete': "['8']"}*

```diff
@@ -25,14 +25,27 @@
             ],
             "vae": [
                 "4",
                 2
             ]
         }
     },
+    "14": {
+        "class_type": "VAEDecodeTiled",
+        "inputs": {
+            "samples": [
+                "3",
+                0
+            ],
+            "vae": [
+                "4",
+                2
+            ]
+        }
+    },
     "3": {
         "class_type": "KSampler",
         "inputs": {
             "cfg": 8.0,
             "denoise": 1.0,
             "latent_image": [
                 "5",
@@ -48,15 +61,15 @@
             ],
             "positive": [
                 "6",
                 0
             ],
             "sampler_name": "euler",
             "scheduler": "normal",
-            "seed": 549947196061527,
+            "seed": 843159458049729,
             "steps": 20
         }
     },
     "4": {
         "class_type": "CheckpointLoaderSimple",
         "inputs": {
             "ckpt_name": "Deliberate.ckpt"
@@ -86,31 +99,18 @@
             "clip": [
                 "10",
                 0
             ],
             "text": "painting, drawing, artwork"
         }
     },
-    "8": {
-        "class_type": "VAEDecode",
-        "inputs": {
-            "samples": [
-                "3",
-                0
-            ],
-            "vae": [
-                "4",
-                2
-            ]
-        }
-    },
     "9": {
         "class_type": "SaveImage",
         "inputs": {
             "filename_prefix": "ComfyUI",
             "images": [
-                "8",
+                "14",
                 0
             ]
         }
     }
 }
```

### Comparing `hordelib-0.9.5/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json` & `hordelib-1.0.0/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8435897435897437%*

 * *Differences: {"'11'": "{'inputs': {'seed': 347776641452924}}",*

 * * "'12'": "{'inputs': {'images': {insert: [(0, '21')], delete: [0]}}}",*

 * * "'21'": "OrderedDict([('inputs', OrderedDict([('samples', ['11', 0]), ('vae', ['16', 2])])), "*

 * *         "('class_type', 'VAEDecodeTiled')])",*

 * * "'3'": "{'inputs': {'seed': 1096039238624618}}",*

 * * 'delete': "['13']"}*

```diff
@@ -31,41 +31,28 @@
             ],
             "positive": [
                 "6",
                 0
             ],
             "sampler_name": "dpmpp_2m",
             "scheduler": "simple",
-            "seed": 1016912243210385,
+            "seed": 347776641452924,
             "steps": 14
         }
     },
     "12": {
         "class_type": "SaveImage",
         "inputs": {
             "filename_prefix": "ComfyUI",
             "images": [
-                "13",
+                "21",
                 0
             ]
         }
     },
-    "13": {
-        "class_type": "VAEDecode",
-        "inputs": {
-            "samples": [
-                "11",
-                0
-            ],
-            "vae": [
-                "16",
-                2
-            ]
-        }
-    },
     "16": {
         "class_type": "CheckpointLoaderSimple",
         "inputs": {
             "ckpt_name": "Deliberate.ckpt"
         }
     },
     "17": {
@@ -94,14 +81,27 @@
             ],
             "vae": [
                 "16",
                 2
             ]
         }
     },
+    "21": {
+        "class_type": "VAEDecodeTiled",
+        "inputs": {
+            "samples": [
+                "11",
+                0
+            ],
+            "vae": [
+                "16",
+                2
+            ]
+        }
+    },
     "3": {
         "class_type": "KSampler",
         "inputs": {
             "cfg": 8.0,
             "denoise": 1.0,
             "latent_image": [
                 "5",
@@ -117,15 +117,15 @@
             ],
             "positive": [
                 "6",
                 0
             ],
             "sampler_name": "dpmpp_sde",
             "scheduler": "normal",
-            "seed": 1094518095629290,
+            "seed": 1096039238624618,
             "steps": 12
         }
     },
     "5": {
         "class_type": "EmptyLatentImage",
         "inputs": {
             "batch_size": 1,
```

### Comparing `hordelib-0.9.5/hordelib/pipelines/pipeline_stable_diffusion_paint.json` & `hordelib-1.0.0/hordelib/pipelines/pipeline_stable_diffusion_paint.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8162878787878789%*

 * *Differences: {"'15'": "OrderedDict([('inputs', OrderedDict([('samples', ['3', 0]), ('vae', ['4', 2])])), "*

 * *         "('class_type', 'VAEDecodeTiled')])",*

 * * "'9'": "{'inputs': {'images': {insert: [(0, '15')], delete: [0]}}}",*

 * * 'delete': "['8']"}*

```diff
@@ -29,14 +29,27 @@
             ],
             "vae": [
                 "4",
                 2
             ]
         }
     },
+    "15": {
+        "class_type": "VAEDecodeTiled",
+        "inputs": {
+            "samples": [
+                "3",
+                0
+            ],
+            "vae": [
+                "4",
+                2
+            ]
+        }
+    },
     "3": {
         "class_type": "KSampler",
         "inputs": {
             "cfg": 8.0,
             "denoise": 1.0,
             "latent_image": [
                 "5",
@@ -90,31 +103,18 @@
             "clip": [
                 "10",
                 0
             ],
             "text": "painting, drawing, artwork"
         }
     },
-    "8": {
-        "class_type": "VAEDecode",
-        "inputs": {
-            "samples": [
-                "3",
-                0
-            ],
-            "vae": [
-                "4",
-                2
-            ]
-        }
-    },
     "9": {
         "class_type": "SaveImage",
         "inputs": {
             "filename_prefix": "ComfyUI",
             "images": [
-                "8",
+                "15",
                 0
             ]
         }
     }
 }
```

### Comparing `hordelib-0.9.5/hordelib/safety_checker.py` & `hordelib-1.0.0/hordelib/safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/utils/blip/blip.py` & `hordelib-1.0.0/hordelib/utils/blip/blip.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,9 +267,8 @@
         )
     for key in model.state_dict().keys():
         if key in state_dict.keys():
             if state_dict[key].shape != model.state_dict()[key].shape:
                 del state_dict[key]
 
     msg = model.load_state_dict(state_dict, strict=False)
-    print("load checkpoint from %s" % url_or_filename)
     return model, msg
```

### Comparing `hordelib-0.9.5/hordelib/utils/blip/med.py` & `hordelib-1.0.0/hordelib/utils/blip/med.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/utils/blip/vit.py` & `hordelib-1.0.0/hordelib/utils/blip/vit.py`

 * *Files 1% similar despite different names*

```diff
@@ -343,12 +343,11 @@
             pos_tokens,
             size=(new_size, new_size),
             mode="bicubic",
             align_corners=False,
         )
         pos_tokens = pos_tokens.permute(0, 2, 3, 1).flatten(1, 2)
         new_pos_embed = torch.cat((extra_tokens, pos_tokens), dim=1)
-        print("reshape position embedding from %d to %d" % (orig_size**2, new_size**2))
 
         return new_pos_embed
     else:
         return pos_embed_checkpoint
```

### Comparing `hordelib-0.9.5/hordelib/utils/cast.py` & `hordelib-1.0.0/hordelib/utils/cast.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/utils/ioredirect.py` & `hordelib-1.0.0/hordelib/utils/ioredirect.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/hordelib/utils/logger.py` & `hordelib-1.0.0/hordelib/utils/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,16 @@
     def initialise(cls, setup_logging=True):
         if setup_logging:
             cls.setup()
             cls.set_sinks()
         else:
             cls.setup_compatibility()
 
+        logger.disable("hordelib.clip.interrogate")
+
     @classmethod
     def setup_compatibility(cls):
         logger.__class__.generation = partialmethod(logger.__class__.log, "INFO")
         logger.__class__.prompt = partialmethod(logger.__class__.log, "INFO")
         logger.__class__.init = partialmethod(logger.__class__.log, "INFO")
         logger.__class__.init_ok = partialmethod(logger.__class__.log, "INFO")
         logger.__class__.init_warn = partialmethod(logger.__class__.log, "INFO")
```

### Comparing `hordelib-0.9.5/hordelib.egg-info/PKG-INFO` & `hordelib-1.0.0/hordelib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hordelib
-Version: 0.9.5
+Version: 1.0.0
 Summary: A thin wrapper around ComfyUI to allow use by AI Horde.
 Author-email: Jug <jugdev@proton.me>, db0 <mail@dbzer0.com>, tazlin <tazlin.on.github@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -682,21 +682,22 @@
 [![PyPI Version][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 ![GitHub license][license-url]
 
 [![Build][build-image]][build-url]
 [![Test Images][main-test-image]][main-test-url]
 [![Test Images][pr-test-image]][pr-test-url]
+[![All Models][all-model-images]][all-model-url]
 [![Release Changelog][changelog-image]][changelog-url]
 
-`hordelib` is a thin wrapper around [ComfyUI](https://github.com/comfyanonymous/ComfyUI) primarily to enable the [AI Horde](https://aihorde.net/) to run inference pipelines designed visually in the ComfyUI GUI.
+`hordelib` is a wrapper around [ComfyUI](https://github.com/comfyanonymous/ComfyUI) primarily to enable the [AI Horde](https://aihorde.net/) to run inference pipelines designed visually in the ComfyUI GUI.
 
 The developers of `hordelib` can be found in the AI Horde Discord server: [https://discord.gg/3DxrhksKzn](https://discord.gg/3DxrhksKzn)
 
-NOTE: This project is in development and is not yet in use by Stable Horde.
+`hordelib` has been the default inference backend library of the [AI Horde](https://aihorde.net/) since `hordelib` v1.0.0.
 
 ## Purpose
 
 The goal here is to be able to design inference pipelines in the excellent ComfyUI, and then call those inference pipelines programmatically. Whilst providing features that maintain compatibility with the existing horde implementation.
 
 ## Installation
 
@@ -830,15 +831,26 @@
 `hordelib/pipelines/`
 Contains the above pipeline JSON files converted to the format required by the backend pipeline processor. These are converted from the web app, see _Converting ComfyUI pipelines_ below.
 
 `hordelib/nodes/` These are the custom ComfyUI nodes we use for `hordelib` specific processing.
 
 ### Running ComfyUI Web Application
 
-`tox -e comfyui`
+In this example we install the dependencies in the OS default environment. When using the git version of `hordelib`, from the project root:
+
+`pip install -r requirements.txt --extra-index-url https://download.pytorch.org/whl/cu118 --upgrade`
+
+Ensure ComfyUI is installed and patched, one way is running the tests:
+
+`tox`
+
+From then on to run ComfyUI:
+
+`cd ComfyUI`
+`python main.py`
 
 Then open a browser at: http://127.0.0.1:8188/
 
 ### Designing ComfyUI Pipelines
 
 Use the standard ComfyUI web app. Use the "title" attribute to name the nodes, these names become parameter names in the `hordelib`. For example, a KSampler with the "title" of "sampler2" would become a parameter `sampler2.seed`, `sampler2.cfg`, etc. Load the pipeline `hordelib/pipeline_designs/pipeline_stable_diffusion.json` in the ComfyUI web app for an example.
 
@@ -867,15 +879,15 @@
 
 ### Standalone "clean" environment test from Pypi
 
 Here's an example:
 
 Start in a new empty directory. Create requirements.txt:
 ```
---extra-index-url https://download.pytorch.org/whl/cu117
+--extra-index-url https://download.pytorch.org/whl/cu118
 hordelib
 ```
 
 Create the directory `images/` and copy the `test_db0.jpg` into it.
 
 Copy `run_controlnet.py` from the `hordelib/tests/` directory.
 
@@ -926,14 +938,16 @@
 
 [pypi-image]: https://badge.fury.io/py/hordelib.svg?branch=main&kill_cache=1
 [pypi-url]: https://badge.fury.io/py/hordelib
 [downloads-image]: https://pepy.tech/badge/hordelib
 [downloads-url]: https://pepy.tech/project/hordelib
 [license-url]: https://img.shields.io/github/license/jug-dev/hordelib
 [build-image]: https://github.com/jug-dev/hordelib/actions/workflows/maintests.yml/badge.svg?branch=main
+[all-model-images]: https://badgen.net/badge/all-models/images/blue?icon=awesome
 [build-url]: http://hordelib.s3-website-eu-west-1.amazonaws.com/
 [main-test-image]: https://badgen.net/badge/main/latest-images/blue?icon=awesome
 [main-test-url]: http://hordelib.s3-website-eu-west-1.amazonaws.com/
 [pr-test-image]: https://badgen.net/badge/develop/latest-images/blue?icon=awesome
 [pr-test-url]: http://hordelib.s3-website-eu-west-1.amazonaws.com/unstable
+[all-model-url]: http://hordelib.s3-website-eu-west-1.amazonaws.com/all_models/
 [changelog-image]: https://img.shields.io/badge/Release-Changelog-yellow
 [changelog-url]: https://github.com/jug-dev/hordelib/blob/releases/CHANGELOG.md
```

### Comparing `hordelib-0.9.5/hordelib.egg-info/SOURCES.txt` & `hordelib-1.0.0/hordelib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,63 +9,81 @@
 pyproject.toml
 requirements.dev.txt
 requirements.txt
 tox.ini
 .github/workflows/maintests.yml
 .github/workflows/prtests.yml
 .github/workflows/release.yml
+examples/kudos.py
+examples/make_index.py
+examples/make_index_all_models.py
+examples/run_all_models.py
+examples/run_all_stress_tests.py
 examples/run_clip.py
 examples/run_controlnet.py
 examples/run_controlnet_annotator.py
 examples/run_facefix.py
 examples/run_img2img.py
 examples/run_img2img_hires.py
 examples/run_img2img_inpaint.py
 examples/run_img2img_inpaint_mask.py
 examples/run_img2img_outpaint.py
 examples/run_inpainting.py
+examples/run_kudos_test.py
 examples/run_memory_test.py
-examples/run_stress_test.py
+examples/run_stress_test_cnet.py
+examples/run_stress_test_cnet_preproc.py
+examples/run_stress_test_dynamic.py
+examples/run_stress_test_img2img.py
+examples/run_stress_test_mixed.py
+examples/run_stress_test_pp.py
+examples/run_stress_test_txt2img.py
+examples/run_stress_test_txt2img_hiresfix.py
 examples/run_txt2img.py
 examples/run_txt2img_hires.py
+examples/run_txt2img_local_model.py
 examples/run_upscale.py
 hordelib/__init__.py
 hordelib/_version.py
+hordelib/benchmark.py
 hordelib/comfy_horde.py
 hordelib/config_path.py
 hordelib/consts.py
 hordelib/horde.py
 hordelib/initialisation.py
 hordelib/install_comfy.patch
 hordelib/install_comfy.py
-hordelib/run_comfyui.py
+hordelib/preload.py
 hordelib/safety_checker.py
 hordelib/settings.py
 hordelib/shared_model_manager.py
+hordelib/train.py
 hordelib.egg-info/PKG-INFO
 hordelib.egg-info/SOURCES.txt
 hordelib.egg-info/dependency_links.txt
 hordelib.egg-info/requires.txt
 hordelib.egg-info/top_level.txt
 hordelib/_comfyui/.gitignore
 hordelib/_comfyui/LICENSE
 hordelib/_comfyui/README.md
 hordelib/_comfyui/comfyui_screenshot.png
 hordelib/_comfyui/execution.py
+hordelib/_comfyui/extra_model_paths.yaml
 hordelib/_comfyui/extra_model_paths.yaml.example
 hordelib/_comfyui/folder_paths.py
 hordelib/_comfyui/main.py
 hordelib/_comfyui/nodes.py
 hordelib/_comfyui/requirements.txt
 hordelib/_comfyui/server.py
 hordelib/_comfyui/comfy/cli_args.py
 hordelib/_comfyui/comfy/clip_vision.py
 hordelib/_comfyui/comfy/clip_vision_config_h.json
 hordelib/_comfyui/comfy/clip_vision_config_vitl.json
 hordelib/_comfyui/comfy/diffusers_convert.py
+hordelib/_comfyui/comfy/gligen.py
 hordelib/_comfyui/comfy/model_management.py
 hordelib/_comfyui/comfy/samplers.py
 hordelib/_comfyui/comfy/sd.py
 hordelib/_comfyui/comfy/sd1_clip.py
 hordelib/_comfyui/comfy/sd1_clip_config.json
 hordelib/_comfyui/comfy/sd2_clip.py
 hordelib/_comfyui/comfy/sd2_clip_config.json
@@ -190,28 +208,30 @@
 hordelib/_comfyui/models/configs/v2-inference-v_fp32.yaml
 hordelib/_comfyui/models/configs/v2-inference.yaml
 hordelib/_comfyui/models/configs/v2-inference_fp32.yaml
 hordelib/_comfyui/models/configs/v2-inpainting-inference.yaml
 hordelib/_comfyui/models/controlnet/put_controlnets_and_t2i_here
 hordelib/_comfyui/models/diffusers/put_diffusers_models_here
 hordelib/_comfyui/models/embeddings/put_embeddings_or_textual_inversion_concepts_here
+hordelib/_comfyui/models/gligen/put_gligen_models_here
 hordelib/_comfyui/models/loras/put_loras_here
 hordelib/_comfyui/models/style_models/put_t2i_style_model_here
 hordelib/_comfyui/models/upscale_models/put_esrgan_and_other_upscale_models_here
 hordelib/_comfyui/models/vae/put_vae_here
 hordelib/_comfyui/notebooks/comfyui_colab.ipynb
 hordelib/_comfyui/output/_output_images_will_be_put_here
 hordelib/_comfyui/script_examples/basic_api_example.py
 hordelib/_comfyui/web/index.html
 hordelib/_comfyui/web/jsconfig.json
 hordelib/_comfyui/web/style.css
 hordelib/_comfyui/web/extensions/logging.js.example
 hordelib/_comfyui/web/extensions/core/colorPalette.js
 hordelib/_comfyui/web/extensions/core/contextMenuFilter.js
 hordelib/_comfyui/web/extensions/core/dynamicPrompts.js
+hordelib/_comfyui/web/extensions/core/editAttention.js
 hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js
 hordelib/_comfyui/web/extensions/core/keybinds.js
 hordelib/_comfyui/web/extensions/core/nodeTemplates.js
 hordelib/_comfyui/web/extensions/core/noteNode.js
 hordelib/_comfyui/web/extensions/core/rerouteNode.js
 hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js
 hordelib/_comfyui/web/extensions/core/slotDefaults.js
@@ -278,15 +298,14 @@
 hordelib/nodes/node_image_output.py
 hordelib/nodes/node_model_loader.py
 hordelib/nodes/node_upscale_model_loader.py
 hordelib/nodes/comfy_controlnet_preprocessors/.gitignore
 hordelib/nodes/comfy_controlnet_preprocessors/LICENSE
 hordelib/nodes/comfy_controlnet_preprocessors/README.md
 hordelib/nodes/comfy_controlnet_preprocessors/__init__.py
-hordelib/nodes/comfy_controlnet_preprocessors/install.py
 hordelib/nodes/comfy_controlnet_preprocessors/requirements.txt
 hordelib/nodes/comfy_controlnet_preprocessors/util.py
 hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py
 hordelib/nodes/comfy_controlnet_preprocessors/canny/__init__.py
 hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py
 hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py
 hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py
@@ -692,28 +711,32 @@
 hordelib/nodes/facerestore/facelib/parsing/resnet.py
 hordelib/nodes/facerestore/facelib/utils/__init__.py
 hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py
 hordelib/nodes/facerestore/facelib/utils/face_utils.py
 hordelib/nodes/facerestore/facelib/utils/misc.py
 hordelib/pipeline_designs/pipeline_controlnet.json
 hordelib/pipeline_designs/pipeline_controlnet_annotator.json
+hordelib/pipeline_designs/pipeline_controlnet_hires_fix.json
 hordelib/pipeline_designs/pipeline_image_facefix.json
 hordelib/pipeline_designs/pipeline_image_upscale.json
 hordelib/pipeline_designs/pipeline_stable_diffusion.json
 hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json
 hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json
 hordelib/pipelines/pipeline_controlnet.json
 hordelib/pipelines/pipeline_controlnet_annotator.json
+hordelib/pipelines/pipeline_controlnet_hires_fix.json
 hordelib/pipelines/pipeline_image_facefix.json
 hordelib/pipelines/pipeline_image_upscale.json
 hordelib/pipelines/pipeline_stable_diffusion.json
 hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json
 hordelib/pipelines/pipeline_stable_diffusion_paint.json
 hordelib/utils/__init__.py
 hordelib/utils/cast.py
+hordelib/utils/dynamicprompt.py
+hordelib/utils/gpuinfo.py
 hordelib/utils/ioredirect.py
 hordelib/utils/logger.py
 hordelib/utils/switch.py
 hordelib/utils/blip/__init__.py
 hordelib/utils/blip/blip.py
 hordelib/utils/blip/med.py
 hordelib/utils/blip/vit.py
@@ -722,25 +745,30 @@
 images/test_facefix.png
 images/test_inpaint.png
 images/test_inpaint_alpha.png
 images/test_inpaint_mask.png
 images/test_inpaint_original.png
 images/test_outpaint.png
 tests/__init__.py
-tests/make_index.py
 tests/test_blip.py
 tests/test_clip.py
 tests/test_comfy.py
+tests/test_cuda.py
+tests/test_dynamic_prompt.py
 tests/test_horde_controlnet_annotator.py
 tests/test_horde_inference.py
 tests/test_horde_inference_controlnet.py
 tests/test_horde_inference_img2img.py
 tests/test_horde_inference_painting.py
 tests/test_horde_pp.py
+tests/test_horde_samplers.py
+tests/test_image_metadata.py
 tests/test_inference.py
 tests/test_initialisation.py
 tests/test_safety_checker.py
 tests/test_shared_model_manager.py
 tests/test_utils.py
+tests/meta/test_build_helper_import_check.py
+tests/model_managers/test_annotators.py
 tests/model_managers/test_comvis.py
 tests/model_managers/test_diffusers.py
 tests/model_managers/test_safety_checker.py
```

### Comparing `hordelib-0.9.5/images/test_annotator.jpg` & `hordelib-1.0.0/images/test_annotator.jpg`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/images/test_db0.jpg` & `hordelib-1.0.0/images/test_db0.jpg`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/images/test_facefix.png` & `hordelib-1.0.0/images/test_facefix.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/images/test_inpaint.png` & `hordelib-1.0.0/images/test_inpaint.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/images/test_inpaint_alpha.png` & `hordelib-1.0.0/images/test_inpaint_alpha.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/images/test_inpaint_mask.png` & `hordelib-1.0.0/images/test_inpaint_mask.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/images/test_inpaint_original.png` & `hordelib-1.0.0/images/test_inpaint_original.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/images/test_outpaint.png` & `hordelib-1.0.0/images/test_outpaint.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/pyproject.toml` & `hordelib-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 dependencies = {file = ["requirements.txt"]}
 
 [tool.setuptools.packages.find]
 exclude = ["ComfyUI"]
 namespaces = false
 
 [options.index-client]
-extra-index-urls = ["https://download.pytorch.org/whl/cu117"]
+extra-index-urls = ["https://download.pytorch.org/whl/cu118"]
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 addopts = [
     "--import-mode=prepend",
     "--ignore=nodes"
 ]
@@ -66,20 +66,21 @@
 # Exclude ComfyUI and any packages we have installed in nodes/
 exclude = '''
 /(
     ComfyUI
   | \.tox
   | comfy_controlnet_preprocessors
   | facerestore
+  | build
 )/
 ''' # If you change this, you probably need to also change [tool.mypy] below
 
 [tool.ruff] # XXX this isn't part of CI yet
 line-length=119
-exclude=["comfy_controlnet_preprocessors", "facerestore"]
+exclude=["comfy_controlnet_preprocessors", "facerestore", "build"]
 ignore=[
     "F401", # imported but unused
     "E402", # Module level import not at top of file
     "A002", # Argument `x` is shadowing a python builtin
     "A001", # Variable `x` is shadowing a python builtin
     "INP001", # ... is part of an implicit namespace package. Add an `__init__.py`.
 ]
```

### Comparing `hordelib-0.9.5/requirements.txt` & `hordelib-1.0.0/requirements.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 # Add this in for tox, comment out for build
-#--extra-index-url https://download.pytorch.org/whl/cu117
+#--extra-index-url https://download.pytorch.org/whl/cu118
+horde_model_reference
+pydantic
 torch>=2.0.0
-xformers>=0.0.18
+xformers>=0.0.19
 torchvision
 torchaudio
 torchdiffeq
 torchsde
 einops
 open-clip-torch
 transformers>=4.25.1
 safetensors
 pytorch_lightning
+pynvml
 aiohttp
 accelerate
 pyyaml
 pillow
 loguru
 GitPython
 clip-anytorch
 diffusers
 omegaconf
 psutil
 typing-extensions
+distro
 # face fixer custom nodes
 opencv-python
 # controlnet custom nodes
 opencv-contrib-python
 opencv-python
-timm==0.6.12
+timm==0.6.13
 torchvision
 scipy
-matplotlib
-scikit-image
-prettytable==3.6.0
-svglib
-reportlab
 addict
-yapf
-mediapipe==0.9.1.0
-fairscale
+fairscale
+scikit-image
+mediapipe>=0.9.1.0
```

### Comparing `hordelib-0.9.5/tests/make_index.py` & `hordelib-1.0.0/examples/make_index.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/tests/model_managers/test_comvis.py` & `hordelib-1.0.0/tests/model_managers/test_comvis.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 class TestCompvis:
     _initialised = False
 
     @pytest.fixture(autouse=True)
     def setup_and_teardown(self):
         if not self._initialised:
-            hordelib.initialise({consts.MODEL_CATEGORY_NAMES.compvis: True})
+            hordelib.initialise()
         from hordelib.model_manager.compvis import CompVisModelManager
 
         self.compvis_model_manager = CompVisModelManager()
         assert self.compvis_model_manager is not None
         yield
         del self.compvis_model_manager
```

### Comparing `hordelib-0.9.5/tests/model_managers/test_diffusers.py` & `hordelib-1.0.0/tests/model_managers/test_diffusers.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 class TestDiffusers:
     _initialised = False
 
     @pytest.fixture(autouse=True)
     def setup_and_teardown(self):
         if not self._initialised:
-            hordelib.initialise({consts.MODEL_CATEGORY_NAMES.diffusers: True})
+            hordelib.initialise()
         from hordelib.model_manager.diffusers import DiffusersModelManager
 
         self.diffusers_model_manager = DiffusersModelManager()
         assert self.diffusers_model_manager is not None
         yield
         del self.diffusers_model_manager
```

### Comparing `hordelib-0.9.5/tests/model_managers/test_safety_checker.py` & `hordelib-1.0.0/tests/model_managers/test_safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/tests/test_blip.py` & `hordelib-1.0.0/tests/test_blip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/tests/test_clip.py` & `hordelib-1.0.0/tests/test_clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/tests/test_comfy.py` & `hordelib-1.0.0/tests/test_comfy.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/tests/test_horde_controlnet_annotator.py` & `hordelib-1.0.0/tests/test_horde_controlnet_annotator.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,14 +23,15 @@
             # "gfpgan": True,
             # "safety_checker": True,
         }
         SharedModelManager.loadModelManagers(**self.default_model_manager_args)
         assert SharedModelManager.manager is not None
         for preproc in HordeLib.CONTROLNET_IMAGE_PREPROCESSOR_MAP.keys():
             SharedModelManager.manager.controlnet.download_control_type(preproc)
+        assert SharedModelManager.preloadAnnotators()
         self.image = Image.open("images/test_annotator.jpg")
         self.width, self.height = self.image.size
         yield
         del self.horde
         SharedModelManager._instance = None
         SharedModelManager.manager = None
```

### Comparing `hordelib-0.9.5/tests/test_horde_inference.py` & `hordelib-1.0.0/tests/test_horde_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,16 +117,16 @@
 
     def test_text_to_image(self):
         data = {
             "sampler_name": "k_dpmpp_2m",
             "cfg_scale": 7.5,
             "denoising_strength": 1.0,
             "seed": 123456789,
-            "height": 512,
-            "width": 512,
+            "height": 512.1,  # test param fix
+            "width": 512.1,  # test param fix
             "karras": True,
             "tiling": False,
             "hires_fix": False,
             "clip_skip": 1,
             "control_type": None,
             "image_is_control": False,
             "return_control_map": False,
```

### Comparing `hordelib-0.9.5/tests/test_horde_inference_controlnet.py` & `hordelib-1.0.0/tests/test_horde_inference_controlnet.py`

 * *Files 25% similar despite different names*

```diff
@@ -68,7 +68,64 @@
                 )
                 is True
             )
             data["control_type"] = preproc
             pil_image = self.horde.basic_inference(data)
             assert pil_image is not None
             pil_image.save(f"images/horde_controlnet_{preproc}.webp", quality=90)
+
+    def test_controlnet_strength(self):
+        data = {
+            "sampler_name": "k_dpmpp_2m",
+            "cfg_scale": 7.5,
+            "denoising_strength": 1.0,
+            "seed": 123456789,
+            "height": 512,
+            "width": 512,
+            "karras": True,
+            "tiling": False,
+            "hires_fix": False,
+            "clip_skip": 1,
+            "control_type": "canny",
+            "image_is_control": False,
+            "return_control_map": False,
+            "prompt": "a man walking on the moon",
+            "ddim_steps": 25,
+            "n_iter": 1,
+            "model": "Deliberate",
+            "source_image": Image.open("images/test_db0.jpg"),
+            "source_processing": "img2img",
+        }
+        for strength in [1.0, 0.5, 0.2]:
+            data["control_strength"] = strength
+            pil_image = self.horde.basic_inference(data)
+            assert pil_image is not None
+            pil_image.save(f"images/horde_controlnet_strength_{strength}.webp", quality=90)
+
+    def test_controlnet_hires_fix(self):
+        data = {
+            "sampler_name": "k_dpmpp_2m",
+            "cfg_scale": 7.5,
+            "denoising_strength": 1.0,
+            "seed": 1234345378856789,
+            "height": 768,
+            "width": 768,
+            "karras": True,
+            "tiling": False,
+            "hires_fix": True,
+            "hires_fix_denoising_strength": 0.0,
+            "clip_skip": 1,
+            "control_type": "canny",
+            "image_is_control": False,
+            "return_control_map": False,
+            "prompt": "a man walking in the jungle",
+            "ddim_steps": 15,
+            "n_iter": 1,
+            "model": "Deliberate",
+            "source_image": Image.open("images/test_db0.jpg"),
+            "source_processing": "img2img",
+        }
+        for denoise in [0.4, 0.5, 0.6]:
+            data["hires_fix_denoising_strength"] = denoise
+            pil_image = self.horde.basic_inference(data)
+            assert pil_image is not None
+            pil_image.save(f"images/horde_controlnet_hires_fix_denoise_{denoise}.webp", quality=90)
```

### Comparing `hordelib-0.9.5/tests/test_horde_inference_img2img.py` & `hordelib-1.0.0/tests/test_horde_inference_img2img.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/tests/test_horde_inference_painting.py` & `hordelib-1.0.0/tests/test_horde_inference_painting.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/tests/test_horde_pp.py` & `hordelib-1.0.0/tests/test_horde_pp.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 class TestHordeUpscaling:
     @pytest.fixture(autouse=True, scope="class")
     def setup_and_teardown(self):
         TestHordeUpscaling.horde = HordeLib()
 
         TestHordeUpscaling.image = Image.open("images/test_db0.jpg")
+        TestHordeUpscaling.real_image = Image.open("images/test_annotator.jpg")
         (
             TestHordeUpscaling.width,
             TestHordeUpscaling.height,
         ) = TestHordeUpscaling.image.size
         yield
         del TestHordeUpscaling.horde
 
@@ -75,14 +76,26 @@
         assert pil_image is not None
         width, height = pil_image.size
         assert width == self.width * 4
         assert height == self.height * 4
         pil_image.save("images/horde_image_upscale_NMKD_Siax.webp", quality=90)
 
     @pytest.mark.mm_model("esrgan")
+    def test_image_upscale_NMKD_Siax_resize(self):
+        SharedModelManager.manager.load("NMKD_Siax")
+        assert SharedModelManager.manager.esrgan.is_model_loaded("NMKD_Siax") is True
+        data = {"model": "NMKD_Siax", "source_image": self.real_image, "width": 1280, "height": 1280}
+        pil_image = self.horde.image_upscale(data)
+        assert pil_image is not None
+        width, height = pil_image.size
+        assert width == 1280
+        assert height == 1280
+        pil_image.save("images/horde_image_upscale_NMKD_Siax_resize.webp", quality=90)
+
+    @pytest.mark.mm_model("esrgan")
     def test_image_upscale_RealESRGAN_x4plus_anime_6B(self):
         SharedModelManager.manager.load("RealESRGAN_x4plus_anime_6B")
         assert (
             SharedModelManager.manager.esrgan.is_model_loaded(
                 "RealESRGAN_x4plus_anime_6B",
             )
             is True
```

### Comparing `hordelib-0.9.5/tests/test_inference.py` & `hordelib-1.0.0/tests/test_inference.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/tests/test_safety_checker.py` & `hordelib-1.0.0/tests/test_safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.9.5/tests/test_shared_model_manager.py` & `hordelib-1.0.0/tests/test_shared_model_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 # test_horde.py
+import glob
+import pathlib
+
 import pytest
 
+from hordelib.cache import get_cache_directory
+from hordelib.consts import EXCLUDED_MODEL_NAMES
 from hordelib.horde import HordeLib
 from hordelib.shared_model_manager import SharedModelManager
+from hordelib.utils.logger import HordeLog
 
 
 class TestSharedModelManager:
     horde = HordeLib()
     default_model_manager_args: dict
 
     @pytest.fixture(autouse=True)
     def setup_and_teardown(self):
         self.horde = HordeLib()
+        HordeLog.initialise(True)
+        HordeLog.set_logger_verbosity(5)
+        HordeLog.quiesce_logger(0)
 
         self.default_model_manager_args = {  # XXX # TODO
             # aitemplate
             "blip": True,
             "clip": True,
             "codeformer": True,
             "compvis": True,
@@ -81,20 +90,28 @@
         assert SharedModelManager.manager.is_model_loaded("Deliberate") is False
 
     def test_model_load_checking(self):
         assert SharedModelManager.manager is not None
         assert SharedModelManager.manager.is_model_loaded("Deliberate") is False
         assert SharedModelManager.manager.is_model_loaded("GFPGAN") is False
         assert SharedModelManager.manager.is_model_loaded("RealESRGAN_x4plus") is False
+        assert SharedModelManager.manager.is_model_loaded("4x_NMKD_Superscale_SP") is False
         SharedModelManager.manager.load("Deliberate")
         SharedModelManager.manager.load("GFPGAN")
         SharedModelManager.manager.load("RealESRGAN_x4plus")
+        SharedModelManager.manager.load("4x_NMKD_Superscale_SP")
         assert SharedModelManager.manager.is_model_loaded("Deliberate") is True
         assert SharedModelManager.manager.is_model_loaded("GFPGAN") is True
         assert SharedModelManager.manager.is_model_loaded("RealESRGAN_x4plus") is True
+        assert SharedModelManager.manager.is_model_loaded("4x_NMKD_Superscale_SP") is True
+
+    def test_model_excluding(self):
+        assert SharedModelManager.manager is not None
+        for excluded_model in EXCLUDED_MODEL_NAMES:
+            assert not SharedModelManager.manager.load(excluded_model)
 
     def test_check_sha(self):
         """Check the sha256 hashes of all models. If the .sha file doesn't exist, this will write it out."""
         assert SharedModelManager.manager is not None
         for model_manager in SharedModelManager.manager.active_model_managers:
             for model in model_manager.available_models:
                 model_file_details = model_manager.get_model_files(model)
@@ -106,7 +123,10 @@
         pass
 
     def test_check_validate_all_available_models(self):
         assert SharedModelManager.manager is not None
         for model_manager in SharedModelManager.manager.active_model_managers:
             for model in model_manager.available_models:
                 assert model_manager.validate_model(model)
+
+    def test_preload_annotators(self):
+        assert SharedModelManager.preloadAnnotators()
```

