# Comparing `tmp/llama_index_sl-0.5.3.tar.gz` & `tmp/llama_index_sl-0.5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_sl-0.5.3.tar", last modified: Sun May 14 18:50:00 2023, max compression
+gzip compressed data, was "llama_index_sl-0.5.3.1.tar", last modified: Sun May 14 19:00:05 2023, max compression
```

## Comparing `llama_index_sl-0.5.3.tar` & `llama_index_sl-0.5.3.1.tar`

### file list

```diff
@@ -1,268 +1,268 @@
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.437888 llama_index_sl-0.5.3/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      493 2023-05-14 18:50:00.437888 llama_index_sl-0.5.3/PKG-INFO
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.385888 llama_index_sl-0.5.3/llama_index/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)        6 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/VERSION
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     4468 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      322 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/async_utils.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.385888 llama_index_sl-0.5.3/llama_index/composability/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      119 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/composability/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      171 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/composability/graph.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      242 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/constants.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.385888 llama_index_sl-0.5.3/llama_index/data_structs/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      373 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/data_structs/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    12377 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/data_structs/data_structs.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    12300 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/data_structs/data_structs_v2.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      264 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/data_structs/node_mapping.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     4669 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/data_structs/node_v2.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2669 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/data_structs/struct_type.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      908 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/data_structs/table.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1032 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/data_structs/table_v2.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     4976 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/docstore.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     5278 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/docstore_v2.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.385888 llama_index_sl-0.5.3/llama_index/embeddings/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       17 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/embeddings/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     7650 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/embeddings/base.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      934 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/embeddings/langchain.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    10103 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/embeddings/openai.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      559 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/embeddings/utils.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.389888 llama_index_sl-0.5.3/llama_index/evaluation/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      118 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/evaluation/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     4409 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/evaluation/base.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      544 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/img_utils.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.389888 llama_index_sl-0.5.3/llama_index/indices/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      542 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    14712 2023-04-14 13:49:41.000000 llama_index_sl-0.5.3/llama_index/indices/base.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.389888 llama_index_sl-0.5.3/llama_index/indices/common/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       17 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/common/__init__.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.389888 llama_index_sl-0.5.3/llama_index/indices/common/struct_store/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       19 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/common/struct_store/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     8107 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/common/struct_store/base.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      776 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/common/struct_store/schema.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2629 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/common/struct_store/sql.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.389888 llama_index_sl-0.5.3/llama_index/indices/common/tree/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       17 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/common/tree/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     7129 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/common/tree/base.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.389888 llama_index_sl-0.5.3/llama_index/indices/composability/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      180 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/composability/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     9125 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/composability/graph.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.389888 llama_index_sl-0.5.3/llama_index/indices/empty/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      113 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/empty/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2163 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/empty/base.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.393888 llama_index_sl-0.5.3/llama_index/indices/keyword_table/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      401 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/keyword_table/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     7060 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/keyword_table/base.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      650 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/keyword_table/rake_base.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      844 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/keyword_table/simple_base.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2264 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/keyword_table/utils.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.393888 llama_index_sl-0.5.3/llama_index/indices/knowledge_graph/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      154 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/knowledge_graph/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     8016 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/knowledge_graph/base.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.393888 llama_index_sl-0.5.3/llama_index/indices/list/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      125 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/list/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3623 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/list/base.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.393888 llama_index_sl-0.5.3/llama_index/indices/postprocessor/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       83 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/postprocessor/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2687 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/postprocessor/node.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     8464 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/prompt_helper.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.393888 llama_index_sl-0.5.3/llama_index/indices/query/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       17 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    14782 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/base.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2581 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/embedding_utils.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.393888 llama_index_sl-0.5.3/llama_index/indices/query/empty/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      142 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/empty/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2178 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/empty/base.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.393888 llama_index_sl-0.5.3/llama_index/indices/query/keyword_table/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      313 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/keyword_table/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     6271 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/keyword_table/query.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.393888 llama_index_sl-0.5.3/llama_index/indices/query/knowledge_graph/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      144 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/knowledge_graph/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     9601 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/knowledge_graph/query.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.397888 llama_index_sl-0.5.3/llama_index/indices/query/list/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      255 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/list/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3095 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/list/embedding_query.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1539 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/list/query.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.397888 llama_index_sl-0.5.3/llama_index/indices/query/query_combiner/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      140 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/query_combiner/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     8753 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/query_combiner/base.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       30 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/query_combiner/prompts.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    12961 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/query_runner.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.397888 llama_index_sl-0.5.3/llama_index/indices/query/query_transform/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      281 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/query_transform/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     9145 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/query_transform/base.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     5920 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/query_transform/prompts.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     4834 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/schema.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.397888 llama_index_sl-0.5.3/llama_index/indices/query/struct_store/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      248 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/struct_store/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     4755 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/struct_store/pandas.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     6674 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/struct_store/sql.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.397888 llama_index_sl-0.5.3/llama_index/indices/query/tree/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      386 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/tree/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     5499 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/tree/embedding_query.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    14258 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/tree/leaf_query.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1798 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/tree/retrieve_query.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2229 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/tree/summarize_query.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.401888 llama_index_sl-0.5.3/llama_index/indices/query/vector_store/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      168 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/vector_store/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3265 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/vector_store/base.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     9429 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/query/vector_store/queries.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3891 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/registry.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.401888 llama_index_sl-0.5.3/llama_index/indices/response/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       17 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/response/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    15119 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/response/builder.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3310 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/service_context.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.401888 llama_index_sl-0.5.3/llama_index/indices/struct_store/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      299 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/struct_store/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2115 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/struct_store/base.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     5765 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/struct_store/container_builder.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2624 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/struct_store/pandas.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     8060 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/struct_store/sql.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.401888 llama_index_sl-0.5.3/llama_index/indices/tree/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      146 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/tree/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     5203 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/tree/base.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     6997 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/tree/inserter.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2005 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/utils.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.401888 llama_index_sl-0.5.3/llama_index/indices/vector_store/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      607 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/vector_store/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    10666 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/vector_store/base.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    25545 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/indices/vector_store/vector_indices.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.401888 llama_index_sl-0.5.3/llama_index/langchain_helpers/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       39 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/langchain_helpers/__init__.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.401888 llama_index_sl-0.5.3/llama_index/langchain_helpers/agents/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      555 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/langchain_helpers/agents/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2924 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/langchain_helpers/agents/agents.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1132 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/langchain_helpers/agents/toolkits.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3001 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/langchain_helpers/agents/tools.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      252 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/langchain_helpers/chain_wrapper.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     7571 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/langchain_helpers/memory_wrapper.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3299 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/langchain_helpers/sql_wrapper.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    17458 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/langchain_helpers/text_splitter.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.405888 llama_index_sl-0.5.3/llama_index/llm_predictor/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      254 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/llm_predictor/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    10593 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/llm_predictor/base.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     4275 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/llm_predictor/chatgpt.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2274 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/llm_predictor/structured.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.405888 llama_index_sl-0.5.3/llama_index/logger/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       95 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/logger/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      995 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/logger/base.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.405888 llama_index_sl-0.5.3/llama_index/node_parser/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      113 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/node_parser/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      407 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/node_parser/interface.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3108 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/node_parser/node_utils.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1127 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/node_parser/simple.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.409888 llama_index_sl-0.5.3/llama_index/optimization/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      144 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/optimization/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     4248 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/optimization/optimizer.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.409888 llama_index_sl-0.5.3/llama_index/output_parsers/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      230 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/output_parsers/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      611 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/output_parsers/base.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2742 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/output_parsers/guardrails.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1828 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/output_parsers/langchain.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.413888 llama_index_sl-0.5.3/llama_index/playground/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      202 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/playground/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     5637 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/playground/base.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.417888 llama_index_sl-0.5.3/llama_index/prompts/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       87 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/prompts/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     6626 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/prompts/base.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1969 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/prompts/chat_prompts.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1134 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/prompts/default_prompt_selectors.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    10843 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/prompts/default_prompts.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      992 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/prompts/prompt_type.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     7685 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/prompts/prompts.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.425888 llama_index_sl-0.5.3/llama_index/readers/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2749 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      659 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/base.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.425888 llama_index_sl-0.5.3/llama_index/readers/chatgpt_plugin/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      145 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/chatgpt_plugin/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2111 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/chatgpt_plugin/base.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3895 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/chroma.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3328 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/database.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     4981 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/discord_reader.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     7413 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/download.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2392 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/elasticsearch.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2478 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/faiss.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.429888 llama_index_sl-0.5.3/llama_index/readers/file/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       19 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/file/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     8436 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/file/base.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1342 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/file/base_parser.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2315 2023-04-14 13:57:02.000000 llama_index_sl-0.5.3/llama_index/readers/file/docs_parser.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1318 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/file/epub_parser.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     4106 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/file/image_parser.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3616 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/file/markdown_parser.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3162 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/file/mbox_parser.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3945 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/file/slides_parser.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3357 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/file/tabular_parser.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1770 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/file/video_audio.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.429888 llama_index_sl-0.5.3/llama_index/readers/github_readers/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       17 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/github_readers/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    11686 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/github_readers/github_api_client.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    15928 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/github_readers/github_repository_reader.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     5473 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/github_readers/utils.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.429888 llama_index_sl-0.5.3/llama_index/readers/google_readers/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       17 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/google_readers/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     5659 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/google_readers/gdocs.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     4989 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/google_readers/gsheets.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3708 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/json.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.429888 llama_index_sl-0.5.3/llama_index/readers/llamahub_modules/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/llamahub_modules/__init__.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.429888 llama_index_sl-0.5.3/llama_index/readers/make_com/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       19 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/make_com/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1696 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/make_com/wrapper.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1261 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/mbox.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2260 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/mongo.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     5679 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/notion.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1601 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/obsidian.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2766 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/pinecone.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3279 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/qdrant.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.429888 llama_index_sl-0.5.3/llama_index/readers/schema/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       17 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/schema/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1214 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/schema/base.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     7060 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/slack.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.433888 llama_index_sl-0.5.3/llama_index/readers/steamship/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       17 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/steamship/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3498 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/steamship/file_reader.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      984 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/string_iterable.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1918 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/twitter.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.433888 llama_index_sl-0.5.3/llama_index/readers/weaviate/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       17 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/weaviate/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     8666 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/weaviate/data_structs.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3986 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/weaviate/reader.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1867 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/weaviate/utils.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     7987 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/web.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      981 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/wikipedia.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1255 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/readers/youtube_transcript.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.433888 llama_index_sl-0.5.3/llama_index/response/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       19 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/response/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2039 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/response/notebook_utils.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3126 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/response/schema.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      262 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/response/utils.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2768 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/schema.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.433888 llama_index_sl-0.5.3/llama_index/token_counter/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       17 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/token_counter/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     4664 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/token_counter/mock_chain_wrapper.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      722 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/token_counter/mock_embed_model.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2874 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/token_counter/token_counter.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      908 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/token_counter/utils.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.433888 llama_index_sl-0.5.3/llama_index/tools/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       13 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/tools/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      723 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/tools/file_utils.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    11192 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/tools/migrate_v1_to_v2.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     5296 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/utils.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.437888 llama_index_sl-0.5.3/llama_index/vector_stores/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      859 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/vector_stores/__init__.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     5218 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/vector_stores/chatgpt_plugin.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     4170 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/vector_stores/chroma.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3925 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/vector_stores/faiss.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     6665 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/vector_stores/opensearch.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     7112 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/vector_stores/pinecone.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     6903 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/vector_stores/qdrant.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3521 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/vector_stores/simple.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1469 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/vector_stores/types.py
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3776 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3/llama_index/vector_stores/weaviate.py
-drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 18:50:00.437888 llama_index_sl-0.5.3/llama_index_sl.egg-info/
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      493 2023-05-14 18:50:00.000000 llama_index_sl-0.5.3/llama_index_sl.egg-info/PKG-INFO
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     8326 2023-05-14 18:50:00.000000 llama_index_sl-0.5.3/llama_index_sl.egg-info/SOURCES.txt
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)        1 2023-05-14 18:50:00.000000 llama_index_sl-0.5.3/llama_index_sl.egg-info/dependency_links.txt
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)        9 2023-05-14 18:50:00.000000 llama_index_sl-0.5.3/llama_index_sl.egg-info/requires.txt
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       12 2023-05-14 18:50:00.000000 llama_index_sl-0.5.3/llama_index_sl.egg-info/top_level.txt
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       38 2023-05-14 18:50:00.437888 llama_index_sl-0.5.3/setup.cfg
--rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      674 2023-05-14 18:49:10.000000 llama_index_sl-0.5.3/setup.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.212334 llama_index_sl-0.5.3.1/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      495 2023-05-14 19:00:05.212334 llama_index_sl-0.5.3.1/PKG-INFO
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.160389 llama_index_sl-0.5.3.1/llama_index/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)        7 2023-05-14 18:59:53.000000 llama_index_sl-0.5.3.1/llama_index/VERSION
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     4468 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      322 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/async_utils.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.160389 llama_index_sl-0.5.3.1/llama_index/composability/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      119 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/composability/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      171 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/composability/graph.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      242 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/constants.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.164385 llama_index_sl-0.5.3.1/llama_index/data_structs/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      373 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/data_structs/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    12377 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/data_structs/data_structs.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    12300 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/data_structs/data_structs_v2.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      264 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/data_structs/node_mapping.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     4669 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/data_structs/node_v2.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2669 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/data_structs/struct_type.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      908 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/data_structs/table.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1032 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/data_structs/table_v2.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     4976 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/docstore.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     5278 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/docstore_v2.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.164385 llama_index_sl-0.5.3.1/llama_index/embeddings/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       17 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/embeddings/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     7650 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/embeddings/base.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      934 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/embeddings/langchain.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    10103 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/embeddings/openai.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      559 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/embeddings/utils.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.164385 llama_index_sl-0.5.3.1/llama_index/evaluation/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      118 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/evaluation/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     4409 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/evaluation/base.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      544 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/img_utils.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.164385 llama_index_sl-0.5.3.1/llama_index/indices/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      542 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    14712 2023-04-14 13:49:41.000000 llama_index_sl-0.5.3.1/llama_index/indices/base.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.164385 llama_index_sl-0.5.3.1/llama_index/indices/common/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       17 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/common/__init__.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.168381 llama_index_sl-0.5.3.1/llama_index/indices/common/struct_store/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       19 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/common/struct_store/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     8107 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/common/struct_store/base.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      776 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/common/struct_store/schema.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2629 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/common/struct_store/sql.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.168381 llama_index_sl-0.5.3.1/llama_index/indices/common/tree/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       17 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/common/tree/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     7129 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/common/tree/base.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.168381 llama_index_sl-0.5.3.1/llama_index/indices/composability/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      180 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/composability/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     9125 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/composability/graph.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.168381 llama_index_sl-0.5.3.1/llama_index/indices/empty/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      113 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/empty/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2163 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/empty/base.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.168381 llama_index_sl-0.5.3.1/llama_index/indices/keyword_table/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      401 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/keyword_table/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     7060 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/keyword_table/base.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      650 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/keyword_table/rake_base.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      844 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/keyword_table/simple_base.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2264 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/keyword_table/utils.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.168381 llama_index_sl-0.5.3.1/llama_index/indices/knowledge_graph/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      154 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/knowledge_graph/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     8016 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/knowledge_graph/base.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.172376 llama_index_sl-0.5.3.1/llama_index/indices/list/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      125 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/list/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3623 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/list/base.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.172376 llama_index_sl-0.5.3.1/llama_index/indices/postprocessor/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       83 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/postprocessor/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2687 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/postprocessor/node.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     8464 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/prompt_helper.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.172376 llama_index_sl-0.5.3.1/llama_index/indices/query/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       17 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    14782 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/base.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2581 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/embedding_utils.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.172376 llama_index_sl-0.5.3.1/llama_index/indices/query/empty/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      142 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/empty/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2178 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/empty/base.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.172376 llama_index_sl-0.5.3.1/llama_index/indices/query/keyword_table/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      313 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/keyword_table/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     6271 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/keyword_table/query.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.172376 llama_index_sl-0.5.3.1/llama_index/indices/query/knowledge_graph/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      144 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/knowledge_graph/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     9601 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/knowledge_graph/query.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.176372 llama_index_sl-0.5.3.1/llama_index/indices/query/list/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      255 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/list/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3095 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/list/embedding_query.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1539 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/list/query.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.176372 llama_index_sl-0.5.3.1/llama_index/indices/query/query_combiner/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      140 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/query_combiner/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     8753 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/query_combiner/base.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       30 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/query_combiner/prompts.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    12961 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/query_runner.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.176372 llama_index_sl-0.5.3.1/llama_index/indices/query/query_transform/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      281 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/query_transform/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     9145 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/query_transform/base.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     5920 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/query_transform/prompts.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     4834 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/schema.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.176372 llama_index_sl-0.5.3.1/llama_index/indices/query/struct_store/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      248 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/struct_store/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     4755 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/struct_store/pandas.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     6674 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/struct_store/sql.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.176372 llama_index_sl-0.5.3.1/llama_index/indices/query/tree/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      386 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/tree/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     5499 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/tree/embedding_query.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    14258 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/tree/leaf_query.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1798 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/tree/retrieve_query.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2229 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/tree/summarize_query.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.180368 llama_index_sl-0.5.3.1/llama_index/indices/query/vector_store/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      168 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/vector_store/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3265 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/vector_store/base.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     9429 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/query/vector_store/queries.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3891 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/registry.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.180368 llama_index_sl-0.5.3.1/llama_index/indices/response/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       17 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/response/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    15119 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/response/builder.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3310 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/service_context.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.180368 llama_index_sl-0.5.3.1/llama_index/indices/struct_store/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      299 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/struct_store/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2115 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/struct_store/base.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     5765 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/struct_store/container_builder.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2624 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/struct_store/pandas.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     8060 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/struct_store/sql.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.180368 llama_index_sl-0.5.3.1/llama_index/indices/tree/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      146 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/tree/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     5203 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/tree/base.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     6997 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/tree/inserter.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2005 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/utils.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.180368 llama_index_sl-0.5.3.1/llama_index/indices/vector_store/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      607 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/vector_store/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    10666 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/vector_store/base.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    25545 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/indices/vector_store/vector_indices.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.184364 llama_index_sl-0.5.3.1/llama_index/langchain_helpers/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       39 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/langchain_helpers/__init__.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.184364 llama_index_sl-0.5.3.1/llama_index/langchain_helpers/agents/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      555 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/langchain_helpers/agents/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2924 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/langchain_helpers/agents/agents.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1132 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/langchain_helpers/agents/toolkits.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3001 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/langchain_helpers/agents/tools.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      252 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/langchain_helpers/chain_wrapper.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     7571 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/langchain_helpers/memory_wrapper.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3299 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/langchain_helpers/sql_wrapper.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    17458 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/langchain_helpers/text_splitter.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.184364 llama_index_sl-0.5.3.1/llama_index/llm_predictor/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      254 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/llm_predictor/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    10599 2023-05-14 18:57:13.000000 llama_index_sl-0.5.3.1/llama_index/llm_predictor/base.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     4275 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/llm_predictor/chatgpt.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2274 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/llm_predictor/structured.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.184364 llama_index_sl-0.5.3.1/llama_index/logger/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       95 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/logger/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      995 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/logger/base.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.184364 llama_index_sl-0.5.3.1/llama_index/node_parser/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      113 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/node_parser/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      407 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/node_parser/interface.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3108 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/node_parser/node_utils.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1127 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/node_parser/simple.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.188360 llama_index_sl-0.5.3.1/llama_index/optimization/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      144 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/optimization/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     4248 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/optimization/optimizer.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.188360 llama_index_sl-0.5.3.1/llama_index/output_parsers/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      230 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/output_parsers/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      611 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/output_parsers/base.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2742 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/output_parsers/guardrails.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1828 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/output_parsers/langchain.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.188360 llama_index_sl-0.5.3.1/llama_index/playground/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      202 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/playground/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     5637 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/playground/base.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.188360 llama_index_sl-0.5.3.1/llama_index/prompts/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       87 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/prompts/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     6632 2023-05-14 18:58:06.000000 llama_index_sl-0.5.3.1/llama_index/prompts/base.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1969 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/prompts/chat_prompts.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1134 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/prompts/default_prompt_selectors.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    10843 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/prompts/default_prompts.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      992 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/prompts/prompt_type.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     7685 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/prompts/prompts.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.196351 llama_index_sl-0.5.3.1/llama_index/readers/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2749 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      659 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/base.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.196351 llama_index_sl-0.5.3.1/llama_index/readers/chatgpt_plugin/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      145 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/chatgpt_plugin/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2111 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/chatgpt_plugin/base.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3895 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/chroma.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3328 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/database.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     4981 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/discord_reader.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     7413 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/download.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2392 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/elasticsearch.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2478 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/faiss.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.196351 llama_index_sl-0.5.3.1/llama_index/readers/file/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       19 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/file/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     8436 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/file/base.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1342 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/file/base_parser.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2315 2023-04-14 13:57:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/file/docs_parser.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1318 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/file/epub_parser.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     4106 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/file/image_parser.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3616 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/file/markdown_parser.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3162 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/file/mbox_parser.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3945 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/file/slides_parser.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3357 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/file/tabular_parser.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1770 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/file/video_audio.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.200347 llama_index_sl-0.5.3.1/llama_index/readers/github_readers/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       17 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/github_readers/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    11686 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/github_readers/github_api_client.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    15928 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/github_readers/github_repository_reader.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     5473 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/github_readers/utils.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.200347 llama_index_sl-0.5.3.1/llama_index/readers/google_readers/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       17 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/google_readers/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     5659 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/google_readers/gdocs.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     4989 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/google_readers/gsheets.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3708 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/json.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.200347 llama_index_sl-0.5.3.1/llama_index/readers/llamahub_modules/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/llamahub_modules/__init__.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.200347 llama_index_sl-0.5.3.1/llama_index/readers/make_com/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       19 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/make_com/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1696 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/make_com/wrapper.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1261 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/mbox.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2260 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/mongo.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     5679 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/notion.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1601 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/obsidian.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2766 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/pinecone.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3279 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/qdrant.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.200347 llama_index_sl-0.5.3.1/llama_index/readers/schema/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       17 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/schema/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1214 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/schema/base.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     7060 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/slack.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.200347 llama_index_sl-0.5.3.1/llama_index/readers/steamship/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       17 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/steamship/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3498 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/steamship/file_reader.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      984 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/string_iterable.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1918 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/twitter.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.204343 llama_index_sl-0.5.3.1/llama_index/readers/weaviate/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       17 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/weaviate/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     8666 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/weaviate/data_structs.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3986 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/weaviate/reader.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1867 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/weaviate/utils.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     7987 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/web.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      981 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/wikipedia.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1255 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/readers/youtube_transcript.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.204343 llama_index_sl-0.5.3.1/llama_index/response/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       19 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/response/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2039 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/response/notebook_utils.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3126 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/response/schema.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      262 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/response/utils.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2768 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/schema.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.204343 llama_index_sl-0.5.3.1/llama_index/token_counter/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       17 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/token_counter/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     4664 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/token_counter/mock_chain_wrapper.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      722 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/token_counter/mock_embed_model.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     2874 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/token_counter/token_counter.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      908 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/token_counter/utils.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.208339 llama_index_sl-0.5.3.1/llama_index/tools/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       13 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/tools/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      723 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/tools/file_utils.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)    11192 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/tools/migrate_v1_to_v2.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     5296 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/utils.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.208339 llama_index_sl-0.5.3.1/llama_index/vector_stores/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      859 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/vector_stores/__init__.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     5218 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/vector_stores/chatgpt_plugin.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     4170 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/vector_stores/chroma.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3925 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/vector_stores/faiss.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     6665 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/vector_stores/opensearch.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     7112 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/vector_stores/pinecone.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     6903 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/vector_stores/qdrant.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3521 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/vector_stores/simple.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     1469 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/vector_stores/types.py
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     3776 2023-03-31 18:47:02.000000 llama_index_sl-0.5.3.1/llama_index/vector_stores/weaviate.py
+drwxrwxr-x   0 ahmedemad  (1000) ahmedemad  (1000)        0 2023-05-14 19:00:05.208339 llama_index_sl-0.5.3.1/llama_index_sl.egg-info/
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      495 2023-05-14 19:00:05.000000 llama_index_sl-0.5.3.1/llama_index_sl.egg-info/PKG-INFO
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)     8326 2023-05-14 19:00:05.000000 llama_index_sl-0.5.3.1/llama_index_sl.egg-info/SOURCES.txt
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)        1 2023-05-14 19:00:05.000000 llama_index_sl-0.5.3.1/llama_index_sl.egg-info/dependency_links.txt
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)        9 2023-05-14 19:00:05.000000 llama_index_sl-0.5.3.1/llama_index_sl.egg-info/requires.txt
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       12 2023-05-14 19:00:05.000000 llama_index_sl-0.5.3.1/llama_index_sl.egg-info/top_level.txt
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)       38 2023-05-14 19:00:05.212334 llama_index_sl-0.5.3.1/setup.cfg
+-rw-rw-r--   0 ahmedemad  (1000) ahmedemad  (1000)      676 2023-05-14 18:59:49.000000 llama_index_sl-0.5.3.1/setup.py
```

### Comparing `llama_index_sl-0.5.3/llama_index/__init__.py` & `llama_index_sl-0.5.3.1/llama_index/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/data_structs/data_structs.py` & `llama_index_sl-0.5.3.1/llama_index/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/data_structs/data_structs_v2.py` & `llama_index_sl-0.5.3.1/llama_index/data_structs/data_structs_v2.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/data_structs/node_v2.py` & `llama_index_sl-0.5.3.1/llama_index/data_structs/node_v2.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/data_structs/struct_type.py` & `llama_index_sl-0.5.3.1/llama_index/data_structs/struct_type.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/data_structs/table.py` & `llama_index_sl-0.5.3.1/llama_index/data_structs/table.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/data_structs/table_v2.py` & `llama_index_sl-0.5.3.1/llama_index/data_structs/table_v2.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/docstore.py` & `llama_index_sl-0.5.3.1/llama_index/docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/docstore_v2.py` & `llama_index_sl-0.5.3.1/llama_index/docstore_v2.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/embeddings/base.py` & `llama_index_sl-0.5.3.1/llama_index/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/embeddings/langchain.py` & `llama_index_sl-0.5.3.1/llama_index/embeddings/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/embeddings/openai.py` & `llama_index_sl-0.5.3.1/llama_index/embeddings/openai.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/embeddings/utils.py` & `llama_index_sl-0.5.3.1/llama_index/embeddings/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/evaluation/base.py` & `llama_index_sl-0.5.3.1/llama_index/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/img_utils.py` & `llama_index_sl-0.5.3.1/llama_index/img_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/__init__.py` & `llama_index_sl-0.5.3.1/llama_index/indices/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/base.py` & `llama_index_sl-0.5.3.1/llama_index/indices/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/common/struct_store/base.py` & `llama_index_sl-0.5.3.1/llama_index/indices/common/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/common/struct_store/schema.py` & `llama_index_sl-0.5.3.1/llama_index/indices/common/struct_store/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/common/struct_store/sql.py` & `llama_index_sl-0.5.3.1/llama_index/indices/common/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/common/tree/base.py` & `llama_index_sl-0.5.3.1/llama_index/indices/common/tree/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/composability/graph.py` & `llama_index_sl-0.5.3.1/llama_index/indices/composability/graph.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/empty/base.py` & `llama_index_sl-0.5.3.1/llama_index/indices/empty/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/keyword_table/base.py` & `llama_index_sl-0.5.3.1/llama_index/indices/keyword_table/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/keyword_table/rake_base.py` & `llama_index_sl-0.5.3.1/llama_index/indices/keyword_table/rake_base.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/keyword_table/simple_base.py` & `llama_index_sl-0.5.3.1/llama_index/indices/keyword_table/simple_base.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/keyword_table/utils.py` & `llama_index_sl-0.5.3.1/llama_index/indices/keyword_table/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/knowledge_graph/base.py` & `llama_index_sl-0.5.3.1/llama_index/indices/knowledge_graph/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/list/base.py` & `llama_index_sl-0.5.3.1/llama_index/indices/list/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/postprocessor/node.py` & `llama_index_sl-0.5.3.1/llama_index/indices/postprocessor/node.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/prompt_helper.py` & `llama_index_sl-0.5.3.1/llama_index/indices/prompt_helper.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/query/base.py` & `llama_index_sl-0.5.3.1/llama_index/indices/query/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/query/embedding_utils.py` & `llama_index_sl-0.5.3.1/llama_index/indices/query/embedding_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/query/empty/base.py` & `llama_index_sl-0.5.3.1/llama_index/indices/query/empty/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/query/keyword_table/query.py` & `llama_index_sl-0.5.3.1/llama_index/indices/query/keyword_table/query.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/query/knowledge_graph/query.py` & `llama_index_sl-0.5.3.1/llama_index/indices/query/knowledge_graph/query.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/query/list/embedding_query.py` & `llama_index_sl-0.5.3.1/llama_index/indices/query/list/embedding_query.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/query/list/query.py` & `llama_index_sl-0.5.3.1/llama_index/indices/query/list/query.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/query/query_combiner/base.py` & `llama_index_sl-0.5.3.1/llama_index/indices/query/query_combiner/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/query/query_runner.py` & `llama_index_sl-0.5.3.1/llama_index/indices/query/query_runner.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/query/query_transform/base.py` & `llama_index_sl-0.5.3.1/llama_index/indices/query/query_transform/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/query/query_transform/prompts.py` & `llama_index_sl-0.5.3.1/llama_index/indices/query/query_transform/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/query/schema.py` & `llama_index_sl-0.5.3.1/llama_index/indices/query/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/query/struct_store/pandas.py` & `llama_index_sl-0.5.3.1/llama_index/indices/query/struct_store/pandas.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/query/struct_store/sql.py` & `llama_index_sl-0.5.3.1/llama_index/indices/query/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/query/tree/embedding_query.py` & `llama_index_sl-0.5.3.1/llama_index/indices/query/tree/embedding_query.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/query/tree/leaf_query.py` & `llama_index_sl-0.5.3.1/llama_index/indices/query/tree/leaf_query.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/query/tree/retrieve_query.py` & `llama_index_sl-0.5.3.1/llama_index/indices/query/tree/retrieve_query.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/query/tree/summarize_query.py` & `llama_index_sl-0.5.3.1/llama_index/indices/query/tree/summarize_query.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/query/vector_store/base.py` & `llama_index_sl-0.5.3.1/llama_index/indices/query/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/query/vector_store/queries.py` & `llama_index_sl-0.5.3.1/llama_index/indices/query/vector_store/queries.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/registry.py` & `llama_index_sl-0.5.3.1/llama_index/indices/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/response/builder.py` & `llama_index_sl-0.5.3.1/llama_index/indices/response/builder.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/service_context.py` & `llama_index_sl-0.5.3.1/llama_index/indices/service_context.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/struct_store/base.py` & `llama_index_sl-0.5.3.1/llama_index/indices/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/struct_store/container_builder.py` & `llama_index_sl-0.5.3.1/llama_index/indices/struct_store/container_builder.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/struct_store/pandas.py` & `llama_index_sl-0.5.3.1/llama_index/indices/struct_store/pandas.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/struct_store/sql.py` & `llama_index_sl-0.5.3.1/llama_index/indices/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/tree/base.py` & `llama_index_sl-0.5.3.1/llama_index/indices/tree/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/tree/inserter.py` & `llama_index_sl-0.5.3.1/llama_index/indices/tree/inserter.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/utils.py` & `llama_index_sl-0.5.3.1/llama_index/indices/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/vector_store/__init__.py` & `llama_index_sl-0.5.3.1/llama_index/indices/vector_store/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/vector_store/base.py` & `llama_index_sl-0.5.3.1/llama_index/indices/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/indices/vector_store/vector_indices.py` & `llama_index_sl-0.5.3.1/llama_index/indices/vector_store/vector_indices.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/langchain_helpers/agents/__init__.py` & `llama_index_sl-0.5.3.1/llama_index/langchain_helpers/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/langchain_helpers/agents/agents.py` & `llama_index_sl-0.5.3.1/llama_index/langchain_helpers/agents/agents.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/langchain_helpers/agents/toolkits.py` & `llama_index_sl-0.5.3.1/llama_index/langchain_helpers/agents/toolkits.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/langchain_helpers/agents/tools.py` & `llama_index_sl-0.5.3.1/llama_index/langchain_helpers/agents/tools.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/langchain_helpers/memory_wrapper.py` & `llama_index_sl-0.5.3.1/llama_index/langchain_helpers/memory_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/langchain_helpers/sql_wrapper.py` & `llama_index_sl-0.5.3.1/llama_index/langchain_helpers/sql_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/langchain_helpers/text_splitter.py` & `llama_index_sl-0.5.3.1/llama_index/langchain_helpers/text_splitter.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/llm_predictor/base.py` & `llama_index_sl-0.5.3.1/llama_index/llm_predictor/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 from dataclasses import dataclass
 from typing import Any, Generator, Optional, Protocol, Tuple
 
 import openai
 from langchain import Cohere, LLMChain, OpenAI
 from langchain.chat_models import ChatOpenAI
 from langchain.llms import AI21
-from langchain.schema import BaseLanguageModel
-
+from langchain.base_language import BaseLanguageModel
 from llama_index.constants import MAX_CHUNK_SIZE, NUM_OUTPUTS
 from llama_index.prompts.base import Prompt
 from llama_index.utils import (
     ErrorToRetry,
     globals_helper,
     retry_on_exceptions_with_backoff,
 )
```

### Comparing `llama_index_sl-0.5.3/llama_index/llm_predictor/chatgpt.py` & `llama_index_sl-0.5.3.1/llama_index/llm_predictor/chatgpt.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/llm_predictor/structured.py` & `llama_index_sl-0.5.3.1/llama_index/llm_predictor/structured.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/logger/base.py` & `llama_index_sl-0.5.3.1/llama_index/logger/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/node_parser/node_utils.py` & `llama_index_sl-0.5.3.1/llama_index/node_parser/node_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/node_parser/simple.py` & `llama_index_sl-0.5.3.1/llama_index/node_parser/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/optimization/optimizer.py` & `llama_index_sl-0.5.3.1/llama_index/optimization/optimizer.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/output_parsers/base.py` & `llama_index_sl-0.5.3.1/llama_index/output_parsers/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/output_parsers/guardrails.py` & `llama_index_sl-0.5.3.1/llama_index/output_parsers/guardrails.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/output_parsers/langchain.py` & `llama_index_sl-0.5.3.1/llama_index/output_parsers/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/playground/base.py` & `llama_index_sl-0.5.3.1/llama_index/playground/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/prompts/base.py` & `llama_index_sl-0.5.3.1/llama_index/prompts/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 from copy import deepcopy
 from string import Formatter
 from typing import Any, Dict, List, Optional, Type, TypeVar
 
 from langchain import BasePromptTemplate as BaseLangchainPrompt
 from langchain import PromptTemplate as LangchainPrompt
 from langchain.chains.prompt_selector import ConditionalPromptSelector
-from langchain.schema import BaseLanguageModel
-
+from langchain.base_language import BaseLanguageModel
 from llama_index.output_parsers.base import BaseOutputParser
 from llama_index.prompts.prompt_type import PromptType
 
 PMT = TypeVar("PMT", bound="Prompt")
 
 
 class Prompt:
```

### Comparing `llama_index_sl-0.5.3/llama_index/prompts/chat_prompts.py` & `llama_index_sl-0.5.3.1/llama_index/prompts/chat_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/prompts/default_prompt_selectors.py` & `llama_index_sl-0.5.3.1/llama_index/prompts/default_prompt_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/prompts/default_prompts.py` & `llama_index_sl-0.5.3.1/llama_index/prompts/default_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/prompts/prompt_type.py` & `llama_index_sl-0.5.3.1/llama_index/prompts/prompt_type.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/prompts/prompts.py` & `llama_index_sl-0.5.3.1/llama_index/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/__init__.py` & `llama_index_sl-0.5.3.1/llama_index/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/base.py` & `llama_index_sl-0.5.3.1/llama_index/readers/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/chatgpt_plugin/base.py` & `llama_index_sl-0.5.3.1/llama_index/readers/chatgpt_plugin/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/chroma.py` & `llama_index_sl-0.5.3.1/llama_index/readers/chroma.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/database.py` & `llama_index_sl-0.5.3.1/llama_index/readers/database.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/discord_reader.py` & `llama_index_sl-0.5.3.1/llama_index/readers/discord_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/download.py` & `llama_index_sl-0.5.3.1/llama_index/readers/download.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/elasticsearch.py` & `llama_index_sl-0.5.3.1/llama_index/readers/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/faiss.py` & `llama_index_sl-0.5.3.1/llama_index/readers/faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/file/base.py` & `llama_index_sl-0.5.3.1/llama_index/readers/file/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/file/base_parser.py` & `llama_index_sl-0.5.3.1/llama_index/readers/file/base_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/file/docs_parser.py` & `llama_index_sl-0.5.3.1/llama_index/readers/file/docs_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/file/epub_parser.py` & `llama_index_sl-0.5.3.1/llama_index/readers/file/epub_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/file/image_parser.py` & `llama_index_sl-0.5.3.1/llama_index/readers/file/image_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/file/markdown_parser.py` & `llama_index_sl-0.5.3.1/llama_index/readers/file/markdown_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/file/mbox_parser.py` & `llama_index_sl-0.5.3.1/llama_index/readers/file/mbox_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/file/slides_parser.py` & `llama_index_sl-0.5.3.1/llama_index/readers/file/slides_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/file/tabular_parser.py` & `llama_index_sl-0.5.3.1/llama_index/readers/file/tabular_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/file/video_audio.py` & `llama_index_sl-0.5.3.1/llama_index/readers/file/video_audio.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/github_readers/github_api_client.py` & `llama_index_sl-0.5.3.1/llama_index/readers/github_readers/github_api_client.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/github_readers/github_repository_reader.py` & `llama_index_sl-0.5.3.1/llama_index/readers/github_readers/github_repository_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/github_readers/utils.py` & `llama_index_sl-0.5.3.1/llama_index/readers/github_readers/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/google_readers/gdocs.py` & `llama_index_sl-0.5.3.1/llama_index/readers/google_readers/gdocs.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/google_readers/gsheets.py` & `llama_index_sl-0.5.3.1/llama_index/readers/google_readers/gsheets.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/json.py` & `llama_index_sl-0.5.3.1/llama_index/readers/json.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/make_com/wrapper.py` & `llama_index_sl-0.5.3.1/llama_index/readers/make_com/wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/mbox.py` & `llama_index_sl-0.5.3.1/llama_index/readers/mbox.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/mongo.py` & `llama_index_sl-0.5.3.1/llama_index/readers/mongo.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/notion.py` & `llama_index_sl-0.5.3.1/llama_index/readers/notion.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/obsidian.py` & `llama_index_sl-0.5.3.1/llama_index/readers/obsidian.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/pinecone.py` & `llama_index_sl-0.5.3.1/llama_index/readers/pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/qdrant.py` & `llama_index_sl-0.5.3.1/llama_index/readers/qdrant.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/schema/base.py` & `llama_index_sl-0.5.3.1/llama_index/readers/schema/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/slack.py` & `llama_index_sl-0.5.3.1/llama_index/readers/slack.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/steamship/file_reader.py` & `llama_index_sl-0.5.3.1/llama_index/readers/steamship/file_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/string_iterable.py` & `llama_index_sl-0.5.3.1/llama_index/readers/string_iterable.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/twitter.py` & `llama_index_sl-0.5.3.1/llama_index/readers/twitter.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/weaviate/data_structs.py` & `llama_index_sl-0.5.3.1/llama_index/readers/weaviate/data_structs.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/weaviate/reader.py` & `llama_index_sl-0.5.3.1/llama_index/readers/weaviate/reader.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/weaviate/utils.py` & `llama_index_sl-0.5.3.1/llama_index/readers/weaviate/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/web.py` & `llama_index_sl-0.5.3.1/llama_index/readers/web.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/wikipedia.py` & `llama_index_sl-0.5.3.1/llama_index/readers/wikipedia.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/readers/youtube_transcript.py` & `llama_index_sl-0.5.3.1/llama_index/readers/youtube_transcript.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/response/notebook_utils.py` & `llama_index_sl-0.5.3.1/llama_index/response/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/response/schema.py` & `llama_index_sl-0.5.3.1/llama_index/response/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/schema.py` & `llama_index_sl-0.5.3.1/llama_index/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/token_counter/mock_chain_wrapper.py` & `llama_index_sl-0.5.3.1/llama_index/token_counter/mock_chain_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/token_counter/mock_embed_model.py` & `llama_index_sl-0.5.3.1/llama_index/token_counter/mock_embed_model.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/token_counter/token_counter.py` & `llama_index_sl-0.5.3.1/llama_index/token_counter/token_counter.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/token_counter/utils.py` & `llama_index_sl-0.5.3.1/llama_index/token_counter/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/tools/file_utils.py` & `llama_index_sl-0.5.3.1/llama_index/tools/file_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/tools/migrate_v1_to_v2.py` & `llama_index_sl-0.5.3.1/llama_index/tools/migrate_v1_to_v2.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/utils.py` & `llama_index_sl-0.5.3.1/llama_index/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/vector_stores/__init__.py` & `llama_index_sl-0.5.3.1/llama_index/vector_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/vector_stores/chatgpt_plugin.py` & `llama_index_sl-0.5.3.1/llama_index/vector_stores/chatgpt_plugin.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/vector_stores/chroma.py` & `llama_index_sl-0.5.3.1/llama_index/vector_stores/chroma.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/vector_stores/faiss.py` & `llama_index_sl-0.5.3.1/llama_index/vector_stores/faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/vector_stores/opensearch.py` & `llama_index_sl-0.5.3.1/llama_index/vector_stores/opensearch.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/vector_stores/pinecone.py` & `llama_index_sl-0.5.3.1/llama_index/vector_stores/pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/vector_stores/qdrant.py` & `llama_index_sl-0.5.3.1/llama_index/vector_stores/qdrant.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/vector_stores/simple.py` & `llama_index_sl-0.5.3.1/llama_index/vector_stores/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/vector_stores/types.py` & `llama_index_sl-0.5.3.1/llama_index/vector_stores/types.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index/vector_stores/weaviate.py` & `llama_index_sl-0.5.3.1/llama_index/vector_stores/weaviate.py`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/llama_index_sl.egg-info/SOURCES.txt` & `llama_index_sl-0.5.3.1/llama_index_sl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llama_index_sl-0.5.3/setup.py` & `llama_index_sl-0.5.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = '0.5.3'
+VERSION = '0.5.3.1'
 DESCRIPTION = 'llama_index edited for unicode support and pdfminer.six'
 
 # Setting up
 setup(
     name="llama_index_sl",
     version=VERSION,
     author="sl",
```

