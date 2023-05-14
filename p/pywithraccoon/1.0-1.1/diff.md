# Comparing `tmp/pywithraccoon-1.0.tar.gz` & `tmp/pywithraccoon-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywithraccoon-1.0.tar", last modified: Sun May 14 07:55:15 2023, max compression
+gzip compressed data, was "pywithraccoon-1.1.tar", last modified: Sun May 14 08:06:23 2023, max compression
```

## Comparing `pywithraccoon-1.0.tar` & `pywithraccoon-1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 07:55:15.249301 pywithraccoon-1.0/
--rw-rw-rw-   0        0        0       98 2023-05-14 07:55:15.247309 pywithraccoon-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       36 2023-05-14 07:51:24.000000 pywithraccoon-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 07:55:15.185732 pywithraccoon-1.0/pywithraccoon/
--rw-rw-rw-   0        0        0        0 2023-05-14 07:47:56.000000 pywithraccoon-1.0/pywithraccoon/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-14 07:48:06.000000 pywithraccoon-1.0/pywithraccoon/pdf2image.py
--rw-rw-rw-   0        0        0        0 2023-05-14 07:48:17.000000 pywithraccoon-1.0/pywithraccoon/pdf2text.py
-drwxrwxrwx   0        0        0        0 2023-05-14 07:55:15.241179 pywithraccoon-1.0/pywithraccoon.egg-info/
--rw-rw-rw-   0        0        0       98 2023-05-14 07:55:14.000000 pywithraccoon-1.0/pywithraccoon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-05-14 07:55:14.000000 pywithraccoon-1.0/pywithraccoon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 07:55:14.000000 pywithraccoon-1.0/pywithraccoon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-14 07:55:14.000000 pywithraccoon-1.0/pywithraccoon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 07:55:15.250303 pywithraccoon-1.0/setup.cfg
--rw-rw-rw-   0        0        0      228 2023-05-14 07:54:46.000000 pywithraccoon-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 08:06:23.342439 pywithraccoon-1.1/
+-rw-rw-rw-   0        0        0    35829 2023-05-14 07:57:35.000000 pywithraccoon-1.1/LICENSE
+-rw-rw-rw-   0        0        0      121 2023-05-14 08:06:23.340435 pywithraccoon-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       36 2023-05-14 07:51:24.000000 pywithraccoon-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 08:06:23.288752 pywithraccoon-1.1/pywithraccoon/
+-rw-rw-rw-   0        0        0        0 2023-05-14 07:47:56.000000 pywithraccoon-1.1/pywithraccoon/__init__.py
+-rw-rw-rw-   0        0        0       36 2023-05-14 08:05:51.000000 pywithraccoon-1.1/pywithraccoon/pdf2image.py
+-rw-rw-rw-   0        0        0       35 2023-05-14 08:06:06.000000 pywithraccoon-1.1/pywithraccoon/pdf2text.py
+drwxrwxrwx   0        0        0        0 2023-05-14 08:06:23.335021 pywithraccoon-1.1/pywithraccoon.egg-info/
+-rw-rw-rw-   0        0        0      121 2023-05-14 08:06:22.000000 pywithraccoon-1.1/pywithraccoon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-05-14 08:06:23.000000 pywithraccoon-1.1/pywithraccoon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 08:06:22.000000 pywithraccoon-1.1/pywithraccoon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-14 08:06:22.000000 pywithraccoon-1.1/pywithraccoon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 08:06:23.342439 pywithraccoon-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      228 2023-05-14 08:05:15.000000 pywithraccoon-1.1/setup.py
```

