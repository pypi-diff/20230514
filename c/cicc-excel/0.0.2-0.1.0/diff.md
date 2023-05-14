# Comparing `tmp/cicc_excel-0.0.2.tar.gz` & `tmp/cicc_excel-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cicc_excel-0.0.2.tar", last modified: Fri May  5 13:14:24 2023, max compression
+gzip compressed data, was "cicc_excel-0.1.0.tar", last modified: Sun May 14 13:49:19 2023, max compression
```

## Comparing `cicc_excel-0.0.2.tar` & `cicc_excel-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 js         (501) staff       (20)        0 2023-05-05 13:14:24.000000 cicc_excel-0.0.2/
--rw-r--r--   0 js         (501) staff       (20)     1651 2023-05-05 13:14:24.000000 cicc_excel-0.0.2/PKG-INFO
--rwxr-xr-x   0 js         (501) staff       (20)      783 2023-05-05 13:09:46.000000 cicc_excel-0.0.2/README.md
-drwxr-xr-x   0 js         (501) staff       (20)        0 2023-05-05 13:14:24.000000 cicc_excel-0.0.2/cicc_excel/
--rwxr-xr-x   0 js         (501) staff       (20)        0 2020-07-20 03:22:51.000000 cicc_excel-0.0.2/cicc_excel/__init__.py
--rwxr-xr-x   0 js         (501) staff       (20)    12078 2023-05-05 12:54:10.000000 cicc_excel-0.0.2/cicc_excel/excelwriter.py
-drwxr-xr-x   0 js         (501) staff       (20)        0 2023-05-05 13:14:24.000000 cicc_excel-0.0.2/cicc_excel.egg-info/
--rwxr-xr-x   0 js         (501) staff       (20)     1651 2023-05-05 13:14:24.000000 cicc_excel-0.0.2/cicc_excel.egg-info/PKG-INFO
--rwxr-xr-x   0 js         (501) staff       (20)      203 2023-05-05 13:14:24.000000 cicc_excel-0.0.2/cicc_excel.egg-info/SOURCES.txt
--rwxr-xr-x   0 js         (501) staff       (20)        1 2023-05-05 13:14:24.000000 cicc_excel-0.0.2/cicc_excel.egg-info/dependency_links.txt
--rwxr-xr-x   0 js         (501) staff       (20)       11 2023-05-05 13:14:24.000000 cicc_excel-0.0.2/cicc_excel.egg-info/top_level.txt
--rw-r--r--   0 js         (501) staff       (20)       38 2023-05-05 13:14:24.000000 cicc_excel-0.0.2/setup.cfg
--rwxr-xr-x   0 js         (501) staff       (20)      771 2023-05-05 13:01:10.000000 cicc_excel-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 13:49:18.970000 cicc_excel-0.1.0/
+-rw-rw-rw-   0        0        0     1093 2023-05-14 05:35:00.000000 cicc_excel-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1705 2023-05-14 13:49:20.000000 cicc_excel-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1142 2023-05-14 13:39:04.000000 cicc_excel-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 13:49:19.000000 cicc_excel-0.1.0/cicc_excel/
+-rw-rw-rw-   0        0        0        0 2023-05-14 05:35:00.000000 cicc_excel-0.1.0/cicc_excel/__init__.py
+-rw-rw-rw-   0        0        0    13055 2023-05-14 13:44:14.000000 cicc_excel-0.1.0/cicc_excel/excelwriter.py
+drwxrwxrwx   0        0        0        0 2023-05-14 13:49:19.030000 cicc_excel-0.1.0/cicc_excel.egg-info/
+-rw-rw-rw-   0        0        0     1705 2023-05-14 13:49:20.000000 cicc_excel-0.1.0/cicc_excel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-05-14 13:49:20.000000 cicc_excel-0.1.0/cicc_excel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 13:49:20.000000 cicc_excel-0.1.0/cicc_excel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-14 13:49:20.000000 cicc_excel-0.1.0/cicc_excel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-14 13:49:20.000000 cicc_excel-0.1.0/cicc_excel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 13:49:20.000000 cicc_excel-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      867 2023-05-14 13:43:54.000000 cicc_excel-0.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

