# Comparing `tmp/importer-local-0.0.1.tar.gz` & `tmp/importer-local-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "importer-local-0.0.1.tar", last modified: Sat May 13 12:22:18 2023, max compression
+gzip compressed data, was "importer-local-0.0.2.tar", last modified: Sat May 13 17:05:01 2023, max compression
```

## Comparing `importer-local-0.0.1.tar` & `importer-local-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 12:22:18.886570 importer-local-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-13 12:22:18.882570 importer-local-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-13 12:22:02.000000 importer-local-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 12:22:18.882570 importer-local-0.0.1/importer_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-13 12:22:18.000000 importer-local-0.0.1/importer_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-13 12:22:18.000000 importer-local-0.0.1/importer_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 12:22:18.000000 importer-local-0.0.1/importer_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 12:22:18.000000 importer-local-0.0.1/importer_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 12:22:18.886570 importer-local-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-13 12:22:02.000000 importer-local-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:05:01.914219 importer-local-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-13 17:05:01.914219 importer-local-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-13 17:04:50.000000 importer-local-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:05:01.914219 importer-local-0.0.2/importer_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-13 17:05:01.000000 importer-local-0.0.2/importer_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-13 17:05:01.000000 importer-local-0.0.2/importer_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 17:05:01.000000 importer-local-0.0.2/importer_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 17:05:01.000000 importer-local-0.0.2/importer_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 17:05:01.914219 importer-local-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-13 17:04:50.000000 importer-local-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:05:01.914219 importer-local-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-13 17:04:50.000000 importer-local-0.0.2/tests/test_importer.py
```

### Comparing `importer-local-0.0.1/setup.py` & `importer-local-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
      # TODO: Please update the name
      name='importer-local',
-     version='0.0.1',
+     version='0.0.2',
      author="Circles",
      author_email="info@circles.life",
      description="PyPI Package for Circles Local importer Python",
      long_description="This is a package for sharing common XXX function used in different repositories",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

