# Comparing `tmp/gkjzjh146-1.2.tar.gz` & `tmp/gkjzjh146-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gkjzjh146-1.2.tar", last modified: Sun May 14 04:41:35 2023, max compression
+gzip compressed data, was "dist\gkjzjh146-1.3.tar", last modified: Sun May 14 04:45:55 2023, max compression
```

## Comparing `gkjzjh146-1.2.tar` & `gkjzjh146-1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 04:41:35.000000 gkjzjh146-1.2/
--rw-rw-rw-   0        0        0      149 2023-05-14 04:41:35.000000 gkjzjh146-1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-14 04:41:35.000000 gkjzjh146-1.2/gkjzjh146/
--rw-rw-rw-   0        0        0      196 2023-05-14 03:09:06.000000 gkjzjh146-1.2/gkjzjh146/gkj2jh146.py
-drwxrwxrwx   0        0        0        0 2023-05-14 04:41:35.000000 gkjzjh146-1.2/gkjzjh146.egg-info/
--rw-rw-rw-   0        0        0      149 2023-05-14 04:41:35.000000 gkjzjh146-1.2/gkjzjh146.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-05-14 04:41:35.000000 gkjzjh146-1.2/gkjzjh146.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 04:41:35.000000 gkjzjh146-1.2/gkjzjh146.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-14 04:41:35.000000 gkjzjh146-1.2/gkjzjh146.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-14 04:41:35.000000 gkjzjh146-1.2/gkjzjh146.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 04:41:35.000000 gkjzjh146-1.2/setup.cfg
--rw-rw-rw-   0        0        0      944 2023-05-14 04:40:49.000000 gkjzjh146-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 04:45:55.000000 gkjzjh146-1.3/
+-rw-rw-rw-   0        0        0      159 2023-05-14 04:45:55.000000 gkjzjh146-1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-14 04:45:55.000000 gkjzjh146-1.3/gkjzjh146/
+-rw-rw-rw-   0        0        0      196 2023-05-14 03:09:06.000000 gkjzjh146-1.3/gkjzjh146/gkj2jh146.py
+drwxrwxrwx   0        0        0        0 2023-05-14 04:45:55.000000 gkjzjh146-1.3/gkjzjh146.egg-info/
+-rw-rw-rw-   0        0        0      159 2023-05-14 04:45:55.000000 gkjzjh146-1.3/gkjzjh146.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2023-05-14 04:45:55.000000 gkjzjh146-1.3/gkjzjh146.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 04:45:55.000000 gkjzjh146-1.3/gkjzjh146.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-14 04:45:55.000000 gkjzjh146-1.3/gkjzjh146.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-14 04:45:55.000000 gkjzjh146-1.3/gkjzjh146.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 04:45:55.000000 gkjzjh146-1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1160 2023-05-14 04:45:51.000000 gkjzjh146-1.3/setup.py
```

