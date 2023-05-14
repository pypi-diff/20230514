# Comparing `tmp/pdf-annotations-diff-0.0.1.tar.gz` & `tmp/pdf-annotations-diff-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf-annotations-diff-0.0.1.tar", last modified: Sun May 14 09:34:34 2023, max compression
+gzip compressed data, was "pdf-annotations-diff-0.0.2.tar", last modified: Sun May 14 09:47:45 2023, max compression
```

## Comparing `pdf-annotations-diff-0.0.1.tar` & `pdf-annotations-diff-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 sameer    (1000) sameer    (1000)        0 2023-05-14 09:34:34.144170 pdf-annotations-diff-0.0.1/
--rw-r--r--   0 sameer    (1000) sameer    (1000)     1068 2023-05-14 09:08:55.000000 pdf-annotations-diff-0.0.1/LICENSE
--rw-r--r--   0 sameer    (1000) sameer    (1000)      596 2023-05-14 09:34:34.144170 pdf-annotations-diff-0.0.1/PKG-INFO
-drwxr-xr-x   0 sameer    (1000) sameer    (1000)        0 2023-05-14 09:34:34.144170 pdf-annotations-diff-0.0.1/pdf_annotations_diff.egg-info/
--rw-r--r--   0 sameer    (1000) sameer    (1000)      596 2023-05-14 09:34:34.000000 pdf-annotations-diff-0.0.1/pdf_annotations_diff.egg-info/PKG-INFO
--rw-r--r--   0 sameer    (1000) sameer    (1000)      306 2023-05-14 09:34:34.000000 pdf-annotations-diff-0.0.1/pdf_annotations_diff.egg-info/SOURCES.txt
--rw-r--r--   0 sameer    (1000) sameer    (1000)        1 2023-05-14 09:34:34.000000 pdf-annotations-diff-0.0.1/pdf_annotations_diff.egg-info/dependency_links.txt
--rw-r--r--   0 sameer    (1000) sameer    (1000)       67 2023-05-14 09:34:34.000000 pdf-annotations-diff-0.0.1/pdf_annotations_diff.egg-info/entry_points.txt
--rw-r--r--   0 sameer    (1000) sameer    (1000)        8 2023-05-14 09:34:34.000000 pdf-annotations-diff-0.0.1/pdf_annotations_diff.egg-info/requires.txt
--rw-r--r--   0 sameer    (1000) sameer    (1000)       21 2023-05-14 09:34:34.000000 pdf-annotations-diff-0.0.1/pdf_annotations_diff.egg-info/top_level.txt
--rwxr-xr-x   0 sameer    (1000) sameer    (1000)     2909 2023-05-14 09:30:21.000000 pdf-annotations-diff-0.0.1/pdf_annotations_diff.py
--rw-r--r--   0 sameer    (1000) sameer    (1000)       38 2023-05-14 09:34:34.144170 pdf-annotations-diff-0.0.1/setup.cfg
--rw-r--r--   0 sameer    (1000) sameer    (1000)      895 2023-05-14 09:33:50.000000 pdf-annotations-diff-0.0.1/setup.py
+drwxr-xr-x   0 sameer    (1000) sameer    (1000)        0 2023-05-14 09:47:45.256188 pdf-annotations-diff-0.0.2/
+-rw-r--r--   0 sameer    (1000) sameer    (1000)     1068 2023-05-14 09:08:55.000000 pdf-annotations-diff-0.0.2/LICENSE
+-rw-r--r--   0 sameer    (1000) sameer    (1000)     3236 2023-05-14 09:47:45.256188 pdf-annotations-diff-0.0.2/PKG-INFO
+-rw-r--r--   0 sameer    (1000) sameer    (1000)     2599 2023-05-14 09:43:04.000000 pdf-annotations-diff-0.0.2/README.md
+drwxr-xr-x   0 sameer    (1000) sameer    (1000)        0 2023-05-14 09:47:45.256188 pdf-annotations-diff-0.0.2/pdf_annotations_diff.egg-info/
+-rw-r--r--   0 sameer    (1000) sameer    (1000)     3236 2023-05-14 09:47:45.000000 pdf-annotations-diff-0.0.2/pdf_annotations_diff.egg-info/PKG-INFO
+-rw-r--r--   0 sameer    (1000) sameer    (1000)      316 2023-05-14 09:47:45.000000 pdf-annotations-diff-0.0.2/pdf_annotations_diff.egg-info/SOURCES.txt
+-rw-r--r--   0 sameer    (1000) sameer    (1000)        1 2023-05-14 09:47:45.000000 pdf-annotations-diff-0.0.2/pdf_annotations_diff.egg-info/dependency_links.txt
+-rw-r--r--   0 sameer    (1000) sameer    (1000)       67 2023-05-14 09:47:45.000000 pdf-annotations-diff-0.0.2/pdf_annotations_diff.egg-info/entry_points.txt
+-rw-r--r--   0 sameer    (1000) sameer    (1000)        8 2023-05-14 09:47:45.000000 pdf-annotations-diff-0.0.2/pdf_annotations_diff.egg-info/requires.txt
+-rw-r--r--   0 sameer    (1000) sameer    (1000)       21 2023-05-14 09:47:45.000000 pdf-annotations-diff-0.0.2/pdf_annotations_diff.egg-info/top_level.txt
+-rwxr-xr-x   0 sameer    (1000) sameer    (1000)     2909 2023-05-14 09:30:21.000000 pdf-annotations-diff-0.0.2/pdf_annotations_diff.py
+-rw-r--r--   0 sameer    (1000) sameer    (1000)       38 2023-05-14 09:47:45.256188 pdf-annotations-diff-0.0.2/setup.cfg
+-rw-r--r--   0 sameer    (1000) sameer    (1000)     1193 2023-05-14 09:45:43.000000 pdf-annotations-diff-0.0.2/setup.py
```

### Comparing `pdf-annotations-diff-0.0.1/LICENSE` & `pdf-annotations-diff-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdf-annotations-diff-0.0.1/pdf_annotations_diff.py` & `pdf-annotations-diff-0.0.2/pdf_annotations_diff.py`

 * *Files identical despite different names*

