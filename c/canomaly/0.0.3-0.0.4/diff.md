# Comparing `tmp/canomaly-0.0.3.tar.gz` & `tmp/canomaly-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canomaly-0.0.3.tar", last modified: Sun May 14 02:12:42 2023, max compression
+gzip compressed data, was "canomaly-0.0.4.tar", last modified: Sun May 14 03:39:15 2023, max compression
```

## Comparing `canomaly-0.0.3.tar` & `canomaly-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 02:12:42.405759 canomaly-0.0.3/
--rw-rw-r--   0 galen     (1000) galen     (1000)    35149 2023-05-13 19:23:41.000000 canomaly-0.0.3/LICENSE
--rw-rw-r--   0 galen     (1000) galen     (1000)      631 2023-05-14 02:12:42.405759 canomaly-0.0.3/PKG-INFO
--rw-rw-r--   0 galen     (1000) galen     (1000)      112 2023-05-13 19:23:41.000000 canomaly-0.0.3/README.md
--rw-rw-r--   0 galen     (1000) galen     (1000)      593 2023-05-14 02:12:01.000000 canomaly-0.0.3/pyproject.toml
--rw-rw-r--   0 galen     (1000) galen     (1000)       83 2023-05-14 02:12:42.405759 canomaly-0.0.3/setup.cfg
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 02:12:42.397759 canomaly-0.0.3/src/
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 02:12:42.397759 canomaly-0.0.3/src/canomaly/
--rw-rw-r--   0 galen     (1000) galen     (1000)        0 2023-05-13 19:24:11.000000 canomaly-0.0.3/src/canomaly/__init__.py
--rw-rw-r--   0 galen     (1000) galen     (1000)     2575 2023-05-14 01:36:21.000000 canomaly-0.0.3/src/canomaly/searchtools.py
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 02:12:42.401759 canomaly-0.0.3/src/canomaly.egg-info/
--rw-rw-r--   0 galen     (1000) galen     (1000)      631 2023-05-14 02:12:42.000000 canomaly-0.0.3/src/canomaly.egg-info/PKG-INFO
--rw-rw-r--   0 galen     (1000) galen     (1000)      305 2023-05-14 02:12:42.000000 canomaly-0.0.3/src/canomaly.egg-info/SOURCES.txt
--rw-rw-r--   0 galen     (1000) galen     (1000)        1 2023-05-14 02:12:42.000000 canomaly-0.0.3/src/canomaly.egg-info/dependency_links.txt
--rw-rw-r--   0 galen     (1000) galen     (1000)       12 2023-05-14 02:12:42.000000 canomaly-0.0.3/src/canomaly.egg-info/requires.txt
--rw-rw-r--   0 galen     (1000) galen     (1000)        9 2023-05-14 02:12:42.000000 canomaly-0.0.3/src/canomaly.egg-info/top_level.txt
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 02:12:42.401759 canomaly-0.0.3/tests/
--rw-rw-r--   0 galen     (1000) galen     (1000)     1204 2023-05-14 01:39:34.000000 canomaly-0.0.3/tests/test_cumulative_regex.py
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 03:39:15.927883 canomaly-0.0.4/
+-rw-rw-r--   0 galen     (1000) galen     (1000)    35149 2023-05-13 19:23:41.000000 canomaly-0.0.4/LICENSE
+-rw-rw-r--   0 galen     (1000) galen     (1000)     2162 2023-05-14 03:39:15.927883 canomaly-0.0.4/PKG-INFO
+-rw-rw-r--   0 galen     (1000) galen     (1000)     1643 2023-05-14 02:43:30.000000 canomaly-0.0.4/README.md
+-rw-rw-r--   0 galen     (1000) galen     (1000)      593 2023-05-14 03:39:01.000000 canomaly-0.0.4/pyproject.toml
+-rw-rw-r--   0 galen     (1000) galen     (1000)       83 2023-05-14 03:39:15.927883 canomaly-0.0.4/setup.cfg
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 03:39:15.919883 canomaly-0.0.4/src/
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 03:39:15.923883 canomaly-0.0.4/src/canomaly/
+-rw-rw-r--   0 galen     (1000) galen     (1000)        0 2023-05-13 19:24:11.000000 canomaly-0.0.4/src/canomaly/__init__.py
+-rw-rw-r--   0 galen     (1000) galen     (1000)     2527 2023-05-14 03:35:38.000000 canomaly-0.0.4/src/canomaly/searchtools.py
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 03:39:15.927883 canomaly-0.0.4/src/canomaly.egg-info/
+-rw-rw-r--   0 galen     (1000) galen     (1000)     2162 2023-05-14 03:39:15.000000 canomaly-0.0.4/src/canomaly.egg-info/PKG-INFO
+-rw-rw-r--   0 galen     (1000) galen     (1000)      305 2023-05-14 03:39:15.000000 canomaly-0.0.4/src/canomaly.egg-info/SOURCES.txt
+-rw-rw-r--   0 galen     (1000) galen     (1000)        1 2023-05-14 03:39:15.000000 canomaly-0.0.4/src/canomaly.egg-info/dependency_links.txt
+-rw-rw-r--   0 galen     (1000) galen     (1000)       12 2023-05-14 03:39:15.000000 canomaly-0.0.4/src/canomaly.egg-info/requires.txt
+-rw-rw-r--   0 galen     (1000) galen     (1000)        9 2023-05-14 03:39:15.000000 canomaly-0.0.4/src/canomaly.egg-info/top_level.txt
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-14 03:39:15.927883 canomaly-0.0.4/tests/
+-rw-rw-r--   0 galen     (1000) galen     (1000)     3365 2023-05-14 03:32:01.000000 canomaly-0.0.4/tests/test_cumulative_regex.py
```

### Comparing `canomaly-0.0.3/LICENSE` & `canomaly-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `canomaly-0.0.3/pyproject.toml` & `canomaly-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "canomaly"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Galen Seilis", email="galen.seilis@seilis.ca" },
 ]
 description = "Detecting cumulative changes in data."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `canomaly-0.0.3/src/canomaly/searchtools.py` & `canomaly-0.0.4/src/canomaly/searchtools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-'''
+"""
 Search for cumulative changes in data.
-'''
+"""
 
 from tdda import rexpy
 import pandas as pd
 
-def _frozenset_target_by_group(df: pd.DataFrame, target: str, group: str) -> pd.DataFrame:
+
+def _frozenset_target_by_group(
+    df: pd.DataFrame, target: str, group: str
+) -> pd.DataFrame:
     """
     Groups the values of the target column in df by the corresponding values of
     the group column and returns a new dataframe with a column containing
     frozensets of the grouped values.
 
     Parameters:
     -----------
@@ -24,17 +27,19 @@
     --------
     pandas.DataFrame
         A new dataframe with a column containing frozensets of the values of
         the target column grouped by the corresponding values of the group
         column.
     """
     # Group target values by corresponding values of group
-    grouped = df.groupby(group)[target]\
-              .apply(lambda x: frozenset(x))\
-              .reset_index(name=target + '_grouped')
+    grouped = (
+        df.groupby(group)[target]
+        .apply(frozenset)
+        .reset_index(name=target + "_grouped")
+    )
     return grouped
 
 
 def cumrexpy(df: pd.DataFrame, target: str, group: str) -> pd.Series:
     """
     Applies a cumulative extraction of regular expressions to the grouped values
     of the target column in a pandas dataframe.
@@ -53,20 +58,18 @@
     pandas.Series
         A new series containing the cumulative extraction of regular
         expressions applied to the values of the target column grouped by the
         corresponding values of the group column.
     """
     df_frozen = _frozenset_target_by_group(df, target, group)
     df_frozen = df_frozen.set_index(group)
-    result = df_frozen[f'{target}_grouped']\
-             .apply(list)\
-             .cumsum()\
-             .apply(rexpy.extract)
+    result = df_frozen[f"{target}_grouped"].apply(list).cumsum().apply(rexpy.extract)
     return result
 
+
 def df_seq_diff(df: pd.DataFrame) -> pd.DataFrame:
     """
     Returns a dataframe with rows that have at least one changed value compared to the previous row.
 
     Parameters:
     -----------
     df : pandas.DataFrame
```

