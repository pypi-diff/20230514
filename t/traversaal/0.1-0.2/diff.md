# Comparing `tmp/traversaal-0.1.tar.gz` & `tmp/traversaal-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traversaal-0.1.tar", last modified: Sun May 14 06:21:01 2023, max compression
+gzip compressed data, was "traversaal-0.2.tar", last modified: Sun May 14 06:30:27 2023, max compression
```

## Comparing `traversaal-0.1.tar` & `traversaal-0.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxr-xr-x   0 aimzlicious   (501) staff       (20)        0 2023-05-14 06:21:01.091887 traversaal-0.1/
--rw-r--r--   0 aimzlicious   (501) staff       (20)      197 2023-05-14 06:21:01.091746 traversaal-0.1/PKG-INFO
--rw-r--r--   0 aimzlicious   (501) staff       (20)       38 2023-05-14 06:21:01.091926 traversaal-0.1/setup.cfg
--rw-r--r--   0 aimzlicious   (501) staff       (20)      381 2023-05-14 06:17:47.000000 traversaal-0.1/setup.py
-drwxr-xr-x   0 aimzlicious   (501) staff       (20)        0 2023-05-14 06:21:01.091581 traversaal-0.1/traversaal.egg-info/
--rw-r--r--   0 aimzlicious   (501) staff       (20)      197 2023-05-14 06:21:01.000000 traversaal-0.1/traversaal.egg-info/PKG-INFO
--rw-r--r--   0 aimzlicious   (501) staff       (20)      177 2023-05-14 06:21:01.000000 traversaal-0.1/traversaal.egg-info/SOURCES.txt
--rw-r--r--   0 aimzlicious   (501) staff       (20)        1 2023-05-14 06:21:01.000000 traversaal-0.1/traversaal.egg-info/dependency_links.txt
--rw-r--r--   0 aimzlicious   (501) staff       (20)       25 2023-05-14 06:21:01.000000 traversaal-0.1/traversaal.egg-info/requires.txt
--rw-r--r--   0 aimzlicious   (501) staff       (20)        1 2023-05-14 06:21:01.000000 traversaal-0.1/traversaal.egg-info/top_level.txt
+drwxr-xr-x   0 aimzlicious   (501) staff       (20)        0 2023-05-14 06:30:27.261619 traversaal-0.2/
+-rw-r--r--   0 aimzlicious   (501) staff       (20)      197 2023-05-14 06:30:27.261477 traversaal-0.2/PKG-INFO
+-rw-r--r--   0 aimzlicious   (501) staff       (20)     1521 2023-05-14 06:27:33.000000 traversaal-0.2/README.md
+-rw-r--r--   0 aimzlicious   (501) staff       (20)       38 2023-05-14 06:30:27.261657 traversaal-0.2/setup.cfg
+-rw-r--r--   0 aimzlicious   (501) staff       (20)      381 2023-05-14 06:30:22.000000 traversaal-0.2/setup.py
+drwxr-xr-x   0 aimzlicious   (501) staff       (20)        0 2023-05-14 06:30:27.261314 traversaal-0.2/traversaal.egg-info/
+-rw-r--r--   0 aimzlicious   (501) staff       (20)      197 2023-05-14 06:30:27.000000 traversaal-0.2/traversaal.egg-info/PKG-INFO
+-rw-r--r--   0 aimzlicious   (501) staff       (20)      187 2023-05-14 06:30:27.000000 traversaal-0.2/traversaal.egg-info/SOURCES.txt
+-rw-r--r--   0 aimzlicious   (501) staff       (20)        1 2023-05-14 06:30:27.000000 traversaal-0.2/traversaal.egg-info/dependency_links.txt
+-rw-r--r--   0 aimzlicious   (501) staff       (20)       25 2023-05-14 06:30:27.000000 traversaal-0.2/traversaal.egg-info/requires.txt
+-rw-r--r--   0 aimzlicious   (501) staff       (20)        1 2023-05-14 06:30:27.000000 traversaal-0.2/traversaal.egg-info/top_level.txt
```

