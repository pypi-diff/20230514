# Comparing `tmp/sg_hello_pypi-0.1.0.tar.gz` & `tmp/sg_hello_pypi-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sg_hello_pypi-0.1.0.tar", max compression
+gzip compressed data, was "sg_hello_pypi-0.2.1.tar", max compression
```

## Comparing `sg_hello_pypi-0.1.0.tar` & `sg_hello_pypi-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1054 2023-05-09 14:23:34.935168 sg_hello_pypi-0.1.0/LICENSE
--rw-r--r--   0        0        0       13 2023-05-09 14:23:34.935168 sg_hello_pypi-0.1.0/README.md
--rw-r--r--   0        0        0      452 2023-05-09 14:23:34.935168 sg_hello_pypi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      139 2023-05-09 14:23:34.935168 sg_hello_pypi-0.1.0/sg_hello_pypi/__init__.py
--rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 sg_hello_pypi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1054 2023-05-14 12:04:54.650317 sg_hello_pypi-0.2.1/LICENSE
+-rw-r--r--   0        0        0      284 2023-05-14 12:04:54.650317 sg_hello_pypi-0.2.1/README.md
+-rw-r--r--   0        0        0      452 2023-05-14 12:04:54.650317 sg_hello_pypi-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      139 2023-05-14 12:04:54.650317 sg_hello_pypi-0.2.1/sg_hello_pypi/__init__.py
+-rw-r--r--   0        0        0      861 1970-01-01 00:00:00.000000 sg_hello_pypi-0.2.1/PKG-INFO
```

### Comparing `sg_hello_pypi-0.1.0/LICENSE` & `sg_hello_pypi-0.2.1/LICENSE`

 * *Files identical despite different names*

