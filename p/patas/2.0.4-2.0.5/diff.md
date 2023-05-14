# Comparing `tmp/patas-2.0.4.tar.gz` & `tmp/patas-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patas-2.0.4.tar", last modified: Sat May 13 20:45:20 2023, max compression
+gzip compressed data, was "patas-2.0.5.tar", last modified: Sun May 14 13:59:41 2023, max compression
```

## Comparing `patas-2.0.4.tar` & `patas-2.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-13 20:45:20.359359 patas-2.0.4/
--rw-rw-r--   0 diego     (1000) diego     (1000)    13945 2023-05-13 20:45:20.359359 patas-2.0.4/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)    13512 2023-05-13 20:44:01.000000 patas-2.0.4/README.md
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-13 20:45:20.359359 patas-2.0.4/patas/
--rw-rw-r--   0 diego     (1000) diego     (1000)       19 2023-05-08 20:38:56.000000 patas-2.0.4/patas/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)    32279 2023-05-13 20:39:28.000000 patas-2.0.4/patas/argparsers.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      220 2023-05-13 20:45:19.000000 patas-2.0.4/patas/consts.py
--rw-rw-r--   0 diego     (1000) diego     (1000)    16391 2023-05-13 20:39:28.000000 patas-2.0.4/patas/graphics.py
--rw-rw-r--   0 diego     (1000) diego     (1000)    26220 2023-05-11 14:18:45.000000 patas-2.0.4/patas/grid_explorer.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      330 2023-05-06 20:57:54.000000 patas-2.0.4/patas/log.py
--rwxrwxr-x   0 diego     (1000) diego     (1000)     9837 2023-05-13 20:39:28.000000 patas-2.0.4/patas/main.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     7619 2023-05-11 22:04:38.000000 patas-2.0.4/patas/parse.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1005 2023-05-11 22:04:50.000000 patas-2.0.4/patas/query_engine.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     6117 2023-05-11 20:10:23.000000 patas-2.0.4/patas/schemas.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     9283 2023-05-10 13:33:56.000000 patas-2.0.4/patas/utils.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-13 20:45:20.359359 patas-2.0.4/patas.egg-info/
--rw-rw-r--   0 diego     (1000) diego     (1000)    13945 2023-05-13 20:45:20.000000 patas-2.0.4/patas.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      425 2023-05-13 20:45:20.000000 patas-2.0.4/patas.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2023-05-13 20:45:20.000000 patas-2.0.4/patas.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       42 2023-05-13 20:45:20.000000 patas-2.0.4/patas.egg-info/entry_points.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       26 2023-05-13 20:45:20.000000 patas-2.0.4/patas.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       12 2023-05-13 20:45:20.000000 patas-2.0.4/patas.egg-info/top_level.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2023-05-13 20:45:20.359359 patas-2.0.4/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      852 2023-05-10 22:45:33.000000 patas-2.0.4/setup.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-13 20:45:20.359359 patas-2.0.4/tests/
--rw-rw-r--   0 diego     (1000) diego     (1000)       18 2023-05-07 16:31:37.000000 patas-2.0.4/tests/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1420 2023-05-07 16:54:01.000000 patas-2.0.4/tests/test_schemas.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-14 13:59:41.173720 patas-2.0.5/
+-rw-rw-r--   0 diego     (1000) diego     (1000)    13930 2023-05-14 13:59:41.173720 patas-2.0.5/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)    13512 2023-05-13 20:44:01.000000 patas-2.0.5/README.md
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-14 13:59:41.173720 patas-2.0.5/patas/
+-rw-rw-r--   0 diego     (1000) diego     (1000)       19 2023-05-08 20:38:56.000000 patas-2.0.5/patas/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)    32279 2023-05-13 20:39:28.000000 patas-2.0.5/patas/argparsers.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      205 2023-05-14 13:59:35.000000 patas-2.0.5/patas/consts.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)    16391 2023-05-13 20:39:28.000000 patas-2.0.5/patas/graphics.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)    26220 2023-05-11 14:18:45.000000 patas-2.0.5/patas/grid_explorer.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      330 2023-05-06 20:57:54.000000 patas-2.0.5/patas/log.py
+-rwxrwxr-x   0 diego     (1000) diego     (1000)     9837 2023-05-13 20:39:28.000000 patas-2.0.5/patas/main.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     7619 2023-05-11 22:04:38.000000 patas-2.0.5/patas/parse.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1021 2023-05-14 13:58:00.000000 patas-2.0.5/patas/query_engine.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     6117 2023-05-11 20:10:23.000000 patas-2.0.5/patas/schemas.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     9283 2023-05-10 13:33:56.000000 patas-2.0.5/patas/utils.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-14 13:59:41.173720 patas-2.0.5/patas.egg-info/
+-rw-rw-r--   0 diego     (1000) diego     (1000)    13930 2023-05-14 13:59:41.000000 patas-2.0.5/patas.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      425 2023-05-14 13:59:41.000000 patas-2.0.5/patas.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2023-05-14 13:59:41.000000 patas-2.0.5/patas.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       42 2023-05-14 13:59:41.000000 patas-2.0.5/patas.egg-info/entry_points.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       26 2023-05-14 13:59:41.000000 patas-2.0.5/patas.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       12 2023-05-14 13:59:41.000000 patas-2.0.5/patas.egg-info/top_level.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2023-05-14 13:59:41.173720 patas-2.0.5/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      852 2023-05-10 22:45:33.000000 patas-2.0.5/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-14 13:59:41.173720 patas-2.0.5/tests/
+-rw-rw-r--   0 diego     (1000) diego     (1000)       18 2023-05-07 16:31:37.000000 patas-2.0.5/tests/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1420 2023-05-07 16:54:01.000000 patas-2.0.5/tests/test_schemas.py
```

### Comparing `patas-2.0.4/PKG-INFO` & `patas-2.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: patas
-Version: 2.0.4
-Summary: Parallelize any program and aggregate results from stdout.
+Version: 2.0.5
+Summary: Hyperparameter search with a single command
 Home-page: https://github.com/diegofps/patas
 Author: Diego Souza
 Author-email: diegofpsouza+patas@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `patas-2.0.4/README.md` & `patas-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `patas-2.0.4/patas/argparsers.py` & `patas-2.0.5/patas/argparsers.py`

 * *Files identical despite different names*

### Comparing `patas-2.0.4/patas/graphics.py` & `patas-2.0.5/patas/graphics.py`

 * *Files identical despite different names*

### Comparing `patas-2.0.4/patas/grid_explorer.py` & `patas-2.0.5/patas/grid_explorer.py`

 * *Files identical despite different names*

### Comparing `patas-2.0.4/patas/main.py` & `patas-2.0.5/patas/main.py`

 * *Files identical despite different names*

### Comparing `patas-2.0.4/patas/parse.py` & `patas-2.0.5/patas/parse.py`

 * *Files identical despite different names*

### Comparing `patas-2.0.4/patas/query_engine.py` & `patas-2.0.5/patas/query_engine.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     def query(self, query, pretty_print):
         
 
         tables = " ".join(self.tables)
 
         if pretty_print:
-            cmd = f"csvsql -d ',' --query {quote_single(query)} {tables} 2> /dev/null | csvlook"
+            cmd = f"csvsql -d ',' --query {quote_single(query)} {tables} 2> /dev/null | csvlook --no-inference" 
         else:
             cmd = f"csvsql -d ',' --query {quote_single(query)} {tables} 2> /dev/null"
         
         status, _ = run(cmd)
 
         if status != 0:
             abort("Could not call csvkit, is it accessible in $PATH?")
```

### Comparing `patas-2.0.4/patas/schemas.py` & `patas-2.0.5/patas/schemas.py`

 * *Files identical despite different names*

### Comparing `patas-2.0.4/patas/utils.py` & `patas-2.0.5/patas/utils.py`

 * *Files identical despite different names*

### Comparing `patas-2.0.4/patas.egg-info/PKG-INFO` & `patas-2.0.5/patas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: patas
-Version: 2.0.4
-Summary: Parallelize any program and aggregate results from stdout.
+Version: 2.0.5
+Summary: Hyperparameter search with a single command
 Home-page: https://github.com/diegofps/patas
 Author: Diego Souza
 Author-email: diegofpsouza+patas@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `patas-2.0.4/setup.py` & `patas-2.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `patas-2.0.4/tests/test_schemas.py` & `patas-2.0.5/tests/test_schemas.py`

 * *Files identical despite different names*

