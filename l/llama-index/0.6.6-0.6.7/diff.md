# Comparing `tmp/llama_index-0.6.6.tar.gz` & `tmp/llama_index-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index-0.6.6.tar", last modified: Sat May 13 00:11:40 2023, max compression
+gzip compressed data, was "llama_index-0.6.7.tar", last modified: Sun May 14 19:13:20 2023, max compression
```

## Comparing `llama_index-0.6.6.tar` & `llama_index-0.6.7.tar`

### file list

```diff
@@ -1,472 +1,477 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.107422 llama_index-0.6.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-13 00:11:20.000000 llama_index-0.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-13 00:11:20.000000 llama_index-0.6.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-13 00:11:40.107422 llama_index-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-13 00:11:20.000000 llama_index-0.6.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.059422 llama_index-0.6.6/llama_index/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/async_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.063422 llama_index-0.6.6/llama_index/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/callbacks/llama_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/callbacks/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.063422 llama_index-0.6.6/llama_index/composability/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/composability/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/composability/joint_qa_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.063422 llama_index-0.6.6/llama_index/data_structs/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/data_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/data_structs/data_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/data_structs/document_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/data_structs/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/data_structs/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/data_structs/struct_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/data_structs/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.067422 llama_index-0.6.6/llama_index/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/embeddings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/embeddings/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/embeddings/langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/embeddings/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/embeddings/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.067422 llama_index-0.6.6/llama_index/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12080 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/evaluation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/evaluation/dataset_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/img_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.067422 llama_index-0.6.6/llama_index/indices/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/base_retriever.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.067422 llama_index-0.6.6/llama_index/indices/common/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.067422 llama_index-0.6.6/llama_index/indices/common/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/common/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/common/struct_store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/common/struct_store/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/common/struct_store/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.071422 llama_index-0.6.6/llama_index/indices/common_tree/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/common_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/common_tree/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.071422 llama_index-0.6.6/llama_index/indices/composability/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/composability/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.071422 llama_index-0.6.6/llama_index/indices/document_summary/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/document_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/document_summary/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/document_summary/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.071422 llama_index-0.6.6/llama_index/indices/empty/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/empty/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/empty/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.071422 llama_index-0.6.6/llama_index/indices/keyword_table/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/keyword_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/keyword_table/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/keyword_table/rake_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/keyword_table/retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/keyword_table/simple_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/keyword_table/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.071422 llama_index-0.6.6/llama_index/indices/knowledge_graph/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/knowledge_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/knowledge_graph/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/knowledge_graph/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.071422 llama_index-0.6.6/llama_index/indices/list/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/list/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/list/retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.071422 llama_index-0.6.6/llama_index/indices/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/postprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/postprocessor/cohere_rerank.py
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/postprocessor/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/postprocessor/node_recency.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/postprocessor/pii.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/postprocessor/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/prompt_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.071422 llama_index-0.6.6/llama_index/indices/query/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/query/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/query/embedding_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.071422 llama_index-0.6.6/llama_index/indices/query/query_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/query/query_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/query/query_transform/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/query/query_transform/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/query/response_synthesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.075422 llama_index-0.6.6/llama_index/indices/response/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21926 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/response/response_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/response/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/service_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.075422 llama_index-0.6.6/llama_index/indices/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/struct_store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/struct_store/container_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/struct_store/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/struct_store/pandas_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/struct_store/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/struct_store/sql_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.075422 llama_index-0.6.6/llama_index/indices/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/tree/all_leaf_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/tree/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/tree/inserter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/tree/select_leaf_embedding_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)    15309 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/tree/select_leaf_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/tree/tree_root_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.075422 llama_index-0.6.6/llama_index/indices/vector_store/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/vector_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/vector_store/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.075422 llama_index-0.6.6/llama_index/indices/vector_store/retrievers/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/vector_store/retrievers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.075422 llama_index-0.6.6/llama_index/indices/vector_store/retrievers/auto_retriever/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/vector_store/retrievers/auto_retriever/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/indices/vector_store/retrievers/retriever.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.075422 llama_index-0.6.6/llama_index/langchain_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/langchain_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.075422 llama_index-0.6.6/llama_index/langchain_helpers/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/langchain_helpers/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/langchain_helpers/agents/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/langchain_helpers/agents/toolkits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/langchain_helpers/agents/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/langchain_helpers/chain_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/langchain_helpers/memory_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/langchain_helpers/sql_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/langchain_helpers/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)    19719 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/langchain_helpers/text_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.079422 llama_index-0.6.6/llama_index/llm_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/llm_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/llm_predictor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/llm_predictor/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/llm_predictor/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/llm_predictor/structured.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.079422 llama_index-0.6.6/llama_index/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/logger/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.079422 llama_index-0.6.6/llama_index/node_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/node_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/node_parser/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/node_parser/node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/node_parser/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.079422 llama_index-0.6.6/llama_index/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/optimization/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.079422 llama_index-0.6.6/llama_index/output_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/output_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/output_parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/output_parsers/guardrails.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/output_parsers/langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/output_parsers/selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.079422 llama_index-0.6.6/llama_index/playground/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/playground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/playground/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.079422 llama_index-0.6.6/llama_index/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/prompts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/prompts/chat_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/prompts/default_prompt_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/prompts/default_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/prompts/prompt_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/prompts/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.079422 llama_index-0.6.6/llama_index/query_engine/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/query_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/query_engine/graph_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/query_engine/multistep_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/query_engine/retriever_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/query_engine/router_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/query_engine/transform_query_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.083422 llama_index-0.6.6/llama_index/readers/
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.083422 llama_index-0.6.6/llama_index/readers/chatgpt_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/chatgpt_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/chatgpt_plugin/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/deeplake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/discord_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/faiss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.087422 llama_index-0.6.6/llama_index/readers/file/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/file/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/file/base_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/file/docs_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/file/epub_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/file/image_caption_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/file/image_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/file/image_vision_llm_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/file/ipynb_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/file/markdown_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/file/mbox_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/file/slides_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/file/tabular_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/file/video_audio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.087422 llama_index-0.6.6/llama_index/readers/github_readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/github_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/github_readers/github_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15889 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/github_readers/github_repository_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/github_readers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.087422 llama_index-0.6.6/llama_index/readers/google_readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/google_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/google_readers/gdocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/google_readers/gsheets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.087422 llama_index-0.6.6/llama_index/readers/make_com/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/make_com/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/make_com/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/mbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/milvus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/notion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/obsidian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.087422 llama_index-0.6.6/llama_index/readers/redis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/redis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.087422 llama_index-0.6.6/llama_index/readers/schema/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/schema/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/slack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.087422 llama_index-0.6.6/llama_index/readers/steamship/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/steamship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/steamship/file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/string_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/twitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.087422 llama_index-0.6.6/llama_index/readers/weaviate/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/weaviate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/weaviate/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/weaviate/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/weaviate/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/web.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/wikipedia.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/readers/youtube_transcript.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.091422 llama_index-0.6.6/llama_index/response/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/response/notebook_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/response/pprint_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/response/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/response/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.091422 llama_index-0.6.6/llama_index/retrievers/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/retrievers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/retrievers/transform_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.091422 llama_index-0.6.6/llama_index/selectors/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/selectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/selectors/llm_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/selectors/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/selectors/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.091422 llama_index-0.6.6/llama_index/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.091422 llama_index-0.6.6/llama_index/storage/docstore/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/storage/docstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/storage/docstore/keyval_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/storage/docstore/mongo_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/storage/docstore/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/storage/docstore/simple_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/storage/docstore/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/storage/docstore/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.091422 llama_index-0.6.6/llama_index/storage/index_store/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/storage/index_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/storage/index_store/keyval_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/storage/index_store/mongo_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/storage/index_store/simple_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/storage/index_store/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/storage/index_store/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.091422 llama_index-0.6.6/llama_index/storage/kvstore/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/storage/kvstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/storage/kvstore/mongodb_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/storage/kvstore/simple_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/storage/kvstore/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/storage/storage_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.095422 llama_index-0.6.6/llama_index/token_counter/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/token_counter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/token_counter/mock_chain_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/token_counter/mock_embed_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/token_counter/token_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/token_counter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.095422 llama_index-0.6.6/llama_index/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/tools/query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/tools/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.095422 llama_index-0.6.6/llama_index/tts/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/tts/bark.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/tts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/tts/elevenlabs.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.095422 llama_index-0.6.6/llama_index/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/vector_stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/vector_stores/chatgpt_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/vector_stores/chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/vector_stores/deeplake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/vector_stores/faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/vector_stores/lancedb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/vector_stores/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)    15898 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/vector_stores/milvus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/vector_stores/myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/vector_stores/opensearch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/vector_stores/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/vector_stores/qdrant.py
--rw-r--r--   0 runner    (1001) docker     (123)    14195 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/vector_stores/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/vector_stores/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/vector_stores/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/vector_stores/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/vector_stores/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-05-13 00:11:20.000000 llama_index-0.6.6/llama_index/vector_stores/weaviate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.059422 llama_index-0.6.6/llama_index.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-13 00:11:40.000000 llama_index-0.6.6/llama_index.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14603 2023-05-13 00:11:40.000000 llama_index-0.6.6/llama_index.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 00:11:40.000000 llama_index-0.6.6/llama_index.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-13 00:11:40.000000 llama_index-0.6.6/llama_index.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-13 00:11:40.000000 llama_index-0.6.6/llama_index.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-13 00:11:20.000000 llama_index-0.6.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 00:11:40.107422 llama_index-0.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-13 00:11:20.000000 llama_index-0.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.095422 llama_index-0.6.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.095422 llama_index-0.6.6/tests/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/callbacks/test_llama_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.095422 llama_index-0.6.6/tests/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/embeddings/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.099422 llama_index-0.6.6/tests/indices/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.099422 llama_index-0.6.6/tests/indices/composability/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/composability/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.099422 llama_index-0.6.6/tests/indices/document_summary/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/document_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/document_summary/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/document_summary/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.099422 llama_index-0.6.6/tests/indices/empty/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/empty/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.099422 llama_index-0.6.6/tests/indices/keyword_table/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/keyword_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/keyword_table/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/keyword_table/test_retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/keyword_table/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.099422 llama_index-0.6.6/tests/indices/knowledge_graph/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/knowledge_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/knowledge_graph/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/knowledge_graph/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/knowledge_graph/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.099422 llama_index-0.6.6/tests/indices/list/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/list/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/list/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.099422 llama_index-0.6.6/tests/indices/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/postprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/postprocessor/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.099422 llama_index-0.6.6/tests/indices/query/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/query/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.099422 llama_index-0.6.6/tests/indices/query/query_transform/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/query/query_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/query/query_transform/mock_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/query/query_transform/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/query/test_compose.py
--rw-r--r--   0 runner    (1001) docker     (123)    12483 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/query/test_compose_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/query/test_query_bundle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.103422 llama_index-0.6.6/tests/indices/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/struct_store/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11931 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/struct_store/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/struct_store/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/struct_store/test_sql_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/test_loading_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/test_node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/test_prompt_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.103422 llama_index-0.6.6/tests/indices/tree/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/tree/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/tree/test_embedding_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/tree/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/tree/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.103422 llama_index-0.6.6/tests/indices/vector_store/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/vector_store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.103422 llama_index-0.6.6/tests/indices/vector_store/auto_retriever/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/vector_store/auto_retriever/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/vector_store/auto_retriever/test_output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/vector_store/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/vector_store/mock_faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/vector_store/mock_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/vector_store/test_faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/vector_store/test_myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/vector_store/test_pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/vector_store/test_retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/vector_store/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/indices/vector_store/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.103422 llama_index-0.6.6/tests/langchain_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/langchain_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/langchain_helpers/test_text_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.103422 llama_index-0.6.6/tests/llm_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/llm_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/llm_predictor/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.103422 llama_index-0.6.6/tests/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/logger/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.103422 llama_index-0.6.6/tests/mock_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/mock_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/mock_utils/mock_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/mock_utils/mock_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/mock_utils/mock_text_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/mock_utils/mock_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.103422 llama_index-0.6.6/tests/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/optimization/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.103422 llama_index-0.6.6/tests/output_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/output_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/output_parsers/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/output_parsers/test_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.103422 llama_index-0.6.6/tests/playground/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/playground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/playground/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.107422 llama_index-0.6.6/tests/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/prompts/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.107422 llama_index-0.6.6/tests/readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/readers/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/readers/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/readers/test_mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/readers/test_string_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.107422 llama_index-0.6.6/tests/selectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/selectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/selectors/test_llm_selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.107422 llama_index-0.6.6/tests/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/storage/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.107422 llama_index-0.6.6/tests/storage/docstore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/storage/docstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/storage/docstore/test_mongo_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/storage/docstore/test_simple_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/storage/test_storage_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.107422 llama_index-0.6.6/tests/token_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/token_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/token_predictor/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:40.107422 llama_index-0.6.6/tests/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/vector_stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/vector_stores/test_qdrant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-13 00:11:20.000000 llama_index-0.6.6/tests/vector_stores/test_weaviate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.940501 llama_index-0.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-14 19:13:04.000000 llama_index-0.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-14 19:13:04.000000 llama_index-0.6.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-14 19:13:20.940501 llama_index-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-14 19:13:04.000000 llama_index-0.6.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.884500 llama_index-0.6.7/llama_index/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/async_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.888500 llama_index-0.6.7/llama_index/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/callbacks/aim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/callbacks/llama_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/callbacks/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.888500 llama_index-0.6.7/llama_index/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/composability/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/composability/joint_qa_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.888500 llama_index-0.6.7/llama_index/data_structs/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/data_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/data_structs/data_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/data_structs/document_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/data_structs/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/data_structs/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/data_structs/struct_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/data_structs/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.888500 llama_index-0.6.7/llama_index/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/embeddings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/embeddings/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/embeddings/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/embeddings/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/embeddings/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.888500 llama_index-0.6.7/llama_index/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12080 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/evaluation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/evaluation/dataset_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/img_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.892500 llama_index-0.6.7/llama_index/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/base_retriever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.892500 llama_index-0.6.7/llama_index/indices/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.892500 llama_index-0.6.7/llama_index/indices/common/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/common/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/common/struct_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/common/struct_store/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/common/struct_store/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.892500 llama_index-0.6.7/llama_index/indices/common_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/common_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/common_tree/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.892500 llama_index-0.6.7/llama_index/indices/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/composability/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.892500 llama_index-0.6.7/llama_index/indices/document_summary/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/document_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/document_summary/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/document_summary/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.892500 llama_index-0.6.7/llama_index/indices/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/empty/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/empty/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.892500 llama_index-0.6.7/llama_index/indices/keyword_table/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/keyword_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/keyword_table/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/keyword_table/rake_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/keyword_table/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/keyword_table/simple_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/keyword_table/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.892500 llama_index-0.6.7/llama_index/indices/knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/knowledge_graph/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/knowledge_graph/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.896500 llama_index-0.6.7/llama_index/indices/list/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/list/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/list/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.896500 llama_index-0.6.7/llama_index/indices/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/postprocessor/cohere_rerank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/postprocessor/llm_rerank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/postprocessor/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/postprocessor/node_recency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/postprocessor/pii.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/postprocessor/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/prompt_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.896500 llama_index-0.6.7/llama_index/indices/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/query/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/query/embedding_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.896500 llama_index-0.6.7/llama_index/indices/query/query_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/query/query_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/query/query_transform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/query/query_transform/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/query/response_synthesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.896500 llama_index-0.6.7/llama_index/indices/response/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21926 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/response/response_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/response/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/service_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.900500 llama_index-0.6.7/llama_index/indices/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/struct_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/struct_store/container_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/struct_store/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/struct_store/pandas_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/struct_store/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/struct_store/sql_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.900500 llama_index-0.6.7/llama_index/indices/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/tree/all_leaf_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/tree/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/tree/inserter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/tree/select_leaf_embedding_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15309 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/tree/select_leaf_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/tree/tree_root_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.900500 llama_index-0.6.7/llama_index/indices/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/vector_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/vector_store/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.900500 llama_index-0.6.7/llama_index/indices/vector_store/retrievers/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/vector_store/retrievers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.900500 llama_index-0.6.7/llama_index/indices/vector_store/retrievers/auto_retriever/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/vector_store/retrievers/auto_retriever/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/indices/vector_store/retrievers/retriever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.900500 llama_index-0.6.7/llama_index/langchain_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/langchain_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.900500 llama_index-0.6.7/llama_index/langchain_helpers/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/langchain_helpers/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/langchain_helpers/agents/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/langchain_helpers/agents/toolkits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/langchain_helpers/agents/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/langchain_helpers/chain_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/langchain_helpers/memory_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/langchain_helpers/sql_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/langchain_helpers/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19719 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/langchain_helpers/text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.904500 llama_index-0.6.7/llama_index/llm_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/llm_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/llm_predictor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/llm_predictor/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/llm_predictor/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/llm_predictor/structured.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.904500 llama_index-0.6.7/llama_index/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/logger/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.904500 llama_index-0.6.7/llama_index/node_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/node_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/node_parser/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/node_parser/node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/node_parser/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.904500 llama_index-0.6.7/llama_index/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/optimization/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.904500 llama_index-0.6.7/llama_index/output_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/output_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/output_parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/output_parsers/guardrails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/output_parsers/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/output_parsers/selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.904500 llama_index-0.6.7/llama_index/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/playground/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.908500 llama_index-0.6.7/llama_index/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/prompts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/prompts/chat_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/prompts/choice_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/prompts/default_choice_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/prompts/default_prompt_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/prompts/default_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/prompts/prompt_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/prompts/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.908500 llama_index-0.6.7/llama_index/query_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/query_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/query_engine/graph_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/query_engine/multistep_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/query_engine/retriever_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/query_engine/router_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/query_engine/transform_query_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.912500 llama_index-0.6.7/llama_index/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.912500 llama_index-0.6.7/llama_index/readers/chatgpt_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/chatgpt_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/chatgpt_plugin/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/deeplake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/discord_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/faiss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.912500 llama_index-0.6.7/llama_index/readers/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/file/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/file/base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/file/docs_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/file/epub_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/file/image_caption_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/file/image_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/file/image_vision_llm_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/file/ipynb_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/file/markdown_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/file/mbox_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/file/slides_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/file/tabular_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/file/video_audio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.912500 llama_index-0.6.7/llama_index/readers/github_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/github_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/github_readers/github_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15889 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/github_readers/github_repository_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/github_readers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.916500 llama_index-0.6.7/llama_index/readers/google_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/google_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/google_readers/gdocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/google_readers/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.916500 llama_index-0.6.7/llama_index/readers/make_com/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/make_com/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/make_com/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/mbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/notion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/obsidian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.916500 llama_index-0.6.7/llama_index/readers/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/redis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.916500 llama_index-0.6.7/llama_index/readers/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/schema/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.916500 llama_index-0.6.7/llama_index/readers/steamship/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/steamship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/steamship/file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/string_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/twitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.916500 llama_index-0.6.7/llama_index/readers/weaviate/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/weaviate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/weaviate/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/weaviate/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/weaviate/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/readers/youtube_transcript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.916500 llama_index-0.6.7/llama_index/response/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/response/notebook_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/response/pprint_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/response/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/response/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.916500 llama_index-0.6.7/llama_index/retrievers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/retrievers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/retrievers/transform_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.916500 llama_index-0.6.7/llama_index/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/selectors/llm_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/selectors/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/selectors/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.916500 llama_index-0.6.7/llama_index/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.920500 llama_index-0.6.7/llama_index/storage/docstore/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/storage/docstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/storage/docstore/keyval_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/storage/docstore/mongo_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/storage/docstore/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/storage/docstore/simple_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/storage/docstore/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/storage/docstore/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.920500 llama_index-0.6.7/llama_index/storage/index_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/storage/index_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/storage/index_store/keyval_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/storage/index_store/mongo_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/storage/index_store/simple_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/storage/index_store/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/storage/index_store/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.920500 llama_index-0.6.7/llama_index/storage/kvstore/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/storage/kvstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/storage/kvstore/mongodb_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/storage/kvstore/simple_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/storage/kvstore/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/storage/storage_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.920500 llama_index-0.6.7/llama_index/token_counter/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/token_counter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/token_counter/mock_chain_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/token_counter/mock_embed_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/token_counter/token_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/token_counter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.920500 llama_index-0.6.7/llama_index/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/tools/query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/tools/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.920500 llama_index-0.6.7/llama_index/tts/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/tts/bark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/tts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/tts/elevenlabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.924501 llama_index-0.6.7/llama_index/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/vector_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/vector_stores/chatgpt_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/vector_stores/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/vector_stores/deeplake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/vector_stores/faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/vector_stores/lancedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/vector_stores/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15898 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/vector_stores/milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/vector_stores/myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/vector_stores/opensearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/vector_stores/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/vector_stores/qdrant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14345 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/vector_stores/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/vector_stores/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/vector_stores/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/vector_stores/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/vector_stores/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-05-14 19:13:04.000000 llama_index-0.6.7/llama_index/vector_stores/weaviate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.884500 llama_index-0.6.7/llama_index.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-14 19:13:20.000000 llama_index-0.6.7/llama_index.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14809 2023-05-14 19:13:20.000000 llama_index-0.6.7/llama_index.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 19:13:20.000000 llama_index-0.6.7/llama_index.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-14 19:13:20.000000 llama_index-0.6.7/llama_index.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-14 19:13:20.000000 llama_index-0.6.7/llama_index.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-14 19:13:04.000000 llama_index-0.6.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 19:13:20.940501 llama_index-0.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-14 19:13:04.000000 llama_index-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.924501 llama_index-0.6.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.924501 llama_index-0.6.7/tests/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/callbacks/test_llama_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.924501 llama_index-0.6.7/tests/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/embeddings/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.928501 llama_index-0.6.7/tests/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.928501 llama_index-0.6.7/tests/indices/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/composability/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.928501 llama_index-0.6.7/tests/indices/document_summary/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/document_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/document_summary/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/document_summary/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.928501 llama_index-0.6.7/tests/indices/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/empty/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.928501 llama_index-0.6.7/tests/indices/keyword_table/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/keyword_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/keyword_table/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/keyword_table/test_retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/keyword_table/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.928501 llama_index-0.6.7/tests/indices/knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/knowledge_graph/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/knowledge_graph/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/knowledge_graph/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.928501 llama_index-0.6.7/tests/indices/list/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/list/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/list/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.928501 llama_index-0.6.7/tests/indices/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/postprocessor/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/postprocessor/test_llm_rerank.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.932501 llama_index-0.6.7/tests/indices/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/query/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.932501 llama_index-0.6.7/tests/indices/query/query_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/query/query_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/query/query_transform/mock_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/query/query_transform/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/query/test_compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12483 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/query/test_compose_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/query/test_query_bundle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.932501 llama_index-0.6.7/tests/indices/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/struct_store/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11931 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/struct_store/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/struct_store/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/struct_store/test_sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/test_loading_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/test_node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/test_prompt_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.932501 llama_index-0.6.7/tests/indices/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/tree/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/tree/test_embedding_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/tree/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/tree/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.932501 llama_index-0.6.7/tests/indices/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/vector_store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.932501 llama_index-0.6.7/tests/indices/vector_store/auto_retriever/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/vector_store/auto_retriever/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/vector_store/auto_retriever/test_output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/vector_store/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/vector_store/mock_faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/vector_store/mock_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/vector_store/test_faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/vector_store/test_myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/vector_store/test_pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/vector_store/test_retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/vector_store/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/indices/vector_store/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.936501 llama_index-0.6.7/tests/langchain_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/langchain_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/langchain_helpers/test_text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.936501 llama_index-0.6.7/tests/llm_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/llm_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/llm_predictor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.936501 llama_index-0.6.7/tests/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/logger/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.936501 llama_index-0.6.7/tests/mock_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/mock_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/mock_utils/mock_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/mock_utils/mock_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/mock_utils/mock_text_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/mock_utils/mock_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.936501 llama_index-0.6.7/tests/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/optimization/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.936501 llama_index-0.6.7/tests/output_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/output_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/output_parsers/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/output_parsers/test_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.936501 llama_index-0.6.7/tests/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/playground/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.936501 llama_index-0.6.7/tests/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/prompts/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.936501 llama_index-0.6.7/tests/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/readers/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/readers/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/readers/test_mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/readers/test_string_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.936501 llama_index-0.6.7/tests/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/selectors/test_llm_selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.940501 llama_index-0.6.7/tests/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/storage/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.940501 llama_index-0.6.7/tests/storage/docstore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/storage/docstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/storage/docstore/test_mongo_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/storage/docstore/test_simple_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/storage/test_storage_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.940501 llama_index-0.6.7/tests/token_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/token_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/token_predictor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:20.940501 llama_index-0.6.7/tests/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/vector_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/vector_stores/test_qdrant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-14 19:13:04.000000 llama_index-0.6.7/tests/vector_stores/test_weaviate.py
```

### Comparing `llama_index-0.6.6/LICENSE` & `llama_index-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/PKG-INFO` & `llama_index-0.6.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama_index
-Version: 0.6.6
+Version: 0.6.7
 Summary: Interface between LLMs and your data
 Home-page: https://github.com/jerryjliu/llama_index
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🗂️ LlamaIndex 🦙
```

### Comparing `llama_index-0.6.6/README.md` & `llama_index-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/__init__.py` & `llama_index-0.6.7/llama_index/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/callbacks/base.py` & `llama_index-0.6.7/llama_index/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/callbacks/llama_debug.py` & `llama_index-0.6.7/llama_index/callbacks/llama_debug.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/callbacks/schema.py` & `llama_index-0.6.7/llama_index/callbacks/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/composability/joint_qa_summary.py` & `llama_index-0.6.7/llama_index/composability/joint_qa_summary.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/data_structs/data_structs.py` & `llama_index-0.6.7/llama_index/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/data_structs/document_summary.py` & `llama_index-0.6.7/llama_index/data_structs/document_summary.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/data_structs/node.py` & `llama_index-0.6.7/llama_index/data_structs/node.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/data_structs/registry.py` & `llama_index-0.6.7/llama_index/data_structs/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/data_structs/struct_type.py` & `llama_index-0.6.7/llama_index/data_structs/struct_type.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/data_structs/table.py` & `llama_index-0.6.7/llama_index/data_structs/table.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/embeddings/base.py` & `llama_index-0.6.7/llama_index/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/embeddings/google.py` & `llama_index-0.6.7/llama_index/embeddings/google.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/embeddings/langchain.py` & `llama_index-0.6.7/llama_index/embeddings/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/embeddings/openai.py` & `llama_index-0.6.7/llama_index/embeddings/openai.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/embeddings/utils.py` & `llama_index-0.6.7/llama_index/embeddings/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/evaluation/base.py` & `llama_index-0.6.7/llama_index/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/evaluation/dataset_generation.py` & `llama_index-0.6.7/llama_index/evaluation/dataset_generation.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/img_utils.py` & `llama_index-0.6.7/llama_index/img_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/__init__.py` & `llama_index-0.6.7/llama_index/indices/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/base.py` & `llama_index-0.6.7/llama_index/indices/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/base_retriever.py` & `llama_index-0.6.7/llama_index/indices/base_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/common/struct_store/base.py` & `llama_index-0.6.7/llama_index/indices/common/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/common/struct_store/schema.py` & `llama_index-0.6.7/llama_index/indices/common/struct_store/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/common/struct_store/sql.py` & `llama_index-0.6.7/llama_index/indices/common/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/common_tree/base.py` & `llama_index-0.6.7/llama_index/indices/common_tree/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/composability/graph.py` & `llama_index-0.6.7/llama_index/indices/composability/graph.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/document_summary/base.py` & `llama_index-0.6.7/llama_index/indices/document_summary/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/document_summary/retrievers.py` & `llama_index-0.6.7/llama_index/indices/document_summary/retrievers.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,76 +6,29 @@
 
 from llama_index.callbacks.schema import CBEventType
 from llama_index.indices.document_summary.base import GPTDocumentSummaryIndex
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.base_retriever import BaseRetriever
 from typing import Any, List, Optional, Callable, Tuple, Dict
 from llama_index.data_structs.node import Node, NodeWithScore
-from llama_index.prompts.prompts import QuestionAnswerPrompt
+from llama_index.prompts.choice_select import ChoiceSelectPrompt
 from llama_index.indices.service_context import ServiceContext
 from llama_index.indices.query.embedding_utils import (
     get_top_k_embeddings,
 )
+from llama_index.prompts.choice_select import (
+    DEFAULT_CHOICE_SELECT_PROMPT,
+)
 import logging
-
-logger = logging.getLogger(__name__)
-
-
-DEFAULT_CHOICE_SELECT_PROMPT_TMPL = (
-    "A list of documents is shown below. Each document has a number next to it along "
-    "with a summary of the document. A question is also provided. \n"
-    "Respond with the numbers of the documents "
-    "you should consult to answer the question, in order of relevance, as well \n"
-    "as the relevance score. The relevance score is a number from 1-10 based on "
-    "how relevant you think the document is to the question.\n"
-    "Do not include any documents that are not relevant to the question. \n"
-    "Example format: \n"
-    "Document 1:\n<summary of document 1>\n\n"
-    "Document 2:\n<summary of document 2>\n\n"
-    "...\n\n"
-    "Document 10:\n<summary of document 10>\n\n"
-    "Question: <question>\n"
-    "Answer:\n"
-    "Doc: 9, Relevance: 7\n"
-    "Doc: 3, Relevance: 4\n"
-    "Doc: 7, Relevance: 3\n\n"
-    "Let's try this now: \n\n"
-    "{context_str}\n"
-    "Question: {query_str}\n"
-    "Answer:\n"
+from llama_index.indices.utils import (
+    default_format_node_batch_fn,
+    default_parse_choice_select_answer_fn,
 )
-DEFAULT_CHOICE_SELECT_PROMPT = QuestionAnswerPrompt(DEFAULT_CHOICE_SELECT_PROMPT_TMPL)
-
 
-def default_format_node_batch_fn(
-    summary_nodes: List[Node],
-) -> str:
-    """Default format node batch function."""
-    fmt_node_txts = []
-    for idx in range(len(summary_nodes)):
-        number = idx + 1
-        fmt_node_txts.append(f"Document {number}:\n{summary_nodes[idx].get_text()}")
-    return "\n\n".join(fmt_node_txts)
-
-
-def default_parse_choice_select_answer_fn(
-    answer: str, num_choices: int
-) -> Tuple[List[int], Optional[List[float]]]:
-    """Default parse choice select answer function."""
-    answer_lines = answer.split("\n")
-    answer_nums = []
-    answer_relevances = []
-    for answer_line in answer_lines:
-        line_tokens = answer_line.split(",")
-        answer_num = int(line_tokens[0].split(":")[1].strip())
-        if answer_num > num_choices:
-            continue
-        answer_nums.append(answer_num)
-        answer_relevances.append(float(line_tokens[1].split(":")[1].strip()))
-    return answer_nums, answer_relevances
+logger = logging.getLogger(__name__)
 
 
 class DocumentSummaryIndexRetriever(BaseRetriever):
     """Document Summary Index Retriever.
 
     By default, select relevant summaries from index using LLM calls.
 
@@ -83,15 +36,15 @@
         index (GPTDocumentSummaryIndex): The index to retrieve from.
 
     """
 
     def __init__(
         self,
         index: GPTDocumentSummaryIndex,
-        choice_select_prompt: Optional[QuestionAnswerPrompt] = None,
+        choice_select_prompt: Optional[ChoiceSelectPrompt] = None,
         choice_batch_size: int = 10,
         format_node_batch_fn: Optional[Callable] = None,
         parse_choice_select_answer_fn: Optional[Callable] = None,
         service_context: Optional[ServiceContext] = None,
         **kwargs: Any,
     ) -> None:
         self._index = index
```

### Comparing `llama_index-0.6.6/llama_index/indices/empty/base.py` & `llama_index-0.6.7/llama_index/indices/empty/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/empty/retrievers.py` & `llama_index-0.6.7/llama_index/indices/empty/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/keyword_table/__init__.py` & `llama_index-0.6.7/llama_index/indices/keyword_table/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/keyword_table/base.py` & `llama_index-0.6.7/llama_index/indices/keyword_table/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/keyword_table/rake_base.py` & `llama_index-0.6.7/llama_index/indices/keyword_table/rake_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/keyword_table/retrievers.py` & `llama_index-0.6.7/llama_index/indices/keyword_table/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/keyword_table/simple_base.py` & `llama_index-0.6.7/llama_index/indices/keyword_table/simple_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/keyword_table/utils.py` & `llama_index-0.6.7/llama_index/indices/keyword_table/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/knowledge_graph/base.py` & `llama_index-0.6.7/llama_index/indices/knowledge_graph/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/knowledge_graph/retrievers.py` & `llama_index-0.6.7/llama_index/indices/knowledge_graph/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/list/base.py` & `llama_index-0.6.7/llama_index/indices/list/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.service_context import ServiceContext
 
 
 class ListRetrieverMode(str, Enum):
     DEFAULT = "default"
     EMBEDDING = "embedding"
+    LLM = "llm"
 
 
 class GPTListIndex(BaseGPTIndex[IndexList]):
     """GPT List Index.
 
     The list index is a simple data structure where nodes are stored in
     a sequence. During index construction, the document texts are
@@ -59,20 +60,23 @@
         self,
         retriever_mode: Union[str, ListRetrieverMode] = ListRetrieverMode.DEFAULT,
         **kwargs: Any,
     ) -> BaseRetriever:
         from llama_index.indices.list.retrievers import (
             ListIndexEmbeddingRetriever,
             ListIndexRetriever,
+            ListIndexLLMRetriever,
         )
 
         if retriever_mode == ListRetrieverMode.DEFAULT:
             return ListIndexRetriever(self, **kwargs)
         elif retriever_mode == ListRetrieverMode.EMBEDDING:
             return ListIndexEmbeddingRetriever(self, **kwargs)
+        elif retriever_mode == ListRetrieverMode.LLM:
+            return ListIndexLLMRetriever(self, **kwargs)
         else:
             raise ValueError(f"Unknown retriever mode: {retriever_mode}")
 
     def _build_index_from_nodes(self, nodes: Sequence[Node]) -> IndexList:
         """Build the index from documents.
 
         Args:
```

### Comparing `llama_index-0.6.6/llama_index/indices/loading.py` & `llama_index-0.6.7/llama_index/indices/loading.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/postprocessor/__init__.py` & `llama_index-0.6.7/llama_index/indices/postprocessor/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,22 +12,24 @@
     EmbeddingRecencyPostprocessor,
     TimeWeightedPostprocessor,
 )
 from llama_index.indices.postprocessor.pii import (
     PIINodePostprocessor,
     NERPIINodePostprocessor,
 )
+from llama_index.indices.postprocessor.llm_rerank import LLMRerank
 
 from llama_index.indices.postprocessor.cohere_rerank import CohereRerank
 
 __all__ = [
     "SimilarityPostprocessor",
     "KeywordNodePostprocessor",
     "PrevNextNodePostprocessor",
     "AutoPrevNextNodePostprocessor",
     "FixedRecencyPostprocessor",
     "EmbeddingRecencyPostprocessor",
     "TimeWeightedPostprocessor",
     "PIINodePostprocessor",
     "NERPIINodePostprocessor",
     "CohereRerank",
+    "LLMRerank",
 ]
```

### Comparing `llama_index-0.6.6/llama_index/indices/postprocessor/cohere_rerank.py` & `llama_index-0.6.7/llama_index/indices/postprocessor/cohere_rerank.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/postprocessor/node.py` & `llama_index-0.6.7/llama_index/indices/postprocessor/node.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/postprocessor/node_recency.py` & `llama_index-0.6.7/llama_index/indices/postprocessor/node_recency.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/postprocessor/pii.py` & `llama_index-0.6.7/llama_index/indices/postprocessor/pii.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/prompt_helper.py` & `llama_index-0.6.7/llama_index/indices/prompt_helper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/query/base.py` & `llama_index-0.6.7/llama_index/indices/query/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/query/embedding_utils.py` & `llama_index-0.6.7/llama_index/indices/query/embedding_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/query/query_transform/base.py` & `llama_index-0.6.7/llama_index/indices/query/query_transform/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/query/query_transform/prompts.py` & `llama_index-0.6.7/llama_index/indices/query/query_transform/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/query/response_synthesis.py` & `llama_index-0.6.7/llama_index/indices/query/response_synthesis.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/query/schema.py` & `llama_index-0.6.7/llama_index/indices/query/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/registry.py` & `llama_index-0.6.7/llama_index/indices/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/response/response_builder.py` & `llama_index-0.6.7/llama_index/indices/response/response_builder.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/service_context.py` & `llama_index-0.6.7/llama_index/indices/service_context.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/struct_store/__init__.py` & `llama_index-0.6.7/llama_index/indices/struct_store/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/struct_store/base.py` & `llama_index-0.6.7/llama_index/indices/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/struct_store/container_builder.py` & `llama_index-0.6.7/llama_index/indices/struct_store/container_builder.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/struct_store/pandas.py` & `llama_index-0.6.7/llama_index/indices/struct_store/pandas.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/struct_store/pandas_query.py` & `llama_index-0.6.7/llama_index/indices/struct_store/pandas_query.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/struct_store/sql.py` & `llama_index-0.6.7/llama_index/indices/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/struct_store/sql_query.py` & `llama_index-0.6.7/llama_index/indices/struct_store/sql_query.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/tree/__init__.py` & `llama_index-0.6.7/llama_index/indices/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/tree/all_leaf_retriever.py` & `llama_index-0.6.7/llama_index/indices/tree/all_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/tree/base.py` & `llama_index-0.6.7/llama_index/indices/tree/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/tree/inserter.py` & `llama_index-0.6.7/llama_index/indices/tree/inserter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/tree/select_leaf_embedding_retriever.py` & `llama_index-0.6.7/llama_index/indices/tree/select_leaf_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/tree/select_leaf_retriever.py` & `llama_index-0.6.7/llama_index/indices/tree/select_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/tree/tree_root_retriever.py` & `llama_index-0.6.7/llama_index/indices/tree/tree_root_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/utils.py` & `llama_index-0.6.7/llama_index/indices/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Utilities for GPT indices."""
 import logging
 import re
-from typing import Dict, List, Optional, Set
+from typing import Dict, List, Optional, Set, Tuple
 
 from llama_index.data_structs.node import Node
 from llama_index.utils import globals_helper, truncate_text
 from llama_index.vector_stores.types import VectorStoreQueryResult
 
 _logger = logging.getLogger(__name__)
 
@@ -54,7 +54,48 @@
     fmt_txts = []
     for node_idx, node_similarity, node in zip(result.ids, similarities, result.nodes):
         fmt_txt = f"> [Node {node_idx}] [Similarity score: \
             {float(node_similarity):.6}] {truncate_text(node.get_text(), 100)}"
         fmt_txts.append(fmt_txt)
     top_k_node_text = "\n".join(fmt_txts)
     logger.debug(f"> Top {len(result.nodes)} nodes:\n{top_k_node_text}")
+
+
+def default_format_node_batch_fn(
+    summary_nodes: List[Node],
+) -> str:
+    """Default format node batch function.
+
+    Assign each summary node a number, and format the batch of nodes.
+
+    """
+    fmt_node_txts = []
+    for idx in range(len(summary_nodes)):
+        number = idx + 1
+        fmt_node_txts.append(f"Document {number}:\n{summary_nodes[idx].get_text()}")
+    return "\n\n".join(fmt_node_txts)
+
+
+def default_parse_choice_select_answer_fn(
+    answer: str, num_choices: int, raise_error: bool = False
+) -> Tuple[List[int], Optional[List[float]]]:
+    """Default parse choice select answer function."""
+    answer_lines = answer.split("\n")
+    answer_nums = []
+    answer_relevances = []
+    for answer_line in answer_lines:
+        line_tokens = answer_line.split(",")
+        if len(line_tokens) != 2:
+            if not raise_error:
+                continue
+            else:
+                raise ValueError(
+                    f"Invalid answer line: {answer_line}. "
+                    "Answer line must be of the form: "
+                    "answer_num: <int>, answer_relevance: <float>"
+                )
+        answer_num = int(line_tokens[0].split(":")[1].strip())
+        if answer_num > num_choices:
+            continue
+        answer_nums.append(answer_num)
+        answer_relevances.append(float(line_tokens[1].split(":")[1].strip()))
+    return answer_nums, answer_relevances
```

### Comparing `llama_index-0.6.6/llama_index/indices/vector_store/base.py` & `llama_index-0.6.7/llama_index/indices/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py` & `llama_index-0.6.7/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py` & `llama_index-0.6.7/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py` & `llama_index-0.6.7/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,25 @@
+"""Autoretriever prompts."""
+
 from typing import List
 
 from llama_index.prompts.base import Prompt
 from llama_index.prompts.prompt_type import PromptType
 from llama_index.vector_stores.types import (
     ExactMatchFilter,
     MetadataInfo,
     VectorStoreInfo,
     VectorStoreQuerySpec,
 )
 
+# NOTE: these prompts are inspired from langchain's self-query prompt,
+# and adapted to our use case.
+# https://github.com/hwchase17/langchain/tree/main/langchain/chains/query_constructor/prompt.py
+
+
 PREFIX = """\
 Your goal is to structure the user's query to match the request schema provided below.
 
 << Structured Request Schema >>
 When responding use a markdown code snippet with a JSON object formatted in the \
 following schema:
```

### Comparing `llama_index-0.6.6/llama_index/indices/vector_store/retrievers/retriever.py` & `llama_index-0.6.7/llama_index/indices/vector_store/retrievers/retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/langchain_helpers/agents/__init__.py` & `llama_index-0.6.7/llama_index/langchain_helpers/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/langchain_helpers/agents/agents.py` & `llama_index-0.6.7/llama_index/langchain_helpers/agents/agents.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/langchain_helpers/agents/toolkits.py` & `llama_index-0.6.7/llama_index/langchain_helpers/agents/toolkits.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/langchain_helpers/agents/tools.py` & `llama_index-0.6.7/llama_index/langchain_helpers/agents/tools.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/langchain_helpers/memory_wrapper.py` & `llama_index-0.6.7/llama_index/langchain_helpers/memory_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/langchain_helpers/sql_wrapper.py` & `llama_index-0.6.7/llama_index/langchain_helpers/sql_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/langchain_helpers/streaming.py` & `llama_index-0.6.7/llama_index/langchain_helpers/streaming.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/langchain_helpers/text_splitter.py` & `llama_index-0.6.7/llama_index/langchain_helpers/text_splitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/llm_predictor/base.py` & `llama_index-0.6.7/llama_index/llm_predictor/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/llm_predictor/chatgpt.py` & `llama_index-0.6.7/llama_index/llm_predictor/chatgpt.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/llm_predictor/huggingface.py` & `llama_index-0.6.7/llama_index/llm_predictor/huggingface.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/llm_predictor/structured.py` & `llama_index-0.6.7/llama_index/llm_predictor/structured.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/logger/base.py` & `llama_index-0.6.7/llama_index/logger/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/node_parser/interface.py` & `llama_index-0.6.7/llama_index/node_parser/interface.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/node_parser/node_utils.py` & `llama_index-0.6.7/llama_index/node_parser/node_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/node_parser/simple.py` & `llama_index-0.6.7/llama_index/node_parser/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/optimization/optimizer.py` & `llama_index-0.6.7/llama_index/optimization/optimizer.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/output_parsers/base.py` & `llama_index-0.6.7/llama_index/output_parsers/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/output_parsers/guardrails.py` & `llama_index-0.6.7/llama_index/output_parsers/guardrails.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/output_parsers/langchain.py` & `llama_index-0.6.7/llama_index/output_parsers/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/output_parsers/selection.py` & `llama_index-0.6.7/llama_index/output_parsers/selection.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/playground/base.py` & `llama_index-0.6.7/llama_index/playground/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/prompts/base.py` & `llama_index-0.6.7/llama_index/prompts/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/prompts/chat_prompts.py` & `llama_index-0.6.7/llama_index/prompts/chat_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/prompts/default_prompt_selectors.py` & `llama_index-0.6.7/llama_index/prompts/default_prompt_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/prompts/default_prompts.py` & `llama_index-0.6.7/llama_index/prompts/default_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/prompts/prompt_type.py` & `llama_index-0.6.7/llama_index/prompts/prompt_type.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/prompts/prompts.py` & `llama_index-0.6.7/llama_index/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/query_engine/__init__.py` & `llama_index-0.6.7/llama_index/query_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/query_engine/graph_query_engine.py` & `llama_index-0.6.7/llama_index/query_engine/graph_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/query_engine/multistep_query_engine.py` & `llama_index-0.6.7/llama_index/query_engine/multistep_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/query_engine/retriever_query_engine.py` & `llama_index-0.6.7/llama_index/query_engine/retriever_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/query_engine/router_query_engine.py` & `llama_index-0.6.7/llama_index/query_engine/router_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/query_engine/transform_query_engine.py` & `llama_index-0.6.7/llama_index/query_engine/transform_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/__init__.py` & `llama_index-0.6.7/llama_index/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/base.py` & `llama_index-0.6.7/llama_index/readers/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/chatgpt_plugin/base.py` & `llama_index-0.6.7/llama_index/readers/chatgpt_plugin/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/chroma.py` & `llama_index-0.6.7/llama_index/readers/chroma.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/database.py` & `llama_index-0.6.7/llama_index/readers/database.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/deeplake.py` & `llama_index-0.6.7/llama_index/readers/deeplake.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/discord_reader.py` & `llama_index-0.6.7/llama_index/readers/discord_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/download.py` & `llama_index-0.6.7/llama_index/readers/download.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/elasticsearch.py` & `llama_index-0.6.7/llama_index/readers/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/faiss.py` & `llama_index-0.6.7/llama_index/readers/faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/file/base.py` & `llama_index-0.6.7/llama_index/readers/file/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/file/base_parser.py` & `llama_index-0.6.7/llama_index/readers/file/base_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/file/docs_parser.py` & `llama_index-0.6.7/llama_index/readers/file/docs_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/file/epub_parser.py` & `llama_index-0.6.7/llama_index/readers/file/epub_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/file/image_caption_parser.py` & `llama_index-0.6.7/llama_index/readers/file/image_caption_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/file/image_parser.py` & `llama_index-0.6.7/llama_index/readers/file/image_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/file/image_vision_llm_parser.py` & `llama_index-0.6.7/llama_index/readers/file/image_vision_llm_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/file/ipynb_parser.py` & `llama_index-0.6.7/llama_index/readers/file/ipynb_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/file/markdown_parser.py` & `llama_index-0.6.7/llama_index/readers/file/markdown_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/file/mbox_parser.py` & `llama_index-0.6.7/llama_index/readers/file/mbox_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/file/slides_parser.py` & `llama_index-0.6.7/llama_index/readers/file/slides_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/file/tabular_parser.py` & `llama_index-0.6.7/llama_index/readers/file/tabular_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/file/video_audio.py` & `llama_index-0.6.7/llama_index/readers/file/video_audio.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/github_readers/github_api_client.py` & `llama_index-0.6.7/llama_index/readers/github_readers/github_api_client.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/github_readers/github_repository_reader.py` & `llama_index-0.6.7/llama_index/readers/github_readers/github_repository_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/github_readers/utils.py` & `llama_index-0.6.7/llama_index/readers/github_readers/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/google_readers/gdocs.py` & `llama_index-0.6.7/llama_index/readers/google_readers/gdocs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/google_readers/gsheets.py` & `llama_index-0.6.7/llama_index/readers/google_readers/gsheets.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/json.py` & `llama_index-0.6.7/llama_index/readers/json.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/make_com/wrapper.py` & `llama_index-0.6.7/llama_index/readers/make_com/wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/mbox.py` & `llama_index-0.6.7/llama_index/readers/mbox.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/metal.py` & `llama_index-0.6.7/llama_index/readers/metal.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/milvus.py` & `llama_index-0.6.7/llama_index/readers/milvus.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/mongo.py` & `llama_index-0.6.7/llama_index/readers/mongo.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/myscale.py` & `llama_index-0.6.7/llama_index/readers/myscale.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/notion.py` & `llama_index-0.6.7/llama_index/readers/notion.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/obsidian.py` & `llama_index-0.6.7/llama_index/readers/obsidian.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/pinecone.py` & `llama_index-0.6.7/llama_index/readers/pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/qdrant.py` & `llama_index-0.6.7/llama_index/readers/qdrant.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/redis/utils.py` & `llama_index-0.6.7/llama_index/readers/redis/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/schema/base.py` & `llama_index-0.6.7/llama_index/readers/schema/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/slack.py` & `llama_index-0.6.7/llama_index/readers/slack.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/steamship/file_reader.py` & `llama_index-0.6.7/llama_index/readers/steamship/file_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/string_iterable.py` & `llama_index-0.6.7/llama_index/readers/string_iterable.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/twitter.py` & `llama_index-0.6.7/llama_index/readers/twitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/weaviate/client.py` & `llama_index-0.6.7/llama_index/readers/weaviate/client.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/weaviate/reader.py` & `llama_index-0.6.7/llama_index/readers/weaviate/reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/weaviate/utils.py` & `llama_index-0.6.7/llama_index/readers/weaviate/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/web.py` & `llama_index-0.6.7/llama_index/readers/web.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/wikipedia.py` & `llama_index-0.6.7/llama_index/readers/wikipedia.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/readers/youtube_transcript.py` & `llama_index-0.6.7/llama_index/readers/youtube_transcript.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/response/notebook_utils.py` & `llama_index-0.6.7/llama_index/response/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/response/pprint_utils.py` & `llama_index-0.6.7/llama_index/response/pprint_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/response/schema.py` & `llama_index-0.6.7/llama_index/response/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/retrievers/__init__.py` & `llama_index-0.6.7/llama_index/retrievers/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/retrievers/transform_retriever.py` & `llama_index-0.6.7/llama_index/retrievers/transform_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/schema.py` & `llama_index-0.6.7/llama_index/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/selectors/llm_selectors.py` & `llama_index-0.6.7/llama_index/selectors/llm_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/selectors/prompts.py` & `llama_index-0.6.7/llama_index/selectors/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/selectors/types.py` & `llama_index-0.6.7/llama_index/selectors/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/storage/docstore/__init__.py` & `llama_index-0.6.7/llama_index/storage/docstore/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/storage/docstore/keyval_docstore.py` & `llama_index-0.6.7/llama_index/storage/docstore/keyval_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/storage/docstore/mongo_docstore.py` & `llama_index-0.6.7/llama_index/storage/docstore/mongo_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/storage/docstore/registry.py` & `llama_index-0.6.7/llama_index/storage/docstore/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/storage/docstore/simple_docstore.py` & `llama_index-0.6.7/llama_index/storage/docstore/simple_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/storage/docstore/types.py` & `llama_index-0.6.7/llama_index/storage/docstore/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/storage/docstore/utils.py` & `llama_index-0.6.7/llama_index/storage/docstore/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/storage/index_store/keyval_index_store.py` & `llama_index-0.6.7/llama_index/storage/index_store/keyval_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/storage/index_store/mongo_index_store.py` & `llama_index-0.6.7/llama_index/storage/index_store/mongo_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/storage/index_store/simple_index_store.py` & `llama_index-0.6.7/llama_index/storage/index_store/simple_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/storage/index_store/types.py` & `llama_index-0.6.7/llama_index/storage/index_store/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/storage/index_store/utils.py` & `llama_index-0.6.7/llama_index/storage/index_store/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/storage/kvstore/mongodb_kvstore.py` & `llama_index-0.6.7/llama_index/storage/kvstore/mongodb_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/storage/kvstore/simple_kvstore.py` & `llama_index-0.6.7/llama_index/storage/kvstore/simple_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/storage/kvstore/types.py` & `llama_index-0.6.7/llama_index/storage/kvstore/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/storage/storage_context.py` & `llama_index-0.6.7/llama_index/storage/storage_context.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/token_counter/mock_chain_wrapper.py` & `llama_index-0.6.7/llama_index/token_counter/mock_chain_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/token_counter/mock_embed_model.py` & `llama_index-0.6.7/llama_index/token_counter/mock_embed_model.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/token_counter/token_counter.py` & `llama_index-0.6.7/llama_index/token_counter/token_counter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/token_counter/utils.py` & `llama_index-0.6.7/llama_index/token_counter/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/tools/query_engine.py` & `llama_index-0.6.7/llama_index/tools/query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/tts/bark.py` & `llama_index-0.6.7/llama_index/tts/bark.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/tts/base.py` & `llama_index-0.6.7/llama_index/tts/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/tts/elevenlabs.py` & `llama_index-0.6.7/llama_index/tts/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/utils.py` & `llama_index-0.6.7/llama_index/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/vector_stores/__init__.py` & `llama_index-0.6.7/llama_index/vector_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/vector_stores/chatgpt_plugin.py` & `llama_index-0.6.7/llama_index/vector_stores/chatgpt_plugin.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/vector_stores/chroma.py` & `llama_index-0.6.7/llama_index/vector_stores/chroma.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/vector_stores/deeplake.py` & `llama_index-0.6.7/llama_index/vector_stores/deeplake.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/vector_stores/faiss.py` & `llama_index-0.6.7/llama_index/vector_stores/faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/vector_stores/lancedb.py` & `llama_index-0.6.7/llama_index/vector_stores/lancedb.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/vector_stores/metal.py` & `llama_index-0.6.7/llama_index/vector_stores/metal.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/vector_stores/milvus.py` & `llama_index-0.6.7/llama_index/vector_stores/milvus.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/vector_stores/myscale.py` & `llama_index-0.6.7/llama_index/vector_stores/myscale.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/vector_stores/opensearch.py` & `llama_index-0.6.7/llama_index/vector_stores/opensearch.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/vector_stores/pinecone.py` & `llama_index-0.6.7/llama_index/vector_stores/pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/vector_stores/qdrant.py` & `llama_index-0.6.7/llama_index/vector_stores/qdrant.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/vector_stores/redis.py` & `llama_index-0.6.7/llama_index/vector_stores/redis.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,14 +199,18 @@
             ValueError: If query.query_embedding is None.
             redis.exceptions.RedisError: If there is an error querying the index.
             redis.exceptions.TimeoutError: If there is a timeout querying the index.
         """
         from redis.exceptions import RedisError
         from redis.exceptions import TimeoutError as RedisTimeoutError
 
+        # TODO: implement this
+        if query.filters is not None:
+            raise ValueError("Metadata filters not implemented for Redis yet.")
+
         return_fields = ["id", "doc_id", "text", self._vector_key, "vector_score"]
 
         redis_query = get_redis_query(
             return_fields=return_fields,
             top_k=query.similarity_top_k,
             vector_field=self._vector_field,
         )
```

### Comparing `llama_index-0.6.6/llama_index/vector_stores/registry.py` & `llama_index-0.6.7/llama_index/vector_stores/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/vector_stores/simple.py` & `llama_index-0.6.7/llama_index/vector_stores/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/vector_stores/types.py` & `llama_index-0.6.7/llama_index/vector_stores/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/vector_stores/utils.py` & `llama_index-0.6.7/llama_index/vector_stores/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index/vector_stores/weaviate.py` & `llama_index-0.6.7/llama_index/vector_stores/weaviate.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/llama_index.egg-info/PKG-INFO` & `llama_index-0.6.7/llama_index.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index
-Version: 0.6.6
+Version: 0.6.7
 Summary: Interface between LLMs and your data
 Home-page: https://github.com/jerryjliu/llama_index
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🗂️ LlamaIndex 🦙
```

### Comparing `llama_index-0.6.6/llama_index.egg-info/SOURCES.txt` & `llama_index-0.6.7/llama_index.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 llama_index/utils.py
 llama_index.egg-info/PKG-INFO
 llama_index.egg-info/SOURCES.txt
 llama_index.egg-info/dependency_links.txt
 llama_index.egg-info/requires.txt
 llama_index.egg-info/top_level.txt
 llama_index/callbacks/__init__.py
+llama_index/callbacks/aim.py
 llama_index/callbacks/base.py
 llama_index/callbacks/llama_debug.py
 llama_index/callbacks/schema.py
 llama_index/composability/__init__.py
 llama_index/composability/base.py
 llama_index/composability/joint_qa_summary.py
 llama_index/data_structs/__init__.py
@@ -73,14 +74,15 @@
 llama_index/indices/knowledge_graph/base.py
 llama_index/indices/knowledge_graph/retrievers.py
 llama_index/indices/list/__init__.py
 llama_index/indices/list/base.py
 llama_index/indices/list/retrievers.py
 llama_index/indices/postprocessor/__init__.py
 llama_index/indices/postprocessor/cohere_rerank.py
+llama_index/indices/postprocessor/llm_rerank.py
 llama_index/indices/postprocessor/node.py
 llama_index/indices/postprocessor/node_recency.py
 llama_index/indices/postprocessor/pii.py
 llama_index/indices/postprocessor/types.py
 llama_index/indices/query/__init__.py
 llama_index/indices/query/base.py
 llama_index/indices/query/embedding_utils.py
@@ -143,14 +145,16 @@
 llama_index/output_parsers/langchain.py
 llama_index/output_parsers/selection.py
 llama_index/playground/__init__.py
 llama_index/playground/base.py
 llama_index/prompts/__init__.py
 llama_index/prompts/base.py
 llama_index/prompts/chat_prompts.py
+llama_index/prompts/choice_select.py
+llama_index/prompts/default_choice_select.py
 llama_index/prompts/default_prompt_selectors.py
 llama_index/prompts/default_prompts.py
 llama_index/prompts/prompt_type.py
 llama_index/prompts/prompts.py
 llama_index/query_engine/__init__.py
 llama_index/query_engine/graph_query_engine.py
 llama_index/query_engine/multistep_query_engine.py
@@ -307,14 +311,15 @@
 tests/indices/knowledge_graph/test_base.py
 tests/indices/knowledge_graph/test_retrievers.py
 tests/indices/list/__init__.py
 tests/indices/list/test_index.py
 tests/indices/list/test_retrievers.py
 tests/indices/postprocessor/__init__.py
 tests/indices/postprocessor/test_base.py
+tests/indices/postprocessor/test_llm_rerank.py
 tests/indices/query/__init__.py
 tests/indices/query/conftest.py
 tests/indices/query/test_compose.py
 tests/indices/query/test_compose_vector.py
 tests/indices/query/test_query_bundle.py
 tests/indices/query/query_transform/__init__.py
 tests/indices/query/query_transform/mock_utils.py
```

### Comparing `llama_index-0.6.6/setup.py` & `llama_index-0.6.7/setup.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/callbacks/test_llama_debug.py` & `llama_index-0.6.7/tests/callbacks/test_llama_debug.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/conftest.py` & `llama_index-0.6.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/embeddings/test_base.py` & `llama_index-0.6.7/tests/embeddings/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/composability/test_utils.py` & `llama_index-0.6.7/tests/indices/composability/test_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/conftest.py` & `llama_index-0.6.7/tests/indices/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/document_summary/test_index.py` & `llama_index-0.6.7/tests/indices/document_summary/test_index.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/empty/test_base.py` & `llama_index-0.6.7/tests/indices/empty/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/keyword_table/test_base.py` & `llama_index-0.6.7/tests/indices/keyword_table/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/keyword_table/test_retrievers.py` & `llama_index-0.6.7/tests/indices/keyword_table/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/keyword_table/test_utils.py` & `llama_index-0.6.7/tests/indices/keyword_table/test_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/knowledge_graph/test_base.py` & `llama_index-0.6.7/tests/indices/knowledge_graph/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/knowledge_graph/test_retrievers.py` & `llama_index-0.6.7/tests/indices/knowledge_graph/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/list/test_index.py` & `llama_index-0.6.7/tests/indices/list/test_index.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/postprocessor/test_base.py` & `llama_index-0.6.7/tests/indices/postprocessor/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/query/conftest.py` & `llama_index-0.6.7/tests/indices/query/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/query/query_transform/test_base.py` & `llama_index-0.6.7/tests/indices/query/query_transform/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/query/test_compose.py` & `llama_index-0.6.7/tests/indices/query/test_compose.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/query/test_compose_vector.py` & `llama_index-0.6.7/tests/indices/query/test_compose_vector.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/query/test_query_bundle.py` & `llama_index-0.6.7/tests/indices/query/test_query_bundle.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/struct_store/conftest.py` & `llama_index-0.6.7/tests/indices/struct_store/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/struct_store/test_base.py` & `llama_index-0.6.7/tests/indices/struct_store/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/struct_store/test_pandas.py` & `llama_index-0.6.7/tests/indices/struct_store/test_pandas.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/struct_store/test_sql_query.py` & `llama_index-0.6.7/tests/indices/struct_store/test_sql_query.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/test_loading.py` & `llama_index-0.6.7/tests/indices/test_loading.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/test_loading_graph.py` & `llama_index-0.6.7/tests/indices/test_loading_graph.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/test_node_utils.py` & `llama_index-0.6.7/tests/indices/test_node_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/test_prompt_helper.py` & `llama_index-0.6.7/tests/indices/test_prompt_helper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/tree/conftest.py` & `llama_index-0.6.7/tests/indices/tree/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/tree/test_embedding_retriever.py` & `llama_index-0.6.7/tests/indices/tree/test_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/tree/test_index.py` & `llama_index-0.6.7/tests/indices/tree/test_index.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/tree/test_retrievers.py` & `llama_index-0.6.7/tests/indices/tree/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/vector_store/auto_retriever/test_output_parser.py` & `llama_index-0.6.7/tests/indices/vector_store/auto_retriever/test_output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/vector_store/conftest.py` & `llama_index-0.6.7/tests/indices/vector_store/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/vector_store/mock_faiss.py` & `llama_index-0.6.7/tests/indices/vector_store/mock_faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/vector_store/mock_services.py` & `llama_index-0.6.7/tests/indices/vector_store/mock_services.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/vector_store/test_faiss.py` & `llama_index-0.6.7/tests/indices/vector_store/test_faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/vector_store/test_myscale.py` & `llama_index-0.6.7/tests/indices/vector_store/test_myscale.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/vector_store/test_pinecone.py` & `llama_index-0.6.7/tests/indices/vector_store/test_pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/vector_store/test_retrievers.py` & `llama_index-0.6.7/tests/indices/vector_store/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/vector_store/test_simple.py` & `llama_index-0.6.7/tests/indices/vector_store/test_simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/indices/vector_store/utils.py` & `llama_index-0.6.7/tests/indices/vector_store/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/langchain_helpers/test_text_splitter.py` & `llama_index-0.6.7/tests/langchain_helpers/test_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/llm_predictor/test_base.py` & `llama_index-0.6.7/tests/llm_predictor/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/logger/test_base.py` & `llama_index-0.6.7/tests/logger/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/mock_utils/mock_predict.py` & `llama_index-0.6.7/tests/mock_utils/mock_predict.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import json
 from typing import Any, Dict, Tuple
 
 from llama_index.indices.query.query_transform.prompts import (
     DecomposeQueryTransformPrompt,
 )
 from llama_index.prompts.base import Prompt
+from llama_index.prompts.choice_select import ChoiceSelectPrompt
 from llama_index.prompts.prompt_type import PromptType
 from llama_index.token_counter.utils import mock_extract_keywords_response
 
 
 def _mock_summary_predict(prompt_args: Dict) -> str:
     """Mock summary predict."""
     return prompt_args["context_str"]
@@ -121,14 +122,19 @@
 
 def _mock_pandas(prompt_args: Dict) -> str:
     """Mock pandas prompt."""
     query_str = prompt_args["query_str"]
     return f'df["{query_str}"].iloc[0]'
 
 
+def _mock_choice_select(prompt_args: Dict) -> str:
+    """Mock choice select prompt."""
+    return "Doc: 1, Relevance: 5"
+
+
 def mock_llmpredictor_predict(prompt: Prompt, **prompt_args: Any) -> Tuple[str, str]:
     """Mock predict method of LLMPredictor.
 
     Depending on the prompt, return response.
 
     """
     formatted_prompt = prompt.format(**prompt_args)
@@ -158,14 +164,16 @@
     elif prompt.prompt_type == PromptType.SINGLE_SELECT:
         response = _mock_single_select()
     elif prompt.prompt_type == PromptType.MULTI_SELECT:
         response = _mock_multi_select(full_prompt_args)
     elif prompt.prompt_type == PromptType.CUSTOM:
         if isinstance(prompt, DecomposeQueryTransformPrompt):
             response = _mock_decompose_query(full_prompt_args)
+        elif isinstance(prompt, ChoiceSelectPrompt):
+            response = _mock_choice_select(full_prompt_args)
         else:
             raise ValueError("Invalid prompt to use with mocks.")
     elif prompt.prompt_type == PromptType.PANDAS:
         response = _mock_pandas(full_prompt_args)
     else:
         raise ValueError("Invalid prompt to use with mocks.")
 
@@ -209,14 +217,16 @@
     elif prompt.prompt_type == PromptType.SINGLE_SELECT:
         response = _mock_single_select()
     elif prompt.prompt_type == PromptType.MULTI_SELECT:
         response = _mock_multi_select(full_prompt_args)
     elif prompt.prompt_type == PromptType.CUSTOM:
         if isinstance(prompt, DecomposeQueryTransformPrompt):
             response = _mock_decompose_query(full_prompt_args)
+        elif isinstance(prompt, ChoiceSelectPrompt):
+            response = _mock_choice_select(full_prompt_args)
         else:
             raise ValueError("Invalid prompt to use with mocks.")
     elif prompt.prompt_type == PromptType.PANDAS:
         response = _mock_pandas(full_prompt_args)
     else:
         raise ValueError("Invalid prompt to use with mocks.")
```

### Comparing `llama_index-0.6.6/tests/mock_utils/mock_prompts.py` & `llama_index-0.6.7/tests/mock_utils/mock_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/mock_utils/mock_text_splitter.py` & `llama_index-0.6.7/tests/mock_utils/mock_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/mock_utils/mock_utils.py` & `llama_index-0.6.7/tests/mock_utils/mock_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/optimization/test_base.py` & `llama_index-0.6.7/tests/optimization/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/output_parsers/test_base.py` & `llama_index-0.6.7/tests/output_parsers/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/output_parsers/test_selection.py` & `llama_index-0.6.7/tests/output_parsers/test_selection.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/playground/test_base.py` & `llama_index-0.6.7/tests/playground/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/prompts/test_base.py` & `llama_index-0.6.7/tests/prompts/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/readers/test_file.py` & `llama_index-0.6.7/tests/readers/test_file.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/readers/test_json.py` & `llama_index-0.6.7/tests/readers/test_json.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/readers/test_mongo.py` & `llama_index-0.6.7/tests/readers/test_mongo.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/selectors/test_llm_selectors.py` & `llama_index-0.6.7/tests/selectors/test_llm_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/storage/conftest.py` & `llama_index-0.6.7/tests/storage/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/storage/docstore/test_mongo_docstore.py` & `llama_index-0.6.7/tests/storage/docstore/test_mongo_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/storage/docstore/test_simple_docstore.py` & `llama_index-0.6.7/tests/storage/docstore/test_simple_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/storage/test_storage_context.py` & `llama_index-0.6.7/tests/storage/test_storage_context.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/test_utils.py` & `llama_index-0.6.7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/token_predictor/test_base.py` & `llama_index-0.6.7/tests/token_predictor/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/vector_stores/test_qdrant.py` & `llama_index-0.6.7/tests/vector_stores/test_qdrant.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.6/tests/vector_stores/test_weaviate.py` & `llama_index-0.6.7/tests/vector_stores/test_weaviate.py`

 * *Files identical despite different names*

