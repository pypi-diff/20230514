# Comparing `tmp/dlt-0.2.6a2.tar.gz` & `tmp/dlt-0.2.7a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlt-0.2.6a2.tar", max compression
+gzip compressed data, was "dlt-0.2.7a0.tar", max compression
```

## Comparing `dlt-0.2.6a2.tar` & `dlt-0.2.7a0.tar`

### file list

```diff
@@ -1,209 +1,209 @@
--rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.2.6a2/LICENSE.txt
--rw-r--r--   0        0        0     4214 2023-04-30 21:17:44.388805 dlt-0.2.6a2/README.md
--rw-r--r--   0        0        0     1711 2023-04-30 21:17:44.388805 dlt-0.2.6a2/dlt/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 21:17:44.388805 dlt-0.2.6a2/dlt/cli/__init__.py
--rw-r--r--   0        0        0    15909 2023-05-05 10:04:39.176579 dlt-0.2.6a2/dlt/cli/_dlt.py
--rw-r--r--   0        0        0     3858 2023-05-07 18:29:53.319469 dlt-0.2.6a2/dlt/cli/config_toml_writer.py
--rw-r--r--   0        0        0    16663 2023-04-22 20:26:30.632198 dlt-0.2.6a2/dlt/cli/deploy_command.py
--rw-r--r--   0        0        0     1853 2023-04-30 21:17:44.388805 dlt-0.2.6a2/dlt/cli/echo.py
--rw-r--r--   0        0        0      435 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/cli/exceptions.py
--rw-r--r--   0        0        0    18888 2023-04-22 20:26:30.632198 dlt-0.2.6a2/dlt/cli/init_command.py
--rw-r--r--   0        0        0    10489 2023-04-30 21:17:44.388805 dlt-0.2.6a2/dlt/cli/pipeline_command.py
--rw-r--r--   0        0        0     9419 2023-04-03 18:50:36.893525 dlt-0.2.6a2/dlt/cli/pipeline_files.py
--rw-r--r--   0        0        0     4510 2023-05-04 15:57:31.375706 dlt-0.2.6a2/dlt/cli/source_detection.py
--rw-r--r--   0        0        0     1899 2023-04-22 20:26:30.632198 dlt-0.2.6a2/dlt/cli/telemetry_command.py
--rw-r--r--   0        0        0     3757 2023-04-30 21:17:44.388805 dlt-0.2.6a2/dlt/cli/utils.py
--rw-r--r--   0        0        0      307 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/__init__.py
--rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.2.6a2/dlt/common/arithmetics.py
--rw-r--r--   0        0        0      428 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/configuration/__init__.py
--rw-r--r--   0        0        0     4184 2023-05-07 13:09:43.709469 dlt-0.2.6a2/dlt/common/configuration/accessors.py
--rw-r--r--   0        0        0     3469 2023-05-07 15:40:06.149469 dlt-0.2.6a2/dlt/common/configuration/container.py
--rw-r--r--   0        0        0     5884 2023-04-22 20:26:30.632198 dlt-0.2.6a2/dlt/common/configuration/exceptions.py
--rw-r--r--   0        0        0     7912 2023-04-22 20:26:30.632198 dlt-0.2.6a2/dlt/common/configuration/inject.py
--rw-r--r--   0        0        0     1198 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/configuration/paths.py
--rw-r--r--   0        0        0      306 2023-05-06 21:48:15.113451 dlt-0.2.6a2/dlt/common/configuration/providers/__init__.py
--rw-r--r--   0        0        0     1108 2023-04-26 11:34:23.292768 dlt-0.2.6a2/dlt/common/configuration/providers/airflow.py
--rw-r--r--   0        0        0     1116 2023-05-07 12:57:30.109469 dlt-0.2.6a2/dlt/common/configuration/providers/context.py
--rw-r--r--   0        0        0     1335 2023-05-07 15:00:38.059469 dlt-0.2.6a2/dlt/common/configuration/providers/dictionary.py
--rw-r--r--   0        0        0     1981 2023-05-07 13:01:36.889469 dlt-0.2.6a2/dlt/common/configuration/providers/environ.py
--rw-r--r--   0        0        0     9498 2023-05-07 18:33:09.349469 dlt-0.2.6a2/dlt/common/configuration/providers/google_secrets.py
--rw-r--r--   0        0        0     1108 2023-05-07 12:58:14.469469 dlt-0.2.6a2/dlt/common/configuration/providers/provider.py
--rw-r--r--   0        0        0     5235 2023-05-07 18:28:29.189469 dlt-0.2.6a2/dlt/common/configuration/providers/toml.py
--rw-r--r--   0        0        0    17421 2023-05-07 15:41:10.039469 dlt-0.2.6a2/dlt/common/configuration/resolve.py
--rw-r--r--   0        0        0     1176 2023-05-06 11:01:57.676603 dlt-0.2.6a2/dlt/common/configuration/specs/__init__.py
--rw-r--r--   0        0        0     1817 2023-05-06 11:01:10.206603 dlt-0.2.6a2/dlt/common/configuration/specs/api_credentials.py
--rw-r--r--   0        0        0    13108 2023-05-07 15:36:02.179469 dlt-0.2.6a2/dlt/common/configuration/specs/base_configuration.py
--rw-r--r--   0        0        0     4405 2023-05-07 19:22:59.599469 dlt-0.2.6a2/dlt/common/configuration/specs/config_providers_context.py
--rw-r--r--   0        0        0     2792 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/configuration/specs/config_section_context.py
--rw-r--r--   0        0        0     1798 2023-05-07 15:28:27.649469 dlt-0.2.6a2/dlt/common/configuration/specs/connection_string_credentials.py
--rw-r--r--   0        0        0     2125 2023-04-24 18:26:21.111453 dlt-0.2.6a2/dlt/common/configuration/specs/exceptions.py
--rw-r--r--   0        0        0    12725 2023-05-07 18:34:32.579469 dlt-0.2.6a2/dlt/common/configuration/specs/gcp_credentials.py
--rw-r--r--   0        0        0      725 2023-05-07 08:35:40.786864 dlt-0.2.6a2/dlt/common/configuration/specs/known_sections.py
--rw-r--r--   0        0        0      556 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/configuration/specs/load_volume_configuration.py
--rw-r--r--   0        0        0      417 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/configuration/specs/normalize_volume_configuration.py
--rw-r--r--   0        0        0     2455 2023-04-30 21:17:44.388805 dlt-0.2.6a2/dlt/common/configuration/specs/run_configuration.py
--rw-r--r--   0        0        0      944 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/configuration/specs/schema_volume_configuration.py
--rw-r--r--   0        0        0     6026 2023-05-06 20:38:37.173451 dlt-0.2.6a2/dlt/common/configuration/utils.py
--rw-r--r--   0        0        0      142 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/data_types/__init__.py
--rw-r--r--   0        0        0     6306 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/data_types/type_helpers.py
--rw-r--r--   0        0        0      214 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/data_types/typing.py
--rw-r--r--   0        0        0      260 2023-03-23 14:48:20.701618 dlt-0.2.6a2/dlt/common/data_writers/__init__.py
--rw-r--r--   0        0        0     5893 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/data_writers/buffered.py
--rw-r--r--   0        0        0     2395 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/data_writers/escape.py
--rw-r--r--   0        0        0      962 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/data_writers/exceptions.py
--rw-r--r--   0        0        0     5159 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/data_writers/writers.py
--rw-r--r--   0        0        0       97 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/destination/__init__.py
--rw-r--r--   0        0        0     2206 2023-04-05 08:03:40.638919 dlt-0.2.6a2/dlt/common/destination/capabilities.py
--rw-r--r--   0        0        0    10682 2023-04-24 11:35:34.867759 dlt-0.2.6a2/dlt/common/destination/reference.py
--rw-r--r--   0        0        0     6121 2023-04-30 21:17:44.388805 dlt-0.2.6a2/dlt/common/exceptions.py
--rw-r--r--   0        0        0     4954 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/git.py
--rw-r--r--   0        0        0     5248 2023-04-10 08:12:53.759595 dlt-0.2.6a2/dlt/common/json/__init__.py
--rw-r--r--   0        0        0     1802 2023-04-10 08:12:53.769595 dlt-0.2.6a2/dlt/common/json/_orjson.py
--rw-r--r--   0        0        0     2939 2023-04-10 08:12:53.769595 dlt-0.2.6a2/dlt/common/json/_simplejson.py
--rw-r--r--   0        0        0     1536 2023-04-29 12:58:55.943219 dlt-0.2.6a2/dlt/common/jsonpath.py
--rw-r--r--   0        0        0      232 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/normalizers/__init__.py
--rw-r--r--   0        0        0     1197 2023-05-07 15:38:15.119469 dlt-0.2.6a2/dlt/common/normalizers/configuration.py
--rw-r--r--   0        0        0      472 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/normalizers/exceptions.py
--rw-r--r--   0        0        0     1644 2023-04-06 15:27:24.759561 dlt-0.2.6a2/dlt/common/normalizers/json/__init__.py
--rw-r--r--   0        0        0    13396 2023-04-06 15:27:24.759561 dlt-0.2.6a2/dlt/common/normalizers/json/relational.py
--rw-r--r--   0        0        0       64 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/normalizers/naming/__init__.py
--rw-r--r--   0        0        0      807 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/normalizers/naming/direct.py
--rw-r--r--   0        0        0     1069 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/normalizers/naming/duck_case.py
--rw-r--r--   0        0        0      792 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/normalizers/naming/exceptions.py
--rw-r--r--   0        0        0     3753 2023-04-05 08:03:40.638919 dlt-0.2.6a2/dlt/common/normalizers/naming/naming.py
--rw-r--r--   0        0        0     3002 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/normalizers/naming/snake_case.py
--rw-r--r--   0        0        0      358 2023-04-02 09:09:15.855769 dlt-0.2.6a2/dlt/common/normalizers/typing.py
--rw-r--r--   0        0        0     2337 2023-04-06 15:27:24.759561 dlt-0.2.6a2/dlt/common/normalizers/utils.py
--rw-r--r--   0        0        0      451 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/pendulum.py
--rw-r--r--   0        0        0    16937 2023-04-30 21:17:44.388805 dlt-0.2.6a2/dlt/common/pipeline.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/reflection/__init__.py
--rw-r--r--   0        0        0      374 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/reflection/function_visitor.py
--rw-r--r--   0        0        0     4891 2023-04-09 16:39:04.593180 dlt-0.2.6a2/dlt/common/reflection/spec.py
--rw-r--r--   0        0        0     5069 2023-04-24 18:26:21.111453 dlt-0.2.6a2/dlt/common/reflection/utils.py
--rw-r--r--   0        0        0      174 2023-04-30 21:17:44.388805 dlt-0.2.6a2/dlt/common/runners/__init__.py
--rw-r--r--   0        0        0      508 2023-04-30 21:17:44.388805 dlt-0.2.6a2/dlt/common/runners/configuration.py
--rw-r--r--   0        0        0     2635 2023-04-30 21:17:44.388805 dlt-0.2.6a2/dlt/common/runners/pool_runner.py
--rw-r--r--   0        0        0     4046 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/common/runners/runnable.py
--rw-r--r--   0        0        0     3145 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/common/runners/stdout.py
--rw-r--r--   0        0        0     2137 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/common/runners/synth_pickle.py
--rw-r--r--   0        0        0      105 2023-04-30 21:17:44.388805 dlt-0.2.6a2/dlt/common/runners/typing.py
--rw-r--r--   0        0        0     5590 2023-05-06 08:15:02.906603 dlt-0.2.6a2/dlt/common/runners/venv.py
--rw-r--r--   0        0        0       36 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/common/runtime/__init__.py
--rw-r--r--   0        0        0    13441 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/common/runtime/collector.py
--rw-r--r--   0        0        0     4264 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/common/runtime/exec_info.py
--rw-r--r--   0        0        0      647 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/common/runtime/init.py
--rw-r--r--   0        0        0     4002 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/common/runtime/logger.py
--rw-r--r--   0        0        0     2052 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/common/runtime/prometheus.py
--rw-r--r--   0        0        0     7170 2023-04-22 20:26:30.632198 dlt-0.2.6a2/dlt/common/runtime/segment.py
--rw-r--r--   0        0        0     2493 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/common/runtime/sentry.py
--rw-r--r--   0        0        0     2027 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/common/runtime/signals.py
--rw-r--r--   0        0        0      616 2023-04-03 18:50:36.893525 dlt-0.2.6a2/dlt/common/runtime/slack.py
--rw-r--r--   0        0        0      720 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/common/runtime/telemetry.py
--rw-r--r--   0        0        0      387 2023-04-03 18:50:36.893525 dlt-0.2.6a2/dlt/common/schema/__init__.py
--rw-r--r--   0        0        0     1927 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/common/schema/detections.py
--rw-r--r--   0        0        0     2974 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/common/schema/exceptions.py
--rw-r--r--   0        0        0    25175 2023-04-09 16:39:04.593180 dlt-0.2.6a2/dlt/common/schema/schema.py
--rw-r--r--   0        0        0     3004 2023-04-22 20:26:30.632198 dlt-0.2.6a2/dlt/common/schema/typing.py
--rw-r--r--   0        0        0    23087 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/common/schema/utils.py
--rw-r--r--   0        0        0      410 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/common/storages/__init__.py
--rw-r--r--   0        0        0     1906 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/common/storages/data_item_storage.py
--rw-r--r--   0        0        0     2804 2023-04-03 18:50:36.893525 dlt-0.2.6a2/dlt/common/storages/exceptions.py
--rw-r--r--   0        0        0     9059 2023-04-05 08:03:40.638919 dlt-0.2.6a2/dlt/common/storages/file_storage.py
--rw-r--r--   0        0        0     2685 2023-04-13 08:33:43.967587 dlt-0.2.6a2/dlt/common/storages/live_schema_storage.py
--rw-r--r--   0        0        0    21810 2023-04-29 12:58:55.953219 dlt-0.2.6a2/dlt/common/storages/load_storage.py
--rw-r--r--   0        0        0     2414 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/common/storages/normalize_storage.py
--rw-r--r--   0        0        0     8508 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/common/storages/schema_storage.py
--rw-r--r--   0        0        0     2525 2023-04-24 18:26:21.111453 dlt-0.2.6a2/dlt/common/storages/versioned_storage.py
--rw-r--r--   0        0        0     2634 2023-05-06 13:51:40.766603 dlt-0.2.6a2/dlt/common/time.py
--rw-r--r--   0        0        0     4736 2023-04-03 18:50:36.893525 dlt-0.2.6a2/dlt/common/typing.py
--rw-r--r--   0        0        0    11275 2023-04-24 18:26:21.111453 dlt-0.2.6a2/dlt/common/utils.py
--rw-r--r--   0        0        0     3686 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/common/validation.py
--rw-r--r--   0        0        0     1185 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/common/wei.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/destinations/__init__.py
--rw-r--r--   0        0        0      437 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/destinations/bigquery/README.md
--rw-r--r--   0        0        0     1813 2023-04-05 08:03:40.638919 dlt-0.2.6a2/dlt/destinations/bigquery/__init__.py
--rw-r--r--   0        0        0    12347 2023-05-06 08:09:11.286603 dlt-0.2.6a2/dlt/destinations/bigquery/bigquery.py
--rw-r--r--   0        0        0      386 2023-05-06 08:06:12.886603 dlt-0.2.6a2/dlt/destinations/bigquery/configuration.py
--rw-r--r--   0        0        0    10342 2023-05-07 21:18:02.789469 dlt-0.2.6a2/dlt/destinations/bigquery/sql_client.py
--rw-r--r--   0        0        0     1935 2023-04-05 08:03:40.638919 dlt-0.2.6a2/dlt/destinations/duckdb/__init__.py
--rw-r--r--   0        0        0     7008 2023-05-07 15:38:35.819469 dlt-0.2.6a2/dlt/destinations/duckdb/configuration.py
--rw-r--r--   0        0        0     2754 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/destinations/duckdb/duck.py
--rw-r--r--   0        0        0     6936 2023-04-21 22:25:54.789942 dlt-0.2.6a2/dlt/destinations/duckdb/sql_client.py
--rw-r--r--   0        0        0     1671 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/destinations/dummy/__init__.py
--rw-r--r--   0        0        0      736 2023-04-03 18:50:36.893525 dlt-0.2.6a2/dlt/destinations/dummy/configuration.py
--rw-r--r--   0        0        0     4975 2023-04-24 11:35:34.867759 dlt-0.2.6a2/dlt/destinations/dummy/dummy.py
--rw-r--r--   0        0        0     4159 2023-04-05 08:03:40.638919 dlt-0.2.6a2/dlt/destinations/exceptions.py
--rw-r--r--   0        0        0     4983 2023-04-05 08:03:40.638919 dlt-0.2.6a2/dlt/destinations/insert_job_client.py
--rw-r--r--   0        0        0    15357 2023-05-02 21:00:32.948848 dlt-0.2.6a2/dlt/destinations/job_client_impl.py
--rw-r--r--   0        0        0     1303 2023-04-05 08:03:40.638919 dlt-0.2.6a2/dlt/destinations/job_impl.py
--rw-r--r--   0        0        0      251 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/destinations/postgres/README.md
--rw-r--r--   0        0        0     1934 2023-04-05 08:03:40.638919 dlt-0.2.6a2/dlt/destinations/postgres/__init__.py
--rw-r--r--   0        0        0     1232 2023-05-06 08:19:47.236603 dlt-0.2.6a2/dlt/destinations/postgres/configuration.py
--rw-r--r--   0        0        0     3025 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/destinations/postgres/postgres.py
--rw-r--r--   0        0        0     6074 2023-05-06 08:20:42.386603 dlt-0.2.6a2/dlt/destinations/postgres/sql_client.py
--rw-r--r--   0        0        0     1159 2023-04-03 18:50:36.893525 dlt-0.2.6a2/dlt/destinations/redshift/README.md
--rw-r--r--   0        0        0     1905 2023-04-05 08:03:40.638919 dlt-0.2.6a2/dlt/destinations/redshift/__init__.py
--rw-r--r--   0        0        0      570 2023-05-06 08:30:19.436603 dlt-0.2.6a2/dlt/destinations/redshift/configuration.py
--rw-r--r--   0        0        0     3761 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/destinations/redshift/redshift.py
--rw-r--r--   0        0        0     7110 2023-04-29 12:58:55.953219 dlt-0.2.6a2/dlt/destinations/sql_client.py
--rw-r--r--   0        0        0    10101 2023-04-09 16:39:04.593180 dlt-0.2.6a2/dlt/destinations/sql_merge_job.py
--rw-r--r--   0        0        0     1931 2023-04-24 18:26:21.111453 dlt-0.2.6a2/dlt/destinations/typing.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.2.6a2/dlt/extract/__init__.py
--rw-r--r--   0        0        0    22860 2023-05-07 10:39:43.846864 dlt-0.2.6a2/dlt/extract/decorators.py
--rw-r--r--   0        0        0    12645 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/extract/exceptions.py
--rw-r--r--   0        0        0     8449 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/extract/extract.py
--rw-r--r--   0        0        0    14658 2023-05-07 15:38:58.249469 dlt-0.2.6a2/dlt/extract/incremental.py
--rw-r--r--   0        0        0    31567 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/extract/pipe.py
--rw-r--r--   0        0        0     9683 2023-04-22 20:26:30.632198 dlt-0.2.6a2/dlt/extract/schema.py
--rw-r--r--   0        0        0    34195 2023-05-07 10:42:54.466864 dlt-0.2.6a2/dlt/extract/source.py
--rw-r--r--   0        0        0     4350 2023-04-22 20:26:30.632198 dlt-0.2.6a2/dlt/extract/typing.py
--rw-r--r--   0        0        0      593 2023-04-06 20:38:35.239561 dlt-0.2.6a2/dlt/extract/utils.py
--rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.2.6a2/dlt/helpers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/helpers/airflow/__init__.py
--rw-r--r--   0        0        0     2907 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/helpers/dbt/__init__.py
--rw-r--r--   0        0        0     1220 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/helpers/dbt/configuration.py
--rw-r--r--   0        0        0     6137 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/helpers/dbt/dbt_utils.py
--rw-r--r--   0        0        0      758 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/helpers/dbt/exceptions.py
--rw-r--r--   0        0        0     3583 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/helpers/dbt/profiles.yml
--rw-r--r--   0        0        0    13032 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/helpers/dbt/runner.py
--rw-r--r--   0        0        0     2373 2023-03-23 14:48:32.571618 dlt-0.2.6a2/dlt/helpers/pandas.py
--rw-r--r--   0        0        0     1035 2023-03-23 14:48:32.571618 dlt-0.2.6a2/dlt/helpers/parquet.py
--rw-r--r--   0        0        0    13371 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/helpers/streamlit.py
--rw-r--r--   0        0        0       31 2023-03-23 14:48:32.571618 dlt-0.2.6a2/dlt/load/__init__.py
--rw-r--r--   0        0        0     1019 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/load/configuration.py
--rw-r--r--   0        0        0     1993 2023-04-05 08:03:40.638919 dlt-0.2.6a2/dlt/load/exceptions.py
--rw-r--r--   0        0        0    19928 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/load/load.py
--rw-r--r--   0        0        0       32 2023-03-23 14:48:32.571618 dlt-0.2.6a2/dlt/normalize/__init__.py
--rw-r--r--   0        0        0     1098 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/normalize/configuration.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.2.6a2/dlt/normalize/exceptions.py
--rw-r--r--   0        0        0    16576 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/normalize/normalize.py
--rw-r--r--   0        0        0     1880 2023-03-23 14:48:32.571618 dlt-0.2.6a2/dlt/pipeline/README.md
--rw-r--r--   0        0        0    13138 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/pipeline/__init__.py
--rw-r--r--   0        0        0     1858 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/pipeline/configuration.py
--rw-r--r--   0        0        0      363 2023-04-22 20:26:30.632198 dlt-0.2.6a2/dlt/pipeline/current.py
--rw-r--r--   0        0        0     4829 2023-03-23 14:48:32.571618 dlt-0.2.6a2/dlt/pipeline/dbt.py
--rw-r--r--   0        0        0     2891 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/pipeline/exceptions.py
--rw-r--r--   0        0        0     8764 2023-05-02 21:05:46.788848 dlt-0.2.6a2/dlt/pipeline/helpers.py
--rw-r--r--   0        0        0      122 2023-04-06 15:27:24.759561 dlt-0.2.6a2/dlt/pipeline/mark.py
--rw-r--r--   0        0        0    56514 2023-05-06 11:07:29.546603 dlt-0.2.6a2/dlt/pipeline/pipeline.py
--rw-r--r--   0        0        0      985 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/pipeline/progress.py
--rw-r--r--   0        0        0     4200 2023-04-10 08:12:53.769595 dlt-0.2.6a2/dlt/pipeline/state_sync.py
--rw-r--r--   0        0        0     7990 2023-04-03 18:50:36.903525 dlt-0.2.6a2/dlt/pipeline/trace.py
--rw-r--r--   0        0        0     4563 2023-04-03 18:50:36.903525 dlt-0.2.6a2/dlt/pipeline/track.py
--rw-r--r--   0        0        0       91 2023-03-23 14:48:32.571618 dlt-0.2.6a2/dlt/pipeline/typing.py
--rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.2.6a2/dlt/py.typed
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.2.6a2/dlt/reflection/__init__.py
--rw-r--r--   0        0        0      563 2023-03-23 14:48:32.571618 dlt-0.2.6a2/dlt/reflection/names.py
--rw-r--r--   0        0        0     5617 2023-05-06 09:23:33.456603 dlt-0.2.6a2/dlt/reflection/script_inspector.py
--rw-r--r--   0        0        0     6186 2023-03-23 14:48:32.571618 dlt-0.2.6a2/dlt/reflection/script_visitor.py
--rw-r--r--   0        0        0      124 2023-05-05 18:33:47.789796 dlt-0.2.6a2/dlt/sources/__init__.py
--rw-r--r--   0        0        0      320 2023-05-06 11:10:16.076603 dlt-0.2.6a2/dlt/sources/credentials.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.2.6a2/dlt/sources/helpers/__init__.py
--rw-r--r--   0        0        0      574 2023-03-23 14:48:37.261618 dlt-0.2.6a2/dlt/sources/helpers/requests/__init__.py
--rw-r--r--   0        0        0     9092 2023-04-24 18:26:21.111453 dlt-0.2.6a2/dlt/sources/helpers/requests/retry.py
--rw-r--r--   0        0        0     1336 2023-03-23 14:48:32.571618 dlt-0.2.6a2/dlt/sources/helpers/requests/session.py
--rw-r--r--   0        0        0      679 2023-04-06 15:27:24.759561 dlt-0.2.6a2/dlt/sources/helpers/transform.py
--rw-r--r--   0        0        0     1125 2023-04-22 20:26:30.632198 dlt-0.2.6a2/dlt/version.py
--rw-r--r--   0        0        0     4056 2023-05-07 18:36:19.729469 dlt-0.2.6a2/pyproject.toml
--rw-r--r--   0        0        0     7395 1970-01-01 00:00:00.000000 dlt-0.2.6a2/setup.py
--rw-r--r--   0        0        0     7323 1970-01-01 00:00:00.000000 dlt-0.2.6a2/PKG-INFO
+-rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.2.7a0/LICENSE.txt
+-rw-r--r--   0        0        0     4214 2023-04-30 21:17:44.388805 dlt-0.2.7a0/README.md
+-rw-r--r--   0        0        0     1711 2023-04-30 21:17:44.388805 dlt-0.2.7a0/dlt/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 21:17:44.388805 dlt-0.2.7a0/dlt/cli/__init__.py
+-rw-r--r--   0        0        0    15909 2023-05-07 23:03:04.659469 dlt-0.2.7a0/dlt/cli/_dlt.py
+-rw-r--r--   0        0        0     3858 2023-05-07 23:03:04.659469 dlt-0.2.7a0/dlt/cli/config_toml_writer.py
+-rw-r--r--   0        0        0    16665 2023-05-14 16:22:17.789348 dlt-0.2.7a0/dlt/cli/deploy_command.py
+-rw-r--r--   0        0        0     1853 2023-04-30 21:17:44.388805 dlt-0.2.7a0/dlt/cli/echo.py
+-rw-r--r--   0        0        0      435 2023-03-23 14:48:32.551618 dlt-0.2.7a0/dlt/cli/exceptions.py
+-rw-r--r--   0        0        0    18832 2023-05-14 16:22:17.769348 dlt-0.2.7a0/dlt/cli/init_command.py
+-rw-r--r--   0        0        0    10489 2023-04-30 21:17:44.388805 dlt-0.2.7a0/dlt/cli/pipeline_command.py
+-rw-r--r--   0        0        0     9422 2023-05-14 16:22:17.789348 dlt-0.2.7a0/dlt/cli/pipeline_files.py
+-rw-r--r--   0        0        0     4510 2023-05-07 23:03:04.659469 dlt-0.2.7a0/dlt/cli/source_detection.py
+-rw-r--r--   0        0        0     1899 2023-04-22 20:26:30.632198 dlt-0.2.7a0/dlt/cli/telemetry_command.py
+-rw-r--r--   0        0        0     3757 2023-04-30 21:17:44.388805 dlt-0.2.7a0/dlt/cli/utils.py
+-rw-r--r--   0        0        0      307 2023-03-23 14:48:32.551618 dlt-0.2.7a0/dlt/common/__init__.py
+-rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.2.7a0/dlt/common/arithmetics.py
+-rw-r--r--   0        0        0      428 2023-03-23 14:48:32.551618 dlt-0.2.7a0/dlt/common/configuration/__init__.py
+-rw-r--r--   0        0        0     4243 2023-05-11 21:59:36.410516 dlt-0.2.7a0/dlt/common/configuration/accessors.py
+-rw-r--r--   0        0        0     3469 2023-05-07 23:03:04.659469 dlt-0.2.7a0/dlt/common/configuration/container.py
+-rw-r--r--   0        0        0     5884 2023-04-22 20:26:30.632198 dlt-0.2.7a0/dlt/common/configuration/exceptions.py
+-rw-r--r--   0        0        0     7912 2023-04-22 20:26:30.632198 dlt-0.2.7a0/dlt/common/configuration/inject.py
+-rw-r--r--   0        0        0     1791 2023-05-14 16:22:32.439349 dlt-0.2.7a0/dlt/common/configuration/paths.py
+-rw-r--r--   0        0        0      306 2023-05-07 23:03:04.659469 dlt-0.2.7a0/dlt/common/configuration/providers/__init__.py
+-rw-r--r--   0        0        0     1108 2023-04-26 11:34:23.292768 dlt-0.2.7a0/dlt/common/configuration/providers/airflow.py
+-rw-r--r--   0        0        0     1116 2023-05-07 23:03:04.659469 dlt-0.2.7a0/dlt/common/configuration/providers/context.py
+-rw-r--r--   0        0        0     1335 2023-05-07 23:03:04.659469 dlt-0.2.7a0/dlt/common/configuration/providers/dictionary.py
+-rw-r--r--   0        0        0     1981 2023-05-07 23:03:04.659469 dlt-0.2.7a0/dlt/common/configuration/providers/environ.py
+-rw-r--r--   0        0        0     9441 2023-05-08 12:15:33.980224 dlt-0.2.7a0/dlt/common/configuration/providers/google_secrets.py
+-rw-r--r--   0        0        0     1108 2023-05-07 23:03:04.659469 dlt-0.2.7a0/dlt/common/configuration/providers/provider.py
+-rw-r--r--   0        0        0     5237 2023-05-14 16:16:41.679349 dlt-0.2.7a0/dlt/common/configuration/providers/toml.py
+-rw-r--r--   0        0        0    17262 2023-05-11 21:40:17.390516 dlt-0.2.7a0/dlt/common/configuration/resolve.py
+-rw-r--r--   0        0        0     1176 2023-05-07 23:03:04.659469 dlt-0.2.7a0/dlt/common/configuration/specs/__init__.py
+-rw-r--r--   0        0        0     1817 2023-05-07 23:03:04.659469 dlt-0.2.7a0/dlt/common/configuration/specs/api_credentials.py
+-rw-r--r--   0        0        0    13108 2023-05-07 23:03:04.659469 dlt-0.2.7a0/dlt/common/configuration/specs/base_configuration.py
+-rw-r--r--   0        0        0     5521 2023-05-14 17:53:31.839348 dlt-0.2.7a0/dlt/common/configuration/specs/config_providers_context.py
+-rw-r--r--   0        0        0     2792 2023-03-23 14:48:32.551618 dlt-0.2.7a0/dlt/common/configuration/specs/config_section_context.py
+-rw-r--r--   0        0        0     1798 2023-05-07 23:03:04.669469 dlt-0.2.7a0/dlt/common/configuration/specs/connection_string_credentials.py
+-rw-r--r--   0        0        0     2125 2023-04-24 18:26:21.111453 dlt-0.2.7a0/dlt/common/configuration/specs/exceptions.py
+-rw-r--r--   0        0        0    12725 2023-05-07 23:03:04.669469 dlt-0.2.7a0/dlt/common/configuration/specs/gcp_credentials.py
+-rw-r--r--   0        0        0      725 2023-05-07 23:03:04.669469 dlt-0.2.7a0/dlt/common/configuration/specs/known_sections.py
+-rw-r--r--   0        0        0      556 2023-03-23 14:48:32.551618 dlt-0.2.7a0/dlt/common/configuration/specs/load_volume_configuration.py
+-rw-r--r--   0        0        0      417 2023-03-23 14:48:32.551618 dlt-0.2.7a0/dlt/common/configuration/specs/normalize_volume_configuration.py
+-rw-r--r--   0        0        0     2455 2023-04-30 21:17:44.388805 dlt-0.2.7a0/dlt/common/configuration/specs/run_configuration.py
+-rw-r--r--   0        0        0      944 2023-03-23 14:48:32.551618 dlt-0.2.7a0/dlt/common/configuration/specs/schema_volume_configuration.py
+-rw-r--r--   0        0        0     6026 2023-05-07 23:03:04.669469 dlt-0.2.7a0/dlt/common/configuration/utils.py
+-rw-r--r--   0        0        0      142 2023-03-23 14:48:32.551618 dlt-0.2.7a0/dlt/common/data_types/__init__.py
+-rw-r--r--   0        0        0     6306 2023-03-23 14:48:32.551618 dlt-0.2.7a0/dlt/common/data_types/type_helpers.py
+-rw-r--r--   0        0        0      214 2023-03-23 14:48:32.551618 dlt-0.2.7a0/dlt/common/data_types/typing.py
+-rw-r--r--   0        0        0      260 2023-03-23 14:48:20.701618 dlt-0.2.7a0/dlt/common/data_writers/__init__.py
+-rw-r--r--   0        0        0     5893 2023-03-23 14:48:32.551618 dlt-0.2.7a0/dlt/common/data_writers/buffered.py
+-rw-r--r--   0        0        0     2395 2023-03-23 14:48:32.551618 dlt-0.2.7a0/dlt/common/data_writers/escape.py
+-rw-r--r--   0        0        0      962 2023-03-23 14:48:32.551618 dlt-0.2.7a0/dlt/common/data_writers/exceptions.py
+-rw-r--r--   0        0        0     5159 2023-03-23 14:48:32.551618 dlt-0.2.7a0/dlt/common/data_writers/writers.py
+-rw-r--r--   0        0        0       97 2023-03-23 14:48:32.551618 dlt-0.2.7a0/dlt/common/destination/__init__.py
+-rw-r--r--   0        0        0     2206 2023-04-05 08:03:40.638919 dlt-0.2.7a0/dlt/common/destination/capabilities.py
+-rw-r--r--   0        0        0    10682 2023-04-24 11:35:34.867759 dlt-0.2.7a0/dlt/common/destination/reference.py
+-rw-r--r--   0        0        0     6121 2023-04-30 21:17:44.388805 dlt-0.2.7a0/dlt/common/exceptions.py
+-rw-r--r--   0        0        0     4954 2023-03-23 14:48:32.551618 dlt-0.2.7a0/dlt/common/git.py
+-rw-r--r--   0        0        0     5248 2023-04-10 08:12:53.759595 dlt-0.2.7a0/dlt/common/json/__init__.py
+-rw-r--r--   0        0        0     1802 2023-04-10 08:12:53.769595 dlt-0.2.7a0/dlt/common/json/_orjson.py
+-rw-r--r--   0        0        0     2939 2023-04-10 08:12:53.769595 dlt-0.2.7a0/dlt/common/json/_simplejson.py
+-rw-r--r--   0        0        0     1536 2023-04-29 12:58:55.943219 dlt-0.2.7a0/dlt/common/jsonpath.py
+-rw-r--r--   0        0        0      232 2023-03-23 14:48:32.551618 dlt-0.2.7a0/dlt/common/normalizers/__init__.py
+-rw-r--r--   0        0        0     1197 2023-05-07 23:03:04.669469 dlt-0.2.7a0/dlt/common/normalizers/configuration.py
+-rw-r--r--   0        0        0      472 2023-03-23 14:48:32.551618 dlt-0.2.7a0/dlt/common/normalizers/exceptions.py
+-rw-r--r--   0        0        0     1644 2023-04-06 15:27:24.759561 dlt-0.2.7a0/dlt/common/normalizers/json/__init__.py
+-rw-r--r--   0        0        0    13382 2023-05-14 10:08:46.250838 dlt-0.2.7a0/dlt/common/normalizers/json/relational.py
+-rw-r--r--   0        0        0       64 2023-03-23 14:48:32.551618 dlt-0.2.7a0/dlt/common/normalizers/naming/__init__.py
+-rw-r--r--   0        0        0      807 2023-03-23 14:48:32.551618 dlt-0.2.7a0/dlt/common/normalizers/naming/direct.py
+-rw-r--r--   0        0        0     1069 2023-03-23 14:48:32.551618 dlt-0.2.7a0/dlt/common/normalizers/naming/duck_case.py
+-rw-r--r--   0        0        0      792 2023-03-23 14:48:32.551618 dlt-0.2.7a0/dlt/common/normalizers/naming/exceptions.py
+-rw-r--r--   0        0        0     3753 2023-04-05 08:03:40.638919 dlt-0.2.7a0/dlt/common/normalizers/naming/naming.py
+-rw-r--r--   0        0        0     3002 2023-03-23 14:48:32.551618 dlt-0.2.7a0/dlt/common/normalizers/naming/snake_case.py
+-rw-r--r--   0        0        0      358 2023-04-02 09:09:15.855769 dlt-0.2.7a0/dlt/common/normalizers/typing.py
+-rw-r--r--   0        0        0     2337 2023-04-06 15:27:24.759561 dlt-0.2.7a0/dlt/common/normalizers/utils.py
+-rw-r--r--   0        0        0      451 2023-03-23 14:48:32.551618 dlt-0.2.7a0/dlt/common/pendulum.py
+-rw-r--r--   0        0        0    16937 2023-05-14 16:06:45.749348 dlt-0.2.7a0/dlt/common/pipeline.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.551618 dlt-0.2.7a0/dlt/common/reflection/__init__.py
+-rw-r--r--   0        0        0      374 2023-03-23 14:48:32.551618 dlt-0.2.7a0/dlt/common/reflection/function_visitor.py
+-rw-r--r--   0        0        0     4891 2023-04-09 16:39:04.593180 dlt-0.2.7a0/dlt/common/reflection/spec.py
+-rw-r--r--   0        0        0     5069 2023-04-24 18:26:21.111453 dlt-0.2.7a0/dlt/common/reflection/utils.py
+-rw-r--r--   0        0        0      174 2023-04-30 21:17:44.388805 dlt-0.2.7a0/dlt/common/runners/__init__.py
+-rw-r--r--   0        0        0      508 2023-04-30 21:17:44.388805 dlt-0.2.7a0/dlt/common/runners/configuration.py
+-rw-r--r--   0        0        0     2635 2023-05-14 11:08:47.420838 dlt-0.2.7a0/dlt/common/runners/pool_runner.py
+-rw-r--r--   0        0        0     4046 2023-03-23 14:48:32.561618 dlt-0.2.7a0/dlt/common/runners/runnable.py
+-rw-r--r--   0        0        0     3145 2023-03-23 14:48:32.561618 dlt-0.2.7a0/dlt/common/runners/stdout.py
+-rw-r--r--   0        0        0     2137 2023-03-23 14:48:32.561618 dlt-0.2.7a0/dlt/common/runners/synth_pickle.py
+-rw-r--r--   0        0        0      105 2023-04-30 21:17:44.388805 dlt-0.2.7a0/dlt/common/runners/typing.py
+-rw-r--r--   0        0        0     5590 2023-05-07 23:03:04.669469 dlt-0.2.7a0/dlt/common/runners/venv.py
+-rw-r--r--   0        0        0       36 2023-04-30 21:17:44.398805 dlt-0.2.7a0/dlt/common/runtime/__init__.py
+-rw-r--r--   0        0        0    13441 2023-04-30 21:17:44.398805 dlt-0.2.7a0/dlt/common/runtime/collector.py
+-rw-r--r--   0        0        0     4501 2023-05-13 12:04:06.827355 dlt-0.2.7a0/dlt/common/runtime/exec_info.py
+-rw-r--r--   0        0        0      647 2023-04-30 21:17:44.398805 dlt-0.2.7a0/dlt/common/runtime/init.py
+-rw-r--r--   0        0        0     4002 2023-04-30 21:17:44.398805 dlt-0.2.7a0/dlt/common/runtime/logger.py
+-rw-r--r--   0        0        0     2052 2023-04-30 21:17:44.398805 dlt-0.2.7a0/dlt/common/runtime/prometheus.py
+-rw-r--r--   0        0        0     7170 2023-05-14 16:06:45.749348 dlt-0.2.7a0/dlt/common/runtime/segment.py
+-rw-r--r--   0        0        0     2493 2023-04-30 21:17:44.398805 dlt-0.2.7a0/dlt/common/runtime/sentry.py
+-rw-r--r--   0        0        0     2027 2023-04-30 21:17:44.398805 dlt-0.2.7a0/dlt/common/runtime/signals.py
+-rw-r--r--   0        0        0      616 2023-04-03 18:50:36.893525 dlt-0.2.7a0/dlt/common/runtime/slack.py
+-rw-r--r--   0        0        0      720 2023-04-30 21:17:44.398805 dlt-0.2.7a0/dlt/common/runtime/telemetry.py
+-rw-r--r--   0        0        0      387 2023-04-03 18:50:36.893525 dlt-0.2.7a0/dlt/common/schema/__init__.py
+-rw-r--r--   0        0        0     1927 2023-03-23 14:48:32.561618 dlt-0.2.7a0/dlt/common/schema/detections.py
+-rw-r--r--   0        0        0     2974 2023-03-23 14:48:32.561618 dlt-0.2.7a0/dlt/common/schema/exceptions.py
+-rw-r--r--   0        0        0    25175 2023-04-09 16:39:04.593180 dlt-0.2.7a0/dlt/common/schema/schema.py
+-rw-r--r--   0        0        0     3004 2023-04-22 20:26:30.632198 dlt-0.2.7a0/dlt/common/schema/typing.py
+-rw-r--r--   0        0        0    23087 2023-04-30 21:17:44.398805 dlt-0.2.7a0/dlt/common/schema/utils.py
+-rw-r--r--   0        0        0      410 2023-03-23 14:48:32.561618 dlt-0.2.7a0/dlt/common/storages/__init__.py
+-rw-r--r--   0        0        0     1906 2023-03-23 14:48:32.561618 dlt-0.2.7a0/dlt/common/storages/data_item_storage.py
+-rw-r--r--   0        0        0     2804 2023-04-03 18:50:36.893525 dlt-0.2.7a0/dlt/common/storages/exceptions.py
+-rw-r--r--   0        0        0    10891 2023-05-14 17:32:51.649349 dlt-0.2.7a0/dlt/common/storages/file_storage.py
+-rw-r--r--   0        0        0     2685 2023-04-13 08:33:43.967587 dlt-0.2.7a0/dlt/common/storages/live_schema_storage.py
+-rw-r--r--   0        0        0    21806 2023-05-14 11:49:03.530838 dlt-0.2.7a0/dlt/common/storages/load_storage.py
+-rw-r--r--   0        0        0     2414 2023-03-23 14:48:32.561618 dlt-0.2.7a0/dlt/common/storages/normalize_storage.py
+-rw-r--r--   0        0        0     8508 2023-03-23 14:48:32.561618 dlt-0.2.7a0/dlt/common/storages/schema_storage.py
+-rw-r--r--   0        0        0     2525 2023-04-24 18:26:21.111453 dlt-0.2.7a0/dlt/common/storages/versioned_storage.py
+-rw-r--r--   0        0        0     2634 2023-05-07 23:03:04.669469 dlt-0.2.7a0/dlt/common/time.py
+-rw-r--r--   0        0        0     4736 2023-04-03 18:50:36.893525 dlt-0.2.7a0/dlt/common/typing.py
+-rw-r--r--   0        0        0    11275 2023-04-24 18:26:21.111453 dlt-0.2.7a0/dlt/common/utils.py
+-rw-r--r--   0        0        0     3686 2023-03-23 14:48:32.561618 dlt-0.2.7a0/dlt/common/validation.py
+-rw-r--r--   0        0        0     1185 2023-03-23 14:48:32.561618 dlt-0.2.7a0/dlt/common/wei.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.561618 dlt-0.2.7a0/dlt/destinations/__init__.py
+-rw-r--r--   0        0        0      437 2023-03-23 14:48:32.561618 dlt-0.2.7a0/dlt/destinations/bigquery/README.md
+-rw-r--r--   0        0        0     1813 2023-04-05 08:03:40.638919 dlt-0.2.7a0/dlt/destinations/bigquery/__init__.py
+-rw-r--r--   0        0        0    12347 2023-05-07 23:03:04.669469 dlt-0.2.7a0/dlt/destinations/bigquery/bigquery.py
+-rw-r--r--   0        0        0      386 2023-05-07 23:03:04.669469 dlt-0.2.7a0/dlt/destinations/bigquery/configuration.py
+-rw-r--r--   0        0        0    10342 2023-05-07 23:03:04.669469 dlt-0.2.7a0/dlt/destinations/bigquery/sql_client.py
+-rw-r--r--   0        0        0     1935 2023-04-05 08:03:40.638919 dlt-0.2.7a0/dlt/destinations/duckdb/__init__.py
+-rw-r--r--   0        0        0     7008 2023-05-07 23:03:04.669469 dlt-0.2.7a0/dlt/destinations/duckdb/configuration.py
+-rw-r--r--   0        0        0     2754 2023-03-23 14:48:32.561618 dlt-0.2.7a0/dlt/destinations/duckdb/duck.py
+-rw-r--r--   0        0        0     6936 2023-04-21 22:25:54.789942 dlt-0.2.7a0/dlt/destinations/duckdb/sql_client.py
+-rw-r--r--   0        0        0     1671 2023-03-23 14:48:32.561618 dlt-0.2.7a0/dlt/destinations/dummy/__init__.py
+-rw-r--r--   0        0        0      736 2023-04-03 18:50:36.893525 dlt-0.2.7a0/dlt/destinations/dummy/configuration.py
+-rw-r--r--   0        0        0     4975 2023-04-24 11:35:34.867759 dlt-0.2.7a0/dlt/destinations/dummy/dummy.py
+-rw-r--r--   0        0        0     4159 2023-04-05 08:03:40.638919 dlt-0.2.7a0/dlt/destinations/exceptions.py
+-rw-r--r--   0        0        0     4983 2023-04-05 08:03:40.638919 dlt-0.2.7a0/dlt/destinations/insert_job_client.py
+-rw-r--r--   0        0        0    15357 2023-05-07 23:03:04.669469 dlt-0.2.7a0/dlt/destinations/job_client_impl.py
+-rw-r--r--   0        0        0     1303 2023-04-05 08:03:40.638919 dlt-0.2.7a0/dlt/destinations/job_impl.py
+-rw-r--r--   0        0        0      251 2023-03-23 14:48:32.561618 dlt-0.2.7a0/dlt/destinations/postgres/README.md
+-rw-r--r--   0        0        0     1934 2023-04-05 08:03:40.638919 dlt-0.2.7a0/dlt/destinations/postgres/__init__.py
+-rw-r--r--   0        0        0     1232 2023-05-07 23:03:04.669469 dlt-0.2.7a0/dlt/destinations/postgres/configuration.py
+-rw-r--r--   0        0        0     3025 2023-03-23 14:48:32.561618 dlt-0.2.7a0/dlt/destinations/postgres/postgres.py
+-rw-r--r--   0        0        0     6074 2023-05-07 23:03:04.669469 dlt-0.2.7a0/dlt/destinations/postgres/sql_client.py
+-rw-r--r--   0        0        0     1159 2023-04-03 18:50:36.893525 dlt-0.2.7a0/dlt/destinations/redshift/README.md
+-rw-r--r--   0        0        0     1905 2023-04-05 08:03:40.638919 dlt-0.2.7a0/dlt/destinations/redshift/__init__.py
+-rw-r--r--   0        0        0      570 2023-05-07 23:03:04.669469 dlt-0.2.7a0/dlt/destinations/redshift/configuration.py
+-rw-r--r--   0        0        0     3761 2023-03-23 14:48:32.561618 dlt-0.2.7a0/dlt/destinations/redshift/redshift.py
+-rw-r--r--   0        0        0     7110 2023-04-29 12:58:55.953219 dlt-0.2.7a0/dlt/destinations/sql_client.py
+-rw-r--r--   0        0        0    10101 2023-04-09 16:39:04.593180 dlt-0.2.7a0/dlt/destinations/sql_merge_job.py
+-rw-r--r--   0        0        0     1931 2023-04-24 18:26:21.111453 dlt-0.2.7a0/dlt/destinations/typing.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.2.7a0/dlt/extract/__init__.py
+-rw-r--r--   0        0        0    22830 2023-05-09 14:38:16.599571 dlt-0.2.7a0/dlt/extract/decorators.py
+-rw-r--r--   0        0        0    12645 2023-04-30 21:17:44.398805 dlt-0.2.7a0/dlt/extract/exceptions.py
+-rw-r--r--   0        0        0     8449 2023-04-30 21:17:44.398805 dlt-0.2.7a0/dlt/extract/extract.py
+-rw-r--r--   0        0        0    14658 2023-05-07 23:03:04.669469 dlt-0.2.7a0/dlt/extract/incremental.py
+-rw-r--r--   0        0        0    31567 2023-04-30 21:17:44.398805 dlt-0.2.7a0/dlt/extract/pipe.py
+-rw-r--r--   0        0        0     9683 2023-04-22 20:26:30.632198 dlt-0.2.7a0/dlt/extract/schema.py
+-rw-r--r--   0        0        0    34195 2023-05-07 23:03:04.669469 dlt-0.2.7a0/dlt/extract/source.py
+-rw-r--r--   0        0        0     4350 2023-04-22 20:26:30.632198 dlt-0.2.7a0/dlt/extract/typing.py
+-rw-r--r--   0        0        0      593 2023-04-06 20:38:35.239561 dlt-0.2.7a0/dlt/extract/utils.py
+-rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.2.7a0/dlt/helpers/__init__.py
+-rw-r--r--   0        0        0      267 2023-05-14 13:03:58.089348 dlt-0.2.7a0/dlt/helpers/airflow.py
+-rw-r--r--   0        0        0     2907 2023-03-23 14:48:32.561618 dlt-0.2.7a0/dlt/helpers/dbt/__init__.py
+-rw-r--r--   0        0        0     1220 2023-03-23 14:48:32.561618 dlt-0.2.7a0/dlt/helpers/dbt/configuration.py
+-rw-r--r--   0        0        0     6137 2023-03-23 14:48:32.561618 dlt-0.2.7a0/dlt/helpers/dbt/dbt_utils.py
+-rw-r--r--   0        0        0      758 2023-03-23 14:48:32.561618 dlt-0.2.7a0/dlt/helpers/dbt/exceptions.py
+-rw-r--r--   0        0        0     3583 2023-03-23 14:48:32.561618 dlt-0.2.7a0/dlt/helpers/dbt/profiles.yml
+-rw-r--r--   0        0        0    13032 2023-04-30 21:17:44.398805 dlt-0.2.7a0/dlt/helpers/dbt/runner.py
+-rw-r--r--   0        0        0     2490 2023-05-14 17:57:08.929349 dlt-0.2.7a0/dlt/helpers/pandas.py
+-rw-r--r--   0        0        0     1035 2023-03-23 14:48:32.571618 dlt-0.2.7a0/dlt/helpers/parquet.py
+-rw-r--r--   0        0        0    13371 2023-04-30 21:17:44.398805 dlt-0.2.7a0/dlt/helpers/streamlit.py
+-rw-r--r--   0        0        0       31 2023-03-23 14:48:32.571618 dlt-0.2.7a0/dlt/load/__init__.py
+-rw-r--r--   0        0        0     1019 2023-04-30 21:17:44.398805 dlt-0.2.7a0/dlt/load/configuration.py
+-rw-r--r--   0        0        0     1993 2023-04-05 08:03:40.638919 dlt-0.2.7a0/dlt/load/exceptions.py
+-rw-r--r--   0        0        0    19928 2023-04-30 21:17:44.398805 dlt-0.2.7a0/dlt/load/load.py
+-rw-r--r--   0        0        0       32 2023-03-23 14:48:32.571618 dlt-0.2.7a0/dlt/normalize/__init__.py
+-rw-r--r--   0        0        0     1098 2023-04-30 21:17:44.398805 dlt-0.2.7a0/dlt/normalize/configuration.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.2.7a0/dlt/normalize/exceptions.py
+-rw-r--r--   0        0        0    16576 2023-04-30 21:17:44.398805 dlt-0.2.7a0/dlt/normalize/normalize.py
+-rw-r--r--   0        0        0     1880 2023-03-23 14:48:32.571618 dlt-0.2.7a0/dlt/pipeline/README.md
+-rw-r--r--   0        0        0    13138 2023-04-30 21:17:44.398805 dlt-0.2.7a0/dlt/pipeline/__init__.py
+-rw-r--r--   0        0        0     1858 2023-04-30 21:17:44.398805 dlt-0.2.7a0/dlt/pipeline/configuration.py
+-rw-r--r--   0        0        0      363 2023-04-22 20:26:30.632198 dlt-0.2.7a0/dlt/pipeline/current.py
+-rw-r--r--   0        0        0     4829 2023-03-23 14:48:32.571618 dlt-0.2.7a0/dlt/pipeline/dbt.py
+-rw-r--r--   0        0        0     2891 2023-04-30 21:17:44.398805 dlt-0.2.7a0/dlt/pipeline/exceptions.py
+-rw-r--r--   0        0        0     8764 2023-05-07 23:03:04.669469 dlt-0.2.7a0/dlt/pipeline/helpers.py
+-rw-r--r--   0        0        0      122 2023-04-06 15:27:24.759561 dlt-0.2.7a0/dlt/pipeline/mark.py
+-rw-r--r--   0        0        0    56518 2023-05-12 19:49:25.500620 dlt-0.2.7a0/dlt/pipeline/pipeline.py
+-rw-r--r--   0        0        0      985 2023-04-30 21:17:44.398805 dlt-0.2.7a0/dlt/pipeline/progress.py
+-rw-r--r--   0        0        0     4200 2023-04-10 08:12:53.769595 dlt-0.2.7a0/dlt/pipeline/state_sync.py
+-rw-r--r--   0        0        0     7990 2023-04-03 18:50:36.903525 dlt-0.2.7a0/dlt/pipeline/trace.py
+-rw-r--r--   0        0        0     4563 2023-04-03 18:50:36.903525 dlt-0.2.7a0/dlt/pipeline/track.py
+-rw-r--r--   0        0        0       91 2023-03-23 14:48:32.571618 dlt-0.2.7a0/dlt/pipeline/typing.py
+-rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.2.7a0/dlt/py.typed
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.2.7a0/dlt/reflection/__init__.py
+-rw-r--r--   0        0        0      563 2023-03-23 14:48:32.571618 dlt-0.2.7a0/dlt/reflection/names.py
+-rw-r--r--   0        0        0     5617 2023-05-07 23:03:04.669469 dlt-0.2.7a0/dlt/reflection/script_inspector.py
+-rw-r--r--   0        0        0     6186 2023-03-23 14:48:32.571618 dlt-0.2.7a0/dlt/reflection/script_visitor.py
+-rw-r--r--   0        0        0      124 2023-05-07 23:03:04.669469 dlt-0.2.7a0/dlt/sources/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-07 23:03:04.669469 dlt-0.2.7a0/dlt/sources/credentials.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.2.7a0/dlt/sources/helpers/__init__.py
+-rw-r--r--   0        0        0      574 2023-03-23 14:48:37.261618 dlt-0.2.7a0/dlt/sources/helpers/requests/__init__.py
+-rw-r--r--   0        0        0     9106 2023-05-09 21:59:17.759566 dlt-0.2.7a0/dlt/sources/helpers/requests/retry.py
+-rw-r--r--   0        0        0     1336 2023-03-23 14:48:32.571618 dlt-0.2.7a0/dlt/sources/helpers/requests/session.py
+-rw-r--r--   0        0        0      679 2023-04-06 15:27:24.759561 dlt-0.2.7a0/dlt/sources/helpers/transform.py
+-rw-r--r--   0        0        0     1125 2023-04-22 20:26:30.632198 dlt-0.2.7a0/dlt/version.py
+-rw-r--r--   0        0        0     4056 2023-05-14 18:19:56.689349 dlt-0.2.7a0/pyproject.toml
+-rw-r--r--   0        0        0     7371 1970-01-01 00:00:00.000000 dlt-0.2.7a0/setup.py
+-rw-r--r--   0        0        0     7323 1970-01-01 00:00:00.000000 dlt-0.2.7a0/PKG-INFO
```

### Comparing `dlt-0.2.6a2/LICENSE.txt` & `dlt-0.2.7a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/README.md` & `dlt-0.2.7a0/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/__init__.py` & `dlt-0.2.7a0/dlt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/cli/_dlt.py` & `dlt-0.2.7a0/dlt/cli/_dlt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/cli/config_toml_writer.py` & `dlt-0.2.7a0/dlt/cli/config_toml_writer.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/cli/deploy_command.py` & `dlt-0.2.7a0/dlt/cli/deploy_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # import pkg_resources
 import pipdeptree
 
 import dlt
 
 from dlt.common.configuration.exceptions import LookupTrace
 from dlt.common.configuration.providers import ConfigTomlProvider, EnvironProvider, SECRETS_TOML
-from dlt.common.configuration.paths import make_dlt_project_path
+from dlt.common.configuration.paths import make_dlt_settings_path
 from dlt.common.configuration.utils import serialize_value
 from dlt.common.git import get_origin, get_repo, is_dirty
 from dlt.common.configuration.specs.run_configuration import get_default_pipeline_name
 from dlt.common.reflection.utils import evaluate_node_literal
 from dlt.common.pipeline import LoadInfo
 from dlt.common.storages import FileStorage
 from dlt.common.typing import StrAny
@@ -179,15 +179,15 @@
             " You can also run the pipeline manually." if run_on_dispatch else "",
             " Pipeline will also run on each push to the repository." if run_on_push else "",
         ))
         fmt.echo("* The dependencies that will be used to run the pipeline are stored in %s. If you change add more dependencies, remember to refresh your deployment by running the same 'deploy' command again." % fmt.bold(requirements_txt_name))
         fmt.echo()
         fmt.echo("You should now add the secrets to github repository secrets, commit and push the pipeline files to github.")
         fmt.echo("1. Add the following secret values (typically stored in %s): \n%s\nin %s" % (
-            fmt.bold(make_dlt_project_path(SECRETS_TOML)),
+            fmt.bold(make_dlt_settings_path(SECRETS_TOML)),
             fmt.bold("\n".join(env_prov.get_key_name(s_v.key, *s_v.sections) for s_v in secret_envs)),
             fmt.bold(github_origin_to_url(origin, "/settings/secrets/actions"))
         ))
         fmt.echo()
         # if fmt.confirm("Do you want to list the values of the secrets in the format suitable for github?", default=True):
         for s_v in secret_envs:
             fmt.secho("Name:", fg="green")
```

### Comparing `dlt-0.2.6a2/dlt/cli/echo.py` & `dlt-0.2.7a0/dlt/cli/echo.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/cli/init_command.py` & `dlt-0.2.7a0/dlt/cli/init_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import os
 import ast
 import shutil
 from types import ModuleType
 from typing import Dict, List, Sequence, Tuple
 from importlib.metadata import version as pkg_version
-from dlt.cli.telemetry_command import telemetry_status_command
 
 from dlt.common import git
-from dlt.common.configuration.paths import get_dlt_project_dir, make_dlt_project_path
+from dlt.common.configuration.paths import get_dlt_settings_dir, make_dlt_settings_path
 from dlt.common.configuration.specs import known_sections
 from dlt.common.configuration.providers import CONFIG_TOML, SECRETS_TOML, ConfigTomlProvider, SecretsTomlProvider
 from dlt.common.normalizers import default_normalizers, import_normalizers
 from dlt.common.pipeline import get_dlt_repos_dir
 from dlt.version import DLT_PKG_NAME, __version__
 from dlt.common.destination.reference import DestinationReference
 from dlt.common.reflection.utils import rewrite_python_script
@@ -119,15 +118,15 @@
         if is_new_pipeline:
             fmt.echo("Pipeline %s was added to your project!" % fmt.bold(pipeline_name))
             fmt.echo("* See the usage examples and code snippets to copy from %s" % fmt.bold(pipeline_files.dest_pipeline_script))
         else:
             fmt.echo("Pipeline %s was updated to the newest version!" % fmt.bold(pipeline_name))
 
     if is_new_pipeline:
-        fmt.echo("* Add credentials for %s and other secrets in %s" % (fmt.bold(destination_name), fmt.bold(make_dlt_project_path(SECRETS_TOML))))
+        fmt.echo("* Add credentials for %s and other secrets in %s" % (fmt.bold(destination_name), fmt.bold(make_dlt_settings_path(SECRETS_TOML))))
 
     if dependency_system:
         fmt.echo("* Add the required dependencies to %s:" % fmt.bold(dependency_system))
         for dep in pipeline_files.requirements:
             fmt.echo("  " + fmt.bold(dep))
         fmt.echo("  If the dlt dependency is already added, make sure you install the extra for %s to it" % fmt.bold(destination_name))
         if dependency_system == utils.REQUIREMENTS_TXT:
@@ -164,16 +163,16 @@
     # copy pipeline files from here
     pipelines_storage = FileStorage(clone_storage.make_full_path(PIPELINES_MODULE_NAME))
     # load init module and get init files and script
     init_module = load_script_module(clone_storage.storage_path, INIT_MODULE_NAME)
     pipeline_script, template_files = _get_template_files(init_module, use_generic_template)
     # prepare destination storage
     dest_storage = FileStorage(os.path.abspath("."))
-    if not dest_storage.has_folder(get_dlt_project_dir()):
-        dest_storage.create_folder(get_dlt_project_dir())
+    if not dest_storage.has_folder(get_dlt_settings_dir()):
+        dest_storage.create_folder(get_dlt_settings_dir())
     # get local index of pipeline files
     local_index = files_ops.load_pipeline_local_index(pipeline_name)
     # folder deleted at dest - full refresh
     if not dest_storage.has_folder(pipeline_name):
         local_index["files"] = {}
     # is update or new pipeline
     is_new_pipeline = len(local_index["files"]) == 0
@@ -219,15 +218,15 @@
         dest_pipeline_script = norm_source_name + ".py"
         pipeline_files = PipelineFiles(True, init_storage, pipeline_script, dest_pipeline_script, template_files, [], "")
         if dest_storage.has_file(dest_pipeline_script):
             fmt.warning("Pipeline script %s already exist, exiting" % dest_pipeline_script)
             return
 
     # add .dlt/*.toml files to be copied
-    pipeline_files.files.extend([make_dlt_project_path(CONFIG_TOML), make_dlt_project_path(SECRETS_TOML)])
+    pipeline_files.files.extend([make_dlt_settings_path(CONFIG_TOML), make_dlt_settings_path(SECRETS_TOML)])
 
     # add dlt extras line to requirements
     req_dep = f"{DLT_PKG_NAME}[{destination_name}]"
     req_dep_line = f"{req_dep}>={pkg_version(DLT_PKG_NAME)}"
     pipeline_files.requirements.insert(0, req_dep_line)
 
     # read module source and parse it
```

### Comparing `dlt-0.2.6a2/dlt/cli/pipeline_command.py` & `dlt-0.2.7a0/dlt/cli/pipeline_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/cli/pipeline_files.py` & `dlt-0.2.7a0/dlt/cli/pipeline_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import yaml
 import posixpath
 from pathlib import Path
 from typing import Dict, NamedTuple, Sequence, Tuple, TypedDict, List
 from dlt.cli.exceptions import PipelineRepoError
 
 from dlt.common import git
-from dlt.common.configuration.paths import make_dlt_project_path
+from dlt.common.configuration.paths import make_dlt_settings_path
 from dlt.common.storages import FileStorage
 
 from dlt.common.reflection.utils import get_module_docstring
 
 from dlt.cli import utils
 
 
@@ -47,21 +47,21 @@
 
 class TPipelinesFileIndex(TypedDict):
     engine_version: int
     pipelines: Dict[str, TPipelineFileIndex]
 
 
 def _save_dot_pipelines(index: TPipelinesFileIndex) -> None:
-    with open(make_dlt_project_path(PIPELINES_INIT_INFO_FILE), "w", encoding="utf-8") as f:
+    with open(make_dlt_settings_path(PIPELINES_INIT_INFO_FILE), "w", encoding="utf-8") as f:
         yaml.dump(index, f, allow_unicode=True, default_flow_style=False, sort_keys=False)
 
 
 def _load_dot_pipelines() -> TPipelinesFileIndex:
     try:
-        with open(make_dlt_project_path(PIPELINES_INIT_INFO_FILE), "r", encoding="utf-8") as f:
+        with open(make_dlt_settings_path(PIPELINES_INIT_INFO_FILE), "r", encoding="utf-8") as f:
             index: TPipelinesFileIndex = yaml.safe_load(f)
             if not index:
                 raise FileNotFoundError(PIPELINES_INIT_INFO_FILE)
             return index
     except FileNotFoundError:
         return {
             "engine_version": PIPELINES_INIT_INFO_ENGINE_VERSION,
```

### Comparing `dlt-0.2.6a2/dlt/cli/source_detection.py` & `dlt-0.2.7a0/dlt/cli/source_detection.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/cli/telemetry_command.py` & `dlt-0.2.7a0/dlt/cli/telemetry_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/cli/utils.py` & `dlt-0.2.7a0/dlt/cli/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/arithmetics.py` & `dlt-0.2.7a0/dlt/common/arithmetics.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/configuration/accessors.py` & `dlt-0.2.7a0/dlt/common/configuration/accessors.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,16 @@
         type_hint = type_hint or self.default_type
         # split field into sections and a key
         sections = field.split(".")
         key = sections.pop()
         value = None
         traces: List[LookupTrace] = []
         for provider in self.config_providers:
+            if provider.is_empty:
+                continue
             value, effective_field = provider.get_value(key, type_hint, None, *sections)
             trace = LookupTrace(provider.name, sections, effective_field, value)
             traces.append(trace)
             if value is not None:
                 # log trace
                 if is_base_configuration_inner_hint(type_hint):
                     config: BaseConfiguration = type_hint  # type: ignore
```

### Comparing `dlt-0.2.6a2/dlt/common/configuration/container.py` & `dlt-0.2.7a0/dlt/common/configuration/container.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/configuration/exceptions.py` & `dlt-0.2.7a0/dlt/common/configuration/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/configuration/inject.py` & `dlt-0.2.7a0/dlt/common/configuration/inject.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/configuration/paths.py` & `dlt-0.2.7a0/dlt/common/configuration/paths.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,45 @@
 import os
 import tempfile
 
+# dlt settings folder
 DOT_DLT = ".dlt"
 
+# dlt data dir is by default not set, see get_dlt_data_dir for details
+DLT_DATA_DIR: str = None
+
 
 def get_dlt_project_dir() -> str:
-    """Returns the dlt project folder. The path is always relative to the current working directory."""
-    return os.path.join(".", DOT_DLT)
+    """The dlt project dir is the current working directory but may be overridden by DLT_PROJECT_DIR env variable."""
+    return os.environ.get("DLT_PROJECT_DIR", ".")
+
+
+def get_dlt_settings_dir() -> str:
+    """Returns a path to dlt settings directory. If not overridden it resides in current working directory
+
+    The name of the setting folder is '.dlt'. The path is current working directory '.' but may be overridden by DLT_PROJECT_DIR env variable.
+    """
+    return os.path.join(get_dlt_project_dir(), DOT_DLT)
 
 
-def make_dlt_project_path(path: str) -> str:
-    """Returns path to file in dlt project folder. The path is always relative to the current working directory"""
-    return os.path.join(DOT_DLT, path)
+def make_dlt_settings_path(path: str) -> str:
+    """Returns path to file in dlt settings folder."""
+    return os.path.join(get_dlt_settings_dir(), path)
 
 
-def get_dlt_home_dir() -> str:
+def get_dlt_data_dir() -> str:
     """ Gets default directory where pipelines' data will be stored
-        1. in user home directory ~/.dlt/
-        2. if current user is root in /var/dlt/
-        3. if current user does not have a home directory in /tmp/dlt/
+        1. in user home directory: ~/.dlt/
+        2. if current user is root: in /var/dlt/
+        3. if current user does not have a home directory: in /tmp/dlt/
+        4. if DLT_DATA_DIR is set in env then it is used
     """
+    if "DLT_DATA_DIR" in os.environ:
+        return os.environ["DLT_DATA_DIR"]
+
     # getuid not available on Windows
     if hasattr(os, "getuid") and os.geteuid() == 0:
         # we are root so use standard /var
         return os.path.join("/var", "dlt")
 
     home = _get_user_home_dir()
     if home is None:
```

### Comparing `dlt-0.2.6a2/dlt/common/configuration/providers/airflow.py` & `dlt-0.2.7a0/dlt/common/configuration/providers/airflow.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/configuration/providers/context.py` & `dlt-0.2.7a0/dlt/common/configuration/providers/context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/configuration/providers/dictionary.py` & `dlt-0.2.7a0/dlt/common/configuration/providers/dictionary.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/configuration/providers/environ.py` & `dlt-0.2.7a0/dlt/common/configuration/providers/environ.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/configuration/providers/google_secrets.py` & `dlt-0.2.7a0/dlt/common/configuration/providers/google_secrets.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,14 @@
         """Initializes provider with service account credentials and loads `dlt_secrets_toml` as `toml` document.
 
         In order to enable service account to read google manager secrets:
         - enable Google Secrets Manager api in your project
         - add roles/secretmanager.secretAccessor to allow access to all secrets or enable access per secret
 
         """
-        print("GoogleSecretsProvider INSTANCE CREATED!")
         self.only_secrets = only_secrets
         self.only_toml_fragments = only_toml_fragments
         self.credentials = credentials
         self._vault_lookups: Dict[str, pendulum.DateTime] = {}
 
         super().__init__(tomlkit.document())
         self._update_from_vault("dlt_secrets_toml", None, AnyType, None, ())
```

### Comparing `dlt-0.2.6a2/dlt/common/configuration/providers/provider.py` & `dlt-0.2.7a0/dlt/common/configuration/providers/provider.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/configuration/providers/toml.py` & `dlt-0.2.7a0/dlt/common/configuration/providers/toml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import tomlkit
 from tomlkit.items import Item as TOMLItem
 from tomlkit.container import Container as TOMLContainer
 from typing import Any, Optional, Tuple, Type, Union
 
-from dlt.common.configuration.paths import get_dlt_project_dir, get_dlt_home_dir
+from dlt.common.configuration.paths import get_dlt_settings_dir, get_dlt_data_dir
 from dlt.common.utils import update_dict_nested
 
 from .provider import ConfigProvider, ConfigProviderException, get_key_name
 
 CONFIG_TOML = "config.toml"
 SECRETS_TOML = "secrets.toml"
 
@@ -63,28 +63,28 @@
             TomlProviderReadException: File could not be read, most probably `toml` parsing error
         """
         toml_document = self._read_toml_file(file_name, project_dir, add_global_config)
         super().__init__(toml_document)
 
     def _read_toml_file(self, file_name: str, project_dir: str = None, add_global_config: bool = False) -> tomlkit.TOMLDocument:
         self._file_name = file_name
-        self._toml_path = os.path.join(project_dir or get_dlt_project_dir(), file_name)
+        self._toml_path = os.path.join(project_dir or get_dlt_settings_dir(), file_name)
         self._add_global_config = add_global_config
         try:
             project_toml = self._read_toml(self._toml_path)
             if add_global_config:
                 global_toml = self._read_toml(os.path.join(self.global_config_path(), file_name))
                 project_toml = update_dict_nested(global_toml, project_toml)
             return project_toml
         except Exception as ex:
             raise TomlProviderReadException(self.name, file_name, self._toml_path, str(ex))
 
     @staticmethod
     def global_config_path() -> str:
-        return get_dlt_home_dir()
+        return get_dlt_data_dir()
 
     def write_toml(self) -> None:
         assert not self._add_global_config, "Will not write configs when `add_global_config` flag was set"
         with open(self._toml_path, "w", encoding="utf-8") as f:
             tomlkit.dump(self._toml, f)
 
     @staticmethod
```

### Comparing `dlt-0.2.6a2/dlt/common/configuration/resolve.py` & `dlt-0.2.7a0/dlt/common/configuration/resolve.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,17 +334,14 @@
             # pass empty sections
             ns = []
 
     value = None
     while True:
         if config_section and provider.supports_sections:
             full_ns = ns.copy()
-            # pipeline, when provided, is the most outer and always present
-            # if pipeline_name:
-            #     full_ns.insert(0, pipeline_name)
             # config section, is always present and innermost
             if config_section:
                 full_ns.append(config_section)
         else:
             full_ns = ns
         value, ns_key = provider.get_value(key, hint, pipeline_name, *full_ns)
         # if secret is obtained from non secret provider, we must fail
```

### Comparing `dlt-0.2.6a2/dlt/common/configuration/specs/__init__.py` & `dlt-0.2.7a0/dlt/common/configuration/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/configuration/specs/api_credentials.py` & `dlt-0.2.7a0/dlt/common/configuration/specs/api_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/configuration/specs/base_configuration.py` & `dlt-0.2.7a0/dlt/common/configuration/specs/base_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/configuration/specs/config_providers_context.py` & `dlt-0.2.7a0/dlt/common/configuration/specs/config_providers_context.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 
 
-from typing import List
+import contextlib
+import io
+from typing import Any, List
 from dlt.common.configuration.exceptions import DuplicateConfigProviderException
 from dlt.common.configuration.providers import ConfigProvider, EnvironProvider, ContextProvider, SecretsTomlProvider, ConfigTomlProvider, GoogleSecretsProvider
 from dlt.common.configuration.specs.base_configuration import ContainerInjectableContext
 from dlt.common.configuration.specs import GcpServiceAccountCredentials, BaseConfiguration, configspec, known_sections
-from dlt.common.runtime.exec_info import is_running_in_airflow_task
+from dlt.common.runtime.exec_info import is_airflow_installed
 
 
 @configspec
 class ConfigProvidersConfiguration(BaseConfiguration):
     enable_airflow_secrets: bool = True
     enable_google_secrets: bool = False
     only_toml_fragments: bool = True
@@ -28,23 +30,31 @@
         super().__init__()
         # add default providers
         self.providers = ConfigProvidersContext.initial_providers()
         # ContextProvider will provide contexts when embedded in configurations
         self.context_provider = ContextProvider()
 
     def add_extras(self) -> None:
-        """Adds extra providers using the initial ones."""
-        self.providers += _extra_providers()
+        """Adds extra providers. Extra providers may use initial providers when setting up"""
+        for provider in _extra_providers():
+            self[provider.name] = provider
 
     def __getitem__(self, name: str) -> ConfigProvider:
         try:
             return next(p for p in self.providers if p.name == name)
         except StopIteration:
             raise KeyError(name)
 
+    def __setitem__(self, name: str, provider: ConfigProvider) -> None:
+        idx = next((i for i, p in enumerate(self.providers) if p.name == name), -1)
+        if idx == -1:
+            self.providers.append(provider)
+        else:
+            self.providers[idx] = provider
+
     def __contains__(self, name: object) -> bool:
         try:
             self.__getitem__(name)  # type: ignore
             return True
         except KeyError:
             return False
 
@@ -84,33 +94,47 @@
 def _airflow_providers() -> List[ConfigProvider]:
     """Returns a list of configuration providers for an Airflow environment.
 
     This function attempts to import Airflow to determine whether it
     is running in an Airflow environment. If Airflow is not installed,
     an empty list is returned. If Airflow is installed, the function
     returns a list containing the Airflow providers.
+
+    Depending on how DAG is defined this function may be called outside of task and
+    task context will be not available. Still we want the provider to function so
+    we just test if Airflow can be imported.
     """
-    if not is_running_in_airflow_task():
+    if not is_airflow_installed():
         return []
 
-    from airflow.models import Variable # noqa
-    from airflow.operators.python import get_current_context  # noqa
+    # hide stdio. airflow typically dumps tons of warnings and deprecations to stdout and stderr
+    with contextlib.redirect_stdout(io.StringIO()), contextlib.redirect_stderr(io.StringIO()):
+        from airflow.models import Variable # noqa
+
+        from dlt.common.configuration.providers.airflow import (
+            AirflowSecretsTomlProvider,
+            AIRFLOW_SECRETS_TOML_VARIABLE_KEY
+        )
 
-    from dlt.common.configuration.providers.airflow import (
-        AirflowSecretsTomlProvider,
-        AIRFLOW_SECRETS_TOML_VARIABLE_KEY
-    )
-
-    secrets_toml_var = Variable.get(
-        AIRFLOW_SECRETS_TOML_VARIABLE_KEY,
-        default_var=None
-    )
+        secrets_toml_var = Variable.get(
+            AIRFLOW_SECRETS_TOML_VARIABLE_KEY,
+            default_var=None
+        )
 
     if secrets_toml_var is not None:
         return [AirflowSecretsTomlProvider()]
     else:
-        ti = get_current_context()["ti"]
-        ti.log.warning(
-            f"Airflow variable '{AIRFLOW_SECRETS_TOML_VARIABLE_KEY}' "
-            "not found. AirflowSecretsTomlProvider will not be used."
-        )
+        message = f"Airflow variable '{AIRFLOW_SECRETS_TOML_VARIABLE_KEY}' not found. AirflowSecretsTomlProvider will not be used."
+        try:
+            # prefer logging to task logger
+            from airflow.operators.python import get_current_context  # noqa
+
+            ti = get_current_context()["ti"]
+            ti.log.warning(message)
+        except Exception:
+            # otherwise log to dlt logger
+            from dlt.common import logger
+            if logger.is_logging():
+                logger.warning(message)
+            else:
+                print(message)
         return []
```

### Comparing `dlt-0.2.6a2/dlt/common/configuration/specs/config_section_context.py` & `dlt-0.2.7a0/dlt/common/configuration/specs/config_section_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/configuration/specs/connection_string_credentials.py` & `dlt-0.2.7a0/dlt/common/configuration/specs/connection_string_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/configuration/specs/exceptions.py` & `dlt-0.2.7a0/dlt/common/configuration/specs/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/configuration/specs/gcp_credentials.py` & `dlt-0.2.7a0/dlt/common/configuration/specs/gcp_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/configuration/specs/known_sections.py` & `dlt-0.2.7a0/dlt/common/configuration/specs/known_sections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/configuration/specs/load_volume_configuration.py` & `dlt-0.2.7a0/dlt/common/configuration/specs/load_volume_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/configuration/specs/run_configuration.py` & `dlt-0.2.7a0/dlt/common/configuration/specs/run_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/configuration/specs/schema_volume_configuration.py` & `dlt-0.2.7a0/dlt/common/configuration/specs/schema_volume_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/configuration/utils.py` & `dlt-0.2.7a0/dlt/common/configuration/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/data_types/type_helpers.py` & `dlt-0.2.7a0/dlt/common/data_types/type_helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/data_writers/buffered.py` & `dlt-0.2.7a0/dlt/common/data_writers/buffered.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/data_writers/escape.py` & `dlt-0.2.7a0/dlt/common/data_writers/escape.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/data_writers/exceptions.py` & `dlt-0.2.7a0/dlt/common/data_writers/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/data_writers/writers.py` & `dlt-0.2.7a0/dlt/common/data_writers/writers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/destination/capabilities.py` & `dlt-0.2.7a0/dlt/common/destination/capabilities.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/destination/reference.py` & `dlt-0.2.7a0/dlt/common/destination/reference.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/exceptions.py` & `dlt-0.2.7a0/dlt/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/git.py` & `dlt-0.2.7a0/dlt/common/git.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/json/__init__.py` & `dlt-0.2.7a0/dlt/common/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/json/_orjson.py` & `dlt-0.2.7a0/dlt/common/json/_orjson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/json/_simplejson.py` & `dlt-0.2.7a0/dlt/common/json/_simplejson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/jsonpath.py` & `dlt-0.2.7a0/dlt/common/jsonpath.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/normalizers/configuration.py` & `dlt-0.2.7a0/dlt/common/normalizers/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/normalizers/json/__init__.py` & `dlt-0.2.7a0/dlt/common/normalizers/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/normalizers/json/relational.py` & `dlt-0.2.7a0/dlt/common/normalizers/json/relational.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,16 +191,16 @@
         table = self.schema.naming.shorten_fragments(*parent_path, *ident_path)
 
         for idx, v in enumerate(seq):
             # yield child table row
             if isinstance(v, dict):
                 yield from self._normalize_row(v, extend, ident_path, parent_path, parent_row_id, idx, _r_lvl)
             elif isinstance(v, list):
-                # normalize lists of lists, we assume all lists in the list have the same type so they should go to the same table
-                yield from self._normalize_list(v, extend, ("list", ), parent_path + ident_path, parent_row_id, _r_lvl + 1)
+                # to normalize lists of lists, we must create a tracking intermediary table by creating a mock row
+                yield from  self._normalize_row({"list": v}, extend, ident_path, parent_path, parent_row_id, idx, _r_lvl + 1)
             else:
                 # list of simple types
                 child_row_hash = DataItemNormalizer._get_child_row_hash(parent_row_id, table, idx)
                 wrap_v = wrap_in_dict(v)
                 wrap_v["_dlt_id"] = child_row_hash
                 e = DataItemNormalizer._link_row(wrap_v, parent_row_id, idx)
                 DataItemNormalizer._extend_row(extend, e)
```

### Comparing `dlt-0.2.6a2/dlt/common/normalizers/naming/direct.py` & `dlt-0.2.7a0/dlt/common/normalizers/naming/direct.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/normalizers/naming/duck_case.py` & `dlt-0.2.7a0/dlt/common/normalizers/naming/duck_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/normalizers/naming/exceptions.py` & `dlt-0.2.7a0/dlt/common/normalizers/naming/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/normalizers/naming/naming.py` & `dlt-0.2.7a0/dlt/common/normalizers/naming/naming.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/normalizers/naming/snake_case.py` & `dlt-0.2.7a0/dlt/common/normalizers/naming/snake_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/normalizers/utils.py` & `dlt-0.2.7a0/dlt/common/normalizers/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/pipeline.py` & `dlt-0.2.7a0/dlt/common/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from dlt.common import pendulum
 from dlt.common.configuration import configspec
 from dlt.common.configuration import known_sections
 from dlt.common.configuration.container import Container
 from dlt.common.configuration.exceptions import ContextDefaultCannotBeCreated
 from dlt.common.configuration.specs import ContainerInjectableContext
 from dlt.common.configuration.specs.config_section_context import ConfigSectionContext
-from dlt.common.configuration.paths import get_dlt_home_dir
+from dlt.common.configuration.paths import get_dlt_data_dir
 from dlt.common.configuration.specs import RunConfiguration
 from dlt.common.destination.reference import DestinationReference, TDestinationReferenceArg
 from dlt.common.exceptions import DestinationHasFailedJobs, PipelineStateNotAvailable, SourceSectionNotAvailable
 from dlt.common.schema import Schema
 from dlt.common.schema.typing import TColumnKey, TColumnSchema, TWriteDisposition
 from dlt.common.storages.load_storage import LoadPackageInfo
 from dlt.common.typing import DictStrAny, REPattern
@@ -389,13 +389,13 @@
 
 def get_dlt_pipelines_dir() -> str:
     """ Gets default directory where pipelines' data will be stored
         1. in user home directory ~/.dlt/pipelines/
         2. if current user is root in /var/dlt/pipelines
         3. if current user does not have a home directory in /tmp/dlt/pipelines
     """
-    return os.path.join(get_dlt_home_dir(), "pipelines")
+    return os.path.join(get_dlt_data_dir(), "pipelines")
 
 
 def get_dlt_repos_dir() -> str:
     """Gets default directory where command repositories will be stored"""
-    return os.path.join(get_dlt_home_dir(), "repos")
+    return os.path.join(get_dlt_data_dir(), "repos")
```

### Comparing `dlt-0.2.6a2/dlt/common/reflection/spec.py` & `dlt-0.2.7a0/dlt/common/reflection/spec.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/reflection/utils.py` & `dlt-0.2.7a0/dlt/common/reflection/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/runners/pool_runner.py` & `dlt-0.2.7a0/dlt/common/runners/pool_runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/runners/runnable.py` & `dlt-0.2.7a0/dlt/common/runners/runnable.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/runners/stdout.py` & `dlt-0.2.7a0/dlt/common/runners/stdout.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/runners/synth_pickle.py` & `dlt-0.2.7a0/dlt/common/runners/synth_pickle.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/runners/venv.py` & `dlt-0.2.7a0/dlt/common/runners/venv.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/runtime/collector.py` & `dlt-0.2.7a0/dlt/common/runtime/collector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/runtime/exec_info.py` & `dlt-0.2.7a0/dlt/common/runtime/exec_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,26 +77,34 @@
 
             get_current_context()
             return {"AIRFLOW_TASK": True}
     except Exception:
         return None
 
 
+def is_airflow_installed() -> bool:
+    try:
+        with contextlib.redirect_stdout(io.StringIO()), contextlib.redirect_stderr(io.StringIO()):
+            import airflow
+        return True
+    except ImportError:
+        return False
+
+
 def is_running_in_airflow_task() -> bool:
     try:
         with contextlib.redirect_stdout(io.StringIO()), contextlib.redirect_stderr(io.StringIO()):
             from airflow.operators.python import get_current_context
 
             context = get_current_context()
             return context is not None and 'ti' in context
     except Exception:
         return False
 
 
-
 def dlt_version_info(pipeline_name: str) -> StrStr:
     """Gets dlt version info including commit and image version available in docker"""
     version_info = {"dlt_version": __version__, "pipeline_name": pipeline_name}
     # extract envs with build info
     version_info.update(filter_env_vars(["COMMIT_SHA", "IMAGE_VERSION"]))
 
     return version_info
```

### Comparing `dlt-0.2.6a2/dlt/common/runtime/init.py` & `dlt-0.2.7a0/dlt/common/runtime/init.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/runtime/logger.py` & `dlt-0.2.7a0/dlt/common/runtime/logger.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/runtime/prometheus.py` & `dlt-0.2.7a0/dlt/common/runtime/prometheus.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/runtime/segment.py` & `dlt-0.2.7a0/dlt/common/runtime/segment.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import multiprocessing
 import atexit
 import base64
 import requests
 import platform
 from concurrent.futures import ThreadPoolExecutor
 from typing import Literal, Optional
-from dlt.common.configuration.paths import get_dlt_home_dir
+from dlt.common.configuration.paths import get_dlt_data_dir
 
 from dlt.common.runtime import logger
 from dlt.common.configuration.specs import RunConfiguration
 from dlt.common.runtime.exec_info import exec_info_names, in_continuous_integration
 from dlt.common.typing import DictStrAny, StrAny
 from dlt.common.utils import uniq_id
 from dlt.version import __version__, DLT_PKG_NAME
@@ -108,15 +108,15 @@
         "Authorization": "Basic {}".format(write_key),
         "Content-Type": "application/json",
     }
 
 
 def get_anonymous_id() -> str:
     """Creates or reads a anonymous user id"""
-    home_dir = get_dlt_home_dir()
+    home_dir = get_dlt_data_dir()
     if not os.path.isdir(home_dir):
         os.makedirs(home_dir, exist_ok=True)
     anonymous_id_file = os.path.join(home_dir, ".anonymous_id")
     if not os.path.isfile(anonymous_id_file):
         anonymous_id = uniq_id()
         with open(anonymous_id_file, "w", encoding="utf-8") as f:
             f.write(anonymous_id)
```

### Comparing `dlt-0.2.6a2/dlt/common/runtime/sentry.py` & `dlt-0.2.7a0/dlt/common/runtime/sentry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/runtime/signals.py` & `dlt-0.2.7a0/dlt/common/runtime/signals.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/runtime/slack.py` & `dlt-0.2.7a0/dlt/common/runtime/slack.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/runtime/telemetry.py` & `dlt-0.2.7a0/dlt/common/runtime/telemetry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/schema/detections.py` & `dlt-0.2.7a0/dlt/common/schema/detections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/schema/exceptions.py` & `dlt-0.2.7a0/dlt/common/schema/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/schema/schema.py` & `dlt-0.2.7a0/dlt/common/schema/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/schema/typing.py` & `dlt-0.2.7a0/dlt/common/schema/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/schema/utils.py` & `dlt-0.2.7a0/dlt/common/schema/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/storages/data_item_storage.py` & `dlt-0.2.7a0/dlt/common/storages/data_item_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/storages/exceptions.py` & `dlt-0.2.7a0/dlt/common/storages/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/storages/file_storage.py` & `dlt-0.2.7a0/dlt/common/storages/file_storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import re
 import stat
+import errno
 import tempfile
 import shutil
 import pathvalidate
 from typing import IO, Any, List
 from dlt.common.typing import AnyFun
 
 from dlt.common.utils import encoding_for_mode, uniq_id
@@ -137,19 +138,64 @@
         # note: some interesting stuff on links https://lightrun.com/answers/conan-io-conan-research-investigate-symlinks-and-hard-links
         os.link(
             self.make_full_path(from_relative_path),
             self.make_full_path(to_relative_path)
         )
 
     def atomic_rename(self, from_relative_path: str, to_relative_path: str) -> None:
+        """Renames a path using os.rename which is atomic on POSIX, Windows and NFS v4.
+
+        Method falls back to non-atomic method in following cases:
+        1. On Windows when destination file exists
+        2. If underlying file system does not support atomic rename
+        3. All buckets mapped with FUSE are not atomic
+        """
+
         os.rename(
             self.make_full_path(from_relative_path),
             self.make_full_path(to_relative_path)
         )
 
+    def rename_tree(self, from_relative_path: str, to_relative_path: str) -> None:
+        """Renames a tree using os.rename if possible making it atomic
+
+        If we get 'too many open files': in that case `rename_tree_files is used
+        """
+
+        try:
+            self.atomic_rename(from_relative_path, to_relative_path)
+            return
+        except OSError as ex:
+            if ex.errno != errno.EMFILE:
+                raise
+        self.rename_tree_files(from_relative_path, to_relative_path)
+
+    def rename_tree_files(self, from_relative_path: str, to_relative_path: str) -> None:
+        """Renames files in a tree recursively using os.rename."""
+        from_path = self.make_full_path(from_relative_path)
+        to_path = self.make_full_path(to_relative_path)
+
+        if not os.path.isdir(from_path):
+            raise ValueError(f"{from_path} is not a directory")
+
+        # make sure the destination directory exists
+        os.makedirs(to_path, exist_ok=True)
+
+        # move files and directories from source to destination starting from leafs
+        for root, _, files in os.walk(from_path, topdown=False):
+            to_root = root.replace(from_path, to_path, 1)
+            os.makedirs(to_root, exist_ok=True)
+
+            for name in files:
+                file_from_path = os.path.join(root, name)
+                os.rename(file_from_path, os.path.join(to_root, name))
+
+            if not os.listdir(root):
+                os.rmdir(root)
+
     def atomic_import(self, external_file_path: str, to_folder: str) -> str:
         """Moves a file at `external_file_path` into the `to_folder` effectively importing file into storage"""
         return self.to_relative_path(FileStorage.copy_atomic(external_file_path, self.make_full_path(to_folder)))
         # file_name = FileStorage.get_file_name_from_file_path(external_path)
         # os.rename(external_path, os.path.join(self.make_full_path(to_folder), file_name))
 
     def in_storage(self, path: str) -> bool:
```

### Comparing `dlt-0.2.6a2/dlt/common/storages/live_schema_storage.py` & `dlt-0.2.7a0/dlt/common/storages/live_schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/storages/load_storage.py` & `dlt-0.2.7a0/dlt/common/storages/load_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
         return self.storage.save(join(load_id, LoadStorage.SCHEMA_FILE_NAME), dump)
 
     def save_temp_schema_updates(self, load_id: str, schema_update: TSchemaTables) -> None:
         with self.storage.open_file(join(load_id, LoadStorage.SCHEMA_UPDATES_FILE_NAME), mode="wb") as f:
             json.dump(schema_update, f)
 
     def commit_temp_load_package(self, load_id: str) -> None:
-        self.storage.atomic_rename(load_id, self.get_package_path(load_id))
+        self.storage.rename_tree(load_id, self.get_package_path(load_id))
 
     def list_packages(self) -> Sequence[str]:
         loads = self.storage.list_folder_dirs(LoadStorage.NORMALIZED_FOLDER, to_root=False)
         # start from the oldest packages
         return sorted(loads)
 
     def list_completed_packages(self) -> Sequence[str]:
@@ -343,15 +343,15 @@
                 self._get_job_folder_path(load_id, LoadStorage.COMPLETED_JOBS_FOLDER),
             recursively=True)
         # save marker file
         completed_state: TLoadPackageState = "aborted" if aborted else "loaded"
         self.storage.save(join(load_path, LoadStorage.PACKAGE_COMPLETED_FILE_NAME), completed_state)
         # move to completed
         completed_path = self.get_completed_package_path(load_id)
-        self.storage.atomic_rename(load_path, completed_path)
+        self.storage.rename_tree(load_path, completed_path)
 
     def delete_completed_package(self, load_id: str) -> None:
         package_path = self.get_completed_package_path(load_id)
         if not self.storage.has_folder(package_path):
             raise LoadPackageNotFound(load_id)
         self.storage.delete_folder(package_path, recursively=True)
```

### Comparing `dlt-0.2.6a2/dlt/common/storages/normalize_storage.py` & `dlt-0.2.7a0/dlt/common/storages/normalize_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/storages/schema_storage.py` & `dlt-0.2.7a0/dlt/common/storages/schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/storages/versioned_storage.py` & `dlt-0.2.7a0/dlt/common/storages/versioned_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/time.py` & `dlt-0.2.7a0/dlt/common/time.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/typing.py` & `dlt-0.2.7a0/dlt/common/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/utils.py` & `dlt-0.2.7a0/dlt/common/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/validation.py` & `dlt-0.2.7a0/dlt/common/validation.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/common/wei.py` & `dlt-0.2.7a0/dlt/common/wei.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/destinations/bigquery/__init__.py` & `dlt-0.2.7a0/dlt/destinations/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/destinations/bigquery/bigquery.py` & `dlt-0.2.7a0/dlt/destinations/bigquery/bigquery.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/destinations/bigquery/sql_client.py` & `dlt-0.2.7a0/dlt/destinations/bigquery/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/destinations/duckdb/__init__.py` & `dlt-0.2.7a0/dlt/destinations/duckdb/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/destinations/duckdb/configuration.py` & `dlt-0.2.7a0/dlt/destinations/duckdb/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/destinations/duckdb/duck.py` & `dlt-0.2.7a0/dlt/destinations/duckdb/duck.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/destinations/duckdb/sql_client.py` & `dlt-0.2.7a0/dlt/destinations/duckdb/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/destinations/dummy/__init__.py` & `dlt-0.2.7a0/dlt/destinations/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/destinations/dummy/configuration.py` & `dlt-0.2.7a0/dlt/destinations/dummy/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/destinations/dummy/dummy.py` & `dlt-0.2.7a0/dlt/destinations/dummy/dummy.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/destinations/exceptions.py` & `dlt-0.2.7a0/dlt/destinations/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/destinations/insert_job_client.py` & `dlt-0.2.7a0/dlt/destinations/insert_job_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/destinations/job_client_impl.py` & `dlt-0.2.7a0/dlt/destinations/job_client_impl.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/destinations/job_impl.py` & `dlt-0.2.7a0/dlt/destinations/job_impl.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/destinations/postgres/__init__.py` & `dlt-0.2.7a0/dlt/destinations/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/destinations/postgres/configuration.py` & `dlt-0.2.7a0/dlt/destinations/postgres/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/destinations/postgres/postgres.py` & `dlt-0.2.7a0/dlt/destinations/postgres/postgres.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/destinations/postgres/sql_client.py` & `dlt-0.2.7a0/dlt/destinations/postgres/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/destinations/redshift/README.md` & `dlt-0.2.7a0/dlt/destinations/redshift/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/destinations/redshift/__init__.py` & `dlt-0.2.7a0/dlt/destinations/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/destinations/redshift/configuration.py` & `dlt-0.2.7a0/dlt/destinations/redshift/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/destinations/redshift/redshift.py` & `dlt-0.2.7a0/dlt/destinations/redshift/redshift.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/destinations/sql_client.py` & `dlt-0.2.7a0/dlt/destinations/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/destinations/sql_merge_job.py` & `dlt-0.2.7a0/dlt/destinations/sql_merge_job.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/destinations/typing.py` & `dlt-0.2.7a0/dlt/destinations/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/extract/decorators.py` & `dlt-0.2.7a0/dlt/extract/decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,15 @@
     table_name: TTableHintTemplate[str] = None,
     write_disposition: TTableHintTemplate[TWriteDisposition] = None,
     columns: TTableHintTemplate[TTableSchemaColumns] = None,
     primary_key: TTableHintTemplate[TColumnKey] = None,
     merge_key: TTableHintTemplate[TColumnKey] = None,
     selected: bool = True,
     spec: Type[BaseConfiguration] = None
-) -> Callable[[Callable[TResourceFunParams, Any]], Callable[TResourceFunParams, DltResource]]:
+) -> Callable[[Callable[TResourceFunParams, Any]], DltResource]:
     ...
 
 
 
 @overload
 def resource(
     data: Union[List[Any], Tuple[Any], Iterator[Any]],
```

### Comparing `dlt-0.2.6a2/dlt/extract/exceptions.py` & `dlt-0.2.7a0/dlt/extract/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/extract/extract.py` & `dlt-0.2.7a0/dlt/extract/extract.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/extract/incremental.py` & `dlt-0.2.7a0/dlt/extract/incremental.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/extract/pipe.py` & `dlt-0.2.7a0/dlt/extract/pipe.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/extract/schema.py` & `dlt-0.2.7a0/dlt/extract/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/extract/source.py` & `dlt-0.2.7a0/dlt/extract/source.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/extract/typing.py` & `dlt-0.2.7a0/dlt/extract/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/extract/utils.py` & `dlt-0.2.7a0/dlt/extract/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/helpers/dbt/__init__.py` & `dlt-0.2.7a0/dlt/helpers/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/helpers/dbt/configuration.py` & `dlt-0.2.7a0/dlt/helpers/dbt/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/helpers/dbt/dbt_utils.py` & `dlt-0.2.7a0/dlt/helpers/dbt/dbt_utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/helpers/dbt/exceptions.py` & `dlt-0.2.7a0/dlt/helpers/dbt/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/helpers/dbt/profiles.yml` & `dlt-0.2.7a0/dlt/helpers/dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/helpers/dbt/runner.py` & `dlt-0.2.7a0/dlt/helpers/dbt/runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/helpers/pandas.py` & `dlt-0.2.7a0/dlt/helpers/pandas.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from typing import Any
 
+from deprecated import deprecated
+
 from dlt.common.exceptions import MissingDependencyException
 from dlt.destinations.sql_client import SqlClientBase
 
 try:
     import pandas as pd
     from pandas.io.sql import _wrap_result
 except ImportError:
     raise MissingDependencyException("DLT Pandas Helpers", ["pandas"])
 
 
-
+@deprecated(reason="Use `df` method on cursor returned from client.execute_query")
 def query_results_to_df(
     client: SqlClientBase[Any], query: str, index_col: Any = None, coerce_float: bool = True, parse_dates: Any = None, dtype: Any = None
 ) -> pd.DataFrame:
     """
     A helper function that executes a query in the destination and returns the result as Pandas `DataFrame`
 
     This method reuses `read_sql` method of `Pandas` with the sql client obtained from `Pipeline.sql_client` method.
```

### Comparing `dlt-0.2.6a2/dlt/helpers/parquet.py` & `dlt-0.2.7a0/dlt/helpers/parquet.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/helpers/streamlit.py` & `dlt-0.2.7a0/dlt/helpers/streamlit.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/load/configuration.py` & `dlt-0.2.7a0/dlt/load/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/load/exceptions.py` & `dlt-0.2.7a0/dlt/load/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/load/load.py` & `dlt-0.2.7a0/dlt/load/load.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/normalize/configuration.py` & `dlt-0.2.7a0/dlt/normalize/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/normalize/normalize.py` & `dlt-0.2.7a0/dlt/normalize/normalize.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/pipeline/README.md` & `dlt-0.2.7a0/dlt/pipeline/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/pipeline/__init__.py` & `dlt-0.2.7a0/dlt/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/pipeline/configuration.py` & `dlt-0.2.7a0/dlt/pipeline/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/pipeline/dbt.py` & `dlt-0.2.7a0/dlt/pipeline/dbt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/pipeline/exceptions.py` & `dlt-0.2.7a0/dlt/pipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/pipeline/helpers.py` & `dlt-0.2.7a0/dlt/pipeline/helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/pipeline/pipeline.py` & `dlt-0.2.7a0/dlt/pipeline/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,15 +306,15 @@
             # shares schema storage with the pipeline so we do not need to install
             normalize = Normalize(collector=self.collector, config=normalize_config, schema_storage=self._schema_storage)
             try:
                 with signals.delayed_signals():
                     runner.run_pool(normalize.config, normalize)
                 return NormalizeInfo()
             except Exception as n_ex:
-                raise PipelineStepFailed(self, "normalize", n_ex, Normalize()) from n_ex
+                raise PipelineStepFailed(self, "normalize", n_ex, NormalizeInfo()) from n_ex
 
     @with_runtime_trace
     @with_schemas_sync
     @with_state_sync()
     @with_config_section((known_sections.LOAD,))
     def load(
         self,
```

### Comparing `dlt-0.2.6a2/dlt/pipeline/progress.py` & `dlt-0.2.7a0/dlt/pipeline/progress.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/pipeline/state_sync.py` & `dlt-0.2.7a0/dlt/pipeline/state_sync.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/pipeline/trace.py` & `dlt-0.2.7a0/dlt/pipeline/trace.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/pipeline/track.py` & `dlt-0.2.7a0/dlt/pipeline/track.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/reflection/names.py` & `dlt-0.2.7a0/dlt/reflection/names.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/reflection/script_inspector.py` & `dlt-0.2.7a0/dlt/reflection/script_inspector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/reflection/script_visitor.py` & `dlt-0.2.7a0/dlt/reflection/script_visitor.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/sources/helpers/requests/__init__.py` & `dlt-0.2.7a0/dlt/sources/helpers/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/sources/helpers/requests/retry.py` & `dlt-0.2.7a0/dlt/sources/helpers/requests/retry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 from email.utils import parsedate_tz, mktime_tz
-from functools import partial, wraps
-import inspect
 import re
 import time
 from typing import Optional, cast, Callable, Type, Union, Sequence, Tuple, List, TYPE_CHECKING, Any
 from threading import local
 
 from requests import Response, HTTPError, ConnectionError, Timeout, Session as BaseSession
 from requests.adapters import HTTPAdapter
@@ -99,20 +97,20 @@
     retry_conds = [retry_if_status(status_codes), retry_if_exception_type(tuple(exceptions))]
     if condition is not None:
         if callable(condition):
             retry_condition = [condition]
         retry_conds.extend([retry_if_predicate(c) for c in retry_condition])
 
     wait_cls = wait_exponential_retry_after if respect_retry_after_header else wait_exponential
-
     return Retrying(
         wait=wait_cls(multiplier=backoff_factor),
         retry=(retry_any(*retry_conds)),
         stop=stop_after_attempt(max_attempts),
-        reraise=True
+        reraise=True,
+        retry_error_callback=lambda state: state.outcome.result()
     )
 
 
 class Client:
     """Wrapper for `requests` to create a `Session` with configurable retry functionality.
 
     ### Summary
```

### Comparing `dlt-0.2.6a2/dlt/sources/helpers/requests/session.py` & `dlt-0.2.7a0/dlt/sources/helpers/requests/session.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/sources/helpers/transform.py` & `dlt-0.2.7a0/dlt/sources/helpers/transform.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/dlt/version.py` & `dlt-0.2.7a0/dlt/version.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a2/pyproject.toml` & `dlt-0.2.7a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dlt"
-version = "0.2.6a2"
+version = "0.2.7a0"
 description = "DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run."
 authors = ["dltHub Inc. <services@dlthub.com>"]
 maintainers = [ "Marcin Rudolf <marcin@dlthub.com>", "Adrian Brudaru <adrian@dlthub.com>", "Ty Dunn <ty@dlthub.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/dlt-hub"
 repository = "https://github.com/dlt-hub/dlt"
```

### Comparing `dlt-0.2.6a2/setup.py` & `dlt-0.2.7a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
  'dlt.destinations.bigquery',
  'dlt.destinations.duckdb',
  'dlt.destinations.dummy',
  'dlt.destinations.postgres',
  'dlt.destinations.redshift',
  'dlt.extract',
  'dlt.helpers',
- 'dlt.helpers.airflow',
  'dlt.helpers.dbt',
  'dlt.load',
  'dlt.normalize',
  'dlt.pipeline',
  'dlt.reflection',
  'dlt.sources',
  'dlt.sources.helpers',
@@ -90,15 +89,15 @@
  'redshift:platform_python_implementation == "PyPy"': ['psycopg2cffi>=2.9.0']}
 
 entry_points = \
 {'console_scripts': ['dlt = dlt.cli._dlt:_main']}
 
 setup_kwargs = {
     'name': 'dlt',
-    'version': '0.2.6a2',
+    'version': '0.2.7a0',
     'description': 'DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.',
     'long_description': '<h1 align="center">\n    <strong>data load tool (dlt) — the open-source Python library for data loading</strong>\n</h1>\n<p align="center">\nBe it a Google Colab notebook, AWS Lambda function, an Airflow DAG, your local laptop,<br/>or a GPT-4 assisted development playground—<strong>dlt</strong> can be dropped in anywhere.\n</p>\n\n<div align="center">\n  <a target="_blank" href="https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g" style="background:none">\n    <img src="https://img.shields.io/badge/slack-join-dlt.svg?labelColor=191937&color=6F6FF7&logo=slack" />\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/v/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/pyversions/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n</div>\n\n## Installation\n\ndlt supports Python 3.8+.\n\n```bash\npip install dlt\n```\n\n## Quick Start\n\nLoad chess game data from chess.com API and save it in DuckDB:\n\n```python\nimport dlt\nfrom chess import chess # a utility function that grabs data from the chess.com API\n\n# create a dlt pipeline that will load chess game data to the DuckDB destination\npipeline = dlt.pipeline(\n    pipeline_name=\'chess_pipeline\',\n    destination=\'duckdb\',\n    dataset_name=\'games_data\'\n)\n\n# use chess.com API to grab data about a few players\ndata = chess([\'magnuscarlsen\', \'rpragchess\'], start_month=\'2022/11\', end_month=\'2022/12\')\n\n# extract, normalize, and load the data\npipeline.run(data)\n```\n\nTry it out in our **[Colab Demo](https://colab.research.google.com/drive/1NfSB1DpwbbHX9_t5vlalBTf13utwpMGx?usp=sharing)**\n\n## Features\n\n- **Automatic Schema:** Data structure inspection and schema creation for the destination.\n- **Data Normalization:** Consistent and verified data before loading.\n- **Seamless Integration:** Colab, AWS Lambda, Airflow, and local environments.\n- **Scalable:** Adapts to growing data needs in production.\n- **Easy Maintenance:** Clear data pipeline structure for updates.\n- **Rapid Exploration:** Quickly explore and gain insights from new data sources.\n- **Versatile Usage:** Suitable for ad-hoc exploration to advanced loading infrastructures.\n- **Start in Seconds with CLI:** Powerful CLI for managing, deploying and inspecting local pipelines.\n- **Incremental Loading:** Load only new or changed data and avoid loading old records again.\n- **Open Source:** Free and Apache 2.0 Licensed.\n\n## Ready to use Pipelines and Destinations\n\nExplore ready to use pipelines (e.g. Google Sheets) in the [Pipelines docs](https://dlthub.com/docs/pipelines/chess) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/destinations/bigquery).\n\n## Documentation\n\nFor detailed usage and configuration, please refer to the [official documentation](https://dlthub.com/docs).\n\n## Examples\n\nYou can find examples for various use cases in the [examples](docs/examples) folder.\n\n## Get Involved\n\nThe dlt project is quickly growing, and we\'re excited to have you join our community! Here\'s how you can get involved:\n\n- **Connect with the Community**: Join other dlt users and contributors on our [Slack](https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g)\n- **Report issues and suggest features**: Please use the [GitHub Issues](https://github.com/dlt-hub/dlt/issues) to report bugs or suggest new features. Before creating a new issue, make sure to search the tracker for possible duplicates and add a comment if you find one.\n- **Contribute Pipelines**: Pipelines are data processing steps that help move and transform data between various sources and destinations. Contribute your custom pipelines to the [dlt-hub/pipelines](https://github.com/dlt-hub/pipelines) to help other folks in handling their data tasks.\n- **Contribute code**: Check out our [contributing guidelines](CONTRIBUTING.md) for information on how to make a pull request.\n- **Improve documentation**: Help us enhance the dlt documentation.\n\n## License\n\nDLT is released under the [Apache 2.0 License](LICENSE.txt).\n',
     'author': 'dltHub Inc.',
     'author_email': 'services@dlthub.com',
     'maintainer': 'Marcin Rudolf',
     'maintainer_email': 'marcin@dlthub.com',
     'url': 'https://github.com/dlt-hub',
```

### Comparing `dlt-0.2.6a2/PKG-INFO` & `dlt-0.2.7a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlt
-Version: 0.2.6a2
+Version: 0.2.7a0
 Summary: DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.
 Home-page: https://github.com/dlt-hub
 License: Apache-2.0
 Keywords: etl
 Author: dltHub Inc.
 Author-email: services@dlthub.com
 Maintainer: Marcin Rudolf
```

