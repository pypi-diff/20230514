# Comparing `tmp/calapy-0.1.8.tar.gz` & `tmp/calapy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calapy-0.1.8.tar", last modified: Wed Jun 30 15:11:02 2021, max compression
+gzip compressed data, was "calapy-0.1.9.tar", last modified: Tue Jul 20 14:06:53 2021, max compression
```

## Comparing `calapy-0.1.8.tar` & `calapy-0.1.9.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxrwx   0        0        0        0 2021-06-30 15:11:02.144822 calapy-0.1.8/
--rw-rw-rw-   0        0        0     1097 2019-10-24 15:29:18.000000 calapy-0.1.8/LICENSE.txt
--rw-rw-rw-   0        0        0      610 2021-06-30 15:11:02.143497 calapy-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      138 2021-04-18 17:23:58.000000 calapy-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2021-06-30 15:10:55.284373 calapy-0.1.8/calapy/
--rw-rw-rw-   0        0        0     1690 2021-06-30 15:01:34.000000 calapy-0.1.8/calapy/__init__.py
--rw-rw-rw-   0        0        0    29683 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/array.py
--rw-rw-rw-   0        0        0     4999 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/check.py
--rw-rw-rw-   0        0        0     4518 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/clock.py
--rw-rw-rw-   0        0        0    61228 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/combinations.py
--rw-rw-rw-   0        0        0     5654 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/directory.py
--rw-rw-rw-   0        0        0      423 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/download.py
--rw-rw-rw-   0        0        0     5532 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/format.py
--rw-rw-rw-   0        0        0     1374 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/hacks.py
--rw-rw-rw-   0        0        0      417 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/image.py
--rw-rw-rw-   0        0        0     3040 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/maths.py
--rw-rw-rw-   0        0        0    22096 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/mixamo.py
-drwxrwxrwx   0        0        0        0 2021-06-30 15:10:56.249953 calapy-0.1.8/calapy/ml/
--rw-rw-rw-   0        0        0     1093 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/ml/__init__.py
-drwxrwxrwx   0        0        0        0 2021-06-30 15:10:57.000227 calapy-0.1.8/calapy/ml/datasets/
--rw-rw-rw-   0        0        0      124 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/ml/datasets/__init__.py
--rw-rw-rw-   0        0        0    27766 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/ml/datasets/csv.py
--rw-rw-rw-   0        0        0    26998 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/ml/datasets/image.py
--rw-rw-rw-   0        0        0     4051 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/ml/datasets/tools.py
--rw-rw-rw-   0        0        0      470 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/ml/device.py
--rw-rw-rw-   0        0        0     2268 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/ml/features.py
-drwxrwxrwx   0        0        0        0 2021-06-30 15:10:57.361726 calapy-0.1.8/calapy/ml/models/
--rw-rw-rw-   0        0        0      982 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/ml/models/__init__.py
--rw-rw-rw-   0        0        0     5978 2021-06-04 00:10:43.000000 calapy-0.1.8/calapy/ml/models/image.py
--rw-rw-rw-   0        0        0     5207 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/ml/test.py
--rw-rw-rw-   0        0        0     8806 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/ml/train.py
--rw-rw-rw-   0        0        0      310 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/pkl.py
-drwxrwxrwx   0        0        0        0 2021-06-30 15:10:58.917339 calapy-0.1.8/calapy/plot/
--rw-rw-rw-   0        0        0     1105 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/plot/__init__.py
--rw-rw-rw-   0        0        0    53353 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/plot/bars.py
--rw-rw-rw-   0        0        0     2996 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/plot/cmaps.py
--rw-rw-rw-   0        0        0      478 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/plot/colors.py
--rw-rw-rw-   0        0        0    30491 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/plot/heatmaps.py
--rw-rw-rw-   0        0        0       16 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/plot/parameters.py
--rw-rw-rw-   0        0        0    30474 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/plot/points.py
--rw-rw-rw-   0        0        0     1161 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/plot/save.py
-drwxrwxrwx   0        0        0        0 2021-06-30 15:10:59.816457 calapy-0.1.8/calapy/preprocessing/
--rw-rw-rw-   0        0        0     1090 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/preprocessing/__init__.py
--rw-rw-rw-   0        0        0    10025 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/preprocessing/axes_to_variables_table.py
--rw-rw-rw-   0        0        0     5695 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/preprocessing/reorder_trials.py
--rw-rw-rw-   0        0        0    22275 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/preprocessing/reshape.py
--rw-rw-rw-   0        0        0     1968 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/preprocessing/rotate_indexes.py
-drwxrwxrwx   0        0        0        0 2021-06-30 15:11:00.928888 calapy-0.1.8/calapy/preprocessing/variables_table_to_axes/
--rw-rw-rw-   0        0        0      112 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/preprocessing/variables_table_to_axes/__init__.py
--rw-rw-rw-   0        0        0    26245 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/preprocessing/variables_table_to_axes/balanced.py
--rw-rw-rw-   0        0        0    46705 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/preprocessing/variables_table_to_axes/balanced_and_unbalanced.py
--rw-rw-rw-   0        0        0    39022 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/preprocessing/variables_table_to_axes/balanced_or_unbalanced.py
--rw-rw-rw-   0        0        0    35062 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/preprocessing/variables_table_to_axes/unbalanced.py
--rw-rw-rw-   0        0        0      643 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/shutdown.py
-drwxrwxrwx   0        0        0        0 2021-06-30 15:11:01.762888 calapy-0.1.8/calapy/stats/
--rw-rw-rw-   0        0        0     1042 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/stats/__init__.py
--rw-rw-rw-   0        0        0    21779 2021-06-19 13:48:40.000000 calapy-0.1.8/calapy/stats/descriptive.py
--rw-rw-rw-   0        0        0    10669 2021-06-19 13:48:40.000000 calapy-0.1.8/calapy/stats/exclusions.py
--rw-rw-rw-   0        0        0    10687 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/stats/paired_t_test.py
--rw-rw-rw-   0        0        0     9448 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/stats/unpaired_t_test.py
-drwxrwxrwx   0        0        0        0 2021-06-30 15:11:02.132282 calapy-0.1.8/calapy/stimulation/
--rw-rw-rw-   0        0        0      988 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/stimulation/__init__.py
--rw-rw-rw-   0        0        0    27929 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/stimulation/display.py
--rw-rw-rw-   0        0        0     7151 2021-05-21 22:52:16.000000 calapy-0.1.8/calapy/strings.py
--rw-rw-rw-   0        0        0    11732 2021-06-24 12:42:24.000000 calapy-0.1.8/calapy/txt.py
-drwxrwxrwx   0        0        0        0 2021-06-30 15:10:55.384296 calapy-0.1.8/calapy.egg-info/
--rw-rw-rw-   0        0        0      610 2021-06-30 15:10:50.000000 calapy-0.1.8/calapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1613 2021-06-30 15:10:51.000000 calapy-0.1.8/calapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-06-30 15:10:50.000000 calapy-0.1.8/calapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2021-06-30 15:10:50.000000 calapy-0.1.8/calapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2021-06-30 15:10:50.000000 calapy-0.1.8/calapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-06-30 15:11:02.144822 calapy-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1246 2021-06-30 15:02:03.000000 calapy-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-07-20 14:06:53.093288 calapy-0.1.9/
+-rw-rw-rw-   0        0        0     1097 2019-10-24 15:29:18.000000 calapy-0.1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      610 2021-07-20 14:06:53.093288 calapy-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      138 2021-04-18 17:23:58.000000 calapy-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2021-07-20 14:06:52.643277 calapy-0.1.9/calapy/
+-rw-rw-rw-   0        0        0     1690 2021-07-20 14:02:52.000000 calapy-0.1.9/calapy/__init__.py
+-rw-rw-rw-   0        0        0    29683 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/array.py
+-rw-rw-rw-   0        0        0     4999 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/check.py
+-rw-rw-rw-   0        0        0     4518 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/clock.py
+-rw-rw-rw-   0        0        0    61228 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/combinations.py
+-rw-rw-rw-   0        0        0     5654 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/directory.py
+-rw-rw-rw-   0        0        0      423 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/download.py
+-rw-rw-rw-   0        0        0     5532 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/format.py
+-rw-rw-rw-   0        0        0     1374 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/hacks.py
+-rw-rw-rw-   0        0        0      417 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/image.py
+-rw-rw-rw-   0        0        0     3040 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/maths.py
+-rw-rw-rw-   0        0        0    22096 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/mixamo.py
+drwxrwxrwx   0        0        0        0 2021-07-20 14:06:52.753278 calapy-0.1.9/calapy/ml/
+-rw-rw-rw-   0        0        0     1093 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/ml/__init__.py
+drwxrwxrwx   0        0        0        0 2021-07-20 14:06:52.793279 calapy-0.1.9/calapy/ml/datasets/
+-rw-rw-rw-   0        0        0      124 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/ml/datasets/__init__.py
+-rw-rw-rw-   0        0        0    27766 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/ml/datasets/csv.py
+-rw-rw-rw-   0        0        0    26998 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/ml/datasets/image.py
+-rw-rw-rw-   0        0        0     4051 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/ml/datasets/tools.py
+-rw-rw-rw-   0        0        0      470 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/ml/device.py
+-rw-rw-rw-   0        0        0     2268 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/ml/features.py
+drwxrwxrwx   0        0        0        0 2021-07-20 14:06:52.823277 calapy-0.1.9/calapy/ml/models/
+-rw-rw-rw-   0        0        0      982 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/ml/models/__init__.py
+-rw-rw-rw-   0        0        0     6065 2021-07-12 15:44:17.000000 calapy-0.1.9/calapy/ml/models/image.py
+-rw-rw-rw-   0        0        0    12871 2021-07-14 19:58:43.000000 calapy-0.1.9/calapy/ml/test.py
+-rw-rw-rw-   0        0        0     8806 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/ml/train.py
+-rw-rw-rw-   0        0        0      310 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/pkl.py
+drwxrwxrwx   0        0        0        0 2021-07-20 14:06:52.913278 calapy-0.1.9/calapy/plot/
+-rw-rw-rw-   0        0        0     1105 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/plot/__init__.py
+-rw-rw-rw-   0        0        0    53353 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/plot/bars.py
+-rw-rw-rw-   0        0        0     2996 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/plot/cmaps.py
+-rw-rw-rw-   0        0        0      478 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/plot/colors.py
+-rw-rw-rw-   0        0        0    30491 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/plot/heatmaps.py
+-rw-rw-rw-   0        0        0       16 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/plot/parameters.py
+-rw-rw-rw-   0        0        0    30474 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/plot/points.py
+-rw-rw-rw-   0        0        0     1161 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/plot/save.py
+drwxrwxrwx   0        0        0        0 2021-07-20 14:06:52.963287 calapy-0.1.9/calapy/preprocessing/
+-rw-rw-rw-   0        0        0     1090 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0    10025 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/preprocessing/axes_to_variables_table.py
+-rw-rw-rw-   0        0        0     5695 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/preprocessing/reorder_trials.py
+-rw-rw-rw-   0        0        0    22275 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/preprocessing/reshape.py
+-rw-rw-rw-   0        0        0     1968 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/preprocessing/rotate_indexes.py
+drwxrwxrwx   0        0        0        0 2021-07-20 14:06:53.013277 calapy-0.1.9/calapy/preprocessing/variables_table_to_axes/
+-rw-rw-rw-   0        0        0      112 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/preprocessing/variables_table_to_axes/__init__.py
+-rw-rw-rw-   0        0        0    26245 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/preprocessing/variables_table_to_axes/balanced.py
+-rw-rw-rw-   0        0        0    46705 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/preprocessing/variables_table_to_axes/balanced_and_unbalanced.py
+-rw-rw-rw-   0        0        0    39022 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/preprocessing/variables_table_to_axes/balanced_or_unbalanced.py
+-rw-rw-rw-   0        0        0    35062 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/preprocessing/variables_table_to_axes/unbalanced.py
+-rw-rw-rw-   0        0        0      643 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/shutdown.py
+drwxrwxrwx   0        0        0        0 2021-07-20 14:06:53.073280 calapy-0.1.9/calapy/stats/
+-rw-rw-rw-   0        0        0     1042 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/stats/__init__.py
+-rw-rw-rw-   0        0        0    21779 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/stats/descriptive.py
+-rw-rw-rw-   0        0        0    10669 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/stats/exclusions.py
+-rw-rw-rw-   0        0        0    10687 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/stats/paired_t_test.py
+-rw-rw-rw-   0        0        0     9448 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/stats/unpaired_t_test.py
+drwxrwxrwx   0        0        0        0 2021-07-20 14:06:53.093288 calapy-0.1.9/calapy/stimulation/
+-rw-rw-rw-   0        0        0      988 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/stimulation/__init__.py
+-rw-rw-rw-   0        0        0    27929 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/stimulation/display.py
+-rw-rw-rw-   0        0        0     7151 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/strings.py
+-rw-rw-rw-   0        0        0    11732 2021-07-12 13:22:29.000000 calapy-0.1.9/calapy/txt.py
+drwxrwxrwx   0        0        0        0 2021-07-20 14:06:52.683277 calapy-0.1.9/calapy.egg-info/
+-rw-rw-rw-   0        0        0      610 2021-07-20 14:06:52.000000 calapy-0.1.9/calapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1613 2021-07-20 14:06:52.000000 calapy-0.1.9/calapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-07-20 14:06:52.000000 calapy-0.1.9/calapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2021-07-20 14:06:52.000000 calapy-0.1.9/calapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2021-07-20 14:06:52.000000 calapy-0.1.9/calapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-07-20 14:06:53.093288 calapy-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1246 2021-07-12 16:11:01.000000 calapy-0.1.9/setup.py
```

### Comparing `calapy-0.1.8/LICENSE.txt` & `calapy-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/PKG-INFO` & `calapy-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calapy
-Version: 0.1.8
+Version: 0.1.9
 Summary: personal package
 Home-page: https://pypi.org/project/calapy
 Author: Carmelo Calafiore
 Author-email: cc18849@essex.ac.uk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `calapy-0.1.8/calapy/__init__.py` & `calapy-0.1.9/calapy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 
-__release_day__ = 30
-__release_month_num__ = 6
+__release_day__ = 20
+__release_month_num__ = 7
 __release_year__ = 2021
 
 
 __release_date_object__ = datetime.date(__release_year__, __release_month_num__, __release_day__)
 __release_date__ = __release_date_object__.__format__('%d %B %Y')
 __release_month_name__ = __release_date_object__.__format__('%B')
 del datetime
```

### Comparing `calapy-0.1.8/calapy/array.py` & `calapy-0.1.9/calapy/array.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/check.py` & `calapy-0.1.9/calapy/check.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/clock.py` & `calapy-0.1.9/calapy/clock.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/combinations.py` & `calapy-0.1.9/calapy/combinations.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/directory.py` & `calapy-0.1.9/calapy/directory.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/format.py` & `calapy-0.1.9/calapy/format.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/hacks.py` & `calapy-0.1.9/calapy/hacks.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/maths.py` & `calapy-0.1.9/calapy/maths.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/mixamo.py` & `calapy-0.1.9/calapy/mixamo.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/ml/__init__.py` & `calapy-0.1.9/calapy/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/ml/datasets/csv.py` & `calapy-0.1.9/calapy/ml/datasets/csv.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/ml/datasets/image.py` & `calapy-0.1.9/calapy/ml/datasets/image.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/ml/datasets/tools.py` & `calapy-0.1.9/calapy/ml/datasets/tools.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/ml/features.py` & `calapy-0.1.9/calapy/ml/features.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/ml/models/__init__.py` & `calapy-0.1.9/calapy/ml/models/__init__.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/ml/models/image.py` & `calapy-0.1.9/calapy/ml/models/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
             num_ftrs = resnet.fc.in_features
             if softmax:
                 resnet.fc = torch.nn.Sequential(torch.nn.Linear(num_ftrs, K), torch.nn.Softmax())
             else:
                 # Here the size of each output sample is set to K.
                 resnet.fc = torch.nn.Linear(num_ftrs, K)
         if isinstance(pretrained, str):
+            # TODO: what if the model was saved with cuda and is being loaded to cpu?
             state_dict = torch.load(pretrained)
             resnet.load_state_dict(state_dict)
     else:
         resnet = ResNetNoLastLayer(name_resnet)
 
         if isinstance(pretrained, str):
             state_dict = torch.load(pretrained)
```

### Comparing `calapy-0.1.8/calapy/ml/train.py` & `calapy-0.1.9/calapy/ml/train.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/plot/__init__.py` & `calapy-0.1.9/calapy/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/plot/bars.py` & `calapy-0.1.9/calapy/plot/bars.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/plot/cmaps.py` & `calapy-0.1.9/calapy/plot/cmaps.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/plot/heatmaps.py` & `calapy-0.1.9/calapy/plot/heatmaps.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/plot/points.py` & `calapy-0.1.9/calapy/plot/points.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/plot/save.py` & `calapy-0.1.9/calapy/plot/save.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/preprocessing/__init__.py` & `calapy-0.1.9/calapy/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/preprocessing/axes_to_variables_table.py` & `calapy-0.1.9/calapy/preprocessing/axes_to_variables_table.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/preprocessing/reorder_trials.py` & `calapy-0.1.9/calapy/preprocessing/reorder_trials.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/preprocessing/reshape.py` & `calapy-0.1.9/calapy/preprocessing/reshape.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/preprocessing/rotate_indexes.py` & `calapy-0.1.9/calapy/preprocessing/rotate_indexes.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/preprocessing/variables_table_to_axes/balanced.py` & `calapy-0.1.9/calapy/preprocessing/variables_table_to_axes/balanced.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/preprocessing/variables_table_to_axes/balanced_and_unbalanced.py` & `calapy-0.1.9/calapy/preprocessing/variables_table_to_axes/balanced_and_unbalanced.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/preprocessing/variables_table_to_axes/balanced_or_unbalanced.py` & `calapy-0.1.9/calapy/preprocessing/variables_table_to_axes/balanced_or_unbalanced.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/preprocessing/variables_table_to_axes/unbalanced.py` & `calapy-0.1.9/calapy/preprocessing/variables_table_to_axes/unbalanced.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/shutdown.py` & `calapy-0.1.9/calapy/shutdown.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/stats/__init__.py` & `calapy-0.1.9/calapy/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/stats/descriptive.py` & `calapy-0.1.9/calapy/stats/descriptive.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/stats/exclusions.py` & `calapy-0.1.9/calapy/stats/exclusions.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/stats/paired_t_test.py` & `calapy-0.1.9/calapy/stats/paired_t_test.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/stats/unpaired_t_test.py` & `calapy-0.1.9/calapy/stats/unpaired_t_test.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/stimulation/__init__.py` & `calapy-0.1.9/calapy/stimulation/__init__.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/stimulation/display.py` & `calapy-0.1.9/calapy/stimulation/display.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/strings.py` & `calapy-0.1.9/calapy/strings.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy/txt.py` & `calapy-0.1.9/calapy/txt.py`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/calapy.egg-info/PKG-INFO` & `calapy-0.1.9/calapy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calapy
-Version: 0.1.8
+Version: 0.1.9
 Summary: personal package
 Home-page: https://pypi.org/project/calapy
 Author: Carmelo Calafiore
 Author-email: cc18849@essex.ac.uk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `calapy-0.1.8/calapy.egg-info/SOURCES.txt` & `calapy-0.1.9/calapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `calapy-0.1.8/setup.py` & `calapy-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="calapy",
-    version="0.1.8",
+    version="0.1.9",
     author="Carmelo Calafiore",
     author_email="cc18849@essex.ac.uk",
     description="personal package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pypi.org/project/calapy",
     packages=setuptools.find_packages(),
```

