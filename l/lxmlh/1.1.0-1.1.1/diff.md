# Comparing `tmp/lxmlh-1.1.0.tar.gz` & `tmp/lxmlh-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lxmlh-1.1.0.tar", last modified: Mon Mar 27 01:49:09 2023, max compression
+gzip compressed data, was "lxmlh-1.1.1.tar", last modified: Sun May 14 12:59:33 2023, max compression
```

## Comparing `lxmlh-1.1.0.tar` & `lxmlh-1.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 01:49:09.636522 lxmlh-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-03-27 01:48:56.000000 lxmlh-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-27 01:48:56.000000 lxmlh-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-03-27 01:49:09.636522 lxmlh-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-03-27 01:48:56.000000 lxmlh-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 01:49:09.632522 lxmlh-1.1.0/lxmlh/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-27 01:48:56.000000 lxmlh-1.1.0/lxmlh/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-03-27 01:48:56.000000 lxmlh-1.1.0/lxmlh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-03-27 01:48:56.000000 lxmlh-1.1.0/lxmlh/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-03-27 01:48:56.000000 lxmlh-1.1.0/lxmlh/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-03-27 01:48:56.000000 lxmlh-1.1.0/lxmlh/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 01:49:09.636522 lxmlh-1.1.0/lxmlh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-03-27 01:49:09.000000 lxmlh-1.1.0/lxmlh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-27 01:49:09.000000 lxmlh-1.1.0/lxmlh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 01:49:09.000000 lxmlh-1.1.0/lxmlh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 01:49:09.000000 lxmlh-1.1.0/lxmlh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-27 01:49:09.000000 lxmlh-1.1.0/lxmlh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-27 01:49:09.000000 lxmlh-1.1.0/lxmlh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-27 01:48:56.000000 lxmlh-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-03-27 01:49:09.636522 lxmlh-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 01:49:09.636522 lxmlh-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-03-27 01:48:56.000000 lxmlh-1.1.0/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-03-27 01:48:56.000000 lxmlh-1.1.0/tests/test_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:59:33.885358 lxmlh-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-14 12:59:24.000000 lxmlh-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-14 12:59:24.000000 lxmlh-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-14 12:59:33.885358 lxmlh-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-14 12:59:24.000000 lxmlh-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:59:33.885358 lxmlh-1.1.1/lxmlh/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 12:59:24.000000 lxmlh-1.1.1/lxmlh/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-14 12:59:24.000000 lxmlh-1.1.1/lxmlh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-14 12:59:24.000000 lxmlh-1.1.1/lxmlh/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-05-14 12:59:24.000000 lxmlh-1.1.1/lxmlh/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-05-14 12:59:24.000000 lxmlh-1.1.1/lxmlh/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:59:33.885358 lxmlh-1.1.1/lxmlh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-14 12:59:33.000000 lxmlh-1.1.1/lxmlh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-14 12:59:33.000000 lxmlh-1.1.1/lxmlh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 12:59:33.000000 lxmlh-1.1.1/lxmlh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 12:59:33.000000 lxmlh-1.1.1/lxmlh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-14 12:59:33.000000 lxmlh-1.1.1/lxmlh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-14 12:59:33.000000 lxmlh-1.1.1/lxmlh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-14 12:59:24.000000 lxmlh-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-14 12:59:33.885358 lxmlh-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:59:33.885358 lxmlh-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-14 12:59:24.000000 lxmlh-1.1.1/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-14 12:59:24.000000 lxmlh-1.1.1/tests/test_parsers.py
```

### Comparing `lxmlh-1.1.0/LICENSE` & `lxmlh-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lxmlh-1.1.0/PKG-INFO` & `lxmlh-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lxmlh
-Version: 1.1.0
+Version: 1.1.1
 Summary: lxml helper Python package
 Home-page: https://github.com/sami-m-g/lxmlh
 Author: Mina Sami
 Author-email: <sami.mg@outlook.com>
 Maintainer: Mina Sami
 Maintainer-email: <sami.mg@outlook.com>
 License: BSD license
```

### Comparing `lxmlh-1.1.0/README.md` & `lxmlh-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `lxmlh-1.1.0/lxmlh/__init__.py` & `lxmlh-1.1.1/lxmlh/__init__.py`

 * *Files identical despite different names*

### Comparing `lxmlh-1.1.0/lxmlh/helpers.py` & `lxmlh-1.1.1/lxmlh/helpers.py`

 * *Files identical despite different names*

### Comparing `lxmlh-1.1.0/lxmlh/parsers.py` & `lxmlh-1.1.1/lxmlh/parsers.py`

 * *Files identical despite different names*

### Comparing `lxmlh-1.1.0/lxmlh.egg-info/PKG-INFO` & `lxmlh-1.1.1/lxmlh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lxmlh
-Version: 1.1.0
+Version: 1.1.1
 Summary: lxml helper Python package
 Home-page: https://github.com/sami-m-g/lxmlh
 Author: Mina Sami
 Author-email: <sami.mg@outlook.com>
 Maintainer: Mina Sami
 Maintainer-email: <sami.mg@outlook.com>
 License: BSD license
```

### Comparing `lxmlh-1.1.0/setup.cfg` & `lxmlh-1.1.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=.
 python_requires = >=3.8
 install_requires = 
 	lxml==4.9.2
-	numpy==1.23.3
+	numpy>=1.23.3
 
 [options.packages.find]
 where = .
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `lxmlh-1.1.0/tests/test_helpers.py` & `lxmlh-1.1.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `lxmlh-1.1.0/tests/test_parsers.py` & `lxmlh-1.1.1/tests/test_parsers.py`

 * *Files identical despite different names*

