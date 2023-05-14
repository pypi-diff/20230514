# Comparing `tmp/redisgraph-bulk-loader-0.9.8.tar.gz` & `tmp/redisgraph-bulk-loader-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/redisgraph-bulk-loader-0.9.8.tar", last modified: Tue May  4 20:07:15 2021, max compression
+gzip compressed data, was "dist/redisgraph-bulk-loader-0.9.9.tar", last modified: Wed May  5 18:21:40 2021, max compression
```

## Comparing `redisgraph-bulk-loader-0.9.8.tar` & `redisgraph-bulk-loader-0.9.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 tower-linux  (1000) tower-linux  (1000)        0 2021-05-04 20:07:15.365009 redisgraph-bulk-loader-0.9.8/
--rw-r--r--   0 tower-linux  (1000) tower-linux  (1000)     1518 2020-05-01 17:17:26.000000 redisgraph-bulk-loader-0.9.8/LICENSE
--rw-r--r--   0 tower-linux  (1000) tower-linux  (1000)       40 2020-05-11 14:48:24.000000 redisgraph-bulk-loader-0.9.8/MANIFEST.in
--rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)    17829 2021-05-04 20:07:15.365009 redisgraph-bulk-loader-0.9.8/PKG-INFO
--rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)    15596 2021-02-19 20:46:59.000000 redisgraph-bulk-loader-0.9.8/README.md
-drwxrwxr-x   0 tower-linux  (1000) tower-linux  (1000)        0 2021-05-04 20:07:15.361009 redisgraph-bulk-loader-0.9.8/redisgraph_bulk_loader/
--rw-r--r--   0 tower-linux  (1000) tower-linux  (1000)       33 2020-06-17 19:26:05.000000 redisgraph-bulk-loader-0.9.8/redisgraph_bulk_loader/__init__.py
--rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)     8105 2021-05-04 20:06:41.000000 redisgraph-bulk-loader-0.9.8/redisgraph_bulk_loader/bulk_insert.py
--rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)     6874 2021-05-04 20:06:41.000000 redisgraph-bulk-loader-0.9.8/redisgraph_bulk_loader/bulk_update.py
--rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)     1333 2021-03-02 19:21:26.000000 redisgraph-bulk-loader-0.9.8/redisgraph_bulk_loader/config.py
--rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)    11559 2021-04-23 14:11:23.000000 redisgraph-bulk-loader-0.9.8/redisgraph_bulk_loader/entity_file.py
--rw-r--r--   0 tower-linux  (1000) tower-linux  (1000)      117 2020-06-17 19:26:05.000000 redisgraph-bulk-loader-0.9.8/redisgraph_bulk_loader/exceptions.py
--rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)     4119 2021-04-23 14:11:23.000000 redisgraph-bulk-loader-0.9.8/redisgraph_bulk_loader/label.py
--rw-r--r--   0 tower-linux  (1000) tower-linux  (1000)     2392 2020-06-17 19:26:05.000000 redisgraph-bulk-loader-0.9.8/redisgraph_bulk_loader/query_buffer.py
--rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)     4335 2021-04-23 14:11:23.000000 redisgraph-bulk-loader-0.9.8/redisgraph_bulk_loader/relation_type.py
-drwxrwxr-x   0 tower-linux  (1000) tower-linux  (1000)        0 2021-05-04 20:07:15.365009 redisgraph-bulk-loader-0.9.8/redisgraph_bulk_loader.egg-info/
--rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)    17829 2021-05-04 20:07:15.000000 redisgraph-bulk-loader-0.9.8/redisgraph_bulk_loader.egg-info/PKG-INFO
--rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)      806 2021-05-04 20:07:15.000000 redisgraph-bulk-loader-0.9.8/redisgraph_bulk_loader.egg-info/SOURCES.txt
--rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)        1 2021-05-04 20:07:15.000000 redisgraph-bulk-loader-0.9.8/redisgraph_bulk_loader.egg-info/dependency_links.txt
--rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)      187 2021-05-04 20:07:15.000000 redisgraph-bulk-loader-0.9.8/redisgraph_bulk_loader.egg-info/entry_points.txt
--rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)       25 2021-05-04 20:07:15.000000 redisgraph-bulk-loader-0.9.8/redisgraph_bulk_loader.egg-info/requires.txt
--rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)       28 2021-05-04 20:07:15.000000 redisgraph-bulk-loader-0.9.8/redisgraph_bulk_loader.egg-info/top_level.txt
--rw-r--r--   0 tower-linux  (1000) tower-linux  (1000)       25 2020-05-11 14:48:24.000000 redisgraph-bulk-loader-0.9.8/requirements.txt
--rw-r--r--   0 tower-linux  (1000) tower-linux  (1000)       79 2021-05-04 20:07:15.365009 redisgraph-bulk-loader-0.9.8/setup.cfg
--rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)     1143 2021-05-04 20:06:11.000000 redisgraph-bulk-loader-0.9.8/setup.py
-drwxrwxr-x   0 tower-linux  (1000) tower-linux  (1000)        0 2021-05-04 20:07:15.365009 redisgraph-bulk-loader-0.9.8/test/
--rw-r--r--   0 tower-linux  (1000) tower-linux  (1000)        0 2020-05-11 14:48:24.000000 redisgraph-bulk-loader-0.9.8/test/__init__.py
--rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)    33122 2021-04-23 14:11:25.000000 redisgraph-bulk-loader-0.9.8/test/test_bulk_loader.py
--rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)    14001 2021-02-19 20:46:59.000000 redisgraph-bulk-loader-0.9.8/test/test_bulk_update.py
--rw-r--r--   0 tower-linux  (1000) tower-linux  (1000)     1648 2020-06-17 19:26:05.000000 redisgraph-bulk-loader-0.9.8/test/test_config.py
--rw-r--r--   0 tower-linux  (1000) tower-linux  (1000)     2068 2020-06-17 19:26:05.000000 redisgraph-bulk-loader-0.9.8/test/test_label.py
--rw-r--r--   0 tower-linux  (1000) tower-linux  (1000)     2138 2020-06-17 19:26:05.000000 redisgraph-bulk-loader-0.9.8/test/test_relation_type.py
+drwxrwxr-x   0 tower-linux  (1000) tower-linux  (1000)        0 2021-05-05 18:21:40.263064 redisgraph-bulk-loader-0.9.9/
+-rw-r--r--   0 tower-linux  (1000) tower-linux  (1000)     1518 2020-05-01 17:17:26.000000 redisgraph-bulk-loader-0.9.9/LICENSE
+-rw-r--r--   0 tower-linux  (1000) tower-linux  (1000)       40 2020-05-11 14:48:24.000000 redisgraph-bulk-loader-0.9.9/MANIFEST.in
+-rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)    17829 2021-05-05 18:21:40.263064 redisgraph-bulk-loader-0.9.9/PKG-INFO
+-rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)    15596 2021-02-19 20:46:59.000000 redisgraph-bulk-loader-0.9.9/README.md
+drwxrwxr-x   0 tower-linux  (1000) tower-linux  (1000)        0 2021-05-05 18:21:40.263064 redisgraph-bulk-loader-0.9.9/redisgraph_bulk_loader/
+-rw-r--r--   0 tower-linux  (1000) tower-linux  (1000)       33 2020-06-17 19:26:05.000000 redisgraph-bulk-loader-0.9.9/redisgraph_bulk_loader/__init__.py
+-rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)     8103 2021-05-05 18:18:55.000000 redisgraph-bulk-loader-0.9.9/redisgraph_bulk_loader/bulk_insert.py
+-rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)     6874 2021-05-04 20:06:41.000000 redisgraph-bulk-loader-0.9.9/redisgraph_bulk_loader/bulk_update.py
+-rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)     1333 2021-03-02 19:21:26.000000 redisgraph-bulk-loader-0.9.9/redisgraph_bulk_loader/config.py
+-rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)    11559 2021-04-23 14:11:23.000000 redisgraph-bulk-loader-0.9.9/redisgraph_bulk_loader/entity_file.py
+-rw-r--r--   0 tower-linux  (1000) tower-linux  (1000)      117 2020-06-17 19:26:05.000000 redisgraph-bulk-loader-0.9.9/redisgraph_bulk_loader/exceptions.py
+-rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)     4119 2021-04-23 14:11:23.000000 redisgraph-bulk-loader-0.9.9/redisgraph_bulk_loader/label.py
+-rw-r--r--   0 tower-linux  (1000) tower-linux  (1000)     2392 2020-06-17 19:26:05.000000 redisgraph-bulk-loader-0.9.9/redisgraph_bulk_loader/query_buffer.py
+-rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)     4335 2021-04-23 14:11:23.000000 redisgraph-bulk-loader-0.9.9/redisgraph_bulk_loader/relation_type.py
+drwxrwxr-x   0 tower-linux  (1000) tower-linux  (1000)        0 2021-05-05 18:21:40.263064 redisgraph-bulk-loader-0.9.9/redisgraph_bulk_loader.egg-info/
+-rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)    17829 2021-05-05 18:21:40.000000 redisgraph-bulk-loader-0.9.9/redisgraph_bulk_loader.egg-info/PKG-INFO
+-rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)      806 2021-05-05 18:21:40.000000 redisgraph-bulk-loader-0.9.9/redisgraph_bulk_loader.egg-info/SOURCES.txt
+-rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)        1 2021-05-05 18:21:40.000000 redisgraph-bulk-loader-0.9.9/redisgraph_bulk_loader.egg-info/dependency_links.txt
+-rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)      187 2021-05-05 18:21:40.000000 redisgraph-bulk-loader-0.9.9/redisgraph_bulk_loader.egg-info/entry_points.txt
+-rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)       24 2021-05-05 18:21:40.000000 redisgraph-bulk-loader-0.9.9/redisgraph_bulk_loader.egg-info/requires.txt
+-rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)       28 2021-05-05 18:21:40.000000 redisgraph-bulk-loader-0.9.9/redisgraph_bulk_loader.egg-info/top_level.txt
+-rw-r--r--   0 tower-linux  (1000) tower-linux  (1000)       24 2021-05-05 17:30:07.000000 redisgraph-bulk-loader-0.9.9/requirements.txt
+-rw-r--r--   0 tower-linux  (1000) tower-linux  (1000)       79 2021-05-05 18:21:40.263064 redisgraph-bulk-loader-0.9.9/setup.cfg
+-rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)     1143 2021-05-05 18:21:35.000000 redisgraph-bulk-loader-0.9.9/setup.py
+drwxrwxr-x   0 tower-linux  (1000) tower-linux  (1000)        0 2021-05-05 18:21:40.263064 redisgraph-bulk-loader-0.9.9/test/
+-rw-r--r--   0 tower-linux  (1000) tower-linux  (1000)        0 2020-05-11 14:48:24.000000 redisgraph-bulk-loader-0.9.9/test/__init__.py
+-rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)    33122 2021-04-23 14:11:25.000000 redisgraph-bulk-loader-0.9.9/test/test_bulk_loader.py
+-rw-rw-r--   0 tower-linux  (1000) tower-linux  (1000)    14001 2021-02-19 20:46:59.000000 redisgraph-bulk-loader-0.9.9/test/test_bulk_update.py
+-rw-r--r--   0 tower-linux  (1000) tower-linux  (1000)     1648 2020-06-17 19:26:05.000000 redisgraph-bulk-loader-0.9.9/test/test_config.py
+-rw-r--r--   0 tower-linux  (1000) tower-linux  (1000)     2068 2020-06-17 19:26:05.000000 redisgraph-bulk-loader-0.9.9/test/test_label.py
+-rw-r--r--   0 tower-linux  (1000) tower-linux  (1000)     2138 2020-06-17 19:26:05.000000 redisgraph-bulk-loader-0.9.9/test/test_relation_type.py
```

### Comparing `redisgraph-bulk-loader-0.9.8/LICENSE` & `redisgraph-bulk-loader-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `redisgraph-bulk-loader-0.9.8/PKG-INFO` & `redisgraph-bulk-loader-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redisgraph-bulk-loader
-Version: 0.9.8
+Version: 0.9.9
 Summary: RedisGraph Bulk Import Tool
 Home-page: https://github.com/redisgraph/redisgraph-bulk-loader
 Author: RedisLabs
 Author-email: oss@redislabs.com
 License: UNKNOWN
 Description: [![license](https://img.shields.io/github/license/RedisGraph/redisgraph-bulk-loader.svg)](https://github.com/RedisGraph/redisgraph-bulk-loader)
         [![CircleCI](https://circleci.com/gh/RedisGraph/redisgraph-bulk-loader/tree/master.svg?style=svg)](https://circleci.com/gh/RedisGraph/redisgraph-bulk-loader/tree/master)
```

### Comparing `redisgraph-bulk-loader-0.9.8/README.md` & `redisgraph-bulk-loader-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `redisgraph-bulk-loader-0.9.8/redisgraph_bulk_loader/bulk_insert.py` & `redisgraph-bulk-loader-0.9.9/redisgraph_bulk_loader/bulk_insert.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 @click.option('--enforce-schema', '-d', default=False, is_flag=True, help='Enforce the schema described in CSV header rows')
 @click.option('--skip-invalid-nodes', '-s', default=False, is_flag=True, help='ignore nodes that use previously defined IDs')
 @click.option('--skip-invalid-edges', '-e', default=False, is_flag=True, help='ignore invalid edges, print an error message and continue loading (True), or stop loading after an edge loading failure (False)')
 @click.option('--quote', '-q', default=0, help='the quoting format used in the CSV file. QUOTE_MINIMAL=0,QUOTE_ALL=1,QUOTE_NONNUMERIC=2,QUOTE_NONE=3')
 @click.option('--escapechar', '-x', default='\\', help='the escape char used for the CSV reader (default \\). Use "none" for None.')
 # Buffer size restrictions
 @click.option('--max-token-count', '-c', default=1024, help='max number of processed CSVs to send per query (default 1024)')
-@click.option('--max-buffer-size', '-b', default=2048, help='max buffer size in megabytes (default 2048)')
+@click.option('--max-buffer-size', '-b', default=512, help='max buffer size in megabytes (default 512)')
 @click.option('--max-token-size', '-t', default=500, help='max size of each token in megabytes (default 500, max 512)')
 @click.option('--index', '-i', multiple=True, help='Label:Propery on which to create an index')
 @click.option('--full-text-index', '-f', multiple=True, help='Label:Propery on which to create an full text search index')
 def bulk_insert(graph, host, port, password, user, unix_socket_path, nodes, nodes_with_label, relations, relations_with_type, separator, enforce_schema, skip_invalid_nodes, skip_invalid_edges, escapechar, quote, max_token_count, max_buffer_size, max_token_size, index, full_text_index):
     if sys.version_info[0] < 3:
         raise Exception("Python 3 is required for the RedisGraph bulk loader.")
```

### Comparing `redisgraph-bulk-loader-0.9.8/redisgraph_bulk_loader/bulk_update.py` & `redisgraph-bulk-loader-0.9.9/redisgraph_bulk_loader/bulk_update.py`

 * *Files identical despite different names*

### Comparing `redisgraph-bulk-loader-0.9.8/redisgraph_bulk_loader/config.py` & `redisgraph-bulk-loader-0.9.9/redisgraph_bulk_loader/config.py`

 * *Files identical despite different names*

### Comparing `redisgraph-bulk-loader-0.9.8/redisgraph_bulk_loader/entity_file.py` & `redisgraph-bulk-loader-0.9.9/redisgraph_bulk_loader/entity_file.py`

 * *Files identical despite different names*

### Comparing `redisgraph-bulk-loader-0.9.8/redisgraph_bulk_loader/label.py` & `redisgraph-bulk-loader-0.9.9/redisgraph_bulk_loader/label.py`

 * *Files identical despite different names*

### Comparing `redisgraph-bulk-loader-0.9.8/redisgraph_bulk_loader/query_buffer.py` & `redisgraph-bulk-loader-0.9.9/redisgraph_bulk_loader/query_buffer.py`

 * *Files identical despite different names*

### Comparing `redisgraph-bulk-loader-0.9.8/redisgraph_bulk_loader/relation_type.py` & `redisgraph-bulk-loader-0.9.9/redisgraph_bulk_loader/relation_type.py`

 * *Files identical despite different names*

### Comparing `redisgraph-bulk-loader-0.9.8/redisgraph_bulk_loader.egg-info/PKG-INFO` & `redisgraph-bulk-loader-0.9.9/redisgraph_bulk_loader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redisgraph-bulk-loader
-Version: 0.9.8
+Version: 0.9.9
 Summary: RedisGraph Bulk Import Tool
 Home-page: https://github.com/redisgraph/redisgraph-bulk-loader
 Author: RedisLabs
 Author-email: oss@redislabs.com
 License: UNKNOWN
 Description: [![license](https://img.shields.io/github/license/RedisGraph/redisgraph-bulk-loader.svg)](https://github.com/RedisGraph/redisgraph-bulk-loader)
         [![CircleCI](https://circleci.com/gh/RedisGraph/redisgraph-bulk-loader/tree/master.svg?style=svg)](https://circleci.com/gh/RedisGraph/redisgraph-bulk-loader/tree/master)
```

### Comparing `redisgraph-bulk-loader-0.9.8/redisgraph_bulk_loader.egg-info/SOURCES.txt` & `redisgraph-bulk-loader-0.9.9/redisgraph_bulk_loader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redisgraph-bulk-loader-0.9.8/setup.py` & `redisgraph-bulk-loader-0.9.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 requirements = list(map(str.strip, open("requirements.txt").readlines()))
 
 
 setup(
     name='redisgraph-bulk-loader',
-    version='0.9.8',
+    version='0.9.9',
     description='RedisGraph Bulk Import Tool',
     long_description=read_all("README.md"),
     long_description_content_type='text/markdown',
     url='https://github.com/redisgraph/redisgraph-bulk-loader',
     python_requires='>=3',
     packages=find_packages(),
     install_requires=requirements,
```

### Comparing `redisgraph-bulk-loader-0.9.8/test/test_bulk_loader.py` & `redisgraph-bulk-loader-0.9.9/test/test_bulk_loader.py`

 * *Files identical despite different names*

### Comparing `redisgraph-bulk-loader-0.9.8/test/test_bulk_update.py` & `redisgraph-bulk-loader-0.9.9/test/test_bulk_update.py`

 * *Files identical despite different names*

### Comparing `redisgraph-bulk-loader-0.9.8/test/test_config.py` & `redisgraph-bulk-loader-0.9.9/test/test_config.py`

 * *Files identical despite different names*

### Comparing `redisgraph-bulk-loader-0.9.8/test/test_label.py` & `redisgraph-bulk-loader-0.9.9/test/test_label.py`

 * *Files identical despite different names*

### Comparing `redisgraph-bulk-loader-0.9.8/test/test_relation_type.py` & `redisgraph-bulk-loader-0.9.9/test/test_relation_type.py`

 * *Files identical despite different names*

