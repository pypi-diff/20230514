# Comparing `tmp/wireprobe-0.1.7.tar.gz` & `tmp/wireprobe-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wireprobe-0.1.7.tar", last modified: Sun May 14 14:10:45 2023, max compression
+gzip compressed data, was "wireprobe-0.1.9.tar", last modified: Sun May 14 14:37:14 2023, max compression
```

## Comparing `wireprobe-0.1.7.tar` & `wireprobe-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:10:45.634052 wireprobe-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-14 14:10:34.000000 wireprobe-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-14 14:10:45.634052 wireprobe-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-14 14:10:34.000000 wireprobe-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:10:45.630052 wireprobe-0.1.7/fabfile/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:10:45.630052 wireprobe-0.1.7/fabfile/Config/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-14 14:10:34.000000 wireprobe-0.1.7/fabfile/Config/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:10:34.000000 wireprobe-0.1.7/fabfile/Config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:10:45.630052 wireprobe-0.1.7/fabfile/Notifications/
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-14 14:10:34.000000 wireprobe-0.1.7/fabfile/Notifications/Telegram.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:10:34.000000 wireprobe-0.1.7/fabfile/Notifications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:10:45.634052 wireprobe-0.1.7/fabfile/wireprobe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-14 14:10:45.000000 wireprobe-0.1.7/fabfile/wireprobe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-14 14:10:45.000000 wireprobe-0.1.7/fabfile/wireprobe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 14:10:45.000000 wireprobe-0.1.7/fabfile/wireprobe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-14 14:10:45.000000 wireprobe-0.1.7/fabfile/wireprobe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-14 14:10:45.000000 wireprobe-0.1.7/fabfile/wireprobe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 14:10:45.634052 wireprobe-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-14 14:10:34.000000 wireprobe-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:37:14.249445 wireprobe-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-14 14:37:01.000000 wireprobe-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-14 14:37:14.249445 wireprobe-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-14 14:37:01.000000 wireprobe-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:37:14.249445 wireprobe-0.1.9/fabfile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:37:14.249445 wireprobe-0.1.9/fabfile/Config/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-14 14:37:01.000000 wireprobe-0.1.9/fabfile/Config/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:37:01.000000 wireprobe-0.1.9/fabfile/Config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-14 14:37:01.000000 wireprobe-0.1.9/fabfile/HealthCheck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:37:14.249445 wireprobe-0.1.9/fabfile/Notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-14 14:37:01.000000 wireprobe-0.1.9/fabfile/Notifications/Telegram.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:37:01.000000 wireprobe-0.1.9/fabfile/Notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-14 14:37:01.000000 wireprobe-0.1.9/fabfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 14:37:14.249445 wireprobe-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-14 14:37:01.000000 wireprobe-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:37:14.249445 wireprobe-0.1.9/wireprobe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-14 14:37:14.000000 wireprobe-0.1.9/wireprobe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-14 14:37:14.000000 wireprobe-0.1.9/wireprobe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 14:37:14.000000 wireprobe-0.1.9/wireprobe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-14 14:37:14.000000 wireprobe-0.1.9/wireprobe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-14 14:37:14.000000 wireprobe-0.1.9/wireprobe.egg-info/top_level.txt
```

### Comparing `wireprobe-0.1.7/LICENSE` & `wireprobe-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wireprobe-0.1.7/README.md` & `wireprobe-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `wireprobe-0.1.7/fabfile/Notifications/Telegram.py` & `wireprobe-0.1.9/fabfile/Notifications/Telegram.py`

 * *Files identical despite different names*

