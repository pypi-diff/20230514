# Comparing `tmp/cluedin-1.0.0.tar.gz` & `tmp/cluedin-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cluedin-1.0.0.tar", max compression
+gzip compressed data, was "cluedin-2.0.0rc1.tar", max compression
```

## Comparing `cluedin-1.0.0.tar` & `cluedin-2.0.0rc1.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0     1921 2023-05-07 18:04:57.326657 cluedin-1.0.0/README.md
--rw-r--r--   0        0        0      119 2023-05-07 15:56:18.443909 cluedin-1.0.0/cluedin/__init__.py
--rw-r--r--   0        0        0      664 2023-05-06 19:21:43.490227 cluedin-1.0.0/cluedin/auth.py
--rw-r--r--   0        0        0     1120 2023-05-07 16:45:36.605300 cluedin-1.0.0/cluedin/gql.py
--rw-r--r--   0        0        0      681 2023-05-07 15:56:40.250091 cluedin-1.0.0/cluedin/urls.py
--rw-r--r--   0        0        0      264 2023-05-06 19:41:45.000595 cluedin-1.0.0/cluedin/utils.py
--rw-r--r--   0        0        0      562 2023-05-07 19:23:43.864922 cluedin-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2694 1970-01-01 00:00:00.000000 cluedin-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-05-01 19:58:59.989579 cluedin-2.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     5472 2023-05-14 18:26:29.967372 cluedin-2.0.0rc1/cluedin/README.md
+-rw-r--r--   0        0        0      173 2023-05-14 10:49:18.017492 cluedin-2.0.0rc1/cluedin/__init__.py
+-rw-r--r--   0        0        0     3036 2023-05-14 18:11:54.236396 cluedin-2.0.0rc1/cluedin/account.py
+-rw-r--r--   0        0        0     5735 2023-05-14 18:11:54.245612 cluedin-2.0.0rc1/cluedin/context.py
+-rw-r--r--   0        0        0      119 2023-05-14 18:12:04.244035 cluedin-2.0.0rc1/cluedin/env.py
+-rw-r--r--   0        0        0     2061 2023-05-14 18:11:54.236405 cluedin-2.0.0rc1/cluedin/gql.py
+-rw-r--r--   0        0        0      492 2023-05-14 11:15:24.953207 cluedin-2.0.0rc1/cluedin/jwt.py
+-rw-r--r--   0        0        0     3853 2023-05-14 18:11:54.236485 cluedin-2.0.0rc1/cluedin/public.py
+-rw-r--r--   0        0        0      574 2023-05-13 22:10:06.320474 cluedin-2.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     6188 1970-01-01 00:00:00.000000 cluedin-2.0.0rc1/PKG-INFO
```

### Comparing `cluedin-1.0.0/pyproject.toml` & `cluedin-2.0.0rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "cluedin"
-version = "1.0.0"
+version = "2.0.0.rc1"
 description = "A Python client for CluedIn API."
 authors = ["Roman Klimenko <romaklimenko@gmail.com>"]
-readme = "README.md"
+readme = "cluedin/README.md"
 license = "MIT"
 keywords = ["cluedin", "mdm", "master data management"]
 maintainers = ["Roman Klimenko <romaklimenko@gmail.com>"]
 homepage = "https://github.com/romaklimenko/cluedin"
 repository = "https://github.com/romaklimenko/cluedin"
 
 [tool.poetry.dependencies]
```

