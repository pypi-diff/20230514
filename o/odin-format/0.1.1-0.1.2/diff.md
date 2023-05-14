# Comparing `tmp/odin_format-0.1.1.tar.gz` & `tmp/odin_format-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odin_format-0.1.1.tar", max compression
+gzip compressed data, was "odin_format-0.1.2.tar", max compression
```

## Comparing `odin_format-0.1.1.tar` & `odin_format-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0        0 2023-05-14 18:02:45.068300 odin_format-0.1.1/README.md
--rw-r--r--   0        0        0      419 2023-05-14 18:28:06.808103 odin_format-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 18:08:19.258257 odin_format-0.1.1/src/odin_format/__init__.py
--rw-r--r--   0        0        0      121 2023-05-14 18:26:20.738114 odin_format-0.1.1/src/odin_format/__main__.py
--rw-r--r--   0        0        0      252 2023-05-14 18:05:56.928275 odin_format-0.1.1/src/odin_format/formatter.py
--rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 odin_format-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-14 18:02:45.068300 odin_format-0.1.2/README.md
+-rw-r--r--   0        0        0      683 2023-05-14 19:50:08.617454 odin_format-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      125 2023-05-14 19:40:44.997530 odin_format-0.1.2/src/odin_format/__init__.py
+-rw-r--r--   0        0        0     1666 2023-05-14 19:46:10.577485 odin_format-0.1.2/src/odin_format/formatter.py
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 odin_format-0.1.2/PKG-INFO
```

