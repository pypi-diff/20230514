# Comparing `tmp/qunqunpdf-1.1.tar.gz` & `tmp/qunqunpdf-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qunqunpdf-1.1.tar", last modified: Sun May 14 02:19:25 2023, max compression
+gzip compressed data, was "qunqunpdf-1.2.tar", last modified: Sun May 14 02:31:11 2023, max compression
```

## Comparing `qunqunpdf-1.1.tar` & `qunqunpdf-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 02:19:25.974367 qunqunpdf-1.1/
--rw-rw-rw-   0        0        0    35821 2023-05-14 02:11:33.000000 qunqunpdf-1.1/LICENSE
--rw-rw-rw-   0        0        0      118 2023-05-14 02:19:25.972920 qunqunpdf-1.1/PKG-INFO
--rw-rw-rw-   0        0        0       37 2023-05-14 02:11:05.000000 qunqunpdf-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 02:19:25.966564 qunqunpdf-1.1/qunqunpdf/
--rw-rw-rw-   0        0        0        0 2023-05-14 02:07:19.000000 qunqunpdf-1.1/qunqunpdf/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-14 02:08:27.000000 qunqunpdf-1.1/qunqunpdf/pdf2image.py
--rw-rw-rw-   0        0        0       39 2023-05-14 02:07:57.000000 qunqunpdf-1.1/qunqunpdf/pdf2text.py
-drwxrwxrwx   0        0        0        0 2023-05-14 02:19:25.971920 qunqunpdf-1.1/qunqunpdf.egg-info/
--rw-rw-rw-   0        0        0      118 2023-05-14 02:19:25.000000 qunqunpdf-1.1/qunqunpdf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-05-14 02:19:25.000000 qunqunpdf-1.1/qunqunpdf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 02:19:25.000000 qunqunpdf-1.1/qunqunpdf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-14 02:19:25.000000 qunqunpdf-1.1/qunqunpdf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 02:19:25.974367 qunqunpdf-1.1/setup.cfg
--rw-rw-rw-   0        0        0      231 2023-05-14 02:18:54.000000 qunqunpdf-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 02:31:11.211026 qunqunpdf-1.2/
+-rw-rw-rw-   0        0        0    35821 2023-05-14 02:11:33.000000 qunqunpdf-1.2/LICENSE
+-rw-rw-rw-   0        0        0      118 2023-05-14 02:31:11.211026 qunqunpdf-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       37 2023-05-14 02:11:05.000000 qunqunpdf-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 02:31:11.201866 qunqunpdf-1.2/qunqunpdf/
+-rw-rw-rw-   0        0        0        0 2023-05-14 02:07:19.000000 qunqunpdf-1.2/qunqunpdf/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-14 02:08:27.000000 qunqunpdf-1.2/qunqunpdf/pdf2image.py
+-rw-rw-rw-   0        0        0       39 2023-05-14 02:07:57.000000 qunqunpdf-1.2/qunqunpdf/pdf2text.py
+drwxrwxrwx   0        0        0        0 2023-05-14 02:31:11.210023 qunqunpdf-1.2/qunqunpdf.egg-info/
+-rw-rw-rw-   0        0        0      118 2023-05-14 02:31:11.000000 qunqunpdf-1.2/qunqunpdf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-05-14 02:31:11.000000 qunqunpdf-1.2/qunqunpdf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 02:31:11.000000 qunqunpdf-1.2/qunqunpdf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-14 02:31:11.000000 qunqunpdf-1.2/qunqunpdf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 02:31:11.211026 qunqunpdf-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      231 2023-05-14 02:30:50.000000 qunqunpdf-1.2/setup.py
```

### Comparing `qunqunpdf-1.1/LICENSE` & `qunqunpdf-1.2/LICENSE`

 * *Files identical despite different names*

