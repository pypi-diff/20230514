# Comparing `tmp/pynterface-0.0.0.tar.gz` & `tmp/pynterface-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynterface-0.0.0.tar", last modified: Sun May 14 04:00:41 2023, max compression
+gzip compressed data, was "pynterface-0.0.1.tar", last modified: Sun May 14 18:06:37 2023, max compression
```

## Comparing `pynterface-0.0.0.tar` & `pynterface-0.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-14 04:00:41.968570 pynterface-0.0.0/
--rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-05-04 02:59:32.000000 pynterface-0.0.0/LICENSE
--rw-r--r--   0 vivaan     (501) staff       (20)       33 2023-05-14 03:48:17.000000 pynterface-0.0.0/MANIFEST.in
--rw-r--r--   0 vivaan     (501) staff       (20)      321 2023-05-14 04:00:41.968289 pynterface-0.0.0/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)       66 2023-05-09 01:55:04.000000 pynterface-0.0.0/README.md
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-14 04:00:41.966428 pynterface-0.0.0/pynterface/
--rw-r--r--   0 vivaan     (501) staff       (20)      238 2023-05-14 02:09:21.000000 pynterface-0.0.0/pynterface/__init__.py
--rw-r--r--   0 vivaan     (501) staff       (20)     2840 2023-05-14 01:50:32.000000 pynterface-0.0.0/pynterface/input.py
--rw-r--r--   0 vivaan     (501) staff       (20)     6495 2023-05-09 23:26:51.000000 pynterface-0.0.0/pynterface/loading.py
--rw-r--r--   0 vivaan     (501) staff       (20)     3525 2023-05-14 01:47:16.000000 pynterface-0.0.0/pynterface/menu.py
--rw-r--r--   0 vivaan     (501) staff       (20)     5209 2023-05-14 02:09:21.000000 pynterface-0.0.0/pynterface/printing.py
--rw-r--r--   0 vivaan     (501) staff       (20)     5848 2023-05-14 02:31:12.000000 pynterface-0.0.0/pynterface/style.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-14 04:00:41.967949 pynterface-0.0.0/pynterface.egg-info/
--rw-r--r--   0 vivaan     (501) staff       (20)      321 2023-05-14 04:00:41.000000 pynterface-0.0.0/pynterface.egg-info/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)      301 2023-05-14 04:00:41.000000 pynterface-0.0.0/pynterface.egg-info/SOURCES.txt
--rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-05-14 04:00:41.000000 pynterface-0.0.0/pynterface.egg-info/dependency_links.txt
--rw-r--r--   0 vivaan     (501) staff       (20)       11 2023-05-14 04:00:41.000000 pynterface-0.0.0/pynterface.egg-info/top_level.txt
--rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-05-14 04:00:41.968648 pynterface-0.0.0/setup.cfg
--rw-r--r--   0 vivaan     (501) staff       (20)      515 2023-05-14 03:58:35.000000 pynterface-0.0.0/setup.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-14 18:06:37.295855 pynterface-0.0.1/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-05-04 02:59:32.000000 pynterface-0.0.1/LICENSE
+-rw-r--r--   0 vivaan     (501) staff       (20)       33 2023-05-14 03:48:17.000000 pynterface-0.0.1/MANIFEST.in
+-rw-r--r--   0 vivaan     (501) staff       (20)     1484 2023-05-14 18:06:37.295554 pynterface-0.0.1/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)     1156 2023-05-14 04:10:04.000000 pynterface-0.0.1/README.md
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-14 18:06:37.293350 pynterface-0.0.1/pynterface/
+-rw-r--r--   0 vivaan     (501) staff       (20)      238 2023-05-14 18:02:44.000000 pynterface-0.0.1/pynterface/__init__.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     2840 2023-05-14 01:50:32.000000 pynterface-0.0.1/pynterface/input.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     6495 2023-05-09 23:26:51.000000 pynterface-0.0.1/pynterface/loading.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     3525 2023-05-14 01:47:16.000000 pynterface-0.0.1/pynterface/menu.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     5209 2023-05-14 02:09:21.000000 pynterface-0.0.1/pynterface/printing.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     5848 2023-05-14 02:31:12.000000 pynterface-0.0.1/pynterface/style.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-14 18:06:37.295192 pynterface-0.0.1/pynterface.egg-info/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1484 2023-05-14 18:06:37.000000 pynterface-0.0.1/pynterface.egg-info/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)      301 2023-05-14 18:06:37.000000 pynterface-0.0.1/pynterface.egg-info/SOURCES.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-05-14 18:06:37.000000 pynterface-0.0.1/pynterface.egg-info/dependency_links.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)       11 2023-05-14 18:06:37.000000 pynterface-0.0.1/pynterface.egg-info/top_level.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-05-14 18:06:37.295957 pynterface-0.0.1/setup.cfg
+-rw-r--r--   0 vivaan     (501) staff       (20)      612 2023-05-14 04:04:56.000000 pynterface-0.0.1/setup.py
```

### Comparing `pynterface-0.0.0/LICENSE` & `pynterface-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynterface-0.0.0/pynterface/input.py` & `pynterface-0.0.1/pynterface/input.py`

 * *Files identical despite different names*

### Comparing `pynterface-0.0.0/pynterface/loading.py` & `pynterface-0.0.1/pynterface/loading.py`

 * *Files identical despite different names*

### Comparing `pynterface-0.0.0/pynterface/menu.py` & `pynterface-0.0.1/pynterface/menu.py`

 * *Files identical despite different names*

### Comparing `pynterface-0.0.0/pynterface/printing.py` & `pynterface-0.0.1/pynterface/printing.py`

 * *Files identical despite different names*

### Comparing `pynterface-0.0.0/pynterface/style.py` & `pynterface-0.0.1/pynterface/style.py`

 * *Files identical despite different names*

