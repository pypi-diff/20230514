# Comparing `tmp/depthcharge-ms-0.2.0.tar.gz` & `tmp/depthcharge-ms-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depthcharge-ms-0.2.0.tar", last modified: Thu Apr  6 15:33:52 2023, max compression
+gzip compressed data, was "depthcharge-ms-0.2.1.tar", last modified: Sun May 14 05:03:38 2023, max compression
```

## Comparing `depthcharge-ms-0.2.0.tar` & `depthcharge-ms-0.2.1.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:33:52.470213 depthcharge-ms-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:33:52.462213 depthcharge-ms-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:33:52.466213 depthcharge-ms-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-06 15:33:52.470213 depthcharge-ms-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:33:52.466213 depthcharge-ms-0.2.0/data/
--rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/data/TMT10-Trial-8.mgf
--rw-r--r--   0 runner    (1001) docker     (123)   333865 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/data/TMT10-Trial-8.mzML
--rw-r--r--   0 runner    (1001) docker     (123)    67798 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/data/TMT10-Trial-8.mzXML
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:33:52.466213 depthcharge-ms-0.2.0/depthcharge/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/depthcharge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:33:52.466213 depthcharge-ms-0.2.0/depthcharge/components/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/depthcharge/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/depthcharge/components/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/depthcharge/components/feedforward.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/depthcharge/components/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    15872 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/depthcharge/components/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:33:52.466213 depthcharge-ms-0.2.0/depthcharge/data/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/depthcharge/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/depthcharge/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/depthcharge/data/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/depthcharge/data/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/depthcharge/data/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/depthcharge/masses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/depthcharge/similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/depthcharge/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/depthcharge/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:33:52.466213 depthcharge-ms-0.2.0/depthcharge_ms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-06 15:33:52.000000 depthcharge-ms-0.2.0/depthcharge_ms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-06 15:33:52.000000 depthcharge-ms-0.2.0/depthcharge_ms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 15:33:52.000000 depthcharge-ms-0.2.0/depthcharge_ms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-06 15:33:52.000000 depthcharge-ms-0.2.0/depthcharge_ms.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-06 15:33:52.000000 depthcharge-ms-0.2.0/depthcharge_ms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-06 15:33:52.000000 depthcharge-ms-0.2.0/depthcharge_ms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:33:52.466213 depthcharge-ms-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:33:52.470213 depthcharge-ms-0.2.0/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-06 15:33:52.470213 depthcharge-ms-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:33:52.470213 depthcharge-ms-0.2.0/static/
--rw-r--r--   0 runner    (1001) docker     (123)    15364 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/static/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    24683 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/static/logo-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    25343 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/static/logo-light.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:33:52.470213 depthcharge-ms-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:33:52.470213 depthcharge-ms-0.2.0/tests/unit_tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:33:52.470213 depthcharge-ms-0.2.0/tests/unit_tests/test_components/
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/tests/unit_tests/test_components/test_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/tests/unit_tests/test_components/test_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:33:52.470213 depthcharge-ms-0.2.0/tests/unit_tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/tests/unit_tests/test_data/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/tests/unit_tests/test_data/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/tests/unit_tests/test_data/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/tests/unit_tests/test_masses.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-06 15:33:28.000000 depthcharge-ms-0.2.0/tests/unit_tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.180362 depthcharge-ms-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.172362 depthcharge-ms-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.176362 depthcharge-ms-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-14 05:03:38.180362 depthcharge-ms-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.176362 depthcharge-ms-0.2.1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/data/TMT10-Trial-8.mgf
+-rw-r--r--   0 runner    (1001) docker     (123)   333865 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/data/TMT10-Trial-8.mzML
+-rw-r--r--   0 runner    (1001) docker     (123)    67798 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/data/TMT10-Trial-8.mzXML
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.176362 depthcharge-ms-0.2.1/depthcharge/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.176362 depthcharge-ms-0.2.1/depthcharge/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/components/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/components/feedforward.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/components/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15540 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/components/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.176362 depthcharge-ms-0.2.1/depthcharge/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/data/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/data/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/data/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/masses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.180362 depthcharge-ms-0.2.1/depthcharge_ms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-14 05:03:38.000000 depthcharge-ms-0.2.1/depthcharge_ms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-14 05:03:38.000000 depthcharge-ms-0.2.1/depthcharge_ms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 05:03:38.000000 depthcharge-ms-0.2.1/depthcharge_ms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-14 05:03:38.000000 depthcharge-ms-0.2.1/depthcharge_ms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-14 05:03:38.000000 depthcharge-ms-0.2.1/depthcharge_ms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 05:03:38.000000 depthcharge-ms-0.2.1/depthcharge_ms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.180362 depthcharge-ms-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.180362 depthcharge-ms-0.2.1/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-14 05:03:38.180362 depthcharge-ms-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.180362 depthcharge-ms-0.2.1/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15364 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/static/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    24683 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/static/logo-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25343 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/static/logo-light.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.180362 depthcharge-ms-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.180362 depthcharge-ms-0.2.1/tests/unit_tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.180362 depthcharge-ms-0.2.1/tests/unit_tests/test_components/
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/tests/unit_tests/test_components/test_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/tests/unit_tests/test_components/test_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.180362 depthcharge-ms-0.2.1/tests/unit_tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/tests/unit_tests/test_data/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/tests/unit_tests/test_data/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/tests/unit_tests/test_data/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/tests/unit_tests/test_data/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/tests/unit_tests/test_masses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/tests/unit_tests/test_utils.py
```

### Comparing `depthcharge-ms-0.2.0/.github/workflows/lint.yml` & `depthcharge-ms-0.2.1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/.github/workflows/publish.yml` & `depthcharge-ms-0.2.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/.github/workflows/tests.yml` & `depthcharge-ms-0.2.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/CHANGELOG.md` & `depthcharge-ms-0.2.1/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
-## [0.2.0] - 2023-03-06
+## [v0.2.1] - 2023-05-13
+### Changed
+- Change target mask from float to boolean.
+- Log the number spectra that are skipped due to an invalid precursor charge.
+
+## [v0.2.0] - 2023-03-06
 ### Breaking Changes
 - Dropped pytorch-lightning as a dependency.
 - Removed SpectrumDataModule
 - Removed full-blown models (depthcharge.models)
 - Fixed sinusoidal encoders (Issue #27)
 - `MassEncoder` is now `FloatEncoder`, because its generally useful for encoding floating-point numbers.
 
@@ -19,15 +24,15 @@
 
 ### Changed
 - Tensorboard is now an optional dependency.
 
 ### Removed
 - The example de novo peptide sequencing model.
 
-## [0.1.0] - 2022-11-15
+## [v0.1.0] - 2022-11-15
 ### Changed
 - The `detokenize()` method now returns a list instead of a string.
 
-## [0.0.1] - 2022-09-29
+## [v0.0.1] - 2022-09-29
 ### Added
 - This if the first release! All changes from this point forward will be
   recorded in this changelog.
```

### Comparing `depthcharge-ms-0.2.0/CODE_OF_CONDUCT.md` & `depthcharge-ms-0.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/CONTRIBUTING.md` & `depthcharge-ms-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/LICENSE` & `depthcharge-ms-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/PKG-INFO` & `depthcharge-ms-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: depthcharge-ms
-Version: 0.2.0
+Version: 0.2.1
 Summary: A deep learning toolkit for proteomics
 Home-page: https://github.com/wfondrie/depthcharge
 Author: William E. Fondrie
 Author-email: fondriew@gmail.com
 License: Apache 2.0
 Project-URL: Documentation, https://depthcharge.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/wfondrie/depthcharge/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: depthcharge-ms Version: 0.2.0 Summary: A deep
+Metadata-Version: 2.1 Name: depthcharge-ms Version: 0.2.1 Summary: A deep
 learning toolkit for proteomics Home-page: https://github.com/wfondrie/
 depthcharge Author: William E. Fondrie Author-email: fondriew@gmail.com
 License: Apache 2.0 Project-URL: Documentation, https://
 depthcharge.readthedocs.io Project-URL: Bug Tracker, https://github.com/
 wfondrie/depthcharge/issues Project-URL: Discussion Board, https://github.com/
 wfondrie/depthcharge/discussions Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: Apache Software License Classifier:
```

### Comparing `depthcharge-ms-0.2.0/README.md` & `depthcharge-ms-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/data/TMT10-Trial-8.mgf` & `depthcharge-ms-0.2.1/data/TMT10-Trial-8.mgf`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/data/TMT10-Trial-8.mzML` & `depthcharge-ms-0.2.1/data/TMT10-Trial-8.mzML`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/data/TMT10-Trial-8.mzXML` & `depthcharge-ms-0.2.1/data/TMT10-Trial-8.mzXML`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/depthcharge/components/encoders.py` & `depthcharge-ms-0.2.1/depthcharge/components/encoders.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/depthcharge/components/feedforward.py` & `depthcharge-ms-0.2.1/depthcharge/components/feedforward.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/depthcharge/components/transformers.py` & `depthcharge-ms-0.2.1/depthcharge/components/transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -445,26 +445,15 @@
             tgt_key_padding_mask=tgt_key_padding_mask,
             memory_key_padding_mask=memory_key_padding_mask.to(self.device),
         )
         return self.final(preds), tokens
 
 
 def generate_tgt_mask(sz):
-    """Generate a square mask for the sequence. The masked positions
-    are filled with float('-inf'). Unmasked positions are filled with
-    float(0.0).
-
-    This function is a slight modification of the version in the PyTorch
-    repository.
+    """Generate a square mask for the sequence.
 
     Parameters
     ----------
     sz : int
         The length of the target sequence.
     """
-    mask = (torch.triu(torch.ones(sz, sz)) == 1).transpose(0, 1)
-    mask = (
-        mask.float()
-        .masked_fill(mask == 0, float("-inf"))
-        .masked_fill(mask == 1, float(0.0))
-    )
-    return mask
+    return ~torch.triu(torch.ones(sz, sz, dtype=torch.bool)).transpose(0, 1)
```

### Comparing `depthcharge-ms-0.2.0/depthcharge/data/datasets.py` & `depthcharge-ms-0.2.1/depthcharge/data/datasets.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/depthcharge/data/hdf5.py` & `depthcharge-ms-0.2.1/depthcharge/data/hdf5.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/depthcharge/data/parsers.py` & `depthcharge-ms-0.2.1/depthcharge/data/parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,20 @@
         ----------
         spectrum : dict
             The dictionary defining the spectrum in a given format.
         """
         pass
 
     def read(self):
-        """Read the ms data file"""
+        """Read the ms data file.
+
+        Returns
+        -------
+        Self
+        """
         n_skipped = 0
         with self.open() as spectra:
             for spectrum in tqdm(spectra, desc=str(self.path), unit="spectra"):
                 try:
                     self.parse_spectrum(spectrum)
                 except (IndexError, KeyError, ValueError):
                     n_skipped += 1
@@ -90,14 +95,15 @@
         # Build the index
         sizes = np.array([0] + [s.shape[0] for s in self.mz_arrays])
         self.offset = sizes[:-1].cumsum()
         self.mz_arrays = np.concatenate(self.mz_arrays).astype(np.float64)
         self.intensity_arrays = np.concatenate(self.intensity_arrays).astype(
             np.float32
         )
+        return self
 
     @property
     def n_spectra(self):
         """The number of spectra"""
         return self.offset.shape[0]
 
     @property
@@ -158,14 +164,16 @@
 
         if self.valid_charge is None or precursor_charge in self.valid_charge:
             self.mz_arrays.append(spectrum["m/z array"])
             self.intensity_arrays.append(spectrum["intensity array"])
             self.precursor_mz.append(precursor_mz)
             self.precursor_charge.append(precursor_charge)
             self.scan_id.append(_parse_scan_id(spectrum["id"]))
+        else:
+            raise ValueError("Invalid precursor charge")
 
 
 class MzxmlParser(BaseParser):
     """Parse mass spectra from an mzXML file.
 
     Parameters
     ----------
@@ -210,14 +218,16 @@
 
         if self.valid_charge is None or precursor_charge in self.valid_charge:
             self.mz_arrays.append(spectrum["m/z array"])
             self.intensity_arrays.append(spectrum["intensity array"])
             self.precursor_mz.append(precursor_mz)
             self.precursor_charge.append(precursor_charge)
             self.scan_id.append(_parse_scan_id(spectrum["id"]))
+        else:
+            raise ValueError("Invalid precursor charge")
 
 
 class MgfParser(BaseParser):
     """Parse mass spectra from an MGF file.
 
     Parameters
     ----------
@@ -243,28 +253,30 @@
         super().__init__(
             ms_data_file,
             ms_level=ms_level,
             valid_charge=valid_charge,
             id_type="index",
         )
         self.annotations = [] if annotations else None
-        self._counter = 0
+        self._counter = -1
 
     def open(self):
         """Open the MGF file for reading"""
         return MGF(str(self.path))
 
     def parse_spectrum(self, spectrum):
         """Parse a single spectrum.
 
         Parameters
         ----------
         spectrum : dict
             The dictionary defining the spectrum in MGF format.
         """
+        self._counter += 1
+
         if self.ms_level > 1:
             precursor_mz = float(spectrum["params"]["pepmass"][0])
             precursor_charge = int(spectrum["params"].get("charge", [0])[0])
         else:
             precursor_mz, precursor_charge = None, 0
 
         if self.annotations is not None:
@@ -272,16 +284,16 @@
 
         if self.valid_charge is None or precursor_charge in self.valid_charge:
             self.mz_arrays.append(spectrum["m/z array"])
             self.intensity_arrays.append(spectrum["intensity array"])
             self.precursor_mz.append(precursor_mz)
             self.precursor_charge.append(precursor_charge)
             self.scan_id.append(self._counter)
-
-        self._counter += 1
+        else:
+            raise ValueError("Invalid precursor charge")
 
 
 def _parse_scan_id(scan_str):
     """Remove the string prefix from the scan ID.
 
     Adapted from:
     https://github.com/bittremieux/GLEAMS/blob/
```

### Comparing `depthcharge-ms-0.2.0/depthcharge/data/preprocessing.py` & `depthcharge-ms-0.2.1/depthcharge/data/preprocessing.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
 def remove_precursor_peak(
     mz_array: torch.Tensor,
     int_array: torch.Tensor,
     precursor_mz: float,
     tol: float = 1.5,
 ) -> Tuple[torch.Tensor, torch.Tensor]:
-    """Square root the intensities and scale to unit norm.
+    """Remove peaks near the precursor m/z.
 
     Parameters
     ----------
     mz_array : torch.Tensor of shape (n_peaks,)
         The m/z values of the peaks in the spectrum.
     int_array : torch.Tensor of shape (n_peaks,)
         The intensity values of the peaks in the spectrum.
```

### Comparing `depthcharge-ms-0.2.0/depthcharge/masses.py` & `depthcharge-ms-0.2.1/depthcharge/masses.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/depthcharge/similarity.py` & `depthcharge-ms-0.2.1/depthcharge/similarity.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/depthcharge/utils.py` & `depthcharge-ms-0.2.1/depthcharge/utils.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/depthcharge/version.py` & `depthcharge-ms-0.2.1/depthcharge/version.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/depthcharge_ms.egg-info/PKG-INFO` & `depthcharge-ms-0.2.1/depthcharge_ms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: depthcharge-ms
-Version: 0.2.0
+Version: 0.2.1
 Summary: A deep learning toolkit for proteomics
 Home-page: https://github.com/wfondrie/depthcharge
 Author: William E. Fondrie
 Author-email: fondriew@gmail.com
 License: Apache 2.0
 Project-URL: Documentation, https://depthcharge.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/wfondrie/depthcharge/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: depthcharge-ms Version: 0.2.0 Summary: A deep
+Metadata-Version: 2.1 Name: depthcharge-ms Version: 0.2.1 Summary: A deep
 learning toolkit for proteomics Home-page: https://github.com/wfondrie/
 depthcharge Author: William E. Fondrie Author-email: fondriew@gmail.com
 License: Apache 2.0 Project-URL: Documentation, https://
 depthcharge.readthedocs.io Project-URL: Bug Tracker, https://github.com/
 wfondrie/depthcharge/issues Project-URL: Discussion Board, https://github.com/
 wfondrie/depthcharge/discussions Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: Apache Software License Classifier:
```

### Comparing `depthcharge-ms-0.2.0/depthcharge_ms.egg-info/SOURCES.txt` & `depthcharge-ms-0.2.1/depthcharge_ms.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -45,8 +45,9 @@
 tests/conftest.py
 tests/unit_tests/test_masses.py
 tests/unit_tests/test_utils.py
 tests/unit_tests/test_components/test_encoders.py
 tests/unit_tests/test_components/test_transformers.py
 tests/unit_tests/test_data/test_datasets.py
 tests/unit_tests/test_data/test_index.py
-tests/unit_tests/test_data/test_loaders.py
+tests/unit_tests/test_data/test_loaders.py
+tests/unit_tests/test_data/test_parsers.py
```

### Comparing `depthcharge-ms-0.2.0/docs/README.md` & `depthcharge-ms-0.2.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/mkdocs.yml` & `depthcharge-ms-0.2.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/pyproject.toml` & `depthcharge-ms-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/setup.cfg` & `depthcharge-ms-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/static/icon.svg` & `depthcharge-ms-0.2.1/static/icon.svg`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/static/logo-dark.png` & `depthcharge-ms-0.2.1/static/logo-dark.png`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/static/logo-light.png` & `depthcharge-ms-0.2.1/static/logo-light.png`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/tests/conftest.py` & `depthcharge-ms-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/tests/unit_tests/test_components/test_encoders.py` & `depthcharge-ms-0.2.1/tests/unit_tests/test_components/test_encoders.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/tests/unit_tests/test_components/test_transformers.py` & `depthcharge-ms-0.2.1/tests/unit_tests/test_components/test_transformers.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/tests/unit_tests/test_data/test_datasets.py` & `depthcharge-ms-0.2.1/tests/unit_tests/test_data/test_datasets.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/tests/unit_tests/test_data/test_index.py` & `depthcharge-ms-0.2.1/tests/unit_tests/test_data/test_index.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/tests/unit_tests/test_data/test_loaders.py` & `depthcharge-ms-0.2.1/tests/unit_tests/test_data/test_loaders.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.0/tests/unit_tests/test_masses.py` & `depthcharge-ms-0.2.1/tests/unit_tests/test_masses.py`

 * *Files identical despite different names*

