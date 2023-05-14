# Comparing `tmp/nebulae-0.6.7.tar.gz` & `tmp/nebulae-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nebulae-0.6.7.tar", last modified: Thu May  4 18:13:54 2023, max compression
+gzip compressed data, was "nebulae-0.6.9.tar", last modified: Sun May 14 19:02:37 2023, max compression
```

## Comparing `nebulae-0.6.7.tar` & `nebulae-0.6.9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:13:54.452844 nebulae-0.6.7/
--rw-r--r--   0 root         (0) root         (0)    16769 2023-05-04 18:13:54.452844 nebulae-0.6.7/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:13:54.452844 nebulae-0.6.7/nebulae/
--rw-r--r--   0 root         (0) root         (0)      862 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:13:54.452844 nebulae-0.6.7/nebulae/aerolog/
--rw-r--r--   0 root         (0) root         (0)      733 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/aerolog/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14072 2023-05-03 14:06:07.000000 nebulae-0.6.7/nebulae/aerolog/dashboard.py
--rw-r--r--   0 root         (0) root         (0)     7911 2023-05-03 19:00:43.000000 nebulae-0.6.7/nebulae/aerolog/inspector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:13:54.452844 nebulae-0.6.7/nebulae/astro/
--rw-r--r--   0 root         (0) root         (0)      735 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/astro/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76912 2023-05-04 17:23:15.000000 nebulae-0.6.7/nebulae/astro/craft.py
--rw-r--r--   0 root         (0) root         (0)     3187 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/astro/dock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:13:54.452844 nebulae-0.6.7/nebulae/astro/hangar/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:13:54.452844 nebulae-0.6.7/nebulae/astro/hangar/Classic/
--rw-r--r--   0 root         (0) root         (0)      667 2023-05-01 06:31:07.000000 nebulae-0.6.7/nebulae/astro/hangar/Classic/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4861 2023-05-02 18:30:06.000000 nebulae-0.6.7/nebulae/astro/hangar/Classic/resnet.py
--rw-r--r--   0 root         (0) root         (0)     3916 2023-05-01 06:31:07.000000 nebulae-0.6.7/nebulae/astro/hangar/Classic/vgg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:13:54.452844 nebulae-0.6.7/nebulae/astro/hangar/GAN/
--rw-r--r--   0 root         (0) root         (0)      667 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/astro/hangar/GAN/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27430 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/astro/hangar/GAN/architect.py
--rw-r--r--   0 root         (0) root         (0)     1838 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/astro/hangar/GAN/biggan.py
--rw-r--r--   0 root         (0) root         (0)     1378 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/astro/hangar/GAN/dcgan.py
--rw-r--r--   0 root         (0) root         (0)     1384 2023-05-01 06:31:07.000000 nebulae-0.6.7/nebulae/astro/hangar/GAN/fcgan.py
--rw-r--r--   0 root         (0) root         (0)     1330 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/astro/hangar/GAN/gan.py
--rw-r--r--   0 root         (0) root         (0)     3571 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/astro/hangar/GAN/infogan.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-05-01 06:31:07.000000 nebulae-0.6.7/nebulae/astro/hangar/GAN/resgan.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/astro/hangar/GAN/wgan.py
--rw-r--r--   0 root         (0) root         (0)     1914 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/astro/hangar/GAN/wgan_div.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:13:54.452844 nebulae-0.6.7/nebulae/astro/hangar/Seq2Seq/
--rw-r--r--   0 root         (0) root         (0)      667 2023-05-01 06:31:07.000000 nebulae-0.6.7/nebulae/astro/hangar/Seq2Seq/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6860 2023-05-01 06:31:07.000000 nebulae-0.6.7/nebulae/astro/hangar/Seq2Seq/architect.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:13:54.452844 nebulae-0.6.7/nebulae/astro/hangar/VAE/
--rw-r--r--   0 root         (0) root         (0)      666 2023-05-01 06:31:07.000000 nebulae-0.6.7/nebulae/astro/hangar/VAE/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21531 2023-05-01 06:31:07.000000 nebulae-0.6.7/nebulae/astro/hangar/VAE/architect.py
--rw-r--r--   0 root         (0) root         (0)     1091 2023-05-01 06:31:07.000000 nebulae-0.6.7/nebulae/astro/hangar/VAE/dcvae.py
--rw-r--r--   0 root         (0) root         (0)     1077 2023-05-01 06:31:07.000000 nebulae-0.6.7/nebulae/astro/hangar/VAE/resvae.py
--rw-r--r--   0 root         (0) root         (0)     1070 2023-05-01 06:31:07.000000 nebulae-0.6.7/nebulae/astro/hangar/VAE/vae.py
--rw-r--r--   0 root         (0) root         (0)     1813 2023-05-01 06:31:07.000000 nebulae-0.6.7/nebulae/astro/hangar/VAE/vqvae.py
--rw-r--r--   0 root         (0) root         (0)     1267 2023-05-01 06:31:07.000000 nebulae-0.6.7/nebulae/astro/hangar/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:13:54.452844 nebulae-0.6.7/nebulae/cockpit/
--rw-r--r--   0 root         (0) root         (0)      897 2023-05-02 06:11:46.000000 nebulae-0.6.7/nebulae/cockpit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4543 2023-05-04 16:44:17.000000 nebulae-0.6.7/nebulae/cockpit/engine.py
--rw-r--r--   0 root         (0) root         (0)     6137 2023-05-04 01:57:25.000000 nebulae-0.6.7/nebulae/cockpit/multiverse.py
--rw-r--r--   0 root         (0) root         (0)     3516 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/cockpit/time_machine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:13:54.452844 nebulae-0.6.7/nebulae/fuel/
--rw-r--r--   0 root         (0) root         (0)     1005 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/fuel/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37708 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/fuel/comburant.py
--rw-r--r--   0 root         (0) root         (0)     9783 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/fuel/generator.py
--rw-r--r--   0 root         (0) root         (0)     8160 2023-05-03 13:55:26.000000 nebulae-0.6.7/nebulae/fuel/tank.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:13:54.452844 nebulae-0.6.7/nebulae/kit/
--rw-r--r--   0 root         (0) root         (0)     1096 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/kit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1362 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/kit/decorator.py
--rw-r--r--   0 root         (0) root         (0)    25772 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/kit/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:13:54.452844 nebulae-0.6.7/nebulae/law/
--rw-r--r--   0 root         (0) root         (0)      698 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/law/__init__.py
--rw-r--r--   0 root         (0) root         (0)      928 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/law/constant.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:13:54.452844 nebulae-0.6.7/nebulae.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16769 2023-05-04 18:13:54.000000 nebulae-0.6.7/nebulae.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1466 2023-05-04 18:13:54.000000 nebulae-0.6.7/nebulae.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 18:13:54.000000 nebulae-0.6.7/nebulae.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-04 18:13:54.000000 nebulae-0.6.7/nebulae.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-04 18:13:54.000000 nebulae-0.6.7/nebulae.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 18:13:54.452844 nebulae-0.6.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)    15711 2023-05-04 17:27:36.000000 nebulae-0.6.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 19:02:37.304797 nebulae-0.6.9/
+-rw-r--r--   0 root         (0) root         (0)    16719 2023-05-14 19:02:37.304797 nebulae-0.6.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 19:02:37.300797 nebulae-0.6.9/nebulae/
+-rw-r--r--   0 root         (0) root         (0)      862 2023-05-05 15:53:37.000000 nebulae-0.6.9/nebulae/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 19:02:37.300797 nebulae-0.6.9/nebulae/aerolog/
+-rw-r--r--   0 root         (0) root         (0)      733 2023-05-01 06:31:06.000000 nebulae-0.6.9/nebulae/aerolog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14687 2023-05-14 18:17:15.000000 nebulae-0.6.9/nebulae/aerolog/dashboard.py
+-rw-r--r--   0 root         (0) root         (0)     8025 2023-05-13 14:35:12.000000 nebulae-0.6.9/nebulae/aerolog/inspector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 19:02:37.300797 nebulae-0.6.9/nebulae/astro/
+-rw-r--r--   0 root         (0) root         (0)      735 2023-05-01 06:31:06.000000 nebulae-0.6.9/nebulae/astro/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76950 2023-05-13 17:41:25.000000 nebulae-0.6.9/nebulae/astro/craft.py
+-rw-r--r--   0 root         (0) root         (0)     3187 2023-05-01 06:31:06.000000 nebulae-0.6.9/nebulae/astro/dock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 19:02:37.300797 nebulae-0.6.9/nebulae/astro/hangar/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 19:02:37.300797 nebulae-0.6.9/nebulae/astro/hangar/Classic/
+-rw-r--r--   0 root         (0) root         (0)      667 2023-05-01 06:31:07.000000 nebulae-0.6.9/nebulae/astro/hangar/Classic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4861 2023-05-02 18:30:06.000000 nebulae-0.6.9/nebulae/astro/hangar/Classic/resnet.py
+-rw-r--r--   0 root         (0) root         (0)     3916 2023-05-01 06:31:07.000000 nebulae-0.6.9/nebulae/astro/hangar/Classic/vgg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 19:02:37.304797 nebulae-0.6.9/nebulae/astro/hangar/GAN/
+-rw-r--r--   0 root         (0) root         (0)      667 2023-05-01 06:31:06.000000 nebulae-0.6.9/nebulae/astro/hangar/GAN/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27436 2023-05-05 17:06:10.000000 nebulae-0.6.9/nebulae/astro/hangar/GAN/architect.py
+-rw-r--r--   0 root         (0) root         (0)     1838 2023-05-01 06:31:06.000000 nebulae-0.6.9/nebulae/astro/hangar/GAN/biggan.py
+-rw-r--r--   0 root         (0) root         (0)     1378 2023-05-01 06:31:06.000000 nebulae-0.6.9/nebulae/astro/hangar/GAN/dcgan.py
+-rw-r--r--   0 root         (0) root         (0)     1384 2023-05-01 06:31:07.000000 nebulae-0.6.9/nebulae/astro/hangar/GAN/fcgan.py
+-rw-r--r--   0 root         (0) root         (0)     1330 2023-05-01 06:31:06.000000 nebulae-0.6.9/nebulae/astro/hangar/GAN/gan.py
+-rw-r--r--   0 root         (0) root         (0)     3571 2023-05-01 06:31:06.000000 nebulae-0.6.9/nebulae/astro/hangar/GAN/infogan.py
+-rw-r--r--   0 root         (0) root         (0)     1915 2023-05-05 16:52:44.000000 nebulae-0.6.9/nebulae/astro/hangar/GAN/resgan.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-05-01 06:31:06.000000 nebulae-0.6.9/nebulae/astro/hangar/GAN/wgan.py
+-rw-r--r--   0 root         (0) root         (0)     1914 2023-05-01 06:31:06.000000 nebulae-0.6.9/nebulae/astro/hangar/GAN/wgan_div.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 19:02:37.304797 nebulae-0.6.9/nebulae/astro/hangar/Seq2Seq/
+-rw-r--r--   0 root         (0) root         (0)      667 2023-05-01 06:31:07.000000 nebulae-0.6.9/nebulae/astro/hangar/Seq2Seq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6860 2023-05-01 06:31:07.000000 nebulae-0.6.9/nebulae/astro/hangar/Seq2Seq/architect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 19:02:37.304797 nebulae-0.6.9/nebulae/astro/hangar/VAE/
+-rw-r--r--   0 root         (0) root         (0)      666 2023-05-01 06:31:07.000000 nebulae-0.6.9/nebulae/astro/hangar/VAE/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21531 2023-05-01 06:31:07.000000 nebulae-0.6.9/nebulae/astro/hangar/VAE/architect.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-05-01 06:31:07.000000 nebulae-0.6.9/nebulae/astro/hangar/VAE/dcvae.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2023-05-01 06:31:07.000000 nebulae-0.6.9/nebulae/astro/hangar/VAE/resvae.py
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-05-01 06:31:07.000000 nebulae-0.6.9/nebulae/astro/hangar/VAE/vae.py
+-rw-r--r--   0 root         (0) root         (0)     1813 2023-05-01 06:31:07.000000 nebulae-0.6.9/nebulae/astro/hangar/VAE/vqvae.py
+-rw-r--r--   0 root         (0) root         (0)     1267 2023-05-01 06:31:07.000000 nebulae-0.6.9/nebulae/astro/hangar/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 19:02:37.304797 nebulae-0.6.9/nebulae/cockpit/
+-rw-r--r--   0 root         (0) root         (0)      897 2023-05-02 06:11:46.000000 nebulae-0.6.9/nebulae/cockpit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4581 2023-05-13 14:32:56.000000 nebulae-0.6.9/nebulae/cockpit/engine.py
+-rw-r--r--   0 root         (0) root         (0)     6183 2023-05-13 18:34:52.000000 nebulae-0.6.9/nebulae/cockpit/multiverse.py
+-rw-r--r--   0 root         (0) root         (0)     3970 2023-05-14 09:14:52.000000 nebulae-0.6.9/nebulae/cockpit/time_machine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 19:02:37.304797 nebulae-0.6.9/nebulae/fuel/
+-rw-r--r--   0 root         (0) root         (0)     1005 2023-05-01 06:31:06.000000 nebulae-0.6.9/nebulae/fuel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37621 2023-05-14 09:05:16.000000 nebulae-0.6.9/nebulae/fuel/comburant.py
+-rw-r--r--   0 root         (0) root         (0)     9783 2023-05-01 06:31:06.000000 nebulae-0.6.9/nebulae/fuel/generator.py
+-rw-r--r--   0 root         (0) root         (0)     8171 2023-05-13 14:33:16.000000 nebulae-0.6.9/nebulae/fuel/tank.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 19:02:37.304797 nebulae-0.6.9/nebulae/kit/
+-rw-r--r--   0 root         (0) root         (0)     1096 2023-05-01 06:31:06.000000 nebulae-0.6.9/nebulae/kit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1123 2023-05-14 17:25:41.000000 nebulae-0.6.9/nebulae/kit/decorator.py
+-rw-r--r--   0 root         (0) root         (0)    25772 2023-05-01 06:31:06.000000 nebulae-0.6.9/nebulae/kit/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 19:02:37.304797 nebulae-0.6.9/nebulae/law/
+-rw-r--r--   0 root         (0) root         (0)      698 2023-05-01 06:31:06.000000 nebulae-0.6.9/nebulae/law/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      954 2023-05-13 14:28:13.000000 nebulae-0.6.9/nebulae/law/constant.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 19:02:37.300797 nebulae-0.6.9/nebulae.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16719 2023-05-14 19:02:37.000000 nebulae-0.6.9/nebulae.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1466 2023-05-14 19:02:37.000000 nebulae-0.6.9/nebulae.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 19:02:37.000000 nebulae-0.6.9/nebulae.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      114 2023-05-14 19:02:37.000000 nebulae-0.6.9/nebulae.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-14 19:02:37.000000 nebulae-0.6.9/nebulae.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 19:02:37.304797 nebulae-0.6.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)    16027 2023-05-14 18:12:08.000000 nebulae-0.6.9/setup.py
```

### Comparing `nebulae-0.6.7/PKG-INFO` & `nebulae-0.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nebulae
-Version: 0.6.7
-Summary: A novel and simple framework based on prevalent DL frameworks and other image processing libs. v0.6.7: fix bugs of device allocation and attribute getter in EMA; add on_device argument in EMA for faster update with higher memory occupied; add gearbox argument in Engine to apply Module.compile() in PyTorch 2.
+Version: 0.6.9
+Summary: A novel and simple framework based on prevalent DL frameworks and other image processing libs. v0.6.9: replace 'RANK' with 'NEB_RANK' for distributed training in environ variables; add subdir argument in DashBoard.log(); add wipe argument in DashBoard.gauge()
 Home-page: https://github.com/
 Author: Seria
 Author-email: zzqsummerai@yeah.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nebulae-0.6.7/nebulae/__init__.py` & `nebulae-0.6.9/nebulae/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/aerolog/__init__.py` & `nebulae-0.6.9/nebulae/aerolog/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/aerolog/dashboard.py` & `nebulae-0.6.9/nebulae/aerolog/dashboard.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,31 +25,32 @@
 from ..kit.utility import curve2str
 import matplotlib.pyplot as plt
 import seaborn as sns
 import numpy as np
 import time
 import pandas as pd
 import os
-import warnings
+from sys import stdout
+from ..law import Constant
 
 
 
 class DashBoard(object):
     palette = ['#F08080', '#00BFFF', '#FFFF00', '#2E8B57', '#6A5ACD', '#FFD700', '#808080']
     linestyle = ['-', '--', '-.', ':']
-    def __init__(self, log_path='./aerolog', window=1, divisor=10, span=30, format=None):
+    def __init__(self, log_dir='./aerolog', window=1, divisor=10, span=30, format=None):
         '''
         :param config:
         :param window: the window length of moving average
         :param format: a list of which the element is format and mode, e.g. ['3f', 'raw']
         '''
-        self.rank = int(os.environ.get('RANK', -1))
-        if not os.path.exists(log_path):
-            os.mkdir(log_path)
-        self.log_path = log_path
+        self.rank = int(os.environ.get(Constant.ENV_RANK, -1))
+        if not os.path.exists(log_dir):
+            os.mkdir(log_dir)
+        self.log_dir = log_dir
         self.window = window
         self.divisor = divisor
         self.span = span
         self.format = format
 
         self.max_epoch = 0
         self.first_call = True # if it is the first call for self.gauge()
@@ -87,18 +88,19 @@
             return ''
         elif mode == 'tailor':
             string = form(value)
             return ' %s ➠ \033[1;36m%s\033[0m |' % (abbr, string)
         else:
             raise KeyError('%s is an illegal format option.' % mode)
 
-    def gauge(self, entry, mile, epoch, mpe, stage, interval=1, duration=None, plot=True, flush=0,
+    def gauge(self, entry, mile, epoch, mpe, stage, interval=1, duration=None, plot=True, wipe=False, flush=0,
               is_global=True, is_elastic=False, in_loop=(-1,), last_for=1):
         if self.rank>0:
             return
+        assert not (plot and wipe), 'NEBULAE ERROR ⨷ plot and wipe are mutually exclusive.'
         epoch += 1
         mile += 1
         string_mile = ''
         flag_display = False
         flag_epoch_end = False
         len_loop = len(in_loop)
         assert in_loop[0]<0 or len_loop>1, 'NEBULAE ERROR ⨷ the dashboard should loop through more than one curve.'
@@ -186,24 +188,36 @@
             progress = int((mile - 1) / mpe * 20 + 0.4)
             yellow_bar = progress * ' '
             space_bar = (20 - progress) * ' '
             if duration is None:
                 duration = '--:--'
             else:
                 duration = '%.3f'%duration
+            if wipe:
+                end_char = '\r'
+            else:
+                end_char = '\n'
             print('| %d%s Epoch ✇ %d Miles ⊰⟦\033[43m%s\033[0m%s⟧⊱︎ ⧲ %ss/mile | %s |%s     '
-                  % (epoch, ordinal, mile, yellow_bar, space_bar, duration, stage, string_mile), end='\n')
-            if curve_exists:
-                print(f'\033[{self.divisor+flush+7}A')
+                  % (epoch, ordinal, mile, yellow_bar, space_bar, duration, stage, string_mile), end=end_char)
+            if wipe:
+                stdout.flush()
             else:
-                print(f'\033[2A')
+                if curve_exists:
+                    print(f'\033[{self.divisor+flush+7}A')
+                else:
+                    print(f'\033[2A')
+            
         if flag_epoch_end:
-            for _ in range(self.divisor+flush+6):
-                print(w * ' ')
-            print(f'\033[{self.divisor+flush+7}A')
+            if wipe:
+                print(2 * w * ' ', end='\r')
+                stdout.flush()
+            else:
+                for _ in range(self.divisor+flush+6):
+                    print(w * ' ')
+                print(f'\033[{self.divisor+flush+7}A')
             ordinal = self._getOridinal(epoch)
             mileage = str(epoch * mpe)
             display = '| %d%s Epoch ✇ %s Miles ︎⧲ %.2fs/epoch | %s |%s' \
                       % (epoch, ordinal, mileage, time.time() - self.time, stage, string_epoch)
             print('+' + (len(display) - 3 - cnt * 11) * '-' + '+' + 30 * ' ')
             print(display)
             print('+' + (len(display) - 3 - cnt * 11) * '-' + '+' + 30 * ' ')
@@ -235,17 +249,22 @@
             if a > m[1]:
                 m[1] = a
                 idx[1] = i
         idx[0] += 1
         idx[1] += 1
         return m + idx
 
-    def log(self, gauge=True, tachograph=True, history=''):
+    def log(self, gauge=True, tachograph=True, history='', subdir=''):
         if self.rank>0:
             return
+        if subdir:
+            log_dir = os.path.join(self.log_dir, subdir)
+            os.makedirs(log_dir, exist_ok=True)
+        else:
+            log_dir = self.log_dir
         if history:
             for f in os.listdir(history):
                 if not f.endswith('csv'):
                     continue
                 df = pd.read_csv(os.path.join(history, f), header=0)
                 value = df.values
                 unit = df.columns[0]
@@ -276,15 +295,15 @@
                     ymin, ymax, xmin, xmax = self._argm(self.gauge_mile[b])
                     xoff = len(self.trail_mile[stage]) * 0.02
                     yoff = (ymax - ymin) * 0.02
                     ax.annotate(('%%%s' % (self.format[entry][0])) % ymin, (xmin - xoff, ymin + yoff))
                     ax.annotate(('%%%s' % (self.format[entry][0])) % ymax, (xmax - xoff, ymax + yoff))
                     data = pd.DataFrame({b: self.gauge_mile[b]}, index=self.trail_mile[stage])
                     sns.lineplot(data=data, markers=False, ax=ax)
-                    plt.savefig(os.path.join(self.log_path, '%s_%s_%.3g_mile_%d.jpg'
+                    plt.savefig(os.path.join(log_dir, '%s_%s_%.3g_mile_%d.jpg'
                                     % (k.replace('/', '-'), stage, self.gauge_mile[b][-1], self.trail_mile[stage][-1])))
                     plt.close()
 
             for k in boards.keys():
                 fig = plt.figure()
                 ax = fig.add_subplot(111)
                 stage = 'UNK'
@@ -296,32 +315,32 @@
                         yoff = (ymax - ymin) * 0.02
                         ax.annotate(('%%%s' % (self.format[entry][0])) % ymin, (xmin - xoff, ymin + yoff))
                         ax.annotate(('%%%s' % (self.format[entry][0])) % ymax, (xmax - xoff, ymax + yoff))
                 if len(boards[k]) > 0 and self.max_epoch > 0:
                     data = pd.DataFrame({b: np.asarray(self.gauge_epoch[b]) for b in boards[k]},
                                         index=self.trail_epoch[stage])
                     sns.lineplot(data=data, markers=True, ax=ax)
-                    plt.savefig(os.path.join(self.log_path, '%s_epoch_%d.jpg' % (k, self.max_epoch)))
+                    plt.savefig(os.path.join(log_dir, '%s_epoch_%d.jpg' % (k, self.max_epoch)))
                 plt.close()
         if tachograph:
             for k in self.gauge_mile.keys():
                 stage, metric = k.split(':')
                 df = pd.DataFrame(data={'mile': self.trail_mile[stage], k: self.gauge_mile[k]})
-                df.to_csv(os.path.join(self.log_path, '%s_%s_mile.csv'%(metric.replace('/', '-'), stage)), index=None)
+                df.to_csv(os.path.join(log_dir, '%s_%s_mile.csv'%(metric.replace('/', '-'), stage)), index=None)
                 df = pd.DataFrame(data={'epoch': self.trail_epoch[stage], k: self.gauge_epoch[k]})
-                df.to_csv(os.path.join(self.log_path, '%s_%s_epoch.csv' % (metric.replace('/', '-'), stage)), index=None)
+                df.to_csv(os.path.join(log_dir, '%s_%s_epoch.csv' % (metric.replace('/', '-'), stage)), index=None)
 
 
 if __name__ == "__main__":
     import random as rand
-    # db = DashBoard(log_path="/Users/Seria/Desktop/nebulae/test/ckpt",
-    #                 window=15, divisor=15, span=70,
-    #                 format={"Acc": [".2f", "percent"], "Loss": [".3f", "raw"], "MAE": [".3f", "raw"]})
-    # for epoch in range(5):
-    #     for mile in range(10):
-    #         probe = {'Acc':rand.random(), 'Loss':rand.random()}
-    #         db.gauge(probe, mile, epoch, 10, 'TRAIN', interval=1, is_global=True)
-    #
-    #     for mile in range(10):
-    #         probe = {'Acc':rand.random()}
-    #         db.gauge(probe, mile, epoch, 10, 'DEV', interval=1, is_global=True)
-    # db.log()
+    db = DashBoard(log_dir="/Users/Seria/Desktop/nebulae/test/ckpt",
+                    window=15, divisor=15, span=70,
+                    format={"Acc": [".2f", "percent"], "Loss": [".3f", "raw"], "MAE": [".3f", "raw"]})
+    for epoch in range(5):
+        for mile in range(10):
+            probe = {'Acc':rand.random(), 'Loss':rand.random()}
+            db.gauge(probe, mile, epoch, 10, 'TRAIN', interval=1, is_global=True)
+    
+        for mile in range(10):
+            probe = {'Acc':rand.random()}
+            db.gauge(probe, mile, epoch, 10, 'DEV', interval=1, is_global=True)
+    db.log()
```

### Comparing `nebulae-0.6.7/nebulae/aerolog/inspector.py` & `nebulae-0.6.9/nebulae/aerolog/inspector.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,30 +28,32 @@
 from ..cockpit.multiverse import DDP
 
 from graphviz import Digraph
 import os
 import sys
 import torch
 from ptflops.pytorch_engine import add_flops_counting_methods
+from ..law import Constant
 
 class Inspector(object):
 
     def __init__(self, export_path='./craft', verbose=True, hidden=(), onnx_ver=-1):
         self.export_path = export_path
+        os.makedirs(os.path.dirname(export_path), exist_ok=True)
         self.verbose = verbose
         self.hidden = hidden
         self.onnx_ver = onnx_ver
         self.layout = Digraph(comment='The Space Craft', format='jpg')
         self.layout.attr('node', shape='doublecircle')
         self.seen = []
         self.displayed = [] # already printed on screen
         self.shapes = {}
 
     def paint(self, archit, *dummy_args, **dummy_kwargs):
-        rank = int(os.environ.get('RANK', -1))
+        rank = int(os.environ.get(Constant.ENV_RANK, -1))
         if rank > 0:
             return
 
         if isinstance(archit, (DP, DDP)):
             archit = archit.module
         if ver2num(torch.__version__) >= ver2num('2.0') and isinstance(archit, torch._dynamo.OptimizedModule):
             self.archit = archit._orig_mod
@@ -136,15 +138,15 @@
 
         flops_count, params_count = flops_model.compute_average_flops_cost()
         flops_model.stop_flops_count()
 
         return flops_count
 
     def dissect(self, archit, *dummy_args, **dummy_kwargs):
-        rank = int(os.environ.get('RANK', -1))
+        rank = int(os.environ.get(Constant.ENV_RANK, -1))
         if rank > 0:
             return
         
         if isinstance(archit, (DP, DDP)):
             archit = archit.module
         if ver2num(torch.__version__) >= ver2num('2.0') and isinstance(archit, torch._dynamo.OptimizedModule):
             archit = archit._orig_mod
```

### Comparing `nebulae-0.6.7/nebulae/astro/__init__.py` & `nebulae-0.6.9/nebulae/astro/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/astro/craft.py` & `nebulae-0.6.9/nebulae/astro/craft.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from functools import partial
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from ..cockpit.engine import Engine
 from ..cockpit import CPU, GPU
 from ..kit import ver2num
+from ..law import Constant
 
 __all__ = ('Rudder', 'Prober', 'Nozzle',
            'NEAREST', 'LINEAR', 'CUBIC', 'AREA',
            'CONSTANT', 'REFLECT', 'REPLICATE',
            'Void', 'XavierNorm', 'XavierUnif', 'Normal', 'Uniform', 'Orthog', 'Zeros', 'Ones',
            'Conv', 'TransConv', 'GraphConvEig', 'GraphConvLap', 'GraphConvAdj', 'Dense', 'Embed', 'Pad', 'Identity',
            'RNN', 'BiRNN', 'LSTM', 'BiLSTM', 'MHAttn',
@@ -606,15 +607,15 @@
 
 class EMA(Craft):
     def __init__(self, hull, decay_fn=lambda x: 0.9, on_device=False, scope='EMA'):
         super(EMA, self).__init__(scope)
         self.counter = 0
         self.decay_fn = decay_fn
         self.on_device = on_device
-        self._rank = int(os.environ.get('RANK', -1))
+        self._rank = int(os.environ.get(Constant.ENV_RANK, -1))
         self['hull'] = hull
         self.swapped = False # whether have swapped to its shadow
 
         # initialize shadow as hull itself
         self.shadow = {}
         hull_params = hull.state_dict()
         # note that params have not been to GPU even cuda is enabled
```

### Comparing `nebulae-0.6.7/nebulae/astro/dock.py` & `nebulae-0.6.9/nebulae/astro/dock.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/astro/hangar/Classic/__init__.py` & `nebulae-0.6.9/nebulae/astro/hangar/Classic/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/astro/hangar/Classic/resnet.py` & `nebulae-0.6.9/nebulae/astro/hangar/Classic/resnet.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/astro/hangar/Classic/vgg.py` & `nebulae-0.6.9/nebulae/astro/hangar/Classic/vgg.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/astro/hangar/GAN/__init__.py` & `nebulae-0.6.9/nebulae/astro/hangar/GAN/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/astro/hangar/GAN/architect.py` & `nebulae-0.6.9/nebulae/astro/hangar/GAN/architect.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,15 +386,15 @@
         z = self.fc(self['latent_code'])
         z = self.reshape(z, (-1, self.ichs[0], self.min_res, self.min_res))
 
         if self.cn:
             for i in range(len(self.ochs)):
                 rb = getattr(self, 'blk_%d' % i)
                 z = rb((z, self['latent_code']))
-                n_shape = z.shape
+                n_shape = list(z.shape)
                 n_shape[1] = 1
                 noise = dock.coat(np.random.normal(size=n_shape).astype('float32'))
                 strength = dock.coat(np.array(0).astype('float32'), as_const=False)
                 z += strength * noise
                 z = self.up(z)
 
             z = self.nf(z, self['latent_code'])
```

### Comparing `nebulae-0.6.7/nebulae/astro/hangar/GAN/biggan.py` & `nebulae-0.6.9/nebulae/astro/hangar/GAN/biggan.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/astro/hangar/GAN/dcgan.py` & `nebulae-0.6.9/nebulae/astro/hangar/GAN/dcgan.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/astro/hangar/GAN/fcgan.py` & `nebulae-0.6.9/nebulae/astro/hangar/GAN/fcgan.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/astro/hangar/GAN/gan.py` & `nebulae-0.6.9/nebulae/astro/hangar/GAN/gan.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/astro/hangar/GAN/infogan.py` & `nebulae-0.6.9/nebulae/astro/hangar/GAN/infogan.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/astro/hangar/GAN/resgan.py` & `nebulae-0.6.9/nebulae/astro/hangar/GAN/resgan.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 
 
 class Discriminator(Craft):
     def __init__(self, in_shape, base_chs, norm_fn, attention, spec_norm, w_init, scope='DSC'):
         super(Discriminator, self).__init__(scope)
         H, W, C = in_shape
         min_size = min(H, W)
-        factor = {64: base_chs / 32,
-                  128: base_chs / 16,
-                  256: base_chs / 64}
+        factor = {64: base_chs // 32,
+                  128: base_chs // 16,
+                  256: base_chs // 64}
         self.backbone = ResD(in_shape, base_chs, norm_fn, attention, spec_norm, w_init)
         if spec_norm:
             self.cls = dock.SN(dock.Dense(int(H * W * factor[min_size]), 1))
         else:
             self.cls = dock.Dense(int(H * W * factor[min_size]), 1)
 
     def run(self, x):
```

### Comparing `nebulae-0.6.7/nebulae/astro/hangar/GAN/wgan.py` & `nebulae-0.6.9/nebulae/astro/hangar/GAN/wgan.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/astro/hangar/GAN/wgan_div.py` & `nebulae-0.6.9/nebulae/astro/hangar/GAN/wgan_div.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/astro/hangar/Seq2Seq/__init__.py` & `nebulae-0.6.9/nebulae/astro/hangar/Seq2Seq/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/astro/hangar/Seq2Seq/architect.py` & `nebulae-0.6.9/nebulae/astro/hangar/Seq2Seq/architect.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/astro/hangar/VAE/__init__.py` & `nebulae-0.6.9/nebulae/astro/hangar/VAE/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/astro/hangar/VAE/architect.py` & `nebulae-0.6.9/nebulae/astro/hangar/VAE/architect.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/astro/hangar/VAE/dcvae.py` & `nebulae-0.6.9/nebulae/astro/hangar/VAE/dcvae.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/astro/hangar/VAE/resvae.py` & `nebulae-0.6.9/nebulae/astro/hangar/VAE/resvae.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/astro/hangar/VAE/vae.py` & `nebulae-0.6.9/nebulae/astro/hangar/VAE/vae.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/astro/hangar/VAE/vqvae.py` & `nebulae-0.6.9/nebulae/astro/hangar/VAE/vqvae.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/astro/hangar/__init__.py` & `nebulae-0.6.9/nebulae/astro/hangar/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/cockpit/__init__.py` & `nebulae-0.6.9/nebulae/cockpit/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/cockpit/engine.py` & `nebulae-0.6.9/nebulae/cockpit/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
    ===========  \__  NOBUG  __/  ===========
    
 '''
 # -*- coding:utf-8 -*-
 import os
 import torch
 from ..kit.utility import GPUtil, ver2num
+from ..law import Constant
 
 CPU = 0
 GPU = 1
 
 DYNAMIC = 20
 STATIC = 21
 FIXED = 22
@@ -40,15 +41,15 @@
     device: CPU or GPU
     available_gpus
     gpu_mem_fraction
     if_conserve
     least_mem
     '''
     def __init__(self, device=GPU, ngpu=1, least_mem=2048, avail_gpus=(), multi_piston=False, gearbox=DYNAMIC):
-        self.rank = int(os.environ.get('RANK', -1))
+        self.rank = int(os.environ.get(Constant.ENV_RANK, -1))
         self.device = device
         self.multi_piston = multi_piston
         if gearbox in (STATIC, FIXED) and ver2num(torch.__version__) < ver2num('2.0'):
             print('NEBULAE WARNING ◘ The PyTorch version is lower than 2.0, hence the gearbox will be DYNAMIC as default.')
             gearbox = DYNAMIC
         self.gearbox = gearbox
         # look for available gpu devices
```

### Comparing `nebulae-0.6.7/nebulae/cockpit/multiverse.py` & `nebulae-0.6.9/nebulae/cockpit/multiverse.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 '''
 # -*- coding:utf-8 -*-
 import torch
 import os
 # import multiprocessing as mp
 import torch.multiprocessing as mp
 from ..kit.utility import ver2num
+from ..law import Constant
 
 if ver2num(torch.__version__) >= ver2num('1.6.0'):
     is_new_version = True
 else:
     is_new_version = False
 
 if is_new_version:
@@ -120,45 +121,44 @@
         self.rank = -1
         self.env = os.environ.copy()
         self.env["MASTER_ADDR"] = '127.0.0.1'
         self.env["MASTER_PORT"] = '12345'
         self.env["WORLD_SIZE"] = str(nworld)
         # self.env["OMP_NUM_THREADS"] = '1'
 
-    def cleanup(self):
-        torch.distributed.destroy_process_group()
+    def __del__(self):
+        if self.rank == 0:
+            torch.distributed.destroy_process_group()
 
     def __call__(self, *args, **kwargs):
         # mp.set_start_method('spawn')
         ps = []
         for r in range(self.nworld):
-            self.rank = r
-            self.env['RANK'] = str(r)
+            self.env[Constant.ENV_RANK] = str(r)
             self.env['LOCAL_RANK'] = str(r)
             p = mp.Process(target=self.universe, args=(self,)+args, kwargs=kwargs)
             p.start()
             ps.append(p)
         for p in ps:
             p.join()
 
         # mp.spawn(self.universe, args=(self,)+args, nprocs=self.nworld)
 
     def init(self):#, rank):
-        # os.environ['RANK'] = str(rank)
+        # os.environ[Constant.ENV_RANK] = str(rank)
         for k, v in self.env.items():
             os.environ[k] = v
-        rank = int(os.environ['RANK'])
-        torch.distributed.init_process_group(backend="nccl", rank=rank, world_size=self.nworld)
+        self.rank = int(os.environ[Constant.ENV_RANK])
+        torch.distributed.init_process_group(backend="nccl", rank=self.rank, world_size=self.nworld)
 
     def _sync(self, model):
-        rank = int(os.environ['RANK'])
         scope = model.scope
         if is_new_version:
             model = torch.nn.SyncBatchNorm.convert_sync_batchnorm(model)
-            model = DDP(model, device_ids=[rank], output_device=rank)
+            model = DDP(model, device_ids=[self.rank], output_device=self.rank)
         else:
             model = parallel.convert_syncbn_model(model)
             model = DDP(model, delay_allreduce=True)
 
         model.scope = scope
         return model
```

### Comparing `nebulae-0.6.7/nebulae/cockpit/time_machine.py` & `nebulae-0.6.9/nebulae/cockpit/time_machine.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,77 +21,89 @@
    ===========  \__  NOBUG  __/  ===========
    
 '''
 # -*- coding:utf-8 -*-
 import torch
 import os
 from glob import glob
+from ..law import Constant
 
 
 
 class TimeMachine(object):
-    def __init__(self, ckpt_path, save_path, max_anchors=-1):
+    def __init__(self, ckpt_dir, save_dir, max_anchors=-1):
         '''
         Time Machine saves current states or restores saved states
         '''
-        self.rank = int(os.environ.get('RANK', -1))
-        self.ckpt_path = ckpt_path
-        self.save_path = save_path
+        self.rank = int(os.environ.get(Constant.ENV_RANK, -1))
+        self.ckpt_dir = ckpt_dir
+        self.save_dir = save_dir
+        os.makedirs(ckpt_dir, exist_ok=True)
+        os.makedirs(save_dir, exist_ok=True)
         self.max_anchors = max_anchors
         self.counter = 1
         self.anchors = []
 
     def to(self, craft, optz=None, file='', ckpt_scope=None, frozen=False):
-        assert self.ckpt_path is not None, Exception('NEBULAE ERROR ⨷ anchor location is not provided.')
+        assert self.ckpt_dir is not None, Exception('NEBULAE ERROR ⨷ anchor location is not provided.')
 
-        ckpt_path = os.path.join(self.ckpt_path, file)
-        if os.path.isfile(ckpt_path):
-            moment = ckpt_path
+        ckpt_dir = os.path.join(self.ckpt_dir, file)
+        if os.path.isfile(ckpt_dir):
+            moment = ckpt_dir
         else:
-            architecture = glob(os.path.join(ckpt_path,'*.pth'))
+            architecture = glob(os.path.join(ckpt_dir, '*.pth'))
             latest = -1
             moment = None
             for arch in architecture:
                 last_mod = os.path.getmtime(arch)
                 if last_mod > latest:
                     moment = arch
                     latest = last_mod
         if moment is None:
             raise Exception('NEBULAE ERROR ⨷ valid anchor is not found.')
 
         states = torch.load(moment)
         if optz is not None:
-            optz.load_state_dict(states['optz'])
+            if isinstance(optz, dict):
+                for k, v in optz.items():
+                    v.load_state_dict(states[k])
+            else:
+                optz.load_state_dict(states['optz'])
             states = states['net']
         if not ckpt_scope is None:
             ckpt_scope = ckpt_scope.replace('/', '.')
             states = {k: v for k, v in states.items() if k.startswith(ckpt_scope)}
         craft.load_state_dict(states, strict=frozen)
         if self.rank <= 0:
             print('+' + ((10 + len(moment)) * '-') + '+')
             print('| Back to \033[1;34m%s\033[0m |' % moment)
             print('+' + ((10 + len(moment)) * '-') + '+')
 
     def drop(self, craft, optz=None, file='', save_scope=None, frozen=False):
         if self.rank>0:
             return
-        assert self.save_path is not None, Exception('NEBULAE ERROR ⨷ there is nowhere to drop anchor.')
+        assert self.save_dir is not None, Exception('NEBULAE ERROR ⨷ there is nowhere to drop anchor.')
 
-        save_path = os.path.join(self.save_path, file)
+        save_dir = os.path.join(self.save_dir, file)
         states = craft.state_dict()
         if save_scope is not None:
             save_scope = save_scope.replace('/', '.')
             states = {k:v for k,v in states.items() if k.startswith(save_scope)}
         if optz is not None:
-            states = {'net': states, 'optz': optz.state_dict()}
+            if isinstance(optz, dict):
+                states = {'net': states}
+                for k, v in optz.items():
+                    states[k] = v.state_dict()
+            else:
+                states = {'net': states, 'optz': optz.state_dict()}
 
-        if save_path.endswith('.pth'):
-            save_ckpt = save_path
+        if save_dir.endswith('.pth'):
+            save_ckpt = save_dir
         else:
-            save_ckpt = os.path.join(save_path, '%s-%d.pth'%(craft.scope, self.counter))
+            save_ckpt = os.path.join(save_dir, '%s-%d.pth'%(craft.scope, self.counter))
         torch.save(states, save_ckpt)
         self.counter += 1
         self.anchors.append(save_ckpt)
         if self.max_anchors > 0 and len(self.anchors) > self.max_anchors:
             os.remove(self.anchors[0])
             del self.anchors[0]
         print('| Anchor is dropped at \033[1;34m%s\033[0m |' % save_ckpt)
```

### Comparing `nebulae-0.6.7/nebulae/fuel/__init__.py` & `nebulae-0.6.9/nebulae/fuel/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/fuel/comburant.py` & `nebulae-0.6.9/nebulae/fuel/comburant.py`

 * *Files 2% similar despite different names*

```diff
@@ -1034,26 +1034,28 @@
         return _vid_encode(imgs, fps, br, 'av1', self._format)
 
 
 
 if __name__ == '__main__':
     from time import time
     import cv2
+    from os.path import join as pjoin
     from PIL import ImageEnhance
+    DROOT = '/Users/Seria/Desktop/nebulae/test'
     # >| VABC test
     seq = []
     for i in range(5):
-        img = cv2.imread('/Users/Seria/Desktop/nebulae/test/vid/%04d.png'%(i+1))
+        img = cv2.imread('/vid/%04d.png'%(i+1))
         img = img[:,:,::-1]
         seq.append(img)
     cbr = Comburant(H264(30, 6e5))
     dst = cbr(seq)
     for i in range(5):
-        # dst[i].save('/Users/Seria/Desktop/nebulae/test/img/%04d.png'%(i+1), format='PNG', compress_level=0)
-        cv2.imwrite('/Users/Seria/Desktop/nebulae/test/img/np-lr-%03d.png' % (i + 1),
+        # dst[i].save(pjoin(DROOT, 'img/%04d.png'%(i+1)), format='PNG', compress_level=0)
+        cv2.imwrite(pjoin(DROOT, 'img/np-lr-%03d.png' % (i + 1)),
                     dst[i][:, :, ::-1], [cv2.IMWRITE_PNG_COMPRESSION, 0])
 
 
     # >| ABC test
     cbr = Comburant(Crop((128, 128), central=True, pair_fn=multiple((1, 2))),
                     Resize((100, 100), pair_fn=multiple((1, 2))),
                     Flip(HORIZONTAL),
@@ -1069,26 +1071,26 @@
                     JPEG(90),
                     )#format=PIL, end=False)
     t_ = time()
     niter = 20
     lrs = []
     hrs = []
     for i in range(niter):
-        path = '/Users/Seria/Desktop/nebulae/test/vid/%04d.png'%(i+1)
+        path = pjoin(DROOT, 'vid/%04d.png'%(i+1))
 
         # img = Image.open(path)
         # hrs.append(img)
         # lrs.append(img.resize((img.size[0] // 2, img.size[1] // 2)))
 
         img = cv2.imread(path)
         img = img[:,:,::-1]
         hrs.append(img)
         lrs.append(cv2.resize(img, (img.shape[1]//2, img.shape[0]//2)))
 
     imgs = cbr([lrs, hrs])
     _t = time()
     for i in range(1):
-        # imgs[0][i].save('/Users/Seria/Desktop/nebulae/test/img/pil-lr-%03d.png' % (i + 1), format='PNG', compress_level=0)
-        # imgs[1][i].save('/Users/Seria/Desktop/nebulae/test/img/pil-hr-%03d.png' % (i + 1), format='PNG', compress_level=0)
-        cv2.imwrite('/Users/Seria/Desktop/nebulae/test/img/np-lr-%03d.png'%(i+1), imgs[0][i][:,:,::-1])#, [cv2.IMWRITE_PNG_COMPRESSION, 0])
-        cv2.imwrite('/Users/Seria/Desktop/nebulae/test/img/np-hr-%03d.png'%(i+1), imgs[1][i][:,:,::-1])#, [cv2.IMWRITE_PNG_COMPRESSION, 0])
+        # imgs[0][i].save(pjoin(DROOT, 'img/pil-lr-%03d.png' % (i + 1)), format='PNG', compress_level=0)
+        # imgs[1][i].save(pjoin(DROOT, 'img/pil-hr-%03d.png' % (i + 1)), format='PNG', compress_level=0)
+        cv2.imwrite(pjoin(DROOT, 'img/np-lr-%03d.png'%(i+1)), imgs[0][i][:,:,::-1])#, [cv2.IMWRITE_PNG_COMPRESSION, 0])
+        cv2.imwrite(pjoin(DROOT, 'img/np-hr-%03d.png'%(i+1)), imgs[1][i][:,:,::-1])#, [cv2.IMWRITE_PNG_COMPRESSION, 0])
     print((_t-t_)/niter)
```

### Comparing `nebulae-0.6.7/nebulae/fuel/generator.py` & `nebulae-0.6.9/nebulae/fuel/generator.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/fuel/tank.py` & `nebulae-0.6.9/nebulae/fuel/tank.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
     def __len__(self):
         return self._length
 
 
 class Depot(object):
     def __init__(self, engine):
-        self.rank = int(os.environ.get('RANK', -1))
+        self.rank = int(os.environ.get(Constant.ENV_RANK, -1))
         self.nworld = int(os.environ.get('WORLD_SIZE', 1))
         if hasattr(engine, 'chip'):
             if engine.multi_piston:
                 self._chip = torch.device('cuda')
             else:
                 self._chip = engine.chip[self.rank]
             self._coater = engine.coat
```

### Comparing `nebulae-0.6.7/nebulae/kit/__init__.py` & `nebulae-0.6.9/nebulae/kit/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/kit/decorator.py` & `nebulae-0.6.9/nebulae/kit/decorator.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,26 +33,14 @@
         if not isinstance(ret, tuple):
             ret = (ret,)
         return (_t - t_,) + ret
 
     return _wrapper
 
 
-# def Formula(fn):
-#     def _decorator(func):
-#         def _wrapper(*args, **kwargs):
-#             ret = func(*args, **kwargs)
-#             ret.pods = fn
-#             return ret
-#
-#         return _wrapper
-#
-#     return _decorator
-
-
 def SPST(func):
     def _wrapper(*args, **kwargs):
         cv2.setNumThreads(0)
         cv2.ocl.setUseOpenCL(False)
         return func(*args, **kwargs)
 
     return _wrapper
```

### Comparing `nebulae-0.6.7/nebulae/kit/utility.py` & `nebulae-0.6.9/nebulae/kit/utility.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/law/__init__.py` & `nebulae-0.6.9/nebulae/law/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/nebulae/law/constant.py` & `nebulae-0.6.9/nebulae/law/constant.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,12 +20,13 @@
          `\--\_    -. ___ .-    _/--/‘
    ===========  \__  NOBUG  __/  ===========
    
 '''
 # -*- coding:utf-8 -*-
 class Constant(object):
     CORE = 'PYTORCH'
+    ENV_RANK = 'NEB_RANK'
     FIELD_SEP = '"'
     CHAR_SEP = ','
     FRAME_KEY = '_MAX_FRAMES'
     VALID_DTYPE = ['uint8', 'uint16', 'uint32', 'int8', 'int16', 'int32', 'int64',
                     'float16', 'float32', 'float64', 'str', 'bool']
```

### Comparing `nebulae-0.6.7/nebulae.egg-info/PKG-INFO` & `nebulae-0.6.9/nebulae.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nebulae
-Version: 0.6.7
-Summary: A novel and simple framework based on prevalent DL frameworks and other image processing libs. v0.6.7: fix bugs of device allocation and attribute getter in EMA; add on_device argument in EMA for faster update with higher memory occupied; add gearbox argument in Engine to apply Module.compile() in PyTorch 2.
+Version: 0.6.9
+Summary: A novel and simple framework based on prevalent DL frameworks and other image processing libs. v0.6.9: replace 'RANK' with 'NEB_RANK' for distributed training in environ variables; add subdir argument in DashBoard.log(); add wipe argument in DashBoard.gauge()
 Home-page: https://github.com/
 Author: Seria
 Author-email: zzqsummerai@yeah.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nebulae-0.6.7/nebulae.egg-info/SOURCES.txt` & `nebulae-0.6.9/nebulae.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.7/setup.py` & `nebulae-0.6.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,21 +26,24 @@
 import setuptools
 
 with open("Nebulae_Brochure.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nebulae",
-    version="0.6.7",
+    version="0.6.9",
     author="Seria",
     author_email="zzqsummerai@yeah.net",
     description="A novel and simple framework based on prevalent DL frameworks and other image processing libs."
-                + " v0.6.7: fix bugs of device allocation and attribute getter in EMA;"
-                + " add on_device argument in EMA for faster update with higher memory occupied;"
-                + " add gearbox argument in Engine to apply Module.compile() in PyTorch 2.",
+                + " v0.6.9: replace 'RANK' with 'NEB_RANK' for distributed training in environ variables;"
+                + " add subdir argument in DashBoard.log(); add wipe argument in DashBoard.gauge()",
+                # + " v0.6.8: TimeMachine supports optz input as a dictionary.",
+                # + " v0.6.7: fix bugs of device allocation and attribute getter in EMA;"
+                # + " add on_device argument in EMA for faster update with higher memory occupied;"
+                # + " add gearbox argument in Engine to apply Module.compile() in PyTorch 2.",
                 # + " v0.6.6: add in_loop and last_for args in DashBoard.gauge().",
                 # + " v0.6.5: remove ControlPanel; add in_loop and last_for args in DashBoard.gauge;"
                 # + " add Lamb optimizer; replace BluePrint module with Inspector.",
                 # + " v0.6.4: DashBoard.log() now plots curves only by metrics;"
                 # + " add Scatter, Gather, Tile, Argmax, Argmin in dock; add Lion and delete AdaBelief in optimizers.",
                 # + " v0.6.3: OHEM loss supports an additional mask as input.",
                 # + " v0.6.2: change plot tools from matplotlib to seaborn;"
@@ -189,15 +192,15 @@
                 # + " v0.0.15: fix a bug would lead to wrong implementation of ** symbol."
                 # + " v0.0.14: unable to assemble DUPLICATE component without name but passing existent name is allowed."
                 # + " v0.0.13: allow users to assemble DUPLICATE component without passing name;"
                 # + " add RESIZE component;"
                 # + " shorten automatically generated component names."
                 # + " v0.0.12: fix wrong implementation on data augmentation;"
                 # + " FuelGenerator will keep original image size if width or height is not given.",
-                # sudo python setup.py sdist bdist_wheel && sudo twine upload dist/*
+                # sudo python cleanup.py && sudo python setup.py sdist bdist_wheel && twine upload dist/*
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/",
     packages=setuptools.find_packages(),
     install_requires=
     ['h5py',
      'pillow',
```

