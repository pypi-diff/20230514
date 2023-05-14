# Comparing `tmp/qunqunpdf-1.2.tar.gz` & `tmp/qunqunpdf-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qunqunpdf-1.2.tar", last modified: Sun May 14 02:31:11 2023, max compression
+gzip compressed data, was "qunqunpdf-1.3.tar", last modified: Sun May 14 02:40:36 2023, max compression
```

## Comparing `qunqunpdf-1.2.tar` & `qunqunpdf-1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 02:31:11.211026 qunqunpdf-1.2/
--rw-rw-rw-   0        0        0    35821 2023-05-14 02:11:33.000000 qunqunpdf-1.2/LICENSE
--rw-rw-rw-   0        0        0      118 2023-05-14 02:31:11.211026 qunqunpdf-1.2/PKG-INFO
--rw-rw-rw-   0        0        0       37 2023-05-14 02:11:05.000000 qunqunpdf-1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 02:31:11.201866 qunqunpdf-1.2/qunqunpdf/
--rw-rw-rw-   0        0        0        0 2023-05-14 02:07:19.000000 qunqunpdf-1.2/qunqunpdf/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-14 02:08:27.000000 qunqunpdf-1.2/qunqunpdf/pdf2image.py
--rw-rw-rw-   0        0        0       39 2023-05-14 02:07:57.000000 qunqunpdf-1.2/qunqunpdf/pdf2text.py
-drwxrwxrwx   0        0        0        0 2023-05-14 02:31:11.210023 qunqunpdf-1.2/qunqunpdf.egg-info/
--rw-rw-rw-   0        0        0      118 2023-05-14 02:31:11.000000 qunqunpdf-1.2/qunqunpdf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-05-14 02:31:11.000000 qunqunpdf-1.2/qunqunpdf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 02:31:11.000000 qunqunpdf-1.2/qunqunpdf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-14 02:31:11.000000 qunqunpdf-1.2/qunqunpdf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 02:31:11.211026 qunqunpdf-1.2/setup.cfg
--rw-rw-rw-   0        0        0      231 2023-05-14 02:30:50.000000 qunqunpdf-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 02:40:36.404562 qunqunpdf-1.3/
+-rw-rw-rw-   0        0        0    35821 2023-05-14 02:11:33.000000 qunqunpdf-1.3/LICENSE
+-rw-rw-rw-   0        0        0      118 2023-05-14 02:40:36.404562 qunqunpdf-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       37 2023-05-14 02:11:05.000000 qunqunpdf-1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 02:40:36.396459 qunqunpdf-1.3/qunqunpdf/
+-rw-rw-rw-   0        0        0        0 2023-05-14 02:07:19.000000 qunqunpdf-1.3/qunqunpdf/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-14 02:08:27.000000 qunqunpdf-1.3/qunqunpdf/pdf2image.py
+-rw-rw-rw-   0        0        0       39 2023-05-14 02:07:57.000000 qunqunpdf-1.3/qunqunpdf/pdf2text.py
+drwxrwxrwx   0        0        0        0 2023-05-14 02:40:36.404562 qunqunpdf-1.3/qunqunpdf.egg-info/
+-rw-rw-rw-   0        0        0      118 2023-05-14 02:40:36.000000 qunqunpdf-1.3/qunqunpdf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-05-14 02:40:36.000000 qunqunpdf-1.3/qunqunpdf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 02:40:36.000000 qunqunpdf-1.3/qunqunpdf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-14 02:40:36.000000 qunqunpdf-1.3/qunqunpdf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 02:40:36.405921 qunqunpdf-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      231 2023-05-14 02:39:34.000000 qunqunpdf-1.3/setup.py
```

### Comparing `qunqunpdf-1.2/LICENSE` & `qunqunpdf-1.3/LICENSE`

 * *Files identical despite different names*

