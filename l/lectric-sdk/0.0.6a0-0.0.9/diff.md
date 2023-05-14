# Comparing `tmp/lectric-sdk-0.0.6a0.tar.gz` & `tmp/lectric-sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lectric-sdk-0.0.6a0.tar", last modified: Thu Jan  5 00:15:43 2023, max compression
+gzip compressed data, was "lectric-sdk-0.0.9.tar", last modified: Fri Apr 21 17:18:52 2023, max compression
```

## Comparing `lectric-sdk-0.0.6a0.tar` & `lectric-sdk-0.0.9.tar`

### file list

```diff
@@ -1,82 +1,97 @@
-drwxrwxrwx   0        0        0        0 2023-01-05 00:15:43.313644 lectric-sdk-0.0.6a0/
--rw-rw-rw-   0        0        0      125 2023-01-04 23:50:40.000000 lectric-sdk-0.0.6a0/MANIFEST.in
--rw-rw-rw-   0        0        0     3017 2023-01-05 00:15:43.312636 lectric-sdk-0.0.6a0/PKG-INFO
--rw-rw-rw-   0        0        0     2705 2022-08-31 19:45:15.000000 lectric-sdk-0.0.6a0/README.md
-drwxrwxrwx   0        0        0        0 2023-01-05 00:15:43.068637 lectric-sdk-0.0.6a0/lectric/
--rw-rw-rw-   0        0        0        9 2023-01-05 00:12:43.000000 lectric-sdk-0.0.6a0/lectric/VERSION
--rw-rw-rw-   0        0        0      432 2023-01-04 23:39:55.000000 lectric-sdk-0.0.6a0/lectric/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-05 00:15:43.073637 lectric-sdk-0.0.6a0/lectric/api/
--rw-rw-rw-   0        0        0       47 2022-12-08 06:14:10.000000 lectric-sdk-0.0.6a0/lectric/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-05 00:15:43.104642 lectric-sdk-0.0.6a0/lectric/api/collection/
--rw-rw-rw-   0        0        0        0 2022-12-08 06:14:10.000000 lectric-sdk-0.0.6a0/lectric/api/collection/__init__.py
--rw-rw-rw-   0        0        0     3931 2022-12-08 06:14:10.000000 lectric-sdk-0.0.6a0/lectric/api/collection/create_collection_collection_create_post.py
--rw-rw-rw-   0        0        0     4229 2022-12-12 20:03:18.000000 lectric-sdk-0.0.6a0/lectric/api/collection/delete_entities_collection_entities_delete.py
--rw-rw-rw-   0        0        0     3540 2022-12-08 06:14:10.000000 lectric-sdk-0.0.6a0/lectric/api/collection/drop_collection_collection_delete.py
--rw-rw-rw-   0        0        0     3388 2022-12-08 06:14:10.000000 lectric-sdk-0.0.6a0/lectric/api/collection/exists_collection_collection_exists_name_get.py
--rw-rw-rw-   0        0        0     3459 2022-12-08 06:14:10.000000 lectric-sdk-0.0.6a0/lectric/api/collection/get_collection_collection_get_name_get.py
--rw-rw-rw-   0        0        0     3545 2022-12-08 06:14:10.000000 lectric-sdk-0.0.6a0/lectric/api/collection/get_indexes_collection_indexes_name_get.py
--rw-rw-rw-   0        0        0     3396 2022-12-08 06:14:10.000000 lectric-sdk-0.0.6a0/lectric/api/collection/is_empty_collection_collection_empty_name_get.py
--rw-rw-rw-   0        0        0     2698 2022-12-08 06:14:10.000000 lectric-sdk-0.0.6a0/lectric/api/collection/list_collections_collection_list_get.py
--rw-rw-rw-   0        0        0     3448 2022-12-08 06:14:10.000000 lectric-sdk-0.0.6a0/lectric/api/collection/sizeof_collection_collection_size_name_get.py
-drwxrwxrwx   0        0        0        0 2023-01-05 00:15:43.117640 lectric-sdk-0.0.6a0/lectric/api/default/
--rw-rw-rw-   0        0        0        0 2022-12-08 06:14:10.000000 lectric-sdk-0.0.6a0/lectric/api/default/__init__.py
--rw-rw-rw-   0        0        0     2461 2022-12-08 06:14:10.000000 lectric-sdk-0.0.6a0/lectric/api/default/list_connections_connections_get.py
--rw-rw-rw-   0        0        0     1608 2022-12-08 06:14:10.000000 lectric-sdk-0.0.6a0/lectric/api/default/root_auth_auth_get.py
--rw-rw-rw-   0        0        0     1550 2022-12-08 06:14:10.000000 lectric-sdk-0.0.6a0/lectric/api/default/root_get.py
-drwxrwxrwx   0        0        0        0 2023-01-05 00:15:43.127637 lectric-sdk-0.0.6a0/lectric/api/index/
--rw-rw-rw-   0        0        0        0 2022-12-08 06:14:10.000000 lectric-sdk-0.0.6a0/lectric/api/index/__init__.py
--rw-rw-rw-   0        0        0     3757 2022-12-08 06:14:10.000000 lectric-sdk-0.0.6a0/lectric/api/index/create_index_create_post.py
--rw-rw-rw-   0        0        0     3865 2022-12-08 06:14:10.000000 lectric-sdk-0.0.6a0/lectric/api/index/delete_index_collection_name_field_name_delete.py
-drwxrwxrwx   0        0        0        0 2023-01-05 00:15:43.134640 lectric-sdk-0.0.6a0/lectric/api/ingest/
--rw-rw-rw-   0        0        0        0 2022-12-08 06:14:10.000000 lectric-sdk-0.0.6a0/lectric/api/ingest/__init__.py
--rw-rw-rw-   0        0        0     3600 2022-12-08 06:14:10.000000 lectric-sdk-0.0.6a0/lectric/api/ingest/ingest_ingest_post.py
-drwxrwxrwx   0        0        0        0 2023-01-05 00:15:43.146647 lectric-sdk-0.0.6a0/lectric/api/query/
--rw-rw-rw-   0        0        0        0 2022-12-08 06:14:10.000000 lectric-sdk-0.0.6a0/lectric/api/query/__init__.py
--rw-rw-rw-   0        0        0     3738 2022-12-08 06:14:10.000000 lectric-sdk-0.0.6a0/lectric/api/query/query_query_fields_post.py
--rw-rw-rw-   0        0        0     3852 2022-12-08 06:14:10.000000 lectric-sdk-0.0.6a0/lectric/api/query/query_query_vectors_post.py
--rw-rw-rw-   0        0        0     1708 2022-12-08 06:14:10.000000 lectric-sdk-0.0.6a0/lectric/client.py
--rw-rw-rw-   0        0        0      359 2022-08-12 21:03:44.000000 lectric-sdk-0.0.6a0/lectric/helpers.py
--rw-rw-rw-   0        0        0     9923 2022-12-12 20:03:18.000000 lectric-sdk-0.0.6a0/lectric/lectric_client.py
-drwxrwxrwx   0        0        0        0 2023-01-05 00:15:43.259641 lectric-sdk-0.0.6a0/lectric/models/
--rw-rw-rw-   0        0        0     1607 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/__init__.py
--rw-rw-rw-   0        0        0     3555 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/collection.py
--rw-rw-rw-   0        0        0     3671 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/collection_in_spec.py
--rw-rw-rw-   0        0        0      181 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/collection_in_spec_object_type.py
--rw-rw-rw-   0        0        0      163 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/collection_object_type.py
--rw-rw-rw-   0        0        0     3563 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/collection_schema.py
--rw-rw-rw-   0        0        0      181 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/collection_schema_object_type.py
--rw-rw-rw-   0        0        0     4672 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/field_schema.py
--rw-rw-rw-   0        0        0      166 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/field_schema_object_type.py
--rw-rw-rw-   0        0        0     3193 2022-12-12 20:03:18.000000 lectric-sdk-0.0.6a0/lectric/models/hit.py
--rw-rw-rw-   0        0        0      142 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/hit_object_type.py
--rw-rw-rw-   0        0        0     1411 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/hit_result.py
--rw-rw-rw-   0        0        0     2378 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/http_validation_error.py
--rw-rw-rw-   0        0        0     3591 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/index.py
--rw-rw-rw-   0        0        0     3336 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/index_in_spec.py
--rw-rw-rw-   0        0        0      166 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/index_in_spec_object_type.py
--rw-rw-rw-   0        0        0      148 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/index_object_type.py
--rw-rw-rw-   0        0        0     4955 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/index_params.py
--rw-rw-rw-   0        0        0      166 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/index_params_object_type.py
--rw-rw-rw-   0        0        0     3245 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/input_data.py
--rw-rw-rw-   0        0        0      160 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/input_data_object_type.py
--rw-rw-rw-   0        0        0     3590 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/query_meta_params.py
--rw-rw-rw-   0        0        0      178 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/query_meta_params_object_type.py
--rw-rw-rw-   0        0        0     3221 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/query_params.py
--rw-rw-rw-   0        0        0      166 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/query_params_object_type.py
--rw-rw-rw-   0        0        0     3951 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/query_response.py
--rw-rw-rw-   0        0        0      172 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/query_response_object_type.py
--rw-rw-rw-   0        0        0     4408 2022-12-12 20:03:18.000000 lectric-sdk-0.0.6a0/lectric/models/query_spec.py
--rw-rw-rw-   0        0        0      160 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/query_spec_object_type.py
--rw-rw-rw-   0        0        0     2507 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/validation_error.py
--rw-rw-rw-   0        0        0     6489 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/vector_query_spec.py
--rw-rw-rw-   0        0        0      178 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/models/vector_query_spec_object_type.py
--rw-rw-rw-   0        0        0      982 2022-12-08 06:14:11.000000 lectric-sdk-0.0.6a0/lectric/types.py
-drwxrwxrwx   0        0        0        0 2023-01-05 00:15:43.308639 lectric-sdk-0.0.6a0/lectric_sdk.egg-info/
--rw-rw-rw-   0        0        0     3017 2023-01-05 00:15:42.000000 lectric-sdk-0.0.6a0/lectric_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2685 2023-01-05 00:15:42.000000 lectric-sdk-0.0.6a0/lectric_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-05 00:15:42.000000 lectric-sdk-0.0.6a0/lectric_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-05 00:15:42.000000 lectric-sdk-0.0.6a0/lectric_sdk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       62 2023-01-05 00:15:42.000000 lectric-sdk-0.0.6a0/lectric_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-01-05 00:15:42.000000 lectric-sdk-0.0.6a0/lectric_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-05 00:15:43.313644 lectric-sdk-0.0.6a0/setup.cfg
--rw-rw-rw-   0        0        0      891 2023-01-04 23:34:03.000000 lectric-sdk-0.0.6a0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 17:18:52.070785 lectric-sdk-0.0.9/
+-rw-rw-rw-   0        0        0      125 2023-01-05 17:26:11.000000 lectric-sdk-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3917 2023-04-21 17:18:52.068784 lectric-sdk-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2705 2023-01-05 17:26:11.000000 lectric-sdk-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 17:18:51.312818 lectric-sdk-0.0.9/lectric/
+-rw-rw-rw-   0        0        0        6 2023-03-19 08:00:22.000000 lectric-sdk-0.0.9/lectric/VERSION
+-rw-rw-rw-   0        0        0      462 2023-04-21 17:17:43.000000 lectric-sdk-0.0.9/lectric/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 17:18:51.316269 lectric-sdk-0.0.9/lectric/api/
+-rw-rw-rw-   0        0        0       47 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 17:18:51.361205 lectric-sdk-0.0.9/lectric/api/collection/
+-rw-rw-rw-   0        0        0        0 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/collection/__init__.py
+-rw-rw-rw-   0        0        0     3931 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/collection/create_collection_collection_create_post.py
+-rw-rw-rw-   0        0        0     4229 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/collection/delete_entities_collection_entities_delete.py
+-rw-rw-rw-   0        0        0     3540 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/collection/drop_collection_collection_delete.py
+-rw-rw-rw-   0        0        0     4064 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/collection/exists_collection_collection_exists_name_get.py
+-rw-rw-rw-   0        0        0     3459 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/collection/get_collection_collection_get_name_get.py
+-rw-rw-rw-   0        0        0     3545 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/collection/get_indexes_collection_indexes_name_get.py
+-rw-rw-rw-   0        0        0     3396 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/collection/is_empty_collection_collection_empty_name_get.py
+-rw-rw-rw-   0        0        0     2698 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/collection/list_collections_collection_list_get.py
+-rw-rw-rw-   0        0        0     4585 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/collection/sample_collection_sample_get.py
+-rw-rw-rw-   0        0        0     4133 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/collection/sizeof_collection_collection_size_name_get.py
+drwxrwxrwx   0        0        0        0 2023-04-21 17:18:51.383723 lectric-sdk-0.0.9/lectric/api/default/
+-rw-rw-rw-   0        0        0        0 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/default/__init__.py
+-rw-rw-rw-   0        0        0     2461 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/default/list_connections_connections_get.py
+-rw-rw-rw-   0        0        0     1608 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/default/root_auth_auth_get.py
+-rw-rw-rw-   0        0        0     1550 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/default/root_get.py
+drwxrwxrwx   0        0        0        0 2023-04-21 17:18:51.473733 lectric-sdk-0.0.9/lectric/api/exact/
+-rw-rw-rw-   0        0        0        0 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/exact/__init__.py
+-rw-rw-rw-   0        0        0     3937 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/exact/create_collection_exact_create_collection_post.py
+-rw-rw-rw-   0        0        0     3498 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/exact/delete_collections_exact_collection_delete.py
+-rw-rw-rw-   0        0        0     2590 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/exact/get_available_algos_exact_algos_get.py
+-rw-rw-rw-   0        0        0     3255 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/exact/is_algo_available_exact_available_algo_get.py
+-rw-rw-rw-   0        0        0     2717 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/exact/list_collections_exact_list_get.py
+-rw-rw-rw-   0        0        0     5429 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/exact/lookup_by_file_exact_lookup_file_collection_name_post.py
+-rw-rw-rw-   0        0        0     4484 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/exact/lookup_by_uri_exact_lookup_hash_uri_collection_name_get.py
+-rw-rw-rw-   0        0        0     5775 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/exact/put_entry_by_file_exact_hash_collection_name_file_put.py
+-rw-rw-rw-   0        0        0     5537 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/exact/put_entry_by_uri_exact_hash_collection_name_uri_put.py
+drwxrwxrwx   0        0        0        0 2023-04-21 17:18:51.484723 lectric-sdk-0.0.9/lectric/api/index/
+-rw-rw-rw-   0        0        0        0 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/index/__init__.py
+-rw-rw-rw-   0        0        0     3757 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/index/create_index_create_post.py
+-rw-rw-rw-   0        0        0     3865 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/index/delete_index_collection_name_field_name_delete.py
+drwxrwxrwx   0        0        0        0 2023-04-21 17:18:51.507871 lectric-sdk-0.0.9/lectric/api/ingest/
+-rw-rw-rw-   0        0        0        0 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/ingest/__init__.py
+-rw-rw-rw-   0        0        0     3600 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/ingest/ingest_ingest_post.py
+drwxrwxrwx   0        0        0        0 2023-04-21 17:18:51.569293 lectric-sdk-0.0.9/lectric/api/query/
+-rw-rw-rw-   0        0        0        0 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/query/__init__.py
+-rw-rw-rw-   0        0        0     3738 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/query/query_query_fields_post.py
+-rw-rw-rw-   0        0        0     3852 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/api/query/query_query_vectors_post.py
+-rw-rw-rw-   0        0        0     1708 2023-04-21 17:17:41.000000 lectric-sdk-0.0.9/lectric/client.py
+-rw-rw-rw-   0        0        0     1180 2023-02-08 17:59:04.000000 lectric-sdk-0.0.9/lectric/helpers.py
+-rw-rw-rw-   0        0        0    16846 2023-04-20 06:54:01.000000 lectric-sdk-0.0.9/lectric/lectric_client.py
+-rw-rw-rw-   0        0        0     1300 2023-04-21 17:09:52.000000 lectric-sdk-0.0.9/lectric/lectric_types.py
+drwxrwxrwx   0        0        0        0 2023-04-21 17:18:51.916783 lectric-sdk-0.0.9/lectric/models/
+-rw-rw-rw-   0        0        0     1863 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/__init__.py
+-rw-rw-rw-   0        0        0     2381 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/body_lookup_by_file_exact_lookup_file_collection_name_post.py
+-rw-rw-rw-   0        0        0     2379 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/body_put_entry_by_file_exact_hash_collection_name_file_put.py
+-rw-rw-rw-   0        0        0     3903 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/collection.py
+-rw-rw-rw-   0        0        0     4019 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/collection_in_spec.py
+-rw-rw-rw-   0        0        0      181 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/collection_in_spec_object_type.py
+-rw-rw-rw-   0        0        0      163 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/collection_object_type.py
+-rw-rw-rw-   0        0        0     3765 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/collection_schema.py
+-rw-rw-rw-   0        0        0      181 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/collection_schema_object_type.py
+-rw-rw-rw-   0        0        0     4672 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/field_schema.py
+-rw-rw-rw-   0        0        0      166 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/field_schema_object_type.py
+-rw-rw-rw-   0        0        0     3193 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/hit.py
+-rw-rw-rw-   0        0        0      142 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/hit_object_type.py
+-rw-rw-rw-   0        0        0     1411 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/hit_result.py
+-rw-rw-rw-   0        0        0     2378 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/http_validation_error.py
+-rw-rw-rw-   0        0        0     3591 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/index.py
+-rw-rw-rw-   0        0        0     3336 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/index_in_spec.py
+-rw-rw-rw-   0        0        0      166 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/index_in_spec_object_type.py
+-rw-rw-rw-   0        0        0      148 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/index_object_type.py
+-rw-rw-rw-   0        0        0     4955 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/index_params.py
+-rw-rw-rw-   0        0        0      166 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/index_params_object_type.py
+-rw-rw-rw-   0        0        0     3245 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/input_data.py
+-rw-rw-rw-   0        0        0      160 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/input_data_object_type.py
+-rw-rw-rw-   0        0        0     3590 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/query_meta_params.py
+-rw-rw-rw-   0        0        0      178 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/query_meta_params_object_type.py
+-rw-rw-rw-   0        0        0     3130 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/query_params.py
+-rw-rw-rw-   0        0        0      166 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/query_params_object_type.py
+-rw-rw-rw-   0        0        0     3990 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/query_response.py
+-rw-rw-rw-   0        0        0      172 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/query_response_object_type.py
+-rw-rw-rw-   0        0        0     4408 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/query_spec.py
+-rw-rw-rw-   0        0        0      160 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/query_spec_object_type.py
+-rw-rw-rw-   0        0        0     2507 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/validation_error.py
+-rw-rw-rw-   0        0        0     6489 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/vector_query_spec.py
+-rw-rw-rw-   0        0        0      178 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/models/vector_query_spec_object_type.py
+-rw-rw-rw-   0        0        0      982 2023-04-21 17:17:42.000000 lectric-sdk-0.0.9/lectric/types.py
+drwxrwxrwx   0        0        0        0 2023-04-21 17:18:52.064785 lectric-sdk-0.0.9/lectric_sdk.egg-info/
+-rw-rw-rw-   0        0        0     3917 2023-04-21 17:18:50.000000 lectric-sdk-0.0.9/lectric_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3555 2023-04-21 17:18:50.000000 lectric-sdk-0.0.9/lectric_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 17:18:50.000000 lectric-sdk-0.0.9/lectric_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-21 17:18:50.000000 lectric-sdk-0.0.9/lectric_sdk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       68 2023-04-21 17:18:50.000000 lectric-sdk-0.0.9/lectric_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-21 17:18:50.000000 lectric-sdk-0.0.9/lectric_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 17:18:52.071795 lectric-sdk-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      909 2023-03-01 01:09:40.000000 lectric-sdk-0.0.9/setup.py
```

### Comparing `lectric-sdk-0.0.6a0/PKG-INFO` & `lectric-sdk-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: lectric-sdk
-Version: 0.0.6a0
-Summary: Lectric client
-Author: Disa Mhembere
-Author-email: disamhembere@microsoft.com
-Keywords: lectric,vdb,vector database
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-
 # Lectric Software Development Kit (SDK)
 
 Programmatic access to the lectric vector database service.
 
 ## Installation
 
 The SDK is exposed as a simple python package. There are two main ways it can be installed.
```

### Comparing `lectric-sdk-0.0.6a0/lectric/api/collection/create_collection_collection_create_post.py` & `lectric-sdk-0.0.9/lectric/api/collection/create_collection_collection_create_post.py`

 * *Files identical despite different names*

### Comparing `lectric-sdk-0.0.6a0/lectric/api/collection/delete_entities_collection_entities_delete.py` & `lectric-sdk-0.0.9/lectric/api/collection/delete_entities_collection_entities_delete.py`

 * *Files identical despite different names*

### Comparing `lectric-sdk-0.0.6a0/lectric/api/collection/drop_collection_collection_delete.py` & `lectric-sdk-0.0.9/lectric/api/collection/drop_collection_collection_delete.py`

 * *Files identical despite different names*

### Comparing `lectric-sdk-0.0.6a0/lectric/api/collection/exists_collection_collection_exists_name_get.py` & `lectric-sdk-0.0.9/lectric/api/exact/delete_collections_exact_collection_delete.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
 from ...client import AuthenticatedClient
 from ...models.http_validation_error import HTTPValidationError
-from ...types import Response
+from ...types import UNSET, Response
 
 
 def _get_kwargs(
-    name: str,
     *,
     client: AuthenticatedClient,
+    name: str,
 ) -> Dict[str, Any]:
-    url = "{}/collection/exists/{name}".format(client.base_url, name=name)
+    url = "{}/exact/collection".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
+    params: Dict[str, Any] = {}
+    params["name"] = name
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
     return {
-        "method": "get",
+        "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "params": params,
     }
 
 
 def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError]]:
     if response.status_code == 200:
         response_200 = cast(Any, response.json())
         return response_200
@@ -46,106 +52,106 @@
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    name: str,
     *,
     client: AuthenticatedClient,
+    name: str,
 ) -> Response[Union[Any, HTTPValidationError]]:
-    """Exists Collection
+    """Delete Collections
 
-     Does a collection with this name exist?
+     Delete exact collections
 
     Args:
         name (str):
 
     Returns:
         Response[Union[Any, HTTPValidationError]]
     """
 
     kwargs = _get_kwargs(
-        name=name,
         client=client,
+        name=name,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    name: str,
     *,
     client: AuthenticatedClient,
+    name: str,
 ) -> Optional[Union[Any, HTTPValidationError]]:
-    """Exists Collection
+    """Delete Collections
 
-     Does a collection with this name exist?
+     Delete exact collections
 
     Args:
         name (str):
 
     Returns:
         Response[Union[Any, HTTPValidationError]]
     """
 
     return sync_detailed(
-        name=name,
         client=client,
+        name=name,
     ).parsed
 
 
 async def asyncio_detailed(
-    name: str,
     *,
     client: AuthenticatedClient,
+    name: str,
 ) -> Response[Union[Any, HTTPValidationError]]:
-    """Exists Collection
+    """Delete Collections
 
-     Does a collection with this name exist?
+     Delete exact collections
 
     Args:
         name (str):
 
     Returns:
         Response[Union[Any, HTTPValidationError]]
     """
 
     kwargs = _get_kwargs(
-        name=name,
         client=client,
+        name=name,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    name: str,
     *,
     client: AuthenticatedClient,
+    name: str,
 ) -> Optional[Union[Any, HTTPValidationError]]:
-    """Exists Collection
+    """Delete Collections
 
-     Does a collection with this name exist?
+     Delete exact collections
 
     Args:
         name (str):
 
     Returns:
         Response[Union[Any, HTTPValidationError]]
     """
 
     return (
         await asyncio_detailed(
-            name=name,
             client=client,
+            name=name,
         )
     ).parsed
```

### Comparing `lectric-sdk-0.0.6a0/lectric/api/collection/get_collection_collection_get_name_get.py` & `lectric-sdk-0.0.9/lectric/api/collection/get_collection_collection_get_name_get.py`

 * *Files identical despite different names*

### Comparing `lectric-sdk-0.0.6a0/lectric/api/collection/get_indexes_collection_indexes_name_get.py` & `lectric-sdk-0.0.9/lectric/api/collection/get_indexes_collection_indexes_name_get.py`

 * *Files identical despite different names*

### Comparing `lectric-sdk-0.0.6a0/lectric/api/collection/is_empty_collection_collection_empty_name_get.py` & `lectric-sdk-0.0.9/lectric/api/collection/is_empty_collection_collection_empty_name_get.py`

 * *Files identical despite different names*

### Comparing `lectric-sdk-0.0.6a0/lectric/api/collection/list_collections_collection_list_get.py` & `lectric-sdk-0.0.9/lectric/api/collection/list_collections_collection_list_get.py`

 * *Files identical despite different names*

### Comparing `lectric-sdk-0.0.6a0/lectric/api/collection/sizeof_collection_collection_size_name_get.py` & `lectric-sdk-0.0.9/lectric/api/index/create_index_create_post.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,151 +1,155 @@
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
 from ...client import AuthenticatedClient
 from ...models.http_validation_error import HTTPValidationError
+from ...models.index_in_spec import IndexInSpec
 from ...types import Response
 
 
 def _get_kwargs(
-    name: str,
     *,
     client: AuthenticatedClient,
+    json_body: IndexInSpec,
 ) -> Dict[str, Any]:
-    url = "{}/collection/size/{name}".format(client.base_url, name=name)
+    url = "{}/index/create".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
+    json_json_body = json_body.to_dict()
+
     return {
-        "method": "get",
+        "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError, int]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError]]:
     if response.status_code == 200:
-        response_200 = cast(int, response.json())
+        response_200 = cast(Any, response.json())
         return response_200
     if response.status_code == 404:
         response_404 = cast(Any, None)
         return response_404
     if response.status_code == 422:
         response_422 = HTTPValidationError.from_dict(response.json())
 
         return response_422
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, HTTPValidationError, int]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, HTTPValidationError]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    name: str,
     *,
     client: AuthenticatedClient,
-) -> Response[Union[Any, HTTPValidationError, int]]:
-    """Sizeof Collection
+    json_body: IndexInSpec,
+) -> Response[Union[Any, HTTPValidationError]]:
+    """Create
 
-     Get the number of entities in a collection
+     Create an index on field name specified (must be defined within schema first)
 
     Args:
-        name (str):
+        json_body (IndexInSpec):
 
     Returns:
-        Response[Union[Any, HTTPValidationError, int]]
+        Response[Union[Any, HTTPValidationError]]
     """
 
     kwargs = _get_kwargs(
-        name=name,
         client=client,
+        json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    name: str,
     *,
     client: AuthenticatedClient,
-) -> Optional[Union[Any, HTTPValidationError, int]]:
-    """Sizeof Collection
+    json_body: IndexInSpec,
+) -> Optional[Union[Any, HTTPValidationError]]:
+    """Create
 
-     Get the number of entities in a collection
+     Create an index on field name specified (must be defined within schema first)
 
     Args:
-        name (str):
+        json_body (IndexInSpec):
 
     Returns:
-        Response[Union[Any, HTTPValidationError, int]]
+        Response[Union[Any, HTTPValidationError]]
     """
 
     return sync_detailed(
-        name=name,
         client=client,
+        json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
-    name: str,
     *,
     client: AuthenticatedClient,
-) -> Response[Union[Any, HTTPValidationError, int]]:
-    """Sizeof Collection
+    json_body: IndexInSpec,
+) -> Response[Union[Any, HTTPValidationError]]:
+    """Create
 
-     Get the number of entities in a collection
+     Create an index on field name specified (must be defined within schema first)
 
     Args:
-        name (str):
+        json_body (IndexInSpec):
 
     Returns:
-        Response[Union[Any, HTTPValidationError, int]]
+        Response[Union[Any, HTTPValidationError]]
     """
 
     kwargs = _get_kwargs(
-        name=name,
         client=client,
+        json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    name: str,
     *,
     client: AuthenticatedClient,
-) -> Optional[Union[Any, HTTPValidationError, int]]:
-    """Sizeof Collection
+    json_body: IndexInSpec,
+) -> Optional[Union[Any, HTTPValidationError]]:
+    """Create
 
-     Get the number of entities in a collection
+     Create an index on field name specified (must be defined within schema first)
 
     Args:
-        name (str):
+        json_body (IndexInSpec):
 
     Returns:
-        Response[Union[Any, HTTPValidationError, int]]
+        Response[Union[Any, HTTPValidationError]]
     """
 
     return (
         await asyncio_detailed(
-            name=name,
             client=client,
+            json_body=json_body,
         )
     ).parsed
```

### Comparing `lectric-sdk-0.0.6a0/lectric/api/default/list_connections_connections_get.py` & `lectric-sdk-0.0.9/lectric/api/default/list_connections_connections_get.py`

 * *Files identical despite different names*

### Comparing `lectric-sdk-0.0.6a0/lectric/api/default/root_auth_auth_get.py` & `lectric-sdk-0.0.9/lectric/api/default/root_auth_auth_get.py`

 * *Files identical despite different names*

### Comparing `lectric-sdk-0.0.6a0/lectric/api/default/root_get.py` & `lectric-sdk-0.0.9/lectric/api/default/root_get.py`

 * *Files identical despite different names*

### Comparing `lectric-sdk-0.0.6a0/lectric/api/index/create_index_create_post.py` & `lectric-sdk-0.0.9/lectric/api/ingest/ingest_ingest_post.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
 from ...client import AuthenticatedClient
 from ...models.http_validation_error import HTTPValidationError
-from ...models.index_in_spec import IndexInSpec
+from ...models.input_data import InputData
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: AuthenticatedClient,
-    json_body: IndexInSpec,
+    json_body: InputData,
 ) -> Dict[str, Any]:
-    url = "{}/index/create".format(client.base_url)
+    url = "{}/ingest".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     json_json_body = json_body.to_dict()
 
     return {
@@ -52,22 +52,22 @@
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
-    json_body: IndexInSpec,
+    json_body: InputData,
 ) -> Response[Union[Any, HTTPValidationError]]:
-    """Create
+    """Ingest
 
-     Create an index on field name specified (must be defined within schema first)
+     Ingest data into a collection already created
 
     Args:
-        json_body (IndexInSpec):
+        json_body (InputData):
 
     Returns:
         Response[Union[Any, HTTPValidationError]]
     """
 
     kwargs = _get_kwargs(
         client=client,
@@ -81,44 +81,44 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
-    json_body: IndexInSpec,
+    json_body: InputData,
 ) -> Optional[Union[Any, HTTPValidationError]]:
-    """Create
+    """Ingest
 
-     Create an index on field name specified (must be defined within schema first)
+     Ingest data into a collection already created
 
     Args:
-        json_body (IndexInSpec):
+        json_body (InputData):
 
     Returns:
         Response[Union[Any, HTTPValidationError]]
     """
 
     return sync_detailed(
         client=client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
-    json_body: IndexInSpec,
+    json_body: InputData,
 ) -> Response[Union[Any, HTTPValidationError]]:
-    """Create
+    """Ingest
 
-     Create an index on field name specified (must be defined within schema first)
+     Ingest data into a collection already created
 
     Args:
-        json_body (IndexInSpec):
+        json_body (InputData):
 
     Returns:
         Response[Union[Any, HTTPValidationError]]
     """
 
     kwargs = _get_kwargs(
         client=client,
@@ -130,22 +130,22 @@
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
-    json_body: IndexInSpec,
+    json_body: InputData,
 ) -> Optional[Union[Any, HTTPValidationError]]:
-    """Create
+    """Ingest
 
-     Create an index on field name specified (must be defined within schema first)
+     Ingest data into a collection already created
 
     Args:
-        json_body (IndexInSpec):
+        json_body (InputData):
 
     Returns:
         Response[Union[Any, HTTPValidationError]]
     """
 
     return (
         await asyncio_detailed(
```

### Comparing `lectric-sdk-0.0.6a0/lectric/api/index/delete_index_collection_name_field_name_delete.py` & `lectric-sdk-0.0.9/lectric/api/index/delete_index_collection_name_field_name_delete.py`

 * *Files identical despite different names*

### Comparing `lectric-sdk-0.0.6a0/lectric/api/ingest/ingest_ingest_post.py` & `lectric-sdk-0.0.9/lectric/api/exact/create_collection_exact_create_collection_post.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
 from ...client import AuthenticatedClient
+from ...models.collection import Collection
+from ...models.collection_in_spec import CollectionInSpec
 from ...models.http_validation_error import HTTPValidationError
-from ...models.input_data import InputData
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: AuthenticatedClient,
-    json_body: InputData,
+    json_body: CollectionInSpec,
 ) -> Dict[str, Any]:
-    url = "{}/ingest".format(client.base_url)
+    url = "{}/exact/create/collection".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     json_json_body = json_body.to_dict()
 
     return {
@@ -26,51 +27,52 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Collection, HTTPValidationError]]:
     if response.status_code == 200:
-        response_200 = cast(Any, response.json())
+        response_200 = Collection.from_dict(response.json())
+
         return response_200
     if response.status_code == 404:
         response_404 = cast(Any, None)
         return response_404
     if response.status_code == 422:
         response_422 = HTTPValidationError.from_dict(response.json())
 
         return response_422
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, HTTPValidationError]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[Any, Collection, HTTPValidationError]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
-    json_body: InputData,
-) -> Response[Union[Any, HTTPValidationError]]:
-    """Ingest
+    json_body: CollectionInSpec,
+) -> Response[Union[Any, Collection, HTTPValidationError]]:
+    """Create Collection
 
-     Ingest data into a collection already created
+     Create a collection by name with a specific schema
 
     Args:
-        json_body (InputData):
+        json_body (CollectionInSpec):
 
     Returns:
-        Response[Union[Any, HTTPValidationError]]
+        Response[Union[Any, Collection, HTTPValidationError]]
     """
 
     kwargs = _get_kwargs(
         client=client,
         json_body=json_body,
     )
 
@@ -81,47 +83,47 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
-    json_body: InputData,
-) -> Optional[Union[Any, HTTPValidationError]]:
-    """Ingest
+    json_body: CollectionInSpec,
+) -> Optional[Union[Any, Collection, HTTPValidationError]]:
+    """Create Collection
 
-     Ingest data into a collection already created
+     Create a collection by name with a specific schema
 
     Args:
-        json_body (InputData):
+        json_body (CollectionInSpec):
 
     Returns:
-        Response[Union[Any, HTTPValidationError]]
+        Response[Union[Any, Collection, HTTPValidationError]]
     """
 
     return sync_detailed(
         client=client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
-    json_body: InputData,
-) -> Response[Union[Any, HTTPValidationError]]:
-    """Ingest
+    json_body: CollectionInSpec,
+) -> Response[Union[Any, Collection, HTTPValidationError]]:
+    """Create Collection
 
-     Ingest data into a collection already created
+     Create a collection by name with a specific schema
 
     Args:
-        json_body (InputData):
+        json_body (CollectionInSpec):
 
     Returns:
-        Response[Union[Any, HTTPValidationError]]
+        Response[Union[Any, Collection, HTTPValidationError]]
     """
 
     kwargs = _get_kwargs(
         client=client,
         json_body=json_body,
     )
 
@@ -130,25 +132,25 @@
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
-    json_body: InputData,
-) -> Optional[Union[Any, HTTPValidationError]]:
-    """Ingest
+    json_body: CollectionInSpec,
+) -> Optional[Union[Any, Collection, HTTPValidationError]]:
+    """Create Collection
 
-     Ingest data into a collection already created
+     Create a collection by name with a specific schema
 
     Args:
-        json_body (InputData):
+        json_body (CollectionInSpec):
 
     Returns:
-        Response[Union[Any, HTTPValidationError]]
+        Response[Union[Any, Collection, HTTPValidationError]]
     """
 
     return (
         await asyncio_detailed(
             client=client,
             json_body=json_body,
         )
```

### Comparing `lectric-sdk-0.0.6a0/lectric/api/query/query_query_fields_post.py` & `lectric-sdk-0.0.9/lectric/api/query/query_query_fields_post.py`

 * *Files identical despite different names*

### Comparing `lectric-sdk-0.0.6a0/lectric/api/query/query_query_vectors_post.py` & `lectric-sdk-0.0.9/lectric/api/query/query_query_vectors_post.py`

 * *Files identical despite different names*

### Comparing `lectric-sdk-0.0.6a0/lectric/client.py` & `lectric-sdk-0.0.9/lectric/client.py`

 * *Files identical despite different names*

### Comparing `lectric-sdk-0.0.6a0/lectric/models/__init__.py` & `lectric-sdk-0.0.9/lectric/models/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 """ Contains all the data models used in inputs/outputs """
 
+from .body_lookup_by_file_exact_lookup_file_collection_name_post import (
+    BodyLookupByFileExactLookupFileCollectionNamePost,
+)
+from .body_put_entry_by_file_exact_hash_collection_name_file_put import BodyPutEntryByFileExactHashCollectionNameFilePut
 from .collection import Collection
 from .collection_in_spec import CollectionInSpec
 from .collection_in_spec_object_type import CollectionInSpecObjectType
 from .collection_object_type import CollectionObjectType
 from .collection_schema import CollectionSchema
 from .collection_schema_object_type import CollectionSchemaObjectType
 from .field_schema import FieldSchema
```

### Comparing `lectric-sdk-0.0.6a0/lectric/models/collection.py` & `lectric-sdk-0.0.9/lectric/models/collection.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,58 +19,65 @@
 class Collection:
     """
     Attributes:
         name (str):
         coll_schema (CollectionSchema):
         object_type (Union[Unset, CollectionObjectType]):  Default: CollectionObjectType.COLLECTION.
         consistency_level (Union[Unset, str]):  Default: 'Session'.
+        approx (Union[Unset, bool]):  Default: True.
     """
 
     name: str
     coll_schema: CollectionSchema
     object_type: Union[Unset, CollectionObjectType] = CollectionObjectType.COLLECTION
     consistency_level: Union[Unset, str] = "Session"
+    approx: Union[Unset, bool] = True
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def __init__(
         self,
         name: str,
         coll_schema: CollectionSchema,
         object_type: Union[Unset, CollectionObjectType] = CollectionObjectType.COLLECTION,
         consistency_level: Union[Unset, str] = "Session",
+        approx: Union[Unset, bool] = True,
     ):
         """ """
 
         self.name = name
         self.coll_schema = coll_schema
         self.object_type = object_type
         self.consistency_level = consistency_level
+        self.approx = approx
 
     def to_dict(self) -> Dict[str, Any]:
         name = self.name
         coll_schema = self.coll_schema.to_dict()
 
         object_type: Union[Unset, str] = UNSET
         if not isinstance(self.object_type, Unset):
             object_type = self.object_type.value
 
         consistency_level = self.consistency_level
+        approx = self.approx
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "name": name,
                 "coll_schema": coll_schema,
             }
         )
         if object_type is not UNSET:
             field_dict["object_type"] = object_type
         if consistency_level is not UNSET:
             field_dict["consistency_level"] = consistency_level
+        if approx is not UNSET:
+            field_dict["approx"] = approx
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         name = d.pop("name")
@@ -82,19 +89,22 @@
         if isinstance(_object_type, Unset):
             object_type = UNSET
         else:
             object_type = CollectionObjectType(_object_type)
 
         consistency_level = unset_if_none(d, "consistency_level")
 
+        approx = unset_if_none(d, "approx")
+
         collection = cls(
             name=name,
             coll_schema=coll_schema,
             object_type=object_type,
             consistency_level=consistency_level,
+            approx=approx,
         )
 
         collection.additional_properties = d
         return collection
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `lectric-sdk-0.0.6a0/lectric/models/collection_in_spec.py` & `lectric-sdk-0.0.9/lectric/models/collection_in_spec.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,58 +19,65 @@
 class CollectionInSpec:
     """
     Attributes:
         name (str):
         coll_schema (CollectionSchema):
         object_type (Union[Unset, CollectionInSpecObjectType]):  Default: CollectionInSpecObjectType.COLLECTIONINSPEC.
         consistency_level (Union[Unset, str]):  Default: 'Session'.
+        approx (Union[Unset, bool]):  Default: True.
     """
 
     name: str
     coll_schema: CollectionSchema
     object_type: Union[Unset, CollectionInSpecObjectType] = CollectionInSpecObjectType.COLLECTIONINSPEC
     consistency_level: Union[Unset, str] = "Session"
+    approx: Union[Unset, bool] = True
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def __init__(
         self,
         name: str,
         coll_schema: CollectionSchema,
         object_type: Union[Unset, CollectionInSpecObjectType] = CollectionInSpecObjectType.COLLECTIONINSPEC,
         consistency_level: Union[Unset, str] = "Session",
+        approx: Union[Unset, bool] = True,
     ):
         """ """
 
         self.name = name
         self.coll_schema = coll_schema
         self.object_type = object_type
         self.consistency_level = consistency_level
+        self.approx = approx
 
     def to_dict(self) -> Dict[str, Any]:
         name = self.name
         coll_schema = self.coll_schema.to_dict()
 
         object_type: Union[Unset, str] = UNSET
         if not isinstance(self.object_type, Unset):
             object_type = self.object_type.value
 
         consistency_level = self.consistency_level
+        approx = self.approx
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "name": name,
                 "coll_schema": coll_schema,
             }
         )
         if object_type is not UNSET:
             field_dict["object_type"] = object_type
         if consistency_level is not UNSET:
             field_dict["consistency_level"] = consistency_level
+        if approx is not UNSET:
+            field_dict["approx"] = approx
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         name = d.pop("name")
@@ -82,19 +89,22 @@
         if isinstance(_object_type, Unset):
             object_type = UNSET
         else:
             object_type = CollectionInSpecObjectType(_object_type)
 
         consistency_level = unset_if_none(d, "consistency_level")
 
+        approx = unset_if_none(d, "approx")
+
         collection_in_spec = cls(
             name=name,
             coll_schema=coll_schema,
             object_type=object_type,
             consistency_level=consistency_level,
+            approx=approx,
         )
 
         collection_in_spec.additional_properties = d
         return collection_in_spec
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `lectric-sdk-0.0.6a0/lectric/models/collection_schema.py` & `lectric-sdk-0.0.9/lectric/models/collection_schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,85 +15,85 @@
     return _dict[key]
 
 
 @attr.s(auto_attribs=True)
 class CollectionSchema:
     """
     Attributes:
-        fields (List[FieldSchema]):
         object_type (Union[Unset, CollectionSchemaObjectType]):  Default: CollectionSchemaObjectType.COLLECTIONSCHEMA.
+        fields (Union[Unset, List[FieldSchema]]):
         description (Union[Unset, str]):  Default: ''.
     """
 
-    fields: List[FieldSchema]
     object_type: Union[Unset, CollectionSchemaObjectType] = CollectionSchemaObjectType.COLLECTIONSCHEMA
+    fields: Union[Unset, List[FieldSchema]] = UNSET
     description: Union[Unset, str] = ""
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def __init__(
         self,
-        fields: List[FieldSchema],
         object_type: Union[Unset, CollectionSchemaObjectType] = CollectionSchemaObjectType.COLLECTIONSCHEMA,
+        fields: Union[Unset, List[FieldSchema]] = UNSET,
         description: Union[Unset, str] = "",
     ):
         """ """
 
-        self.fields = fields
         self.object_type = object_type
+        self.fields = fields
         self.description = description
 
     def to_dict(self) -> Dict[str, Any]:
-        fields = []
-        for fields_item_data in self.fields:
-            fields_item = fields_item_data.to_dict()
-
-            fields.append(fields_item)
-
         object_type: Union[Unset, str] = UNSET
         if not isinstance(self.object_type, Unset):
             object_type = self.object_type.value
 
+        fields: Union[Unset, List[Dict[str, Any]]] = UNSET
+        if not isinstance(self.fields, Unset):
+            fields = []
+            for fields_item_data in self.fields:
+                fields_item = fields_item_data.to_dict()
+
+                fields.append(fields_item)
+
         description = self.description
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "fields": fields,
-            }
-        )
+        field_dict.update({})
         if object_type is not UNSET:
             field_dict["object_type"] = object_type
+        if fields is not UNSET:
+            field_dict["fields"] = fields
         if description is not UNSET:
             field_dict["description"] = description
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        fields = []
-        _fields = d.pop("fields")
-        for fields_item_data in _fields:
-            fields_item = FieldSchema.from_dict(fields_item_data)
-
-            fields.append(fields_item)
-
         _object_type = unset_if_none(d, "object_type")
         object_type: Union[Unset, CollectionSchemaObjectType]
         if isinstance(_object_type, Unset):
             object_type = UNSET
         else:
             object_type = CollectionSchemaObjectType(_object_type)
 
+        fields = []
+        _fields = unset_if_none(d, "fields")
+        for fields_item_data in _fields or []:
+            fields_item = FieldSchema.from_dict(fields_item_data)
+
+            fields.append(fields_item)
+
         description = unset_if_none(d, "description")
 
         collection_schema = cls(
-            fields=fields,
             object_type=object_type,
+            fields=fields,
             description=description,
         )
 
         collection_schema.additional_properties = d
         return collection_schema
 
     @property
```

### Comparing `lectric-sdk-0.0.6a0/lectric/models/field_schema.py` & `lectric-sdk-0.0.9/lectric/models/field_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,37 +15,37 @@
 
 
 @attr.s(auto_attribs=True)
 class FieldSchema:
     """
     Attributes:
         name (str):
-        dtype (str):
+        dtype (int):
         object_type (Union[Unset, FieldSchemaObjectType]):  Default: FieldSchemaObjectType.FIELDSCHEMA.
         is_primary (Union[Unset, bool]):
         auto_id (Union[Unset, bool]):
         description (Union[Unset, str]):  Default: ''.
         dim (Union[Unset, int]):
         max_length (Union[Unset, int]):
     """
 
     name: str
-    dtype: str
+    dtype: int
     object_type: Union[Unset, FieldSchemaObjectType] = FieldSchemaObjectType.FIELDSCHEMA
     is_primary: Union[Unset, bool] = False
     auto_id: Union[Unset, bool] = False
     description: Union[Unset, str] = ""
     dim: Union[Unset, int] = UNSET
     max_length: Union[Unset, int] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def __init__(
         self,
         name: str,
-        dtype: str,
+        dtype: int,
         object_type: Union[Unset, FieldSchemaObjectType] = FieldSchemaObjectType.FIELDSCHEMA,
         is_primary: Union[Unset, bool] = False,
         auto_id: Union[Unset, bool] = False,
         description: Union[Unset, str] = "",
         dim: Union[Unset, int] = UNSET,
         max_length: Union[Unset, int] = UNSET,
     ):
```

### Comparing `lectric-sdk-0.0.6a0/lectric/models/hit.py` & `lectric-sdk-0.0.9/lectric/models/hit.py`

 * *Files identical despite different names*

### Comparing `lectric-sdk-0.0.6a0/lectric/models/hit_result.py` & `lectric-sdk-0.0.9/lectric/models/hit_result.py`

 * *Files identical despite different names*

### Comparing `lectric-sdk-0.0.6a0/lectric/models/http_validation_error.py` & `lectric-sdk-0.0.9/lectric/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `lectric-sdk-0.0.6a0/lectric/models/index.py` & `lectric-sdk-0.0.9/lectric/models/index.py`

 * *Files identical despite different names*

### Comparing `lectric-sdk-0.0.6a0/lectric/models/index_in_spec.py` & `lectric-sdk-0.0.9/lectric/models/index_in_spec.py`

 * *Files identical despite different names*

### Comparing `lectric-sdk-0.0.6a0/lectric/models/index_params.py` & `lectric-sdk-0.0.9/lectric/models/index_params.py`

 * *Files identical despite different names*

### Comparing `lectric-sdk-0.0.6a0/lectric/models/input_data.py` & `lectric-sdk-0.0.9/lectric/models/input_data.py`

 * *Files identical despite different names*

### Comparing `lectric-sdk-0.0.6a0/lectric/models/query_meta_params.py` & `lectric-sdk-0.0.9/lectric/models/query_meta_params.py`

 * *Files identical despite different names*

### Comparing `lectric-sdk-0.0.6a0/lectric/models/query_params.py` & `lectric-sdk-0.0.9/lectric/models/query_params.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,73 +16,73 @@
 
 
 @attr.s(auto_attribs=True)
 class QueryParams:
     """
     Attributes:
         metric_type (str): A string corresponding to the Enum: VectorSpace
-        search_params (QueryMetaParams):
+        params (QueryMetaParams):
         object_type (Union[Unset, QueryParamsObjectType]):  Default: QueryParamsObjectType.QUERYPARAMS.
     """
 
     metric_type: str
-    search_params: QueryMetaParams
+    params: QueryMetaParams
     object_type: Union[Unset, QueryParamsObjectType] = QueryParamsObjectType.QUERYPARAMS
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def __init__(
         self,
         metric_type: str,
-        search_params: QueryMetaParams,
+        params: QueryMetaParams,
         object_type: Union[Unset, QueryParamsObjectType] = QueryParamsObjectType.QUERYPARAMS,
     ):
         """ """
 
         self.metric_type = metric_type
-        self.search_params = search_params
+        self.params = params
         self.object_type = object_type
 
     def to_dict(self) -> Dict[str, Any]:
         metric_type = self.metric_type
-        search_params = self.search_params.to_dict()
+        params = self.params.to_dict()
 
         object_type: Union[Unset, str] = UNSET
         if not isinstance(self.object_type, Unset):
             object_type = self.object_type.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "metric_type": metric_type,
-                "search_params": search_params,
+                "params": params,
             }
         )
         if object_type is not UNSET:
             field_dict["object_type"] = object_type
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         metric_type = d.pop("metric_type")
 
-        search_params = QueryMetaParams.from_dict(d.pop("search_params"))
+        params = QueryMetaParams.from_dict(d.pop("params"))
 
         _object_type = unset_if_none(d, "object_type")
         object_type: Union[Unset, QueryParamsObjectType]
         if isinstance(_object_type, Unset):
             object_type = UNSET
         else:
             object_type = QueryParamsObjectType(_object_type)
 
         query_params = cls(
             metric_type=metric_type,
-            search_params=search_params,
+            params=params,
             object_type=object_type,
         )
 
         query_params.additional_properties = d
         return query_params
 
     @property
```

### Comparing `lectric-sdk-0.0.6a0/lectric/models/query_response.py` & `lectric-sdk-0.0.9/lectric/models/query_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,63 +16,63 @@
 
 
 @attr.s(auto_attribs=True)
 class QueryResponse:
     """
     Attributes:
         hits (List[List[Hit]]):
-        query_time (float):
-        response_time (float):
+        query_latency (float):
+        total_latency (float):
         object_type (Union[Unset, QueryResponseObjectType]):  Default: QueryResponseObjectType.QUERYRESPONSE.
     """
 
     hits: List[List[Hit]]
-    query_time: float
-    response_time: float
+    query_latency: float
+    total_latency: float
     object_type: Union[Unset, QueryResponseObjectType] = QueryResponseObjectType.QUERYRESPONSE
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def __init__(
         self,
         hits: List[List[Hit]],
-        query_time: float,
-        response_time: float,
+        query_latency: float,
+        total_latency: float,
         object_type: Union[Unset, QueryResponseObjectType] = QueryResponseObjectType.QUERYRESPONSE,
     ):
         """ """
 
         self.hits = hits
-        self.query_time = query_time
-        self.response_time = response_time
+        self.query_latency = query_latency
+        self.total_latency = total_latency
         self.object_type = object_type
 
     def to_dict(self) -> Dict[str, Any]:
         hits = []
         for hits_item_data in self.hits:
             hits_item = []
             for hits_item_item_data in hits_item_data:
                 hits_item_item = hits_item_item_data.to_dict()
 
                 hits_item.append(hits_item_item)
 
             hits.append(hits_item)
 
-        query_time = self.query_time
-        response_time = self.response_time
+        query_latency = self.query_latency
+        total_latency = self.total_latency
         object_type: Union[Unset, str] = UNSET
         if not isinstance(self.object_type, Unset):
             object_type = self.object_type.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "hits": hits,
-                "query_time": query_time,
-                "response_time": response_time,
+                "query_latency": query_latency,
+                "total_latency": total_latency,
             }
         )
         if object_type is not UNSET:
             field_dict["object_type"] = object_type
 
         return field_dict
 
@@ -87,29 +87,29 @@
             for hits_item_item_data in _hits_item:
                 hits_item_item = Hit.from_dict(hits_item_item_data)
 
                 hits_item.append(hits_item_item)
 
             hits.append(hits_item)
 
-        query_time = d.pop("query_time")
+        query_latency = d.pop("query_latency")
 
-        response_time = d.pop("response_time")
+        total_latency = d.pop("total_latency")
 
         _object_type = unset_if_none(d, "object_type")
         object_type: Union[Unset, QueryResponseObjectType]
         if isinstance(_object_type, Unset):
             object_type = UNSET
         else:
             object_type = QueryResponseObjectType(_object_type)
 
         query_response = cls(
             hits=hits,
-            query_time=query_time,
-            response_time=response_time,
+            query_latency=query_latency,
+            total_latency=total_latency,
             object_type=object_type,
         )
 
         query_response.additional_properties = d
         return query_response
 
     @property
```

### Comparing `lectric-sdk-0.0.6a0/lectric/models/query_spec.py` & `lectric-sdk-0.0.9/lectric/models/query_spec.py`

 * *Files identical despite different names*

### Comparing `lectric-sdk-0.0.6a0/lectric/models/validation_error.py` & `lectric-sdk-0.0.9/lectric/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `lectric-sdk-0.0.6a0/lectric/models/vector_query_spec.py` & `lectric-sdk-0.0.9/lectric/models/vector_query_spec.py`

 * *Files identical despite different names*

### Comparing `lectric-sdk-0.0.6a0/lectric/types.py` & `lectric-sdk-0.0.9/lectric/types.py`

 * *Files identical despite different names*

### Comparing `lectric-sdk-0.0.6a0/setup.py` & `lectric-sdk-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,13 +21,14 @@
     keywords=['lectric', 'vdb', 'vector database'],
     classifiers=["Programming Language :: Python :: 3",
                  "Operating System :: OS Independent"],
     install_requires=[
         "setuptools>=41.0.1",
         "httpx>=0.23.0",
         "attrs>=21.4.0",
+        "wheel",
         "requests",
         "numpy"
     ],
     python_requires=">=3.6",
     zip_safe=False
 )
```

