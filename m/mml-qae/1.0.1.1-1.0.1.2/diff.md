# Comparing `tmp/mml_qae-1.0.1.1.tar.gz` & `tmp/mml_qae-1.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mml_qae-1.0.1.1.tar", last modified: Sun May 14 05:34:13 2023, max compression
+gzip compressed data, was "dist\mml_qae-1.0.1.2.tar", last modified: Sun May 14 06:54:34 2023, max compression
```

## Comparing `mml_qae-1.0.1.1.tar` & `mml_qae-1.0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 05:34:13.000000 mml_qae-1.0.1.1/
--rw-rw-rw-   0        0        0     1445 2023-05-14 05:34:13.000000 mml_qae-1.0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-13 07:16:05.000000 mml_qae-1.0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 05:34:13.000000 mml_qae-1.0.1.1/mml_qae/
--rw-rw-rw-   0        0        0        0 2023-05-13 07:17:18.000000 mml_qae-1.0.1.1/mml_qae/__init__.py
--rw-rw-rw-   0        0        0     2808 2023-05-14 05:11:34.000000 mml_qae-1.0.1.1/mml_qae/lists_of_number.py
--rw-rw-rw-   0        0        0     1363 2023-05-13 08:27:02.000000 mml_qae-1.0.1.1/mml_qae/one_list_of_number.py
-drwxrwxrwx   0        0        0        0 2023-05-14 05:34:13.000000 mml_qae-1.0.1.1/mml_qae.egg-info/
--rw-rw-rw-   0        0        0     1445 2023-05-14 05:34:13.000000 mml_qae-1.0.1.1/mml_qae.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-05-14 05:34:13.000000 mml_qae-1.0.1.1/mml_qae.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 05:34:13.000000 mml_qae-1.0.1.1/mml_qae.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-14 05:34:13.000000 mml_qae-1.0.1.1/mml_qae.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 05:34:13.000000 mml_qae-1.0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1535 2023-05-14 05:34:01.000000 mml_qae-1.0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 06:54:34.000000 mml_qae-1.0.1.2/
+-rw-rw-rw-   0        0        0     3380 2023-05-14 06:54:34.000000 mml_qae-1.0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2638 2023-05-14 06:46:51.000000 mml_qae-1.0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 06:54:34.000000 mml_qae-1.0.1.2/mml_qae/
+-rw-rw-rw-   0        0        0        0 2023-05-13 07:17:18.000000 mml_qae-1.0.1.2/mml_qae/__init__.py
+-rw-rw-rw-   0        0        0     2808 2023-05-14 05:11:34.000000 mml_qae-1.0.1.2/mml_qae/lists_of_number.py
+-rw-rw-rw-   0        0        0     1363 2023-05-13 08:27:02.000000 mml_qae-1.0.1.2/mml_qae/one_list_of_number.py
+drwxrwxrwx   0        0        0        0 2023-05-14 06:54:34.000000 mml_qae-1.0.1.2/mml_qae.egg-info/
+-rw-rw-rw-   0        0        0     3380 2023-05-14 06:54:34.000000 mml_qae-1.0.1.2/mml_qae.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-05-14 06:54:34.000000 mml_qae-1.0.1.2/mml_qae.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 06:54:34.000000 mml_qae-1.0.1.2/mml_qae.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-14 06:54:34.000000 mml_qae-1.0.1.2/mml_qae.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 06:54:34.000000 mml_qae-1.0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      668 2023-05-14 06:54:30.000000 mml_qae-1.0.1.2/setup.py
```

### Comparing `mml_qae-1.0.1.1/mml_qae/lists_of_number.py` & `mml_qae-1.0.1.2/mml_qae/lists_of_number.py`

 * *Files identical despite different names*

### Comparing `mml_qae-1.0.1.1/mml_qae/one_list_of_number.py` & `mml_qae-1.0.1.2/mml_qae/one_list_of_number.py`

 * *Files identical despite different names*

