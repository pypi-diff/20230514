# Comparing `tmp/elastiknn-client-8.6.2.1.tar.gz` & `tmp/elastiknn-client-8.7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/elastiknn-client-8.6.2.1.tar", last modified: Mon Feb 27 22:27:51 2023, max compression
+gzip compressed data, was "dist/elastiknn-client-8.7.0.0.tar", last modified: Sat Apr  8 04:38:27 2023, max compression
```

## Comparing `elastiknn-client-8.6.2.1.tar` & `elastiknn-client-8.7.0.0.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 22:27:51.000000 elastiknn-client-8.6.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-27 22:27:09.000000 elastiknn-client-8.6.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-02-27 22:27:51.000000 elastiknn-client-8.6.2.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 22:27:51.000000 elastiknn-client-8.6.2.1/elastiknn/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-27 22:27:09.000000 elastiknn-client-8.6.2.1/elastiknn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-02-27 22:27:09.000000 elastiknn-client-8.6.2.1/elastiknn/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-02-27 22:27:09.000000 elastiknn-client-8.6.2.1/elastiknn/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-02-27 22:27:09.000000 elastiknn-client-8.6.2.1/elastiknn/codec.py
--rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-02-27 22:27:09.000000 elastiknn-client-8.6.2.1/elastiknn/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-02-27 22:27:09.000000 elastiknn-client-8.6.2.1/elastiknn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 22:27:51.000000 elastiknn-client-8.6.2.1/elastiknn_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-02-27 22:27:51.000000 elastiknn-client-8.6.2.1/elastiknn_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-02-27 22:27:51.000000 elastiknn-client-8.6.2.1/elastiknn_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 22:27:51.000000 elastiknn-client-8.6.2.1/elastiknn_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-02-27 22:27:51.000000 elastiknn-client-8.6.2.1/elastiknn_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-27 22:27:51.000000 elastiknn-client-8.6.2.1/elastiknn_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 22:27:51.000000 elastiknn-client-8.6.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-02-27 22:27:09.000000 elastiknn-client-8.6.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 04:38:27.000000 elastiknn-client-8.7.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-08 04:37:40.000000 elastiknn-client-8.7.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-08 04:38:27.000000 elastiknn-client-8.7.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 04:38:27.000000 elastiknn-client-8.7.0.0/elastiknn/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-08 04:37:40.000000 elastiknn-client-8.7.0.0/elastiknn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-04-08 04:37:40.000000 elastiknn-client-8.7.0.0/elastiknn/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-08 04:37:40.000000 elastiknn-client-8.7.0.0/elastiknn/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-08 04:37:40.000000 elastiknn-client-8.7.0.0/elastiknn/codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-04-08 04:37:40.000000 elastiknn-client-8.7.0.0/elastiknn/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-08 04:37:40.000000 elastiknn-client-8.7.0.0/elastiknn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 04:38:27.000000 elastiknn-client-8.7.0.0/elastiknn_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-08 04:38:27.000000 elastiknn-client-8.7.0.0/elastiknn_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-08 04:38:27.000000 elastiknn-client-8.7.0.0/elastiknn_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 04:38:27.000000 elastiknn-client-8.7.0.0/elastiknn_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-08 04:38:27.000000 elastiknn-client-8.7.0.0/elastiknn_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-08 04:38:27.000000 elastiknn-client-8.7.0.0/elastiknn_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 04:38:27.000000 elastiknn-client-8.7.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-08 04:37:40.000000 elastiknn-client-8.7.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 04:38:27.000000 elastiknn-client-8.7.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-08 04:37:40.000000 elastiknn-client-8.7.0.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-08 04:37:40.000000 elastiknn-client-8.7.0.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-08 04:37:40.000000 elastiknn-client-8.7.0.0/tests/test_utils.py
```

### Comparing `elastiknn-client-8.6.2.1/elastiknn/api.py` & `elastiknn-client-8.7.0.0/elastiknn/api.py`

 * *Files identical despite different names*

### Comparing `elastiknn-client-8.6.2.1/elastiknn/client.py` & `elastiknn-client-8.7.0.0/elastiknn/client.py`

 * *Files identical despite different names*

### Comparing `elastiknn-client-8.6.2.1/elastiknn/models.py` & `elastiknn-client-8.7.0.0/elastiknn/models.py`

 * *Files identical despite different names*

### Comparing `elastiknn-client-8.6.2.1/elastiknn/utils.py` & `elastiknn-client-8.7.0.0/elastiknn/utils.py`

 * *Files identical despite different names*

### Comparing `elastiknn-client-8.6.2.1/setup.py` & `elastiknn-client-8.7.0.0/setup.py`

 * *Files identical despite different names*

