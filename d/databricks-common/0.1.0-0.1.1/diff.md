# Comparing `tmp/databricks_common-0.1.0.tar.gz` & `tmp/databricks_common-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_common-0.1.0.tar", max compression
+gzip compressed data, was "databricks_common-0.1.1.tar", max compression
```

## Comparing `databricks_common-0.1.0.tar` & `databricks_common-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-04-28 04:15:30.515000 databricks_common-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-28 04:15:30.515000 databricks_common-0.1.0/databricks_common/__init__.py
--rw-r--r--   0        0        0    10936 2023-04-28 06:23:10.412114 databricks_common-0.1.0/databricks_common/common.py
--rw-r--r--   0        0        0      195 2023-04-28 06:19:11.070881 databricks_common-0.1.0/databricks_common/main.py
--rw-r--r--   0        0        0      396 2023-04-28 06:13:58.328700 databricks_common-0.1.0/databricks_common/utils/get_spark.py
--rw-r--r--   0        0        0        0 2023-04-28 04:54:58.752421 databricks_common-0.1.0/databricks_common/utils/get_spark_local.py
--rw-r--r--   0        0        0      745 2023-04-28 04:34:36.232896 databricks_common-0.1.0/databricks_common/utils/logger_utils.py
--rw-r--r--   0        0        0      462 2023-04-28 06:18:31.890482 databricks_common-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 databricks_common-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       29 2023-05-14 05:57:38.692660 databricks_common-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-28 04:15:30.515000 databricks_common-0.1.1/databricks_common/__init__.py
+-rw-r--r--   0        0        0    10886 2023-05-14 06:10:06.703054 databricks_common-0.1.1/databricks_common/common.py
+-rw-r--r--   0        0        0      195 2023-04-28 06:19:11.070881 databricks_common-0.1.1/databricks_common/main.py
+-rwxr-xr-x   0        0        0      327 2023-05-14 05:35:02.723163 databricks_common-0.1.1/databricks_common/utils/get_spark.py
+-rw-r--r--   0        0        0        0 2023-04-28 04:54:58.752421 databricks_common-0.1.1/databricks_common/utils/get_spark_local.py
+-rw-r--r--   0        0        0      745 2023-04-28 04:34:36.232896 databricks_common-0.1.1/databricks_common/utils/logger_utils.py
+-rw-r--r--   0        0        0      462 2023-05-14 06:10:28.935713 databricks_common-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      433 1970-01-01 00:00:00.000000 databricks_common-0.1.1/PKG-INFO
```

### Comparing `databricks_common-0.1.0/databricks_common/common.py` & `databricks_common-0.1.1/databricks_common/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 _logger = get_logger()
 
 
 class MetastoreTable:  # TODO: Add tests, add shallow/deep delta clone function
     """
     Class representing a table in the Unity Catalog Metastore. This class is used to reference tables,
-    and perform operations on them. It is not a Spark DataFrame, a PySpark DataFrame, or a Pandas DataFrame.
+    and perform operations on them. It is NOT a DataFrame.
     It offers functionality such as:
     - Checking that the table exists
     - Describing the table
     - Describing the table history
     - Describing the table extended
     - Read the table as a Spark DataFrame
     """
```

### Comparing `databricks_common-0.1.0/databricks_common/utils/logger_utils.py` & `databricks_common-0.1.1/databricks_common/utils/logger_utils.py`

 * *Files identical despite different names*

