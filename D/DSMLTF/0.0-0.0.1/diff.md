# Comparing `tmp/DSMLTF-0.0.tar.gz` & `tmp/DSMLTF-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/DSMLTF-0.0.tar", last modified: Fri May 12 20:22:42 2023, max compression
+gzip compressed data, was "dist/DSMLTF-0.0.1.tar", last modified: Sun May 14 07:34:23 2023, max compression
```

## Comparing `DSMLTF-0.0.tar` & `DSMLTF-0.0.1.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-05-12 20:22:42.000000 DSMLTF-0.0/
-drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-05-12 20:22:42.000000 DSMLTF-0.0/DSMLTF/
--rwxr-xr-x   0 sergejzuev   (501) staff       (20)       27 2023-05-12 20:11:31.000000 DSMLTF-0.0/DSMLTF/__init__.py
--rw-r--r--   0 sergejzuev   (501) staff       (20)    33331 2023-05-12 20:12:50.000000 DSMLTF-0.0/DSMLTF/dsmltf.py
-drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-05-12 20:22:42.000000 DSMLTF-0.0/DSMLTF.egg-info/
--rw-r--r--   0 sergejzuev   (501) staff       (20)      232 2023-05-12 20:22:41.000000 DSMLTF-0.0/DSMLTF.egg-info/PKG-INFO
--rw-r--r--   0 sergejzuev   (501) staff       (20)      203 2023-05-12 20:22:42.000000 DSMLTF-0.0/DSMLTF.egg-info/SOURCES.txt
--rw-r--r--   0 sergejzuev   (501) staff       (20)        1 2023-05-12 20:22:41.000000 DSMLTF-0.0/DSMLTF.egg-info/dependency_links.txt
--rw-r--r--   0 sergejzuev   (501) staff       (20)        1 2023-05-12 20:22:41.000000 DSMLTF-0.0/DSMLTF.egg-info/not-zip-safe
--rw-r--r--   0 sergejzuev   (501) staff       (20)        7 2023-05-12 20:22:41.000000 DSMLTF-0.0/DSMLTF.egg-info/top_level.txt
--rw-r--r--   0 sergejzuev   (501) staff       (20)      232 2023-05-12 20:22:42.000000 DSMLTF-0.0/PKG-INFO
--rw-r--r--   0 sergejzuev   (501) staff       (20)       38 2023-05-12 20:22:42.000000 DSMLTF-0.0/setup.cfg
--rw-r--r--   0 sergejzuev   (501) staff       (20)      234 2023-05-12 20:21:53.000000 DSMLTF-0.0/setup.py
+drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-05-14 07:34:23.000000 DSMLTF-0.0.1/
+drwxr-xr-x   0 sergejzuev   (501) staff       (20)        0 2023-05-14 07:34:23.000000 DSMLTF-0.0.1/DSMLTF.egg-info/
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      695 2023-05-14 07:34:23.000000 DSMLTF-0.0.1/DSMLTF.egg-info/PKG-INFO
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      177 2023-05-14 07:34:23.000000 DSMLTF-0.0.1/DSMLTF.egg-info/SOURCES.txt
+-rw-r--r--   0 sergejzuev   (501) staff       (20)        1 2023-05-14 07:34:23.000000 DSMLTF-0.0.1/DSMLTF.egg-info/dependency_links.txt
+-rw-r--r--   0 sergejzuev   (501) staff       (20)       17 2023-05-14 07:34:23.000000 DSMLTF-0.0.1/DSMLTF.egg-info/requires.txt
+-rw-r--r--   0 sergejzuev   (501) staff       (20)        1 2023-05-14 07:34:23.000000 DSMLTF-0.0.1/DSMLTF.egg-info/top_level.txt
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      695 2023-05-14 07:34:23.000000 DSMLTF-0.0.1/PKG-INFO
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      284 2023-05-14 06:17:21.000000 DSMLTF-0.0.1/README.md
+-rw-r--r--   0 sergejzuev   (501) staff       (20)       38 2023-05-14 07:34:23.000000 DSMLTF-0.0.1/setup.cfg
+-rw-r--r--   0 sergejzuev   (501) staff       (20)      611 2023-05-14 07:34:11.000000 DSMLTF-0.0.1/setup.py
```

