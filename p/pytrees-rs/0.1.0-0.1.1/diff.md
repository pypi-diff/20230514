# Comparing `tmp/pytrees-rs-0.1.0.tar.gz` & `tmp/pytrees-rs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrees-rs-0.1.0.tar", last modified: Thu May 11 09:40:20 2023, max compression
+gzip compressed data, was "pytrees-rs-0.1.1.tar", last modified: Sun May 14 15:39:26 2023, max compression
```

## Comparing `pytrees-rs-0.1.0.tar` & `pytrees-rs-0.1.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 haroldks  (1000) users      (984)        0 2023-05-11 09:40:20.737125 pytrees-rs-0.1.0/
--rw-r--r--   0 haroldks  (1000) users      (984)      912 2023-05-11 09:37:53.000000 pytrees-rs-0.1.0/Cargo.toml
--rw-r--r--   0 haroldks  (1000) users      (984)       43 2022-10-20 14:52:44.000000 pytrees-rs-0.1.0/MANIFEST.in
--rw-r--r--   0 haroldks  (1000) users      (984)      113 2023-05-11 09:40:20.737125 pytrees-rs-0.1.0/PKG-INFO
--rw-r--r--   0 haroldks  (1000) users      (984)      761 2023-05-02 15:15:59.000000 pytrees-rs-0.1.0/README.md
--rw-r--r--   0 haroldks  (1000) users      (984)      253 2023-05-11 09:32:28.000000 pytrees-rs-0.1.0/pyproject.toml
-drwxr-xr-x   0 haroldks  (1000) users      (984)        0 2023-05-11 09:40:20.733792 pytrees-rs-0.1.0/pytrees/
--rw-r--r--   0 haroldks  (1000) users      (984)       94 2023-05-11 09:07:49.000000 pytrees-rs-0.1.0/pytrees/__init__.py
--rw-r--r--   0 haroldks  (1000) users      (984)      659 2023-05-11 09:29:37.000000 pytrees-rs-0.1.0/pytrees/enum_params.py
--rw-r--r--   0 haroldks  (1000) users      (984)       92 2023-02-08 13:59:25.000000 pytrees-rs-0.1.0/pytrees/exceptions.py
-drwxr-xr-x   0 haroldks  (1000) users      (984)        0 2023-05-11 09:40:20.733792 pytrees-rs-0.1.0/pytrees/experiments/
--rw-r--r--   0 haroldks  (1000) users      (984)       44 2023-02-08 13:59:25.000000 pytrees-rs-0.1.0/pytrees/experiments/__init__.py
-drwxr-xr-x   0 haroldks  (1000) users      (984)        0 2023-05-11 09:40:20.733792 pytrees-rs-0.1.0/pytrees/experiments/synthetic/
--rw-r--r--   0 haroldks  (1000) users      (984)      107 2023-02-08 13:59:25.000000 pytrees-rs-0.1.0/pytrees/experiments/synthetic/__init__.py
--rw-r--r--   0 haroldks  (1000) users      (984)     2451 2023-02-08 13:59:25.000000 pytrees-rs-0.1.0/pytrees/experiments/synthetic/fake_data.py
--rw-r--r--   0 haroldks  (1000) users      (984)     2799 2023-02-08 13:59:25.000000 pytrees-rs-0.1.0/pytrees/experiments/synthetic/fake_trees.py
--rw-r--r--   0 haroldks  (1000) users      (984)     1176 2023-02-08 13:59:25.000000 pytrees-rs-0.1.0/pytrees/experiments/synthetic/tree_rules.py
-drwxr-xr-x   0 haroldks  (1000) users      (984)        0 2023-05-11 09:40:20.733792 pytrees-rs-0.1.0/pytrees/experiments/utils/
--rw-r--r--   0 haroldks  (1000) users      (984)       45 2023-02-08 13:59:25.000000 pytrees-rs-0.1.0/pytrees/experiments/utils/__init__.py
--rw-r--r--   0 haroldks  (1000) users      (984)    10142 2023-03-30 14:46:03.000000 pytrees-rs-0.1.0/pytrees/experiments/utils/functions.py
--rw-r--r--   0 haroldks  (1000) users      (984)     2354 2023-05-11 08:21:18.000000 pytrees-rs-0.1.0/pytrees/experiments/utils/models.py
-drwxr-xr-x   0 haroldks  (1000) users      (984)        0 2023-05-11 09:40:20.733792 pytrees-rs-0.1.0/pytrees/lgdt/
--rw-r--r--   0 haroldks  (1000) users      (984)       48 2023-02-08 13:59:25.000000 pytrees-rs-0.1.0/pytrees/lgdt/__init__.py
--rw-r--r--   0 haroldks  (1000) users      (984)     1482 2023-05-11 09:29:37.000000 pytrees-rs-0.1.0/pytrees/lgdt/lgdt.py
-drwxr-xr-x   0 haroldks  (1000) users      (984)        0 2023-05-11 09:40:20.733792 pytrees-rs-0.1.0/pytrees/optimal/
--rw-r--r--   0 haroldks  (1000) users      (984)       91 2023-05-02 15:15:59.000000 pytrees-rs-0.1.0/pytrees/optimal/__init__.py
--rw-r--r--   0 haroldks  (1000) users      (984)     1339 2023-05-11 09:22:45.000000 pytrees-rs-0.1.0/pytrees/optimal/dl85.py
--rw-r--r--   0 haroldks  (1000) users      (984)     1481 2023-05-11 09:22:54.000000 pytrees-rs-0.1.0/pytrees/optimal/lds_dl85.py
--rw-r--r--   0 haroldks  (1000) users      (984)     8046 2023-05-11 09:07:49.000000 pytrees-rs-0.1.0/pytrees/predictor.py
-drwxr-xr-x   0 haroldks  (1000) users      (984)        0 2023-05-11 09:40:20.733792 pytrees-rs-0.1.0/pytrees_rs.egg-info/
--rw-r--r--   0 haroldks  (1000) users      (984)      113 2023-05-11 09:40:20.000000 pytrees-rs-0.1.0/pytrees_rs.egg-info/PKG-INFO
--rw-r--r--   0 haroldks  (1000) users      (984)     1836 2023-05-11 09:40:20.000000 pytrees-rs-0.1.0/pytrees_rs.egg-info/SOURCES.txt
--rw-r--r--   0 haroldks  (1000) users      (984)        1 2023-05-11 09:40:20.000000 pytrees-rs-0.1.0/pytrees_rs.egg-info/dependency_links.txt
--rw-r--r--   0 haroldks  (1000) users      (984)        1 2023-05-11 08:43:06.000000 pytrees-rs-0.1.0/pytrees_rs.egg-info/not-zip-safe
--rw-r--r--   0 haroldks  (1000) users      (984)       36 2023-05-11 09:40:20.000000 pytrees-rs-0.1.0/pytrees_rs.egg-info/requires.txt
--rw-r--r--   0 haroldks  (1000) users      (984)        8 2023-05-11 09:40:20.000000 pytrees-rs-0.1.0/pytrees_rs.egg-info/top_level.txt
--rw-r--r--   0 haroldks  (1000) users      (984)       38 2023-05-11 09:40:20.737125 pytrees-rs-0.1.0/setup.cfg
--rw-r--r--   0 haroldks  (1000) users      (984)      317 2023-05-11 09:29:37.000000 pytrees-rs-0.1.0/setup.py
-drwxr-xr-x   0 haroldks  (1000) users      (984)        0 2023-05-11 09:40:20.733792 pytrees-rs-0.1.0/src/
-drwxr-xr-x   0 haroldks  (1000) users      (984)        0 2023-05-11 09:40:20.733792 pytrees-rs-0.1.0/src/algorithms/
--rw-r--r--   0 haroldks  (1000) users      (984)     7309 2023-05-02 15:15:59.000000 pytrees-rs-0.1.0/src/algorithms/algorithm_trait.rs
--rw-r--r--   0 haroldks  (1000) users      (984)    30636 2023-05-02 15:15:59.000000 pytrees-rs-0.1.0/src/algorithms/dl85.rs
-drwxr-xr-x   0 haroldks  (1000) users      (984)        0 2023-05-11 09:40:20.733792 pytrees-rs-0.1.0/src/algorithms/dl85_utils/
--rw-r--r--   0 haroldks  (1000) users      (984)       61 2023-02-23 11:58:46.000000 pytrees-rs-0.1.0/src/algorithms/dl85_utils/mod.rs
--rw-r--r--   0 haroldks  (1000) users      (984)     4837 2023-02-08 13:59:25.000000 pytrees-rs-0.1.0/src/algorithms/dl85_utils/slb.rs
--rw-r--r--   0 haroldks  (1000) users      (984)     5187 2023-05-02 15:15:59.000000 pytrees-rs-0.1.0/src/algorithms/dl85_utils/stop_conditions.rs
--rw-r--r--   0 haroldks  (1000) users      (984)     2543 2023-05-02 15:15:59.000000 pytrees-rs-0.1.0/src/algorithms/dl85_utils/structs_enums.rs
--rw-r--r--   0 haroldks  (1000) users      (984)     4183 2023-02-08 13:59:25.000000 pytrees-rs-0.1.0/src/algorithms/idk.rs
--rw-r--r--   0 haroldks  (1000) users      (984)    13661 2023-05-02 15:15:59.000000 pytrees-rs-0.1.0/src/algorithms/info_gain.rs
--rw-r--r--   0 haroldks  (1000) users      (984)    33997 2023-05-02 15:15:59.000000 pytrees-rs-0.1.0/src/algorithms/lds_dl85.rs
--rw-r--r--   0 haroldks  (1000) users      (984)     7230 2023-05-02 15:15:59.000000 pytrees-rs-0.1.0/src/algorithms/lgdt.rs
--rw-r--r--   0 haroldks  (1000) users      (984)      163 2023-05-02 15:15:59.000000 pytrees-rs-0.1.0/src/algorithms/mod.rs
--rw-r--r--   0 haroldks  (1000) users      (984)   243075 2023-05-02 15:15:59.000000 pytrees-rs-0.1.0/src/algorithms/murtree.rs
--rw-r--r--   0 haroldks  (1000) users      (984)     8582 2023-05-11 08:06:46.000000 pytrees-rs-0.1.0/src/algorithms/parallel_lgdt.rs
-drwxr-xr-x   0 haroldks  (1000) users      (984)        0 2023-05-11 09:40:20.733792 pytrees-rs-0.1.0/src/dataset/
--rw-r--r--   0 haroldks  (1000) users      (984)     6017 2023-02-08 13:59:25.000000 pytrees-rs-0.1.0/src/dataset/binary_dataset.rs
--rw-r--r--   0 haroldks  (1000) users      (984)      819 2023-05-02 15:15:59.000000 pytrees-rs-0.1.0/src/dataset/data_trait.rs
--rw-r--r--   0 haroldks  (1000) users      (984)       47 2022-08-19 11:06:31.000000 pytrees-rs-0.1.0/src/dataset/data_types.rs
--rw-r--r--   0 haroldks  (1000) users      (984)       60 2022-10-10 14:50:43.000000 pytrees-rs-0.1.0/src/dataset/mod.rs
-drwxr-xr-x   0 haroldks  (1000) users      (984)        0 2023-05-11 09:40:20.733792 pytrees-rs-0.1.0/src/heuristics/
--rw-r--r--   0 haroldks  (1000) users      (984)     6731 2023-05-02 15:15:59.000000 pytrees-rs-0.1.0/src/heuristics/mod.rs
--rw-r--r--   0 haroldks  (1000) users      (984)     2307 2023-05-02 15:15:59.000000 pytrees-rs-0.1.0/src/lib.rs
--rw-r--r--   0 haroldks  (1000) users      (984)     1773 2023-05-11 08:06:46.000000 pytrees-rs-0.1.0/src/main.rs
-drwxr-xr-x   0 haroldks  (1000) users      (984)        0 2023-05-11 09:40:20.733792 pytrees-rs-0.1.0/src/post_process/
--rw-r--r--   0 haroldks  (1000) users      (984)     9490 2023-05-02 15:15:59.000000 pytrees-rs-0.1.0/src/post_process/cc_pruning.rs
--rw-r--r--   0 haroldks  (1000) users      (984)       20 2022-10-24 09:50:38.000000 pytrees-rs-0.1.0/src/post_process/mod.rs
-drwxr-xr-x   0 haroldks  (1000) users      (984)        0 2023-05-11 09:40:20.733792 pytrees-rs-0.1.0/src/pycore/
--rw-r--r--   0 haroldks  (1000) users      (984)    10569 2023-05-11 09:29:37.000000 pytrees-rs-0.1.0/src/pycore/less_greedy.rs
--rw-r--r--   0 haroldks  (1000) users      (984)       38 2023-02-08 13:59:25.000000 pytrees-rs-0.1.0/src/pycore/mod.rs
--rw-r--r--   0 haroldks  (1000) users      (984)     6774 2023-05-02 15:15:59.000000 pytrees-rs-0.1.0/src/pycore/optimal.rs
-drwxr-xr-x   0 haroldks  (1000) users      (984)        0 2023-05-11 09:40:20.733792 pytrees-rs-0.1.0/src/structures/
--rw-r--r--   0 haroldks  (1000) users      (984)     9247 2023-02-08 13:59:25.000000 pytrees-rs-0.1.0/src/structures/binary_tree.rs
--rw-r--r--   0 haroldks  (1000) users      (984)    59730 2023-05-02 15:15:59.000000 pytrees-rs-0.1.0/src/structures/bitsets_structure.rs
-drwxr-xr-x   0 haroldks  (1000) users      (984)        0 2023-05-11 09:40:20.733792 pytrees-rs-0.1.0/src/structures/caching/
--rw-r--r--   0 haroldks  (1000) users      (984)       14 2023-02-08 13:59:25.000000 pytrees-rs-0.1.0/src/structures/caching/mod.rs
--rw-r--r--   0 haroldks  (1000) users      (984)     8430 2023-05-02 15:15:59.000000 pytrees-rs-0.1.0/src/structures/caching/trie.rs
--rw-r--r--   0 haroldks  (1000) users      (984)     4475 2023-02-08 13:59:25.000000 pytrees-rs-0.1.0/src/structures/double_pointer.rs
--rw-r--r--   0 haroldks  (1000) users      (984)     8425 2023-02-08 13:59:25.000000 pytrees-rs-0.1.0/src/structures/horizontal_binary_structure.rs
--rw-r--r--   0 haroldks  (1000) users      (984)      252 2023-02-08 13:59:25.000000 pytrees-rs-0.1.0/src/structures/mod.rs
--rw-r--r--   0 haroldks  (1000) users      (984)     6602 2023-02-23 09:17:28.000000 pytrees-rs-0.1.0/src/structures/raw_binary_structure.rs
--rw-r--r--   0 haroldks  (1000) users      (984)    19988 2023-05-02 15:15:59.000000 pytrees-rs-0.1.0/src/structures/reversible_sparse_bitsets_structure.rs
--rw-r--r--   0 haroldks  (1000) users      (984)     1081 2023-05-02 15:15:59.000000 pytrees-rs-0.1.0/src/structures/structure_trait.rs
--rw-r--r--   0 haroldks  (1000) users      (984)     1196 2023-05-02 15:15:59.000000 pytrees-rs-0.1.0/src/structures/structures_types.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:39:26.724733 pytrees-rs-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-14 15:39:26.724733 pytrees-rs-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:39:26.712733 pytrees-rs-0.1.1/pytrees/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/pytrees/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/pytrees/enum_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/pytrees/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:39:26.712733 pytrees-rs-0.1.1/pytrees/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/pytrees/experiments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:39:26.716733 pytrees-rs-0.1.1/pytrees/experiments/synthetic/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/pytrees/experiments/synthetic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/pytrees/experiments/synthetic/fake_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/pytrees/experiments/synthetic/fake_trees.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/pytrees/experiments/synthetic/tree_rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:39:26.716733 pytrees-rs-0.1.1/pytrees/experiments/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/pytrees/experiments/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/pytrees/experiments/utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/pytrees/experiments/utils/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:39:26.716733 pytrees-rs-0.1.1/pytrees/lgdt/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/pytrees/lgdt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/pytrees/lgdt/lgdt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:39:26.716733 pytrees-rs-0.1.1/pytrees/optimal/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/pytrees/optimal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/pytrees/optimal/dl85.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/pytrees/optimal/lds_dl85.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/pytrees/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:39:26.716733 pytrees-rs-0.1.1/pytrees_rs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-14 15:39:26.000000 pytrees-rs-0.1.1/pytrees_rs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-14 15:39:26.000000 pytrees-rs-0.1.1/pytrees_rs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 15:39:26.000000 pytrees-rs-0.1.1/pytrees_rs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 15:39:26.000000 pytrees-rs-0.1.1/pytrees_rs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-14 15:39:26.000000 pytrees-rs-0.1.1/pytrees_rs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-14 15:39:26.000000 pytrees-rs-0.1.1/pytrees_rs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 15:39:26.724733 pytrees-rs-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:39:26.716733 pytrees-rs-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:39:26.720733 pytrees-rs-0.1.1/src/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/algorithms/algorithm_trait.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    30636 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/algorithms/dl85.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:39:26.720733 pytrees-rs-0.1.1/src/algorithms/dl85_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/algorithms/dl85_utils/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/algorithms/dl85_utils/slb.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/algorithms/dl85_utils/stop_conditions.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/algorithms/dl85_utils/structs_enums.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/algorithms/idk.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/algorithms/info_gain.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    33997 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/algorithms/lds_dl85.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/algorithms/lgdt.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/algorithms/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)   243075 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/algorithms/murtree.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/algorithms/parallel_lgdt.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:39:26.720733 pytrees-rs-0.1.1/src/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/dataset/binary_dataset.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/dataset/data_trait.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/dataset/data_types.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/dataset/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:39:26.720733 pytrees-rs-0.1.1/src/heuristics/
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/heuristics/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:39:26.720733 pytrees-rs-0.1.1/src/post_process/
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/post_process/cc_pruning.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/post_process/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:39:26.720733 pytrees-rs-0.1.1/src/pycore/
+-rw-r--r--   0 runner    (1001) docker     (123)    10569 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/pycore/less_greedy.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/pycore/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/pycore/optimal.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:39:26.724733 pytrees-rs-0.1.1/src/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/structures/binary_tree.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    59730 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/structures/bitsets_structure.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:39:26.724733 pytrees-rs-0.1.1/src/structures/caching/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/structures/caching/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/structures/caching/trie.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/structures/double_pointer.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/structures/horizontal_binary_structure.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/structures/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/structures/raw_binary_structure.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    19988 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/structures/reversible_sparse_bitsets_structure.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/structures/structure_trait.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-14 15:39:16.000000 pytrees-rs-0.1.1/src/structures/structures_types.rs
```

### Comparing `pytrees-rs-0.1.0/Cargo.toml` & `pytrees-rs-0.1.1/Cargo.toml`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/README.md` & `pytrees-rs-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/pytrees/enum_params.py` & `pytrees-rs-0.1.1/pytrees/enum_params.py`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/pytrees/experiments/synthetic/fake_data.py` & `pytrees-rs-0.1.1/pytrees/experiments/synthetic/fake_data.py`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/pytrees/experiments/synthetic/fake_trees.py` & `pytrees-rs-0.1.1/pytrees/experiments/synthetic/fake_trees.py`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/pytrees/experiments/synthetic/tree_rules.py` & `pytrees-rs-0.1.1/pytrees/experiments/synthetic/tree_rules.py`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/pytrees/experiments/utils/functions.py` & `pytrees-rs-0.1.1/pytrees/experiments/utils/functions.py`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/pytrees/experiments/utils/models.py` & `pytrees-rs-0.1.1/pytrees/experiments/utils/models.py`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/pytrees/lgdt/lgdt.py` & `pytrees-rs-0.1.1/pytrees/lgdt/lgdt.py`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/pytrees/optimal/dl85.py` & `pytrees-rs-0.1.1/pytrees/optimal/dl85.py`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/pytrees/optimal/lds_dl85.py` & `pytrees-rs-0.1.1/pytrees/optimal/lds_dl85.py`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/pytrees/predictor.py` & `pytrees-rs-0.1.1/pytrees/predictor.py`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/pytrees_rs.egg-info/SOURCES.txt` & `pytrees-rs-0.1.1/pytrees_rs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/src/algorithms/algorithm_trait.rs` & `pytrees-rs-0.1.1/src/algorithms/algorithm_trait.rs`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/src/algorithms/dl85.rs` & `pytrees-rs-0.1.1/src/algorithms/dl85.rs`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/src/algorithms/dl85_utils/slb.rs` & `pytrees-rs-0.1.1/src/algorithms/dl85_utils/slb.rs`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/src/algorithms/dl85_utils/stop_conditions.rs` & `pytrees-rs-0.1.1/src/algorithms/dl85_utils/stop_conditions.rs`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/src/algorithms/dl85_utils/structs_enums.rs` & `pytrees-rs-0.1.1/src/algorithms/dl85_utils/structs_enums.rs`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/src/algorithms/idk.rs` & `pytrees-rs-0.1.1/src/algorithms/idk.rs`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/src/algorithms/info_gain.rs` & `pytrees-rs-0.1.1/src/algorithms/info_gain.rs`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/src/algorithms/lds_dl85.rs` & `pytrees-rs-0.1.1/src/algorithms/lds_dl85.rs`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/src/algorithms/lgdt.rs` & `pytrees-rs-0.1.1/src/algorithms/lgdt.rs`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/src/algorithms/murtree.rs` & `pytrees-rs-0.1.1/src/algorithms/murtree.rs`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/src/algorithms/parallel_lgdt.rs` & `pytrees-rs-0.1.1/src/algorithms/parallel_lgdt.rs`

 * *Files 4% similar despite different names*

```diff
@@ -206,36 +206,36 @@
             if let Some(parent) = tree.get_node_mut(index) {
                 parent.value.error = parent_error;
             }
             parent_error
         };
     }
 }
-
-#[cfg(test)]
-mod parallel_lgdt_test {
-    use crate::algorithms::algorithm_trait::{Algorithm, Basic};
-    use crate::algorithms::dl85_utils::structs_enums::Specialization::Murtree;
-    use crate::algorithms::info_gain::InfoGain;
-    use crate::algorithms::lgdt::LGDT;
-    use crate::algorithms::murtree::MurTree;
-    use crate::algorithms::parallel_lgdt::ParallelLGDT;
-    use crate::dataset::binary_dataset::BinaryDataset;
-    use crate::dataset::data_trait::Dataset;
-    use crate::structures::bitsets_structure::BitsetStructure;
-    use crate::structures::structure_trait::{BitsetTrait, Structure};
-    use rand::Rng;
-
-    #[test]
-    fn test_parrallel_lgdt_murtree_anneal() {
-        let dataset = BinaryDataset::load("test_data/german-credit.txt", false, 0.0);
-        let bitset_data = BitsetStructure::format_input_data(&dataset);
-        let mut structure = BitsetStructure::new(&bitset_data);
-
-        let steps = 1;
-        let expected_errors = [151usize, 137, 119, 108, 99, 90, 71, 55, 48, 41];
-
-        let a = ParallelLGDT::fit(&mut structure, 5, 7, 8, MurTree::fit);
-        println!();
-        a.print();
-    }
-}
+//
+// #[cfg(test)]
+// mod parallel_lgdt_test {
+//     use crate::algorithms::algorithm_trait::{Algorithm, Basic};
+//     use crate::algorithms::dl85_utils::structs_enums::Specialization::Murtree;
+//     use crate::algorithms::info_gain::InfoGain;
+//     use crate::algorithms::lgdt::LGDT;
+//     use crate::algorithms::murtree::MurTree;
+//     use crate::algorithms::parallel_lgdt::ParallelLGDT;
+//     use crate::dataset::binary_dataset::BinaryDataset;
+//     use crate::dataset::data_trait::Dataset;
+//     use crate::structures::bitsets_structure::BitsetStructure;
+//     use crate::structures::structure_trait::{BitsetTrait, Structure};
+//     use rand::Rng;
+//
+//     #[test]
+//     fn test_parrallel_lgdt_murtree_anneal() {
+//         let dataset = BinaryDataset::load("test_data/german-credit.txt", false, 0.0);
+//         let bitset_data = BitsetStructure::format_input_data(&dataset);
+//         let mut structure = BitsetStructure::new(&bitset_data);
+//
+//         let steps = 1;
+//         let expected_errors = [151usize, 137, 119, 108, 99, 90, 71, 55, 48, 41];
+//
+//         let a = ParallelLGDT::fit(&mut structure, 5, 7, 8, MurTree::fit);
+//         println!();
+//         a.print();
+//     }
+// }
```

### Comparing `pytrees-rs-0.1.0/src/dataset/binary_dataset.rs` & `pytrees-rs-0.1.1/src/dataset/binary_dataset.rs`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/src/dataset/data_trait.rs` & `pytrees-rs-0.1.1/src/dataset/data_trait.rs`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/src/heuristics/mod.rs` & `pytrees-rs-0.1.1/src/heuristics/mod.rs`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/src/lib.rs` & `pytrees-rs-0.1.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/src/main.rs` & `pytrees-rs-0.1.1/src/main.rs`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/src/post_process/cc_pruning.rs` & `pytrees-rs-0.1.1/src/post_process/cc_pruning.rs`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/src/pycore/less_greedy.rs` & `pytrees-rs-0.1.1/src/pycore/less_greedy.rs`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/src/pycore/optimal.rs` & `pytrees-rs-0.1.1/src/pycore/optimal.rs`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/src/structures/binary_tree.rs` & `pytrees-rs-0.1.1/src/structures/binary_tree.rs`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/src/structures/bitsets_structure.rs` & `pytrees-rs-0.1.1/src/structures/bitsets_structure.rs`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/src/structures/caching/trie.rs` & `pytrees-rs-0.1.1/src/structures/caching/trie.rs`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/src/structures/double_pointer.rs` & `pytrees-rs-0.1.1/src/structures/double_pointer.rs`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/src/structures/horizontal_binary_structure.rs` & `pytrees-rs-0.1.1/src/structures/horizontal_binary_structure.rs`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/src/structures/raw_binary_structure.rs` & `pytrees-rs-0.1.1/src/structures/raw_binary_structure.rs`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/src/structures/reversible_sparse_bitsets_structure.rs` & `pytrees-rs-0.1.1/src/structures/reversible_sparse_bitsets_structure.rs`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/src/structures/structure_trait.rs` & `pytrees-rs-0.1.1/src/structures/structure_trait.rs`

 * *Files identical despite different names*

### Comparing `pytrees-rs-0.1.0/src/structures/structures_types.rs` & `pytrees-rs-0.1.1/src/structures/structures_types.rs`

 * *Files identical despite different names*

