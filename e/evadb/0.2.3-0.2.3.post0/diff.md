# Comparing `tmp/evadb-0.2.3.tar.gz` & `tmp/evadb-0.2.3.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evadb-0.2.3.tar", last modified: Fri May 12 02:30:51 2023, max compression
+gzip compressed data, was "evadb-0.2.3.post0.tar", last modified: Sat May 13 22:06:47 2023, max compression
```

## Comparing `evadb-0.2.3.tar` & `evadb-0.2.3.post0.tar`

### file list

```diff
@@ -1,461 +1,461 @@
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.267907 evadb-0.2.3/
--rw-r--r--   0 gtk        (501) staff       (20)    11357 2022-10-22 20:58:06.000000 evadb-0.2.3/LICENSE.txt
--rw-r--r--   0 gtk        (501) staff       (20)    14253 2023-05-12 02:30:51.267668 evadb-0.2.3/PKG-INFO
--rw-r--r--   0 gtk        (501) staff       (20)    13506 2023-05-12 01:08:04.000000 evadb-0.2.3/README.md
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.153537 evadb-0.2.3/eva/
--rw-r--r--   0 gtk        (501) staff       (20)      645 2022-10-22 20:58:06.000000 evadb-0.2.3/eva/__init__.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.154545 evadb-0.2.3/eva/binder/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2022-08-05 20:54:12.000000 evadb-0.2.3/eva/binder/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     4839 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/binder/binder_utils.py
--rw-r--r--   0 gtk        (501) staff       (20)    12812 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/binder/statement_binder.py
--rw-r--r--   0 gtk        (501) staff       (20)     8000 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/binder/statement_binder_context.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.156463 evadb-0.2.3/eva/catalog/
--rw-r--r--   0 gtk        (501) staff       (20)      616 2022-08-05 20:54:12.000000 evadb-0.2.3/eva/catalog/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)    18073 2023-05-12 01:08:04.000000 evadb-0.2.3/eva/catalog/catalog_manager.py
--rw-r--r--   0 gtk        (501) staff       (20)     3076 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/catalog/catalog_type.py
--rw-r--r--   0 gtk        (501) staff       (20)     6946 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/catalog/catalog_utils.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.158600 evadb-0.2.3/eva/catalog/models/
--rw-r--r--   0 gtk        (501) staff       (20)      886 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/catalog/models/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     1499 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/catalog/models/association_models.py
--rw-r--r--   0 gtk        (501) staff       (20)     4672 2023-05-12 01:08:04.000000 evadb-0.2.3/eva/catalog/models/base_model.py
--rw-r--r--   0 gtk        (501) staff       (20)     5110 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/catalog/models/column_catalog.py
--rw-r--r--   0 gtk        (501) staff       (20)     3274 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/catalog/models/index_catalog.py
--rw-r--r--   0 gtk        (501) staff       (20)     2997 2023-01-05 21:52:14.000000 evadb-0.2.3/eva/catalog/models/table_catalog.py
--rw-r--r--   0 gtk        (501) staff       (20)     3532 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/catalog/models/udf_cache_catalog.py
--rw-r--r--   0 gtk        (501) staff       (20)     4429 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/catalog/models/udf_catalog.py
--rw-r--r--   0 gtk        (501) staff       (20)     2262 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/catalog/models/udf_cost_catalog.py
--rw-r--r--   0 gtk        (501) staff       (20)     4722 2023-01-05 21:52:14.000000 evadb-0.2.3/eva/catalog/models/udf_io_catalog.py
--rw-r--r--   0 gtk        (501) staff       (20)     2668 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/catalog/models/udf_metadata_catalog.py
--rw-r--r--   0 gtk        (501) staff       (20)     2127 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/catalog/schema_utils.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.160313 evadb-0.2.3/eva/catalog/services/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2022-08-05 20:54:12.000000 evadb-0.2.3/eva/catalog/services/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     1167 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/catalog/services/base_service.py
--rw-r--r--   0 gtk        (501) staff       (20)     2873 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/catalog/services/column_catalog_service.py
--rw-r--r--   0 gtk        (501) staff       (20)     2887 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/catalog/services/index_catalog_service.py
--rw-r--r--   0 gtk        (501) staff       (20)     4571 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/catalog/services/table_catalog_service.py
--rw-r--r--   0 gtk        (501) staff       (20)     3669 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/catalog/services/udf_cache_catalog_service.py
--rw-r--r--   0 gtk        (501) staff       (20)     3078 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/catalog/services/udf_catalog_service.py
--rw-r--r--   0 gtk        (501) staff       (20)     2826 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/catalog/services/udf_cost_catalog_service.py
--rw-r--r--   0 gtk        (501) staff       (20)     2476 2023-01-05 21:52:14.000000 evadb-0.2.3/eva/catalog/services/udf_io_catalog_service.py
--rw-r--r--   0 gtk        (501) staff       (20)     1936 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/catalog/services/udf_metadata_catalog_service.py
--rw-r--r--   0 gtk        (501) staff       (20)     3119 2023-05-12 01:08:04.000000 evadb-0.2.3/eva/catalog/sql_config.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.161179 evadb-0.2.3/eva/configuration/
--rw-r--r--   0 gtk        (501) staff       (20)      620 2022-08-05 20:54:12.000000 evadb-0.2.3/eva/configuration/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     4200 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/configuration/bootstrap_environment.py
--rw-r--r--   0 gtk        (501) staff       (20)     4146 2023-05-12 01:08:04.000000 evadb-0.2.3/eva/configuration/configuration_manager.py
--rw-r--r--   0 gtk        (501) staff       (20)     1402 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/configuration/constants.py
--rw-r--r--   0 gtk        (501) staff       (20)      882 2023-05-12 01:08:04.000000 evadb-0.2.3/eva/constants.py
--rw-r--r--   0 gtk        (501) staff       (20)      787 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/eva.yml
--rw-r--r--   0 gtk        (501) staff       (20)     1553 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/eva_cmd_client.py
--rw-r--r--   0 gtk        (501) staff       (20)     2399 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/eva_server.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.172929 evadb-0.2.3/eva/executor/
--rw-r--r--   0 gtk        (501) staff       (20)      615 2022-08-05 20:54:12.000000 evadb-0.2.3/eva/executor/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     2137 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/executor/abstract_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     2214 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/executor/apply_and_merge_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     1530 2023-05-12 01:08:04.000000 evadb-0.2.3/eva/executor/create_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     5728 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/executor/create_index_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     3866 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/executor/create_mat_view_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     7642 2023-05-12 01:08:04.000000 evadb-0.2.3/eva/executor/create_udf_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     4738 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/executor/delete_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     2557 2023-05-12 01:08:04.000000 evadb-0.2.3/eva/executor/drop_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     2010 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/executor/drop_udf_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     3013 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/executor/execution_context.py
--rw-r--r--   0 gtk        (501) staff       (20)     3091 2023-05-12 01:08:04.000000 evadb-0.2.3/eva/executor/executor_utils.py
--rw-r--r--   0 gtk        (501) staff       (20)     1523 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/executor/explain_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     3507 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/executor/faiss_index_scan_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     1591 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/executor/function_scan_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     1759 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/executor/groupby_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     1800 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/executor/hash_join_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     2255 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/executor/insert_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     1616 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/executor/join_build_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     1661 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/executor/lateral_join_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     1583 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/executor/limit_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     3086 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/executor/load_csv_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     1579 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/executor/load_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     6065 2023-05-12 01:08:04.000000 evadb-0.2.3/eva/executor/load_multimedia_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     1488 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/executor/nested_loop_join_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     4183 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/executor/orderby_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     8071 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/executor/plan_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     1644 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/executor/pp_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     1277 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/executor/predicate_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     1272 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/executor/project_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     1186 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/executor/rename_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     1413 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/executor/sample_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     1812 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/executor/seq_scan_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     1870 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/executor/show_info_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     2274 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/executor/storage_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     1264 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/executor/union_executor.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.173113 evadb-0.2.3/eva/experimental/
--rw-r--r--   0 gtk        (501) staff       (20)      619 2022-11-03 02:51:44.000000 evadb-0.2.3/eva/experimental/__init__.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.173508 evadb-0.2.3/eva/experimental/ray/
--rw-r--r--   0 gtk        (501) staff       (20)      610 2022-11-06 23:44:54.000000 evadb-0.2.3/eva/experimental/ray/__init__.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.174650 evadb-0.2.3/eva/experimental/ray/executor/
--rw-r--r--   0 gtk        (501) staff       (20)      619 2022-11-03 02:51:43.000000 evadb-0.2.3/eva/experimental/ray/executor/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     3521 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/experimental/ray/executor/exchange_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     1431 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/experimental/ray/executor/ray_stage.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.174981 evadb-0.2.3/eva/experimental/ray/optimizer/
--rw-r--r--   0 gtk        (501) staff       (20)      620 2022-11-03 02:51:43.000000 evadb-0.2.3/eva/experimental/ray/optimizer/__init__.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.175572 evadb-0.2.3/eva/experimental/ray/optimizer/rules/
--rw-r--r--   0 gtk        (501) staff       (20)      626 2022-11-03 02:51:43.000000 evadb-0.2.3/eva/experimental/ray/optimizer/rules/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     4176 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/experimental/ray/optimizer/rules/rules.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.176156 evadb-0.2.3/eva/experimental/ray/planner/
--rw-r--r--   0 gtk        (501) staff       (20)      618 2022-11-03 02:51:44.000000 evadb-0.2.3/eva/experimental/ray/planner/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     1380 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/experimental/ray/planner/exchange_plan.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.181267 evadb-0.2.3/eva/expression/
--rw-r--r--   0 gtk        (501) staff       (20)      617 2022-08-05 20:54:12.000000 evadb-0.2.3/eva/expression/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     5469 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/expression/abstract_expression.py
--rw-r--r--   0 gtk        (501) staff       (20)     3974 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/expression/aggregation_expression.py
--rw-r--r--   0 gtk        (501) staff       (20)     1618 2022-11-03 02:51:43.000000 evadb-0.2.3/eva/expression/arithmetic_expression.py
--rw-r--r--   0 gtk        (501) staff       (20)     4351 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/expression/comparison_expression.py
--rw-r--r--   0 gtk        (501) staff       (20)     2542 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/expression/constant_value_expression.py
--rw-r--r--   0 gtk        (501) staff       (20)    10440 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/expression/expression_utils.py
--rw-r--r--   0 gtk        (501) staff       (20)    10171 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/expression/function_expression.py
--rw-r--r--   0 gtk        (501) staff       (20)     3055 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/expression/logical_expression.py
--rw-r--r--   0 gtk        (501) staff       (20)     4685 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/expression/tuple_value_expression.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.181767 evadb-0.2.3/eva/models/
--rw-r--r--   0 gtk        (501) staff       (20)      633 2022-08-05 20:54:12.000000 evadb-0.2.3/eva/models/__init__.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.182720 evadb-0.2.3/eva/models/catalog/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2022-08-05 20:54:12.000000 evadb-0.2.3/eva/models/catalog/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     1332 2022-10-22 20:58:06.000000 evadb-0.2.3/eva/models/catalog/frame_info.py
--rw-r--r--   0 gtk        (501) staff       (20)      857 2022-10-22 20:58:06.000000 evadb-0.2.3/eva/models/catalog/properties.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.183292 evadb-0.2.3/eva/models/server/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2022-08-05 20:54:12.000000 evadb-0.2.3/eva/models/server/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     1961 2023-05-12 01:08:04.000000 evadb-0.2.3/eva/models/server/response.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.183930 evadb-0.2.3/eva/models/storage/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2022-08-05 20:54:12.000000 evadb-0.2.3/eva/models/storage/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)    14837 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/models/storage/batch.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.189801 evadb-0.2.3/eva/optimizer/
--rw-r--r--   0 gtk        (501) staff       (20)      620 2022-08-05 20:54:12.000000 evadb-0.2.3/eva/optimizer/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     3260 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/optimizer/binder.py
--rw-r--r--   0 gtk        (501) staff       (20)     2129 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/optimizer/cost_model.py
--rw-r--r--   0 gtk        (501) staff       (20)     3450 2022-08-05 20:54:12.000000 evadb-0.2.3/eva/optimizer/group.py
--rw-r--r--   0 gtk        (501) staff       (20)     2669 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/optimizer/group_expression.py
--rw-r--r--   0 gtk        (501) staff       (20)     4335 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/optimizer/memo.py
--rw-r--r--   0 gtk        (501) staff       (20)    35842 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/optimizer/operators.py
--rw-r--r--   0 gtk        (501) staff       (20)     3838 2023-01-05 21:52:14.000000 evadb-0.2.3/eva/optimizer/optimizer_context.py
--rw-r--r--   0 gtk        (501) staff       (20)      982 2022-08-05 20:54:12.000000 evadb-0.2.3/eva/optimizer/optimizer_task_stack.py
--rw-r--r--   0 gtk        (501) staff       (20)    12579 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/optimizer/optimizer_tasks.py
--rw-r--r--   0 gtk        (501) staff       (20)    10874 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/optimizer/optimizer_utils.py
--rw-r--r--   0 gtk        (501) staff       (20)     5897 2023-05-12 01:08:04.000000 evadb-0.2.3/eva/optimizer/plan_generator.py
--rw-r--r--   0 gtk        (501) staff       (20)     1169 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/optimizer/property.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.191568 evadb-0.2.3/eva/optimizer/rules/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2022-08-05 20:54:12.000000 evadb-0.2.3/eva/optimizer/rules/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     1016 2022-08-05 20:54:12.000000 evadb-0.2.3/eva/optimizer/rules/pattern.py
--rw-r--r--   0 gtk        (501) staff       (20)    43623 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/optimizer/rules/rules.py
--rw-r--r--   0 gtk        (501) staff       (20)     7221 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/optimizer/rules/rules_base.py
--rw-r--r--   0 gtk        (501) staff       (20)     7743 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/optimizer/rules/rules_manager.py
--rw-r--r--   0 gtk        (501) staff       (20)    13132 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/optimizer/statement_to_opr_convertor.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.201240 evadb-0.2.3/eva/parser/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2022-08-05 20:54:12.000000 evadb-0.2.3/eva/parser/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     1360 2022-10-22 20:58:06.000000 evadb-0.2.3/eva/parser/alias.py
--rw-r--r--   0 gtk        (501) staff       (20)     2672 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/parser/create_index_statement.py
--rw-r--r--   0 gtk        (501) staff       (20)     2788 2023-01-05 21:52:14.000000 evadb-0.2.3/eva/parser/create_mat_view_statement.py
--rw-r--r--   0 gtk        (501) staff       (20)     4838 2023-01-05 21:52:14.000000 evadb-0.2.3/eva/parser/create_statement.py
--rw-r--r--   0 gtk        (501) staff       (20)     4882 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/parser/create_udf_statement.py
--rw-r--r--   0 gtk        (501) staff       (20)     2048 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/parser/delete_statement.py
--rw-r--r--   0 gtk        (501) staff       (20)     1767 2023-01-05 21:52:14.000000 evadb-0.2.3/eva/parser/drop_statement.py
--rw-r--r--   0 gtk        (501) staff       (20)     1793 2022-08-05 20:54:12.000000 evadb-0.2.3/eva/parser/drop_udf_statement.py
--rw-r--r--   0 gtk        (501) staff       (20)    19477 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/parser/eva.lark
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.204802 evadb-0.2.3/eva/parser/evaql/
--rw-r--r--   0 gtk        (501) staff       (20)    65109 2022-12-22 10:20:18.000000 evadb-0.2.3/eva/parser/evaql/evaql_lexer.py
--rw-r--r--   0 gtk        (501) staff       (20)   408798 2022-12-22 10:20:18.000000 evadb-0.2.3/eva/parser/evaql/evaql_parser.py
--rw-r--r--   0 gtk        (501) staff       (20)    44890 2022-12-22 10:20:18.000000 evadb-0.2.3/eva/parser/evaql/evaql_parserListener.py
--rw-r--r--   0 gtk        (501) staff       (20)    26541 2022-12-22 10:20:18.000000 evadb-0.2.3/eva/parser/evaql/evaql_parserVisitor.py
--rw-r--r--   0 gtk        (501) staff       (20)     1384 2022-11-04 06:56:00.000000 evadb-0.2.3/eva/parser/explain_statement.py
--rw-r--r--   0 gtk        (501) staff       (20)     2922 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/parser/insert_statement.py
--rw-r--r--   0 gtk        (501) staff       (20)     1717 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/parser/lark_parser.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.208541 evadb-0.2.3/eva/parser/lark_visitor/
--rw-r--r--   0 gtk        (501) staff       (20)     2655 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/parser/lark_visitor/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     2161 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/parser/lark_visitor/_common_clauses_ids.py
--rw-r--r--   0 gtk        (501) staff       (20)    10502 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/parser/lark_visitor/_create_statements.py
--rw-r--r--   0 gtk        (501) staff       (20)     1404 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/parser/lark_visitor/_delete_statement.py
--rw-r--r--   0 gtk        (501) staff       (20)     1202 2023-01-05 21:52:14.000000 evadb-0.2.3/eva/parser/lark_visitor/_drop_statement.py
--rw-r--r--   0 gtk        (501) staff       (20)     1006 2023-01-05 21:52:14.000000 evadb-0.2.3/eva/parser/lark_visitor/_explain_statement.py
--rw-r--r--   0 gtk        (501) staff       (20)     4672 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/parser/lark_visitor/_expressions.py
--rw-r--r--   0 gtk        (501) staff       (20)     6231 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/parser/lark_visitor/_functions.py
--rw-r--r--   0 gtk        (501) staff       (20)     2465 2023-01-05 21:52:14.000000 evadb-0.2.3/eva/parser/lark_visitor/_insert_statements.py
--rw-r--r--   0 gtk        (501) staff       (20)     2057 2023-01-05 21:52:14.000000 evadb-0.2.3/eva/parser/lark_visitor/_load_statement.py
--rw-r--r--   0 gtk        (501) staff       (20)      932 2023-01-05 21:52:14.000000 evadb-0.2.3/eva/parser/lark_visitor/_rename_statement.py
--rw-r--r--   0 gtk        (501) staff       (20)     2143 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/parser/lark_visitor/_select_statement.py
--rw-r--r--   0 gtk        (501) staff       (20)     1112 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/parser/lark_visitor/_show_statements.py
--rw-r--r--   0 gtk        (501) staff       (20)     9468 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/parser/lark_visitor/_table_sources.py
--rw-r--r--   0 gtk        (501) staff       (20)     3214 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/parser/load_statement.py
--rw-r--r--   0 gtk        (501) staff       (20)     1228 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/parser/parser.py
--rw-r--r--   0 gtk        (501) staff       (20)     2007 2023-01-05 21:52:14.000000 evadb-0.2.3/eva/parser/rename_statement.py
--rw-r--r--   0 gtk        (501) staff       (20)     5921 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/parser/select_statement.py
--rw-r--r--   0 gtk        (501) staff       (20)     1460 2023-01-05 21:52:14.000000 evadb-0.2.3/eva/parser/show_statement.py
--rw-r--r--   0 gtk        (501) staff       (20)     1052 2022-08-05 20:54:12.000000 evadb-0.2.3/eva/parser/statement.py
--rw-r--r--   0 gtk        (501) staff       (20)     8639 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/parser/table_ref.py
--rw-r--r--   0 gtk        (501) staff       (20)     1679 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/parser/types.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.216073 evadb-0.2.3/eva/plan_nodes/
--rw-r--r--   0 gtk        (501) staff       (20)      614 2022-12-22 07:29:52.000000 evadb-0.2.3/eva/plan_nodes/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     1689 2022-12-22 07:29:52.000000 evadb-0.2.3/eva/plan_nodes/abstract_join_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     3453 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/plan_nodes/abstract_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     1455 2022-12-22 07:29:52.000000 evadb-0.2.3/eva/plan_nodes/abstract_scan_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     1930 2023-01-05 21:52:14.000000 evadb-0.2.3/eva/plan_nodes/apply_and_merge_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     2401 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/plan_nodes/create_index_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     2076 2023-01-05 21:54:27.000000 evadb-0.2.3/eva/plan_nodes/create_mat_view_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     2200 2023-01-05 21:52:14.000000 evadb-0.2.3/eva/plan_nodes/create_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     3603 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/plan_nodes/create_udf_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     1951 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/plan_nodes/delete_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     1660 2022-12-22 07:29:52.000000 evadb-0.2.3/eva/plan_nodes/drop_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     1532 2022-12-22 07:29:52.000000 evadb-0.2.3/eva/plan_nodes/drop_udf_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     1033 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/plan_nodes/explain_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     2355 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/plan_nodes/faiss_index_scan_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     1755 2022-12-22 07:29:52.000000 evadb-0.2.3/eva/plan_nodes/function_scan_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     1499 2022-12-22 07:29:52.000000 evadb-0.2.3/eva/plan_nodes/groupby_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     1712 2023-01-05 21:52:14.000000 evadb-0.2.3/eva/plan_nodes/hash_join_build_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     2179 2023-01-05 21:52:14.000000 evadb-0.2.3/eva/plan_nodes/hash_join_probe_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     2023 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/plan_nodes/insert_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     1408 2023-01-05 21:52:14.000000 evadb-0.2.3/eva/plan_nodes/lateral_join_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     1468 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/plan_nodes/limit_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     2710 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/plan_nodes/load_data_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     1510 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/plan_nodes/nested_loop_join_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     1564 2022-12-22 07:29:52.000000 evadb-0.2.3/eva/plan_nodes/orderby_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     1177 2022-12-22 07:29:52.000000 evadb-0.2.3/eva/plan_nodes/pp_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     1245 2022-12-22 07:29:52.000000 evadb-0.2.3/eva/plan_nodes/predicate_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     1249 2022-12-22 07:29:52.000000 evadb-0.2.3/eva/plan_nodes/project_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     1616 2022-12-22 07:29:52.000000 evadb-0.2.3/eva/plan_nodes/rename_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     1469 2022-12-22 07:29:52.000000 evadb-0.2.3/eva/plan_nodes/sample_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     1760 2022-12-22 07:29:52.000000 evadb-0.2.3/eva/plan_nodes/seq_scan_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     1201 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/plan_nodes/show_info_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     4419 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/plan_nodes/storage_plan.py
--rw-r--r--   0 gtk        (501) staff       (20)     1420 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/plan_nodes/types.py
--rw-r--r--   0 gtk        (501) staff       (20)     1245 2022-12-22 07:29:52.000000 evadb-0.2.3/eva/plan_nodes/union_plan.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.216839 evadb-0.2.3/eva/readers/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2022-08-05 20:54:12.000000 evadb-0.2.3/eva/readers/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     2320 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/readers/abstract_reader.py
--rw-r--r--   0 gtk        (501) staff       (20)     2651 2022-12-22 07:29:52.000000 evadb-0.2.3/eva/readers/csv_reader.py
--rw-r--r--   0 gtk        (501) staff       (20)     5986 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/readers/decord_reader.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.217223 evadb-0.2.3/eva/readers/image/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2022-12-22 07:29:52.000000 evadb-0.2.3/eva/readers/image/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     1067 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/readers/image/opencv_image_reader.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.218535 evadb-0.2.3/eva/server/
--rw-r--r--   0 gtk        (501) staff       (20)      623 2022-08-05 20:54:12.000000 evadb-0.2.3/eva/server/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     3297 2023-05-12 01:08:04.000000 evadb-0.2.3/eva/server/command_handler.py
--rw-r--r--   0 gtk        (501) staff       (20)     3502 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/server/db_api.py
--rw-r--r--   0 gtk        (501) staff       (20)     3276 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/server/interpreter.py
--rw-r--r--   0 gtk        (501) staff       (20)     2866 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/server/server.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.220217 evadb-0.2.3/eva/storage/
--rw-r--r--   0 gtk        (501) staff       (20)      616 2022-08-05 20:54:12.000000 evadb-0.2.3/eva/storage/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     6132 2023-05-12 01:08:04.000000 evadb-0.2.3/eva/storage/abstract_media_storage_engine.py
--rw-r--r--   0 gtk        (501) staff       (20)     2385 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/storage/abstract_storage_engine.py
--rw-r--r--   0 gtk        (501) staff       (20)     1717 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/storage/image_storage_engine.py
--rw-r--r--   0 gtk        (501) staff       (20)     8881 2023-05-12 01:07:44.000000 evadb-0.2.3/eva/storage/sqlite_storage_engine.py
--rw-r--r--   0 gtk        (501) staff       (20)     1688 2023-01-05 21:52:14.000000 evadb-0.2.3/eva/storage/storage_engine.py
--rw-r--r--   0 gtk        (501) staff       (20)     2496 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/storage/video_storage_engine.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.220470 evadb-0.2.3/eva/third_party/
--rw-r--r--   0 gtk        (501) staff       (20)      605 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/third_party/__init__.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.221355 evadb-0.2.3/eva/third_party/huggingface/
--rw-r--r--   0 gtk        (501) staff       (20)      619 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/third_party/huggingface/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     1420 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/third_party/huggingface/binder.py
--rw-r--r--   0 gtk        (501) staff       (20)     6403 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/third_party/huggingface/create.py
--rw-r--r--   0 gtk        (501) staff       (20)     2615 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/third_party/huggingface/model.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.224298 evadb-0.2.3/eva/udfs/
--rw-r--r--   0 gtk        (501) staff       (20)      616 2022-08-05 20:54:12.000000 evadb-0.2.3/eva/udfs/__init__.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.225303 evadb-0.2.3/eva/udfs/abstract/
--rw-r--r--   0 gtk        (501) staff       (20)      625 2022-11-06 23:44:54.000000 evadb-0.2.3/eva/udfs/abstract/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     2441 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/udfs/abstract/abstract_udf.py
--rw-r--r--   0 gtk        (501) staff       (20)     3945 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/udfs/abstract/hf_abstract_udf.py
--rw-r--r--   0 gtk        (501) staff       (20)     3843 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/udfs/abstract/pytorch_abstract_udf.py
--rw-r--r--   0 gtk        (501) staff       (20)     3464 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/udfs/asl_action_recognition.py
--rw-r--r--   0 gtk        (501) staff       (20)     3218 2023-05-12 01:08:04.000000 evadb-0.2.3/eva/udfs/chatgpt.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.226016 evadb-0.2.3/eva/udfs/decorators/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/udfs/decorators/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     2185 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/udfs/decorators/decorators.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.226770 evadb-0.2.3/eva/udfs/decorators/io_descriptors/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/udfs/decorators/io_descriptors/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     2754 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/udfs/decorators/io_descriptors/abstract_types.py
--rw-r--r--   0 gtk        (501) staff       (20)     3375 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/udfs/decorators/io_descriptors/data_types.py
--rw-r--r--   0 gtk        (501) staff       (20)     1437 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/udfs/decorators/utils.py
--rw-r--r--   0 gtk        (501) staff       (20)     5478 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/udfs/emotion_detector.py
--rw-r--r--   0 gtk        (501) staff       (20)     2539 2023-01-05 21:52:14.000000 evadb-0.2.3/eva/udfs/face_detector.py
--rw-r--r--   0 gtk        (501) staff       (20)     5998 2023-05-12 01:08:04.000000 evadb-0.2.3/eva/udfs/fastrcnn_object_detector.py
--rw-r--r--   0 gtk        (501) staff       (20)     1822 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/udfs/feature_extractor.py
--rw-r--r--   0 gtk        (501) staff       (20)     1028 2022-10-22 20:58:06.000000 evadb-0.2.3/eva/udfs/gpu_compatible.py
--rw-r--r--   0 gtk        (501) staff       (20)     2200 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/udfs/mvit_action_recognition.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.228238 evadb-0.2.3/eva/udfs/ndarray/
--rw-r--r--   0 gtk        (501) staff       (20)      638 2022-10-22 20:58:06.000000 evadb-0.2.3/eva/udfs/ndarray/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     2568 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/udfs/ndarray/array_count.py
--rw-r--r--   0 gtk        (501) staff       (20)     1647 2022-11-04 07:07:40.000000 evadb-0.2.3/eva/udfs/ndarray/crop.py
--rw-r--r--   0 gtk        (501) staff       (20)     1179 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/udfs/ndarray/fuzzy_join.py
--rw-r--r--   0 gtk        (501) staff       (20)     1557 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/udfs/ndarray/open.py
--rw-r--r--   0 gtk        (501) staff       (20)     1782 2022-12-22 07:29:52.000000 evadb-0.2.3/eva/udfs/ndarray/similarity.py
--rw-r--r--   0 gtk        (501) staff       (20)     2750 2023-01-05 21:52:14.000000 evadb-0.2.3/eva/udfs/ocr_extractor.py
--rw-r--r--   0 gtk        (501) staff       (20)     7165 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/udfs/udf_bootstrap_queries.py
--rw-r--r--   0 gtk        (501) staff       (20)     3858 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/udfs/yolo_object_detector.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.229832 evadb-0.2.3/eva/utils/
--rw-r--r--   0 gtk        (501) staff       (20)      611 2022-08-05 20:54:12.000000 evadb-0.2.3/eva/utils/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)      909 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/utils/errors.py
--rw-r--r--   0 gtk        (501) staff       (20)     6969 2023-05-12 01:08:04.000000 evadb-0.2.3/eva/utils/generic_utils.py
--rw-r--r--   0 gtk        (501) staff       (20)     1956 2023-05-04 20:52:14.000000 evadb-0.2.3/eva/utils/kv_cache.py
--rw-r--r--   0 gtk        (501) staff       (20)      985 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/utils/logging_manager.py
--rw-r--r--   0 gtk        (501) staff       (20)     1562 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/utils/s3_utils.py
--rw-r--r--   0 gtk        (501) staff       (20)     1692 2023-04-04 16:52:32.000000 evadb-0.2.3/eva/utils/stats.py
--rw-r--r--   0 gtk        (501) staff       (20)      711 2023-05-12 02:29:55.000000 evadb-0.2.3/eva/version.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.230627 evadb-0.2.3/evadb.egg-info/
--rw-r--r--   0 gtk        (501) staff       (20)    14253 2023-05-12 02:30:51.000000 evadb-0.2.3/evadb.egg-info/PKG-INFO
--rw-r--r--   0 gtk        (501) staff       (20)    13509 2023-05-12 02:30:51.000000 evadb-0.2.3/evadb.egg-info/SOURCES.txt
--rw-r--r--   0 gtk        (501) staff       (20)        1 2023-05-12 02:30:51.000000 evadb-0.2.3/evadb.egg-info/dependency_links.txt
--rw-r--r--   0 gtk        (501) staff       (20)       88 2023-05-12 02:30:51.000000 evadb-0.2.3/evadb.egg-info/entry_points.txt
--rw-r--r--   0 gtk        (501) staff       (20)     1135 2023-05-12 02:30:51.000000 evadb-0.2.3/evadb.egg-info/requires.txt
--rw-r--r--   0 gtk        (501) staff       (20)       21 2023-05-12 02:30:51.000000 evadb-0.2.3/evadb.egg-info/top_level.txt
--rw-r--r--   0 gtk        (501) staff       (20)       90 2022-06-05 21:10:08.000000 evadb-0.2.3/pyproject.toml
--rw-r--r--   0 gtk        (501) staff       (20)       38 2023-05-12 02:30:51.267953 evadb-0.2.3/setup.cfg
--rw-r--r--   0 gtk        (501) staff       (20)     4139 2023-05-12 01:08:04.000000 evadb-0.2.3/setup.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.233038 evadb-0.2.3/test/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2022-10-22 20:58:06.000000 evadb-0.2.3/test/__init__.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.235065 evadb-0.2.3/test/benchmark_tests/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2023-01-05 21:52:14.000000 evadb-0.2.3/test/benchmark_tests/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     1176 2023-05-04 20:52:14.000000 evadb-0.2.3/test/benchmark_tests/conftest.py
--rw-r--r--   0 gtk        (501) staff       (20)     6639 2023-05-12 01:08:04.000000 evadb-0.2.3/test/benchmark_tests/test_benchmark_pytorch.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.238650 evadb-0.2.3/test/binder/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2022-08-05 20:54:12.000000 evadb-0.2.3/test/binder/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     2032 2023-01-05 21:52:14.000000 evadb-0.2.3/test/binder/test_binder_utils.py
--rw-r--r--   0 gtk        (501) staff       (20)    14016 2023-04-04 16:52:32.000000 evadb-0.2.3/test/binder/test_statement_binder.py
--rw-r--r--   0 gtk        (501) staff       (20)     7961 2023-04-04 16:52:32.000000 evadb-0.2.3/test/binder/test_statement_binder_context.py
--rw-r--r--   0 gtk        (501) staff       (20)     1796 2022-12-04 01:29:24.000000 evadb-0.2.3/test/binder/test_statement_binder_python37.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.239783 evadb-0.2.3/test/catalog/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2022-08-05 20:54:12.000000 evadb-0.2.3/test/catalog/__init__.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.240428 evadb-0.2.3/test/catalog/models/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2022-08-05 20:54:12.000000 evadb-0.2.3/test/catalog/models/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     7234 2023-04-04 16:52:32.000000 evadb-0.2.3/test/catalog/models/test_models.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.242097 evadb-0.2.3/test/catalog/services/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2022-08-05 20:54:12.000000 evadb-0.2.3/test/catalog/services/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     1918 2023-01-05 21:52:14.000000 evadb-0.2.3/test/catalog/services/test_column_catalog_service.py
--rw-r--r--   0 gtk        (501) staff       (20)     4745 2023-05-04 20:52:14.000000 evadb-0.2.3/test/catalog/services/test_index_catalog_service.py
--rw-r--r--   0 gtk        (501) staff       (20)     3639 2023-04-04 16:52:32.000000 evadb-0.2.3/test/catalog/services/test_table_catalog_service.py
--rw-r--r--   0 gtk        (501) staff       (20)     3639 2023-04-04 16:52:32.000000 evadb-0.2.3/test/catalog/services/test_udf_catalog_service.py
--rw-r--r--   0 gtk        (501) staff       (20)     3210 2023-04-04 16:52:32.000000 evadb-0.2.3/test/catalog/services/test_udf_cost_catalog_service.py
--rw-r--r--   0 gtk        (501) staff       (20)     3035 2023-04-04 16:52:32.000000 evadb-0.2.3/test/catalog/services/test_udf_io_catalog_service.py
--rw-r--r--   0 gtk        (501) staff       (20)     6808 2023-05-12 01:08:04.000000 evadb-0.2.3/test/catalog/test_catalog_manager.py
--rw-r--r--   0 gtk        (501) staff       (20)     1402 2022-12-04 01:29:24.000000 evadb-0.2.3/test/catalog/test_column_type.py
--rw-r--r--   0 gtk        (501) staff       (20)     1910 2023-04-04 16:52:32.000000 evadb-0.2.3/test/catalog/test_sqlalchemy.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.242686 evadb-0.2.3/test/configuration/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2022-08-05 20:54:12.000000 evadb-0.2.3/test/configuration/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     1490 2022-10-22 20:58:06.000000 evadb-0.2.3/test/configuration/test_bootstrap_environment.py
--rw-r--r--   0 gtk        (501) staff       (20)     1616 2023-05-12 01:08:04.000000 evadb-0.2.3/test/configuration/test_configuration_manager.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.245916 evadb-0.2.3/test/executor/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2022-08-05 20:54:12.000000 evadb-0.2.3/test/executor/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     1106 2023-04-04 16:52:32.000000 evadb-0.2.3/test/executor/test_abstract_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     2441 2022-12-22 07:29:52.000000 evadb-0.2.3/test/executor/test_create_mat_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     3987 2023-04-04 16:52:32.000000 evadb-0.2.3/test/executor/test_create_udf_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     4227 2023-05-04 20:52:14.000000 evadb-0.2.3/test/executor/test_execution_context.py
--rw-r--r--   0 gtk        (501) staff       (20)     1275 2022-12-22 06:08:34.000000 evadb-0.2.3/test/executor/test_executor_utils.py
--rw-r--r--   0 gtk        (501) staff       (20)     4650 2022-12-22 07:29:52.000000 evadb-0.2.3/test/executor/test_limit_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     3890 2023-04-04 16:52:32.000000 evadb-0.2.3/test/executor/test_load_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     2884 2022-12-22 07:29:52.000000 evadb-0.2.3/test/executor/test_orderby_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)    10986 2023-04-04 16:52:32.000000 evadb-0.2.3/test/executor/test_plan_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     1397 2022-08-05 20:54:12.000000 evadb-0.2.3/test/executor/test_pp_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     1817 2022-12-22 07:29:52.000000 evadb-0.2.3/test/executor/test_sample_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     2752 2023-05-04 20:52:14.000000 evadb-0.2.3/test/executor/test_seq_scan_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)      847 2022-08-09 16:07:02.000000 evadb-0.2.3/test/executor/utils.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.248263 evadb-0.2.3/test/expression/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2022-08-05 20:54:12.000000 evadb-0.2.3/test/expression/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     3722 2023-04-04 16:52:32.000000 evadb-0.2.3/test/expression/test_abstract_expression.py
--rw-r--r--   0 gtk        (501) staff       (20)     5149 2023-01-05 21:52:14.000000 evadb-0.2.3/test/expression/test_aggregation.py
--rw-r--r--   0 gtk        (501) staff       (20)     2975 2022-12-22 07:29:52.000000 evadb-0.2.3/test/expression/test_arithmetic.py
--rw-r--r--   0 gtk        (501) staff       (20)     5578 2023-01-05 21:52:14.000000 evadb-0.2.3/test/expression/test_comparison.py
--rw-r--r--   0 gtk        (501) staff       (20)     2867 2022-08-05 20:54:12.000000 evadb-0.2.3/test/expression/test_expression_tree.py
--rw-r--r--   0 gtk        (501) staff       (20)     7555 2023-04-04 16:52:32.000000 evadb-0.2.3/test/expression/test_expression_utils.py
--rw-r--r--   0 gtk        (501) staff       (20)     2685 2022-11-03 02:51:43.000000 evadb-0.2.3/test/expression/test_function_expression.py
--rw-r--r--   0 gtk        (501) staff       (20)    10242 2023-05-04 20:52:14.000000 evadb-0.2.3/test/expression/test_logical.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.255030 evadb-0.2.3/test/integration_tests/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2022-08-05 20:54:12.000000 evadb-0.2.3/test/integration_tests/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     3585 2023-05-04 20:52:14.000000 evadb-0.2.3/test/integration_tests/test_array_count.py
--rw-r--r--   0 gtk        (501) staff       (20)     4522 2023-05-12 01:08:04.000000 evadb-0.2.3/test/integration_tests/test_chatgpt.py
--rw-r--r--   0 gtk        (501) staff       (20)     7645 2023-05-04 20:52:14.000000 evadb-0.2.3/test/integration_tests/test_create_index_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     1091 2023-04-04 16:52:32.000000 evadb-0.2.3/test/integration_tests/test_create_table_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     5158 2023-05-04 20:52:14.000000 evadb-0.2.3/test/integration_tests/test_delete_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     4839 2023-04-04 16:52:32.000000 evadb-0.2.3/test/integration_tests/test_drop_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     2569 2023-05-04 20:52:14.000000 evadb-0.2.3/test/integration_tests/test_error_handling_with_ray.py
--rw-r--r--   0 gtk        (501) staff       (20)     4086 2023-05-04 20:52:14.000000 evadb-0.2.3/test/integration_tests/test_explain_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     3183 2023-05-04 20:52:14.000000 evadb-0.2.3/test/integration_tests/test_fuzzy_join.py
--rw-r--r--   0 gtk        (501) staff       (20)    13961 2023-05-12 01:08:04.000000 evadb-0.2.3/test/integration_tests/test_huggingface_udfs.py
--rw-r--r--   0 gtk        (501) staff       (20)     3806 2023-05-12 01:08:04.000000 evadb-0.2.3/test/integration_tests/test_insert_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     2900 2023-05-04 20:52:14.000000 evadb-0.2.3/test/integration_tests/test_like.py
--rw-r--r--   0 gtk        (501) staff       (20)    20623 2023-05-12 01:08:04.000000 evadb-0.2.3/test/integration_tests/test_load_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     5227 2023-05-04 20:52:14.000000 evadb-0.2.3/test/integration_tests/test_mat_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     2658 2023-05-04 20:52:14.000000 evadb-0.2.3/test/integration_tests/test_open.py
--rw-r--r--   0 gtk        (501) staff       (20)    10182 2023-05-04 20:52:14.000000 evadb-0.2.3/test/integration_tests/test_optimizer_rules.py
--rw-r--r--   0 gtk        (501) staff       (20)    10696 2023-05-04 20:52:14.000000 evadb-0.2.3/test/integration_tests/test_pytorch.py
--rw-r--r--   0 gtk        (501) staff       (20)     2953 2023-04-04 16:52:32.000000 evadb-0.2.3/test/integration_tests/test_rename_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     9958 2023-05-12 01:08:04.000000 evadb-0.2.3/test/integration_tests/test_reuse.py
--rw-r--r--   0 gtk        (501) staff       (20)     5210 2023-05-04 20:52:14.000000 evadb-0.2.3/test/integration_tests/test_s3_load_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)    30781 2023-05-04 20:52:14.000000 evadb-0.2.3/test/integration_tests/test_select_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     3277 2023-05-04 20:52:14.000000 evadb-0.2.3/test/integration_tests/test_show_info_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)    12287 2023-05-04 20:52:14.000000 evadb-0.2.3/test/integration_tests/test_similarity.py
--rw-r--r--   0 gtk        (501) staff       (20)    12062 2023-05-04 20:52:14.000000 evadb-0.2.3/test/integration_tests/test_udf_executor.py
--rw-r--r--   0 gtk        (501) staff       (20)     1449 2023-05-12 01:08:04.000000 evadb-0.2.3/test/markers.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.255348 evadb-0.2.3/test/models/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2022-08-05 20:54:12.000000 evadb-0.2.3/test/models/__init__.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.255870 evadb-0.2.3/test/models/catalog/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2022-08-05 20:54:12.000000 evadb-0.2.3/test/models/catalog/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     1010 2022-10-22 20:58:06.000000 evadb-0.2.3/test/models/catalog/test_frame_info.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.256334 evadb-0.2.3/test/models/storage/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2022-08-05 20:54:12.000000 evadb-0.2.3/test/models/storage/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     5919 2023-05-04 20:52:14.000000 evadb-0.2.3/test/models/storage/test_batch.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.258778 evadb-0.2.3/test/optimizer/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2022-08-05 20:54:12.000000 evadb-0.2.3/test/optimizer/__init__.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.259261 evadb-0.2.3/test/optimizer/rules/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2023-04-04 16:52:32.000000 evadb-0.2.3/test/optimizer/rules/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)    11829 2023-05-04 20:52:14.000000 evadb-0.2.3/test/optimizer/rules/test_rules.py
--rw-r--r--   0 gtk        (501) staff       (20)     4195 2023-04-04 16:52:32.000000 evadb-0.2.3/test/optimizer/test_binder.py
--rw-r--r--   0 gtk        (501) staff       (20)     4377 2023-05-04 20:52:14.000000 evadb-0.2.3/test/optimizer/test_cascade_optimizer.py
--rw-r--r--   0 gtk        (501) staff       (20)     4406 2022-08-05 20:54:12.000000 evadb-0.2.3/test/optimizer/test_cost_model.py
--rw-r--r--   0 gtk        (501) staff       (20)     2689 2022-08-05 20:54:12.000000 evadb-0.2.3/test/optimizer/test_group.py
--rw-r--r--   0 gtk        (501) staff       (20)     1996 2022-08-05 20:54:12.000000 evadb-0.2.3/test/optimizer/test_memo.py
--rw-r--r--   0 gtk        (501) staff       (20)     1034 2022-08-05 20:54:12.000000 evadb-0.2.3/test/optimizer/test_optimizer_context.py
--rw-r--r--   0 gtk        (501) staff       (20)     6122 2023-05-04 20:52:14.000000 evadb-0.2.3/test/optimizer/test_optimizer_task.py
--rw-r--r--   0 gtk        (501) staff       (20)     2000 2023-01-05 21:52:14.000000 evadb-0.2.3/test/optimizer/test_optimizer_utils.py
--rw-r--r--   0 gtk        (501) staff       (20)    13335 2023-04-04 16:52:32.000000 evadb-0.2.3/test/optimizer/test_statement_to_opr_convertor.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.260012 evadb-0.2.3/test/parser/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2022-08-05 20:54:12.000000 evadb-0.2.3/test/parser/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)    36047 2023-05-04 20:52:14.000000 evadb-0.2.3/test/parser/test_parser.py
--rw-r--r--   0 gtk        (501) staff       (20)     7781 2023-05-04 20:52:14.000000 evadb-0.2.3/test/parser/test_parser_statements.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.260501 evadb-0.2.3/test/plan_nodes/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2022-12-22 07:29:52.000000 evadb-0.2.3/test/plan_nodes/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     6292 2023-04-04 16:52:32.000000 evadb-0.2.3/test/plan_nodes/test_plan.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.261140 evadb-0.2.3/test/readers/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2022-08-05 20:54:12.000000 evadb-0.2.3/test/readers/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     1688 2023-04-04 16:52:32.000000 evadb-0.2.3/test/readers/test_csv_reader.py
--rw-r--r--   0 gtk        (501) staff       (20)     8104 2023-05-04 20:52:14.000000 evadb-0.2.3/test/readers/test_decord_reader.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.262298 evadb-0.2.3/test/server/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2022-11-04 07:07:40.000000 evadb-0.2.3/test/server/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     1268 2023-01-05 21:52:14.000000 evadb-0.2.3/test/server/test_command_handler.py
--rw-r--r--   0 gtk        (501) staff       (20)     5057 2023-04-04 16:52:32.000000 evadb-0.2.3/test/server/test_db_api.py
--rw-r--r--   0 gtk        (501) staff       (20)     2581 2023-04-04 16:52:32.000000 evadb-0.2.3/test/server/test_interpreter.py
--rw-r--r--   0 gtk        (501) staff       (20)     2066 2023-04-04 16:52:32.000000 evadb-0.2.3/test/server/test_server.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.262877 evadb-0.2.3/test/storage/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2022-08-05 20:54:12.000000 evadb-0.2.3/test/storage/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     4113 2023-05-04 20:52:14.000000 evadb-0.2.3/test/storage/test_sqlite_storage_engine.py
--rw-r--r--   0 gtk        (501) staff       (20)     4023 2023-04-04 16:52:32.000000 evadb-0.2.3/test/storage/test_video_storage.py
--rw-r--r--   0 gtk        (501) staff       (20)     1801 2023-04-04 16:52:32.000000 evadb-0.2.3/test/test_eva_cmd_client.py
--rw-r--r--   0 gtk        (501) staff       (20)     1294 2022-12-22 07:29:52.000000 evadb-0.2.3/test/test_eva_imports.py
--rw-r--r--   0 gtk        (501) staff       (20)     1810 2023-04-04 16:52:32.000000 evadb-0.2.3/test/test_eva_server.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.264000 evadb-0.2.3/test/udfs/
--rw-r--r--   0 gtk        (501) staff       (20)      638 2022-08-05 20:54:12.000000 evadb-0.2.3/test/udfs/__init__.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.264260 evadb-0.2.3/test/udfs/decorators/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2023-04-04 16:52:32.000000 evadb-0.2.3/test/udfs/decorators/__init__.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.264542 evadb-0.2.3/test/udfs/decorators/io_descriptors/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2023-04-04 16:52:32.000000 evadb-0.2.3/test/udfs/decorators/io_descriptors/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     7430 2023-04-04 16:52:32.000000 evadb-0.2.3/test/udfs/decorators/io_descriptors/test_descriptors.py
--rw-r--r--   0 gtk        (501) staff       (20)     2134 2023-04-04 16:52:32.000000 evadb-0.2.3/test/udfs/decorators/test_decorators.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.265256 evadb-0.2.3/test/udfs/ndarray/
--rw-r--r--   0 gtk        (501) staff       (20)      648 2022-10-22 20:58:06.000000 evadb-0.2.3/test/udfs/ndarray/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)      849 2023-04-04 16:52:32.000000 evadb-0.2.3/test/udfs/ndarray/test_array_count.py
--rw-r--r--   0 gtk        (501) staff       (20)     2410 2022-10-22 20:58:06.000000 evadb-0.2.3/test/udfs/ndarray/test_crop.py
--rw-r--r--   0 gtk        (501) staff       (20)     2374 2023-05-04 20:52:14.000000 evadb-0.2.3/test/udfs/ndarray/test_open.py
--rw-r--r--   0 gtk        (501) staff       (20)     4412 2023-05-12 01:08:04.000000 evadb-0.2.3/test/udfs/test_abstract_udf.py
--rw-r--r--   0 gtk        (501) staff       (20)     2154 2022-10-22 20:58:06.000000 evadb-0.2.3/test/udfs/test_emotion_detector.py
--rw-r--r--   0 gtk        (501) staff       (20)     3345 2023-04-04 16:52:32.000000 evadb-0.2.3/test/udfs/test_facenet_udf.py
--rw-r--r--   0 gtk        (501) staff       (20)     2548 2022-08-05 20:54:12.000000 evadb-0.2.3/test/udfs/test_fastrcnn_object_detector.py
--rw-r--r--   0 gtk        (501) staff       (20)     2768 2023-05-04 20:52:14.000000 evadb-0.2.3/test/udfs/test_yolo_object_detector.py
--rw-r--r--   0 gtk        (501) staff       (20)    17437 2023-05-12 01:08:04.000000 evadb-0.2.3/test/util.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.267315 evadb-0.2.3/test/utils/
--rw-r--r--   0 gtk        (501) staff       (20)      587 2022-08-05 20:54:12.000000 evadb-0.2.3/test/utils/__init__.py
--rw-r--r--   0 gtk        (501) staff       (20)     4196 2023-05-04 20:52:14.000000 evadb-0.2.3/test/utils/test_generic_utils.py
--rw-r--r--   0 gtk        (501) staff       (20)     2256 2023-04-04 16:52:32.000000 evadb-0.2.3/test/utils/test_timer.py
--rw-r--r--   0 gtk        (501) staff       (20)     2199 2023-05-12 01:08:04.000000 evadb-0.2.3/test/utils/test_xdist.py
-drwxr-xr-x   0 gtk        (501) staff       (20)        0 2023-05-12 02:30:51.267477 evadb-0.2.3/third_party/
--rw-r--r--   0 gtk        (501) staff       (20)        0 2022-06-05 21:10:08.000000 evadb-0.2.3/third_party/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.607631 evadb-0.2.3.post0/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    11357 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/LICENSE.txt
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    16204 2023-05-13 22:06:47.607631 evadb-0.2.3.post0/PKG-INFO
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13569 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/README.md
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.559629 evadb-0.2.3.post0/eva/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      645 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.559629 evadb-0.2.3.post0/eva/binder/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/binder/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4839 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/eva/binder/binder_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12812 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/eva/binder/statement_binder.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8000 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/binder/statement_binder_context.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.559629 evadb-0.2.3.post0/eva/catalog/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      616 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/catalog/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    18073 2023-05-13 21:57:10.000000 evadb-0.2.3.post0/eva/catalog/catalog_manager.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3076 2023-05-13 20:09:04.000000 evadb-0.2.3.post0/eva/catalog/catalog_type.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6946 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/catalog/catalog_utils.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.563629 evadb-0.2.3.post0/eva/catalog/models/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      886 2023-05-07 23:58:31.000000 evadb-0.2.3.post0/eva/catalog/models/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1499 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/models/association_models.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4672 2023-05-13 21:57:10.000000 evadb-0.2.3.post0/eva/catalog/models/base_model.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5110 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/models/column_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3274 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/models/index_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2997 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/models/table_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3532 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/models/udf_cache_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4429 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/models/udf_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2262 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/models/udf_cost_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4722 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/models/udf_io_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2668 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/models/udf_metadata_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2127 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/schema_utils.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.563629 evadb-0.2.3.post0/eva/catalog/services/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/catalog/services/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1167 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/services/base_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2873 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/services/column_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2887 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/services/index_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4571 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/services/table_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3669 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/services/udf_cache_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3078 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/services/udf_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2826 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/services/udf_cost_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2476 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/services/udf_io_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1936 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/services/udf_metadata_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3119 2023-05-13 21:57:10.000000 evadb-0.2.3.post0/eva/catalog/sql_config.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.563629 evadb-0.2.3.post0/eva/configuration/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      620 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/configuration/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4200 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/configuration/bootstrap_environment.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4146 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/configuration/configuration_manager.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1402 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/configuration/constants.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      882 2023-05-13 21:57:10.000000 evadb-0.2.3.post0/eva/constants.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      787 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/eva.yml
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1553 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/eva_cmd_client.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2399 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/eva_server.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.567629 evadb-0.2.3.post0/eva/executor/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      615 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/executor/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2137 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/abstract_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2214 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/eva/executor/apply_and_merge_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1530 2023-05-13 21:57:10.000000 evadb-0.2.3.post0/eva/executor/create_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5728 2023-05-13 20:09:04.000000 evadb-0.2.3.post0/eva/executor/create_index_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3866 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/create_mat_view_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7642 2023-05-13 21:57:10.000000 evadb-0.2.3.post0/eva/executor/create_udf_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4738 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/delete_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2557 2023-05-13 21:57:10.000000 evadb-0.2.3.post0/eva/executor/drop_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2010 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/drop_udf_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3013 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/execution_context.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3091 2023-05-13 21:57:10.000000 evadb-0.2.3.post0/eva/executor/executor_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1523 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/explain_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3507 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/faiss_index_scan_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1591 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/function_scan_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1759 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/groupby_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1800 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/hash_join_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2255 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/insert_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1616 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/join_build_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1661 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/lateral_join_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1583 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/limit_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3086 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/load_csv_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1579 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/load_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6065 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/eva/executor/load_multimedia_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1488 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/nested_loop_join_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4183 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/orderby_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8071 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/plan_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1644 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/pp_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1277 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/predicate_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1272 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/project_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1186 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/rename_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1413 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/sample_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1812 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/seq_scan_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1870 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/show_info_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2274 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/storage_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1264 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/union_executor.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.567629 evadb-0.2.3.post0/eva/experimental/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      619 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/experimental/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.567629 evadb-0.2.3.post0/eva/experimental/ray/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      610 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/experimental/ray/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.567629 evadb-0.2.3.post0/eva/experimental/ray/executor/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      619 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/experimental/ray/executor/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3521 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/experimental/ray/executor/exchange_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1431 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/experimental/ray/executor/ray_stage.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.567629 evadb-0.2.3.post0/eva/experimental/ray/optimizer/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      620 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/experimental/ray/optimizer/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.567629 evadb-0.2.3.post0/eva/experimental/ray/optimizer/rules/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      626 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/experimental/ray/optimizer/rules/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4176 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/experimental/ray/optimizer/rules/rules.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.567629 evadb-0.2.3.post0/eva/experimental/ray/planner/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      618 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/experimental/ray/planner/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1380 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/experimental/ray/planner/exchange_plan.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.571629 evadb-0.2.3.post0/eva/expression/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      617 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/expression/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5469 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/eva/expression/abstract_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3974 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/expression/aggregation_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1618 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/expression/arithmetic_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4351 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/expression/comparison_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2542 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/expression/constant_value_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10440 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/expression/expression_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10171 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/expression/function_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3055 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/expression/logical_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4685 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/expression/tuple_value_expression.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.571629 evadb-0.2.3.post0/eva/models/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      633 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/models/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.571629 evadb-0.2.3.post0/eva/models/catalog/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/models/catalog/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1332 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/models/catalog/frame_info.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      857 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/models/catalog/properties.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.571629 evadb-0.2.3.post0/eva/models/server/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/models/server/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1961 2023-05-13 21:57:10.000000 evadb-0.2.3.post0/eva/models/server/response.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.571629 evadb-0.2.3.post0/eva/models/storage/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/models/storage/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    14837 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/models/storage/batch.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.571629 evadb-0.2.3.post0/eva/optimizer/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      620 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/optimizer/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3260 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/optimizer/binder.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2129 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/optimizer/cost_model.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3450 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/optimizer/group.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2669 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/optimizer/group_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4335 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/optimizer/memo.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    35842 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/eva/optimizer/operators.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3838 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/optimizer/optimizer_context.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      982 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/optimizer/optimizer_task_stack.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12579 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/optimizer/optimizer_tasks.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10874 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/optimizer/optimizer_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5897 2023-05-13 21:57:10.000000 evadb-0.2.3.post0/eva/optimizer/plan_generator.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1169 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/optimizer/property.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.571629 evadb-0.2.3.post0/eva/optimizer/rules/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/optimizer/rules/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1016 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/optimizer/rules/pattern.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    43623 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/eva/optimizer/rules/rules.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7221 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/eva/optimizer/rules/rules_base.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7743 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/eva/optimizer/rules/rules_manager.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13132 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/eva/optimizer/statement_to_opr_convertor.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.575630 evadb-0.2.3.post0/eva/parser/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/parser/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1360 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/parser/alias.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2672 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/create_index_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2788 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/create_mat_view_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4838 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/create_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4882 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/create_udf_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2048 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/delete_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1767 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/drop_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1793 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/parser/drop_udf_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    19477 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/parser/eva.lark
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.575630 evadb-0.2.3.post0/eva/parser/evaql/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    65109 2022-12-14 06:32:03.000000 evadb-0.2.3.post0/eva/parser/evaql/evaql_lexer.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)   408798 2022-12-14 06:32:04.000000 evadb-0.2.3.post0/eva/parser/evaql/evaql_parser.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    44890 2022-12-14 06:32:04.000000 evadb-0.2.3.post0/eva/parser/evaql/evaql_parserListener.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    26541 2022-12-14 06:32:04.000000 evadb-0.2.3.post0/eva/parser/evaql/evaql_parserVisitor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1384 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/parser/explain_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2922 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/insert_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1717 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/lark_parser.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.579630 evadb-0.2.3.post0/eva/parser/lark_visitor/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2655 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/lark_visitor/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2161 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/parser/lark_visitor/_common_clauses_ids.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10502 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/parser/lark_visitor/_create_statements.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1404 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/lark_visitor/_delete_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1202 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/lark_visitor/_drop_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1006 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/lark_visitor/_explain_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4672 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/lark_visitor/_expressions.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6231 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/parser/lark_visitor/_functions.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2465 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/lark_visitor/_insert_statements.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2057 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/lark_visitor/_load_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      932 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/lark_visitor/_rename_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2143 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/parser/lark_visitor/_select_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1112 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/parser/lark_visitor/_show_statements.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     9468 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/lark_visitor/_table_sources.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3214 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/load_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1228 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/parser.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2007 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/rename_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5921 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/select_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1460 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/show_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1052 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/parser/statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8639 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/table_ref.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1679 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/eva/parser/types.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.583630 evadb-0.2.3.post0/eva/plan_nodes/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      614 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1689 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/abstract_join_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3453 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/abstract_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1455 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/abstract_scan_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1930 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/apply_and_merge_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2401 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/create_index_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2076 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/create_mat_view_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2200 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/create_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3603 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/create_udf_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1951 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/delete_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1660 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/drop_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1532 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/drop_udf_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1033 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/explain_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2355 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/faiss_index_scan_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1755 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/function_scan_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1499 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/groupby_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1712 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/hash_join_build_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2179 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/hash_join_probe_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2023 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/insert_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1408 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/lateral_join_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1468 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/limit_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2710 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/load_data_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1510 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/nested_loop_join_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1564 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/orderby_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1177 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/pp_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1245 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/predicate_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1249 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/project_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1616 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/rename_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1469 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/sample_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1760 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/seq_scan_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1201 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/show_info_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4419 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/storage_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1420 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/types.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1245 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/union_plan.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.583630 evadb-0.2.3.post0/eva/readers/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/readers/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2320 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/readers/abstract_reader.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2651 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/readers/csv_reader.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5986 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/readers/decord_reader.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.583630 evadb-0.2.3.post0/eva/readers/image/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/readers/image/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1067 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/readers/image/opencv_image_reader.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.583630 evadb-0.2.3.post0/eva/server/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      623 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/server/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3284 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/eva/server/command_handler.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3502 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/server/db_api.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3276 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/server/interpreter.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2866 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/server/server.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.583630 evadb-0.2.3.post0/eva/storage/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      616 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/storage/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6132 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/eva/storage/abstract_media_storage_engine.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2385 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/storage/abstract_storage_engine.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1717 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/storage/image_storage_engine.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8881 2023-05-13 20:09:04.000000 evadb-0.2.3.post0/eva/storage/sqlite_storage_engine.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1688 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/storage/storage_engine.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2496 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/storage/video_storage_engine.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.583630 evadb-0.2.3.post0/eva/third_party/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      605 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/third_party/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.583630 evadb-0.2.3.post0/eva/third_party/huggingface/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      619 2023-05-13 20:09:04.000000 evadb-0.2.3.post0/eva/third_party/huggingface/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1420 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/third_party/huggingface/binder.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6403 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/third_party/huggingface/create.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2615 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/third_party/huggingface/model.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.587630 evadb-0.2.3.post0/eva/udfs/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      616 2023-05-03 20:30:47.000000 evadb-0.2.3.post0/eva/udfs/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.587630 evadb-0.2.3.post0/eva/udfs/abstract/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      625 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/udfs/abstract/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2441 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/udfs/abstract/abstract_udf.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3945 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/udfs/abstract/hf_abstract_udf.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3843 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/udfs/abstract/pytorch_abstract_udf.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3464 2023-05-03 20:30:47.000000 evadb-0.2.3.post0/eva/udfs/asl_action_recognition.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3218 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/udfs/chatgpt.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.587630 evadb-0.2.3.post0/eva/udfs/decorators/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/udfs/decorators/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2185 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/udfs/decorators/decorators.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.587630 evadb-0.2.3.post0/eva/udfs/decorators/io_descriptors/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/udfs/decorators/io_descriptors/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2754 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/udfs/decorators/io_descriptors/abstract_types.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3375 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/udfs/decorators/io_descriptors/data_types.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1437 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/eva/udfs/decorators/utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5478 2023-05-03 20:30:47.000000 evadb-0.2.3.post0/eva/udfs/emotion_detector.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2539 2023-05-03 20:30:47.000000 evadb-0.2.3.post0/eva/udfs/face_detector.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5998 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/udfs/fastrcnn_object_detector.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1822 2023-05-03 20:30:47.000000 evadb-0.2.3.post0/eva/udfs/feature_extractor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1028 2023-05-03 20:30:47.000000 evadb-0.2.3.post0/eva/udfs/gpu_compatible.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2200 2023-05-03 20:30:47.000000 evadb-0.2.3.post0/eva/udfs/mvit_action_recognition.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.587630 evadb-0.2.3.post0/eva/udfs/ndarray/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      638 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/udfs/ndarray/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2568 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/udfs/ndarray/array_count.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1647 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/udfs/ndarray/crop.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1179 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/udfs/ndarray/fuzzy_join.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1557 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/udfs/ndarray/open.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1782 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/udfs/ndarray/similarity.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2750 2023-05-03 20:30:47.000000 evadb-0.2.3.post0/eva/udfs/ocr_extractor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7165 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/eva/udfs/udf_bootstrap_queries.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3858 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/udfs/yolo_object_detector.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.587630 evadb-0.2.3.post0/eva/utils/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      611 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/utils/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      909 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/utils/errors.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6969 2023-05-13 21:57:10.000000 evadb-0.2.3.post0/eva/utils/generic_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1956 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/utils/kv_cache.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      985 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/utils/logging_manager.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1562 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/utils/s3_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1692 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/utils/stats.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      717 2023-05-13 22:04:38.000000 evadb-0.2.3.post0/eva/version.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.587630 evadb-0.2.3.post0/evadb.egg-info/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    16204 2023-05-13 22:06:47.000000 evadb-0.2.3.post0/evadb.egg-info/PKG-INFO
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13509 2023-05-13 22:06:47.000000 evadb-0.2.3.post0/evadb.egg-info/SOURCES.txt
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)        1 2023-05-13 22:06:47.000000 evadb-0.2.3.post0/evadb.egg-info/dependency_links.txt
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)       89 2023-05-13 22:06:47.000000 evadb-0.2.3.post0/evadb.egg-info/entry_points.txt
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1121 2023-05-13 22:06:47.000000 evadb-0.2.3.post0/evadb.egg-info/requires.txt
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)       21 2023-05-13 22:06:47.000000 evadb-0.2.3.post0/evadb.egg-info/top_level.txt
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)       90 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/pyproject.toml
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)       38 2023-05-13 22:06:47.607631 evadb-0.2.3.post0/setup.cfg
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4049 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/setup.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.591630 evadb-0.2.3.post0/test/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.591630 evadb-0.2.3.post0/test/benchmark_tests/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/benchmark_tests/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1176 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/benchmark_tests/conftest.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6639 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/test/benchmark_tests/test_benchmark_pytorch.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.591630 evadb-0.2.3.post0/test/binder/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/binder/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2032 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/binder/test_binder_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    14016 2023-05-04 00:59:50.000000 evadb-0.2.3.post0/test/binder/test_statement_binder.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7961 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/binder/test_statement_binder_context.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1796 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/binder/test_statement_binder_python37.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.591630 evadb-0.2.3.post0/test/catalog/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/catalog/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.591630 evadb-0.2.3.post0/test/catalog/models/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/catalog/models/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7234 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/catalog/models/test_models.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.591630 evadb-0.2.3.post0/test/catalog/services/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/catalog/services/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1918 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/catalog/services/test_column_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4745 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/catalog/services/test_index_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3639 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/catalog/services/test_table_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3639 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/catalog/services/test_udf_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3210 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/catalog/services/test_udf_cost_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3035 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/catalog/services/test_udf_io_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6808 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/catalog/test_catalog_manager.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1402 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/catalog/test_column_type.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1910 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/catalog/test_sqlalchemy.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.595630 evadb-0.2.3.post0/test/configuration/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/configuration/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1490 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/configuration/test_bootstrap_environment.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1616 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/configuration/test_configuration_manager.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.595630 evadb-0.2.3.post0/test/executor/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/executor/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1106 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/executor/test_abstract_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2441 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/executor/test_create_mat_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3987 2023-05-03 23:43:07.000000 evadb-0.2.3.post0/test/executor/test_create_udf_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4227 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/executor/test_execution_context.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1275 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/executor/test_executor_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4650 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/executor/test_limit_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3890 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/executor/test_load_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2884 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/executor/test_orderby_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10986 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/executor/test_plan_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1397 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/executor/test_pp_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1817 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/executor/test_sample_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2752 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/executor/test_seq_scan_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      847 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/executor/utils.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.599630 evadb-0.2.3.post0/test/expression/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/expression/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3722 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/expression/test_abstract_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5149 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/expression/test_aggregation.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2975 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/expression/test_arithmetic.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5578 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/expression/test_comparison.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2867 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/expression/test_expression_tree.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7555 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/expression/test_expression_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2685 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/expression/test_function_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10242 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/expression/test_logical.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.599630 evadb-0.2.3.post0/test/integration_tests/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/integration_tests/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3585 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/integration_tests/test_array_count.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4522 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/integration_tests/test_chatgpt.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7645 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/integration_tests/test_create_index_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1091 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/integration_tests/test_create_table_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5158 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/integration_tests/test_delete_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4839 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/integration_tests/test_drop_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2358 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/test/integration_tests/test_error_handling_with_ray.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4086 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/integration_tests/test_explain_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3183 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/integration_tests/test_fuzzy_join.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13961 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/test/integration_tests/test_huggingface_udfs.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3806 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/test/integration_tests/test_insert_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2983 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/test/integration_tests/test_like.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    20623 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/test/integration_tests/test_load_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5227 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/integration_tests/test_mat_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2658 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/integration_tests/test_open.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10182 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/test/integration_tests/test_optimizer_rules.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10755 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/test/integration_tests/test_pytorch.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2953 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/integration_tests/test_rename_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     9958 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/test/integration_tests/test_reuse.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5210 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/integration_tests/test_s3_load_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    30781 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/integration_tests/test_select_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3277 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/integration_tests/test_show_info_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12287 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/integration_tests/test_similarity.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12062 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/integration_tests/test_udf_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1573 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/test/markers.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.599630 evadb-0.2.3.post0/test/models/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/models/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.599630 evadb-0.2.3.post0/test/models/catalog/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/models/catalog/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1010 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/models/catalog/test_frame_info.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.599630 evadb-0.2.3.post0/test/models/storage/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/models/storage/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5919 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/models/storage/test_batch.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.603631 evadb-0.2.3.post0/test/optimizer/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/optimizer/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.603631 evadb-0.2.3.post0/test/optimizer/rules/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/optimizer/rules/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    11829 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/test/optimizer/rules/test_rules.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4195 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/optimizer/test_binder.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4377 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/optimizer/test_cascade_optimizer.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4406 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/optimizer/test_cost_model.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2689 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/optimizer/test_group.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1996 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/optimizer/test_memo.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1034 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/optimizer/test_optimizer_context.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6122 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/optimizer/test_optimizer_task.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2000 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/optimizer/test_optimizer_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13335 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/test/optimizer/test_statement_to_opr_convertor.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.603631 evadb-0.2.3.post0/test/parser/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/parser/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    36047 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/parser/test_parser.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7781 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/parser/test_parser_statements.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.603631 evadb-0.2.3.post0/test/plan_nodes/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/plan_nodes/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6292 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/plan_nodes/test_plan.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.603631 evadb-0.2.3.post0/test/readers/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/readers/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1688 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/readers/test_csv_reader.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8104 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/readers/test_decord_reader.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.603631 evadb-0.2.3.post0/test/server/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/server/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1268 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/server/test_command_handler.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5057 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/server/test_db_api.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2581 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/server/test_interpreter.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2066 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/server/test_server.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.603631 evadb-0.2.3.post0/test/storage/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/storage/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4113 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/storage/test_sqlite_storage_engine.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4023 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/storage/test_video_storage.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1801 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/test_eva_cmd_client.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1294 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/test_eva_imports.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1810 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/test_eva_server.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.603631 evadb-0.2.3.post0/test/udfs/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      638 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/udfs/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.603631 evadb-0.2.3.post0/test/udfs/decorators/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/udfs/decorators/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.607631 evadb-0.2.3.post0/test/udfs/decorators/io_descriptors/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/udfs/decorators/io_descriptors/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7430 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/udfs/decorators/io_descriptors/test_descriptors.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2134 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/udfs/decorators/test_decorators.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.607631 evadb-0.2.3.post0/test/udfs/ndarray/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      648 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/udfs/ndarray/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      849 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/udfs/ndarray/test_array_count.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2410 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/udfs/ndarray/test_crop.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2374 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/udfs/ndarray/test_open.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4412 2023-05-13 21:57:10.000000 evadb-0.2.3.post0/test/udfs/test_abstract_udf.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2154 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/udfs/test_emotion_detector.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3345 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/udfs/test_facenet_udf.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2548 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/udfs/test_fastrcnn_object_detector.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2768 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/udfs/test_yolo_object_detector.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    17437 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/test/util.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.607631 evadb-0.2.3.post0/test/utils/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/utils/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4196 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/utils/test_generic_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2256 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/utils/test_timer.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2199 2023-05-13 21:57:10.000000 evadb-0.2.3.post0/test/utils/test_xdist.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.607631 evadb-0.2.3.post0/third_party/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/third_party/__init__.py
```

### Comparing `evadb-0.2.3/LICENSE.txt` & `evadb-0.2.3.post0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/PKG-INFO` & `evadb-0.2.3.post0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: evadb
-Version: 0.2.3
-Summary: EVA Video Database System (Think MySQL for videos).
-Home-page: https://github.com/georgia-tech-db/eva
-Download-URL: https://github.com/georgia-tech-db/eva
-Author: Georgia Tech Database Group
-Author-email: georgia.tech.db@gmail.com
-License: Apache License 2.0
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 3 - Alpha
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.txt
-
 <div >
   <a href="https://evadb.readthedocs.io/">
     <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-banner.png" alt="EVA" width="1000px" margin-left="-5px">
   </a>
 </div>
 
 # EVA AI-Relational Database System
@@ -51,14 +31,15 @@
 
 ## Quick Links
 
 - [Features](#features)
 - [Quick Start](#quick-start)
 - [Documentation](#documentation)
 - [Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
+- [Architecture Diagram](#architecture-diagram)
 - [Demo](#demo)
 - [Illustrative Applications](#illustrative-applications)
 - [Community and Support](#community-and-support)
 - [Contributing](#contributing)
 - [License](#license)
 
 ## Features
@@ -71,19 +52,20 @@
 - ⌨️ First-class support for PyTorch and HuggingFace models
 - 🐍 Installable via pip and fully implemented in Python
 
 ## Demo
 
 Here are some illustrative EVA-backed applications (all of them are Jupyter notebooks that can be opened in Google Colab):
 
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/08-chatgpt.html">Using ChatGPT to ask questions based on videos</a>
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html">Analysing traffic flow at an intersection</a>
- * 🔮 <a href="https://evadb.readthedocs.io/en/latest/source/tutorials/08-chatgpt.html">Asking questions based on videos</a>
+
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html">Examining the emotion palette of actors in a movie</a>
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html">Classifying images based on their content</a>
- * 🔮 <a href="https://evadb.readthedocs.io/en/latest/source/tutorials/07-object-segmentation-huggingface.html">Image Segmentation using Hugging Face</a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/07-object-segmentation-huggingface.html">Image Segmentation using Hugging Face</a>
  * 🔮 <a href="https://github.com/georgia-tech-db/license-plate-recognition">Recognizing license plates </a>
  * 🔮 <a href="https://github.com/georgia-tech-db/toxicity-classification">Analysing toxicity of social media memes </a>
 
 ## Documentation
 
 * [Detailed Documentation](https://evadb.readthedocs.io/)
   - If you are wondering why you might need an AI-relational database system, start with the page on <a href="https://evadb.readthedocs.io/en/stable/source/overview/video.html#">Video Database Systems</a>.
```

#### html2text {}

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1 Name: evadb Version: 0.2.3 Summary: EVA Video Database
-System (Think MySQL for videos). Home-page: https://github.com/georgia-tech-db/
-eva Download-URL: https://github.com/georgia-tech-db/eva Author: Georgia Tech
-Database Group Author-email: georgia.tech.db@gmail.com License: Apache License
-2.0 Classifier: Intended Audience :: Science/Research Classifier: Topic ::
-Scientific/Engineering :: Information Analysis Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Programming Language :: Python
-:: 3 Classifier: Development Status :: 3 - Alpha Classifier: Operating System
-:: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
-markdown Provides-Extra: dev License-File: LICENSE.txt
 [EVA]
 # EVA AI-Relational Database System
 [Open_EVA_on_Colab] [Slack] [PyPI] [License] [Coverage Status] [Roadmap]
 [Downloads] [Python Versions]
 **** EVA is a database system for building simpler and faster AI-powered
 applications. ****
 EVA is designed for supporting database applications that operate on both
@@ -22,56 +12,56 @@
 reordering. EVA supports an AI-oriented SQL-like query language tailored for
 analyzing unstructured data. It comes with a wide range of models for analyzing
 unstructured data, including models for object detection, question answering,
 OCR, text sentiment classification, face detection, etc. It is fully
 implemented in Python and licensed under the Apache license. ## Quick Links -
 [Features](#features) - [Quick Start](#quick-start) - [Documentation]
 (#documentation) - [Roadmap](https://github.com/orgs/georgia-tech-db/projects/
-3) - [Demo](#demo) - [Illustrative Applications](#illustrative-applications) -
-[Community and Support](#community-and-support) - [Contributing](#contributing)
-- [License](#license) ## Features - ð® Build simpler AI-powered applications
-using short SQL-like queries - â¡ï¸ 10-100x faster AI pipelines using AI-
-centric query optimization - ð° Save money spent on GPU-driven inference -
-ð First-class support for your custom deep learning models through user-
-defined functions - ð¦ Built-in caching to eliminate redundant model
-invocations across queries - â¨ï¸ First-class support for PyTorch and
-HuggingFace models - ð Installable via pip and fully implemented in Python
-## Demo Here are some illustrative EVA-backed applications (all of them are
-Jupyter notebooks that can be opened in Google Colab): * ð® Analysing_traffic
-flow_at_an_intersection * ð® Asking_questions_based_on_videos * ð®
-Examining_the_emotion_palette_of_actors_in_a_movie * ð® Classifying_images
-based_on_their_content * ð® Image_Segmentation_using_Hugging_Face * ð®
-Recognizing_license_plates * ð® Analysing_toxicity_of_social_media_memes ##
-Documentation * [Detailed Documentation](https://evadb.readthedocs.io/) - If
-you are wondering why you might need an AI-relational database system, start
-with the page on Video_Database_Systems. - The Getting_Started page shows how
-you can use EVA for different AI pipelines, and how you can easily extend EVA
-by defining an user-defined function that wraps around your custom deep
-learning model. - The User_Guides section contains Jupyter Notebooks that
-demonstrate how to use various features of EVA. Each notebook includes a link
-to Google Colab to run the code. * [Tutorials](https://github.com/georgia-tech-
-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb) * [Join us on Slack!]
-(https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-
-PlJ4iawLdurDv~aIAq90Dg) * [Medium-Term Roadmap](https://github.com/orgs/
-georgia-tech-db/projects/3) * [Demo](https://github.com/georgia-tech-db/eva/
-blob/master/tutorials/03-emotion-analysis.ipynb) ## Quick Start - Install EVA
-using the pip package manager. EVA supports Python versions >= 3.7: ```shell
-pip install evadb ``` - To launch and connect to an EVA server in a Jupyter
-notebook, check out this [illustrative emotion analysis notebook](https://
-github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-
-analysis.ipynb): ```shell cursor = connect_to_server() ``` - Load a video onto
-the EVA server (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) for
-illustration): ```mysql LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO
-TrafficVideo; ``` - That's it! You can now run queries over the loaded video:
-```mysql SELECT id, data FROM TrafficVideo WHERE id < 5; ``` - Search for
-frames in the video that contain a car: ```mysql SELECT id, data FROM
-TrafficVideo WHERE ['car'] <@ Yolo(data).labels; ``` | Source Video | Query
-Result | |---------------|--------------| |[Source Video] |[Query Result] | -
-Search for frames in the video that contain a pedestrian and a car: ```mysql
-SELECT id, data FROM TrafficVideo WHERE ['pedestrian', 'car'] <@ Yolo
+3) - [Architecture Diagram](#architecture-diagram) - [Demo](#demo) -
+[Illustrative Applications](#illustrative-applications) - [Community and
+Support](#community-and-support) - [Contributing](#contributing) - [License]
+(#license) ## Features - ð® Build simpler AI-powered applications using short
+SQL-like queries - â¡ï¸ 10-100x faster AI pipelines using AI-centric query
+optimization - ð° Save money spent on GPU-driven inference - ð First-class
+support for your custom deep learning models through user-defined functions -
+ð¦ Built-in caching to eliminate redundant model invocations across queries -
+â¨ï¸ First-class support for PyTorch and HuggingFace models - ð
+Installable via pip and fully implemented in Python ## Demo Here are some
+illustrative EVA-backed applications (all of them are Jupyter notebooks that
+can be opened in Google Colab): * ð® Using_ChatGPT_to_ask_questions_based_on
+videos * ð® Analysing_traffic_flow_at_an_intersection * ð® Examining_the
+emotion_palette_of_actors_in_a_movie * ð® Classifying_images_based_on_their
+content * ð® Image_Segmentation_using_Hugging_Face * ð® Recognizing_license
+plates * ð® Analysing_toxicity_of_social_media_memes ## Documentation *
+[Detailed Documentation](https://evadb.readthedocs.io/) - If you are wondering
+why you might need an AI-relational database system, start with the page on
+Video_Database_Systems. - The Getting_Started page shows how you can use EVA
+for different AI pipelines, and how you can easily extend EVA by defining an
+user-defined function that wraps around your custom deep learning model. - The
+User_Guides section contains Jupyter Notebooks that demonstrate how to use
+various features of EVA. Each notebook includes a link to Google Colab to run
+the code. * [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/
+tutorials/03-emotion-analysis.ipynb) * [Join us on Slack!](https://
+join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) *
+[Medium-Term Roadmap](https://github.com/orgs/georgia-tech-db/projects/3) *
+[Demo](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-
+analysis.ipynb) ## Quick Start - Install EVA using the pip package manager. EVA
+supports Python versions >= 3.7: ```shell pip install evadb ``` - To launch and
+connect to an EVA server in a Jupyter notebook, check out this [illustrative
+emotion analysis notebook](https://github.com/georgia-tech-db/eva/blob/master/
+tutorials/03-emotion-analysis.ipynb): ```shell cursor = connect_to_server() ```
+- Load a video onto the EVA server (we use [ua_detrac.mp4](data/ua_detrac/
+ua_detrac.mp4) for illustration): ```mysql LOAD VIDEO "data/ua_detrac/
+ua_detrac.mp4" INTO TrafficVideo; ``` - That's it! You can now run queries over
+the loaded video: ```mysql SELECT id, data FROM TrafficVideo WHERE id < 5; ```
+- Search for frames in the video that contain a car: ```mysql SELECT id, data
+FROM TrafficVideo WHERE ['car'] <@ Yolo(data).labels; ``` | Source Video |
+Query Result | |---------------|--------------| |[Source Video] |[Query Result]
+| - Search for frames in the video that contain a pedestrian and a car:
+```mysql SELECT id, data FROM TrafficVideo WHERE ['pedestrian', 'car'] <@ Yolo
 (data).labels; ``` - Search for frames with more than three cars: ```mysql
 SELECT id, data FROM TrafficVideo WHERE ArrayCount(Yolo(data).labels, 'car') >
 3; ``` - **Use your custom deep learning model in queries** with a user-defined
 function (UDF): ```mysql CREATE UDF IF NOT EXISTS Yolo TYPE ultralytics 'model'
 'yolov8m.pt'; ``` - **Compose multiple models in a single query** to set up
 useful AI pipelines. ```mysql -- Analyse emotions of faces in a video SELECT
 id, bbox, EmotionDetector(Crop(data, bbox)) FROM MovieVideo JOIN LATERAL UNNEST
```

### Comparing `evadb-0.2.3/README.md` & `evadb-0.2.3.post0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,230 +1,251 @@
-<div >
-  <a href="https://evadb.readthedocs.io/">
-    <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-banner.png" alt="EVA" width="1000px" margin-left="-5px">
-  </a>
-</div>
-
-# EVA AI-Relational Database System
-
-<div>
-        <a href="https://colab.research.google.com/github/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb">
-            <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open EVA on Colab"/>
+Metadata-Version: 2.1
+Name: evadb
+Version: 0.2.3.post0
+Summary: EVA AI-Relational Database System
+Home-page: https://github.com/georgia-tech-db/eva
+Author: Georgia Tech Database Group
+Author-email: arulraj@gatech.edu
+License: Apache License 2.0
+Download-URL: https://github.com/georgia-tech-db/eva
+Description: <div >
+          <a href="https://evadb.readthedocs.io/">
+            <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-banner.png" alt="EVA" width="1000px" margin-left="-5px">
+          </a>
+        </div>
+        
+        # EVA AI-Relational Database System
+        
+        <div>
+                <a href="https://colab.research.google.com/github/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb">
+                    <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open EVA on Colab"/>
+                </a>
+                <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">
+                    <img alt="Slack" src="https://img.shields.io/badge/slack-eva-ff69b4.svg?logo=slack">
+                </a>          
+                <img alt="PyPI" src="https://img.shields.io/pypi/v/evadb.svg"/>
+                <img alt="License" src="https://img.shields.io/badge/license-Apache%202-brightgreen.svg?logo=apache"/>
+                <img alt="Coverage Status" src="https://coveralls.io/repos/github/georgia-tech-db/eva/badge.svg?branch=master"/>     
+                <a href="https://github.com/orgs/georgia-tech-db/projects/3">
+                    <img src="https://img.shields.io/badge/eva-roadmap-ff3423" alt="Roadmap"/>
+                </a>
+                <a href="https://pepy.tech/project/evadb">
+                  <img alt="Downloads" src="https://static.pepy.tech/badge/evadb/month"/>
+                </a>
+                <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.7%20|%203.8%20|%203.9%20|%203.10-brightgreen"/>       
+        </div>
+        
+        <p align="center"> <b><h3>EVA is a database system for building simpler and faster AI-powered applications.</b></h3> </p>
+        
+        EVA is designed for supporting database applications that operate on both structured (tables, feature vectors) and unstructured data (videos, podcasts, PDFs, etc.) using deep learning models. It accelerates AI pipelines by 10-100x using a collection of optimizations inspired by time-tested relational database systems, including function caching, sampling, and cost-based predicate reordering. EVA supports an AI-oriented SQL-like query language tailored for analyzing unstructured data. It comes with a wide range of models for analyzing unstructured data, including models for object detection, question answering, OCR, text sentiment classification, face detection, etc. It is fully implemented in Python and licensed under the Apache license.
+        
+        ## Quick Links
+        
+        - [Features](#features)
+        - [Quick Start](#quick-start)
+        - [Documentation](#documentation)
+        - [Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
+        - [Architecture Diagram](#architecture-diagram)
+        - [Demo](#demo)
+        - [Illustrative Applications](#illustrative-applications)
+        - [Community and Support](#community-and-support)
+        - [Contributing](#contributing)
+        - [License](#license)
+        
+        ## Features
+        
+        - ð® Build simpler AI-powered applications using short SQL-like queries
+        - â¡ï¸ 10-100x faster AI pipelines using AI-centric query optimization  
+        - ð° Save money spent on GPU-driven inference
+        - ð First-class support for your custom deep learning models through user-defined functions
+        - ð¦ Built-in caching to eliminate redundant model invocations across queries
+        - â¨ï¸ First-class support for PyTorch and HuggingFace models
+        - ð Installable via pip and fully implemented in Python
+        
+        ## Demo
+        
+        Here are some illustrative EVA-backed applications (all of them are Jupyter notebooks that can be opened in Google Colab):
+        
+         * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/08-chatgpt.html">Using ChatGPT to ask questions based on videos</a>
+         * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html">Analysing traffic flow at an intersection</a>
+        
+         * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html">Examining the emotion palette of actors in a movie</a>
+         * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html">Classifying images based on their content</a>
+         * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/07-object-segmentation-huggingface.html">Image Segmentation using Hugging Face</a>
+         * ð® <a href="https://github.com/georgia-tech-db/license-plate-recognition">Recognizing license plates </a>
+         * ð® <a href="https://github.com/georgia-tech-db/toxicity-classification">Analysing toxicity of social media memes </a>
+        
+        ## Documentation
+        
+        * [Detailed Documentation](https://evadb.readthedocs.io/)
+          - If you are wondering why you might need an AI-relational database system, start with the page on <a href="https://evadb.readthedocs.io/en/stable/source/overview/video.html#">Video Database Systems</a>.
+          - The <a href="https://evadb.readthedocs.io/en/stable/source/overview/installation.html">Getting Started</a> page shows how you can use EVA for different AI pipelines, and how you can easily extend EVA by defining an user-defined function that wraps around your custom deep learning model.
+          - The <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/index.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EVA. Each notebook includes a link to Google Colab to run the code.
+        * [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
+        * [Join us on Slack!](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)
+        * [Medium-Term Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
+        * [Demo](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
+        
+        ## Quick Start
+        
+        - Install EVA using the pip package manager. EVA supports Python versions >= 3.7:
+        
+        ```shell
+        pip install evadb
+        ```
+        
+        - To launch and connect to an EVA server in a Jupyter notebook, check out this [illustrative emotion analysis notebook](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb):
+        ```shell
+        cursor = connect_to_server()
+        ```
+        
+        - Load a video onto the EVA server (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) for illustration):
+        
+        ```mysql
+        LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO TrafficVideo;
+        ```
+        
+        - That's it! You can now run queries over the loaded video:
+        
+        ```mysql
+        SELECT id, data FROM TrafficVideo WHERE id < 5;
+        ```
+        
+        - Search for frames in the video that contain a car:
+        
+        ```mysql
+        SELECT id, data FROM TrafficVideo WHERE ['car'] <@ Yolo(data).labels;
+        ```
+        | Source Video  | Query Result |
+        |---------------|--------------|
+        |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
+        
+        - Search for frames in the video that contain a pedestrian and a car:
+        
+        ```mysql
+        SELECT id, data FROM TrafficVideo WHERE ['pedestrian', 'car'] <@ Yolo(data).labels;
+        ```
+        
+        - Search for frames with more than three cars:
+        
+        ```mysql
+        SELECT id, data FROM TrafficVideo WHERE ArrayCount(Yolo(data).labels, 'car') > 3;
+        ```
+        
+        - **Use your custom deep learning model in queries** with a user-defined function (UDF):
+        
+        ```mysql
+        CREATE UDF IF NOT EXISTS Yolo
+        TYPE  ultralytics
+        'model' 'yolov8m.pt';
+        ```
+        
+        - **Compose multiple models in a single query** to set up useful AI pipelines.
+        
+        ```mysql
+           -- Analyse emotions of faces in a video
+           SELECT id, bbox, EmotionDetector(Crop(data, bbox)) 
+           FROM MovieVideo JOIN LATERAL UNNEST(FaceDetector(data)) AS Face(bbox, conf)  
+           WHERE id < 15;
+        ```
+        
+        - **EVA runs queries faster using its AI-centric query optimizer**. Two key optimizations are:
+        
+           ð¾ **Caching**: EVA automatically caches and reuses previous query results (especially model inference results), eliminating redundant computation and reducing query processing time.
+        
+           ð¯ **Predicate Reordering**: EVA optimizes the order in which the query predicates are evaluated (e.g., runs the faster, more selective model first), leading to faster queries and lower inference costs.
+        
+        Consider these two exploratory queries on a dataset of ð images:
+        <img align="right" style="display:inline;" width="40%" src="https://github.com/georgia-tech-db/eva/blob/master/data/assets/eva_performance_comparison.png?raw=true"></a>
+        
+        ```mysql
+          -- Query 1: Find all images of black-colored dogs
+          SELECT id, bbox FROM dogs 
+          JOIN LATERAL UNNEST(Yolo(data)) AS Obj(label, bbox, score) 
+          WHERE Obj.label = 'dog' 
+            AND Color(Crop(data, bbox)) = 'black'; 
+        
+          -- Query 2: Find all Great Danes that are black-colored
+          SELECT id, bbox FROM dogs 
+          JOIN LATERAL UNNEST(Yolo(data)) AS Obj(label, bbox, score) 
+          WHERE Obj.label = 'dog' 
+            AND DogBreedClassifier(Crop(data, bbox)) = 'great dane' 
+            AND Color(Crop(data, bbox)) = 'black';
+        ```
+        
+        By reusing the results of the first query and reordering the predicates based on the available cached inference results, EVA runs the second query **10x faster**!
+        
+        ## Architecture Diagram
+        
+        The following architecture diagram presents the critical components of the EVA database system. EVA's AI-centric Query Optimizer takes a parsed query as input and generates a query plan that is then executed by the Query Engine. The Query Engine hits multiple storage engines to retrieve the data required for efficiently running the query:
+        1. Structured data (relational database system connected via `sqlalchemy`).
+        2. Unstructured media data (on cloud buckets or local filesystem).
+        3. Vector data (vector database system).
+        
+        <img width="700" alt="Architecture Diagram" src="https://github.com/georgia-tech-db/eva/assets/5521975/01452ec9-87d9-4d27-90b2-c0b1ab29b16c">
+        
+        ## Illustrative Applications 
+        
+        ### ð® [Traffic Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html) (Object Detection Model)
+        | Source Video  | Query Result |
+        |---------------|--------------|
+        |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
+        
+        ### ð® [MNIST Digit Recognition](https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html) (Image Classification Model)
+        | Source Video  | Query Result |
+        |---------------|--------------|
+        |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-input.webp" width="150"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-output.webp" width="150"> |
+        
+        ### ð® [Movie Emotion Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html) (Face Detection + Emotion Classfication Models)
+        
+        | Source Video  | Query Result |
+        |---------------|--------------|
+        |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-input.webp" width="400"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-output.webp" width="400"> |
+        
+        ### ð® [License Plate Recognition](https://github.com/georgia-tech-db/eva-application-template) (Plate Detection + OCR Extraction Models)
+        
+        | Query Result |
+        |--------------|
+        <img alt="Query Result" src="https://github.com/georgia-tech-db/license-plate-recognition/blob/main/README_files/README_12_3.png" width="300"> |
+        
+        ### ð® [Meme Toxicity Classification](https://github.com/georgia-tech-db/toxicity-classification) (OCR Extraction + Toxicity Classification Models)
+        
+        | Query Result |
+        |--------------|
+        <img alt="Query Result" src="https://raw.githubusercontent.com/georgia-tech-db/toxicity-classification/main/README_files/README_16_2.png" width="200"> |
+        
+        ## Community and Support
+        
+        ð If you have general questions about EVA, want to say hello or just follow along, we'd like to invite you to join our [Slack Community](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg).
+        
+        <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">              
+            <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-slack.png" alt="EVA Slack Channel" width="500">
         </a>
-        <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">
-            <img alt="Slack" src="https://img.shields.io/badge/slack-eva-ff69b4.svg?logo=slack">
-        </a>          
-        <img alt="PyPI" src="https://img.shields.io/pypi/v/evadb.svg"/>
-        <img alt="License" src="https://img.shields.io/badge/license-Apache%202-brightgreen.svg?logo=apache"/>
-        <img alt="Coverage Status" src="https://coveralls.io/repos/github/georgia-tech-db/eva/badge.svg?branch=master"/>     
-        <a href="https://github.com/orgs/georgia-tech-db/projects/3">
-            <img src="https://img.shields.io/badge/eva-roadmap-ff3423" alt="Roadmap"/>
-        </a>
-        <a href="https://pepy.tech/project/evadb">
-          <img alt="Downloads" src="https://static.pepy.tech/badge/evadb/month"/>
-        </a>
-        <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.7%20|%203.8%20|%203.9%20|%203.10-brightgreen"/>       
-</div>
-
-<p align="center"> <b><h3>EVA is a database system for building simpler and faster AI-powered applications.</b></h3> </p>
-
-EVA is designed for supporting database applications that operate on both structured (tables, feature vectors) and unstructured data (videos, podcasts, PDFs, etc.) using deep learning models. It accelerates AI pipelines by 10-100x using a collection of optimizations inspired by time-tested relational database systems, including function caching, sampling, and cost-based predicate reordering. EVA supports an AI-oriented SQL-like query language tailored for analyzing unstructured data. It comes with a wide range of models for analyzing unstructured data, including models for object detection, question answering, OCR, text sentiment classification, face detection, etc. It is fully implemented in Python and licensed under the Apache license.
-
-## Quick Links
-
-- [Features](#features)
-- [Quick Start](#quick-start)
-- [Documentation](#documentation)
-- [Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
-- [Demo](#demo)
-- [Illustrative Applications](#illustrative-applications)
-- [Community and Support](#community-and-support)
-- [Contributing](#contributing)
-- [License](#license)
-
-## Features
-
-- 🔮 Build simpler AI-powered applications using short SQL-like queries
-- ⚡️ 10-100x faster AI pipelines using AI-centric query optimization  
-- 💰 Save money spent on GPU-driven inference
-- 🚀 First-class support for your custom deep learning models through user-defined functions
-- 📦 Built-in caching to eliminate redundant model invocations across queries
-- ⌨️ First-class support for PyTorch and HuggingFace models
-- 🐍 Installable via pip and fully implemented in Python
-
-## Demo
-
-Here are some illustrative EVA-backed applications (all of them are Jupyter notebooks that can be opened in Google Colab):
-
- * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html">Analysing traffic flow at an intersection</a>
- * 🔮 <a href="https://evadb.readthedocs.io/en/latest/source/tutorials/08-chatgpt.html">Asking questions based on videos</a>
- * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html">Examining the emotion palette of actors in a movie</a>
- * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html">Classifying images based on their content</a>
- * 🔮 <a href="https://evadb.readthedocs.io/en/latest/source/tutorials/07-object-segmentation-huggingface.html">Image Segmentation using Hugging Face</a>
- * 🔮 <a href="https://github.com/georgia-tech-db/license-plate-recognition">Recognizing license plates </a>
- * 🔮 <a href="https://github.com/georgia-tech-db/toxicity-classification">Analysing toxicity of social media memes </a>
-
-## Documentation
-
-* [Detailed Documentation](https://evadb.readthedocs.io/)
-  - If you are wondering why you might need an AI-relational database system, start with the page on <a href="https://evadb.readthedocs.io/en/stable/source/overview/video.html#">Video Database Systems</a>.
-  - The <a href="https://evadb.readthedocs.io/en/stable/source/overview/installation.html">Getting Started</a> page shows how you can use EVA for different AI pipelines, and how you can easily extend EVA by defining an user-defined function that wraps around your custom deep learning model.
-  - The <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/index.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EVA. Each notebook includes a link to Google Colab to run the code.
-* [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
-* [Join us on Slack!](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)
-* [Medium-Term Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
-* [Demo](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
-
-## Quick Start
-
-- Install EVA using the pip package manager. EVA supports Python versions >= 3.7:
-
-```shell
-pip install evadb
-```
-
-- To launch and connect to an EVA server in a Jupyter notebook, check out this [illustrative emotion analysis notebook](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb):
-```shell
-cursor = connect_to_server()
-```
-
-- Load a video onto the EVA server (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) for illustration):
-
-```mysql
-LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO TrafficVideo;
-```
-
-- That's it! You can now run queries over the loaded video:
-
-```mysql
-SELECT id, data FROM TrafficVideo WHERE id < 5;
-```
-
-- Search for frames in the video that contain a car:
-
-```mysql
-SELECT id, data FROM TrafficVideo WHERE ['car'] <@ Yolo(data).labels;
-```
-| Source Video  | Query Result |
-|---------------|--------------|
-|<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
-
-- Search for frames in the video that contain a pedestrian and a car:
-
-```mysql
-SELECT id, data FROM TrafficVideo WHERE ['pedestrian', 'car'] <@ Yolo(data).labels;
-```
-
-- Search for frames with more than three cars:
-
-```mysql
-SELECT id, data FROM TrafficVideo WHERE ArrayCount(Yolo(data).labels, 'car') > 3;
-```
-
-- **Use your custom deep learning model in queries** with a user-defined function (UDF):
-
-```mysql
-CREATE UDF IF NOT EXISTS Yolo
-TYPE  ultralytics
-'model' 'yolov8m.pt';
-```
-
-- **Compose multiple models in a single query** to set up useful AI pipelines.
-
-```mysql
-   -- Analyse emotions of faces in a video
-   SELECT id, bbox, EmotionDetector(Crop(data, bbox)) 
-   FROM MovieVideo JOIN LATERAL UNNEST(FaceDetector(data)) AS Face(bbox, conf)  
-   WHERE id < 15;
-```
-
-- **EVA runs queries faster using its AI-centric query optimizer**. Two key optimizations are:
-
-   💾 **Caching**: EVA automatically caches and reuses previous query results (especially model inference results), eliminating redundant computation and reducing query processing time.
-
-   🎯 **Predicate Reordering**: EVA optimizes the order in which the query predicates are evaluated (e.g., runs the faster, more selective model first), leading to faster queries and lower inference costs.
-
-Consider these two exploratory queries on a dataset of 🐕 images:
-<img align="right" style="display:inline;" width="40%" src="https://github.com/georgia-tech-db/eva/blob/master/data/assets/eva_performance_comparison.png?raw=true"></a>
-
-```mysql
-  -- Query 1: Find all images of black-colored dogs
-  SELECT id, bbox FROM dogs 
-  JOIN LATERAL UNNEST(Yolo(data)) AS Obj(label, bbox, score) 
-  WHERE Obj.label = 'dog' 
-    AND Color(Crop(data, bbox)) = 'black'; 
-
-  -- Query 2: Find all Great Danes that are black-colored
-  SELECT id, bbox FROM dogs 
-  JOIN LATERAL UNNEST(Yolo(data)) AS Obj(label, bbox, score) 
-  WHERE Obj.label = 'dog' 
-    AND DogBreedClassifier(Crop(data, bbox)) = 'great dane' 
-    AND Color(Crop(data, bbox)) = 'black';
-```
-
-By reusing the results of the first query and reordering the predicates based on the available cached inference results, EVA runs the second query **10x faster**!
-
-## Architecture Diagram
-
-The following architecture diagram presents the critical components of the EVA database system. EVA's AI-centric Query Optimizer takes a parsed query as input and generates a query plan that is then executed by the Query Engine. The Query Engine hits multiple storage engines to retrieve the data required for efficiently running the query:
-1. Structured data (relational database system connected via `sqlalchemy`).
-2. Unstructured media data (on cloud buckets or local filesystem).
-3. Vector data (vector database system).
-
-<img width="700" alt="Architecture Diagram" src="https://github.com/georgia-tech-db/eva/assets/5521975/01452ec9-87d9-4d27-90b2-c0b1ab29b16c">
-
-## Illustrative Applications 
-
-### 🔮 [Traffic Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html) (Object Detection Model)
-| Source Video  | Query Result |
-|---------------|--------------|
-|<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
-
-### 🔮 [MNIST Digit Recognition](https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html) (Image Classification Model)
-| Source Video  | Query Result |
-|---------------|--------------|
-|<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-input.webp" width="150"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-output.webp" width="150"> |
-
-### 🔮 [Movie Emotion Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html) (Face Detection + Emotion Classfication Models)
-
-| Source Video  | Query Result |
-|---------------|--------------|
-|<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-input.webp" width="400"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-output.webp" width="400"> |
-
-### 🔮 [License Plate Recognition](https://github.com/georgia-tech-db/eva-application-template) (Plate Detection + OCR Extraction Models)
-
-| Query Result |
-|--------------|
-<img alt="Query Result" src="https://github.com/georgia-tech-db/license-plate-recognition/blob/main/README_files/README_12_3.png" width="300"> |
-
-### 🔮 [Meme Toxicity Classification](https://github.com/georgia-tech-db/toxicity-classification) (OCR Extraction + Toxicity Classification Models)
-
-| Query Result |
-|--------------|
-<img alt="Query Result" src="https://raw.githubusercontent.com/georgia-tech-db/toxicity-classification/main/README_files/README_16_2.png" width="200"> |
-
-## Community and Support
-
-👋 If you have general questions about EVA, want to say hello or just follow along, we'd like to invite you to join our [Slack Community](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg).
-
-<a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">              
-    <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-slack.png" alt="EVA Slack Channel" width="500">
-</a>
-
-If you run into any problems or issues, please create a Github issue and we'll try our best to help.
-
-Don't see a feature in the list? Search our issue tracker if someone has already requested it and add a comment to it explaining your use-case, or open a new issue if not. We prioritize our roadmap based on user feedback, so we'd love to hear from you.
-
-## Contributing
-
-[![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)](https://pypi.org/project/evadb)
-[![CI Status](https://circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva)
-[![Documentation Status](https://readthedocs.org/projects/evadb/badge/?version=stable)](https://evadb.readthedocs.io/en/stable/index.html)
-
-EVA is the beneficiary of many [contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All kinds of contributions to EVA are appreciated. To file a bug or to request a feature, please use <a href="https://github.com/georgia-tech-db/eva/issues">GitHub issues</a>. <a href="https://github.com/georgia-tech-db/eva/pulls">Pull requests</a> are welcome.
-
-For more information, see our
-[contribution guide](https://evadb.readthedocs.io/en/stable/source/contribute/index.html).
-
-## License
-Copyright (c) 2018-present [Georgia Tech Database Group](http://db.cc.gatech.edu/).
-Licensed under [Apache License](LICENSE).
+        
+        If you run into any problems or issues, please create a Github issue and we'll try our best to help.
+        
+        Don't see a feature in the list? Search our issue tracker if someone has already requested it and add a comment to it explaining your use-case, or open a new issue if not. We prioritize our roadmap based on user feedback, so we'd love to hear from you.
+        
+        ## Contributing
+        
+        [![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)](https://pypi.org/project/evadb)
+        [![CI Status](https://circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva)
+        [![Documentation Status](https://readthedocs.org/projects/evadb/badge/?version=stable)](https://evadb.readthedocs.io/en/stable/index.html)
+        
+        EVA is the beneficiary of many [contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All kinds of contributions to EVA are appreciated. To file a bug or to request a feature, please use <a href="https://github.com/georgia-tech-db/eva/issues">GitHub issues</a>. <a href="https://github.com/georgia-tech-db/eva/pulls">Pull requests</a> are welcome.
+        
+        For more information, see our
+        [contribution guide](https://evadb.readthedocs.io/en/stable/source/contribute/index.html).
+        
+        ## License
+        Copyright (c) 2018-present [Georgia Tech Database Group](http://db.cc.gatech.edu/).
+        Licensed under [Apache License](LICENSE).
+        
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,7 +1,12 @@
+Metadata-Version: 2.1 Name: evadb Version: 0.2.3.post0 Summary: EVA AI-
+Relational Database System Home-page: https://github.com/georgia-tech-db/eva
+Author: Georgia Tech Database Group Author-email: arulraj@gatech.edu License:
+Apache License 2.0 Download-URL: https://github.com/georgia-tech-db/eva
+Description:
 [EVA]
 # EVA AI-Relational Database System
 [Open_EVA_on_Colab] [Slack] [PyPI] [License] [Coverage Status] [Roadmap]
 [Downloads] [Python Versions]
 **** EVA is a database system for building simpler and faster AI-powered
 applications. ****
 EVA is designed for supporting database applications that operate on both
@@ -12,49 +17,50 @@
 reordering. EVA supports an AI-oriented SQL-like query language tailored for
 analyzing unstructured data. It comes with a wide range of models for analyzing
 unstructured data, including models for object detection, question answering,
 OCR, text sentiment classification, face detection, etc. It is fully
 implemented in Python and licensed under the Apache license. ## Quick Links -
 [Features](#features) - [Quick Start](#quick-start) - [Documentation]
 (#documentation) - [Roadmap](https://github.com/orgs/georgia-tech-db/projects/
-3) - [Demo](#demo) - [Illustrative Applications](#illustrative-applications) -
-[Community and Support](#community-and-support) - [Contributing](#contributing)
-- [License](#license) ## Features - ð® Build simpler AI-powered applications
-using short SQL-like queries - â¡ï¸ 10-100x faster AI pipelines using AI-
-centric query optimization - ð° Save money spent on GPU-driven inference -
-ð First-class support for your custom deep learning models through user-
-defined functions - ð¦ Built-in caching to eliminate redundant model
-invocations across queries - â¨ï¸ First-class support for PyTorch and
-HuggingFace models - ð Installable via pip and fully implemented in Python
-## Demo Here are some illustrative EVA-backed applications (all of them are
-Jupyter notebooks that can be opened in Google Colab): * ð® Analysing_traffic
-flow_at_an_intersection * ð® Asking_questions_based_on_videos * ð®
-Examining_the_emotion_palette_of_actors_in_a_movie * ð® Classifying_images
-based_on_their_content * ð® Image_Segmentation_using_Hugging_Face * ð®
-Recognizing_license_plates * ð® Analysing_toxicity_of_social_media_memes ##
-Documentation * [Detailed Documentation](https://evadb.readthedocs.io/) - If
-you are wondering why you might need an AI-relational database system, start
-with the page on Video_Database_Systems. - The Getting_Started page shows how
-you can use EVA for different AI pipelines, and how you can easily extend EVA
-by defining an user-defined function that wraps around your custom deep
-learning model. - The User_Guides section contains Jupyter Notebooks that
-demonstrate how to use various features of EVA. Each notebook includes a link
-to Google Colab to run the code. * [Tutorials](https://github.com/georgia-tech-
-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb) * [Join us on Slack!]
-(https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-
-PlJ4iawLdurDv~aIAq90Dg) * [Medium-Term Roadmap](https://github.com/orgs/
-georgia-tech-db/projects/3) * [Demo](https://github.com/georgia-tech-db/eva/
-blob/master/tutorials/03-emotion-analysis.ipynb) ## Quick Start - Install EVA
-using the pip package manager. EVA supports Python versions >= 3.7: ```shell
-pip install evadb ``` - To launch and connect to an EVA server in a Jupyter
-notebook, check out this [illustrative emotion analysis notebook](https://
-github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-
-analysis.ipynb): ```shell cursor = connect_to_server() ``` - Load a video onto
-the EVA server (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) for
-illustration): ```mysql LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO
+3) - [Architecture Diagram](#architecture-diagram) - [Demo](#demo) -
+[Illustrative Applications](#illustrative-applications) - [Community and
+Support](#community-and-support) - [Contributing](#contributing) - [License]
+(#license) ## Features - Ã°ÂÂÂ® Build simpler AI-powered applications using
+short SQL-like queries - Ã¢ÂÂ¡Ã¯Â¸Â 10-100x faster AI pipelines using AI-
+centric query optimization - Ã°ÂÂÂ° Save money spent on GPU-driven inference
+- Ã°ÂÂÂ First-class support for your custom deep learning models through
+user-defined functions - Ã°ÂÂÂ¦ Built-in caching to eliminate redundant model
+invocations across queries - Ã¢ÂÂ¨Ã¯Â¸Â First-class support for PyTorch and
+HuggingFace models - Ã°ÂÂÂ Installable via pip and fully implemented in
+Python ## Demo Here are some illustrative EVA-backed applications (all of them
+are Jupyter notebooks that can be opened in Google Colab): * Ã°ÂÂÂ® Using
+ChatGPT_to_ask_questions_based_on_videos * Ã°ÂÂÂ® Analysing_traffic_flow_at
+an_intersection * Ã°ÂÂÂ® Examining_the_emotion_palette_of_actors_in_a_movie *
+Ã°ÂÂÂ® Classifying_images_based_on_their_content * Ã°ÂÂÂ® Image
+Segmentation_using_Hugging_Face * Ã°ÂÂÂ® Recognizing_license_plates *
+Ã°ÂÂÂ® Analysing_toxicity_of_social_media_memes ## Documentation * [Detailed
+Documentation](https://evadb.readthedocs.io/) - If you are wondering why you
+might need an AI-relational database system, start with the page on Video
+Database_Systems. - The Getting_Started page shows how you can use EVA for
+different AI pipelines, and how you can easily extend EVA by defining an user-
+defined function that wraps around your custom deep learning model. - The User
+Guides section contains Jupyter Notebooks that demonstrate how to use various
+features of EVA. Each notebook includes a link to Google Colab to run the code.
+* [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-
+emotion-analysis.ipynb) * [Join us on Slack!](https://join.slack.com/t/eva-db/
+shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) * [Medium-Term Roadmap]
+(https://github.com/orgs/georgia-tech-db/projects/3) * [Demo](https://
+github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
+## Quick Start - Install EVA using the pip package manager. EVA supports Python
+versions >= 3.7: ```shell pip install evadb ``` - To launch and connect to an
+EVA server in a Jupyter notebook, check out this [illustrative emotion analysis
+notebook](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-
+emotion-analysis.ipynb): ```shell cursor = connect_to_server() ``` - Load a
+video onto the EVA server (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4)
+for illustration): ```mysql LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO
 TrafficVideo; ``` - That's it! You can now run queries over the loaded video:
 ```mysql SELECT id, data FROM TrafficVideo WHERE id < 5; ``` - Search for
 frames in the video that contain a car: ```mysql SELECT id, data FROM
 TrafficVideo WHERE ['car'] <@ Yolo(data).labels; ``` | Source Video | Query
 Result | |---------------|--------------| |[Source Video] |[Query Result] | -
 Search for frames in the video that contain a pedestrian and a car: ```mysql
 SELECT id, data FROM TrafficVideo WHERE ['pedestrian', 'car'] <@ Yolo
@@ -63,22 +69,22 @@
 3; ``` - **Use your custom deep learning model in queries** with a user-defined
 function (UDF): ```mysql CREATE UDF IF NOT EXISTS Yolo TYPE ultralytics 'model'
 'yolov8m.pt'; ``` - **Compose multiple models in a single query** to set up
 useful AI pipelines. ```mysql -- Analyse emotions of faces in a video SELECT
 id, bbox, EmotionDetector(Crop(data, bbox)) FROM MovieVideo JOIN LATERAL UNNEST
 (FaceDetector(data)) AS Face(bbox, conf) WHERE id < 15; ``` - **EVA runs
 queries faster using its AI-centric query optimizer**. Two key optimizations
-are: ð¾ **Caching**: EVA automatically caches and reuses previous query
+are: Ã°ÂÂÂ¾ **Caching**: EVA automatically caches and reuses previous query
 results (especially model inference results), eliminating redundant computation
-and reducing query processing time. ð¯ **Predicate Reordering**: EVA
+and reducing query processing time. Ã°ÂÂÂ¯ **Predicate Reordering**: EVA
 optimizes the order in which the query predicates are evaluated (e.g., runs the
 faster, more selective model first), leading to faster queries and lower
-inference costs. Consider these two exploratory queries on a dataset of ð
-images: [https://github.com/georgia-tech-db/eva/blob/master/data/assets/
-eva_performance_comparison.png?raw=true]
+inference costs. Consider these two exploratory queries on a dataset of
+Ã°ÂÂÂ images: [https://github.com/georgia-tech-db/eva/blob/master/data/
+assets/eva_performance_comparison.png?raw=true]
  ```mysql -- Query 1: Find all images of black-colored dogs SELECT id, bbox
 FROM dogs JOIN LATERAL UNNEST(Yolo(data)) AS Obj(label, bbox, score) WHERE
 Obj.label = 'dog' AND Color(Crop(data, bbox)) = 'black'; -- Query 2: Find all
 Great Danes that are black-colored SELECT id, bbox FROM dogs JOIN LATERAL
 UNNEST(Yolo(data)) AS Obj(label, bbox, score) WHERE Obj.label = 'dog' AND
 DogBreedClassifier(Crop(data, bbox)) = 'great dane' AND Color(Crop(data, bbox))
 = 'black'; ``` By reusing the results of the first query and reordering the
@@ -87,42 +93,48 @@
 diagram presents the critical components of the EVA database system. EVA's AI-
 centric Query Optimizer takes a parsed query as input and generates a query
 plan that is then executed by the Query Engine. The Query Engine hits multiple
 storage engines to retrieve the data required for efficiently running the
 query: 1. Structured data (relational database system connected via
 `sqlalchemy`). 2. Unstructured media data (on cloud buckets or local
 filesystem). 3. Vector data (vector database system). [Architecture Diagram] ##
-Illustrative Applications ### ð® [Traffic Analysis](https://
+Illustrative Applications ### Ã°ÂÂÂ® [Traffic Analysis](https://
 evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html)
 (Object Detection Model) | Source Video | Query Result | |---------------|-----
----------| |[Source Video] |[Query Result] | ### ð® [MNIST Digit Recognition]
-(https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html) (Image
-Classification Model) | Source Video | Query Result | |---------------|--------
-------| |[Source Video] |[Query Result] | ### ð® [Movie Emotion Analysis]
-(https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-
-analysis.html) (Face Detection + Emotion Classfication Models) | Source Video |
-Query Result | |---------------|--------------| |[Source Video] |[Query Result]
-| ### ð® [License Plate Recognition](https://github.com/georgia-tech-db/eva-
-application-template) (Plate Detection + OCR Extraction Models) | Query Result
-| |--------------| [Query Result] | ### ð® [Meme Toxicity Classification]
-(https://github.com/georgia-tech-db/toxicity-classification) (OCR Extraction +
-Toxicity Classification Models) | Query Result | |--------------| [Query
-Result] | ## Community and Support ð If you have general questions about
-EVA, want to say hello or just follow along, we'd like to invite you to join
-our [Slack Community](https://join.slack.com/t/eva-db/shared_invite/zt-
-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg). [EVA_Slack_Channel] If you run into any
-problems or issues, please create a Github issue and we'll try our best to
-help. Don't see a feature in the list? Search our issue tracker if someone has
-already requested it and add a comment to it explaining your use-case, or open
-a new issue if not. We prioritize our roadmap based on user feedback, so we'd
-love to hear from you. ## Contributing [![PyPI Version](https://img.shields.io/
-pypi/v/evadb.svg)](https://pypi.org/project/evadb) [![CI Status](https://
-circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https://circleci.com/gh/
-georgia-tech-db/eva) [![Documentation Status](https://readthedocs.org/projects/
-evadb/badge/?version=stable)](https://evadb.readthedocs.io/en/stable/
-index.html) EVA is the beneficiary of many [contributors](https://github.com/
-georgia-tech-db/eva/graphs/contributors). All kinds of contributions to EVA are
-appreciated. To file a bug or to request a feature, please use GitHub_issues.
-Pull_requests are welcome. For more information, see our [contribution guide]
-(https://evadb.readthedocs.io/en/stable/source/contribute/index.html). ##
-License Copyright (c) 2018-present [Georgia Tech Database Group](http://
-db.cc.gatech.edu/). Licensed under [Apache License](LICENSE).
+---------| |[Source Video] |[Query Result] | ### Ã°ÂÂÂ® [MNIST Digit
+Recognition](https://evadb.readthedocs.io/en/stable/source/tutorials/01-
+mnist.html) (Image Classification Model) | Source Video | Query Result | |-----
+----------|--------------| |[Source Video] |[Query Result] | ### Ã°ÂÂÂ®
+[Movie Emotion Analysis](https://evadb.readthedocs.io/en/stable/source/
+tutorials/03-emotion-analysis.html) (Face Detection + Emotion Classfication
+Models) | Source Video | Query Result | |---------------|--------------| |
+[Source Video] |[Query Result] | ### Ã°ÂÂÂ® [License Plate Recognition]
+(https://github.com/georgia-tech-db/eva-application-template) (Plate Detection
++ OCR Extraction Models) | Query Result | |--------------| [Query Result] | ###
+Ã°ÂÂÂ® [Meme Toxicity Classification](https://github.com/georgia-tech-db/
+toxicity-classification) (OCR Extraction + Toxicity Classification Models) |
+Query Result | |--------------| [Query Result] | ## Community and Support
+Ã°ÂÂÂ If you have general questions about EVA, want to say hello or just
+follow along, we'd like to invite you to join our [Slack Community](https://
+join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg).
+[EVA_Slack_Channel] If you run into any problems or issues, please create a
+Github issue and we'll try our best to help. Don't see a feature in the list?
+Search our issue tracker if someone has already requested it and add a comment
+to it explaining your use-case, or open a new issue if not. We prioritize our
+roadmap based on user feedback, so we'd love to hear from you. ## Contributing
+[![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)](https://pypi.org/
+project/evadb) [![CI Status](https://circleci.com/gh/georgia-tech-db/
+eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva) [!
+[Documentation Status](https://readthedocs.org/projects/evadb/badge/
+?version=stable)](https://evadb.readthedocs.io/en/stable/index.html) EVA is the
+beneficiary of many [contributors](https://github.com/georgia-tech-db/eva/
+graphs/contributors). All kinds of contributions to EVA are appreciated. To
+file a bug or to request a feature, please use GitHub_issues. Pull_requests are
+welcome. For more information, see our [contribution guide](https://
+evadb.readthedocs.io/en/stable/source/contribute/index.html). ## License
+Copyright (c) 2018-present [Georgia Tech Database Group](http://
+db.cc.gatech.edu/). Licensed under [Apache License](LICENSE). Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
+OSI Approved :: Apache Software License Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Requires-Python: >=3.8 Description-
+Content-Type: text/markdown Provides-Extra: dev
```

### Comparing `evadb-0.2.3/eva/__init__.py` & `evadb-0.2.3.post0/eva/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/binder/__init__.py` & `evadb-0.2.3.post0/eva/binder/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/binder/binder_utils.py` & `evadb-0.2.3.post0/eva/binder/binder_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/binder/statement_binder.py` & `evadb-0.2.3.post0/eva/binder/statement_binder.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/binder/statement_binder_context.py` & `evadb-0.2.3.post0/eva/binder/statement_binder_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/catalog/__init__.py` & `evadb-0.2.3.post0/eva/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/catalog/catalog_manager.py` & `evadb-0.2.3.post0/eva/catalog/catalog_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/catalog/catalog_type.py` & `evadb-0.2.3.post0/eva/catalog/catalog_type.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/catalog/catalog_utils.py` & `evadb-0.2.3.post0/eva/catalog/catalog_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/catalog/models/__init__.py` & `evadb-0.2.3.post0/eva/catalog/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/catalog/models/association_models.py` & `evadb-0.2.3.post0/eva/catalog/models/association_models.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/catalog/models/base_model.py` & `evadb-0.2.3.post0/eva/catalog/models/base_model.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/catalog/models/column_catalog.py` & `evadb-0.2.3.post0/eva/catalog/models/column_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/catalog/models/index_catalog.py` & `evadb-0.2.3.post0/eva/catalog/models/index_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/catalog/models/table_catalog.py` & `evadb-0.2.3.post0/eva/catalog/models/table_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/catalog/models/udf_cache_catalog.py` & `evadb-0.2.3.post0/eva/catalog/models/udf_cache_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/catalog/models/udf_catalog.py` & `evadb-0.2.3.post0/eva/catalog/models/udf_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/catalog/models/udf_cost_catalog.py` & `evadb-0.2.3.post0/eva/catalog/models/udf_cost_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/catalog/models/udf_io_catalog.py` & `evadb-0.2.3.post0/eva/catalog/models/udf_io_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/catalog/models/udf_metadata_catalog.py` & `evadb-0.2.3.post0/eva/catalog/models/udf_metadata_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/catalog/schema_utils.py` & `evadb-0.2.3.post0/eva/catalog/schema_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/catalog/services/__init__.py` & `evadb-0.2.3.post0/eva/catalog/services/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/catalog/services/base_service.py` & `evadb-0.2.3.post0/eva/catalog/services/base_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/catalog/services/column_catalog_service.py` & `evadb-0.2.3.post0/eva/catalog/services/column_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/catalog/services/index_catalog_service.py` & `evadb-0.2.3.post0/eva/catalog/services/index_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/catalog/services/table_catalog_service.py` & `evadb-0.2.3.post0/eva/catalog/services/table_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/catalog/services/udf_cache_catalog_service.py` & `evadb-0.2.3.post0/eva/catalog/services/udf_cache_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/catalog/services/udf_catalog_service.py` & `evadb-0.2.3.post0/eva/catalog/services/udf_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/catalog/services/udf_cost_catalog_service.py` & `evadb-0.2.3.post0/eva/catalog/services/udf_cost_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/catalog/services/udf_io_catalog_service.py` & `evadb-0.2.3.post0/eva/catalog/services/udf_io_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/catalog/services/udf_metadata_catalog_service.py` & `evadb-0.2.3.post0/eva/catalog/services/udf_metadata_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/catalog/sql_config.py` & `evadb-0.2.3.post0/eva/catalog/sql_config.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/configuration/__init__.py` & `evadb-0.2.3.post0/eva/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/configuration/bootstrap_environment.py` & `evadb-0.2.3.post0/eva/configuration/bootstrap_environment.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/configuration/configuration_manager.py` & `evadb-0.2.3.post0/eva/configuration/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/configuration/constants.py` & `evadb-0.2.3.post0/eva/configuration/constants.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/constants.py` & `evadb-0.2.3.post0/eva/constants.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/eva.yml` & `evadb-0.2.3.post0/eva/eva.yml`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/eva_cmd_client.py` & `evadb-0.2.3.post0/eva/eva_cmd_client.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/eva_server.py` & `evadb-0.2.3.post0/eva/eva_server.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/__init__.py` & `evadb-0.2.3.post0/eva/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/abstract_executor.py` & `evadb-0.2.3.post0/eva/executor/abstract_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/apply_and_merge_executor.py` & `evadb-0.2.3.post0/eva/executor/apply_and_merge_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/create_executor.py` & `evadb-0.2.3.post0/eva/executor/create_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/create_index_executor.py` & `evadb-0.2.3.post0/eva/executor/create_index_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/create_mat_view_executor.py` & `evadb-0.2.3.post0/eva/executor/create_mat_view_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/create_udf_executor.py` & `evadb-0.2.3.post0/eva/executor/create_udf_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/delete_executor.py` & `evadb-0.2.3.post0/eva/executor/delete_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/drop_executor.py` & `evadb-0.2.3.post0/eva/executor/drop_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/drop_udf_executor.py` & `evadb-0.2.3.post0/eva/executor/drop_udf_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/execution_context.py` & `evadb-0.2.3.post0/eva/executor/execution_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/executor_utils.py` & `evadb-0.2.3.post0/eva/executor/executor_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/explain_executor.py` & `evadb-0.2.3.post0/eva/executor/explain_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/faiss_index_scan_executor.py` & `evadb-0.2.3.post0/eva/executor/faiss_index_scan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/function_scan_executor.py` & `evadb-0.2.3.post0/eva/executor/function_scan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/groupby_executor.py` & `evadb-0.2.3.post0/eva/executor/groupby_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/hash_join_executor.py` & `evadb-0.2.3.post0/eva/executor/hash_join_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/insert_executor.py` & `evadb-0.2.3.post0/eva/executor/insert_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/join_build_executor.py` & `evadb-0.2.3.post0/eva/executor/join_build_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/lateral_join_executor.py` & `evadb-0.2.3.post0/eva/executor/lateral_join_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/limit_executor.py` & `evadb-0.2.3.post0/eva/executor/limit_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/load_csv_executor.py` & `evadb-0.2.3.post0/eva/executor/load_csv_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/load_executor.py` & `evadb-0.2.3.post0/eva/executor/load_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/load_multimedia_executor.py` & `evadb-0.2.3.post0/eva/executor/load_multimedia_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/nested_loop_join_executor.py` & `evadb-0.2.3.post0/eva/executor/nested_loop_join_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/orderby_executor.py` & `evadb-0.2.3.post0/eva/executor/orderby_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/plan_executor.py` & `evadb-0.2.3.post0/eva/executor/plan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/pp_executor.py` & `evadb-0.2.3.post0/eva/executor/pp_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/predicate_executor.py` & `evadb-0.2.3.post0/eva/executor/predicate_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/project_executor.py` & `evadb-0.2.3.post0/eva/executor/project_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/rename_executor.py` & `evadb-0.2.3.post0/eva/executor/rename_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/sample_executor.py` & `evadb-0.2.3.post0/eva/executor/sample_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/seq_scan_executor.py` & `evadb-0.2.3.post0/eva/executor/seq_scan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/show_info_executor.py` & `evadb-0.2.3.post0/eva/executor/show_info_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/storage_executor.py` & `evadb-0.2.3.post0/eva/executor/storage_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/executor/union_executor.py` & `evadb-0.2.3.post0/eva/executor/union_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/experimental/__init__.py` & `evadb-0.2.3.post0/eva/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/experimental/ray/__init__.py` & `evadb-0.2.3.post0/eva/experimental/ray/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/experimental/ray/executor/__init__.py` & `evadb-0.2.3.post0/eva/experimental/ray/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/experimental/ray/executor/exchange_executor.py` & `evadb-0.2.3.post0/eva/experimental/ray/executor/exchange_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/experimental/ray/executor/ray_stage.py` & `evadb-0.2.3.post0/eva/experimental/ray/executor/ray_stage.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/experimental/ray/optimizer/__init__.py` & `evadb-0.2.3.post0/eva/experimental/ray/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/experimental/ray/optimizer/rules/__init__.py` & `evadb-0.2.3.post0/eva/experimental/ray/optimizer/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/experimental/ray/optimizer/rules/rules.py` & `evadb-0.2.3.post0/eva/experimental/ray/optimizer/rules/rules.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/experimental/ray/planner/__init__.py` & `evadb-0.2.3.post0/eva/experimental/ray/planner/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/experimental/ray/planner/exchange_plan.py` & `evadb-0.2.3.post0/eva/experimental/ray/planner/exchange_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/expression/__init__.py` & `evadb-0.2.3.post0/eva/expression/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/expression/abstract_expression.py` & `evadb-0.2.3.post0/eva/expression/abstract_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/expression/aggregation_expression.py` & `evadb-0.2.3.post0/eva/expression/aggregation_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/expression/arithmetic_expression.py` & `evadb-0.2.3.post0/eva/expression/arithmetic_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/expression/comparison_expression.py` & `evadb-0.2.3.post0/eva/expression/comparison_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/expression/constant_value_expression.py` & `evadb-0.2.3.post0/eva/expression/constant_value_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/expression/expression_utils.py` & `evadb-0.2.3.post0/eva/expression/expression_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/expression/function_expression.py` & `evadb-0.2.3.post0/eva/expression/function_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/expression/logical_expression.py` & `evadb-0.2.3.post0/eva/expression/logical_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/expression/tuple_value_expression.py` & `evadb-0.2.3.post0/eva/expression/tuple_value_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/models/__init__.py` & `evadb-0.2.3.post0/eva/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/models/catalog/__init__.py` & `evadb-0.2.3.post0/eva/models/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/models/catalog/frame_info.py` & `evadb-0.2.3.post0/eva/models/catalog/frame_info.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/models/catalog/properties.py` & `evadb-0.2.3.post0/eva/models/catalog/properties.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/models/server/__init__.py` & `evadb-0.2.3.post0/eva/models/server/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/models/server/response.py` & `evadb-0.2.3.post0/eva/models/server/response.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/models/storage/__init__.py` & `evadb-0.2.3.post0/eva/models/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/models/storage/batch.py` & `evadb-0.2.3.post0/eva/models/storage/batch.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/optimizer/__init__.py` & `evadb-0.2.3.post0/eva/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/optimizer/binder.py` & `evadb-0.2.3.post0/eva/optimizer/binder.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/optimizer/cost_model.py` & `evadb-0.2.3.post0/eva/optimizer/cost_model.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/optimizer/group.py` & `evadb-0.2.3.post0/eva/optimizer/group.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/optimizer/group_expression.py` & `evadb-0.2.3.post0/eva/optimizer/group_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/optimizer/memo.py` & `evadb-0.2.3.post0/eva/optimizer/memo.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/optimizer/operators.py` & `evadb-0.2.3.post0/eva/optimizer/operators.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/optimizer/optimizer_context.py` & `evadb-0.2.3.post0/eva/optimizer/optimizer_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/optimizer/optimizer_task_stack.py` & `evadb-0.2.3.post0/eva/optimizer/optimizer_task_stack.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/optimizer/optimizer_tasks.py` & `evadb-0.2.3.post0/eva/optimizer/optimizer_tasks.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/optimizer/optimizer_utils.py` & `evadb-0.2.3.post0/eva/optimizer/optimizer_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/optimizer/plan_generator.py` & `evadb-0.2.3.post0/eva/optimizer/plan_generator.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/optimizer/property.py` & `evadb-0.2.3.post0/eva/optimizer/property.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/optimizer/rules/__init__.py` & `evadb-0.2.3.post0/eva/optimizer/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/optimizer/rules/pattern.py` & `evadb-0.2.3.post0/eva/optimizer/rules/pattern.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/optimizer/rules/rules.py` & `evadb-0.2.3.post0/eva/optimizer/rules/rules.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/optimizer/rules/rules_base.py` & `evadb-0.2.3.post0/eva/optimizer/rules/rules_base.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/optimizer/rules/rules_manager.py` & `evadb-0.2.3.post0/eva/optimizer/rules/rules_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/optimizer/statement_to_opr_convertor.py` & `evadb-0.2.3.post0/eva/optimizer/statement_to_opr_convertor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/__init__.py` & `evadb-0.2.3.post0/eva/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/alias.py` & `evadb-0.2.3.post0/eva/parser/alias.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/create_index_statement.py` & `evadb-0.2.3.post0/eva/parser/create_index_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/create_mat_view_statement.py` & `evadb-0.2.3.post0/eva/parser/create_mat_view_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/create_statement.py` & `evadb-0.2.3.post0/eva/parser/create_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/create_udf_statement.py` & `evadb-0.2.3.post0/eva/parser/create_udf_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/delete_statement.py` & `evadb-0.2.3.post0/eva/parser/delete_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/drop_statement.py` & `evadb-0.2.3.post0/eva/parser/drop_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/drop_udf_statement.py` & `evadb-0.2.3.post0/eva/parser/drop_udf_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/eva.lark` & `evadb-0.2.3.post0/eva/parser/eva.lark`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/evaql/evaql_lexer.py` & `evadb-0.2.3.post0/eva/parser/evaql/evaql_lexer.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/evaql/evaql_parser.py` & `evadb-0.2.3.post0/eva/parser/evaql/evaql_parser.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/evaql/evaql_parserListener.py` & `evadb-0.2.3.post0/eva/parser/evaql/evaql_parserListener.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/evaql/evaql_parserVisitor.py` & `evadb-0.2.3.post0/eva/parser/evaql/evaql_parserVisitor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/explain_statement.py` & `evadb-0.2.3.post0/eva/parser/explain_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/insert_statement.py` & `evadb-0.2.3.post0/eva/parser/insert_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/lark_parser.py` & `evadb-0.2.3.post0/eva/parser/lark_parser.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/lark_visitor/__init__.py` & `evadb-0.2.3.post0/eva/parser/lark_visitor/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/lark_visitor/_common_clauses_ids.py` & `evadb-0.2.3.post0/eva/parser/lark_visitor/_common_clauses_ids.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/lark_visitor/_create_statements.py` & `evadb-0.2.3.post0/eva/parser/lark_visitor/_create_statements.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/lark_visitor/_delete_statement.py` & `evadb-0.2.3.post0/eva/parser/lark_visitor/_delete_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/lark_visitor/_drop_statement.py` & `evadb-0.2.3.post0/eva/parser/lark_visitor/_drop_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/lark_visitor/_explain_statement.py` & `evadb-0.2.3.post0/eva/parser/lark_visitor/_explain_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/lark_visitor/_expressions.py` & `evadb-0.2.3.post0/eva/parser/lark_visitor/_expressions.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/lark_visitor/_functions.py` & `evadb-0.2.3.post0/eva/parser/lark_visitor/_functions.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/lark_visitor/_insert_statements.py` & `evadb-0.2.3.post0/eva/parser/lark_visitor/_insert_statements.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/lark_visitor/_load_statement.py` & `evadb-0.2.3.post0/eva/parser/lark_visitor/_load_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/lark_visitor/_rename_statement.py` & `evadb-0.2.3.post0/eva/parser/lark_visitor/_rename_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/lark_visitor/_select_statement.py` & `evadb-0.2.3.post0/eva/parser/lark_visitor/_select_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/lark_visitor/_show_statements.py` & `evadb-0.2.3.post0/eva/parser/lark_visitor/_show_statements.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/lark_visitor/_table_sources.py` & `evadb-0.2.3.post0/eva/parser/lark_visitor/_table_sources.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/load_statement.py` & `evadb-0.2.3.post0/eva/parser/load_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/parser.py` & `evadb-0.2.3.post0/eva/parser/parser.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/rename_statement.py` & `evadb-0.2.3.post0/eva/parser/rename_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/select_statement.py` & `evadb-0.2.3.post0/eva/parser/select_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/show_statement.py` & `evadb-0.2.3.post0/eva/parser/show_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/statement.py` & `evadb-0.2.3.post0/eva/parser/statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/table_ref.py` & `evadb-0.2.3.post0/eva/parser/table_ref.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/parser/types.py` & `evadb-0.2.3.post0/eva/parser/types.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/__init__.py` & `evadb-0.2.3.post0/eva/plan_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/abstract_join_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/abstract_join_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/abstract_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/abstract_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/abstract_scan_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/abstract_scan_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/apply_and_merge_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/apply_and_merge_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/create_index_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/create_index_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/create_mat_view_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/create_mat_view_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/create_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/create_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/create_udf_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/create_udf_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/delete_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/delete_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/drop_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/drop_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/drop_udf_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/drop_udf_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/explain_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/explain_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/faiss_index_scan_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/faiss_index_scan_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/function_scan_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/function_scan_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/groupby_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/groupby_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/hash_join_build_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/hash_join_build_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/hash_join_probe_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/hash_join_probe_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/insert_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/insert_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/lateral_join_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/lateral_join_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/limit_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/limit_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/load_data_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/load_data_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/nested_loop_join_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/nested_loop_join_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/orderby_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/orderby_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/pp_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/pp_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/predicate_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/predicate_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/project_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/project_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/rename_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/rename_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/sample_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/sample_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/seq_scan_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/seq_scan_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/show_info_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/show_info_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/storage_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/storage_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/types.py` & `evadb-0.2.3.post0/eva/plan_nodes/types.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/plan_nodes/union_plan.py` & `evadb-0.2.3.post0/eva/plan_nodes/union_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/readers/__init__.py` & `evadb-0.2.3.post0/eva/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/readers/abstract_reader.py` & `evadb-0.2.3.post0/eva/readers/abstract_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/readers/csv_reader.py` & `evadb-0.2.3.post0/eva/readers/csv_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/readers/decord_reader.py` & `evadb-0.2.3.post0/eva/readers/decord_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/readers/image/__init__.py` & `evadb-0.2.3.post0/eva/readers/image/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/readers/image/opencv_image_reader.py` & `evadb-0.2.3.post0/eva/readers/image/opencv_image_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/server/__init__.py` & `evadb-0.2.3.post0/eva/server/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/server/command_handler.py` & `evadb-0.2.3.post0/eva/server/command_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,15 @@
     """
     output = execute_query(query, report_time=True, **kwargs)
     if output:
         batch_list = list(output)
         return Batch.concat(batch_list, copy=False)
 
 
-@asyncio.coroutine
-def handle_request(client_writer, request_message):
+async def handle_request(client_writer, request_message):
     """
     Reads a request from a client and processes it
 
     If user inputs 'quit' stops the event loop
     otherwise just echoes user input
     """
     logger.debug("Receive request: --|" + str(request_message) + "|--")
```

### Comparing `evadb-0.2.3/eva/server/db_api.py` & `evadb-0.2.3.post0/eva/server/db_api.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/server/interpreter.py` & `evadb-0.2.3.post0/eva/server/interpreter.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/server/server.py` & `evadb-0.2.3.post0/eva/server/server.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/storage/__init__.py` & `evadb-0.2.3.post0/eva/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/storage/abstract_media_storage_engine.py` & `evadb-0.2.3.post0/eva/storage/abstract_media_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/storage/abstract_storage_engine.py` & `evadb-0.2.3.post0/eva/storage/abstract_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/storage/image_storage_engine.py` & `evadb-0.2.3.post0/eva/storage/image_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/storage/sqlite_storage_engine.py` & `evadb-0.2.3.post0/eva/storage/sqlite_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/storage/storage_engine.py` & `evadb-0.2.3.post0/eva/storage/storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/storage/video_storage_engine.py` & `evadb-0.2.3.post0/eva/storage/video_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/third_party/__init__.py` & `evadb-0.2.3.post0/eva/third_party/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/third_party/huggingface/__init__.py` & `evadb-0.2.3.post0/eva/third_party/huggingface/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/third_party/huggingface/binder.py` & `evadb-0.2.3.post0/eva/third_party/huggingface/binder.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/third_party/huggingface/create.py` & `evadb-0.2.3.post0/eva/third_party/huggingface/create.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/third_party/huggingface/model.py` & `evadb-0.2.3.post0/eva/third_party/huggingface/model.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/udfs/__init__.py` & `evadb-0.2.3.post0/eva/udfs/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/udfs/abstract/__init__.py` & `evadb-0.2.3.post0/eva/udfs/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/udfs/abstract/abstract_udf.py` & `evadb-0.2.3.post0/eva/udfs/abstract/abstract_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/udfs/abstract/hf_abstract_udf.py` & `evadb-0.2.3.post0/eva/udfs/abstract/hf_abstract_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/udfs/abstract/pytorch_abstract_udf.py` & `evadb-0.2.3.post0/eva/udfs/abstract/pytorch_abstract_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/udfs/asl_action_recognition.py` & `evadb-0.2.3.post0/eva/udfs/asl_action_recognition.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/udfs/chatgpt.py` & `evadb-0.2.3.post0/eva/udfs/chatgpt.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/udfs/decorators/__init__.py` & `evadb-0.2.3.post0/eva/udfs/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/udfs/decorators/decorators.py` & `evadb-0.2.3.post0/eva/udfs/decorators/decorators.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/udfs/decorators/io_descriptors/__init__.py` & `evadb-0.2.3.post0/eva/udfs/decorators/io_descriptors/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/udfs/decorators/io_descriptors/abstract_types.py` & `evadb-0.2.3.post0/eva/udfs/decorators/io_descriptors/abstract_types.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/udfs/decorators/io_descriptors/data_types.py` & `evadb-0.2.3.post0/eva/udfs/decorators/io_descriptors/data_types.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/udfs/decorators/utils.py` & `evadb-0.2.3.post0/eva/udfs/decorators/utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/udfs/emotion_detector.py` & `evadb-0.2.3.post0/eva/udfs/emotion_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/udfs/face_detector.py` & `evadb-0.2.3.post0/eva/udfs/face_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/udfs/fastrcnn_object_detector.py` & `evadb-0.2.3.post0/eva/udfs/fastrcnn_object_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/udfs/feature_extractor.py` & `evadb-0.2.3.post0/eva/udfs/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/udfs/gpu_compatible.py` & `evadb-0.2.3.post0/eva/udfs/gpu_compatible.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/udfs/mvit_action_recognition.py` & `evadb-0.2.3.post0/eva/udfs/mvit_action_recognition.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/udfs/ndarray/__init__.py` & `evadb-0.2.3.post0/eva/udfs/ndarray/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/udfs/ndarray/array_count.py` & `evadb-0.2.3.post0/eva/udfs/ndarray/array_count.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/udfs/ndarray/crop.py` & `evadb-0.2.3.post0/eva/udfs/ndarray/crop.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/udfs/ndarray/fuzzy_join.py` & `evadb-0.2.3.post0/eva/udfs/ndarray/fuzzy_join.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/udfs/ndarray/open.py` & `evadb-0.2.3.post0/eva/udfs/ndarray/open.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/udfs/ndarray/similarity.py` & `evadb-0.2.3.post0/eva/udfs/ndarray/similarity.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/udfs/ocr_extractor.py` & `evadb-0.2.3.post0/eva/udfs/ocr_extractor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/udfs/udf_bootstrap_queries.py` & `evadb-0.2.3.post0/eva/udfs/udf_bootstrap_queries.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/udfs/yolo_object_detector.py` & `evadb-0.2.3.post0/eva/udfs/yolo_object_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/utils/__init__.py` & `evadb-0.2.3.post0/eva/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/utils/errors.py` & `evadb-0.2.3.post0/eva/utils/errors.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/utils/generic_utils.py` & `evadb-0.2.3.post0/eva/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/utils/kv_cache.py` & `evadb-0.2.3.post0/eva/utils/kv_cache.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/utils/logging_manager.py` & `evadb-0.2.3.post0/eva/utils/logging_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/utils/s3_utils.py` & `evadb-0.2.3.post0/eva/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/utils/stats.py` & `evadb-0.2.3.post0/eva/utils/stats.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/eva/version.py` & `evadb-0.2.3.post0/eva/version.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,11 +11,11 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 _MAJOR = "0"
 _MINOR = "2"
-_REVISION = "3"
+_REVISION = "3.post0"
 
 VERSION_SHORT = f"{_MAJOR}.{_MINOR}"
 VERSION = f"{_MAJOR}.{_MINOR}.{_REVISION}"
```

### Comparing `evadb-0.2.3/evadb.egg-info/PKG-INFO` & `evadb-0.2.3.post0/evadb.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,250 +1,251 @@
 Metadata-Version: 2.1
 Name: evadb
-Version: 0.2.3
-Summary: EVA Video Database System (Think MySQL for videos).
+Version: 0.2.3.post0
+Summary: EVA AI-Relational Database System
 Home-page: https://github.com/georgia-tech-db/eva
-Download-URL: https://github.com/georgia-tech-db/eva
 Author: Georgia Tech Database Group
-Author-email: georgia.tech.db@gmail.com
+Author-email: arulraj@gatech.edu
 License: Apache License 2.0
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Download-URL: https://github.com/georgia-tech-db/eva
+Description: <div >
+          <a href="https://evadb.readthedocs.io/">
+            <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-banner.png" alt="EVA" width="1000px" margin-left="-5px">
+          </a>
+        </div>
+        
+        # EVA AI-Relational Database System
+        
+        <div>
+                <a href="https://colab.research.google.com/github/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb">
+                    <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open EVA on Colab"/>
+                </a>
+                <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">
+                    <img alt="Slack" src="https://img.shields.io/badge/slack-eva-ff69b4.svg?logo=slack">
+                </a>          
+                <img alt="PyPI" src="https://img.shields.io/pypi/v/evadb.svg"/>
+                <img alt="License" src="https://img.shields.io/badge/license-Apache%202-brightgreen.svg?logo=apache"/>
+                <img alt="Coverage Status" src="https://coveralls.io/repos/github/georgia-tech-db/eva/badge.svg?branch=master"/>     
+                <a href="https://github.com/orgs/georgia-tech-db/projects/3">
+                    <img src="https://img.shields.io/badge/eva-roadmap-ff3423" alt="Roadmap"/>
+                </a>
+                <a href="https://pepy.tech/project/evadb">
+                  <img alt="Downloads" src="https://static.pepy.tech/badge/evadb/month"/>
+                </a>
+                <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.7%20|%203.8%20|%203.9%20|%203.10-brightgreen"/>       
+        </div>
+        
+        <p align="center"> <b><h3>EVA is a database system for building simpler and faster AI-powered applications.</b></h3> </p>
+        
+        EVA is designed for supporting database applications that operate on both structured (tables, feature vectors) and unstructured data (videos, podcasts, PDFs, etc.) using deep learning models. It accelerates AI pipelines by 10-100x using a collection of optimizations inspired by time-tested relational database systems, including function caching, sampling, and cost-based predicate reordering. EVA supports an AI-oriented SQL-like query language tailored for analyzing unstructured data. It comes with a wide range of models for analyzing unstructured data, including models for object detection, question answering, OCR, text sentiment classification, face detection, etc. It is fully implemented in Python and licensed under the Apache license.
+        
+        ## Quick Links
+        
+        - [Features](#features)
+        - [Quick Start](#quick-start)
+        - [Documentation](#documentation)
+        - [Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
+        - [Architecture Diagram](#architecture-diagram)
+        - [Demo](#demo)
+        - [Illustrative Applications](#illustrative-applications)
+        - [Community and Support](#community-and-support)
+        - [Contributing](#contributing)
+        - [License](#license)
+        
+        ## Features
+        
+        - ð® Build simpler AI-powered applications using short SQL-like queries
+        - â¡ï¸ 10-100x faster AI pipelines using AI-centric query optimization  
+        - ð° Save money spent on GPU-driven inference
+        - ð First-class support for your custom deep learning models through user-defined functions
+        - ð¦ Built-in caching to eliminate redundant model invocations across queries
+        - â¨ï¸ First-class support for PyTorch and HuggingFace models
+        - ð Installable via pip and fully implemented in Python
+        
+        ## Demo
+        
+        Here are some illustrative EVA-backed applications (all of them are Jupyter notebooks that can be opened in Google Colab):
+        
+         * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/08-chatgpt.html">Using ChatGPT to ask questions based on videos</a>
+         * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html">Analysing traffic flow at an intersection</a>
+        
+         * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html">Examining the emotion palette of actors in a movie</a>
+         * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html">Classifying images based on their content</a>
+         * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/07-object-segmentation-huggingface.html">Image Segmentation using Hugging Face</a>
+         * ð® <a href="https://github.com/georgia-tech-db/license-plate-recognition">Recognizing license plates </a>
+         * ð® <a href="https://github.com/georgia-tech-db/toxicity-classification">Analysing toxicity of social media memes </a>
+        
+        ## Documentation
+        
+        * [Detailed Documentation](https://evadb.readthedocs.io/)
+          - If you are wondering why you might need an AI-relational database system, start with the page on <a href="https://evadb.readthedocs.io/en/stable/source/overview/video.html#">Video Database Systems</a>.
+          - The <a href="https://evadb.readthedocs.io/en/stable/source/overview/installation.html">Getting Started</a> page shows how you can use EVA for different AI pipelines, and how you can easily extend EVA by defining an user-defined function that wraps around your custom deep learning model.
+          - The <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/index.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EVA. Each notebook includes a link to Google Colab to run the code.
+        * [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
+        * [Join us on Slack!](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)
+        * [Medium-Term Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
+        * [Demo](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
+        
+        ## Quick Start
+        
+        - Install EVA using the pip package manager. EVA supports Python versions >= 3.7:
+        
+        ```shell
+        pip install evadb
+        ```
+        
+        - To launch and connect to an EVA server in a Jupyter notebook, check out this [illustrative emotion analysis notebook](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb):
+        ```shell
+        cursor = connect_to_server()
+        ```
+        
+        - Load a video onto the EVA server (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) for illustration):
+        
+        ```mysql
+        LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO TrafficVideo;
+        ```
+        
+        - That's it! You can now run queries over the loaded video:
+        
+        ```mysql
+        SELECT id, data FROM TrafficVideo WHERE id < 5;
+        ```
+        
+        - Search for frames in the video that contain a car:
+        
+        ```mysql
+        SELECT id, data FROM TrafficVideo WHERE ['car'] <@ Yolo(data).labels;
+        ```
+        | Source Video  | Query Result |
+        |---------------|--------------|
+        |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
+        
+        - Search for frames in the video that contain a pedestrian and a car:
+        
+        ```mysql
+        SELECT id, data FROM TrafficVideo WHERE ['pedestrian', 'car'] <@ Yolo(data).labels;
+        ```
+        
+        - Search for frames with more than three cars:
+        
+        ```mysql
+        SELECT id, data FROM TrafficVideo WHERE ArrayCount(Yolo(data).labels, 'car') > 3;
+        ```
+        
+        - **Use your custom deep learning model in queries** with a user-defined function (UDF):
+        
+        ```mysql
+        CREATE UDF IF NOT EXISTS Yolo
+        TYPE  ultralytics
+        'model' 'yolov8m.pt';
+        ```
+        
+        - **Compose multiple models in a single query** to set up useful AI pipelines.
+        
+        ```mysql
+           -- Analyse emotions of faces in a video
+           SELECT id, bbox, EmotionDetector(Crop(data, bbox)) 
+           FROM MovieVideo JOIN LATERAL UNNEST(FaceDetector(data)) AS Face(bbox, conf)  
+           WHERE id < 15;
+        ```
+        
+        - **EVA runs queries faster using its AI-centric query optimizer**. Two key optimizations are:
+        
+           ð¾ **Caching**: EVA automatically caches and reuses previous query results (especially model inference results), eliminating redundant computation and reducing query processing time.
+        
+           ð¯ **Predicate Reordering**: EVA optimizes the order in which the query predicates are evaluated (e.g., runs the faster, more selective model first), leading to faster queries and lower inference costs.
+        
+        Consider these two exploratory queries on a dataset of ð images:
+        <img align="right" style="display:inline;" width="40%" src="https://github.com/georgia-tech-db/eva/blob/master/data/assets/eva_performance_comparison.png?raw=true"></a>
+        
+        ```mysql
+          -- Query 1: Find all images of black-colored dogs
+          SELECT id, bbox FROM dogs 
+          JOIN LATERAL UNNEST(Yolo(data)) AS Obj(label, bbox, score) 
+          WHERE Obj.label = 'dog' 
+            AND Color(Crop(data, bbox)) = 'black'; 
+        
+          -- Query 2: Find all Great Danes that are black-colored
+          SELECT id, bbox FROM dogs 
+          JOIN LATERAL UNNEST(Yolo(data)) AS Obj(label, bbox, score) 
+          WHERE Obj.label = 'dog' 
+            AND DogBreedClassifier(Crop(data, bbox)) = 'great dane' 
+            AND Color(Crop(data, bbox)) = 'black';
+        ```
+        
+        By reusing the results of the first query and reordering the predicates based on the available cached inference results, EVA runs the second query **10x faster**!
+        
+        ## Architecture Diagram
+        
+        The following architecture diagram presents the critical components of the EVA database system. EVA's AI-centric Query Optimizer takes a parsed query as input and generates a query plan that is then executed by the Query Engine. The Query Engine hits multiple storage engines to retrieve the data required for efficiently running the query:
+        1. Structured data (relational database system connected via `sqlalchemy`).
+        2. Unstructured media data (on cloud buckets or local filesystem).
+        3. Vector data (vector database system).
+        
+        <img width="700" alt="Architecture Diagram" src="https://github.com/georgia-tech-db/eva/assets/5521975/01452ec9-87d9-4d27-90b2-c0b1ab29b16c">
+        
+        ## Illustrative Applications 
+        
+        ### ð® [Traffic Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html) (Object Detection Model)
+        | Source Video  | Query Result |
+        |---------------|--------------|
+        |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
+        
+        ### ð® [MNIST Digit Recognition](https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html) (Image Classification Model)
+        | Source Video  | Query Result |
+        |---------------|--------------|
+        |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-input.webp" width="150"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-output.webp" width="150"> |
+        
+        ### ð® [Movie Emotion Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html) (Face Detection + Emotion Classfication Models)
+        
+        | Source Video  | Query Result |
+        |---------------|--------------|
+        |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-input.webp" width="400"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-output.webp" width="400"> |
+        
+        ### ð® [License Plate Recognition](https://github.com/georgia-tech-db/eva-application-template) (Plate Detection + OCR Extraction Models)
+        
+        | Query Result |
+        |--------------|
+        <img alt="Query Result" src="https://github.com/georgia-tech-db/license-plate-recognition/blob/main/README_files/README_12_3.png" width="300"> |
+        
+        ### ð® [Meme Toxicity Classification](https://github.com/georgia-tech-db/toxicity-classification) (OCR Extraction + Toxicity Classification Models)
+        
+        | Query Result |
+        |--------------|
+        <img alt="Query Result" src="https://raw.githubusercontent.com/georgia-tech-db/toxicity-classification/main/README_files/README_16_2.png" width="200"> |
+        
+        ## Community and Support
+        
+        ð If you have general questions about EVA, want to say hello or just follow along, we'd like to invite you to join our [Slack Community](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg).
+        
+        <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">              
+            <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-slack.png" alt="EVA Slack Channel" width="500">
+        </a>
+        
+        If you run into any problems or issues, please create a Github issue and we'll try our best to help.
+        
+        Don't see a feature in the list? Search our issue tracker if someone has already requested it and add a comment to it explaining your use-case, or open a new issue if not. We prioritize our roadmap based on user feedback, so we'd love to hear from you.
+        
+        ## Contributing
+        
+        [![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)](https://pypi.org/project/evadb)
+        [![CI Status](https://circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva)
+        [![Documentation Status](https://readthedocs.org/projects/evadb/badge/?version=stable)](https://evadb.readthedocs.io/en/stable/index.html)
+        
+        EVA is the beneficiary of many [contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All kinds of contributions to EVA are appreciated. To file a bug or to request a feature, please use <a href="https://github.com/georgia-tech-db/eva/issues">GitHub issues</a>. <a href="https://github.com/georgia-tech-db/eva/pulls">Pull requests</a> are welcome.
+        
+        For more information, see our
+        [contribution guide](https://evadb.readthedocs.io/en/stable/source/contribute/index.html).
+        
+        ## License
+        Copyright (c) 2018-present [Georgia Tech Database Group](http://db.cc.gatech.edu/).
+        Licensed under [Apache License](LICENSE).
+        
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 3 - Alpha
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-License-File: LICENSE.txt
-
-<div >
-  <a href="https://evadb.readthedocs.io/">
-    <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-banner.png" alt="EVA" width="1000px" margin-left="-5px">
-  </a>
-</div>
-
-# EVA AI-Relational Database System
-
-<div>
-        <a href="https://colab.research.google.com/github/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb">
-            <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open EVA on Colab"/>
-        </a>
-        <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">
-            <img alt="Slack" src="https://img.shields.io/badge/slack-eva-ff69b4.svg?logo=slack">
-        </a>          
-        <img alt="PyPI" src="https://img.shields.io/pypi/v/evadb.svg"/>
-        <img alt="License" src="https://img.shields.io/badge/license-Apache%202-brightgreen.svg?logo=apache"/>
-        <img alt="Coverage Status" src="https://coveralls.io/repos/github/georgia-tech-db/eva/badge.svg?branch=master"/>     
-        <a href="https://github.com/orgs/georgia-tech-db/projects/3">
-            <img src="https://img.shields.io/badge/eva-roadmap-ff3423" alt="Roadmap"/>
-        </a>
-        <a href="https://pepy.tech/project/evadb">
-          <img alt="Downloads" src="https://static.pepy.tech/badge/evadb/month"/>
-        </a>
-        <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.7%20|%203.8%20|%203.9%20|%203.10-brightgreen"/>       
-</div>
-
-<p align="center"> <b><h3>EVA is a database system for building simpler and faster AI-powered applications.</b></h3> </p>
-
-EVA is designed for supporting database applications that operate on both structured (tables, feature vectors) and unstructured data (videos, podcasts, PDFs, etc.) using deep learning models. It accelerates AI pipelines by 10-100x using a collection of optimizations inspired by time-tested relational database systems, including function caching, sampling, and cost-based predicate reordering. EVA supports an AI-oriented SQL-like query language tailored for analyzing unstructured data. It comes with a wide range of models for analyzing unstructured data, including models for object detection, question answering, OCR, text sentiment classification, face detection, etc. It is fully implemented in Python and licensed under the Apache license.
-
-## Quick Links
-
-- [Features](#features)
-- [Quick Start](#quick-start)
-- [Documentation](#documentation)
-- [Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
-- [Demo](#demo)
-- [Illustrative Applications](#illustrative-applications)
-- [Community and Support](#community-and-support)
-- [Contributing](#contributing)
-- [License](#license)
-
-## Features
-
-- 🔮 Build simpler AI-powered applications using short SQL-like queries
-- ⚡️ 10-100x faster AI pipelines using AI-centric query optimization  
-- 💰 Save money spent on GPU-driven inference
-- 🚀 First-class support for your custom deep learning models through user-defined functions
-- 📦 Built-in caching to eliminate redundant model invocations across queries
-- ⌨️ First-class support for PyTorch and HuggingFace models
-- 🐍 Installable via pip and fully implemented in Python
-
-## Demo
-
-Here are some illustrative EVA-backed applications (all of them are Jupyter notebooks that can be opened in Google Colab):
-
- * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html">Analysing traffic flow at an intersection</a>
- * 🔮 <a href="https://evadb.readthedocs.io/en/latest/source/tutorials/08-chatgpt.html">Asking questions based on videos</a>
- * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html">Examining the emotion palette of actors in a movie</a>
- * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html">Classifying images based on their content</a>
- * 🔮 <a href="https://evadb.readthedocs.io/en/latest/source/tutorials/07-object-segmentation-huggingface.html">Image Segmentation using Hugging Face</a>
- * 🔮 <a href="https://github.com/georgia-tech-db/license-plate-recognition">Recognizing license plates </a>
- * 🔮 <a href="https://github.com/georgia-tech-db/toxicity-classification">Analysing toxicity of social media memes </a>
-
-## Documentation
-
-* [Detailed Documentation](https://evadb.readthedocs.io/)
-  - If you are wondering why you might need an AI-relational database system, start with the page on <a href="https://evadb.readthedocs.io/en/stable/source/overview/video.html#">Video Database Systems</a>.
-  - The <a href="https://evadb.readthedocs.io/en/stable/source/overview/installation.html">Getting Started</a> page shows how you can use EVA for different AI pipelines, and how you can easily extend EVA by defining an user-defined function that wraps around your custom deep learning model.
-  - The <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/index.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EVA. Each notebook includes a link to Google Colab to run the code.
-* [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
-* [Join us on Slack!](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)
-* [Medium-Term Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
-* [Demo](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
-
-## Quick Start
-
-- Install EVA using the pip package manager. EVA supports Python versions >= 3.7:
-
-```shell
-pip install evadb
-```
-
-- To launch and connect to an EVA server in a Jupyter notebook, check out this [illustrative emotion analysis notebook](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb):
-```shell
-cursor = connect_to_server()
-```
-
-- Load a video onto the EVA server (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) for illustration):
-
-```mysql
-LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO TrafficVideo;
-```
-
-- That's it! You can now run queries over the loaded video:
-
-```mysql
-SELECT id, data FROM TrafficVideo WHERE id < 5;
-```
-
-- Search for frames in the video that contain a car:
-
-```mysql
-SELECT id, data FROM TrafficVideo WHERE ['car'] <@ Yolo(data).labels;
-```
-| Source Video  | Query Result |
-|---------------|--------------|
-|<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
-
-- Search for frames in the video that contain a pedestrian and a car:
-
-```mysql
-SELECT id, data FROM TrafficVideo WHERE ['pedestrian', 'car'] <@ Yolo(data).labels;
-```
-
-- Search for frames with more than three cars:
-
-```mysql
-SELECT id, data FROM TrafficVideo WHERE ArrayCount(Yolo(data).labels, 'car') > 3;
-```
-
-- **Use your custom deep learning model in queries** with a user-defined function (UDF):
-
-```mysql
-CREATE UDF IF NOT EXISTS Yolo
-TYPE  ultralytics
-'model' 'yolov8m.pt';
-```
-
-- **Compose multiple models in a single query** to set up useful AI pipelines.
-
-```mysql
-   -- Analyse emotions of faces in a video
-   SELECT id, bbox, EmotionDetector(Crop(data, bbox)) 
-   FROM MovieVideo JOIN LATERAL UNNEST(FaceDetector(data)) AS Face(bbox, conf)  
-   WHERE id < 15;
-```
-
-- **EVA runs queries faster using its AI-centric query optimizer**. Two key optimizations are:
-
-   💾 **Caching**: EVA automatically caches and reuses previous query results (especially model inference results), eliminating redundant computation and reducing query processing time.
-
-   🎯 **Predicate Reordering**: EVA optimizes the order in which the query predicates are evaluated (e.g., runs the faster, more selective model first), leading to faster queries and lower inference costs.
-
-Consider these two exploratory queries on a dataset of 🐕 images:
-<img align="right" style="display:inline;" width="40%" src="https://github.com/georgia-tech-db/eva/blob/master/data/assets/eva_performance_comparison.png?raw=true"></a>
-
-```mysql
-  -- Query 1: Find all images of black-colored dogs
-  SELECT id, bbox FROM dogs 
-  JOIN LATERAL UNNEST(Yolo(data)) AS Obj(label, bbox, score) 
-  WHERE Obj.label = 'dog' 
-    AND Color(Crop(data, bbox)) = 'black'; 
-
-  -- Query 2: Find all Great Danes that are black-colored
-  SELECT id, bbox FROM dogs 
-  JOIN LATERAL UNNEST(Yolo(data)) AS Obj(label, bbox, score) 
-  WHERE Obj.label = 'dog' 
-    AND DogBreedClassifier(Crop(data, bbox)) = 'great dane' 
-    AND Color(Crop(data, bbox)) = 'black';
-```
-
-By reusing the results of the first query and reordering the predicates based on the available cached inference results, EVA runs the second query **10x faster**!
-
-## Architecture Diagram
-
-The following architecture diagram presents the critical components of the EVA database system. EVA's AI-centric Query Optimizer takes a parsed query as input and generates a query plan that is then executed by the Query Engine. The Query Engine hits multiple storage engines to retrieve the data required for efficiently running the query:
-1. Structured data (relational database system connected via `sqlalchemy`).
-2. Unstructured media data (on cloud buckets or local filesystem).
-3. Vector data (vector database system).
-
-<img width="700" alt="Architecture Diagram" src="https://github.com/georgia-tech-db/eva/assets/5521975/01452ec9-87d9-4d27-90b2-c0b1ab29b16c">
-
-## Illustrative Applications 
-
-### 🔮 [Traffic Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html) (Object Detection Model)
-| Source Video  | Query Result |
-|---------------|--------------|
-|<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
-
-### 🔮 [MNIST Digit Recognition](https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html) (Image Classification Model)
-| Source Video  | Query Result |
-|---------------|--------------|
-|<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-input.webp" width="150"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-output.webp" width="150"> |
-
-### 🔮 [Movie Emotion Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html) (Face Detection + Emotion Classfication Models)
-
-| Source Video  | Query Result |
-|---------------|--------------|
-|<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-input.webp" width="400"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-output.webp" width="400"> |
-
-### 🔮 [License Plate Recognition](https://github.com/georgia-tech-db/eva-application-template) (Plate Detection + OCR Extraction Models)
-
-| Query Result |
-|--------------|
-<img alt="Query Result" src="https://github.com/georgia-tech-db/license-plate-recognition/blob/main/README_files/README_12_3.png" width="300"> |
-
-### 🔮 [Meme Toxicity Classification](https://github.com/georgia-tech-db/toxicity-classification) (OCR Extraction + Toxicity Classification Models)
-
-| Query Result |
-|--------------|
-<img alt="Query Result" src="https://raw.githubusercontent.com/georgia-tech-db/toxicity-classification/main/README_files/README_16_2.png" width="200"> |
-
-## Community and Support
-
-👋 If you have general questions about EVA, want to say hello or just follow along, we'd like to invite you to join our [Slack Community](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg).
-
-<a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">              
-    <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-slack.png" alt="EVA Slack Channel" width="500">
-</a>
-
-If you run into any problems or issues, please create a Github issue and we'll try our best to help.
-
-Don't see a feature in the list? Search our issue tracker if someone has already requested it and add a comment to it explaining your use-case, or open a new issue if not. We prioritize our roadmap based on user feedback, so we'd love to hear from you.
-
-## Contributing
-
-[![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)](https://pypi.org/project/evadb)
-[![CI Status](https://circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva)
-[![Documentation Status](https://readthedocs.org/projects/evadb/badge/?version=stable)](https://evadb.readthedocs.io/en/stable/index.html)
-
-EVA is the beneficiary of many [contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All kinds of contributions to EVA are appreciated. To file a bug or to request a feature, please use <a href="https://github.com/georgia-tech-db/eva/issues">GitHub issues</a>. <a href="https://github.com/georgia-tech-db/eva/pulls">Pull requests</a> are welcome.
-
-For more information, see our
-[contribution guide](https://evadb.readthedocs.io/en/stable/source/contribute/index.html).
-
-## License
-Copyright (c) 2018-present [Georgia Tech Database Group](http://db.cc.gatech.edu/).
-Licensed under [Apache License](LICENSE).
```

#### html2text {}

```diff
@@ -1,17 +1,12 @@
-Metadata-Version: 2.1 Name: evadb Version: 0.2.3 Summary: EVA Video Database
-System (Think MySQL for videos). Home-page: https://github.com/georgia-tech-db/
-eva Download-URL: https://github.com/georgia-tech-db/eva Author: Georgia Tech
-Database Group Author-email: georgia.tech.db@gmail.com License: Apache License
-2.0 Classifier: Intended Audience :: Science/Research Classifier: Topic ::
-Scientific/Engineering :: Information Analysis Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Programming Language :: Python
-:: 3 Classifier: Development Status :: 3 - Alpha Classifier: Operating System
-:: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
-markdown Provides-Extra: dev License-File: LICENSE.txt
+Metadata-Version: 2.1 Name: evadb Version: 0.2.3.post0 Summary: EVA AI-
+Relational Database System Home-page: https://github.com/georgia-tech-db/eva
+Author: Georgia Tech Database Group Author-email: arulraj@gatech.edu License:
+Apache License 2.0 Download-URL: https://github.com/georgia-tech-db/eva
+Description:
 [EVA]
 # EVA AI-Relational Database System
 [Open_EVA_on_Colab] [Slack] [PyPI] [License] [Coverage Status] [Roadmap]
 [Downloads] [Python Versions]
 **** EVA is a database system for building simpler and faster AI-powered
 applications. ****
 EVA is designed for supporting database applications that operate on both
@@ -22,49 +17,50 @@
 reordering. EVA supports an AI-oriented SQL-like query language tailored for
 analyzing unstructured data. It comes with a wide range of models for analyzing
 unstructured data, including models for object detection, question answering,
 OCR, text sentiment classification, face detection, etc. It is fully
 implemented in Python and licensed under the Apache license. ## Quick Links -
 [Features](#features) - [Quick Start](#quick-start) - [Documentation]
 (#documentation) - [Roadmap](https://github.com/orgs/georgia-tech-db/projects/
-3) - [Demo](#demo) - [Illustrative Applications](#illustrative-applications) -
-[Community and Support](#community-and-support) - [Contributing](#contributing)
-- [License](#license) ## Features - ð® Build simpler AI-powered applications
-using short SQL-like queries - â¡ï¸ 10-100x faster AI pipelines using AI-
-centric query optimization - ð° Save money spent on GPU-driven inference -
-ð First-class support for your custom deep learning models through user-
-defined functions - ð¦ Built-in caching to eliminate redundant model
-invocations across queries - â¨ï¸ First-class support for PyTorch and
-HuggingFace models - ð Installable via pip and fully implemented in Python
-## Demo Here are some illustrative EVA-backed applications (all of them are
-Jupyter notebooks that can be opened in Google Colab): * ð® Analysing_traffic
-flow_at_an_intersection * ð® Asking_questions_based_on_videos * ð®
-Examining_the_emotion_palette_of_actors_in_a_movie * ð® Classifying_images
-based_on_their_content * ð® Image_Segmentation_using_Hugging_Face * ð®
-Recognizing_license_plates * ð® Analysing_toxicity_of_social_media_memes ##
-Documentation * [Detailed Documentation](https://evadb.readthedocs.io/) - If
-you are wondering why you might need an AI-relational database system, start
-with the page on Video_Database_Systems. - The Getting_Started page shows how
-you can use EVA for different AI pipelines, and how you can easily extend EVA
-by defining an user-defined function that wraps around your custom deep
-learning model. - The User_Guides section contains Jupyter Notebooks that
-demonstrate how to use various features of EVA. Each notebook includes a link
-to Google Colab to run the code. * [Tutorials](https://github.com/georgia-tech-
-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb) * [Join us on Slack!]
-(https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-
-PlJ4iawLdurDv~aIAq90Dg) * [Medium-Term Roadmap](https://github.com/orgs/
-georgia-tech-db/projects/3) * [Demo](https://github.com/georgia-tech-db/eva/
-blob/master/tutorials/03-emotion-analysis.ipynb) ## Quick Start - Install EVA
-using the pip package manager. EVA supports Python versions >= 3.7: ```shell
-pip install evadb ``` - To launch and connect to an EVA server in a Jupyter
-notebook, check out this [illustrative emotion analysis notebook](https://
-github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-
-analysis.ipynb): ```shell cursor = connect_to_server() ``` - Load a video onto
-the EVA server (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) for
-illustration): ```mysql LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO
+3) - [Architecture Diagram](#architecture-diagram) - [Demo](#demo) -
+[Illustrative Applications](#illustrative-applications) - [Community and
+Support](#community-and-support) - [Contributing](#contributing) - [License]
+(#license) ## Features - Ã°ÂÂÂ® Build simpler AI-powered applications using
+short SQL-like queries - Ã¢ÂÂ¡Ã¯Â¸Â 10-100x faster AI pipelines using AI-
+centric query optimization - Ã°ÂÂÂ° Save money spent on GPU-driven inference
+- Ã°ÂÂÂ First-class support for your custom deep learning models through
+user-defined functions - Ã°ÂÂÂ¦ Built-in caching to eliminate redundant model
+invocations across queries - Ã¢ÂÂ¨Ã¯Â¸Â First-class support for PyTorch and
+HuggingFace models - Ã°ÂÂÂ Installable via pip and fully implemented in
+Python ## Demo Here are some illustrative EVA-backed applications (all of them
+are Jupyter notebooks that can be opened in Google Colab): * Ã°ÂÂÂ® Using
+ChatGPT_to_ask_questions_based_on_videos * Ã°ÂÂÂ® Analysing_traffic_flow_at
+an_intersection * Ã°ÂÂÂ® Examining_the_emotion_palette_of_actors_in_a_movie *
+Ã°ÂÂÂ® Classifying_images_based_on_their_content * Ã°ÂÂÂ® Image
+Segmentation_using_Hugging_Face * Ã°ÂÂÂ® Recognizing_license_plates *
+Ã°ÂÂÂ® Analysing_toxicity_of_social_media_memes ## Documentation * [Detailed
+Documentation](https://evadb.readthedocs.io/) - If you are wondering why you
+might need an AI-relational database system, start with the page on Video
+Database_Systems. - The Getting_Started page shows how you can use EVA for
+different AI pipelines, and how you can easily extend EVA by defining an user-
+defined function that wraps around your custom deep learning model. - The User
+Guides section contains Jupyter Notebooks that demonstrate how to use various
+features of EVA. Each notebook includes a link to Google Colab to run the code.
+* [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-
+emotion-analysis.ipynb) * [Join us on Slack!](https://join.slack.com/t/eva-db/
+shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) * [Medium-Term Roadmap]
+(https://github.com/orgs/georgia-tech-db/projects/3) * [Demo](https://
+github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
+## Quick Start - Install EVA using the pip package manager. EVA supports Python
+versions >= 3.7: ```shell pip install evadb ``` - To launch and connect to an
+EVA server in a Jupyter notebook, check out this [illustrative emotion analysis
+notebook](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-
+emotion-analysis.ipynb): ```shell cursor = connect_to_server() ``` - Load a
+video onto the EVA server (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4)
+for illustration): ```mysql LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO
 TrafficVideo; ``` - That's it! You can now run queries over the loaded video:
 ```mysql SELECT id, data FROM TrafficVideo WHERE id < 5; ``` - Search for
 frames in the video that contain a car: ```mysql SELECT id, data FROM
 TrafficVideo WHERE ['car'] <@ Yolo(data).labels; ``` | Source Video | Query
 Result | |---------------|--------------| |[Source Video] |[Query Result] | -
 Search for frames in the video that contain a pedestrian and a car: ```mysql
 SELECT id, data FROM TrafficVideo WHERE ['pedestrian', 'car'] <@ Yolo
@@ -73,22 +69,22 @@
 3; ``` - **Use your custom deep learning model in queries** with a user-defined
 function (UDF): ```mysql CREATE UDF IF NOT EXISTS Yolo TYPE ultralytics 'model'
 'yolov8m.pt'; ``` - **Compose multiple models in a single query** to set up
 useful AI pipelines. ```mysql -- Analyse emotions of faces in a video SELECT
 id, bbox, EmotionDetector(Crop(data, bbox)) FROM MovieVideo JOIN LATERAL UNNEST
 (FaceDetector(data)) AS Face(bbox, conf) WHERE id < 15; ``` - **EVA runs
 queries faster using its AI-centric query optimizer**. Two key optimizations
-are: ð¾ **Caching**: EVA automatically caches and reuses previous query
+are: Ã°ÂÂÂ¾ **Caching**: EVA automatically caches and reuses previous query
 results (especially model inference results), eliminating redundant computation
-and reducing query processing time. ð¯ **Predicate Reordering**: EVA
+and reducing query processing time. Ã°ÂÂÂ¯ **Predicate Reordering**: EVA
 optimizes the order in which the query predicates are evaluated (e.g., runs the
 faster, more selective model first), leading to faster queries and lower
-inference costs. Consider these two exploratory queries on a dataset of ð
-images: [https://github.com/georgia-tech-db/eva/blob/master/data/assets/
-eva_performance_comparison.png?raw=true]
+inference costs. Consider these two exploratory queries on a dataset of
+Ã°ÂÂÂ images: [https://github.com/georgia-tech-db/eva/blob/master/data/
+assets/eva_performance_comparison.png?raw=true]
  ```mysql -- Query 1: Find all images of black-colored dogs SELECT id, bbox
 FROM dogs JOIN LATERAL UNNEST(Yolo(data)) AS Obj(label, bbox, score) WHERE
 Obj.label = 'dog' AND Color(Crop(data, bbox)) = 'black'; -- Query 2: Find all
 Great Danes that are black-colored SELECT id, bbox FROM dogs JOIN LATERAL
 UNNEST(Yolo(data)) AS Obj(label, bbox, score) WHERE Obj.label = 'dog' AND
 DogBreedClassifier(Crop(data, bbox)) = 'great dane' AND Color(Crop(data, bbox))
 = 'black'; ``` By reusing the results of the first query and reordering the
@@ -97,42 +93,48 @@
 diagram presents the critical components of the EVA database system. EVA's AI-
 centric Query Optimizer takes a parsed query as input and generates a query
 plan that is then executed by the Query Engine. The Query Engine hits multiple
 storage engines to retrieve the data required for efficiently running the
 query: 1. Structured data (relational database system connected via
 `sqlalchemy`). 2. Unstructured media data (on cloud buckets or local
 filesystem). 3. Vector data (vector database system). [Architecture Diagram] ##
-Illustrative Applications ### ð® [Traffic Analysis](https://
+Illustrative Applications ### Ã°ÂÂÂ® [Traffic Analysis](https://
 evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html)
 (Object Detection Model) | Source Video | Query Result | |---------------|-----
----------| |[Source Video] |[Query Result] | ### ð® [MNIST Digit Recognition]
-(https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html) (Image
-Classification Model) | Source Video | Query Result | |---------------|--------
-------| |[Source Video] |[Query Result] | ### ð® [Movie Emotion Analysis]
-(https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-
-analysis.html) (Face Detection + Emotion Classfication Models) | Source Video |
-Query Result | |---------------|--------------| |[Source Video] |[Query Result]
-| ### ð® [License Plate Recognition](https://github.com/georgia-tech-db/eva-
-application-template) (Plate Detection + OCR Extraction Models) | Query Result
-| |--------------| [Query Result] | ### ð® [Meme Toxicity Classification]
-(https://github.com/georgia-tech-db/toxicity-classification) (OCR Extraction +
-Toxicity Classification Models) | Query Result | |--------------| [Query
-Result] | ## Community and Support ð If you have general questions about
-EVA, want to say hello or just follow along, we'd like to invite you to join
-our [Slack Community](https://join.slack.com/t/eva-db/shared_invite/zt-
-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg). [EVA_Slack_Channel] If you run into any
-problems or issues, please create a Github issue and we'll try our best to
-help. Don't see a feature in the list? Search our issue tracker if someone has
-already requested it and add a comment to it explaining your use-case, or open
-a new issue if not. We prioritize our roadmap based on user feedback, so we'd
-love to hear from you. ## Contributing [![PyPI Version](https://img.shields.io/
-pypi/v/evadb.svg)](https://pypi.org/project/evadb) [![CI Status](https://
-circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https://circleci.com/gh/
-georgia-tech-db/eva) [![Documentation Status](https://readthedocs.org/projects/
-evadb/badge/?version=stable)](https://evadb.readthedocs.io/en/stable/
-index.html) EVA is the beneficiary of many [contributors](https://github.com/
-georgia-tech-db/eva/graphs/contributors). All kinds of contributions to EVA are
-appreciated. To file a bug or to request a feature, please use GitHub_issues.
-Pull_requests are welcome. For more information, see our [contribution guide]
-(https://evadb.readthedocs.io/en/stable/source/contribute/index.html). ##
-License Copyright (c) 2018-present [Georgia Tech Database Group](http://
-db.cc.gatech.edu/). Licensed under [Apache License](LICENSE).
+---------| |[Source Video] |[Query Result] | ### Ã°ÂÂÂ® [MNIST Digit
+Recognition](https://evadb.readthedocs.io/en/stable/source/tutorials/01-
+mnist.html) (Image Classification Model) | Source Video | Query Result | |-----
+----------|--------------| |[Source Video] |[Query Result] | ### Ã°ÂÂÂ®
+[Movie Emotion Analysis](https://evadb.readthedocs.io/en/stable/source/
+tutorials/03-emotion-analysis.html) (Face Detection + Emotion Classfication
+Models) | Source Video | Query Result | |---------------|--------------| |
+[Source Video] |[Query Result] | ### Ã°ÂÂÂ® [License Plate Recognition]
+(https://github.com/georgia-tech-db/eva-application-template) (Plate Detection
++ OCR Extraction Models) | Query Result | |--------------| [Query Result] | ###
+Ã°ÂÂÂ® [Meme Toxicity Classification](https://github.com/georgia-tech-db/
+toxicity-classification) (OCR Extraction + Toxicity Classification Models) |
+Query Result | |--------------| [Query Result] | ## Community and Support
+Ã°ÂÂÂ If you have general questions about EVA, want to say hello or just
+follow along, we'd like to invite you to join our [Slack Community](https://
+join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg).
+[EVA_Slack_Channel] If you run into any problems or issues, please create a
+Github issue and we'll try our best to help. Don't see a feature in the list?
+Search our issue tracker if someone has already requested it and add a comment
+to it explaining your use-case, or open a new issue if not. We prioritize our
+roadmap based on user feedback, so we'd love to hear from you. ## Contributing
+[![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)](https://pypi.org/
+project/evadb) [![CI Status](https://circleci.com/gh/georgia-tech-db/
+eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva) [!
+[Documentation Status](https://readthedocs.org/projects/evadb/badge/
+?version=stable)](https://evadb.readthedocs.io/en/stable/index.html) EVA is the
+beneficiary of many [contributors](https://github.com/georgia-tech-db/eva/
+graphs/contributors). All kinds of contributions to EVA are appreciated. To
+file a bug or to request a feature, please use GitHub_issues. Pull_requests are
+welcome. For more information, see our [contribution guide](https://
+evadb.readthedocs.io/en/stable/source/contribute/index.html). ## License
+Copyright (c) 2018-present [Georgia Tech Database Group](http://
+db.cc.gatech.edu/). Licensed under [Apache License](LICENSE). Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
+OSI Approved :: Apache Software License Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Requires-Python: >=3.8 Description-
+Content-Type: text/markdown Provides-Extra: dev
```

### Comparing `evadb-0.2.3/evadb.egg-info/SOURCES.txt` & `evadb-0.2.3.post0/evadb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/evadb.egg-info/requires.txt` & `evadb-0.2.3.post0/evadb.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,69 +1,71 @@
-numpy<=1.23.5,>=1.19.5
-opencv-python<4.6.0.66,>=4.5.4.60
-pandas>=1.1.5
 Pillow>=8.4.0
-sqlalchemy<2.0.0,>=1.4.0
-sqlalchemy-utils>=0.36.6
-lark>=1.0.0
-pyyaml>=5.1
-importlib-metadata<5.0
-ray>=1.13.0
 aenum>=2.2.0
+boto3
 diskcache>=5.4.0
-eva-decord==0.6.1
-torch>=1.10.0
-torchvision>=0.11.1
-faiss-cpu
+eva-decord>=0.6.1
 facenet-pytorch>=2.5.2
-easyocr>=1.5.0
+faiss-cpu
+importlib-metadata<5.0
 ipython<8.13.0
-thefuzz
-ultralytics
-transformers>=4.27.4
+lark>=1.0.0
+nest_asyncio
+numpy>=1.19.5
 openai>=0.27.4
-timm>=0.6.13
-
-[dev]
-numpy<=1.23.5,>=1.19.5
-opencv-python<4.6.0.66,>=4.5.4.60
+opencv-python>=4.6.0.66
 pandas>=1.1.5
-Pillow>=8.4.0
-sqlalchemy<2.0.0,>=1.4.0
-sqlalchemy-utils>=0.36.6
-lark>=1.0.0
 pyyaml>=5.1
-importlib-metadata<5.0
 ray>=1.13.0
-aenum>=2.2.0
-diskcache>=5.4.0
-eva-decord==0.6.1
+sqlalchemy-utils>=0.36.6
+sqlalchemy<2.0.0,>=1.4.0
+thefuzz
+timm>=0.6.13
 torch>=1.10.0
 torchvision>=0.11.1
-faiss-cpu
-facenet-pytorch>=2.5.2
-easyocr>=1.5.0
-ipython<8.13.0
-thefuzz
-ultralytics
 transformers>=4.27.4
-openai>=0.27.4
-timm>=0.6.13
+ultralytics>=8.0.93
+
+[dev]
+Pillow>=8.4.0
+aenum>=2.2.0
 black>=23.1.0
-isort>=5.10.1
-pytest>=6.1.2
-pytest-cov>=2.11.1
-pytest-random-order>=1.0.4
-pytest-virtualenv
-pytest-asyncio
-pytest-xdist
+boto3
 coveralls>=3.0.1
+diskcache>=5.4.0
+eva-decord>=0.6.1
+facenet-pytorch>=2.5.2
+faiss-cpu
 flake8>=3.9.1
-moto[s3]>=4.1.1
+importlib-metadata<5.0
+ipython<8.13.0
 ipywidgets>=7.7.2
+isort>=5.10.1
+lark>=1.0.0
 matplotlib>=3.3.4
+moto[s3]>=4.1.1
 nbmake>=1.2.1
 nest-asyncio>=1.5.6
-pytest-benchmark
+nest_asyncio
+numpy>=1.19.5
+openai>=0.27.4
+opencv-python>=4.6.0.66
+pandas>=1.1.5
 pymysql>=0.10.1
-wheel>=0.37.1
+pytest-asyncio
+pytest-benchmark
+pytest-cov>=2.11.1
+pytest-random-order>=1.0.4
+pytest-virtualenv
+pytest-xdist
+pytest>=6.1.2
+pyyaml>=5.1
+ray>=1.13.0
 scriv>=0.16.0
+sqlalchemy-utils>=0.36.6
+sqlalchemy<2.0.0,>=1.4.0
+thefuzz
+timm>=0.6.13
+torch>=1.10.0
+torchvision>=0.11.1
+transformers>=4.27.4
+ultralytics>=8.0.93
+wheel>=0.37.1
```

### Comparing `evadb-0.2.3/setup.py` & `evadb-0.2.3.post0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 from typing import Dict
 
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
-DESCRIPTION = "EVA Video Database System (Think MySQL for videos)."
+DESCRIPTION = "EVA AI-Relational Database System"
 NAME = "evadb"
 AUTHOR = "Georgia Tech Database Group"
-AUTHOR_EMAIL = "georgia.tech.db@gmail.com"
+AUTHOR_EMAIL = "arulraj@gatech.edu"
 URL = "https://github.com/georgia-tech-db/eva"
 
 
 def read(path, encoding="utf-8"):
     path = os.path.join(os.path.dirname(__file__), path)
     with io.open(path, encoding=encoding) as fp:
         return fp.read()
@@ -33,27 +33,29 @@
     exec(version_file.read(), VERSION_DICT)
 
 DOWNLOAD_URL = "https://github.com/georgia-tech-db/eva"
 LICENSE = "Apache License 2.0"
 VERSION = VERSION_DICT["VERSION"]
 
 minimal_requirement = [
-    "numpy>=1.19.5,<=1.23.5",
-    "opencv-python>=4.5.4.60,<4.6.0.66",  # bug in easyocr
+    "numpy>=1.19.5",
     "pandas>=1.1.5",
+    "opencv-python>=4.6.0.66",
     "Pillow>=8.4.0",
     "sqlalchemy>=1.4.0,<2.0.0",  # major changes in 2.0.0
     "sqlalchemy-utils>=0.36.6",
     "lark>=1.0.0",
     "pyyaml>=5.1",
     "importlib-metadata<5.0",
     "ray>=1.13.0",
     "aenum>=2.2.0",
     "diskcache>=5.4.0",
-    "eva-decord==0.6.1",
+    "eva-decord>=0.6.1",
+    "boto3",
+    "nest_asyncio"
 ]
 
 formatter_libs = ["black>=23.1.0", "isort>=5.10.1"]
 
 test_libs = [
     "pytest>=6.1.2",
     "pytest-cov>=2.11.1",
@@ -90,18 +92,17 @@
 
 ### NEEDED FOR AN ALTERNATE DATA SYSTEM OTHER THAN SQLITE
 database_libs = ["pymysql>=0.10.1"]
 
 ### NEEDED FOR A BATTERIES-LOADED EXPERIENCE
 udf_libs = [
     "facenet-pytorch>=2.5.2",  # FACE DETECTION
-    "easyocr>=1.5.0",  # OCR EXTRACTION
     "ipython<8.13.0",  # NOTEBOOKS
     "thefuzz",  # FUZZY STRING MATCHING
-    "ultralytics",  # OBJECT DETECTION (opencv issue due to easy-ocr)
+    "ultralytics>=8.0.93",  # OBJECT DETECTION
     "transformers>=4.27.4",  # HUGGINGFACE
     "openai>=0.27.4",  # CHATGPT
     "timm>=0.6.13",  # HUGGINGFACE VISION TASKS
 ]
 
 ### NEEDED FOR EXPERIMENTAL FEATURES
 experimental_libs = []
@@ -129,28 +130,28 @@
     long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=AUTHOR_EMAIL,
     url=URL,
     download_url=DOWNLOAD_URL,
     license=LICENSE,
     classifiers=[
-        "Intended Audience :: Science/Research",
-        "Topic :: Scientific/Engineering :: Information Analysis",
+        "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
-        "Programming Language :: Python :: 3",
-        "Development Status :: 3 - Alpha",
-        "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        # "Programming Language :: Python :: 3.11",
     ],
     packages=find_packages(exclude=["tests", "tests.*"]),
     # https://python-packaging.readthedocs.io/en/latest/command-line-scripts.html#the-console-scripts-entry-point
     entry_points={
         "console_scripts": [
             "eva_server=eva.eva_server:main",
             "eva_client=eva.eva_cmd_client:main",
         ]
     },
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=INSTALL_REQUIRES,
     extras_require=EXTRA_REQUIRES,
     include_package_data=True,
     package_data={"eva": ["eva.yml", "parser/eva.lark"]},
 )
```

### Comparing `evadb-0.2.3/test/__init__.py` & `evadb-0.2.3.post0/test/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/benchmark_tests/__init__.py` & `evadb-0.2.3.post0/test/benchmark_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/benchmark_tests/conftest.py` & `evadb-0.2.3.post0/test/benchmark_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/benchmark_tests/test_benchmark_pytorch.py` & `evadb-0.2.3.post0/test/benchmark_tests/test_benchmark_pytorch.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/binder/__init__.py` & `evadb-0.2.3.post0/test/binder/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/binder/test_binder_utils.py` & `evadb-0.2.3.post0/test/binder/test_binder_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/binder/test_statement_binder.py` & `evadb-0.2.3.post0/test/binder/test_statement_binder.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/binder/test_statement_binder_context.py` & `evadb-0.2.3.post0/test/binder/test_statement_binder_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/binder/test_statement_binder_python37.py` & `evadb-0.2.3.post0/test/binder/test_statement_binder_python37.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/catalog/__init__.py` & `evadb-0.2.3.post0/test/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/catalog/models/__init__.py` & `evadb-0.2.3.post0/test/catalog/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/catalog/models/test_models.py` & `evadb-0.2.3.post0/test/catalog/models/test_models.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/catalog/services/__init__.py` & `evadb-0.2.3.post0/test/catalog/services/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/catalog/services/test_column_catalog_service.py` & `evadb-0.2.3.post0/test/catalog/services/test_column_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/catalog/services/test_index_catalog_service.py` & `evadb-0.2.3.post0/test/catalog/services/test_index_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/catalog/services/test_table_catalog_service.py` & `evadb-0.2.3.post0/test/catalog/services/test_table_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/catalog/services/test_udf_catalog_service.py` & `evadb-0.2.3.post0/test/catalog/services/test_udf_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/catalog/services/test_udf_cost_catalog_service.py` & `evadb-0.2.3.post0/test/catalog/services/test_udf_cost_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/catalog/services/test_udf_io_catalog_service.py` & `evadb-0.2.3.post0/test/catalog/services/test_udf_io_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/catalog/test_catalog_manager.py` & `evadb-0.2.3.post0/test/catalog/test_catalog_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/catalog/test_column_type.py` & `evadb-0.2.3.post0/test/catalog/test_column_type.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/catalog/test_sqlalchemy.py` & `evadb-0.2.3.post0/test/catalog/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/configuration/__init__.py` & `evadb-0.2.3.post0/test/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/configuration/test_bootstrap_environment.py` & `evadb-0.2.3.post0/test/configuration/test_bootstrap_environment.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/configuration/test_configuration_manager.py` & `evadb-0.2.3.post0/test/configuration/test_configuration_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/executor/__init__.py` & `evadb-0.2.3.post0/test/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/executor/test_abstract_executor.py` & `evadb-0.2.3.post0/test/executor/test_abstract_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/executor/test_create_mat_executor.py` & `evadb-0.2.3.post0/test/executor/test_create_mat_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/executor/test_create_udf_executor.py` & `evadb-0.2.3.post0/test/executor/test_create_udf_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/executor/test_execution_context.py` & `evadb-0.2.3.post0/test/executor/test_execution_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/executor/test_executor_utils.py` & `evadb-0.2.3.post0/test/executor/test_executor_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/executor/test_limit_executor.py` & `evadb-0.2.3.post0/test/executor/test_limit_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/executor/test_load_executor.py` & `evadb-0.2.3.post0/test/executor/test_load_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/executor/test_orderby_executor.py` & `evadb-0.2.3.post0/test/executor/test_orderby_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/executor/test_plan_executor.py` & `evadb-0.2.3.post0/test/executor/test_plan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/executor/test_pp_executor.py` & `evadb-0.2.3.post0/test/executor/test_pp_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/executor/test_sample_executor.py` & `evadb-0.2.3.post0/test/executor/test_sample_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/executor/test_seq_scan_executor.py` & `evadb-0.2.3.post0/test/executor/test_seq_scan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/executor/utils.py` & `evadb-0.2.3.post0/test/executor/utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/expression/__init__.py` & `evadb-0.2.3.post0/test/expression/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/expression/test_abstract_expression.py` & `evadb-0.2.3.post0/test/expression/test_abstract_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/expression/test_aggregation.py` & `evadb-0.2.3.post0/test/expression/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/expression/test_arithmetic.py` & `evadb-0.2.3.post0/test/expression/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/expression/test_comparison.py` & `evadb-0.2.3.post0/test/expression/test_comparison.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/expression/test_expression_tree.py` & `evadb-0.2.3.post0/test/expression/test_expression_tree.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/expression/test_expression_utils.py` & `evadb-0.2.3.post0/test/expression/test_expression_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/expression/test_function_expression.py` & `evadb-0.2.3.post0/test/expression/test_function_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/expression/test_logical.py` & `evadb-0.2.3.post0/test/expression/test_logical.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/integration_tests/__init__.py` & `evadb-0.2.3.post0/test/integration_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/integration_tests/test_array_count.py` & `evadb-0.2.3.post0/test/integration_tests/test_array_count.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/integration_tests/test_chatgpt.py` & `evadb-0.2.3.post0/test/integration_tests/test_chatgpt.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/integration_tests/test_create_index_executor.py` & `evadb-0.2.3.post0/test/integration_tests/test_create_index_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/integration_tests/test_create_table_executor.py` & `evadb-0.2.3.post0/test/integration_tests/test_create_table_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/integration_tests/test_delete_executor.py` & `evadb-0.2.3.post0/test/integration_tests/test_delete_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/integration_tests/test_drop_executor.py` & `evadb-0.2.3.post0/test/integration_tests/test_drop_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/integration_tests/test_error_handling_with_ray.py` & `evadb-0.2.3.post0/test/integration_tests/test_error_handling_with_ray.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,24 +52,22 @@
         shutdown_ray()
 
         # Drop table.
         drop_table_query = "DROP TABLE testRayErrorHandling;"
         execute_query_fetch_all(drop_table_query)
 
     def test_ray_error_populate_to_all_stages(self):
-        create_udf_query = """CREATE UDF IF NOT EXISTS OCRExtractor
-                  INPUT  (frame NDARRAY UINT8(3, ANYDIM, ANYDIM))
-                  OUTPUT (labels NDARRAY STR(10),
-                          bboxes NDARRAY FLOAT32(ANYDIM, 4),
-                          scores NDARRAY FLOAT32(ANYDIM))
-                  TYPE  OCRExtraction
-                  IMPL  'eva/udfs/ocr_extractor.py';
+        udf_name, task = "HFObjectDetector", "image-classification"
+        create_udf_query = f"""CREATE UDF {udf_name}
+            TYPE HuggingFace
+            'task' '{task}'
         """
+
         execute_query_fetch_all(create_udf_query)
 
-        select_query = """SELECT OCRExtractor(data) FROM testRayErrorHandling;"""
+        select_query = """SELECT HFObjectDetector(data) FROM testRayErrorHandling;"""
 
         with self.assertRaises(ExecutorError):
             _ = execute_query_fetch_all(select_query)
 
         time.sleep(3)
         self.assertFalse(is_ray_stage_running())
```

### Comparing `evadb-0.2.3/test/integration_tests/test_explain_executor.py` & `evadb-0.2.3.post0/test/integration_tests/test_explain_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/integration_tests/test_fuzzy_join.py` & `evadb-0.2.3.post0/test/integration_tests/test_fuzzy_join.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/integration_tests/test_huggingface_udfs.py` & `evadb-0.2.3.post0/test/integration_tests/test_huggingface_udfs.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/integration_tests/test_insert_executor.py` & `evadb-0.2.3.post0/test/integration_tests/test_insert_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/integration_tests/test_like.py` & `evadb-0.2.3.post0/test/integration_tests/test_like.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import unittest
+from test.markers import ocr_skip_marker
 from test.util import shutdown_ray
 
 from eva.catalog.catalog_manager import CatalogManager
 from eva.configuration.constants import EVA_ROOT_DIR
 from eva.server.command_handler import execute_query_fetch_all
 
 
@@ -31,14 +32,15 @@
         execute_query_fetch_all(f"LOAD IMAGE '{meme2}' INTO MemeImages;")
 
     def tearDown(self):
         shutdown_ray()
         # clean up
         execute_query_fetch_all("DROP TABLE IF EXISTS MemeImages;")
 
+    @ocr_skip_marker
     def test_like_with_ocr(self):
         create_udf_query = """CREATE UDF IF NOT EXISTS OCRExtractor
                   INPUT  (frame NDARRAY UINT8(3, ANYDIM, ANYDIM))
                   OUTPUT (labels NDARRAY STR(10),
                           bboxes NDARRAY FLOAT32(ANYDIM, 4),
                           scores NDARRAY FLOAT32(ANYDIM))
                   TYPE  OCRExtraction
@@ -47,14 +49,15 @@
         execute_query_fetch_all(create_udf_query)
         select_query = """SELECT X.label, X.x, X.y FROM MemeImages JOIN LATERAL UNNEST(OCRExtractor(data)) AS X(label, x, y) WHERE label LIKE {};""".format(
             r"""'.*SWAG.*'"""
         )
         actual_batch = execute_query_fetch_all(select_query)
         self.assertEqual(len(actual_batch), 1)
 
+    @ocr_skip_marker
     def test_like_fails_on_non_string_col(self):
         create_udf_query = """CREATE UDF IF NOT EXISTS OCRExtractor
                   INPUT  (frame NDARRAY UINT8(3, ANYDIM, ANYDIM))
                   OUTPUT (labels NDARRAY STR(10),
                           bboxes NDARRAY FLOAT32(ANYDIM, 4),
                           scores NDARRAY FLOAT32(ANYDIM))
                   TYPE  OCRExtraction
```

### Comparing `evadb-0.2.3/test/integration_tests/test_load_executor.py` & `evadb-0.2.3.post0/test/integration_tests/test_load_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/integration_tests/test_mat_executor.py` & `evadb-0.2.3.post0/test/integration_tests/test_mat_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/integration_tests/test_open.py` & `evadb-0.2.3.post0/test/integration_tests/test_open.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/integration_tests/test_optimizer_rules.py` & `evadb-0.2.3.post0/test/integration_tests/test_optimizer_rules.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/integration_tests/test_pytorch.py` & `evadb-0.2.3.post0/test/integration_tests/test_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import unittest
-from test.markers import windows_skip_marker
+from test.markers import ocr_skip_marker, windows_skip_marker
 from test.util import file_remove, load_udfs_for_testing, shutdown_ray
 
 import cv2
 import numpy as np
 import pytest
 
 from eva.catalog.catalog_manager import CatalogManager
@@ -122,14 +122,15 @@
         select_query = """SELECT FaceDetector(data) FROM MyVideo
                         WHERE id < 5;"""
         actual_batch = execute_query_fetch_all(select_query)
         self.assertEqual(len(actual_batch), 5)
 
     @pytest.mark.torchtest
     @windows_skip_marker
+    @ocr_skip_marker
     def test_should_run_pytorch_and_ocr(self):
         create_udf_query = """CREATE UDF IF NOT EXISTS OCRExtractor
                   INPUT  (frame NDARRAY UINT8(3, ANYDIM, ANYDIM))
                   OUTPUT (labels NDARRAY STR(10),
                           bboxes NDARRAY FLOAT32(ANYDIM, 4),
                           scores NDARRAY FLOAT32(ANYDIM))
                   TYPE  OCRExtraction
@@ -218,14 +219,15 @@
         actual_batch = execute_query_fetch_all(similarity_query)
 
         similar_data = actual_batch.frames["myvideo.data"][0]
         self.assertTrue(np.array_equal(img, similar_data))
 
     @pytest.mark.torchtest
     @windows_skip_marker
+    @ocr_skip_marker
     def test_should_run_ocr_on_cropped_data(self):
         create_udf_query = """CREATE UDF IF NOT EXISTS OCRExtractor
                   INPUT  (text NDARRAY STR(100))
                   OUTPUT (labels NDARRAY STR(10),
                           bboxes NDARRAY FLOAT32(ANYDIM, 4),
                           scores NDARRAY FLOAT32(ANYDIM))
                   TYPE  OCRExtraction
```

### Comparing `evadb-0.2.3/test/integration_tests/test_rename_executor.py` & `evadb-0.2.3.post0/test/integration_tests/test_rename_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/integration_tests/test_reuse.py` & `evadb-0.2.3.post0/test/integration_tests/test_reuse.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/integration_tests/test_s3_load_executor.py` & `evadb-0.2.3.post0/test/integration_tests/test_s3_load_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/integration_tests/test_select_executor.py` & `evadb-0.2.3.post0/test/integration_tests/test_select_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/integration_tests/test_show_info_executor.py` & `evadb-0.2.3.post0/test/integration_tests/test_show_info_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/integration_tests/test_similarity.py` & `evadb-0.2.3.post0/test/integration_tests/test_similarity.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/integration_tests/test_udf_executor.py` & `evadb-0.2.3.post0/test/integration_tests/test_udf_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/markers.py` & `evadb-0.2.3.post0/test/markers.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,7 +40,12 @@
     reason="Only test for ray execution.",
 )
 
 duplicate_skip_marker = pytest.mark.skipif(
     sys.platform == "linux",
     reason="Test case is duplicate. Disabling to speed up test suite",
 )
+
+ocr_skip_marker = pytest.mark.skipif(
+    sys.platform == "linux",
+    reason="We do not have built-in support for OCR",
+)
```

### Comparing `evadb-0.2.3/test/models/__init__.py` & `evadb-0.2.3.post0/test/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/models/catalog/__init__.py` & `evadb-0.2.3.post0/test/models/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/models/catalog/test_frame_info.py` & `evadb-0.2.3.post0/test/models/catalog/test_frame_info.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/models/storage/__init__.py` & `evadb-0.2.3.post0/test/models/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/models/storage/test_batch.py` & `evadb-0.2.3.post0/test/models/storage/test_batch.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/optimizer/__init__.py` & `evadb-0.2.3.post0/test/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/optimizer/rules/__init__.py` & `evadb-0.2.3.post0/test/optimizer/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/optimizer/rules/test_rules.py` & `evadb-0.2.3.post0/test/optimizer/rules/test_rules.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/optimizer/test_binder.py` & `evadb-0.2.3.post0/test/optimizer/test_binder.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/optimizer/test_cascade_optimizer.py` & `evadb-0.2.3.post0/test/optimizer/test_cascade_optimizer.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/optimizer/test_cost_model.py` & `evadb-0.2.3.post0/test/optimizer/test_cost_model.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/optimizer/test_group.py` & `evadb-0.2.3.post0/test/optimizer/test_group.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/optimizer/test_memo.py` & `evadb-0.2.3.post0/test/optimizer/test_memo.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/optimizer/test_optimizer_context.py` & `evadb-0.2.3.post0/test/optimizer/test_optimizer_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/optimizer/test_optimizer_task.py` & `evadb-0.2.3.post0/test/optimizer/test_optimizer_task.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/optimizer/test_optimizer_utils.py` & `evadb-0.2.3.post0/test/optimizer/test_optimizer_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/optimizer/test_statement_to_opr_convertor.py` & `evadb-0.2.3.post0/test/optimizer/test_statement_to_opr_convertor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/parser/__init__.py` & `evadb-0.2.3.post0/test/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/parser/test_parser.py` & `evadb-0.2.3.post0/test/parser/test_parser.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/parser/test_parser_statements.py` & `evadb-0.2.3.post0/test/parser/test_parser_statements.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/plan_nodes/__init__.py` & `evadb-0.2.3.post0/test/plan_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/plan_nodes/test_plan.py` & `evadb-0.2.3.post0/test/plan_nodes/test_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/readers/__init__.py` & `evadb-0.2.3.post0/test/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/readers/test_csv_reader.py` & `evadb-0.2.3.post0/test/readers/test_csv_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/readers/test_decord_reader.py` & `evadb-0.2.3.post0/test/readers/test_decord_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/server/__init__.py` & `evadb-0.2.3.post0/test/server/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/server/test_command_handler.py` & `evadb-0.2.3.post0/test/server/test_command_handler.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/server/test_db_api.py` & `evadb-0.2.3.post0/test/server/test_db_api.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/server/test_interpreter.py` & `evadb-0.2.3.post0/test/server/test_interpreter.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/server/test_server.py` & `evadb-0.2.3.post0/test/server/test_server.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/storage/__init__.py` & `evadb-0.2.3.post0/test/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/storage/test_sqlite_storage_engine.py` & `evadb-0.2.3.post0/test/storage/test_sqlite_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/storage/test_video_storage.py` & `evadb-0.2.3.post0/test/storage/test_video_storage.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/test_eva_cmd_client.py` & `evadb-0.2.3.post0/test/test_eva_cmd_client.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/test_eva_imports.py` & `evadb-0.2.3.post0/test/test_eva_imports.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/test_eva_server.py` & `evadb-0.2.3.post0/test/test_eva_server.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/udfs/__init__.py` & `evadb-0.2.3.post0/test/udfs/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/udfs/decorators/__init__.py` & `evadb-0.2.3.post0/test/udfs/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/udfs/decorators/io_descriptors/__init__.py` & `evadb-0.2.3.post0/test/udfs/decorators/io_descriptors/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/udfs/decorators/io_descriptors/test_descriptors.py` & `evadb-0.2.3.post0/test/udfs/decorators/io_descriptors/test_descriptors.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/udfs/decorators/test_decorators.py` & `evadb-0.2.3.post0/test/udfs/decorators/test_decorators.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/udfs/ndarray/__init__.py` & `evadb-0.2.3.post0/test/udfs/ndarray/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/udfs/ndarray/test_array_count.py` & `evadb-0.2.3.post0/test/udfs/ndarray/test_array_count.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/udfs/ndarray/test_crop.py` & `evadb-0.2.3.post0/test/udfs/ndarray/test_crop.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/udfs/ndarray/test_open.py` & `evadb-0.2.3.post0/test/udfs/ndarray/test_open.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/udfs/test_abstract_udf.py` & `evadb-0.2.3.post0/test/udfs/test_abstract_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/udfs/test_emotion_detector.py` & `evadb-0.2.3.post0/test/udfs/test_emotion_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/udfs/test_facenet_udf.py` & `evadb-0.2.3.post0/test/udfs/test_facenet_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/udfs/test_fastrcnn_object_detector.py` & `evadb-0.2.3.post0/test/udfs/test_fastrcnn_object_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/udfs/test_yolo_object_detector.py` & `evadb-0.2.3.post0/test/udfs/test_yolo_object_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/util.py` & `evadb-0.2.3.post0/test/util.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/utils/__init__.py` & `evadb-0.2.3.post0/test/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/utils/test_generic_utils.py` & `evadb-0.2.3.post0/test/utils/test_generic_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/utils/test_timer.py` & `evadb-0.2.3.post0/test/utils/test_timer.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3/test/utils/test_xdist.py` & `evadb-0.2.3.post0/test/utils/test_xdist.py`

 * *Files identical despite different names*

