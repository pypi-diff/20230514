# Comparing `tmp/nazo_image_utils-0.0.1.tar.gz` & `tmp/nazo_image_utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nazo_image_utils-0.0.1.tar", last modified: Sat May 13 10:29:48 2023, max compression
+gzip compressed data, was "nazo_image_utils-0.0.2.tar", last modified: Sun May 14 05:59:28 2023, max compression
```

## Comparing `nazo_image_utils-0.0.1.tar` & `nazo_image_utils-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 10:29:48.803513 nazo_image_utils-0.0.1/
--rw-rw-rw-   0        0        0      125 2023-05-13 10:29:10.000000 nazo_image_utils-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      728 2023-05-13 10:29:48.803513 nazo_image_utils-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-13 10:29:10.000000 nazo_image_utils-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-13 10:29:48.803513 nazo_image_utils-0.0.1/nazo_image_utils/
--rw-rw-rw-   0        0        0      123 2023-05-13 10:29:10.000000 nazo_image_utils-0.0.1/nazo_image_utils/__init__.py
--rw-rw-rw-   0        0        0     7345 2023-05-13 10:29:10.000000 nazo_image_utils-0.0.1/nazo_image_utils/process_image.py
--rw-rw-rw-   0        0        0   314004 2023-05-13 10:29:48.000000 nazo_image_utils-0.0.1/nazo_image_utils/rand_image.cpp
--rw-rw-rw-   0        0        0     1319 2023-05-13 10:29:10.000000 nazo_image_utils-0.0.1/nazo_image_utils/rand_image.pyi
--rw-rw-rw-   0        0        0     4651 2023-05-13 10:29:10.000000 nazo_image_utils-0.0.1/nazo_image_utils/rand_image.pyx
-drwxrwxrwx   0        0        0        0 2023-05-13 10:29:48.803513 nazo_image_utils-0.0.1/nazo_image_utils.egg-info/
--rw-rw-rw-   0        0        0      728 2023-05-13 10:29:48.000000 nazo_image_utils-0.0.1/nazo_image_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-05-13 10:29:48.000000 nazo_image_utils-0.0.1/nazo_image_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 10:29:48.000000 nazo_image_utils-0.0.1/nazo_image_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-13 10:29:48.000000 nazo_image_utils-0.0.1/nazo_image_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      602 2023-05-13 10:29:10.000000 nazo_image_utils-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-13 10:29:48.803513 nazo_image_utils-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2035 2023-05-13 10:29:10.000000 nazo_image_utils-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 05:59:28.649950 nazo_image_utils-0.0.2/
+-rw-rw-rw-   0        0        0      125 2023-05-14 05:58:40.000000 nazo_image_utils-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3747 2023-05-14 05:59:28.649950 nazo_image_utils-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2839 2023-05-14 05:58:40.000000 nazo_image_utils-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 05:59:28.649950 nazo_image_utils-0.0.2/nazo_image_utils/
+-rw-rw-rw-   0        0        0      123 2023-05-14 05:58:40.000000 nazo_image_utils-0.0.2/nazo_image_utils/__init__.py
+-rw-rw-rw-   0        0        0     7345 2023-05-14 05:58:40.000000 nazo_image_utils-0.0.2/nazo_image_utils/process_image.py
+-rw-rw-rw-   0        0        0   314004 2023-05-14 05:59:27.000000 nazo_image_utils-0.0.2/nazo_image_utils/rand_image.cpp
+-rw-rw-rw-   0        0        0     1319 2023-05-14 05:58:40.000000 nazo_image_utils-0.0.2/nazo_image_utils/rand_image.pyi
+-rw-rw-rw-   0        0        0     4651 2023-05-14 05:58:40.000000 nazo_image_utils-0.0.2/nazo_image_utils/rand_image.pyx
+drwxrwxrwx   0        0        0        0 2023-05-14 05:59:28.649950 nazo_image_utils-0.0.2/nazo_image_utils.egg-info/
+-rw-rw-rw-   0        0        0     3747 2023-05-14 05:59:28.000000 nazo_image_utils-0.0.2/nazo_image_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2023-05-14 05:59:28.000000 nazo_image_utils-0.0.2/nazo_image_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 05:59:28.000000 nazo_image_utils-0.0.2/nazo_image_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-05-14 05:59:28.000000 nazo_image_utils-0.0.2/nazo_image_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-14 05:59:28.000000 nazo_image_utils-0.0.2/nazo_image_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1640 2023-05-14 05:58:40.000000 nazo_image_utils-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-14 05:59:28.649950 nazo_image_utils-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1253 2023-05-14 05:58:40.000000 nazo_image_utils-0.0.2/setup.py
```

### Comparing `nazo_image_utils-0.0.1/nazo_image_utils/process_image.py` & `nazo_image_utils-0.0.2/nazo_image_utils/process_image.py`

 * *Files identical despite different names*

### Comparing `nazo_image_utils-0.0.1/nazo_image_utils/rand_image.cpp` & `nazo_image_utils-0.0.2/nazo_image_utils/rand_image.cpp`

 * *Files identical despite different names*

### Comparing `nazo_image_utils-0.0.1/nazo_image_utils/rand_image.pyi` & `nazo_image_utils-0.0.2/nazo_image_utils/rand_image.pyi`

 * *Files identical despite different names*

### Comparing `nazo_image_utils-0.0.1/nazo_image_utils/rand_image.pyx` & `nazo_image_utils-0.0.2/nazo_image_utils/rand_image.pyx`

 * *Files identical despite different names*

