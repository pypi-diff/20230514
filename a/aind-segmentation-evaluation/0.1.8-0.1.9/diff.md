# Comparing `tmp/aind_segmentation_evaluation-0.1.8.tar.gz` & `tmp/aind_segmentation_evaluation-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_segmentation_evaluation-0.1.8.tar", last modified: Wed May 10 05:48:26 2023, max compression
+gzip compressed data, was "aind_segmentation_evaluation-0.1.9.tar", last modified: Wed May 10 05:48:44 2023, max compression
```

## Comparing `aind_segmentation_evaluation-0.1.8.tar` & `aind_segmentation_evaluation-0.1.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:48:26.811197 aind_segmentation_evaluation-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:48:26.715196 aind_segmentation_evaluation-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:48:26.719196 aind_segmentation_evaluation-0.1.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:48:26.719196 aind_segmentation_evaluation-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/.github/workflows/lint_and_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-10 05:48:26.811197 aind_segmentation_evaluation-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:48:26.719196 aind_segmentation_evaluation-0.1.8/doc_template/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:48:26.719196 aind_segmentation_evaluation-0.1.8/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:48:26.723196 aind_segmentation_evaluation-0.1.8/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)   259838 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:48:26.791197 aind_segmentation_evaluation-0.1.8/resources/
--rw-r--r--   0 runner    (1001) docker     (123)  9456994 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/resources/merge_edges.tif
--rw-r--r--   0 runner    (1001) docker     (123)  9456994 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/resources/merge_sites.tif
--rw-r--r--   0 runner    (1001) docker     (123)  9456994 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/resources/pred_volume.tif
--rw-r--r--   0 runner    (1001) docker     (123)  9456994 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/resources/split_edges.tif
--rw-r--r--   0 runner    (1001) docker     (123)  9456994 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/resources/split_sites.tif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:48:26.807197 aind_segmentation_evaluation-0.1.8/resources/target_graphs/
--rw-r--r--   0 runner    (1001) docker     (123)    72420 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/resources/target_graphs/0.swc
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/resources/target_graphs/1.swc
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/resources/target_graphs/2.swc
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/resources/target_graphs/3.swc
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/resources/target_graphs/4.swc
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/resources/target_graphs/5.swc
--rw-r--r--   0 runner    (1001) docker     (123)  9602600 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/resources/target_volume.tif
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 05:48:26.811197 aind_segmentation_evaluation-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:48:26.715196 aind_segmentation_evaluation-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:48:26.811197 aind_segmentation_evaluation-0.1.8/src/aind_segmentation_evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-10 05:48:05.000000 aind_segmentation_evaluation-0.1.8/src/aind_segmentation_evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/src/aind_segmentation_evaluation/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/src/aind_segmentation_evaluation/explore_branches.py
--rw-r--r--   0 runner    (1001) docker     (123)    11987 2023-05-10 05:48:05.000000 aind_segmentation_evaluation-0.1.8/src/aind_segmentation_evaluation/graph_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     9992 2023-05-10 05:48:05.000000 aind_segmentation_evaluation-0.1.8/src/aind_segmentation_evaluation/merge_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-05-10 05:48:05.000000 aind_segmentation_evaluation-0.1.8/src/aind_segmentation_evaluation/seg_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/src/aind_segmentation_evaluation/split_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/src/aind_segmentation_evaluation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:48:26.811197 aind_segmentation_evaluation-0.1.8/src/aind_segmentation_evaluation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-10 05:48:26.000000 aind_segmentation_evaluation-0.1.8/src/aind_segmentation_evaluation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-10 05:48:26.000000 aind_segmentation_evaluation-0.1.8/src/aind_segmentation_evaluation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 05:48:26.000000 aind_segmentation_evaluation-0.1.8/src/aind_segmentation_evaluation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-10 05:48:26.000000 aind_segmentation_evaluation-0.1.8/src/aind_segmentation_evaluation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-10 05:48:26.000000 aind_segmentation_evaluation-0.1.8/src/aind_segmentation_evaluation.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:48:26.811197 aind_segmentation_evaluation-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-10 05:48:04.000000 aind_segmentation_evaluation-0.1.8/tests/unit_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:48:44.601880 aind_segmentation_evaluation-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:48:44.541881 aind_segmentation_evaluation-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:48:44.541881 aind_segmentation_evaluation-0.1.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:48:44.541881 aind_segmentation_evaluation-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/.github/workflows/lint_and_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-10 05:48:44.601880 aind_segmentation_evaluation-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:48:44.541881 aind_segmentation_evaluation-0.1.9/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:48:44.541881 aind_segmentation_evaluation-0.1.9/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:48:44.545881 aind_segmentation_evaluation-0.1.9/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   259838 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:48:44.589880 aind_segmentation_evaluation-0.1.9/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)  9456994 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/resources/merge_edges.tif
+-rw-r--r--   0 runner    (1001) docker     (123)  9456994 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/resources/merge_sites.tif
+-rw-r--r--   0 runner    (1001) docker     (123)  9456994 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/resources/pred_volume.tif
+-rw-r--r--   0 runner    (1001) docker     (123)  9456994 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/resources/split_edges.tif
+-rw-r--r--   0 runner    (1001) docker     (123)  9456994 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/resources/split_sites.tif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:48:44.597880 aind_segmentation_evaluation-0.1.9/resources/target_graphs/
+-rw-r--r--   0 runner    (1001) docker     (123)    72420 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/resources/target_graphs/0.swc
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/resources/target_graphs/1.swc
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/resources/target_graphs/2.swc
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/resources/target_graphs/3.swc
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/resources/target_graphs/4.swc
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/resources/target_graphs/5.swc
+-rw-r--r--   0 runner    (1001) docker     (123)  9602600 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/resources/target_volume.tif
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 05:48:44.601880 aind_segmentation_evaluation-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:48:44.541881 aind_segmentation_evaluation-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:48:44.601880 aind_segmentation_evaluation-0.1.9/src/aind_segmentation_evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/src/aind_segmentation_evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/src/aind_segmentation_evaluation/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/src/aind_segmentation_evaluation/explore_branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11987 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/src/aind_segmentation_evaluation/graph_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9992 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/src/aind_segmentation_evaluation/merge_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/src/aind_segmentation_evaluation/seg_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/src/aind_segmentation_evaluation/split_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/src/aind_segmentation_evaluation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:48:44.601880 aind_segmentation_evaluation-0.1.9/src/aind_segmentation_evaluation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-10 05:48:44.000000 aind_segmentation_evaluation-0.1.9/src/aind_segmentation_evaluation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-10 05:48:44.000000 aind_segmentation_evaluation-0.1.9/src/aind_segmentation_evaluation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 05:48:44.000000 aind_segmentation_evaluation-0.1.9/src/aind_segmentation_evaluation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-10 05:48:44.000000 aind_segmentation_evaluation-0.1.9/src/aind_segmentation_evaluation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-10 05:48:44.000000 aind_segmentation_evaluation-0.1.9/src/aind_segmentation_evaluation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:48:44.601880 aind_segmentation_evaluation-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-10 05:48:21.000000 aind_segmentation_evaluation-0.1.9/tests/unit_tests.py
```

### Comparing `aind_segmentation_evaluation-0.1.8/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_segmentation_evaluation-0.1.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_segmentation_evaluation-0.1.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/.github/ISSUE_TEMPLATE/user-story.md` & `aind_segmentation_evaluation-0.1.9/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/.github/workflows/lint_and_test.yml` & `aind_segmentation_evaluation-0.1.9/.github/workflows/lint_and_test.yml`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/.github/workflows/tag_and_publish.yml` & `aind_segmentation_evaluation-0.1.9/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/.gitignore` & `aind_segmentation_evaluation-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/LICENSE` & `aind_segmentation_evaluation-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/PKG-INFO` & `aind_segmentation_evaluation-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind_segmentation_evaluation
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python package for evaluating neuron segmentations in terms of the number of splits and merges
 Author-email: Anna Grim <anna.grim@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `aind_segmentation_evaluation-0.1.8/README.md` & `aind_segmentation_evaluation-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/demo.py` & `aind_segmentation_evaluation-0.1.9/demo.py`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/doc_template/Makefile` & `aind_segmentation_evaluation-0.1.9/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/doc_template/make.bat` & `aind_segmentation_evaluation-0.1.9/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/doc_template/source/_static/dark-logo.svg` & `aind_segmentation_evaluation-0.1.9/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/doc_template/source/_static/favicon.ico` & `aind_segmentation_evaluation-0.1.9/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/doc_template/source/_static/light-logo.svg` & `aind_segmentation_evaluation-0.1.9/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/doc_template/source/conf.py` & `aind_segmentation_evaluation-0.1.9/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/pyproject.toml` & `aind_segmentation_evaluation-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/resources/merge_edges.tif` & `aind_segmentation_evaluation-0.1.9/resources/merge_edges.tif`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/resources/merge_sites.tif` & `aind_segmentation_evaluation-0.1.9/resources/merge_sites.tif`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/resources/pred_volume.tif` & `aind_segmentation_evaluation-0.1.9/resources/pred_volume.tif`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/resources/split_edges.tif` & `aind_segmentation_evaluation-0.1.9/resources/split_edges.tif`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/resources/split_sites.tif` & `aind_segmentation_evaluation-0.1.9/resources/split_sites.tif`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/resources/target_graphs/0.swc` & `aind_segmentation_evaluation-0.1.9/resources/target_graphs/0.swc`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/resources/target_graphs/1.swc` & `aind_segmentation_evaluation-0.1.9/resources/target_graphs/1.swc`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/resources/target_graphs/2.swc` & `aind_segmentation_evaluation-0.1.9/resources/target_graphs/2.swc`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/resources/target_graphs/3.swc` & `aind_segmentation_evaluation-0.1.9/resources/target_graphs/3.swc`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/resources/target_graphs/4.swc` & `aind_segmentation_evaluation-0.1.9/resources/target_graphs/4.swc`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/resources/target_graphs/5.swc` & `aind_segmentation_evaluation-0.1.9/resources/target_graphs/5.swc`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/resources/target_volume.tif` & `aind_segmentation_evaluation-0.1.9/resources/target_volume.tif`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/src/aind_segmentation_evaluation/evaluate.py` & `aind_segmentation_evaluation-0.1.9/src/aind_segmentation_evaluation/evaluate.py`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/src/aind_segmentation_evaluation/explore_branches.py` & `aind_segmentation_evaluation-0.1.9/src/aind_segmentation_evaluation/explore_branches.py`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/src/aind_segmentation_evaluation/graph_routines.py` & `aind_segmentation_evaluation-0.1.9/src/aind_segmentation_evaluation/graph_routines.py`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/src/aind_segmentation_evaluation/merge_metric.py` & `aind_segmentation_evaluation-0.1.9/src/aind_segmentation_evaluation/merge_metric.py`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/src/aind_segmentation_evaluation/seg_metrics.py` & `aind_segmentation_evaluation-0.1.9/src/aind_segmentation_evaluation/seg_metrics.py`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/src/aind_segmentation_evaluation/split_metric.py` & `aind_segmentation_evaluation-0.1.9/src/aind_segmentation_evaluation/split_metric.py`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/src/aind_segmentation_evaluation/utils.py` & `aind_segmentation_evaluation-0.1.9/src/aind_segmentation_evaluation/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -103,35 +103,56 @@
     if edge_reverse in set_of_edges:
         set_of_edges.remove(edge_reverse)
     elif edge in set_of_edges:
         set_of_edges.remove(edge)
     return set_of_edges
 
 
-def upload_tensorstore_mask(data_dir):
+def clip(arr, clip):
+    """
+    Clips an array.
+
+    Parameters
+    ----------
+    arr : numpy.array
+        Array to be clipped.
+    clip : int
+        Number of rows/columns to be removed from each dimensions.
+
+    Returns
+    -------
+    clipped_arr : numpy.array
+        Clipped array.
+
+    """
+    clipped_arr = arr[clip:-clip, clip:-clip, clip:-clip]
+    return clipped_arr
+
+
+def upload_google_pred(path_to_data):
     """
     Uploads segmentation mask stored as a directory of shard files.
 
     Parameters
     ----------
-    data_dir : str
+    path_to_data : str
         Path to directory containing shard files.
 
     Returns
     -------
     sparse_volume : dict
         Sparse image volume.
 
     """
     dataset_ts = ts.open(
         {
             "driver": "neuroglancer_precomputed",
             "kvstore": {
                 "driver": "file",
-                "path": data_dir,
+                "path": path_to_data,
             },
         }
     ).result()
     dataset_ts = dataset_ts[ts.d[:].transpose[::-1]]
     volume_ts = dataset_ts[ts.d["channel"][0]]
     sparse_volume = dict()
     for x in range(volume_ts.shape[0]):
```

### Comparing `aind_segmentation_evaluation-0.1.8/src/aind_segmentation_evaluation.egg-info/PKG-INFO` & `aind_segmentation_evaluation-0.1.9/src/aind_segmentation_evaluation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-segmentation-evaluation
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python package for evaluating neuron segmentations in terms of the number of splits and merges
 Author-email: Anna Grim <anna.grim@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `aind_segmentation_evaluation-0.1.8/src/aind_segmentation_evaluation.egg-info/SOURCES.txt` & `aind_segmentation_evaluation-0.1.9/src/aind_segmentation_evaluation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aind_segmentation_evaluation-0.1.8/tests/unit_tests.py` & `aind_segmentation_evaluation-0.1.9/tests/unit_tests.py`

 * *Files identical despite different names*

