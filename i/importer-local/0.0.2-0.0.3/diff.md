# Comparing `tmp/importer-local-0.0.2.tar.gz` & `tmp/importer-local-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "importer-local-0.0.2.tar", last modified: Sat May 13 17:05:01 2023, max compression
+gzip compressed data, was "importer-local-0.0.3.tar", last modified: Sun May 14 16:17:07 2023, max compression
```

## Comparing `importer-local-0.0.2.tar` & `importer-local-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:05:01.914219 importer-local-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-13 17:05:01.914219 importer-local-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-13 17:04:50.000000 importer-local-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:05:01.914219 importer-local-0.0.2/importer_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-13 17:05:01.000000 importer-local-0.0.2/importer_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-13 17:05:01.000000 importer-local-0.0.2/importer_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 17:05:01.000000 importer-local-0.0.2/importer_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 17:05:01.000000 importer-local-0.0.2/importer_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 17:05:01.914219 importer-local-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-13 17:04:50.000000 importer-local-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:05:01.914219 importer-local-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-13 17:04:50.000000 importer-local-0.0.2/tests/test_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:17:07.377735 importer-local-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-14 16:17:07.377735 importer-local-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-14 16:16:56.000000 importer-local-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:17:07.377735 importer-local-0.0.3/importer_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-14 16:17:07.000000 importer-local-0.0.3/importer_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-14 16:17:07.000000 importer-local-0.0.3/importer_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 16:17:07.000000 importer-local-0.0.3/importer_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 16:17:07.000000 importer-local-0.0.3/importer_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 16:17:07.377735 importer-local-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-14 16:16:56.000000 importer-local-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:17:07.377735 importer-local-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-14 16:16:56.000000 importer-local-0.0.3/tests/test_importer.py
```

### Comparing `importer-local-0.0.2/setup.py` & `importer-local-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
      # TODO: Please update the name
      name='importer-local',
-     version='0.0.2',
+     version='0.0.3',
      author="Circles",
      author_email="info@circles.life",
      description="PyPI Package for Circles Local importer Python",
-     long_description="This is a package for sharing common XXX function used in different repositories",
+     long_description="This is a package for sharing common importer function used in different repositories",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
      classifiers=[
          "Programming Language :: Python :: 3",
          "License :: Other/Proprietary License",
          "Operating System :: OS Independent",
```

### Comparing `importer-local-0.0.2/tests/test_importer.py` & `importer-local-0.0.3/tests/test_importer.py`

 * *Files identical despite different names*

