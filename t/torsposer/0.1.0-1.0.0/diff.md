# Comparing `tmp/torsposer-0.1.0.tar.gz` & `tmp/torsposer-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torsposer-0.1.0.tar", max compression
+gzip compressed data, was "torsposer-1.0.0.tar", max compression
```

## Comparing `torsposer-0.1.0.tar` & `torsposer-1.0.0.tar`

### file list

```diff
@@ -1,4 +1,7 @@
--rw-r--r--   0        0        0       84 2023-05-14 10:48:02.657735 torsposer-0.1.0/README.md
--rw-r--r--   0        0        0      370 2023-05-14 10:47:18.020202 torsposer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 10:44:54.667172 torsposer-0.1.0/torsposer/__init__.py
--rw-r--r--   0        0        0      666 1970-01-01 00:00:00.000000 torsposer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1900 2023-05-14 19:20:52.604608 torsposer-1.0.0/README.md
+-rw-r--r--   0        0        0      729 2023-05-14 19:24:01.708535 torsposer-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-14 10:44:54.667172 torsposer-1.0.0/torsposer/__init__.py
+-rw-r--r--   0        0        0     1874 2023-05-14 18:57:17.103999 torsposer-1.0.0/torsposer/__main__.py
+-rw-r--r--   0        0        0     6445 2023-05-14 19:17:42.926054 torsposer-1.0.0/torsposer/exposer.py
+-rw-r--r--   0        0        0     1675 2023-05-14 13:05:18.790297 torsposer-1.0.0/torsposer/utils.py
+-rw-r--r--   0        0        0     2800 1970-01-01 00:00:00.000000 torsposer-1.0.0/PKG-INFO
```

