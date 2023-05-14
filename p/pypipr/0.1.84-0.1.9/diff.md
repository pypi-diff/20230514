# Comparing `tmp/pypipr-0.1.84.tar.gz` & `tmp/pypipr-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypipr-0.1.84.tar", max compression
+gzip compressed data, was "pypipr-0.1.9.tar", max compression
```

## Comparing `pypipr-0.1.84.tar` & `pypipr-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0        0 2022-10-24 06:22:00.291550 pypipr-0.1.84/pypipr/__init__.py
--rw-r--r--   0        0        0    21102 2023-05-14 16:42:57.753780 pypipr-0.1.84/pypipr/pypipr.py
--rw-r--r--   0        0        0      615 2023-05-14 16:44:46.390566 pypipr-0.1.84/pyproject.toml
--rw-r--r--   0        0        0    12022 2023-05-14 15:08:39.694609 pypipr-0.1.84/README.md
--rw-r--r--   0        0        0    12917 1970-01-01 00:00:00.000000 pypipr-0.1.84/setup.py
--rw-r--r--   0        0        0    12108 1970-01-01 00:00:00.000000 pypipr-0.1.84/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-10-11 16:47:36.486008 pypipr-0.1.9/pypipr/__init__.py
+-rw-r--r--   0        0        0     1816 2022-10-14 15:45:39.479083 pypipr-0.1.9/pypipr/iconsole.py
+-rw-r--r--   0        0        0      199 2022-10-14 15:23:12.870383 pypipr-0.1.9/pypipr/iconstant.py
+-rw-r--r--   0        0        0      315 2022-10-14 15:23:37.319991 pypipr-0.1.9/pypipr/idatetime.py
+-rw-r--r--   0        0        0      252 2022-10-14 15:24:05.627645 pypipr-0.1.9/pypipr/pypipr.py
+-rw-r--r--   0        0        0      358 2022-10-14 15:54:43.270169 pypipr-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1746 2022-10-14 15:42:50.506147 pypipr-0.1.9/README.md
+-rw-r--r--   0        0        0     2400 1970-01-01 00:00:00.000000 pypipr-0.1.9/setup.py
+-rw-r--r--   0        0        0     2132 1970-01-01 00:00:00.000000 pypipr-0.1.9/PKG-INFO
```

