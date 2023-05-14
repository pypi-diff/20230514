# Comparing `tmp/FuncsForSPO-4.41.6.tar.gz` & `tmp/FuncsForSPO-4.42.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuncsForSPO-4.41.6.tar", last modified: Thu May 11 16:24:17 2023, max compression
+gzip compressed data, was "FuncsForSPO-4.42.0.tar", last modified: Sun May 14 20:23:27 2023, max compression
```

## Comparing `FuncsForSPO-4.41.6.tar` & `FuncsForSPO-4.42.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.835623 FuncsForSPO-4.41.6/
-drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.433119 FuncsForSPO-4.41.6/FuncsForSPO/
-drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.492286 FuncsForSPO-4.41.6/FuncsForSPO/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-4.41.6/FuncsForSPO/femails/__init__.py
--rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-4.41.6/FuncsForSPO/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.502469 FuncsForSPO-4.41.6/FuncsForSPO/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.6/FuncsForSPO/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-4.41.6/FuncsForSPO/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.514999 FuncsForSPO-4.41.6/FuncsForSPO/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.6/FuncsForSPO/fftp/__init__.py
--rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-4.41.6/FuncsForSPO/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.526733 FuncsForSPO-4.41.6/FuncsForSPO/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.6/FuncsForSPO/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-4.41.6/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.426682 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/
-drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.598677 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fcompress/
--rw-rw-rw-   0        0        0     9269 2023-02-23 17:57:32.000000 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1599 2022-11-17 11:12:03.000000 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.619199 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.627403 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.648415 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     9692 2023-02-23 17:58:42.000000 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     5017 2023-05-08 20:46:58.000000 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.661082 FuncsForSPO-4.41.6/FuncsForSPO/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.6/FuncsForSPO/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-4.41.6/FuncsForSPO/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.674362 FuncsForSPO-4.41.6/FuncsForSPO/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.6/FuncsForSPO/fpython/__init__.py
--rw-rw-rw-   0        0        0    69543 2023-05-10 14:22:37.000000 FuncsForSPO-4.41.6/FuncsForSPO/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.683934 FuncsForSPO-4.41.6/FuncsForSPO/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.6/FuncsForSPO/fregex/__init__.py
--rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-4.41.6/FuncsForSPO/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.695520 FuncsForSPO-4.41.6/FuncsForSPO/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.6/FuncsForSPO/fselenium/__init__.py
--rw-rw-rw-   0        0        0    39076 2023-05-11 16:23:08.000000 FuncsForSPO-4.41.6/FuncsForSPO/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.708750 FuncsForSPO-4.41.6/FuncsForSPO/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.6/FuncsForSPO/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-4.41.6/FuncsForSPO/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.716673 FuncsForSPO-4.41.6/FuncsForSPO/fwinotify/
--rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-4.41.6/FuncsForSPO/fwinotify/__init__.py
--rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-4.41.6/FuncsForSPO/fwinotify/fwinotify.py
-drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.724924 FuncsForSPO-4.41.6/FuncsForSPO/utils/
--rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-4.41.6/FuncsForSPO/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.478895 FuncsForSPO-4.41.6/FuncsForSPO.egg-info/
--rw-rw-rw-   0        0        0     8027 2023-05-11 16:24:17.000000 FuncsForSPO-4.41.6/FuncsForSPO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1331 2023-05-11 16:24:17.000000 FuncsForSPO-4.41.6/FuncsForSPO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 16:24:17.000000 FuncsForSPO-4.41.6/FuncsForSPO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      176 2023-05-11 16:24:17.000000 FuncsForSPO-4.41.6/FuncsForSPO.egg-info/requires.txt
--rw-rw-rw-   0        0        0      350 2023-05-11 16:24:17.000000 FuncsForSPO-4.41.6/FuncsForSPO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-4.41.6/LICENSE
--rw-rw-rw-   0        0        0     8027 2023-05-11 16:24:17.833547 FuncsForSPO-4.41.6/PKG-INFO
--rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-4.41.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-11 16:24:17.837186 FuncsForSPO-4.41.6/setup.cfg
--rw-rw-rw-   0        0        0     2150 2023-05-11 16:24:12.000000 FuncsForSPO-4.41.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 20:23:27.789729 FuncsForSPO-4.42.0/
+drwxrwxrwx   0        0        0        0 2023-05-14 20:23:27.464933 FuncsForSPO-4.42.0/FuncsForSPO/
+drwxrwxrwx   0        0        0        0 2023-05-14 20:23:27.525535 FuncsForSPO-4.42.0/FuncsForSPO/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-4.42.0/FuncsForSPO/femails/__init__.py
+-rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-4.42.0/FuncsForSPO/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-05-14 20:23:27.535487 FuncsForSPO-4.42.0/FuncsForSPO/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-4.42.0/FuncsForSPO/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-4.42.0/FuncsForSPO/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-14 20:23:27.544791 FuncsForSPO-4.42.0/FuncsForSPO/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.42.0/FuncsForSPO/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-4.42.0/FuncsForSPO/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-05-14 20:23:27.555985 FuncsForSPO-4.42.0/FuncsForSPO/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.42.0/FuncsForSPO/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-4.42.0/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-05-14 20:23:27.457679 FuncsForSPO-4.42.0/FuncsForSPO/fpdf/
+drwxrwxrwx   0        0        0        0 2023-05-14 20:23:27.573159 FuncsForSPO-4.42.0/FuncsForSPO/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     9269 2023-02-23 17:57:32.000000 FuncsForSPO-4.42.0/FuncsForSPO/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.42.0/FuncsForSPO/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1599 2022-11-17 11:12:03.000000 FuncsForSPO-4.42.0/FuncsForSPO/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-05-14 20:23:27.590042 FuncsForSPO-4.42.0/FuncsForSPO/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-4.42.0/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.42.0/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-4.42.0/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-05-14 20:23:27.595463 FuncsForSPO-4.42.0/FuncsForSPO/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-4.42.0/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-05-14 20:23:27.611872 FuncsForSPO-4.42.0/FuncsForSPO/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-4.42.0/FuncsForSPO/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     9692 2023-02-23 17:58:42.000000 FuncsForSPO-4.42.0/FuncsForSPO/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     5017 2023-05-08 20:46:58.000000 FuncsForSPO-4.42.0/FuncsForSPO/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-05-14 20:23:27.622954 FuncsForSPO-4.42.0/FuncsForSPO/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.42.0/FuncsForSPO/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-4.42.0/FuncsForSPO/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-05-14 20:23:27.632063 FuncsForSPO-4.42.0/FuncsForSPO/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.42.0/FuncsForSPO/fpython/__init__.py
+-rw-rw-rw-   0        0        0    68146 2023-05-14 20:21:36.000000 FuncsForSPO-4.42.0/FuncsForSPO/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-05-14 20:23:27.644900 FuncsForSPO-4.42.0/FuncsForSPO/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-4.42.0/FuncsForSPO/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-4.42.0/FuncsForSPO/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-05-14 20:23:27.657014 FuncsForSPO-4.42.0/FuncsForSPO/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-4.42.0/FuncsForSPO/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    39076 2023-05-11 16:23:08.000000 FuncsForSPO-4.42.0/FuncsForSPO/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-05-14 20:23:27.670137 FuncsForSPO-4.42.0/FuncsForSPO/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.42.0/FuncsForSPO/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-4.42.0/FuncsForSPO/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-05-14 20:23:27.679640 FuncsForSPO-4.42.0/FuncsForSPO/fwinotify/
+-rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-4.42.0/FuncsForSPO/fwinotify/__init__.py
+-rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-4.42.0/FuncsForSPO/fwinotify/fwinotify.py
+drwxrwxrwx   0        0        0        0 2023-05-14 20:23:27.686488 FuncsForSPO-4.42.0/FuncsForSPO/utils/
+-rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-4.42.0/FuncsForSPO/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-14 20:23:27.514465 FuncsForSPO-4.42.0/FuncsForSPO.egg-info/
+-rw-rw-rw-   0        0        0     8027 2023-05-14 20:23:27.000000 FuncsForSPO-4.42.0/FuncsForSPO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1331 2023-05-14 20:23:27.000000 FuncsForSPO-4.42.0/FuncsForSPO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 20:23:27.000000 FuncsForSPO-4.42.0/FuncsForSPO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      187 2023-05-14 20:23:27.000000 FuncsForSPO-4.42.0/FuncsForSPO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      350 2023-05-14 20:23:27.000000 FuncsForSPO-4.42.0/FuncsForSPO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-4.42.0/LICENSE
+-rw-rw-rw-   0        0        0     8027 2023-05-14 20:23:27.786733 FuncsForSPO-4.42.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-4.42.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-14 20:23:27.790733 FuncsForSPO-4.42.0/setup.cfg
+-rw-rw-rw-   0        0        0     2177 2023-05-14 20:22:57.000000 FuncsForSPO-4.42.0/setup.py
```

### Comparing `FuncsForSPO-4.41.6/FuncsForSPO/femails/femails.py` & `FuncsForSPO-4.42.0/FuncsForSPO/femails/femails.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.6/FuncsForSPO/fexceptions/exceptions.py` & `FuncsForSPO-4.42.0/FuncsForSPO/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.6/FuncsForSPO/fftp/fftp.py` & `FuncsForSPO-4.42.0/FuncsForSPO/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.6/FuncsForSPO/fopenpyxl/openpyxl_funcs.py` & `FuncsForSPO-4.42.0/FuncsForSPO/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fcompress/__compress_online.py` & `FuncsForSPO-4.42.0/FuncsForSPO/fpdf/fcompress/__compress_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fcompress/compress.py` & `FuncsForSPO-4.42.0/FuncsForSPO/fpdf/fcompress/compress.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `FuncsForSPO-4.42.0/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py` & `FuncsForSPO-4.42.0/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py` & `FuncsForSPO-4.42.0/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.6/FuncsForSPO/fpdf/focr/__ocr_online.py` & `FuncsForSPO-4.42.0/FuncsForSPO/fpdf/focr/__ocr_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.6/FuncsForSPO/fpdf/focr/orc.py` & `FuncsForSPO-4.42.0/FuncsForSPO/fpdf/focr/orc.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.6/FuncsForSPO/fpysimplegui/functions_for_sg.py` & `FuncsForSPO-4.42.0/FuncsForSPO/fpysimplegui/functions_for_sg.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.6/FuncsForSPO/fpython/functions_for_py.py` & `FuncsForSPO-4.42.0/FuncsForSPO/fpython/functions_for_py.py`

 * *Files 6% similar despite different names*

```diff
@@ -1477,97 +1477,75 @@
         self.DRIVER.maximize_window()
         return self.DRIVER
 """)
     
     # CRIA ARQUIVO PYTHON EM database
     with open(DATABASE_PATH, 'w', encoding='utf-8') as f:
         f.write("""from FuncsForSPO.fpython.functions_for_py import *
-from FuncsForSPO.fselenium.functions_selenium import *
-from FuncsForSPO.fsqlite.sqlite_functions import *
-from FuncsForSPO.fpysimplegui.functions_for_sg import *
-import pandas as pd
-
-# GLOBAL
-DATABASE_PATH = arquivo_com_caminho_absoluto('bin', 'database.db')
-RESULTADO = cria_dir_no_dir_de_trabalho_atual('Resultados')
-# GLOBAL
-
-# BACKUP
-def faz_backup_do_banco_de_dados():
-    json_config = read_json(arquivo_com_caminho_absoluto('bin', 'config.json'))
-
-    # cria os dirs
-    cria_dir_no_dir_de_trabalho_atual(arquivo_com_caminho_absoluto('bin', 'backup'))
-    
-    path_database_copy = arquivo_com_caminho_absoluto(['bin', 'backup'], f'database_{datetime.now().strftime("%d-%m-%Y_%H-%M-%S")}.db')
-    shutil.copy2(DATABASE_PATH, path_database_copy)
-    return path_database_copy
-# BACKUP
-
-
-# EXPORT
-def exportar_database():
-    cur, con =  connect_db(DATABASE_PATH)
-    arquivos = pd.read_sql('SELECT * FROM arquivos', con)
-    arquivos_com_ocr = pd.read_sql('SELECT * FROM arquivos_com_ocr', con)
-    # TRATAMENTOS
-    arquivos_com_ocr['data_adicao'] = arquivos_com_ocr['data_adicao'].apply(lambda x: datetime.strptime(x, '%Y-%m-%d %H:%M:%S.%f'))
-    
-    arquivos_com_ocr.rename(columns={'caminho_arquivo': 'Caminho do Arquivo'}, inplace=True)
-    arquivos_com_ocr.rename(columns={'nome_do_arquivo': 'Nome do Arquivo'}, inplace=True)
-    arquivos_com_ocr.rename(columns={'ocr': 'OCR do Arquivo'}, inplace=True)
-    arquivos_com_ocr.rename(columns={'data_adicao': 'Data de Envio no Database'}, inplace=True)
-
-
-    arquivos.rename(columns={'caminho_arquivo': 'Caminho do Arquivo'}, inplace=True)
-    arquivos.rename(columns={'nome_do_arquivo': 'Nome do Arquivo'}, inplace=True)
-    # TRATAMENTOS
-    
-    try:
-        with pd.ExcelWriter(os.path.join(RESULTADO, 'DATABASE.xlsx')) as writer:
-            arquivos_com_ocr.to_excel(writer, sheet_name="Arquivos Com OCR", index=False)
-            arquivos.to_excel(writer, sheet_name="PDFs Recuperados da Máquina", index=False)
-    except PermissionError:
-        sleep(10)
-        try:
-            with pd.ExcelWriter(os.path.join(RESULTADO, 'DATABASE.xlsx')) as writer:
-                arquivos_com_ocr.to_excel(writer, sheet_name="Arquivos Com OCR", index=False)
-                arquivos.to_excel(writer, sheet_name="PDFs Recuperados da Máquina", index=False)
-        except PermissionError:
-            faz_log('O Arquivo está aberto, não foi possível exportar...')
-    except OSError:
-        popup_erro('Sem espaço em disco para fazer o arquivo...', 'Sem espaço...')
-        pass
-# EXPORT
-
-# DELETE
-def delete(table):
-    # Apaga todos os dados da tabela enviada
-    cur, con =  connect_db(DATABASE_PATH)
-    query = f'DELETE FROM {table};'
-    cur.execute(query)
-    con.commit()
-# DELETE
-
-# SELECT
-def select(table:str, col: str='*', data_from_line: bool=False):
-    cur, con =  connect_db(DATABASE_PATH)
-    cur.execute(f'SELECT {col} FROM {table}')
-    faz_log(f'SELECT {col} FROM {table}', 'i*')
-    data = []
-    if data_from_line:
-        for line in cur.fetchall():
-            for i in line:
-                data.append(i)
-        return tuple(data)
-    else:
-        for line in cur.fetchall():
-            data.append(line)
-        return tuple(data)
-# SELECT
+from sqlalchemy import create_engine
+from sqlalchemy.orm import sessionmaker
+from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy import Column, String, Integer
+
+engine = create_engine('sqlite:///database.db', pool_size=15, max_overflow=20)
+Base = declarative_base()
+Session = sessionmaker(bind=engine)
+
+
+class TABLE(Base):
+    __tablename__ = 'table'
+
+    id = Column(Integer, primary_key=True, autoincrement=True)
+    status = Column(String)
+    nome = Column(String)
+    
+Base.metadata.create_all(engine)  # cria a tabela no banco de dados
+
+    
+class DBManager:
+    def __init__(self):
+        # Inicializa uma nova sessão com o banco de dados.
+        
+        self.session = Session()
+
+    def create_item(self, status, name):
+        # Cria um novo registro na tabela.
+
+        new_item = TABLE(status=status, name=name)
+        self.session.add(new_item)
+        self.session.commit()
+
+    def get_item(self, id):
+        # Retorna o registro com o ID fornecido
+        return self.session.query(TABLE).filter_by(id=id).first()
+    
+
+    def delete_item(self, id):
+        # Exclui o registro com o ID fornecido da tabela
+
+        delete_item_from_db = self.get_item(id)
+        self.session.delete(delete_item_from_db)
+        self.session.commit()
+        
+    def delete_all(self):
+        # Exclui todos os registros da tabela.
+
+        self.session.query(TABLE).delete()
+        self.session.commit()
+
+    def get_item(self, id):
+        # Retorna o registro com o ID fornecido da tabela. Se nenhum registro for encontrado, retorna None.
+        return self.session.query(TABLE).filter_by(id=id).first()
+    
+
+    def get_column_status(self):
+        # Retorna o registro de status com o ID fornecido da tabela. Se nenhum registro for encontrado, retorna None.
+        return self.session.query(TABLE.status).all()
+    
+    
 
 """)
     
     # CRIA ARQUIVO PYTHON EM exceptions
     with open(EXCEPTIONS_PATH, 'w', encoding='utf-8') as f:
         f.write("""from FuncsForSPO.fexceptions.exceptions import *
 """)
```

### Comparing `FuncsForSPO-4.41.6/FuncsForSPO/fregex/functions_re.py` & `FuncsForSPO-4.42.0/FuncsForSPO/fregex/functions_re.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.6/FuncsForSPO/fselenium/functions_selenium.py` & `FuncsForSPO-4.42.0/FuncsForSPO/fselenium/functions_selenium.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.6/FuncsForSPO/fsqlite/sqlite_functions.py` & `FuncsForSPO-4.42.0/FuncsForSPO/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.6/FuncsForSPO/fwinotify/fwinotify.py` & `FuncsForSPO-4.42.0/FuncsForSPO/fwinotify/fwinotify.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.6/FuncsForSPO/utils/utils.py` & `FuncsForSPO-4.42.0/FuncsForSPO/utils/utils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.6/FuncsForSPO.egg-info/PKG-INFO` & `FuncsForSPO-4.42.0/FuncsForSPO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 4.41.6
+Version: 4.42.0
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-4.41.6/FuncsForSPO.egg-info/SOURCES.txt` & `FuncsForSPO-4.42.0/FuncsForSPO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.6/LICENSE` & `FuncsForSPO-4.42.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.6/PKG-INFO` & `FuncsForSPO-4.42.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 4.41.6
+Version: 4.42.0
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-4.41.6/README.md` & `FuncsForSPO-4.42.0/README.md`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.6/setup.py` & `FuncsForSPO-4.42.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '4.41.6'
+version = '4.42.0'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='FuncsForSPO',
         version=version,
         url='https://github.com/githubpaycon/FuncsForSPO',
@@ -49,11 +49,12 @@
             'packaging',
             'PySimpleGUI',
             'macholib',
             'wget',
             'winotify',
             'pypdf',
             'pywin32',
+            'sqlalchemy',
             'rich==12.6.0',
             'pyinstaller==5.6.2',
         ],
         )
```

