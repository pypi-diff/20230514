# Comparing `tmp/aiuv-0.5.tar.gz` & `tmp/aiuv-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiuv-0.5.tar", last modified: Thu May 11 16:10:49 2023, max compression
+gzip compressed data, was "aiuv-0.6.tar", last modified: Sun May 14 05:44:58 2023, max compression
```

## Comparing `aiuv-0.5.tar` & `aiuv-0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 16:10:49.409531 aiuv-0.5/
--rw-rw-rw-   0        0        0        0 2023-05-11 10:25:19.000000 aiuv-0.5/Licence.txt
--rw-rw-rw-   0        0        0      144 2023-05-11 16:10:49.401527 aiuv-0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-11 16:10:49.401527 aiuv-0.5/aiuv.egg-info/
--rw-rw-rw-   0        0        0      144 2023-05-11 16:10:49.000000 aiuv-0.5/aiuv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      148 2023-05-11 16:10:49.000000 aiuv-0.5/aiuv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 16:10:49.000000 aiuv-0.5/aiuv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-05-11 16:10:49.000000 aiuv-0.5/aiuv.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-11 16:10:49.401527 aiuv-0.5/pkg/
--rw-rw-rw-   0        0        0    18012 2023-05-11 16:09:32.000000 aiuv-0.5/pkg/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-11 16:10:49.409531 aiuv-0.5/setup.cfg
--rw-rw-rw-   0        0        0      183 2023-05-11 16:10:44.000000 aiuv-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 05:44:58.421092 aiuv-0.6/
+-rw-rw-rw-   0        0        0        0 2023-05-11 10:25:19.000000 aiuv-0.6/Licence.txt
+-rw-rw-rw-   0        0        0      144 2023-05-14 05:44:58.421092 aiuv-0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-14 05:44:58.413092 aiuv-0.6/aiuv.egg-info/
+-rw-rw-rw-   0        0        0      144 2023-05-14 05:44:58.000000 aiuv-0.6/aiuv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      148 2023-05-14 05:44:58.000000 aiuv-0.6/aiuv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 05:44:58.000000 aiuv-0.6/aiuv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-05-14 05:44:58.000000 aiuv-0.6/aiuv.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 05:44:58.413092 aiuv-0.6/pkg/
+-rw-rw-rw-   0        0        0    31290 2023-05-14 05:38:54.000000 aiuv-0.6/pkg/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-14 05:44:58.421092 aiuv-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      183 2023-05-14 05:44:26.000000 aiuv-0.6/setup.py
```

