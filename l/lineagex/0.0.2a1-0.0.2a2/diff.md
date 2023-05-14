# Comparing `tmp/lineagex-0.0.2a1.tar.gz` & `tmp/lineagex-0.0.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lineagex-0.0.2a1.tar", max compression
+gzip compressed data, was "lineagex-0.0.2a2.tar", max compression
```

## Comparing `lineagex-0.0.2a1.tar` & `lineagex-0.0.2a2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       55 2023-05-12 01:58:21.769698 lineagex-0.0.2a1/lineagex/__init__.py
--rw-r--r--   0        0        0    54175 2023-04-22 19:33:20.371862 lineagex-0.0.2a1/lineagex/app.js
--rw-r--r--   0        0        0    34528 2023-05-12 01:56:56.456690 lineagex-0.0.2a1/lineagex/ColumnLineage.py
--rw-r--r--   0        0        0    17230 2023-05-11 22:25:23.093987 lineagex-0.0.2a1/lineagex/ColumnLineageNoConn.py
--rw-r--r--   0        0        0      974 2023-05-12 22:15:42.232574 lineagex-0.0.2a1/lineagex/lineagex.py
--rw-r--r--   0        0        0     2355 2023-05-12 02:16:08.034372 lineagex-0.0.2a1/lineagex/LineageXNoConn.py
--rw-r--r--   0        0        0     9896 2023-05-12 22:15:49.236456 lineagex-0.0.2a1/lineagex/LineageXWithConn.py
--rw-r--r--   0        0        0     6556 2023-05-12 02:16:38.442999 lineagex-0.0.2a1/lineagex/SqlToDict.py
--rw-r--r--   0        0        0     1460 2023-05-08 20:36:59.378380 lineagex-0.0.2a1/lineagex/stack.py
--rw-r--r--   0        0        0     6760 2023-05-11 19:49:20.736279 lineagex-0.0.2a1/lineagex/utils.py
--rw-r--r--   0        0        0  3761177 2023-04-22 19:33:20.645016 lineagex-0.0.2a1/lineagex/vendor.js
--rw-r--r--   0        0        0      449 2023-05-12 23:06:59.162026 lineagex-0.0.2a1/pyproject.toml
--rw-r--r--   0        0        0     3492 2023-05-12 22:58:42.152661 lineagex-0.0.2a1/README.md
--rw-r--r--   0        0        0     4192 1970-01-01 00:00:00.000000 lineagex-0.0.2a1/PKG-INFO
+-rw-r--r--   0        0        0       55 2023-05-12 01:58:21.769698 lineagex-0.0.2a2/lineagex/__init__.py
+-rw-r--r--   0        0        0    54175 2023-04-22 19:33:20.371862 lineagex-0.0.2a2/lineagex/app.js
+-rw-r--r--   0        0        0    34528 2023-05-12 01:56:56.456690 lineagex-0.0.2a2/lineagex/ColumnLineage.py
+-rw-r--r--   0        0        0    17230 2023-05-11 22:25:23.093987 lineagex-0.0.2a2/lineagex/ColumnLineageNoConn.py
+-rw-r--r--   0        0        0     1456 2023-05-14 05:10:00.058421 lineagex-0.0.2a2/lineagex/lineagex.py
+-rw-r--r--   0        0        0     2355 2023-05-12 02:16:08.034372 lineagex-0.0.2a2/lineagex/LineageXNoConn.py
+-rw-r--r--   0        0        0     9896 2023-05-12 22:15:49.236456 lineagex-0.0.2a2/lineagex/LineageXWithConn.py
+-rw-r--r--   0        0        0     6556 2023-05-12 02:16:38.442999 lineagex-0.0.2a2/lineagex/SqlToDict.py
+-rw-r--r--   0        0        0     1460 2023-05-08 20:36:59.378380 lineagex-0.0.2a2/lineagex/stack.py
+-rw-r--r--   0        0        0     6760 2023-05-14 05:18:23.887438 lineagex-0.0.2a2/lineagex/utils.py
+-rw-r--r--   0        0        0  3761177 2023-04-22 19:33:20.645016 lineagex-0.0.2a2/lineagex/vendor.js
+-rw-r--r--   0        0        0      449 2023-05-14 05:46:08.238849 lineagex-0.0.2a2/pyproject.toml
+-rw-r--r--   0        0        0     3957 2023-05-14 05:36:49.891755 lineagex-0.0.2a2/README.md
+-rw-r--r--   0        0        0     4657 1970-01-01 00:00:00.000000 lineagex-0.0.2a2/PKG-INFO
```

### Comparing `lineagex-0.0.2a1/lineagex/app.js` & `lineagex-0.0.2a2/lineagex/app.js`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.2a1/lineagex/ColumnLineage.py` & `lineagex-0.0.2a2/lineagex/ColumnLineage.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.2a1/lineagex/ColumnLineageNoConn.py` & `lineagex-0.0.2a2/lineagex/ColumnLineageNoConn.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.2a1/lineagex/LineageXNoConn.py` & `lineagex-0.0.2a2/lineagex/LineageXNoConn.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.2a1/lineagex/LineageXWithConn.py` & `lineagex-0.0.2a2/lineagex/LineageXWithConn.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.2a1/lineagex/SqlToDict.py` & `lineagex-0.0.2a2/lineagex/SqlToDict.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.2a1/lineagex/stack.py` & `lineagex-0.0.2a2/lineagex/stack.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.2a1/lineagex/utils.py` & `lineagex-0.0.2a2/lineagex/utils.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.2a1/lineagex/vendor.js` & `lineagex-0.0.2a2/lineagex/vendor.js`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.2a1/README.md` & `lineagex-0.0.2a2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -60,26 +60,34 @@
   schema1.table1: {
     tables: [schema1.other_table], 
     columns: {
       column1: [schema1.other_table.columns1, schema1.other_table.columns3], column2: [schema1.other_table.columns2, schema1.other_table.columns3]
     }, 
     table_name: schema1.table1
   }, 
-  schema1.table2: {
+  table2: {
     tables: [schema1.table1], 
     columns: {
       new_column1: [schema1.table1.columns1], new_column2: [schema1.table1.column2]
     }, 
-    table_name: schema1.table2
+    table_name: table2
   }, 
 }
 ```
 
 ## How to Navigate the Webpage
-- Start by clicking the star on the right(search) and input a model name that you want to start with.
+![Alt text](/tests/example.png?raw=true "example")
+- Start by clicking the star on the right(select) and input a model name that you want to start with.
 - It should show a table on the canvas with table names and its columns, by clicking the "explore" button on the top right, it will show all the downstream and upstream tables that are related to the columns.
 - Hovering over a column will highlight its downstream and upstream columns as well.
 - You can navigate through the canvas by clicking "explore" on other tables.
+- The buttons on the right from top to bottom are: 
+  - center the lineage to the middle
+  - zoom out
+  - zoom in
+  - select, to search the targeted table and begin the lineage tracing
+  - expand all columns for all table, CAUTION: this might hinder performance if there are many tables
+  - explore all lineage, this would trace all downstream and upstream tables recursively and all columns are shrunk by default for performance
 
 ## FAQ
 - `"not init data"` in the webpage:
 Possibly due to the content of the JSON in the index.html, please check if it is in valid JSON format, and that all keys are in string format.
```

### Comparing `lineagex-0.0.2a1/PKG-INFO` & `lineagex-0.0.2a2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lineagex
-Version: 0.0.2a1
+Version: 0.0.2a2
 Summary: A column lineage tool
 License: MIT
 Author: zshandy
 Author-email: zshandy@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -80,26 +80,34 @@
   schema1.table1: {
     tables: [schema1.other_table], 
     columns: {
       column1: [schema1.other_table.columns1, schema1.other_table.columns3], column2: [schema1.other_table.columns2, schema1.other_table.columns3]
     }, 
     table_name: schema1.table1
   }, 
-  schema1.table2: {
+  table2: {
     tables: [schema1.table1], 
     columns: {
       new_column1: [schema1.table1.columns1], new_column2: [schema1.table1.column2]
     }, 
-    table_name: schema1.table2
+    table_name: table2
   }, 
 }
 ```
 
 ## How to Navigate the Webpage
-- Start by clicking the star on the right(search) and input a model name that you want to start with.
+![Alt text](/tests/example.png?raw=true "example")
+- Start by clicking the star on the right(select) and input a model name that you want to start with.
 - It should show a table on the canvas with table names and its columns, by clicking the "explore" button on the top right, it will show all the downstream and upstream tables that are related to the columns.
 - Hovering over a column will highlight its downstream and upstream columns as well.
 - You can navigate through the canvas by clicking "explore" on other tables.
+- The buttons on the right from top to bottom are: 
+  - center the lineage to the middle
+  - zoom out
+  - zoom in
+  - select, to search the targeted table and begin the lineage tracing
+  - expand all columns for all table, CAUTION: this might hinder performance if there are many tables
+  - explore all lineage, this would trace all downstream and upstream tables recursively and all columns are shrunk by default for performance
 
 ## FAQ
 - `"not init data"` in the webpage:
 Possibly due to the content of the JSON in the index.html, please check if it is in valid JSON format, and that all keys are in string format.
```

