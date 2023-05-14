# Comparing `tmp/pysyn_data-0.3.tar.gz` & `tmp/pysyn_data-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pysyn_data-0.3.tar", last modified: Wed Mar 22 02:00:33 2023, max compression
+gzip compressed data, was "pysyn_data-0.3.1.tar", last modified: Sun May 14 18:54:30 2023, max compression
```

## Comparing `pysyn_data-0.3.tar` & `pysyn_data-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 alokh     (1015) alokh     (1015)        0 2023-03-22 02:00:33.000000 pysyn_data-0.3/
--rw-rw-r--   0 alokh     (1015) alokh     (1015)     2272 2023-03-22 02:00:33.000000 pysyn_data-0.3/PKG-INFO
--rw-rw-r--   0 alokh     (1015) alokh     (1015)     1386 2023-03-22 01:44:30.000000 pysyn_data-0.3/README.md
--rw-rw-r--   0 alokh     (1015) alokh     (1015)     1429 2023-03-22 01:49:07.000000 pysyn_data-0.3/README.rst
-drwxrwxr-x   0 alokh     (1015) alokh     (1015)        0 2023-03-22 02:00:33.000000 pysyn_data-0.3/pysyn_data/
--rw-rw-r--   0 alokh     (1015) alokh     (1015)    18350 2023-03-22 00:33:31.000000 pysyn_data-0.3/pysyn_data/__init__.py
-drwxrwxr-x   0 alokh     (1015) alokh     (1015)        0 2023-03-22 02:00:33.000000 pysyn_data-0.3/pysyn_data.egg-info/
--rw-rw-r--   0 alokh     (1015) alokh     (1015)     2272 2023-03-22 02:00:33.000000 pysyn_data-0.3/pysyn_data.egg-info/PKG-INFO
--rw-rw-r--   0 alokh     (1015) alokh     (1015)      188 2023-03-22 02:00:33.000000 pysyn_data-0.3/pysyn_data.egg-info/SOURCES.txt
--rw-rw-r--   0 alokh     (1015) alokh     (1015)        1 2023-03-22 02:00:33.000000 pysyn_data-0.3/pysyn_data.egg-info/dependency_links.txt
--rw-rw-r--   0 alokh     (1015) alokh     (1015)       11 2023-03-22 02:00:33.000000 pysyn_data-0.3/pysyn_data.egg-info/top_level.txt
--rw-rw-r--   0 alokh     (1015) alokh     (1015)       38 2023-03-22 02:00:33.000000 pysyn_data-0.3/setup.cfg
--rw-rw-r--   0 alokh     (1015) alokh     (1015)      835 2023-03-22 02:00:30.000000 pysyn_data-0.3/setup.py
+drwxrwxr-x   0 alokh     (1015) alokh     (1015)        0 2023-05-14 18:54:30.799362 pysyn_data-0.3.1/
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)     2194 2023-05-14 18:54:30.795362 pysyn_data-0.3.1/PKG-INFO
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)        0 2023-05-14 18:54:30.000000 pysyn_data-0.3.1/README.md
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)     1429 2023-03-22 01:49:07.000000 pysyn_data-0.3.1/README.rst
+drwxrwxr-x   0 alokh     (1015) alokh     (1015)        0 2023-05-14 18:54:30.795362 pysyn_data-0.3.1/pysyn_data/
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)    18350 2023-03-22 00:33:31.000000 pysyn_data-0.3.1/pysyn_data/__init__.py
+drwxrwxr-x   0 alokh     (1015) alokh     (1015)        0 2023-05-14 18:54:30.795362 pysyn_data-0.3.1/pysyn_data.egg-info/
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)     2194 2023-05-14 18:54:30.000000 pysyn_data-0.3.1/pysyn_data.egg-info/PKG-INFO
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)      188 2023-05-14 18:54:30.000000 pysyn_data-0.3.1/pysyn_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)        1 2023-05-14 18:54:30.000000 pysyn_data-0.3.1/pysyn_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)       11 2023-05-14 18:54:30.000000 pysyn_data-0.3.1/pysyn_data.egg-info/top_level.txt
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)       38 2023-05-14 18:54:30.799362 pysyn_data-0.3.1/setup.cfg
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)        0 2023-05-14 18:54:30.000000 pysyn_data-0.3.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pysyn_data-0.3/README.rst` & `pysyn_data-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `pysyn_data-0.3/pysyn_data/__init__.py` & `pysyn_data-0.3.1/pysyn_data/__init__.py`

 * *Files identical despite different names*

