# Comparing `tmp/wireprobe-0.1.4.tar.gz` & `tmp/wireprobe-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wireprobe-0.1.4.tar", last modified: Sun May 14 13:42:30 2023, max compression
+gzip compressed data, was "wireprobe-0.1.5.tar", last modified: Sun May 14 14:01:08 2023, max compression
```

## Comparing `wireprobe-0.1.4.tar` & `wireprobe-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 13:42:30.025195 wireprobe-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-14 13:42:17.000000 wireprobe-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-14 13:42:30.025195 wireprobe-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-14 13:42:17.000000 wireprobe-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 13:42:30.029195 wireprobe-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-14 13:42:17.000000 wireprobe-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 13:42:30.025195 wireprobe-0.1.4/wireprobe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-14 13:42:30.000000 wireprobe-0.1.4/wireprobe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-14 13:42:30.000000 wireprobe-0.1.4/wireprobe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 13:42:30.000000 wireprobe-0.1.4/wireprobe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-14 13:42:30.000000 wireprobe-0.1.4/wireprobe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 13:42:30.000000 wireprobe-0.1.4/wireprobe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:01:08.701011 wireprobe-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-14 14:00:57.000000 wireprobe-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-14 14:01:08.701011 wireprobe-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-14 14:00:57.000000 wireprobe-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 14:01:08.701011 wireprobe-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-14 14:00:57.000000 wireprobe-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:01:08.701011 wireprobe-0.1.5/wireprobe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-14 14:01:08.000000 wireprobe-0.1.5/wireprobe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-14 14:01:08.000000 wireprobe-0.1.5/wireprobe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 14:01:08.000000 wireprobe-0.1.5/wireprobe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-14 14:01:08.000000 wireprobe-0.1.5/wireprobe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 14:01:08.000000 wireprobe-0.1.5/wireprobe.egg-info/top_level.txt
```

### Comparing `wireprobe-0.1.4/LICENSE` & `wireprobe-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wireprobe-0.1.4/README.md` & `wireprobe-0.1.5/README.md`

 * *Files identical despite different names*

