# Comparing `tmp/quorum-0.8.0.tar.gz` & `tmp/quorum-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/quorum-0.8.0.tar", last modified: Fri Jan  6 12:28:53 2023, max compression
+gzip compressed data, was "dist/quorum-0.8.1.tar", last modified: Sun May 14 06:22:53 2023, max compression
```

## Comparing `quorum-0.8.0.tar` & `quorum-0.8.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 12:28:53.000000 quorum-0.8.0/
--rw-r--r--   0 root         (0) root         (0)     1495 2023-01-06 12:28:32.000000 quorum-0.8.0/README.md
--rw-r--r--   0 root         (0) root         (0)       67 2023-01-06 12:28:53.000000 quorum-0.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2947 2023-01-06 12:28:53.000000 quorum-0.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2998 2023-01-06 12:28:32.000000 quorum-0.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 12:28:53.000000 quorum-0.8.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 12:28:53.000000 quorum-0.8.0/src/quorum.egg-info/
--rw-r--r--   0 root         (0) root         (0)        6 2023-01-06 12:28:52.000000 quorum-0.8.0/src/quorum.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-06 12:28:52.000000 quorum-0.8.0/src/quorum.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     2947 2023-01-06 12:28:52.000000 quorum-0.8.0/src/quorum.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        7 2023-01-06 12:28:52.000000 quorum-0.8.0/src/quorum.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-06 12:28:38.000000 quorum-0.8.0/src/quorum.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)     1533 2023-01-06 12:28:52.000000 quorum-0.8.0/src/quorum.egg-info/SOURCES.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 12:28:53.000000 quorum-0.8.0/src/quorum/
--rw-r--r--   0 root         (0) root         (0)    13063 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/legacy.py
--rw-r--r--   0 root         (0) root         (0)     2934 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/amqp.py
--rw-r--r--   0 root         (0) root         (0)    12158 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/export.py
--rw-r--r--   0 root         (0) root         (0)     7167 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1515 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/request.py
--rw-r--r--   0 root         (0) root         (0)     3125 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/amazon.py
--rw-r--r--   0 root         (0) root         (0)     1446 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/common.py
--rw-r--r--   0 root         (0) root         (0)     1822 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/unit_test.py
--rw-r--r--   0 root         (0) root         (0)    29352 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/httpc.py
--rw-r--r--   0 root         (0) root         (0)    14572 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/data.py
--rw-r--r--   0 root         (0) root         (0)    10207 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/defines.py
--rw-r--r--   0 root         (0) root         (0)    11475 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/mail.py
--rw-r--r--   0 root         (0) root         (0)    14534 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/execution.py
--rw-r--r--   0 root         (0) root         (0)     8233 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/route.py
--rw-r--r--   0 root         (0) root         (0)     2567 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/errors.py
--rw-r--r--   0 root         (0) root         (0)     5918 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/crypt.py
--rw-r--r--   0 root         (0) root         (0)     8284 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 12:28:53.000000 quorum-0.8.0/src/quorum/test/
--rw-r--r--   0 root         (0) root         (0)     3637 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/test/export.py
--rw-r--r--   0 root         (0) root         (0)     1193 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2434 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/test/amazon.py
--rw-r--r--   0 root         (0) root         (0)     8415 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/test/httpc.py
--rw-r--r--   0 root         (0) root         (0)     1556 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/test/data.py
--rw-r--r--   0 root         (0) root         (0)     2196 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/test/mail.py
--rw-r--r--   0 root         (0) root         (0)     6706 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/test/execution.py
--rw-r--r--   0 root         (0) root         (0)     2681 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/test/crypt.py
--rw-r--r--   0 root         (0) root         (0)     8314 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/test/typesf.py
--rw-r--r--   0 root         (0) root         (0)     4480 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/test/log.py
--rw-r--r--   0 root         (0) root         (0)     2572 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/test/config.py
--rw-r--r--   0 root         (0) root         (0)     7104 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/test/structures.py
--rw-r--r--   0 root         (0) root         (0)    29883 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/test/util.py
--rw-r--r--   0 root         (0) root         (0)     4413 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/test/base.py
--rw-r--r--   0 root         (0) root         (0)    12229 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/test/validation.py
--rw-r--r--   0 root         (0) root         (0)     4429 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/test/mock.py
--rw-r--r--   0 root         (0) root         (0)    29867 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/test/model.py
--rw-r--r--   0 root         (0) root         (0)     6370 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/test/acl.py
--rw-r--r--   0 root         (0) root         (0)     8653 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/mongodb.py
--rw-r--r--   0 root         (0) root         (0)    35346 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/typesf.py
--rw-r--r--   0 root         (0) root         (0)    14014 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/log.py
--rw-r--r--   0 root         (0) root         (0)     8312 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/config.py
--rw-r--r--   0 root         (0) root         (0)     5581 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/session.py
--rw-r--r--   0 root         (0) root         (0)     4504 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/observer.py
--rw-r--r--   0 root         (0) root         (0)     2212 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/meta.py
--rw-r--r--   0 root         (0) root         (0)     8151 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/structures.py
--rw-r--r--   0 root         (0) root         (0)     4421 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/redisdb.py
--rw-r--r--   0 root         (0) root         (0)    56950 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/util.py
--rw-r--r--   0 root         (0) root         (0)     5913 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/template.py
--rw-r--r--   0 root         (0) root         (0)     7450 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/storage.py
--rw-r--r--   0 root         (0) root         (0)    40032 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/base.py
--rw-r--r--   0 root         (0) root         (0)    10401 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1888 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/date.py
--rw-r--r--   0 root         (0) root         (0)     2762 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/pusherc.py
--rw-r--r--   0 root         (0) root         (0)     1578 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/info.py
--rw-r--r--   0 root         (0) root         (0)    21292 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/validation.py
--rw-r--r--   0 root         (0) root         (0)     1562 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/jsonf.py
--rw-r--r--   0 root         (0) root         (0)     4344 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/formats.py
--rw-r--r--   0 root         (0) root         (0)     4468 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/extras.py
--rw-r--r--   0 root         (0) root         (0)   117879 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/model.py
--rw-r--r--   0 root         (0) root         (0)    12415 2023-01-06 12:28:32.000000 quorum-0.8.0/src/quorum/acl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 06:22:53.000000 quorum-0.8.1/
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-05-14 06:22:36.000000 quorum-0.8.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 06:22:53.000000 quorum-0.8.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 06:22:53.000000 quorum-0.8.1/src/quorum.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 06:22:53.000000 quorum-0.8.1/src/quorum.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-14 06:22:53.000000 quorum-0.8.1/src/quorum.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 06:22:41.000000 quorum-0.8.1/src/quorum.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-14 06:22:53.000000 quorum-0.8.1/src/quorum.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2947 2023-05-14 06:22:53.000000 quorum-0.8.1/src/quorum.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-05-14 06:22:53.000000 quorum-0.8.1/src/quorum.egg-info/SOURCES.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 06:22:53.000000 quorum-0.8.1/src/quorum/
+-rw-r--r--   0 root         (0) root         (0)     7450 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/storage.py
+-rw-r--r--   0 root         (0) root         (0)     5918 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/crypt.py
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/jsonf.py
+-rw-r--r--   0 root         (0) root         (0)    12415 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/acl.py
+-rw-r--r--   0 root         (0) root         (0)    39989 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/base.py
+-rw-r--r--   0 root         (0) root         (0)   117879 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/model.py
+-rw-r--r--   0 root         (0) root         (0)     2567 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/request.py
+-rw-r--r--   0 root         (0) root         (0)     2212 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/meta.py
+-rw-r--r--   0 root         (0) root         (0)     8312 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/config.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/unit_test.py
+-rw-r--r--   0 root         (0) root         (0)    14534 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/execution.py
+-rw-r--r--   0 root         (0) root         (0)    35346 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/typesf.py
+-rw-r--r--   0 root         (0) root         (0)    14572 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/data.py
+-rw-r--r--   0 root         (0) root         (0)    11475 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/mail.py
+-rw-r--r--   0 root         (0) root         (0)    10401 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     8284 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/daemon.py
+-rw-r--r--   0 root         (0) root         (0)     2934 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/amqp.py
+-rw-r--r--   0 root         (0) root         (0)     5913 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/template.py
+-rw-r--r--   0 root         (0) root         (0)     4468 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/extras.py
+-rw-r--r--   0 root         (0) root         (0)     8653 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/mongodb.py
+-rw-r--r--   0 root         (0) root         (0)     2762 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/pusherc.py
+-rw-r--r--   0 root         (0) root         (0)     8151 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/structures.py
+-rw-r--r--   0 root         (0) root         (0)     7167 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21292 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/validation.py
+-rw-r--r--   0 root         (0) root         (0)     4344 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/formats.py
+-rw-r--r--   0 root         (0) root         (0)     3125 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/amazon.py
+-rw-r--r--   0 root         (0) root         (0)     8233 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/route.py
+-rw-r--r--   0 root         (0) root         (0)     4421 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/redisdb.py
+-rw-r--r--   0 root         (0) root         (0)    29352 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/httpc.py
+-rw-r--r--   0 root         (0) root         (0)     4504 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/observer.py
+-rw-r--r--   0 root         (0) root         (0)     1578 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/info.py
+-rw-r--r--   0 root         (0) root         (0)    56950 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/util.py
+-rw-r--r--   0 root         (0) root         (0)    13063 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/legacy.py
+-rw-r--r--   0 root         (0) root         (0)    12158 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/export.py
+-rw-r--r--   0 root         (0) root         (0)     5581 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/session.py
+-rw-r--r--   0 root         (0) root         (0)     1446 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 06:22:53.000000 quorum-0.8.1/src/quorum/test/
+-rw-r--r--   0 root         (0) root         (0)     2681 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/test/crypt.py
+-rw-r--r--   0 root         (0) root         (0)     6370 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/test/acl.py
+-rw-r--r--   0 root         (0) root         (0)     4429 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/test/mock.py
+-rw-r--r--   0 root         (0) root         (0)     4413 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/test/base.py
+-rw-r--r--   0 root         (0) root         (0)    29867 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/test/model.py
+-rw-r--r--   0 root         (0) root         (0)     2572 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/test/config.py
+-rw-r--r--   0 root         (0) root         (0)     6706 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/test/execution.py
+-rw-r--r--   0 root         (0) root         (0)     8314 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/test/typesf.py
+-rw-r--r--   0 root         (0) root         (0)     1556 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/test/data.py
+-rw-r--r--   0 root         (0) root         (0)     2196 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/test/mail.py
+-rw-r--r--   0 root         (0) root         (0)     7104 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/test/structures.py
+-rw-r--r--   0 root         (0) root         (0)     1193 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12229 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/test/validation.py
+-rw-r--r--   0 root         (0) root         (0)     2434 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/test/amazon.py
+-rw-r--r--   0 root         (0) root         (0)     8415 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/test/httpc.py
+-rw-r--r--   0 root         (0) root         (0)    29883 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/test/util.py
+-rw-r--r--   0 root         (0) root         (0)     3637 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/test/export.py
+-rw-r--r--   0 root         (0) root         (0)     4480 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/test/log.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/date.py
+-rw-r--r--   0 root         (0) root         (0)    10207 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/defines.py
+-rw-r--r--   0 root         (0) root         (0)    14014 2023-05-14 06:22:36.000000 quorum-0.8.1/src/quorum/log.py
+-rw-r--r--   0 root         (0) root         (0)     2947 2023-05-14 06:22:53.000000 quorum-0.8.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2998 2023-05-14 06:22:36.000000 quorum-0.8.1/setup.py
+-rw-r--r--   0 root         (0) root         (0)       67 2023-05-14 06:22:53.000000 quorum-0.8.1/setup.cfg
```

### Comparing `quorum-0.8.0/README.md` & `quorum-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/PKG-INFO` & `quorum-0.8.1/src/quorum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum
-Version: 0.8.0
+Version: 0.8.1
 Summary: Quorum Extensions for Flask
 Home-page: http://flask-quorum.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [![Quorum Extensions for Flask](res/logo.png)](http://flask-quorum.hive.pt)
```

### Comparing `quorum-0.8.0/setup.py` & `quorum-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum.egg-info/PKG-INFO` & `quorum-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum
-Version: 0.8.0
+Version: 0.8.1
 Summary: Quorum Extensions for Flask
 Home-page: http://flask-quorum.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [![Quorum Extensions for Flask](res/logo.png)](http://flask-quorum.hive.pt)
```

### Comparing `quorum-0.8.0/src/quorum.egg-info/SOURCES.txt` & `quorum-0.8.1/src/quorum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/legacy.py` & `quorum-0.8.1/src/quorum/legacy.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/amqp.py` & `quorum-0.8.1/src/quorum/amqp.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/export.py` & `quorum-0.8.1/src/quorum/export.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/__init__.py` & `quorum-0.8.1/src/quorum/__init__.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/request.py` & `quorum-0.8.1/src/quorum/request.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/amazon.py` & `quorum-0.8.1/src/quorum/amazon.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/common.py` & `quorum-0.8.1/src/quorum/common.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/unit_test.py` & `quorum-0.8.1/src/quorum/unit_test.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/httpc.py` & `quorum-0.8.1/src/quorum/httpc.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/data.py` & `quorum-0.8.1/src/quorum/data.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/defines.py` & `quorum-0.8.1/src/quorum/defines.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/mail.py` & `quorum-0.8.1/src/quorum/mail.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/execution.py` & `quorum-0.8.1/src/quorum/execution.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/route.py` & `quorum-0.8.1/src/quorum/route.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/errors.py` & `quorum-0.8.1/src/quorum/errors.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/crypt.py` & `quorum-0.8.1/src/quorum/crypt.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/daemon.py` & `quorum-0.8.1/src/quorum/daemon.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/test/export.py` & `quorum-0.8.1/src/quorum/test/export.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/test/__init__.py` & `quorum-0.8.1/src/quorum/test/__init__.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/test/amazon.py` & `quorum-0.8.1/src/quorum/test/amazon.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/test/httpc.py` & `quorum-0.8.1/src/quorum/test/httpc.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/test/data.py` & `quorum-0.8.1/src/quorum/test/data.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/test/mail.py` & `quorum-0.8.1/src/quorum/test/mail.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/test/execution.py` & `quorum-0.8.1/src/quorum/test/execution.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/test/crypt.py` & `quorum-0.8.1/src/quorum/test/crypt.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/test/typesf.py` & `quorum-0.8.1/src/quorum/test/typesf.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/test/log.py` & `quorum-0.8.1/src/quorum/test/log.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/test/config.py` & `quorum-0.8.1/src/quorum/test/config.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/test/structures.py` & `quorum-0.8.1/src/quorum/test/structures.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/test/util.py` & `quorum-0.8.1/src/quorum/test/util.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/test/base.py` & `quorum-0.8.1/src/quorum/test/base.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/test/validation.py` & `quorum-0.8.1/src/quorum/test/validation.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/test/mock.py` & `quorum-0.8.1/src/quorum/test/mock.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/test/model.py` & `quorum-0.8.1/src/quorum/test/model.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/test/acl.py` & `quorum-0.8.1/src/quorum/test/acl.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/mongodb.py` & `quorum-0.8.1/src/quorum/mongodb.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/typesf.py` & `quorum-0.8.1/src/quorum/typesf.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/log.py` & `quorum-0.8.1/src/quorum/log.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/config.py` & `quorum-0.8.1/src/quorum/config.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/session.py` & `quorum-0.8.1/src/quorum/session.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/observer.py` & `quorum-0.8.1/src/quorum/observer.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/meta.py` & `quorum-0.8.1/src/quorum/meta.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/structures.py` & `quorum-0.8.1/src/quorum/structures.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/redisdb.py` & `quorum-0.8.1/src/quorum/redisdb.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/util.py` & `quorum-0.8.1/src/quorum/util.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/template.py` & `quorum-0.8.1/src/quorum/template.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/storage.py` & `quorum-0.8.1/src/quorum/storage.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/base.py` & `quorum-0.8.1/src/quorum/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -968,20 +968,20 @@
 def bundles_path():
     return os.path.join(APP.root_path, "bundles")
 
 def base_path(*args, **kwargs):
     return os.path.join(APP.root_path, *args)
 
 def has_context():
-    return True if flask._app_ctx_stack.top else False
+    return flask.has_app_context()
 
 def ensure_context(function):
     """
     Decorator that makes sure that the underlying execution
-    method/function is run inside a valid app context.
+    method/function is run inside a valid flask app context.
 
     In case there's currently no app context defined it uses
     the global Application reference to create a new one.
 
     :type function: Function
     :param function: The function that is going to be decorated
     by the current ensure decorator.
@@ -991,19 +991,19 @@
     """
 
     @functools.wraps(function)
     def interceptor(*args, **kwargs):
         _ctx = has_context()
         _app_ctx = APP.app_context() if APP else None
         _ensure = True if not _ctx and _app_ctx else False
-        try:
-            if _ensure: flask._app_ctx_stack.push(_app_ctx)
+        if _ensure:
+            with _app_ctx:
+                result = function(*args, **kwargs)
+        else:
             result = function(*args, **kwargs)
-        finally:
-            if _ensure: flask._app_ctx_stack.pop()
         return result
 
     return interceptor
 
 def onrun(function):
     fname = function.__name__
     if fname in RUN_F: return
```

### Comparing `quorum-0.8.0/src/quorum/exceptions.py` & `quorum-0.8.1/src/quorum/exceptions.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/date.py` & `quorum-0.8.1/src/quorum/date.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/pusherc.py` & `quorum-0.8.1/src/quorum/pusherc.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/info.py` & `quorum-0.8.1/src/quorum/info.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 NAME = "quorum"
-VERSION = "0.8.0"
+VERSION = "0.8.1"
 AUTHOR = "Hive Solutions Lda."
 EMAIL = "development@hive.pt"
 DESCRIPTION = "Quorum Extensions for Flask"
 LICENSE = "Apache License, Version 2.0"
 KEYWORDS = "quorum flask"
 URL = "http://flask-quorum.hive.pt"
 COPYRIGHT = "2008-2022 Hive Solutions Lda."
```

### Comparing `quorum-0.8.0/src/quorum/validation.py` & `quorum-0.8.1/src/quorum/validation.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/jsonf.py` & `quorum-0.8.1/src/quorum/jsonf.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/formats.py` & `quorum-0.8.1/src/quorum/formats.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/extras.py` & `quorum-0.8.1/src/quorum/extras.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/model.py` & `quorum-0.8.1/src/quorum/model.py`

 * *Files identical despite different names*

### Comparing `quorum-0.8.0/src/quorum/acl.py` & `quorum-0.8.1/src/quorum/acl.py`

 * *Files identical despite different names*

