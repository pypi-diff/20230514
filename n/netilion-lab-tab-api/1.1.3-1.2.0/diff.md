# Comparing `tmp/netilion_lab_tab_api-1.1.3.tar.gz` & `tmp/netilion_lab_tab_api-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netilion_lab_tab_api-1.1.3.tar", last modified: Fri Dec 16 14:08:06 2022, max compression
+gzip compressed data, was "netilion_lab_tab_api-1.2.0.tar", last modified: Sat May 13 16:53:38 2023, max compression
```

## Comparing `netilion_lab_tab_api-1.1.3.tar` & `netilion_lab_tab_api-1.2.0.tar`

### file list

```diff
@@ -1,166 +1,167 @@
-drwxrwxrwx   0        0        0        0 2022-12-16 14:08:06.668082 netilion_lab_tab_api-1.1.3/
--rw-rw-rw-   0        0        0     1091 2022-12-16 12:16:18.000000 netilion_lab_tab_api-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     3870 2022-12-16 14:08:06.665078 netilion_lab_tab_api-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1996 2022-12-16 14:00:32.000000 netilion_lab_tab_api-1.1.3/README.md
--rw-rw-rw-   0        0        0      871 2022-12-16 14:07:17.000000 netilion_lab_tab_api-1.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-12-16 14:08:06.669087 netilion_lab_tab_api-1.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-12-16 14:08:06.109095 netilion_lab_tab_api-1.1.3/src/
-drwxrwxrwx   0        0        0        0 2022-12-16 14:08:06.129098 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/
--rw-rw-rw-   0        0        0    11682 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-16 14:08:06.251093 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/
--rw-rw-rw-   0        0        0     1326 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/__init__.py
--rw-rw-rw-   0        0        0    50427 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/add_on_api.py
--rw-rw-rw-   0        0        0    17927 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/app_instance_api.py
--rw-rw-rw-   0        0        0   127658 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/batch_api.py
--rw-rw-rw-   0        0        0    33554 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/batch_status_api.py
--rw-rw-rw-   0        0        0    34476 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/batch_type_api.py
--rw-rw-rw-   0        0        0     9850 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/connected_asset_api.py
--rw-rw-rw-   0        0        0     5023 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/connected_asset_config_trigger_api.py
--rw-rw-rw-   0        0        0     5131 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/connected_asset_status_api.py
--rw-rw-rw-   0        0        0    31128 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/document_standard_api.py
--rw-rw-rw-   0        0        0     5655 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/mail_api.py
--rw-rw-rw-   0        0        0   162639 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/recipe_api.py
--rw-rw-rw-   0        0        0    33938 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/recipe_status_api.py
--rw-rw-rw-   0        0        0    34860 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/recipe_type_api.py
--rw-rw-rw-   0        0        0     9072 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/sim_card_api.py
--rw-rw-rw-   0        0        0   249007 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/system_api.py
--rw-rw-rw-   0        0        0    33934 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/system_status_api.py
--rw-rw-rw-   0        0        0    34856 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/system_type_api.py
--rw-rw-rw-   0        0        0    32675 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/value_objects_api.py
--rw-rw-rw-   0        0        0    25302 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api_client.py
--rw-rw-rw-   0        0        0    12611 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/configuration.py
-drwxrwxrwx   0        0        0        0 2022-12-16 14:08:06.662077 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/
--rw-rw-rw-   0        0        0    10157 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/__init__.py
--rw-rw-rw-   0        0        0     8061 2022-12-16 12:19:51.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/add_on_base.py
--rw-rw-rw-   0        0        0     2969 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/add_on_request.py
--rw-rw-rw-   0        0        0     3582 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/add_on_response.py
--rw-rw-rw-   0        0        0     4222 2022-12-16 12:19:52.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/add_ons_response.py
--rw-rw-rw-   0        0        0     3827 2022-12-16 12:19:52.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/app_instance_base.py
--rw-rw-rw-   0        0        0     3041 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/app_instance_request.py
--rw-rw-rw-   0        0        0     5931 2022-12-16 12:19:52.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/app_instance_response.py
--rw-rw-rw-   0        0        0     4438 2022-12-16 12:19:52.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/app_instances_response.py
--rw-rw-rw-   0        0        0     6656 2022-12-16 12:19:52.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/asset_base.py
--rw-rw-rw-   0        0        0     3323 2022-12-16 12:19:52.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/asset_i_ds.py
--rw-rw-rw-   0        0        0     4367 2022-12-16 12:19:52.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/asset_key_value_objects_data.py
--rw-rw-rw-   0        0        0     5135 2022-12-16 12:19:52.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/asset_key_value_objects_response.py
--rw-rw-rw-   0        0        0     6233 2022-12-16 12:19:52.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/asset_key_values_data.py
--rw-rw-rw-   0        0        0     9408 2022-12-16 12:19:52.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/asset_key_values_response.py
--rw-rw-rw-   0        0        0    10273 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/asset_response.py
--rw-rw-rw-   0        0        0     7949 2022-12-16 12:19:52.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/asset_value.py
--rw-rw-rw-   0        0        0     4058 2022-12-16 12:19:52.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/asset_value_object_request.py
--rw-rw-rw-   0        0        0     4314 2022-12-16 12:19:52.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/asset_value_object_request_data.py
--rw-rw-rw-   0        0        0     9353 2022-12-16 12:19:52.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/asset_value_objects_pagination.py
--rw-rw-rw-   0        0        0     3551 2022-12-16 12:19:52.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/asset_value_objects_request.py
--rw-rw-rw-   0        0        0     9137 2022-12-16 12:19:52.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/asset_values_pagination.py
--rw-rw-rw-   0        0        0     3417 2022-12-16 12:19:52.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/asset_values_response.py
--rw-rw-rw-   0        0        0     4201 2022-12-16 12:19:52.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/assets_response.py
--rw-rw-rw-   0        0        0     6680 2022-12-16 12:19:52.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/batch_base.py
--rw-rw-rw-   0        0        0     6086 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/batch_request.py
--rw-rw-rw-   0        0        0     7391 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/batch_response.py
--rw-rw-rw-   0        0        0     5412 2022-12-16 12:19:52.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/batch_status_base.py
--rw-rw-rw-   0        0        0     3695 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/batch_status_request.py
--rw-rw-rw-   0        0        0     4350 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/batch_status_response.py
--rw-rw-rw-   0        0        0     4193 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/batch_statuses.py
--rw-rw-rw-   0        0        0     4387 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/batch_statuses1.py
--rw-rw-rw-   0        0        0     5370 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/batch_type_base.py
--rw-rw-rw-   0        0        0     4311 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/batch_type_request.py
--rw-rw-rw-   0        0        0     4974 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/batch_type_response.py
--rw-rw-rw-   0        0        0     4091 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/batch_types.py
--rw-rw-rw-   0        0        0     4059 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/batches_response.py
--rw-rw-rw-   0        0        0     5133 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/certificate_renewal_request.py
--rw-rw-rw-   0        0        0     5055 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/certificate_renewal_response.py
--rw-rw-rw-   0        0        0    11422 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/connected_asset_request.py
--rw-rw-rw-   0        0        0     3793 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/connected_asset_request_configuration.py
--rw-rw-rw-   0        0        0     8272 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/connected_asset_request_connection.py
--rw-rw-rw-   0        0        0     4358 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/connected_asset_request_firmware.py
--rw-rw-rw-   0        0        0     4964 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/connected_asset_request_values.py
--rw-rw-rw-   0        0        0     7219 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/connected_asset_response.py
--rw-rw-rw-   0        0        0     4322 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/container_export_request.py
--rw-rw-rw-   0        0        0    18868 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/data_export_response.py
--rw-rw-rw-   0        0        0     3476 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/data_exports_response.py
--rw-rw-rw-   0        0        0     4668 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/document_standard_base.py
--rw-rw-rw-   0        0        0     3474 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/document_standard_i_ds.py
--rw-rw-rw-   0        0        0     3758 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/document_standard_response.py
--rw-rw-rw-   0        0        0     4429 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/document_standards_response.py
--rw-rw-rw-   0        0        0     9848 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/error.py
--rw-rw-rw-   0        0        0     3269 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/error_response.py
--rw-rw-rw-   0        0        0     7350 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/firmware_response.py
--rw-rw-rw-   0        0        0     3427 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/id_pictures_body.py
--rw-rw-rw-   0        0        0     3435 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/id_pictures_body1.py
--rw-rw-rw-   0        0        0     3435 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/id_pictures_body2.py
--rw-rw-rw-   0        0        0     6674 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/instrumentation_base.py
--rw-rw-rw-   0        0        0     3613 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/instrumentation_i_ds.py
--rw-rw-rw-   0        0        0     7103 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/instrumentation_response.py
--rw-rw-rw-   0        0        0     4377 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/instrumentations_response.py
--rw-rw-rw-   0        0        0     3344 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/link.py
--rw-rw-rw-   0        0        0     9552 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/links.py
--rw-rw-rw-   0        0        0     3988 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/links1.py
--rw-rw-rw-   0        0        0     7308 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/links2.py
--rw-rw-rw-   0        0        0     6652 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/links3.py
--rw-rw-rw-   0        0        0     4564 2022-12-16 12:19:53.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/links4.py
--rw-rw-rw-   0        0        0     4419 2022-12-16 12:19:54.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/mail_attachment_request.py
--rw-rw-rw-   0        0        0     7362 2022-12-16 12:19:54.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/mail_request.py
--rw-rw-rw-   0        0        0     3302 2022-12-16 12:19:54.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/nested_id.py
--rw-rw-rw-   0        0        0     4096 2022-12-16 12:19:54.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/nested_id_href.py
--rw-rw-rw-   0        0        0     4837 2022-12-16 12:19:54.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/nested_id_href_name.py
--rw-rw-rw-   0        0        0     5255 2022-12-16 12:19:54.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/nested_id_href_serialnumber.py
--rw-rw-rw-   0        0        0     4881 2022-12-16 12:19:54.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/nested_id_href_tag.py
--rw-rw-rw-   0        0        0     5311 2022-12-16 12:19:54.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/node_base.py
--rw-rw-rw-   0        0        0     3294 2022-12-16 12:19:54.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/node_i_ds.py
--rw-rw-rw-   0        0        0     6063 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/node_response.py
--rw-rw-rw-   0        0        0     3992 2022-12-16 12:19:54.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/nodes_response.py
--rw-rw-rw-   0        0        0     8715 2022-12-16 12:19:54.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/pagination.py
--rw-rw-rw-   0        0        0     4866 2022-12-16 12:19:54.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/picture_link_request.py
--rw-rw-rw-   0        0        0     8175 2022-12-16 12:19:54.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/picture_response.py
--rw-rw-rw-   0        0        0     3427 2022-12-16 12:19:54.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/pictures_id_body.py
--rw-rw-rw-   0        0        0     3435 2022-12-16 12:19:54.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/pictures_id_body1.py
--rw-rw-rw-   0        0        0     3435 2022-12-16 12:19:54.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/pictures_id_body2.py
--rw-rw-rw-   0        0        0     4273 2022-12-16 12:19:54.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/pictures_response.py
--rw-rw-rw-   0        0        0     4469 2022-12-16 12:19:54.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/recipe_base.py
--rw-rw-rw-   0        0        0     4846 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/recipe_request.py
--rw-rw-rw-   0        0        0     6127 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/recipe_response.py
--rw-rw-rw-   0        0        0     5433 2022-12-16 12:19:54.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/recipe_status_base.py
--rw-rw-rw-   0        0        0     3711 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/recipe_status_request.py
--rw-rw-rw-   0        0        0     4370 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/recipe_status_response.py
--rw-rw-rw-   0        0        0     4228 2022-12-16 12:19:54.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/recipe_statuses.py
--rw-rw-rw-   0        0        0     4423 2022-12-16 12:19:54.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/recipe_statuses1.py
--rw-rw-rw-   0        0        0     5391 2022-12-16 12:19:54.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/recipe_type_base.py
--rw-rw-rw-   0        0        0     4331 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/recipe_type_request.py
--rw-rw-rw-   0        0        0     4998 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/recipe_type_response.py
--rw-rw-rw-   0        0        0     4126 2022-12-16 12:19:54.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/recipe_types.py
--rw-rw-rw-   0        0        0     4062 2022-12-16 12:19:54.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/recipes_response.py
--rw-rw-rw-   0        0        0     3321 2022-12-16 12:19:54.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/sim_card.py
--rw-rw-rw-   0        0        0     2960 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/sim_card_request.py
--rw-rw-rw-   0        0        0     3593 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/sim_card_response.py
--rw-rw-rw-   0        0        0     5221 2022-12-16 12:19:54.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/specification_base.py
--rw-rw-rw-   0        0        0     4355 2022-12-16 12:19:54.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/specification_history_response.py
--rw-rw-rw-   0        0        0     3064 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/specification_request.py
--rw-rw-rw-   0        0        0     3903 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/specification_response.py
--rw-rw-rw-   0        0        0     2654 2022-12-16 12:19:55.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/specifications_delete.py
--rw-rw-rw-   0        0        0     3523 2022-12-16 12:19:55.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/specifications_rename.py
--rw-rw-rw-   0        0        0     2894 2022-12-16 12:19:55.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/specifications_request.py
--rw-rw-rw-   0        0        0     2898 2022-12-16 12:19:55.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/specifications_response.py
--rw-rw-rw-   0        0        0     4469 2022-12-16 12:19:55.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/system_base.py
--rw-rw-rw-   0        0        0     6118 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/system_request.py
--rw-rw-rw-   0        0        0     7431 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/system_response.py
--rw-rw-rw-   0        0        0     5433 2022-12-16 12:19:55.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/system_status_base.py
--rw-rw-rw-   0        0        0     3711 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/system_status_request.py
--rw-rw-rw-   0        0        0     4370 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/system_status_response.py
--rw-rw-rw-   0        0        0     4228 2022-12-16 12:19:55.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/system_statuses.py
--rw-rw-rw-   0        0        0     4423 2022-12-16 12:19:55.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/system_statuses1.py
--rw-rw-rw-   0        0        0     5391 2022-12-16 12:19:55.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/system_type_base.py
--rw-rw-rw-   0        0        0     4331 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/system_type_request.py
--rw-rw-rw-   0        0        0     4998 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/system_type_response.py
--rw-rw-rw-   0        0        0     4126 2022-12-16 12:19:55.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/system_types.py
--rw-rw-rw-   0        0        0     4062 2022-12-16 12:19:55.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/systems_response.py
--rw-rw-rw-   0        0        0     9789 2022-12-16 12:19:55.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/threshold_base.py
--rw-rw-rw-   0        0        0     3016 2022-12-16 14:00:17.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/threshold_request.py
--rw-rw-rw-   0        0        0    10800 2022-12-16 12:19:55.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/threshold_response.py
--rw-rw-rw-   0        0        0     4345 2022-12-16 12:19:55.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/thresholds_response.py
--rw-rw-rw-   0        0        0    13202 2022-12-16 12:19:57.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/rest.py
-drwxrwxrwx   0        0        0        0 2022-12-16 14:08:06.178094 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api.egg-info/
--rw-rw-rw-   0        0        0     3870 2022-12-16 14:08:06.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8188 2022-12-16 14:08:06.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-16 14:08:06.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2022-12-16 14:08:06.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2022-12-16 14:08:06.000000 netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-13 16:53:38.719362 netilion_lab_tab_api-1.2.0/
+-rw-rw-rw-   0        0        0     1091 2022-12-16 12:16:18.000000 netilion_lab_tab_api-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3870 2023-05-13 16:53:38.717362 netilion_lab_tab_api-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1996 2023-05-13 16:43:19.000000 netilion_lab_tab_api-1.2.0/README.md
+-rw-rw-rw-   0        0        0      871 2023-05-13 16:50:13.000000 netilion_lab_tab_api-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-13 16:53:38.719362 netilion_lab_tab_api-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-13 16:53:38.267377 netilion_lab_tab_api-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-13 16:53:38.286358 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/
+-rw-rw-rw-   0        0        0    11849 2023-05-13 16:43:19.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-13 16:53:38.380359 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/
+-rw-rw-rw-   0        0        0     1333 2023-05-13 16:42:38.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/__init__.py
+-rw-rw-rw-   0        0        0    50427 2023-05-13 16:42:37.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/add_on_api.py
+-rw-rw-rw-   0        0        0    17927 2023-05-13 16:42:37.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/app_instance_api.py
+-rw-rw-rw-   0        0        0   127658 2023-05-13 16:42:38.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/batch_api.py
+-rw-rw-rw-   0        0        0    33554 2023-05-13 16:42:38.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/batch_status_api.py
+-rw-rw-rw-   0        0        0    34476 2023-05-13 16:42:38.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/batch_type_api.py
+-rw-rw-rw-   0        0        0    17386 2023-05-13 16:42:38.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/connected_asset_api_api.py
+-rw-rw-rw-   0        0        0     5023 2023-05-13 16:42:38.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/connected_asset_config_trigger_api.py
+-rw-rw-rw-   0        0        0     5131 2023-05-13 16:42:38.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/connected_asset_status_api.py
+-rw-rw-rw-   0        0        0    31128 2023-05-13 16:42:38.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/document_standard_api.py
+-rw-rw-rw-   0        0        0     5655 2023-05-13 16:42:38.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/mail_api.py
+-rw-rw-rw-   0        0        0   162639 2023-05-13 16:42:38.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/recipe_api.py
+-rw-rw-rw-   0        0        0    33938 2023-05-13 16:42:38.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/recipe_status_api.py
+-rw-rw-rw-   0        0        0    34860 2023-05-13 16:42:38.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/recipe_type_api.py
+-rw-rw-rw-   0        0        0     9068 2023-05-13 16:42:38.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/sim_card_api.py
+-rw-rw-rw-   0        0        0   249007 2023-05-13 16:42:38.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/system_api.py
+-rw-rw-rw-   0        0        0    33934 2023-05-13 16:42:38.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/system_status_api.py
+-rw-rw-rw-   0        0        0    34856 2023-05-13 16:42:38.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/system_type_api.py
+-rw-rw-rw-   0        0        0    32677 2023-05-13 16:42:38.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/value_objects_api.py
+-rw-rw-rw-   0        0        0    25935 2023-05-13 16:44:55.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api_client.py
+-rw-rw-rw-   0        0        0    12964 2023-05-13 16:44:51.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/configuration.py
+drwxrwxrwx   0        0        0        0 2023-05-13 16:53:38.715361 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/
+-rw-rw-rw-   0        0        0    10236 2023-05-13 16:42:38.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/__init__.py
+-rw-rw-rw-   0        0        0     8081 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/add_on_base.py
+-rw-rw-rw-   0        0        0     2969 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/add_on_request.py
+-rw-rw-rw-   0        0        0     3582 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/add_on_response.py
+-rw-rw-rw-   0        0        0     4222 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/add_ons_response.py
+-rw-rw-rw-   0        0        0     3827 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/app_instance_base.py
+-rw-rw-rw-   0        0        0     3041 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/app_instance_request.py
+-rw-rw-rw-   0        0        0     5931 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/app_instance_response.py
+-rw-rw-rw-   0        0        0     4438 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/app_instances_response.py
+-rw-rw-rw-   0        0        0     6656 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/asset_base.py
+-rw-rw-rw-   0        0        0     3323 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/asset_i_ds.py
+-rw-rw-rw-   0        0        0     5695 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/asset_id_upload_body.py
+-rw-rw-rw-   0        0        0     4367 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/asset_key_value_objects_data.py
+-rw-rw-rw-   0        0        0     5135 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/asset_key_value_objects_response.py
+-rw-rw-rw-   0        0        0     6233 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/asset_key_values_data.py
+-rw-rw-rw-   0        0        0     9408 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/asset_key_values_response.py
+-rw-rw-rw-   0        0        0    10273 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/asset_response.py
+-rw-rw-rw-   0        0        0     7949 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/asset_value.py
+-rw-rw-rw-   0        0        0     4058 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/asset_value_object_request.py
+-rw-rw-rw-   0        0        0     4314 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/asset_value_object_request_data.py
+-rw-rw-rw-   0        0        0     9353 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/asset_value_objects_pagination.py
+-rw-rw-rw-   0        0        0     3551 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/asset_value_objects_request.py
+-rw-rw-rw-   0        0        0     9137 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/asset_values_pagination.py
+-rw-rw-rw-   0        0        0     3417 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/asset_values_response.py
+-rw-rw-rw-   0        0        0     4201 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/assets_response.py
+-rw-rw-rw-   0        0        0     6680 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/batch_base.py
+-rw-rw-rw-   0        0        0     6086 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/batch_request.py
+-rw-rw-rw-   0        0        0     7391 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/batch_response.py
+-rw-rw-rw-   0        0        0     5412 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/batch_status_base.py
+-rw-rw-rw-   0        0        0     3695 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/batch_status_request.py
+-rw-rw-rw-   0        0        0     4350 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/batch_status_response.py
+-rw-rw-rw-   0        0        0     4193 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/batch_statuses.py
+-rw-rw-rw-   0        0        0     4387 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/batch_statuses1.py
+-rw-rw-rw-   0        0        0     5370 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/batch_type_base.py
+-rw-rw-rw-   0        0        0     4311 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/batch_type_request.py
+-rw-rw-rw-   0        0        0     4974 2023-05-13 16:42:34.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/batch_type_response.py
+-rw-rw-rw-   0        0        0     4091 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/batch_types.py
+-rw-rw-rw-   0        0        0     4059 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/batches_response.py
+-rw-rw-rw-   0        0        0     5127 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/certificate_renewal_request.py
+-rw-rw-rw-   0        0        0     5055 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/certificate_renewal_response.py
+-rw-rw-rw-   0        0        0    11422 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/connected_asset_request.py
+-rw-rw-rw-   0        0        0     3793 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/connected_asset_request_configuration.py
+-rw-rw-rw-   0        0        0     8272 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/connected_asset_request_connection.py
+-rw-rw-rw-   0        0        0     4358 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/connected_asset_request_firmware.py
+-rw-rw-rw-   0        0        0     4964 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/connected_asset_request_values.py
+-rw-rw-rw-   0        0        0     7221 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/connected_asset_response.py
+-rw-rw-rw-   0        0        0     4322 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/container_export_request.py
+-rw-rw-rw-   0        0        0    18868 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/data_export_response.py
+-rw-rw-rw-   0        0        0     3476 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/data_exports_response.py
+-rw-rw-rw-   0        0        0     4668 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/document_standard_base.py
+-rw-rw-rw-   0        0        0     3474 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/document_standard_i_ds.py
+-rw-rw-rw-   0        0        0     3758 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/document_standard_response.py
+-rw-rw-rw-   0        0        0     4429 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/document_standards_response.py
+-rw-rw-rw-   0        0        0     9852 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/error.py
+-rw-rw-rw-   0        0        0     3269 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/error_response.py
+-rw-rw-rw-   0        0        0     7350 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/firmware_response.py
+-rw-rw-rw-   0        0        0     3427 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/id_pictures_body.py
+-rw-rw-rw-   0        0        0     3435 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/id_pictures_body1.py
+-rw-rw-rw-   0        0        0     3435 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/id_pictures_body2.py
+-rw-rw-rw-   0        0        0     6674 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/instrumentation_base.py
+-rw-rw-rw-   0        0        0     3613 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/instrumentation_i_ds.py
+-rw-rw-rw-   0        0        0     7103 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/instrumentation_response.py
+-rw-rw-rw-   0        0        0     4377 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/instrumentations_response.py
+-rw-rw-rw-   0        0        0     3344 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/link.py
+-rw-rw-rw-   0        0        0     9552 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/links.py
+-rw-rw-rw-   0        0        0     3988 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/links1.py
+-rw-rw-rw-   0        0        0     7308 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/links2.py
+-rw-rw-rw-   0        0        0     6652 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/links3.py
+-rw-rw-rw-   0        0        0     4564 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/links4.py
+-rw-rw-rw-   0        0        0     4419 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/mail_attachment_request.py
+-rw-rw-rw-   0        0        0     7362 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/mail_request.py
+-rw-rw-rw-   0        0        0     3302 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/nested_id.py
+-rw-rw-rw-   0        0        0     4096 2023-05-13 16:42:35.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/nested_id_href.py
+-rw-rw-rw-   0        0        0     4837 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/nested_id_href_name.py
+-rw-rw-rw-   0        0        0     5255 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/nested_id_href_serialnumber.py
+-rw-rw-rw-   0        0        0     4881 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/nested_id_href_tag.py
+-rw-rw-rw-   0        0        0     5311 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/node_base.py
+-rw-rw-rw-   0        0        0     3294 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/node_i_ds.py
+-rw-rw-rw-   0        0        0     6063 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/node_response.py
+-rw-rw-rw-   0        0        0     3992 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/nodes_response.py
+-rw-rw-rw-   0        0        0     8715 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/pagination.py
+-rw-rw-rw-   0        0        0     4866 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/picture_link_request.py
+-rw-rw-rw-   0        0        0     8175 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/picture_response.py
+-rw-rw-rw-   0        0        0     3427 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/pictures_id_body.py
+-rw-rw-rw-   0        0        0     3435 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/pictures_id_body1.py
+-rw-rw-rw-   0        0        0     3435 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/pictures_id_body2.py
+-rw-rw-rw-   0        0        0     4273 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/pictures_response.py
+-rw-rw-rw-   0        0        0     4469 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/recipe_base.py
+-rw-rw-rw-   0        0        0     4846 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/recipe_request.py
+-rw-rw-rw-   0        0        0     6127 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/recipe_response.py
+-rw-rw-rw-   0        0        0     5433 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/recipe_status_base.py
+-rw-rw-rw-   0        0        0     3711 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/recipe_status_request.py
+-rw-rw-rw-   0        0        0     4370 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/recipe_status_response.py
+-rw-rw-rw-   0        0        0     4228 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/recipe_statuses.py
+-rw-rw-rw-   0        0        0     4423 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/recipe_statuses1.py
+-rw-rw-rw-   0        0        0     5391 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/recipe_type_base.py
+-rw-rw-rw-   0        0        0     4331 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/recipe_type_request.py
+-rw-rw-rw-   0        0        0     4998 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/recipe_type_response.py
+-rw-rw-rw-   0        0        0     4126 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/recipe_types.py
+-rw-rw-rw-   0        0        0     4062 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/recipes_response.py
+-rw-rw-rw-   0        0        0     3321 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/sim_card.py
+-rw-rw-rw-   0        0        0     2960 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/sim_card_request.py
+-rw-rw-rw-   0        0        0     3593 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/sim_card_response.py
+-rw-rw-rw-   0        0        0     5221 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/specification_base.py
+-rw-rw-rw-   0        0        0     4355 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/specification_history_response.py
+-rw-rw-rw-   0        0        0     3064 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/specification_request.py
+-rw-rw-rw-   0        0        0     3903 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/specification_response.py
+-rw-rw-rw-   0        0        0     2654 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/specifications_delete.py
+-rw-rw-rw-   0        0        0     3523 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/specifications_rename.py
+-rw-rw-rw-   0        0        0     2894 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/specifications_request.py
+-rw-rw-rw-   0        0        0     2898 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/specifications_response.py
+-rw-rw-rw-   0        0        0     4469 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/system_base.py
+-rw-rw-rw-   0        0        0     6118 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/system_request.py
+-rw-rw-rw-   0        0        0     7431 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/system_response.py
+-rw-rw-rw-   0        0        0     5433 2023-05-13 16:42:36.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/system_status_base.py
+-rw-rw-rw-   0        0        0     3711 2023-05-13 16:42:37.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/system_status_request.py
+-rw-rw-rw-   0        0        0     4370 2023-05-13 16:42:37.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/system_status_response.py
+-rw-rw-rw-   0        0        0     4228 2023-05-13 16:42:37.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/system_statuses.py
+-rw-rw-rw-   0        0        0     4423 2023-05-13 16:42:37.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/system_statuses1.py
+-rw-rw-rw-   0        0        0     5391 2023-05-13 16:42:37.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/system_type_base.py
+-rw-rw-rw-   0        0        0     4331 2023-05-13 16:42:37.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/system_type_request.py
+-rw-rw-rw-   0        0        0     4998 2023-05-13 16:42:37.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/system_type_response.py
+-rw-rw-rw-   0        0        0     4126 2023-05-13 16:42:37.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/system_types.py
+-rw-rw-rw-   0        0        0     4062 2023-05-13 16:42:37.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/systems_response.py
+-rw-rw-rw-   0        0        0     9789 2023-05-13 16:42:37.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/threshold_base.py
+-rw-rw-rw-   0        0        0     3016 2023-05-13 16:42:37.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/threshold_request.py
+-rw-rw-rw-   0        0        0    10800 2023-05-13 16:42:37.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/threshold_response.py
+-rw-rw-rw-   0        0        0     4345 2023-05-13 16:42:37.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/thresholds_response.py
+-rw-rw-rw-   0        0        0    13202 2023-05-13 16:42:38.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/rest.py
+drwxrwxrwx   0        0        0        0 2023-05-13 16:53:38.330357 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api.egg-info/
+-rw-rw-rw-   0        0        0     3870 2023-05-13 16:53:38.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8248 2023-05-13 16:53:38.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-13 16:53:38.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-13 16:53:38.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-13 16:53:38.000000 netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api.egg-info/top_level.txt
```

### Comparing `netilion_lab_tab_api-1.1.3/LICENSE` & `netilion_lab_tab_api-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/PKG-INFO` & `netilion_lab_tab_api-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netilion_lab_tab_api
-Version: 1.1.3
+Version: 1.2.0
 Summary: Client for accessing Lab part of Netilion cloud
 Author-email: Andrey Dodonov <Andrey.Dodonov@endress.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `netilion_lab_tab_api-1.1.3/README.md` & `netilion_lab_tab_api-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/pyproject.toml` & `netilion_lab_tab_api-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=21.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netilion_lab_tab_api"
-version = "1.1.3"
+version = "1.2.0"
 authors = [
   { name="Andrey Dodonov", email="Andrey.Dodonov@endress.com" },
 ]
 description = "Client for accessing Lab part of Netilion cloud"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.4"
```

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/__init__.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,34 @@
 # coding: utf-8
 
 # flake8: noqa
-
 """
     Netilion API Documentation
 
     Welcome to the Netilion API Documentation, which provides interactive access and documentation to our REST API.  This section contains new endpoints which are still under development. You're welcome to test them but please note that they still can change anytime!   # noqa: E501
 
     OpenAPI spec version: 01.00.00
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
-# import apis into sdk package
-from netilion_lab_tab_api.api.add_on_api import AddOnApi
-from netilion_lab_tab_api.api.app_instance_api import AppInstanceApi
-from netilion_lab_tab_api.api.batch_api import BatchApi
-from netilion_lab_tab_api.api.batch_status_api import BatchStatusApi
-from netilion_lab_tab_api.api.batch_type_api import BatchTypeApi
-from netilion_lab_tab_api.api.connected_asset_api import ConnectedAssetApi
-from netilion_lab_tab_api.api.connected_asset_config_trigger_api import ConnectedAssetConfigTriggerApi
-from netilion_lab_tab_api.api.connected_asset_status_api import ConnectedAssetStatusApi
-from netilion_lab_tab_api.api.document_standard_api import DocumentStandardApi
-from netilion_lab_tab_api.api.mail_api import MailApi
-from netilion_lab_tab_api.api.recipe_api import RecipeApi
-from netilion_lab_tab_api.api.recipe_status_api import RecipeStatusApi
-from netilion_lab_tab_api.api.recipe_type_api import RecipeTypeApi
-from netilion_lab_tab_api.api.sim_card_api import SimCardApi
-from netilion_lab_tab_api.api.system_api import SystemApi
-from netilion_lab_tab_api.api.system_status_api import SystemStatusApi
-from netilion_lab_tab_api.api.system_type_api import SystemTypeApi
-from netilion_lab_tab_api.api.value_objects_api import ValueObjectsApi
-# import ApiClient
-from netilion_lab_tab_api.api_client import ApiClient
-from netilion_lab_tab_api.configuration import Configuration
-from netilion_lab_tab_api.configuration import AuthType
-from netilion_lab_tab_api.configuration import OAuthPasswordGrant
-# import models into sdk package
+# import models into model package
 from netilion_lab_tab_api.models.add_on_base import AddOnBase
 from netilion_lab_tab_api.models.add_on_request import AddOnRequest
 from netilion_lab_tab_api.models.add_on_response import AddOnResponse
 from netilion_lab_tab_api.models.add_ons_response import AddOnsResponse
 from netilion_lab_tab_api.models.app_instance_base import AppInstanceBase
 from netilion_lab_tab_api.models.app_instance_request import AppInstanceRequest
 from netilion_lab_tab_api.models.app_instance_response import AppInstanceResponse
 from netilion_lab_tab_api.models.app_instances_response import AppInstancesResponse
 from netilion_lab_tab_api.models.asset_base import AssetBase
 from netilion_lab_tab_api.models.asset_i_ds import AssetIDs
+from netilion_lab_tab_api.models.asset_id_upload_body import AssetIdUploadBody
 from netilion_lab_tab_api.models.asset_key_value_objects_data import AssetKeyValueObjectsData
 from netilion_lab_tab_api.models.asset_key_value_objects_response import AssetKeyValueObjectsResponse
 from netilion_lab_tab_api.models.asset_key_values_data import AssetKeyValuesData
 from netilion_lab_tab_api.models.asset_key_values_response import AssetKeyValuesResponse
 from netilion_lab_tab_api.models.asset_response import AssetResponse
 from netilion_lab_tab_api.models.asset_value import AssetValue
 from netilion_lab_tab_api.models.asset_value_object_request import AssetValueObjectRequest
```

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/__init__.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # import apis into api package
 from netilion_lab_tab_api.api.add_on_api import AddOnApi
 from netilion_lab_tab_api.api.app_instance_api import AppInstanceApi
 from netilion_lab_tab_api.api.batch_api import BatchApi
 from netilion_lab_tab_api.api.batch_status_api import BatchStatusApi
 from netilion_lab_tab_api.api.batch_type_api import BatchTypeApi
-from netilion_lab_tab_api.api.connected_asset_api import ConnectedAssetApi
+from netilion_lab_tab_api.api.connected_asset_api_api import ConnectedAssetAPIApi
 from netilion_lab_tab_api.api.connected_asset_config_trigger_api import ConnectedAssetConfigTriggerApi
 from netilion_lab_tab_api.api.connected_asset_status_api import ConnectedAssetStatusApi
 from netilion_lab_tab_api.api.document_standard_api import DocumentStandardApi
 from netilion_lab_tab_api.api.mail_api import MailApi
 from netilion_lab_tab_api.api.recipe_api import RecipeApi
 from netilion_lab_tab_api.api.recipe_status_api import RecipeStatusApi
 from netilion_lab_tab_api.api.recipe_type_api import RecipeTypeApi
```

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/add_on_api.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/add_on_api.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/app_instance_api.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/app_instance_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_app_instances(self, **kwargs):  # noqa: E501
         """Get a range of app_instances.  # noqa: E501
 
-        Returns a list of all app instances that are available for the requesting user in scope of the client application linked to the api key in the header. You can apply query parameters in the request to get a filtered list. If the query has no machtes, the response will show an empty array.  # noqa: E501
+        Returns a list of all app instances that are available for the requesting user in scope of the client application linked to the api key in the header. You can apply query parameters in the request to get a filtered list. If the query has no matches, the response will show an empty array.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_app_instances(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int page: Page number to load
@@ -247,15 +247,15 @@
         else:
             (data) = self.get_app_instances_with_http_info(**kwargs)  # noqa: E501
             return data
 
     def get_app_instances_with_http_info(self, **kwargs):  # noqa: E501
         """Get a range of app_instances.  # noqa: E501
 
-        Returns a list of all app instances that are available for the requesting user in scope of the client application linked to the api key in the header. You can apply query parameters in the request to get a filtered list. If the query has no machtes, the response will show an empty array.  # noqa: E501
+        Returns a list of all app instances that are available for the requesting user in scope of the client application linked to the api key in the header. You can apply query parameters in the request to get a filtered list. If the query has no matches, the response will show an empty array.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_app_instances_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int page: Page number to load
```

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/batch_api.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/batch_api.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/batch_status_api.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/batch_status_api.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/batch_type_api.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/batch_type_api.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/connected_asset_api.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/sim_card_api.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,89 +16,89 @@
 
 # python 2 and python 3 compatibility library
 import six
 
 from netilion_lab_tab_api.api_client import ApiClient
 
 
-class ConnectedAssetApi(object):
+class SimCardApi(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def get_connected_asset_information(self, asset_id, **kwargs):  # noqa: E501
-        """Returns information for a connected asset.  # noqa: E501
+    def get_asset_sim_card(self, id, **kwargs):  # noqa: E501
+        """Get sim card of an asset  # noqa: E501
 
-        Returns information for a connected asset, containing information like server time, scheduled firmware updates, scheduled certificate updates, etc.  # noqa: E501
+        Returns sim card information of an asset  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_connected_asset_information(asset_id, async_req=True)
+        >>> thread = api.get_asset_sim_card(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param int asset_id: Id of the connected asset (required)
-        :return: ConnectedAssetResponse
+        :param int id: Id of the asset to fetch the sim card for (required)
+        :return: SimCardResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.get_connected_asset_information_with_http_info(asset_id, **kwargs)  # noqa: E501
+            return self.get_asset_sim_card_with_http_info(id, **kwargs)  # noqa: E501
         else:
-            (data) = self.get_connected_asset_information_with_http_info(asset_id, **kwargs)  # noqa: E501
+            (data) = self.get_asset_sim_card_with_http_info(id, **kwargs)  # noqa: E501
             return data
 
-    def get_connected_asset_information_with_http_info(self, asset_id, **kwargs):  # noqa: E501
-        """Returns information for a connected asset.  # noqa: E501
+    def get_asset_sim_card_with_http_info(self, id, **kwargs):  # noqa: E501
+        """Get sim card of an asset  # noqa: E501
 
-        Returns information for a connected asset, containing information like server time, scheduled firmware updates, scheduled certificate updates, etc.  # noqa: E501
+        Returns sim card information of an asset  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_connected_asset_information_with_http_info(asset_id, async_req=True)
+        >>> thread = api.get_asset_sim_card_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param int asset_id: Id of the connected asset (required)
-        :return: ConnectedAssetResponse
+        :param int id: Id of the asset to fetch the sim card for (required)
+        :return: SimCardResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['asset_id']  # noqa: E501
+        all_params = ['id']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_connected_asset_information" % key
+                    " to method get_asset_sim_card" % key
                 )
             params[key] = val
         del params['kwargs']
-        # verify the required parameter 'asset_id' is set
-        if ('asset_id' not in params or
-                params['asset_id'] is None):
-            raise ValueError("Missing the required parameter `asset_id` when calling `get_connected_asset_information`")  # noqa: E501
+        # verify the required parameter 'id' is set
+        if ('id' not in params or
+                params['id'] is None):
+            raise ValueError("Missing the required parameter `id` when calling `get_asset_sim_card`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'asset_id' in params:
-            path_params['asset_id'] = params['asset_id']  # noqa: E501
+        if 'id' in params:
+            path_params['id'] = params['id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
@@ -108,98 +108,98 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['API-Key', 'Authentication']  # noqa: E501
 
         return self.api_client.call_api(
-            '/connected_assets/{asset_id}', 'GET',
+            '/assets/{id}/sim_card', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='ConnectedAssetResponse',  # noqa: E501
+            response_type='SimCardResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def update_connected_asset_information(self, body, asset_id, **kwargs):  # noqa: E501
-        """Updates the information of a connected asset.  # noqa: E501
+    def update_asset_sim_card(self, body, id, **kwargs):  # noqa: E501
+        """Update sim card  # noqa: E501
 
-        Updates the information of a connected asset and processes all measured values collected by a connected asset.  # noqa: E501
+        Update sim card informations of an assets  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.update_connected_asset_information(body, asset_id, async_req=True)
+        >>> thread = api.update_asset_sim_card(body, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param ConnectedAssetRequest body: New asset values (required)
-        :param int asset_id: Id of the connected asset (required)
+        :param SimCardRequest body: Update accessible parameters of a assets sim card. (required)
+        :param int id: Id of the asset to update the sim card for (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.update_connected_asset_information_with_http_info(body, asset_id, **kwargs)  # noqa: E501
+            return self.update_asset_sim_card_with_http_info(body, id, **kwargs)  # noqa: E501
         else:
-            (data) = self.update_connected_asset_information_with_http_info(body, asset_id, **kwargs)  # noqa: E501
+            (data) = self.update_asset_sim_card_with_http_info(body, id, **kwargs)  # noqa: E501
             return data
 
-    def update_connected_asset_information_with_http_info(self, body, asset_id, **kwargs):  # noqa: E501
-        """Updates the information of a connected asset.  # noqa: E501
+    def update_asset_sim_card_with_http_info(self, body, id, **kwargs):  # noqa: E501
+        """Update sim card  # noqa: E501
 
-        Updates the information of a connected asset and processes all measured values collected by a connected asset.  # noqa: E501
+        Update sim card informations of an assets  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.update_connected_asset_information_with_http_info(body, asset_id, async_req=True)
+        >>> thread = api.update_asset_sim_card_with_http_info(body, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param ConnectedAssetRequest body: New asset values (required)
-        :param int asset_id: Id of the connected asset (required)
+        :param SimCardRequest body: Update accessible parameters of a assets sim card. (required)
+        :param int id: Id of the asset to update the sim card for (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['body', 'asset_id']  # noqa: E501
+        all_params = ['body', 'id']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method update_connected_asset_information" % key
+                    " to method update_asset_sim_card" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'body' is set
         if ('body' not in params or
                 params['body'] is None):
-            raise ValueError("Missing the required parameter `body` when calling `update_connected_asset_information`")  # noqa: E501
-        # verify the required parameter 'asset_id' is set
-        if ('asset_id' not in params or
-                params['asset_id'] is None):
-            raise ValueError("Missing the required parameter `asset_id` when calling `update_connected_asset_information`")  # noqa: E501
+            raise ValueError("Missing the required parameter `body` when calling `update_asset_sim_card`")  # noqa: E501
+        # verify the required parameter 'id' is set
+        if ('id' not in params or
+                params['id'] is None):
+            raise ValueError("Missing the required parameter `id` when calling `update_asset_sim_card`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'asset_id' in params:
-            path_params['asset_id'] = params['asset_id']  # noqa: E501
+        if 'id' in params:
+            path_params['id'] = params['id']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
@@ -215,15 +215,15 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['API-Key', 'Authentication']  # noqa: E501
 
         return self.api_client.call_api(
-            '/connected_assets/{asset_id}', 'POST',
+            '/assets/{id}/sim_card', 'PATCH',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type=None,  # noqa: E501
```

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/connected_asset_config_trigger_api.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/connected_asset_config_trigger_api.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/connected_asset_status_api.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/connected_asset_status_api.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/document_standard_api.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/document_standard_api.py`

 * *Files identical despite different names*

```diff
@@ -566,15 +566,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def replace_document_standards_of_document_category(self, body, category_id, **kwargs):  # noqa: E501
         """Replace document standards of a category  # noqa: E501
 
-        Replaces all documents standards belonging to a category. You can send a list of resoucres that will replace all previous values.  # noqa: E501
+        Replaces all documents standards belonging to a category. You can send a list of resources that will replace all previous values.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.replace_document_standards_of_document_category(body, category_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param DocumentStandardIDs body: Resources that shall be replaced (required)
@@ -589,15 +589,15 @@
         else:
             (data) = self.replace_document_standards_of_document_category_with_http_info(body, category_id, **kwargs)  # noqa: E501
             return data
 
     def replace_document_standards_of_document_category_with_http_info(self, body, category_id, **kwargs):  # noqa: E501
         """Replace document standards of a category  # noqa: E501
 
-        Replaces all documents standards belonging to a category. You can send a list of resoucres that will replace all previous values.  # noqa: E501
+        Replaces all documents standards belonging to a category. You can send a list of resources that will replace all previous values.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.replace_document_standards_of_document_category_with_http_info(body, category_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param DocumentStandardIDs body: Resources that shall be replaced (required)
```

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/mail_api.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/mail_api.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/recipe_api.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/recipe_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,15 +344,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_recipe_threshold(self, body, recipe_id, **kwargs):  # noqa: E501
         """Create an recipe threshold  # noqa: E501
 
-        Create a new recipe threshold. This action requires ```can_udpate``` permission on the recipe.  # noqa: E501
+        Create a new recipe threshold. This action requires ```can_update``` permission on the recipe.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.create_recipe_threshold(body, recipe_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param ThresholdRequest body: Object body that will be created. (required)
@@ -367,15 +367,15 @@
         else:
             (data) = self.create_recipe_threshold_with_http_info(body, recipe_id, **kwargs)  # noqa: E501
             return data
 
     def create_recipe_threshold_with_http_info(self, body, recipe_id, **kwargs):  # noqa: E501
         """Create an recipe threshold  # noqa: E501
 
-        Create a new recipe threshold. This action requires ```can_udpate``` permission on the recipe.  # noqa: E501
+        Create a new recipe threshold. This action requires ```can_update``` permission on the recipe.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.create_recipe_threshold_with_http_info(body, recipe_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param ThresholdRequest body: Object body that will be created. (required)
```

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/recipe_status_api.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/recipe_status_api.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/recipe_type_api.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/recipe_type_api.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/system_api.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/system_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -558,15 +558,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_system_container(self, body, id, **kwargs):  # noqa: E501
         """Create an export for a standard container  # noqa: E501
 
-        Creates a data export for system container, currenty only the VDI 2770 standard is supported  # noqa: E501
+        Creates a data export for system container, currently only the VDI 2770 standard is supported  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.create_system_container(body, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param ContainerExportRequest body: Container that should be created. (required)
@@ -581,15 +581,15 @@
         else:
             (data) = self.create_system_container_with_http_info(body, id, **kwargs)  # noqa: E501
             return data
 
     def create_system_container_with_http_info(self, body, id, **kwargs):  # noqa: E501
         """Create an export for a standard container  # noqa: E501
 
-        Creates a data export for system container, currenty only the VDI 2770 standard is supported  # noqa: E501
+        Creates a data export for system container, currently only the VDI 2770 standard is supported  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.create_system_container_with_http_info(body, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param ContainerExportRequest body: Container that should be created. (required)
@@ -665,15 +665,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_system_threshold(self, body, system_id, **kwargs):  # noqa: E501
         """Create an system threshold  # noqa: E501
 
-        Create a new system threshold. This action requires ```can_udpate``` permission on the system.  # noqa: E501
+        Create a new system threshold. This action requires ```can_update``` permission on the system.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.create_system_threshold(body, system_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param ThresholdRequest body: Object body that will be created. (required)
@@ -688,15 +688,15 @@
         else:
             (data) = self.create_system_threshold_with_http_info(body, system_id, **kwargs)  # noqa: E501
             return data
 
     def create_system_threshold_with_http_info(self, body, system_id, **kwargs):  # noqa: E501
         """Create an system threshold  # noqa: E501
 
-        Create a new system threshold. This action requires ```can_udpate``` permission on the system.  # noqa: E501
+        Create a new system threshold. This action requires ```can_update``` permission on the system.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.create_system_threshold_with_http_info(body, system_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param ThresholdRequest body: Object body that will be created. (required)
@@ -3445,15 +3445,15 @@
         :param str type_id: One or multiple ids (comma list). Expected id format is integer
         :param str tenant_id: One or multiple ids (comma list). Expected id format is integer
         :param str specifications_key: Filter accepts `*` as wildcard (if used as single specifications filter), supports comma list of keys in connection with specifications_value filter
         :param str specifications_value: Filter accepts `*` as wildcard, supports comma list of values in connection with specifications_key filter. Does not work for vectors
         :param str parent_id: One or multiple ids (comma list). \"null\" to retrieve all objects without parent, \"!null\" for all objects with parent.
         :param str recipe_id: One or multiple ids (comma list). Expected id format is integer
         :param str node_id: One or multiple ids (comma list). Filter acccepts \"null\" for all objects with no nodes assigned or \"!null\" for any assigned node
-        :param str asset_id: One or multiple ids (comma list). Filter acccepts \"null\" for all objects with no assets assigned or \"!null\" for any assigned asset
+        :param str asset_id: One or multiple ids (comma list). Filter accepts \"null\" for all objects with no assets assigned or \"!null\" for any assigned asset
         :param str instrumentation_id: One or multiple ids (comma list). Filter accepts \"null\" for all objects with no instrumentations assigned or \"!null\" for any assigned instrumentation
         :param str permission: Filter by permission of current user. Accepts `can_permit`, `can_delete`, `can_update`, `can_read` (default)
         :param str order_by: Order result by attribute value, accepts `id`, `name`, `created_at` or `updated_at`. Add `-` as a prefix for descending order. Default value is `id`
         :return: SystemsResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
@@ -3482,15 +3482,15 @@
         :param str type_id: One or multiple ids (comma list). Expected id format is integer
         :param str tenant_id: One or multiple ids (comma list). Expected id format is integer
         :param str specifications_key: Filter accepts `*` as wildcard (if used as single specifications filter), supports comma list of keys in connection with specifications_value filter
         :param str specifications_value: Filter accepts `*` as wildcard, supports comma list of values in connection with specifications_key filter. Does not work for vectors
         :param str parent_id: One or multiple ids (comma list). \"null\" to retrieve all objects without parent, \"!null\" for all objects with parent.
         :param str recipe_id: One or multiple ids (comma list). Expected id format is integer
         :param str node_id: One or multiple ids (comma list). Filter acccepts \"null\" for all objects with no nodes assigned or \"!null\" for any assigned node
-        :param str asset_id: One or multiple ids (comma list). Filter acccepts \"null\" for all objects with no assets assigned or \"!null\" for any assigned asset
+        :param str asset_id: One or multiple ids (comma list). Filter accepts \"null\" for all objects with no assets assigned or \"!null\" for any assigned asset
         :param str instrumentation_id: One or multiple ids (comma list). Filter accepts \"null\" for all objects with no instrumentations assigned or \"!null\" for any assigned instrumentation
         :param str permission: Filter by permission of current user. Accepts `can_permit`, `can_delete`, `can_update`, `can_read` (default)
         :param str order_by: Order result by attribute value, accepts `id`, `name`, `created_at` or `updated_at`. Add `-` as a prefix for descending order. Default value is `id`
         :return: SystemsResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
```

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/system_status_api.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/system_status_api.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/system_type_api.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/system_type_api.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/api/value_objects_api.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/api/value_objects_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def create_asset_value_objects(self, body, asset_id, **kwargs):  # noqa: E501
         """Create asset value objects  # noqa: E501
 
-        Store value objects measured by an asset. For performance reasons, this endpoint behaves somewhat differently than normal endpoints:  * The data passed to this endpoint is processed asynchronously. * This endpoint always returns an empty response with status 204 No Content. * The data will be validated during processing. Invalid data will be dropped silently. * The request size is limited to 500kb, requests larger then 500kb will get an \"413 Payload Too Large\" error.  Data validations and manipultation:    * Keys can only consist of the charaters [a-z A-Z 0-9 . - _ ].   * Keys will be converted to lower case strings.   * Keys must be between 1 and 128 characters long.   * The timestamp is not mandatory and will be set to the time the value was transmitted to the server (This only works if the value objects get transfered one at a time, if you send multiple value objects without timestamp at once, all value objects will get the same timestamp and there for only the last one will be stored)  Difference to path /assets/{asset_id}/values is that the values given here are json objects and not numeric values, the json objects can have any structure.  # noqa: E501
+        Store value objects measured by an asset. For performance reasons, this endpoint behaves somewhat differently than normal endpoints:  * The data passed to this endpoint is processed asynchronously. * This endpoint always returns an empty response with status 204 No Content. * The data will be validated during processing. Invalid data will be dropped silently. * The request size is limited to 500kb, requests larger then 500kb will get an \"413 Payload Too Large\" error.  Data validations and manipulation:    * Keys can only consist of the characters [a-z A-Z 0-9 . - _ ].   * Keys will be converted to lower case strings.   * Keys must be between 1 and 128 characters long.   * The timestamp is not mandatory and will be set to the time the value was transmitted to the server (This only works if the value objects get transferred one at a time, if you send multiple value objects without timestamp at once, all value objects will get the same timestamp and there for only the last one will be stored)  Difference to path /assets/{asset_id}/values is that the values given here are json objects and not numeric values, the json objects can have any structure.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.create_asset_value_objects(body, asset_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param AssetValueObjectsRequest body: Values to store to an asset. (required)
@@ -54,15 +54,15 @@
         else:
             (data) = self.create_asset_value_objects_with_http_info(body, asset_id, **kwargs)  # noqa: E501
             return data
 
     def create_asset_value_objects_with_http_info(self, body, asset_id, **kwargs):  # noqa: E501
         """Create asset value objects  # noqa: E501
 
-        Store value objects measured by an asset. For performance reasons, this endpoint behaves somewhat differently than normal endpoints:  * The data passed to this endpoint is processed asynchronously. * This endpoint always returns an empty response with status 204 No Content. * The data will be validated during processing. Invalid data will be dropped silently. * The request size is limited to 500kb, requests larger then 500kb will get an \"413 Payload Too Large\" error.  Data validations and manipultation:    * Keys can only consist of the charaters [a-z A-Z 0-9 . - _ ].   * Keys will be converted to lower case strings.   * Keys must be between 1 and 128 characters long.   * The timestamp is not mandatory and will be set to the time the value was transmitted to the server (This only works if the value objects get transfered one at a time, if you send multiple value objects without timestamp at once, all value objects will get the same timestamp and there for only the last one will be stored)  Difference to path /assets/{asset_id}/values is that the values given here are json objects and not numeric values, the json objects can have any structure.  # noqa: E501
+        Store value objects measured by an asset. For performance reasons, this endpoint behaves somewhat differently than normal endpoints:  * The data passed to this endpoint is processed asynchronously. * This endpoint always returns an empty response with status 204 No Content. * The data will be validated during processing. Invalid data will be dropped silently. * The request size is limited to 500kb, requests larger then 500kb will get an \"413 Payload Too Large\" error.  Data validations and manipulation:    * Keys can only consist of the characters [a-z A-Z 0-9 . - _ ].   * Keys will be converted to lower case strings.   * Keys must be between 1 and 128 characters long.   * The timestamp is not mandatory and will be set to the time the value was transmitted to the server (This only works if the value objects get transferred one at a time, if you send multiple value objects without timestamp at once, all value objects will get the same timestamp and there for only the last one will be stored)  Difference to path /assets/{asset_id}/values is that the values given here are json objects and not numeric values, the json objects can have any structure.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.create_asset_value_objects_with_http_info(body, asset_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param AssetValueObjectsRequest body: Values to store to an asset. (required)
```

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/configuration.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/configuration.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,353 +1,353 @@
-# coding: utf-8
-
-"""
-    Netilion API Documentation
-
-    Welcome to the Netilion API Documentation, which provides interactive access and documentation to our REST API.  This section contains new endpoints which are still under development. You're welcome to test them but please note that they still can change anytime!   # noqa: E501
-
-    OpenAPI spec version: 01.00.00
-    
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
-"""
-
-from __future__ import absolute_import
-
-import copy
-import logging
-import multiprocessing
-import sys
-import time
-import urllib3
-
-import six
-from six.moves import http_client as httplib
-from enum import Enum
-
-from oauthlib.oauth2 import LegacyApplicationClient
-from requests_oauthlib import OAuth2Session
-
-
-class TypeWithDefault(type):
-    def __init__(cls, name, bases, dct):
-        super(TypeWithDefault, cls).__init__(name, bases, dct)
-        cls._default = None
-
-    def __call__(cls):
-        if cls._default is None:
-            cls._default = type.__call__(cls)
-        return copy.copy(cls._default)
-
-    def set_default(cls, default):
-        cls._default = copy.copy(default)
-
-class AuthType(Enum):
-    BASIC = 1
-    OAUTH_PASSWORD_GRANT = 2
-    CUSTOM = 99
-
-class OAuthPasswordGrant():
-    """NOTE: You can inherit from this class in case this implementation 
-    of OAuth 2.0 password grant type does not work for you.
-    Alternatively you can use AuthType.CUSTOM to have full control over auth headers. 
-    """
-    def __init__(self, username, password, api_key, api_secret, oauth_token_url, prefix = 'Bearer '):
-        # necessary parameters
-        self._username = username
-        self._password = password
-        self._api_key = api_key
-        self._api_secret = api_secret
-        self._oauth_token_url = oauth_token_url
-
-        # optional parameters
-        self._prefix = prefix
-
-        # internal variables
-        self._token = None
-        self._oauth = OAuth2Session(client=LegacyApplicationClient(client_id=self._api_key))
-
-    def get_token(self):
-        """Gets HTTP oauth 2.0 password grant type authentication header (string).
-
-        :return: The token for oauth 2.0 grant type HTTP authentication.
-        """
-        if not self._token:
-            self._token = self._fetch_token()
-        else: 
-            token_expiry = self._token["created_at"] + self._token["expires_in"]
-            token_expired = token_expiry <= time.time()
-            if token_expired:
-                self._token = self._refresh_token()
-        token = self._prefix + self._token["access_token"]
-        return token
-
-    def _fetch_token(self):
-        headers = {
-            "API-Key": self._api_key,
-            "Content-Type": "application/x-www-form-urlencoded",
-        }
-        token =  self._oauth.fetch_token(token_url=self._oauth_token_url,
-                                       username=self._username, password=self._password, client_id=self._api_key,
-                                       client_secret=self._api_secret, include_client_id=True, headers=headers)
-        return token
-
-    def _refresh_token(self, **kwargs):
-        kwargs["client_id"] = self._api_key
-        kwargs["client_secret"] = self._api_secret
-        return self._oauth.refresh_token(self._oauth_token_url, **kwargs)
-
-
-class Configuration(six.with_metaclass(TypeWithDefault, object)):
-    """NOTE: This class is auto generated by the swagger code generator program.
-
-    Ref: https://github.com/swagger-api/swagger-codegen
-    Do not edit the class manually.
-    """
-
-    def __init__(self):
-        """Constructor"""
-        # Default Base url
-        self.host = "/v1"
-        # Temp file folder for downloading files
-        self.temp_folder_path = None
-
-        # Authentication Settings
-        # Select auth type
-        self.auth_type = AuthType.BASIC
-        ######################### 
-        # BASIC
-        # Do not encapsulate basic in a class to stay backwards-compatible
-        #########################
-        # dict to store API key(s)
-        self.api_key = {}
-        # dict to store API prefix (e.g. Bearer)
-        self.api_key_prefix = {}
-        # function to refresh API key if expired
-        self.refresh_api_key_hook = None
-        # Username for HTTP basic authentication
-        self.username = ""
-        # Password for HTTP basic authentication
-        self.password = ""
-        ######################### 
-        # OAuth 2.0 Password Grant 
-        # https://oauth.net/2/grant-types/password/
-        #########################
-        self.oauth_password_grant: OAuthPasswordGrant = None
-        ######################### 
-        # Custom hook to get Auth dictionary header
-        #########################
-        self.get_auth_settings_hook = None
-        # Logging Settings
-        self.logger = {}
-        self.logger["package_logger"] = logging.getLogger("netilion_lab_tab_api")
-        self.logger["urllib3_logger"] = logging.getLogger("urllib3")
-        # Log format
-        self.logger_format = '%(asctime)s %(levelname)s %(message)s'
-        # Log stream handler
-        self.logger_stream_handler = None
-        # Log file handler
-        self.logger_file_handler = None
-        # Debug file location
-        self.logger_file = None
-        # Debug switch
-        self.debug = False
-
-        # SSL/TLS verification
-        # Set this to false to skip verifying SSL certificate when calling API
-        # from https server.
-        self.verify_ssl = True
-        # Set this to customize the certificate file to verify the peer.
-        self.ssl_ca_cert = None
-        # client certificate file
-        self.cert_file = None
-        # client key file
-        self.key_file = None
-        # Set this to True/False to enable/disable SSL hostname verification.
-        self.assert_hostname = None
-
-        # urllib3 connection pool's maximum number of connections saved
-        # per pool. urllib3 uses 1 connection as default value, but this is
-        # not the best value when you are making a lot of possibly parallel
-        # requests to the same host, which is often the case here.
-        # cpu_count * 5 is used as default value to increase performance.
-        self.connection_pool_maxsize = multiprocessing.cpu_count() * 5
-
-        # Proxy URL
-        self.proxy = None
-        # Safe chars for path_param
-        self.safe_chars_for_path_param = ''
-
-    @property
-    def logger_file(self):
-        """The logger file.
-
-        If the logger_file is None, then add stream handler and remove file
-        handler. Otherwise, add file handler and remove stream handler.
-
-        :param value: The logger_file path.
-        :type: str
-        """
-        return self.__logger_file
-
-    @logger_file.setter
-    def logger_file(self, value):
-        """The logger file.
-
-        If the logger_file is None, then add stream handler and remove file
-        handler. Otherwise, add file handler and remove stream handler.
-
-        :param value: The logger_file path.
-        :type: str
-        """
-        self.__logger_file = value
-        if self.__logger_file:
-            # If set logging file,
-            # then add file handler and remove stream handler.
-            self.logger_file_handler = logging.FileHandler(self.__logger_file)
-            self.logger_file_handler.setFormatter(self.logger_formatter)
-            for _, logger in six.iteritems(self.logger):
-                logger.addHandler(self.logger_file_handler)
-                if self.logger_stream_handler:
-                    logger.removeHandler(self.logger_stream_handler)
-        else:
-            # If not set logging file,
-            # then add stream handler and remove file handler.
-            self.logger_stream_handler = logging.StreamHandler()
-            self.logger_stream_handler.setFormatter(self.logger_formatter)
-            for _, logger in six.iteritems(self.logger):
-                logger.addHandler(self.logger_stream_handler)
-                if self.logger_file_handler:
-                    logger.removeHandler(self.logger_file_handler)
-
-    @property
-    def debug(self):
-        """Debug status
-
-        :param value: The debug status, True or False.
-        :type: bool
-        """
-        return self.__debug
-
-    @debug.setter
-    def debug(self, value):
-        """Debug status
-
-        :param value: The debug status, True or False.
-        :type: bool
-        """
-        self.__debug = value
-        if self.__debug:
-            # if debug status is True, turn on debug logging
-            for _, logger in six.iteritems(self.logger):
-                logger.setLevel(logging.DEBUG)
-            # turn on httplib debug
-            httplib.HTTPConnection.debuglevel = 1
-        else:
-            # if debug status is False, turn off debug logging,
-            # setting log level to default `logging.WARNING`
-            for _, logger in six.iteritems(self.logger):
-                logger.setLevel(logging.WARNING)
-            # turn off httplib debug
-            httplib.HTTPConnection.debuglevel = 0
-
-    @property
-    def logger_format(self):
-        """The logger format.
-
-        The logger_formatter will be updated when sets logger_format.
-
-        :param value: The format string.
-        :type: str
-        """
-        return self.__logger_format
-
-    @logger_format.setter
-    def logger_format(self, value):
-        """The logger format.
-
-        The logger_formatter will be updated when sets logger_format.
-
-        :param value: The format string.
-        :type: str
-        """
-        self.__logger_format = value
-        self.logger_formatter = logging.Formatter(self.__logger_format)
-
-    def get_api_key_with_prefix(self, identifier):
-        """Gets API key (with prefix if set).
-
-        :param identifier: The identifier of apiKey.
-        :return: The token for api key authentication.
-        """
-        if self.refresh_api_key_hook:
-            self.refresh_api_key_hook(self)
-
-        key = self.api_key.get(identifier)
-        if key:
-            prefix = self.api_key_prefix.get(identifier)
-            if prefix:
-                return "%s %s" % (prefix, key)
-            else:
-                return key
-
-    def get_basic_auth_token(self):
-        """Gets HTTP basic authentication header (string).
-
-        :return: The token for basic HTTP authentication.
-        """
-        return urllib3.util.make_headers(
-            basic_auth=self.username + ':' + self.password
-        ).get('authorization')
-
-    def auth_settings(self):
-        """Gets Auth Settings dict for api client.
-
-        :return: The Auth Settings information dict.
-        """
-        if self.auth_type == AuthType.BASIC:
-            return {
-                'API-Key':
-                    {
-                        'type': 'api_key',
-                        'in': 'header',
-                        'key': 'API-Key',
-                        'value': self.get_api_key_with_prefix('API-Key')
-                    },
-                'Authentication':
-                    {
-                        'type': 'basic',
-                        'in': 'header',
-                        'key': 'Authorization',
-                        'value': self.get_basic_auth_token()
-                    },
-            }
-        elif self.auth_type == AuthType.OAUTH_PASSWORD_GRANT:
-            if not self.oauth_password_grant:
-                raise RuntimeError('Oauth grant type credentials need to be provided, please initialize oauth_password_grant.')
-            return {
-                'Authentication':
-                {
-                    'type': 'oauth_password_grant',
-                    'in': 'header',
-                    'key': 'Authorization',
-                    'value': self.oauth_password_grant.get_token()
-                },
-            }
-        elif self.auth_type == AuthType.CUSTOM:
-            if not self.get_auth_settings_hook:
-                raise RuntimeError('Please provide a get_auth_settings_hook returning authentication headers, see basic implementation here for an example.')
-            return self.get_auth_settings_hook(self)
-        else:
-            msg = "Auth type {} is not supported".format(self.auth_type)
-            raise ValueError(msg)
-
-    def to_debug_report(self):
-        """Gets the essential information for debugging.
-
-        :return: The report for debugging.
-        """
-        return "Python SDK Debug Report:\n"\
-               "OS: {env}\n"\
-               "Python Version: {pyversion}\n"\
-               "Version of the API: 01.00.00\n"\
-               "SDK Package Version: 0.0.1".\
-               format(env=sys.platform, pyversion=sys.version)
+# coding: utf-8
+
+"""
+    Netilion API Documentation
+
+    Welcome to the Netilion API Documentation, which provides interactive access and documentation to our REST API.  This section contains new endpoints which are still under development. You're welcome to test them but please note that they still can change anytime!   # noqa: E501
+
+    OpenAPI spec version: 01.00.00
+    
+    Generated by: https://github.com/swagger-api/swagger-codegen.git
+"""
+
+from __future__ import absolute_import
+
+import copy
+import logging
+import multiprocessing
+import sys
+import time
+import urllib3
+
+import six
+from six.moves import http_client as httplib
+from enum import Enum
+
+from oauthlib.oauth2 import LegacyApplicationClient
+from requests_oauthlib import OAuth2Session
+
+
+class TypeWithDefault(type):
+    def __init__(cls, name, bases, dct):
+        super(TypeWithDefault, cls).__init__(name, bases, dct)
+        cls._default = None
+
+    def __call__(cls):
+        if cls._default is None:
+            cls._default = type.__call__(cls)
+        return copy.copy(cls._default)
+
+    def set_default(cls, default):
+        cls._default = copy.copy(default)
+
+class AuthType(Enum):
+    BASIC = 1
+    OAUTH_PASSWORD_GRANT = 2
+    CUSTOM = 99
+
+class OAuthPasswordGrant():
+    """NOTE: You can inherit from this class in case this implementation 
+    of OAuth 2.0 password grant type does not work for you.
+    Alternatively you can use AuthType.CUSTOM to have full control over auth headers. 
+    """
+    def __init__(self, username, password, api_key, api_secret, oauth_token_url, prefix = 'Bearer '):
+        # necessary parameters
+        self._username = username
+        self._password = password
+        self._api_key = api_key
+        self._api_secret = api_secret
+        self._oauth_token_url = oauth_token_url
+
+        # optional parameters
+        self._prefix = prefix
+
+        # internal variables
+        self._token = None
+        self._oauth = OAuth2Session(client=LegacyApplicationClient(client_id=self._api_key))
+
+    def get_token(self):
+        """Gets HTTP oauth 2.0 password grant type authentication header (string).
+
+        :return: The token for oauth 2.0 grant type HTTP authentication.
+        """
+        if not self._token:
+            self._token = self._fetch_token()
+        else: 
+            token_expiry = self._token["created_at"] + self._token["expires_in"]
+            token_expired = token_expiry <= time.time()
+            if token_expired:
+                self._token = self._refresh_token()
+        token = self._prefix + self._token["access_token"]
+        return token
+
+    def _fetch_token(self):
+        headers = {
+            "API-Key": self._api_key,
+            "Content-Type": "application/x-www-form-urlencoded",
+        }
+        token =  self._oauth.fetch_token(token_url=self._oauth_token_url,
+                                       username=self._username, password=self._password, client_id=self._api_key,
+                                       client_secret=self._api_secret, include_client_id=True, headers=headers)
+        return token
+
+    def _refresh_token(self, **kwargs):
+        kwargs["client_id"] = self._api_key
+        kwargs["client_secret"] = self._api_secret
+        return self._oauth.refresh_token(self._oauth_token_url, **kwargs)
+
+
+class Configuration(six.with_metaclass(TypeWithDefault, object)):
+    """NOTE: This class is auto generated by the swagger code generator program.
+
+    Ref: https://github.com/swagger-api/swagger-codegen
+    Do not edit the class manually.
+    """
+
+    def __init__(self):
+        """Constructor"""
+        # Default Base url
+        self.host = "/v1"
+        # Temp file folder for downloading files
+        self.temp_folder_path = None
+
+        # Authentication Settings
+        # Select auth type
+        self.auth_type = AuthType.BASIC
+        ######################### 
+        # BASIC
+        # Do not encapsulate basic in a class to stay backwards-compatible
+        #########################
+        # dict to store API key(s)
+        self.api_key = {}
+        # dict to store API prefix (e.g. Bearer)
+        self.api_key_prefix = {}
+        # function to refresh API key if expired
+        self.refresh_api_key_hook = None
+        # Username for HTTP basic authentication
+        self.username = ""
+        # Password for HTTP basic authentication
+        self.password = ""
+        ######################### 
+        # OAuth 2.0 Password Grant 
+        # https://oauth.net/2/grant-types/password/
+        #########################
+        self.oauth_password_grant: OAuthPasswordGrant = None
+        ######################### 
+        # Custom hook to get Auth dictionary header
+        #########################
+        self.get_auth_settings_hook = None
+        # Logging Settings
+        self.logger = {}
+        self.logger["package_logger"] = logging.getLogger("netilion_lab_tab_api")
+        self.logger["urllib3_logger"] = logging.getLogger("urllib3")
+        # Log format
+        self.logger_format = '%(asctime)s %(levelname)s %(message)s'
+        # Log stream handler
+        self.logger_stream_handler = None
+        # Log file handler
+        self.logger_file_handler = None
+        # Debug file location
+        self.logger_file = None
+        # Debug switch
+        self.debug = False
+
+        # SSL/TLS verification
+        # Set this to false to skip verifying SSL certificate when calling API
+        # from https server.
+        self.verify_ssl = True
+        # Set this to customize the certificate file to verify the peer.
+        self.ssl_ca_cert = None
+        # client certificate file
+        self.cert_file = None
+        # client key file
+        self.key_file = None
+        # Set this to True/False to enable/disable SSL hostname verification.
+        self.assert_hostname = None
+
+        # urllib3 connection pool's maximum number of connections saved
+        # per pool. urllib3 uses 1 connection as default value, but this is
+        # not the best value when you are making a lot of possibly parallel
+        # requests to the same host, which is often the case here.
+        # cpu_count * 5 is used as default value to increase performance.
+        self.connection_pool_maxsize = multiprocessing.cpu_count() * 5
+
+        # Proxy URL
+        self.proxy = None
+        # Safe chars for path_param
+        self.safe_chars_for_path_param = ''
+
+    @property
+    def logger_file(self):
+        """The logger file.
+
+        If the logger_file is None, then add stream handler and remove file
+        handler. Otherwise, add file handler and remove stream handler.
+
+        :param value: The logger_file path.
+        :type: str
+        """
+        return self.__logger_file
+
+    @logger_file.setter
+    def logger_file(self, value):
+        """The logger file.
+
+        If the logger_file is None, then add stream handler and remove file
+        handler. Otherwise, add file handler and remove stream handler.
+
+        :param value: The logger_file path.
+        :type: str
+        """
+        self.__logger_file = value
+        if self.__logger_file:
+            # If set logging file,
+            # then add file handler and remove stream handler.
+            self.logger_file_handler = logging.FileHandler(self.__logger_file)
+            self.logger_file_handler.setFormatter(self.logger_formatter)
+            for _, logger in six.iteritems(self.logger):
+                logger.addHandler(self.logger_file_handler)
+                if self.logger_stream_handler:
+                    logger.removeHandler(self.logger_stream_handler)
+        else:
+            # If not set logging file,
+            # then add stream handler and remove file handler.
+            self.logger_stream_handler = logging.StreamHandler()
+            self.logger_stream_handler.setFormatter(self.logger_formatter)
+            for _, logger in six.iteritems(self.logger):
+                logger.addHandler(self.logger_stream_handler)
+                if self.logger_file_handler:
+                    logger.removeHandler(self.logger_file_handler)
+
+    @property
+    def debug(self):
+        """Debug status
+
+        :param value: The debug status, True or False.
+        :type: bool
+        """
+        return self.__debug
+
+    @debug.setter
+    def debug(self, value):
+        """Debug status
+
+        :param value: The debug status, True or False.
+        :type: bool
+        """
+        self.__debug = value
+        if self.__debug:
+            # if debug status is True, turn on debug logging
+            for _, logger in six.iteritems(self.logger):
+                logger.setLevel(logging.DEBUG)
+            # turn on httplib debug
+            httplib.HTTPConnection.debuglevel = 1
+        else:
+            # if debug status is False, turn off debug logging,
+            # setting log level to default `logging.WARNING`
+            for _, logger in six.iteritems(self.logger):
+                logger.setLevel(logging.WARNING)
+            # turn off httplib debug
+            httplib.HTTPConnection.debuglevel = 0
+
+    @property
+    def logger_format(self):
+        """The logger format.
+
+        The logger_formatter will be updated when sets logger_format.
+
+        :param value: The format string.
+        :type: str
+        """
+        return self.__logger_format
+
+    @logger_format.setter
+    def logger_format(self, value):
+        """The logger format.
+
+        The logger_formatter will be updated when sets logger_format.
+
+        :param value: The format string.
+        :type: str
+        """
+        self.__logger_format = value
+        self.logger_formatter = logging.Formatter(self.__logger_format)
+
+    def get_api_key_with_prefix(self, identifier):
+        """Gets API key (with prefix if set).
+
+        :param identifier: The identifier of apiKey.
+        :return: The token for api key authentication.
+        """
+        if self.refresh_api_key_hook:
+            self.refresh_api_key_hook(self)
+
+        key = self.api_key.get(identifier)
+        if key:
+            prefix = self.api_key_prefix.get(identifier)
+            if prefix:
+                return "%s %s" % (prefix, key)
+            else:
+                return key
+
+    def get_basic_auth_token(self):
+        """Gets HTTP basic authentication header (string).
+
+        :return: The token for basic HTTP authentication.
+        """
+        return urllib3.util.make_headers(
+            basic_auth=self.username + ':' + self.password
+        ).get('authorization')
+
+    def auth_settings(self):
+        """Gets Auth Settings dict for api client.
+
+        :return: The Auth Settings information dict.
+        """
+        if self.auth_type == AuthType.BASIC:
+            return {
+                'API-Key':
+                    {
+                        'type': 'api_key',
+                        'in': 'header',
+                        'key': 'API-Key',
+                        'value': self.get_api_key_with_prefix('API-Key')
+                    },
+                'Authentication':
+                    {
+                        'type': 'basic',
+                        'in': 'header',
+                        'key': 'Authorization',
+                        'value': self.get_basic_auth_token()
+                    },
+            }
+        elif self.auth_type == AuthType.OAUTH_PASSWORD_GRANT:
+            if not self.oauth_password_grant:
+                raise RuntimeError('Oauth grant type credentials need to be provided, please initialize oauth_password_grant.')
+            return {
+                'Authentication':
+                {
+                    'type': 'oauth_password_grant',
+                    'in': 'header',
+                    'key': 'Authorization',
+                    'value': self.oauth_password_grant.get_token()
+                },
+            }
+        elif self.auth_type == AuthType.CUSTOM:
+            if not self.get_auth_settings_hook:
+                raise RuntimeError('Please provide a get_auth_settings_hook returning authentication headers, see basic implementation here for an example.')
+            return self.get_auth_settings_hook(self)
+        else:
+            msg = "Auth type {} is not supported".format(self.auth_type)
+            raise ValueError(msg)
+
+    def to_debug_report(self):
+        """Gets the essential information for debugging.
+
+        :return: The report for debugging.
+        """
+        return "Python SDK Debug Report:\n"\
+               "OS: {env}\n"\
+               "Python Version: {pyversion}\n"\
+               "Version of the API: 01.00.00\n"\
+               "SDK Package Version: 1.2.0".\
+               format(env=sys.platform, pyversion=sys.version)
```

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/__init__.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,142 +1,167 @@
-# coding: utf-8
-
-# flake8: noqa
-"""
-    Netilion API Documentation
-
-    Welcome to the Netilion API Documentation, which provides interactive access and documentation to our REST API.  This section contains new endpoints which are still under development. You're welcome to test them but please note that they still can change anytime!   # noqa: E501
-
-    OpenAPI spec version: 01.00.00
-    
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
-"""
-
-from __future__ import absolute_import
-
-# import models into model package
-from netilion_lab_tab_api.models.add_on_base import AddOnBase
-from netilion_lab_tab_api.models.add_on_request import AddOnRequest
-from netilion_lab_tab_api.models.add_on_response import AddOnResponse
-from netilion_lab_tab_api.models.add_ons_response import AddOnsResponse
-from netilion_lab_tab_api.models.app_instance_base import AppInstanceBase
-from netilion_lab_tab_api.models.app_instance_request import AppInstanceRequest
-from netilion_lab_tab_api.models.app_instance_response import AppInstanceResponse
-from netilion_lab_tab_api.models.app_instances_response import AppInstancesResponse
-from netilion_lab_tab_api.models.asset_base import AssetBase
-from netilion_lab_tab_api.models.asset_i_ds import AssetIDs
-from netilion_lab_tab_api.models.asset_key_value_objects_data import AssetKeyValueObjectsData
-from netilion_lab_tab_api.models.asset_key_value_objects_response import AssetKeyValueObjectsResponse
-from netilion_lab_tab_api.models.asset_key_values_data import AssetKeyValuesData
-from netilion_lab_tab_api.models.asset_key_values_response import AssetKeyValuesResponse
-from netilion_lab_tab_api.models.asset_response import AssetResponse
-from netilion_lab_tab_api.models.asset_value import AssetValue
-from netilion_lab_tab_api.models.asset_value_object_request import AssetValueObjectRequest
-from netilion_lab_tab_api.models.asset_value_object_request_data import AssetValueObjectRequestData
-from netilion_lab_tab_api.models.asset_value_objects_pagination import AssetValueObjectsPagination
-from netilion_lab_tab_api.models.asset_value_objects_request import AssetValueObjectsRequest
-from netilion_lab_tab_api.models.asset_values_pagination import AssetValuesPagination
-from netilion_lab_tab_api.models.asset_values_response import AssetValuesResponse
-from netilion_lab_tab_api.models.assets_response import AssetsResponse
-from netilion_lab_tab_api.models.batch_base import BatchBase
-from netilion_lab_tab_api.models.batch_request import BatchRequest
-from netilion_lab_tab_api.models.batch_response import BatchResponse
-from netilion_lab_tab_api.models.batch_status_base import BatchStatusBase
-from netilion_lab_tab_api.models.batch_status_request import BatchStatusRequest
-from netilion_lab_tab_api.models.batch_status_response import BatchStatusResponse
-from netilion_lab_tab_api.models.batch_statuses import BatchStatuses
-from netilion_lab_tab_api.models.batch_statuses1 import BatchStatuses1
-from netilion_lab_tab_api.models.batch_type_base import BatchTypeBase
-from netilion_lab_tab_api.models.batch_type_request import BatchTypeRequest
-from netilion_lab_tab_api.models.batch_type_response import BatchTypeResponse
-from netilion_lab_tab_api.models.batch_types import BatchTypes
-from netilion_lab_tab_api.models.batches_response import BatchesResponse
-from netilion_lab_tab_api.models.certificate_renewal_request import CertificateRenewalRequest
-from netilion_lab_tab_api.models.certificate_renewal_response import CertificateRenewalResponse
-from netilion_lab_tab_api.models.connected_asset_request import ConnectedAssetRequest
-from netilion_lab_tab_api.models.connected_asset_request_configuration import ConnectedAssetRequestConfiguration
-from netilion_lab_tab_api.models.connected_asset_request_connection import ConnectedAssetRequestConnection
-from netilion_lab_tab_api.models.connected_asset_request_firmware import ConnectedAssetRequestFirmware
-from netilion_lab_tab_api.models.connected_asset_request_values import ConnectedAssetRequestValues
-from netilion_lab_tab_api.models.connected_asset_response import ConnectedAssetResponse
-from netilion_lab_tab_api.models.container_export_request import ContainerExportRequest
-from netilion_lab_tab_api.models.data_export_response import DataExportResponse
-from netilion_lab_tab_api.models.data_exports_response import DataExportsResponse
-from netilion_lab_tab_api.models.document_standard_base import DocumentStandardBase
-from netilion_lab_tab_api.models.document_standard_i_ds import DocumentStandardIDs
-from netilion_lab_tab_api.models.document_standard_response import DocumentStandardResponse
-from netilion_lab_tab_api.models.document_standards_response import DocumentStandardsResponse
-from netilion_lab_tab_api.models.error import Error
-from netilion_lab_tab_api.models.error_response import ErrorResponse
-from netilion_lab_tab_api.models.firmware_response import FirmwareResponse
-from netilion_lab_tab_api.models.id_pictures_body import IdPicturesBody
-from netilion_lab_tab_api.models.id_pictures_body1 import IdPicturesBody1
-from netilion_lab_tab_api.models.id_pictures_body2 import IdPicturesBody2
-from netilion_lab_tab_api.models.instrumentation_base import InstrumentationBase
-from netilion_lab_tab_api.models.instrumentation_i_ds import InstrumentationIDs
-from netilion_lab_tab_api.models.instrumentation_response import InstrumentationResponse
-from netilion_lab_tab_api.models.instrumentations_response import InstrumentationsResponse
-from netilion_lab_tab_api.models.link import Link
-from netilion_lab_tab_api.models.links import Links
-from netilion_lab_tab_api.models.links1 import Links1
-from netilion_lab_tab_api.models.links2 import Links2
-from netilion_lab_tab_api.models.links3 import Links3
-from netilion_lab_tab_api.models.links4 import Links4
-from netilion_lab_tab_api.models.mail_attachment_request import MailAttachmentRequest
-from netilion_lab_tab_api.models.mail_request import MailRequest
-from netilion_lab_tab_api.models.nested_id import NestedID
-from netilion_lab_tab_api.models.nested_id_href import NestedIDHref
-from netilion_lab_tab_api.models.nested_id_href_name import NestedIDHrefName
-from netilion_lab_tab_api.models.nested_id_href_serialnumber import NestedIDHrefSerialnumber
-from netilion_lab_tab_api.models.nested_id_href_tag import NestedIDHrefTag
-from netilion_lab_tab_api.models.node_base import NodeBase
-from netilion_lab_tab_api.models.node_i_ds import NodeIDs
-from netilion_lab_tab_api.models.node_response import NodeResponse
-from netilion_lab_tab_api.models.nodes_response import NodesResponse
-from netilion_lab_tab_api.models.pagination import Pagination
-from netilion_lab_tab_api.models.picture_link_request import PictureLinkRequest
-from netilion_lab_tab_api.models.picture_response import PictureResponse
-from netilion_lab_tab_api.models.pictures_id_body import PicturesIdBody
-from netilion_lab_tab_api.models.pictures_id_body1 import PicturesIdBody1
-from netilion_lab_tab_api.models.pictures_id_body2 import PicturesIdBody2
-from netilion_lab_tab_api.models.pictures_response import PicturesResponse
-from netilion_lab_tab_api.models.recipe_base import RecipeBase
-from netilion_lab_tab_api.models.recipe_request import RecipeRequest
-from netilion_lab_tab_api.models.recipe_response import RecipeResponse
-from netilion_lab_tab_api.models.recipe_status_base import RecipeStatusBase
-from netilion_lab_tab_api.models.recipe_status_request import RecipeStatusRequest
-from netilion_lab_tab_api.models.recipe_status_response import RecipeStatusResponse
-from netilion_lab_tab_api.models.recipe_statuses import RecipeStatuses
-from netilion_lab_tab_api.models.recipe_statuses1 import RecipeStatuses1
-from netilion_lab_tab_api.models.recipe_type_base import RecipeTypeBase
-from netilion_lab_tab_api.models.recipe_type_request import RecipeTypeRequest
-from netilion_lab_tab_api.models.recipe_type_response import RecipeTypeResponse
-from netilion_lab_tab_api.models.recipe_types import RecipeTypes
-from netilion_lab_tab_api.models.recipes_response import RecipesResponse
-from netilion_lab_tab_api.models.sim_card import SimCard
-from netilion_lab_tab_api.models.sim_card_request import SimCardRequest
-from netilion_lab_tab_api.models.sim_card_response import SimCardResponse
-from netilion_lab_tab_api.models.specification_base import SpecificationBase
-from netilion_lab_tab_api.models.specification_history_response import SpecificationHistoryResponse
-from netilion_lab_tab_api.models.specification_request import SpecificationRequest
-from netilion_lab_tab_api.models.specification_response import SpecificationResponse
-from netilion_lab_tab_api.models.specifications_delete import SpecificationsDelete
-from netilion_lab_tab_api.models.specifications_rename import SpecificationsRename
-from netilion_lab_tab_api.models.specifications_request import SpecificationsRequest
-from netilion_lab_tab_api.models.specifications_response import SpecificationsResponse
-from netilion_lab_tab_api.models.system_base import SystemBase
-from netilion_lab_tab_api.models.system_request import SystemRequest
-from netilion_lab_tab_api.models.system_response import SystemResponse
-from netilion_lab_tab_api.models.system_status_base import SystemStatusBase
-from netilion_lab_tab_api.models.system_status_request import SystemStatusRequest
-from netilion_lab_tab_api.models.system_status_response import SystemStatusResponse
-from netilion_lab_tab_api.models.system_statuses import SystemStatuses
-from netilion_lab_tab_api.models.system_statuses1 import SystemStatuses1
-from netilion_lab_tab_api.models.system_type_base import SystemTypeBase
-from netilion_lab_tab_api.models.system_type_request import SystemTypeRequest
-from netilion_lab_tab_api.models.system_type_response import SystemTypeResponse
-from netilion_lab_tab_api.models.system_types import SystemTypes
-from netilion_lab_tab_api.models.systems_response import SystemsResponse
-from netilion_lab_tab_api.models.threshold_base import ThresholdBase
-from netilion_lab_tab_api.models.threshold_request import ThresholdRequest
-from netilion_lab_tab_api.models.threshold_response import ThresholdResponse
-from netilion_lab_tab_api.models.thresholds_response import ThresholdsResponse
+# coding: utf-8
+
+# flake8: noqa
+
+"""
+    Netilion API Documentation
+
+    Welcome to the Netilion API Documentation, which provides interactive access and documentation to our REST API.  This section contains new endpoints which are still under development. You're welcome to test them but please note that they still can change anytime!   # noqa: E501
+
+    OpenAPI spec version: 01.00.00
+    
+    Generated by: https://github.com/swagger-api/swagger-codegen.git
+"""
+
+from __future__ import absolute_import
+
+# import apis into sdk package
+from netilion_lab_tab_api.api.add_on_api import AddOnApi
+from netilion_lab_tab_api.api.app_instance_api import AppInstanceApi
+from netilion_lab_tab_api.api.batch_api import BatchApi
+from netilion_lab_tab_api.api.batch_status_api import BatchStatusApi
+from netilion_lab_tab_api.api.batch_type_api import BatchTypeApi
+from netilion_lab_tab_api.api.connected_asset_api import ConnectedAssetApi
+from netilion_lab_tab_api.api.connected_asset_config_trigger_api import ConnectedAssetConfigTriggerApi
+from netilion_lab_tab_api.api.connected_asset_status_api import ConnectedAssetStatusApi
+from netilion_lab_tab_api.api.document_standard_api import DocumentStandardApi
+from netilion_lab_tab_api.api.mail_api import MailApi
+from netilion_lab_tab_api.api.recipe_api import RecipeApi
+from netilion_lab_tab_api.api.recipe_status_api import RecipeStatusApi
+from netilion_lab_tab_api.api.recipe_type_api import RecipeTypeApi
+from netilion_lab_tab_api.api.sim_card_api import SimCardApi
+from netilion_lab_tab_api.api.system_api import SystemApi
+from netilion_lab_tab_api.api.system_status_api import SystemStatusApi
+from netilion_lab_tab_api.api.system_type_api import SystemTypeApi
+from netilion_lab_tab_api.api.value_objects_api import ValueObjectsApi
+# import ApiClient
+from netilion_lab_tab_api.api_client import ApiClient
+from netilion_lab_tab_api.configuration import Configuration
+from netilion_lab_tab_api.configuration import AuthType
+from netilion_lab_tab_api.configuration import OAuthPasswordGrant
+# import models into sdk package
+from netilion_lab_tab_api.models.add_on_base import AddOnBase
+from netilion_lab_tab_api.models.add_on_request import AddOnRequest
+from netilion_lab_tab_api.models.add_on_response import AddOnResponse
+from netilion_lab_tab_api.models.add_ons_response import AddOnsResponse
+from netilion_lab_tab_api.models.app_instance_base import AppInstanceBase
+from netilion_lab_tab_api.models.app_instance_request import AppInstanceRequest
+from netilion_lab_tab_api.models.app_instance_response import AppInstanceResponse
+from netilion_lab_tab_api.models.app_instances_response import AppInstancesResponse
+from netilion_lab_tab_api.models.asset_base import AssetBase
+from netilion_lab_tab_api.models.asset_i_ds import AssetIDs
+from netilion_lab_tab_api.models.asset_key_value_objects_data import AssetKeyValueObjectsData
+from netilion_lab_tab_api.models.asset_key_value_objects_response import AssetKeyValueObjectsResponse
+from netilion_lab_tab_api.models.asset_key_values_data import AssetKeyValuesData
+from netilion_lab_tab_api.models.asset_key_values_response import AssetKeyValuesResponse
+from netilion_lab_tab_api.models.asset_response import AssetResponse
+from netilion_lab_tab_api.models.asset_value import AssetValue
+from netilion_lab_tab_api.models.asset_value_object_request import AssetValueObjectRequest
+from netilion_lab_tab_api.models.asset_value_object_request_data import AssetValueObjectRequestData
+from netilion_lab_tab_api.models.asset_value_objects_pagination import AssetValueObjectsPagination
+from netilion_lab_tab_api.models.asset_value_objects_request import AssetValueObjectsRequest
+from netilion_lab_tab_api.models.asset_values_pagination import AssetValuesPagination
+from netilion_lab_tab_api.models.asset_values_response import AssetValuesResponse
+from netilion_lab_tab_api.models.assets_response import AssetsResponse
+from netilion_lab_tab_api.models.batch_base import BatchBase
+from netilion_lab_tab_api.models.batch_request import BatchRequest
+from netilion_lab_tab_api.models.batch_response import BatchResponse
+from netilion_lab_tab_api.models.batch_status_base import BatchStatusBase
+from netilion_lab_tab_api.models.batch_status_request import BatchStatusRequest
+from netilion_lab_tab_api.models.batch_status_response import BatchStatusResponse
+from netilion_lab_tab_api.models.batch_statuses import BatchStatuses
+from netilion_lab_tab_api.models.batch_statuses1 import BatchStatuses1
+from netilion_lab_tab_api.models.batch_type_base import BatchTypeBase
+from netilion_lab_tab_api.models.batch_type_request import BatchTypeRequest
+from netilion_lab_tab_api.models.batch_type_response import BatchTypeResponse
+from netilion_lab_tab_api.models.batch_types import BatchTypes
+from netilion_lab_tab_api.models.batches_response import BatchesResponse
+from netilion_lab_tab_api.models.certificate_renewal_request import CertificateRenewalRequest
+from netilion_lab_tab_api.models.certificate_renewal_response import CertificateRenewalResponse
+from netilion_lab_tab_api.models.connected_asset_request import ConnectedAssetRequest
+from netilion_lab_tab_api.models.connected_asset_request_configuration import ConnectedAssetRequestConfiguration
+from netilion_lab_tab_api.models.connected_asset_request_connection import ConnectedAssetRequestConnection
+from netilion_lab_tab_api.models.connected_asset_request_firmware import ConnectedAssetRequestFirmware
+from netilion_lab_tab_api.models.connected_asset_request_values import ConnectedAssetRequestValues
+from netilion_lab_tab_api.models.connected_asset_response import ConnectedAssetResponse
+from netilion_lab_tab_api.models.container_export_request import ContainerExportRequest
+from netilion_lab_tab_api.models.data_export_response import DataExportResponse
+from netilion_lab_tab_api.models.data_exports_response import DataExportsResponse
+from netilion_lab_tab_api.models.document_standard_base import DocumentStandardBase
+from netilion_lab_tab_api.models.document_standard_i_ds import DocumentStandardIDs
+from netilion_lab_tab_api.models.document_standard_response import DocumentStandardResponse
+from netilion_lab_tab_api.models.document_standards_response import DocumentStandardsResponse
+from netilion_lab_tab_api.models.error import Error
+from netilion_lab_tab_api.models.error_response import ErrorResponse
+from netilion_lab_tab_api.models.firmware_response import FirmwareResponse
+from netilion_lab_tab_api.models.id_pictures_body import IdPicturesBody
+from netilion_lab_tab_api.models.id_pictures_body1 import IdPicturesBody1
+from netilion_lab_tab_api.models.id_pictures_body2 import IdPicturesBody2
+from netilion_lab_tab_api.models.instrumentation_base import InstrumentationBase
+from netilion_lab_tab_api.models.instrumentation_i_ds import InstrumentationIDs
+from netilion_lab_tab_api.models.instrumentation_response import InstrumentationResponse
+from netilion_lab_tab_api.models.instrumentations_response import InstrumentationsResponse
+from netilion_lab_tab_api.models.link import Link
+from netilion_lab_tab_api.models.links import Links
+from netilion_lab_tab_api.models.links1 import Links1
+from netilion_lab_tab_api.models.links2 import Links2
+from netilion_lab_tab_api.models.links3 import Links3
+from netilion_lab_tab_api.models.links4 import Links4
+from netilion_lab_tab_api.models.mail_attachment_request import MailAttachmentRequest
+from netilion_lab_tab_api.models.mail_request import MailRequest
+from netilion_lab_tab_api.models.nested_id import NestedID
+from netilion_lab_tab_api.models.nested_id_href import NestedIDHref
+from netilion_lab_tab_api.models.nested_id_href_name import NestedIDHrefName
+from netilion_lab_tab_api.models.nested_id_href_serialnumber import NestedIDHrefSerialnumber
+from netilion_lab_tab_api.models.nested_id_href_tag import NestedIDHrefTag
+from netilion_lab_tab_api.models.node_base import NodeBase
+from netilion_lab_tab_api.models.node_i_ds import NodeIDs
+from netilion_lab_tab_api.models.node_response import NodeResponse
+from netilion_lab_tab_api.models.nodes_response import NodesResponse
+from netilion_lab_tab_api.models.pagination import Pagination
+from netilion_lab_tab_api.models.picture_link_request import PictureLinkRequest
+from netilion_lab_tab_api.models.picture_response import PictureResponse
+from netilion_lab_tab_api.models.pictures_id_body import PicturesIdBody
+from netilion_lab_tab_api.models.pictures_id_body1 import PicturesIdBody1
+from netilion_lab_tab_api.models.pictures_id_body2 import PicturesIdBody2
+from netilion_lab_tab_api.models.pictures_response import PicturesResponse
+from netilion_lab_tab_api.models.recipe_base import RecipeBase
+from netilion_lab_tab_api.models.recipe_request import RecipeRequest
+from netilion_lab_tab_api.models.recipe_response import RecipeResponse
+from netilion_lab_tab_api.models.recipe_status_base import RecipeStatusBase
+from netilion_lab_tab_api.models.recipe_status_request import RecipeStatusRequest
+from netilion_lab_tab_api.models.recipe_status_response import RecipeStatusResponse
+from netilion_lab_tab_api.models.recipe_statuses import RecipeStatuses
+from netilion_lab_tab_api.models.recipe_statuses1 import RecipeStatuses1
+from netilion_lab_tab_api.models.recipe_type_base import RecipeTypeBase
+from netilion_lab_tab_api.models.recipe_type_request import RecipeTypeRequest
+from netilion_lab_tab_api.models.recipe_type_response import RecipeTypeResponse
+from netilion_lab_tab_api.models.recipe_types import RecipeTypes
+from netilion_lab_tab_api.models.recipes_response import RecipesResponse
+from netilion_lab_tab_api.models.sim_card import SimCard
+from netilion_lab_tab_api.models.sim_card_request import SimCardRequest
+from netilion_lab_tab_api.models.sim_card_response import SimCardResponse
+from netilion_lab_tab_api.models.specification_base import SpecificationBase
+from netilion_lab_tab_api.models.specification_history_response import SpecificationHistoryResponse
+from netilion_lab_tab_api.models.specification_request import SpecificationRequest
+from netilion_lab_tab_api.models.specification_response import SpecificationResponse
+from netilion_lab_tab_api.models.specifications_delete import SpecificationsDelete
+from netilion_lab_tab_api.models.specifications_rename import SpecificationsRename
+from netilion_lab_tab_api.models.specifications_request import SpecificationsRequest
+from netilion_lab_tab_api.models.specifications_response import SpecificationsResponse
+from netilion_lab_tab_api.models.system_base import SystemBase
+from netilion_lab_tab_api.models.system_request import SystemRequest
+from netilion_lab_tab_api.models.system_response import SystemResponse
+from netilion_lab_tab_api.models.system_status_base import SystemStatusBase
+from netilion_lab_tab_api.models.system_status_request import SystemStatusRequest
+from netilion_lab_tab_api.models.system_status_response import SystemStatusResponse
+from netilion_lab_tab_api.models.system_statuses import SystemStatuses
+from netilion_lab_tab_api.models.system_statuses1 import SystemStatuses1
+from netilion_lab_tab_api.models.system_type_base import SystemTypeBase
+from netilion_lab_tab_api.models.system_type_request import SystemTypeRequest
+from netilion_lab_tab_api.models.system_type_response import SystemTypeResponse
+from netilion_lab_tab_api.models.system_types import SystemTypes
+from netilion_lab_tab_api.models.systems_response import SystemsResponse
+from netilion_lab_tab_api.models.threshold_base import ThresholdBase
+from netilion_lab_tab_api.models.threshold_request import ThresholdRequest
+from netilion_lab_tab_api.models.threshold_response import ThresholdResponse
+from netilion_lab_tab_api.models.thresholds_response import ThresholdsResponse
```

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/add_on_base.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/add_on_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,26 +95,26 @@
 
         self._name = name
 
     @property
     def external_reference(self):
         """Gets the external_reference of this AddOnBase.  # noqa: E501
 
-        can be used to store id of external subscription managment system  # noqa: E501
+        can be used to store id of external subscription management system  # noqa: E501
 
         :return: The external_reference of this AddOnBase.  # noqa: E501
         :rtype: str
         """
         return self._external_reference
 
     @external_reference.setter
     def external_reference(self, external_reference):
         """Sets the external_reference of this AddOnBase.
 
-        can be used to store id of external subscription managment system  # noqa: E501
+        can be used to store id of external subscription management system  # noqa: E501
 
         :param external_reference: The external_reference of this AddOnBase.  # noqa: E501
         :type: str
         """
 
         self._external_reference = external_reference
 
@@ -187,26 +187,26 @@
 
         self._product_code = product_code
 
     @property
     def add_on_type(self):
         """Gets the add_on_type of this AddOnBase.  # noqa: E501
 
-        possible values are: connectivity and addon  # noqa: E501
+        possible values are: connectivity, addon and outcome  # noqa: E501
 
         :return: The add_on_type of this AddOnBase.  # noqa: E501
         :rtype: str
         """
         return self._add_on_type
 
     @add_on_type.setter
     def add_on_type(self, add_on_type):
         """Sets the add_on_type of this AddOnBase.
 
-        possible values are: connectivity and addon  # noqa: E501
+        possible values are: connectivity, addon and outcome  # noqa: E501
 
         :param add_on_type: The add_on_type of this AddOnBase.  # noqa: E501
         :type: str
         """
 
         self._add_on_type = add_on_type
```

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/add_on_request.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/add_on_request.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/add_on_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/add_on_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/add_ons_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/add_ons_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/app_instance_base.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/app_instance_base.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/app_instance_request.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/app_instance_request.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/app_instance_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/app_instance_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/app_instances_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/app_instances_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/asset_base.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/asset_base.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/asset_i_ds.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/asset_i_ds.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/asset_key_value_objects_data.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/asset_key_value_objects_data.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/asset_key_value_objects_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/asset_key_value_objects_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/asset_key_values_data.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/asset_key_values_data.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/asset_key_values_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/asset_key_values_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/asset_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/asset_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/asset_value.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/asset_value.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/asset_value_object_request.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/asset_value_object_request.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/asset_value_object_request_data.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/asset_value_object_request_data.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/asset_value_objects_pagination.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/asset_value_objects_pagination.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/asset_value_objects_request.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/asset_value_objects_request.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/asset_values_pagination.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/asset_values_pagination.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/asset_values_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/asset_values_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/assets_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/assets_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/batch_base.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/batch_base.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/batch_request.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/batch_request.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/batch_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/batch_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/batch_status_base.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/batch_status_base.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/batch_status_request.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/batch_status_request.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/batch_status_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/batch_status_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/batch_statuses.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/batch_statuses.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/batch_statuses1.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/batch_statuses1.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/batch_type_base.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/batch_type_base.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/batch_type_request.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/batch_type_request.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/batch_type_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/batch_type_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/batch_types.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/batch_types.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/batches_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/batches_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/certificate_renewal_request.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/certificate_renewal_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,26 +45,26 @@
         self.status = status
         self.csr = csr
 
     @property
     def status(self):
         """Gets the status of this CertificateRenewalRequest.  # noqa: E501
 
-        The status of the certificate renewal process. \"requesting\" indicates that a csr is sent in the request. \"success\" indicates that the connected asset has installed the new certificate and that the process can be closed. \"failed\" indicates that the connected asset has not installed the new certificate and that the process should be resetted.  # noqa: E501
+        The status of the certificate renewal process. \"requesting\" indicates that a csr is sent in the request. \"success\" indicates that the connected asset has installed the new certificate and that the process can be closed. \"failed\" indicates that the connected asset has not installed the new certificate and that the process should be reset.  # noqa: E501
 
         :return: The status of this CertificateRenewalRequest.  # noqa: E501
         :rtype: str
         """
         return self._status
 
     @status.setter
     def status(self, status):
         """Sets the status of this CertificateRenewalRequest.
 
-        The status of the certificate renewal process. \"requesting\" indicates that a csr is sent in the request. \"success\" indicates that the connected asset has installed the new certificate and that the process can be closed. \"failed\" indicates that the connected asset has not installed the new certificate and that the process should be resetted.  # noqa: E501
+        The status of the certificate renewal process. \"requesting\" indicates that a csr is sent in the request. \"success\" indicates that the connected asset has installed the new certificate and that the process can be closed. \"failed\" indicates that the connected asset has not installed the new certificate and that the process should be reset.  # noqa: E501
 
         :param status: The status of this CertificateRenewalRequest.  # noqa: E501
         :type: str
         """
         if status is None:
             raise ValueError("Invalid value for `status`, must not be `None`")  # noqa: E501
```

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/certificate_renewal_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/certificate_renewal_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/connected_asset_request.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/connected_asset_request.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/connected_asset_request_configuration.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/connected_asset_request_configuration.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/connected_asset_request_connection.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/connected_asset_request_connection.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/connected_asset_request_firmware.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/connected_asset_request_firmware.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/connected_asset_request_values.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/connected_asset_request_values.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/connected_asset_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/connected_asset_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,26 +127,26 @@
 
         self._firmware = firmware
 
     @property
     def diagnosis_command(self):
         """Gets the diagnosis_command of this ConnectedAssetResponse.  # noqa: E501
 
-        dignosis command to be sent to the connected asset  # noqa: E501
+        diagnosis command to be sent to the connected asset  # noqa: E501
 
         :return: The diagnosis_command of this ConnectedAssetResponse.  # noqa: E501
         :rtype: str
         """
         return self._diagnosis_command
 
     @diagnosis_command.setter
     def diagnosis_command(self, diagnosis_command):
         """Sets the diagnosis_command of this ConnectedAssetResponse.
 
-        dignosis command to be sent to the connected asset  # noqa: E501
+        diagnosis command to be sent to the connected asset  # noqa: E501
 
         :param diagnosis_command: The diagnosis_command of this ConnectedAssetResponse.  # noqa: E501
         :type: str
         """
 
         self._diagnosis_command = diagnosis_command
```

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/container_export_request.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/container_export_request.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/data_export_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/data_export_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/data_exports_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/data_exports_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/document_standard_base.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/document_standard_base.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/document_standard_i_ds.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/document_standard_i_ds.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/document_standard_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/document_standard_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/document_standards_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/document_standards_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/error.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/error.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,26 +50,26 @@
         if attribute is not None:
             self.attribute = attribute
 
     @property
     def type(self):
         """Gets the type of this Error.  # noqa: E501
 
-        The type of the error that occured. Possible types are * access_denied - access to the required resource denied * api_lockout - action would lead to an api lockout * assigned - resources has assigned resource * assigned_restriction - resource can't be deleted because of dependents * association_blank - mandatory association was blank * association_not_found - invalid reference used for relation field * association_tenant_conflict - tenant association mismatch * association_conflict - association mismatch * associations_already_added - duplicate association * associations_not_found - invalid references used for relation field * blank - mandatory field was not set * boolean_format - value is not a boolean * date_format - invalid date format for field * date_range - invalid date range * date_time_format - invalid date time format for field * date_year_month_format - invalid date/year month/year format * greater_than - value to high for numeric field * id_format - invalid format of an ID field * internal_server_error - unexpected error on server * invalid - format not allowed * invalid_input - invalid input data caused an error * invalid_enum_value - the given value is not a valid enum value * key_format - invalid key format * lockout - action would lead to a resource lockout * less_than - value to low for numeric field * missing_header - a mandatory request header is missing * missing_parameter - a mandatory request parameter is missing * not_a_number - for numerical fields * not_unique_in_scope - resource not unique in corresponding scope * number_format - wrong input for number * parameter_missing - required parameter for resource is missing * parent - resource can not be deleted cause its a parent to other resources * present - field that should not be set * quota_exceeded - file, image or asset could not be created because the subscription quota has exceeded * service_unavailable - service is currently not available * specification_not_found - specification for given key not found * specifications_not_found - specifications for given keys not found * taken - unique field is already taken * tenant_on_child - tenant parent/child conflict * too_long - length not in valid range * too_short - length not in valid range * unconfirmed - user is unconfirmed * wrong_format - invalid date format for field * wrong_length - does not match exact length  # noqa: E501
+        The type of the error that occurred. Possible types are * access_denied - access to the required resource denied * api_lockout - action would lead to an api lockout * assigned - resources has assigned resource * assigned_restriction - resource can't be deleted because of dependents * association_blank - mandatory association was blank * association_not_found - invalid reference used for relation field * association_tenant_conflict - tenant association mismatch * association_conflict - association mismatch * associations_already_added - duplicate association * associations_not_found - invalid references used for relation field * blank - mandatory field was not set * boolean_format - value is not a boolean * date_format - invalid date format for field * date_range - invalid date range * date_time_format - invalid date time format for field * date_year_month_format - invalid date/year month/year format * greater_than - value to high for numeric field * id_format - invalid format of an ID field * internal_server_error - unexpected error on server * invalid - format not allowed * invalid_input - invalid input data caused an error * invalid_enum_value - the given value is not a valid enum value * key_format - invalid key format * lockout - action would lead to a resource lockout * less_than - value to low for numeric field * missing_header - a mandatory request header is missing * missing_parameter - a mandatory request parameter is missing * not_a_number - for numerical fields * not_unique_in_scope - resource not unique in corresponding scope * number_format - wrong input for number * parameter_missing - required parameter for resource is missing * parent - resource can not be deleted cause its a parent to other resources * present - field that should not be set * quota_exceeded - file, image or asset could not be created because the subscription quota has exceeded * service_unavailable - service is currently not available * specification_not_found - specification for given key not found * specifications_not_found - specifications for given keys not found * taken - unique field is already taken * tenant_on_child - tenant parent/child conflict * too_long - length not in valid range * too_short - length not in valid range * unconfirmed - user is unconfirmed * wrong_format - invalid date format for field * wrong_length - does not match exact length  # noqa: E501
 
         :return: The type of this Error.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """Sets the type of this Error.
 
-        The type of the error that occured. Possible types are * access_denied - access to the required resource denied * api_lockout - action would lead to an api lockout * assigned - resources has assigned resource * assigned_restriction - resource can't be deleted because of dependents * association_blank - mandatory association was blank * association_not_found - invalid reference used for relation field * association_tenant_conflict - tenant association mismatch * association_conflict - association mismatch * associations_already_added - duplicate association * associations_not_found - invalid references used for relation field * blank - mandatory field was not set * boolean_format - value is not a boolean * date_format - invalid date format for field * date_range - invalid date range * date_time_format - invalid date time format for field * date_year_month_format - invalid date/year month/year format * greater_than - value to high for numeric field * id_format - invalid format of an ID field * internal_server_error - unexpected error on server * invalid - format not allowed * invalid_input - invalid input data caused an error * invalid_enum_value - the given value is not a valid enum value * key_format - invalid key format * lockout - action would lead to a resource lockout * less_than - value to low for numeric field * missing_header - a mandatory request header is missing * missing_parameter - a mandatory request parameter is missing * not_a_number - for numerical fields * not_unique_in_scope - resource not unique in corresponding scope * number_format - wrong input for number * parameter_missing - required parameter for resource is missing * parent - resource can not be deleted cause its a parent to other resources * present - field that should not be set * quota_exceeded - file, image or asset could not be created because the subscription quota has exceeded * service_unavailable - service is currently not available * specification_not_found - specification for given key not found * specifications_not_found - specifications for given keys not found * taken - unique field is already taken * tenant_on_child - tenant parent/child conflict * too_long - length not in valid range * too_short - length not in valid range * unconfirmed - user is unconfirmed * wrong_format - invalid date format for field * wrong_length - does not match exact length  # noqa: E501
+        The type of the error that occurred. Possible types are * access_denied - access to the required resource denied * api_lockout - action would lead to an api lockout * assigned - resources has assigned resource * assigned_restriction - resource can't be deleted because of dependents * association_blank - mandatory association was blank * association_not_found - invalid reference used for relation field * association_tenant_conflict - tenant association mismatch * association_conflict - association mismatch * associations_already_added - duplicate association * associations_not_found - invalid references used for relation field * blank - mandatory field was not set * boolean_format - value is not a boolean * date_format - invalid date format for field * date_range - invalid date range * date_time_format - invalid date time format for field * date_year_month_format - invalid date/year month/year format * greater_than - value to high for numeric field * id_format - invalid format of an ID field * internal_server_error - unexpected error on server * invalid - format not allowed * invalid_input - invalid input data caused an error * invalid_enum_value - the given value is not a valid enum value * key_format - invalid key format * lockout - action would lead to a resource lockout * less_than - value to low for numeric field * missing_header - a mandatory request header is missing * missing_parameter - a mandatory request parameter is missing * not_a_number - for numerical fields * not_unique_in_scope - resource not unique in corresponding scope * number_format - wrong input for number * parameter_missing - required parameter for resource is missing * parent - resource can not be deleted cause its a parent to other resources * present - field that should not be set * quota_exceeded - file, image or asset could not be created because the subscription quota has exceeded * service_unavailable - service is currently not available * specification_not_found - specification for given key not found * specifications_not_found - specifications for given keys not found * taken - unique field is already taken * tenant_on_child - tenant parent/child conflict * too_long - length not in valid range * too_short - length not in valid range * unconfirmed - user is unconfirmed * wrong_format - invalid date format for field * wrong_length - does not match exact length  # noqa: E501
 
         :param type: The type of this Error.  # noqa: E501
         :type: str
         """
         if type is None:
             raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
 
@@ -100,26 +100,26 @@
 
         self._message = message
 
     @property
     def attribute(self):
         """Gets the attribute of this Error.  # noqa: E501
 
-        the attribute on which the error occured. This could be used to figure out which field was invalid. Is also set for relation attributes with faulty references  # noqa: E501
+        the attribute on which the error occurred. This could be used to figure out which field was invalid. Is also set for relation attributes with faulty references  # noqa: E501
 
         :return: The attribute of this Error.  # noqa: E501
         :rtype: str
         """
         return self._attribute
 
     @attribute.setter
     def attribute(self, attribute):
         """Sets the attribute of this Error.
 
-        the attribute on which the error occured. This could be used to figure out which field was invalid. Is also set for relation attributes with faulty references  # noqa: E501
+        the attribute on which the error occurred. This could be used to figure out which field was invalid. Is also set for relation attributes with faulty references  # noqa: E501
 
         :param attribute: The attribute of this Error.  # noqa: E501
         :type: str
         """
 
         self._attribute = attribute
```

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/error_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/error_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/firmware_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/firmware_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/id_pictures_body.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/id_pictures_body.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/id_pictures_body1.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/id_pictures_body1.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/id_pictures_body2.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/id_pictures_body2.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/instrumentation_base.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/instrumentation_base.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/instrumentation_i_ds.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/instrumentation_i_ds.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/instrumentation_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/instrumentation_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/instrumentations_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/instrumentations_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/link.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/link.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/links.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/links.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/links1.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/links1.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/links2.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/links2.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/links3.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/links3.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/links4.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/links4.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/mail_attachment_request.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/mail_attachment_request.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/mail_request.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/mail_request.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/nested_id.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/nested_id.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/nested_id_href.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/nested_id_href.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/nested_id_href_name.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/nested_id_href_name.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/nested_id_href_serialnumber.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/nested_id_href_serialnumber.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/nested_id_href_tag.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/nested_id_href_tag.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/node_base.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/node_base.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/node_i_ds.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/node_i_ds.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/node_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/node_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/nodes_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/nodes_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/pagination.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/pagination.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/picture_link_request.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/picture_link_request.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/picture_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/picture_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/pictures_id_body.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/pictures_id_body.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/pictures_id_body1.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/pictures_id_body1.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/pictures_id_body2.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/pictures_id_body2.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/pictures_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/pictures_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/recipe_base.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/recipe_base.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/recipe_request.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/recipe_request.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/recipe_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/recipe_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/recipe_status_base.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/recipe_status_base.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/recipe_status_request.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/recipe_status_request.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/recipe_status_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/recipe_status_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/recipe_statuses.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/recipe_statuses.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/recipe_statuses1.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/recipe_statuses1.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/recipe_type_base.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/recipe_type_base.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/recipe_type_request.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/recipe_type_request.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/recipe_type_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/recipe_type_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/recipe_types.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/recipe_types.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/recipes_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/recipes_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/sim_card.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/sim_card.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/sim_card_request.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/sim_card_request.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/sim_card_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/sim_card_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/specification_base.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/specification_base.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/specification_history_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/specification_history_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/specification_request.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/specification_request.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/specification_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/specification_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/specifications_delete.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/specifications_delete.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/specifications_rename.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/specifications_rename.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/specifications_request.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/specifications_request.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/specifications_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/specifications_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/system_base.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/system_base.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/system_request.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/system_request.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/system_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/system_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/system_status_base.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/system_status_base.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/system_status_request.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/system_status_request.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/system_status_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/system_status_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/system_statuses.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/system_statuses.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/system_statuses1.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/system_statuses1.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/system_type_base.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/system_type_base.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/system_type_request.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/system_type_request.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/system_type_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/system_type_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/system_types.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/system_types.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/systems_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/systems_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/threshold_base.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/threshold_base.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/threshold_request.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/threshold_request.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/threshold_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/threshold_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/models/thresholds_response.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/models/thresholds_response.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api/rest.py` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api/rest.py`

 * *Files identical despite different names*

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api.egg-info/PKG-INFO` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netilion-lab-tab-api
-Version: 1.1.3
+Version: 1.2.0
 Summary: Client for accessing Lab part of Netilion cloud
 Author-email: Andrey Dodonov <Andrey.Dodonov@endress.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `netilion_lab_tab_api-1.1.3/src/netilion_lab_tab_api.egg-info/SOURCES.txt` & `netilion_lab_tab_api-1.2.0/src/netilion_lab_tab_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 src/netilion_lab_tab_api.egg-info/top_level.txt
 src/netilion_lab_tab_api/api/__init__.py
 src/netilion_lab_tab_api/api/add_on_api.py
 src/netilion_lab_tab_api/api/app_instance_api.py
 src/netilion_lab_tab_api/api/batch_api.py
 src/netilion_lab_tab_api/api/batch_status_api.py
 src/netilion_lab_tab_api/api/batch_type_api.py
-src/netilion_lab_tab_api/api/connected_asset_api.py
+src/netilion_lab_tab_api/api/connected_asset_api_api.py
 src/netilion_lab_tab_api/api/connected_asset_config_trigger_api.py
 src/netilion_lab_tab_api/api/connected_asset_status_api.py
 src/netilion_lab_tab_api/api/document_standard_api.py
 src/netilion_lab_tab_api/api/mail_api.py
 src/netilion_lab_tab_api/api/recipe_api.py
 src/netilion_lab_tab_api/api/recipe_status_api.py
 src/netilion_lab_tab_api/api/recipe_type_api.py
@@ -36,14 +36,15 @@
 src/netilion_lab_tab_api/models/add_ons_response.py
 src/netilion_lab_tab_api/models/app_instance_base.py
 src/netilion_lab_tab_api/models/app_instance_request.py
 src/netilion_lab_tab_api/models/app_instance_response.py
 src/netilion_lab_tab_api/models/app_instances_response.py
 src/netilion_lab_tab_api/models/asset_base.py
 src/netilion_lab_tab_api/models/asset_i_ds.py
+src/netilion_lab_tab_api/models/asset_id_upload_body.py
 src/netilion_lab_tab_api/models/asset_key_value_objects_data.py
 src/netilion_lab_tab_api/models/asset_key_value_objects_response.py
 src/netilion_lab_tab_api/models/asset_key_values_data.py
 src/netilion_lab_tab_api/models/asset_key_values_response.py
 src/netilion_lab_tab_api/models/asset_response.py
 src/netilion_lab_tab_api/models/asset_value.py
 src/netilion_lab_tab_api/models/asset_value_object_request.py
```

