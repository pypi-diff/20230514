# Comparing `tmp/multicloud_diagrams-0.2.1.tar.gz` & `tmp/multicloud_diagrams-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multicloud_diagrams-0.2.1.tar", max compression
+gzip compressed data, was "multicloud_diagrams-0.2.2.tar", max compression
```

## Comparing `multicloud_diagrams-0.2.1.tar` & `multicloud_diagrams-0.2.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1069 2023-05-14 15:36:37.276228 multicloud_diagrams-0.2.1/LICENSE
--rw-r--r--   0        0        0        0 2023-05-14 15:51:16.576166 multicloud_diagrams-0.2.1/README.md
--rw-r--r--   0        0        0    17035 2023-05-14 17:33:30.479330 multicloud_diagrams-0.2.1/multicloud_diagrams/__init__.py
--rw-r--r--   0        0        0      509 2023-05-14 18:13:39.252207 multicloud_diagrams-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 multicloud_diagrams-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-14 15:36:37.276228 multicloud_diagrams-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2292 2023-05-14 20:59:03.162735 multicloud_diagrams-0.2.2/README.md
+-rw-r--r--   0        0        0    17035 2023-05-14 17:33:30.479330 multicloud_diagrams-0.2.2/multicloud_diagrams/__init__.py
+-rw-r--r--   0        0        0      509 2023-05-14 20:59:57.294501 multicloud_diagrams-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2810 1970-01-01 00:00:00.000000 multicloud_diagrams-0.2.2/PKG-INFO
```

### Comparing `multicloud_diagrams-0.2.1/LICENSE` & `multicloud_diagrams-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `multicloud_diagrams-0.2.1/multicloud_diagrams/__init__.py` & `multicloud_diagrams-0.2.2/multicloud_diagrams/__init__.py`

 * *Files identical despite different names*

