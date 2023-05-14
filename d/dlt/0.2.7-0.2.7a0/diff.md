# Comparing `tmp/dlt-0.2.7.tar.gz` & `tmp/dlt-0.2.7a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlt-0.2.7.tar", max compression
+gzip compressed data, was "dlt-0.2.7a0.tar", max compression
```

## Comparing `dlt-0.2.7.tar` & `dlt-0.2.7a0.tar`

### file list

```diff
@@ -1,209 +1,209 @@
--rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.2.7/LICENSE.txt
--rw-r--r--   0        0        0     4214 2023-04-30 21:17:44.388805 dlt-0.2.7/README.md
--rw-r--r--   0        0        0     1711 2023-04-30 21:17:44.388805 dlt-0.2.7/dlt/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 21:17:44.388805 dlt-0.2.7/dlt/cli/__init__.py
--rw-r--r--   0        0        0    15909 2023-05-07 23:03:04.659469 dlt-0.2.7/dlt/cli/_dlt.py
--rw-r--r--   0        0        0     3858 2023-05-07 23:03:04.659469 dlt-0.2.7/dlt/cli/config_toml_writer.py
--rw-r--r--   0        0        0    16665 2023-05-14 20:33:31.539348 dlt-0.2.7/dlt/cli/deploy_command.py
--rw-r--r--   0        0        0     1853 2023-04-30 21:17:44.388805 dlt-0.2.7/dlt/cli/echo.py
--rw-r--r--   0        0        0      435 2023-03-23 14:48:32.551618 dlt-0.2.7/dlt/cli/exceptions.py
--rw-r--r--   0        0        0    18832 2023-05-14 20:33:31.539348 dlt-0.2.7/dlt/cli/init_command.py
--rw-r--r--   0        0        0    10489 2023-04-30 21:17:44.388805 dlt-0.2.7/dlt/cli/pipeline_command.py
--rw-r--r--   0        0        0     9422 2023-05-14 20:33:31.539348 dlt-0.2.7/dlt/cli/pipeline_files.py
--rw-r--r--   0        0        0     4510 2023-05-07 23:03:04.659469 dlt-0.2.7/dlt/cli/source_detection.py
--rw-r--r--   0        0        0     1899 2023-04-22 20:26:30.632198 dlt-0.2.7/dlt/cli/telemetry_command.py
--rw-r--r--   0        0        0     3757 2023-04-30 21:17:44.388805 dlt-0.2.7/dlt/cli/utils.py
--rw-r--r--   0        0        0      307 2023-03-23 14:48:32.551618 dlt-0.2.7/dlt/common/__init__.py
--rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.2.7/dlt/common/arithmetics.py
--rw-r--r--   0        0        0      428 2023-03-23 14:48:32.551618 dlt-0.2.7/dlt/common/configuration/__init__.py
--rw-r--r--   0        0        0     4243 2023-05-14 20:33:31.539348 dlt-0.2.7/dlt/common/configuration/accessors.py
--rw-r--r--   0        0        0     3469 2023-05-07 23:03:04.659469 dlt-0.2.7/dlt/common/configuration/container.py
--rw-r--r--   0        0        0     5884 2023-04-22 20:26:30.632198 dlt-0.2.7/dlt/common/configuration/exceptions.py
--rw-r--r--   0        0        0     7912 2023-04-22 20:26:30.632198 dlt-0.2.7/dlt/common/configuration/inject.py
--rw-r--r--   0        0        0     1791 2023-05-14 20:33:31.539348 dlt-0.2.7/dlt/common/configuration/paths.py
--rw-r--r--   0        0        0      306 2023-05-07 23:03:04.659469 dlt-0.2.7/dlt/common/configuration/providers/__init__.py
--rw-r--r--   0        0        0     1108 2023-04-26 11:34:23.292768 dlt-0.2.7/dlt/common/configuration/providers/airflow.py
--rw-r--r--   0        0        0     1116 2023-05-07 23:03:04.659469 dlt-0.2.7/dlt/common/configuration/providers/context.py
--rw-r--r--   0        0        0     1335 2023-05-07 23:03:04.659469 dlt-0.2.7/dlt/common/configuration/providers/dictionary.py
--rw-r--r--   0        0        0     1981 2023-05-07 23:03:04.659469 dlt-0.2.7/dlt/common/configuration/providers/environ.py
--rw-r--r--   0        0        0     9441 2023-05-14 20:33:31.539348 dlt-0.2.7/dlt/common/configuration/providers/google_secrets.py
--rw-r--r--   0        0        0     1108 2023-05-07 23:03:04.659469 dlt-0.2.7/dlt/common/configuration/providers/provider.py
--rw-r--r--   0        0        0     5237 2023-05-14 20:33:31.539348 dlt-0.2.7/dlt/common/configuration/providers/toml.py
--rw-r--r--   0        0        0    17262 2023-05-14 20:33:31.539348 dlt-0.2.7/dlt/common/configuration/resolve.py
--rw-r--r--   0        0        0     1176 2023-05-07 23:03:04.659469 dlt-0.2.7/dlt/common/configuration/specs/__init__.py
--rw-r--r--   0        0        0     1817 2023-05-07 23:03:04.659469 dlt-0.2.7/dlt/common/configuration/specs/api_credentials.py
--rw-r--r--   0        0        0    13108 2023-05-07 23:03:04.659469 dlt-0.2.7/dlt/common/configuration/specs/base_configuration.py
--rw-r--r--   0        0        0     5521 2023-05-14 20:33:31.539348 dlt-0.2.7/dlt/common/configuration/specs/config_providers_context.py
--rw-r--r--   0        0        0     2792 2023-03-23 14:48:32.551618 dlt-0.2.7/dlt/common/configuration/specs/config_section_context.py
--rw-r--r--   0        0        0     1798 2023-05-07 23:03:04.669469 dlt-0.2.7/dlt/common/configuration/specs/connection_string_credentials.py
--rw-r--r--   0        0        0     2125 2023-04-24 18:26:21.111453 dlt-0.2.7/dlt/common/configuration/specs/exceptions.py
--rw-r--r--   0        0        0    12725 2023-05-07 23:03:04.669469 dlt-0.2.7/dlt/common/configuration/specs/gcp_credentials.py
--rw-r--r--   0        0        0      725 2023-05-07 23:03:04.669469 dlt-0.2.7/dlt/common/configuration/specs/known_sections.py
--rw-r--r--   0        0        0      556 2023-03-23 14:48:32.551618 dlt-0.2.7/dlt/common/configuration/specs/load_volume_configuration.py
--rw-r--r--   0        0        0      417 2023-03-23 14:48:32.551618 dlt-0.2.7/dlt/common/configuration/specs/normalize_volume_configuration.py
--rw-r--r--   0        0        0     2455 2023-04-30 21:17:44.388805 dlt-0.2.7/dlt/common/configuration/specs/run_configuration.py
--rw-r--r--   0        0        0      944 2023-03-23 14:48:32.551618 dlt-0.2.7/dlt/common/configuration/specs/schema_volume_configuration.py
--rw-r--r--   0        0        0     6026 2023-05-07 23:03:04.669469 dlt-0.2.7/dlt/common/configuration/utils.py
--rw-r--r--   0        0        0      142 2023-03-23 14:48:32.551618 dlt-0.2.7/dlt/common/data_types/__init__.py
--rw-r--r--   0        0        0     6306 2023-03-23 14:48:32.551618 dlt-0.2.7/dlt/common/data_types/type_helpers.py
--rw-r--r--   0        0        0      214 2023-03-23 14:48:32.551618 dlt-0.2.7/dlt/common/data_types/typing.py
--rw-r--r--   0        0        0      260 2023-03-23 14:48:20.701618 dlt-0.2.7/dlt/common/data_writers/__init__.py
--rw-r--r--   0        0        0     5893 2023-03-23 14:48:32.551618 dlt-0.2.7/dlt/common/data_writers/buffered.py
--rw-r--r--   0        0        0     2395 2023-03-23 14:48:32.551618 dlt-0.2.7/dlt/common/data_writers/escape.py
--rw-r--r--   0        0        0      962 2023-03-23 14:48:32.551618 dlt-0.2.7/dlt/common/data_writers/exceptions.py
--rw-r--r--   0        0        0     5159 2023-03-23 14:48:32.551618 dlt-0.2.7/dlt/common/data_writers/writers.py
--rw-r--r--   0        0        0       97 2023-03-23 14:48:32.551618 dlt-0.2.7/dlt/common/destination/__init__.py
--rw-r--r--   0        0        0     2206 2023-04-05 08:03:40.638919 dlt-0.2.7/dlt/common/destination/capabilities.py
--rw-r--r--   0        0        0    10682 2023-04-24 11:35:34.867759 dlt-0.2.7/dlt/common/destination/reference.py
--rw-r--r--   0        0        0     6121 2023-04-30 21:17:44.388805 dlt-0.2.7/dlt/common/exceptions.py
--rw-r--r--   0        0        0     4954 2023-03-23 14:48:32.551618 dlt-0.2.7/dlt/common/git.py
--rw-r--r--   0        0        0     5253 2023-05-14 20:33:31.539348 dlt-0.2.7/dlt/common/json/__init__.py
--rw-r--r--   0        0        0     1802 2023-04-10 08:12:53.769595 dlt-0.2.7/dlt/common/json/_orjson.py
--rw-r--r--   0        0        0     2939 2023-04-10 08:12:53.769595 dlt-0.2.7/dlt/common/json/_simplejson.py
--rw-r--r--   0        0        0     1536 2023-04-29 12:58:55.943219 dlt-0.2.7/dlt/common/jsonpath.py
--rw-r--r--   0        0        0      232 2023-03-23 14:48:32.551618 dlt-0.2.7/dlt/common/normalizers/__init__.py
--rw-r--r--   0        0        0     1197 2023-05-07 23:03:04.669469 dlt-0.2.7/dlt/common/normalizers/configuration.py
--rw-r--r--   0        0        0      472 2023-03-23 14:48:32.551618 dlt-0.2.7/dlt/common/normalizers/exceptions.py
--rw-r--r--   0        0        0     1644 2023-04-06 15:27:24.759561 dlt-0.2.7/dlt/common/normalizers/json/__init__.py
--rw-r--r--   0        0        0    13382 2023-05-14 20:33:31.539348 dlt-0.2.7/dlt/common/normalizers/json/relational.py
--rw-r--r--   0        0        0       64 2023-03-23 14:48:32.551618 dlt-0.2.7/dlt/common/normalizers/naming/__init__.py
--rw-r--r--   0        0        0      807 2023-03-23 14:48:32.551618 dlt-0.2.7/dlt/common/normalizers/naming/direct.py
--rw-r--r--   0        0        0     1069 2023-03-23 14:48:32.551618 dlt-0.2.7/dlt/common/normalizers/naming/duck_case.py
--rw-r--r--   0        0        0      792 2023-03-23 14:48:32.551618 dlt-0.2.7/dlt/common/normalizers/naming/exceptions.py
--rw-r--r--   0        0        0     3753 2023-04-05 08:03:40.638919 dlt-0.2.7/dlt/common/normalizers/naming/naming.py
--rw-r--r--   0        0        0     3002 2023-03-23 14:48:32.551618 dlt-0.2.7/dlt/common/normalizers/naming/snake_case.py
--rw-r--r--   0        0        0      358 2023-04-02 09:09:15.855769 dlt-0.2.7/dlt/common/normalizers/typing.py
--rw-r--r--   0        0        0     2337 2023-04-06 15:27:24.759561 dlt-0.2.7/dlt/common/normalizers/utils.py
--rw-r--r--   0        0        0      451 2023-03-23 14:48:32.551618 dlt-0.2.7/dlt/common/pendulum.py
--rw-r--r--   0        0        0    16937 2023-05-14 20:33:31.539348 dlt-0.2.7/dlt/common/pipeline.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.551618 dlt-0.2.7/dlt/common/reflection/__init__.py
--rw-r--r--   0        0        0      374 2023-03-23 14:48:32.551618 dlt-0.2.7/dlt/common/reflection/function_visitor.py
--rw-r--r--   0        0        0     4891 2023-04-09 16:39:04.593180 dlt-0.2.7/dlt/common/reflection/spec.py
--rw-r--r--   0        0        0     5069 2023-04-24 18:26:21.111453 dlt-0.2.7/dlt/common/reflection/utils.py
--rw-r--r--   0        0        0      174 2023-04-30 21:17:44.388805 dlt-0.2.7/dlt/common/runners/__init__.py
--rw-r--r--   0        0        0      508 2023-04-30 21:17:44.388805 dlt-0.2.7/dlt/common/runners/configuration.py
--rw-r--r--   0        0        0     2635 2023-05-14 11:08:47.420838 dlt-0.2.7/dlt/common/runners/pool_runner.py
--rw-r--r--   0        0        0     4046 2023-03-23 14:48:32.561618 dlt-0.2.7/dlt/common/runners/runnable.py
--rw-r--r--   0        0        0     3145 2023-03-23 14:48:32.561618 dlt-0.2.7/dlt/common/runners/stdout.py
--rw-r--r--   0        0        0     2137 2023-03-23 14:48:32.561618 dlt-0.2.7/dlt/common/runners/synth_pickle.py
--rw-r--r--   0        0        0      105 2023-04-30 21:17:44.388805 dlt-0.2.7/dlt/common/runners/typing.py
--rw-r--r--   0        0        0     5590 2023-05-07 23:03:04.669469 dlt-0.2.7/dlt/common/runners/venv.py
--rw-r--r--   0        0        0       36 2023-04-30 21:17:44.398805 dlt-0.2.7/dlt/common/runtime/__init__.py
--rw-r--r--   0        0        0    13441 2023-04-30 21:17:44.398805 dlt-0.2.7/dlt/common/runtime/collector.py
--rw-r--r--   0        0        0     4501 2023-05-14 20:33:31.539348 dlt-0.2.7/dlt/common/runtime/exec_info.py
--rw-r--r--   0        0        0      647 2023-04-30 21:17:44.398805 dlt-0.2.7/dlt/common/runtime/init.py
--rw-r--r--   0        0        0     4002 2023-04-30 21:17:44.398805 dlt-0.2.7/dlt/common/runtime/logger.py
--rw-r--r--   0        0        0     2052 2023-04-30 21:17:44.398805 dlt-0.2.7/dlt/common/runtime/prometheus.py
--rw-r--r--   0        0        0     7170 2023-05-14 20:33:31.539348 dlt-0.2.7/dlt/common/runtime/segment.py
--rw-r--r--   0        0        0     2493 2023-04-30 21:17:44.398805 dlt-0.2.7/dlt/common/runtime/sentry.py
--rw-r--r--   0        0        0     2027 2023-04-30 21:17:44.398805 dlt-0.2.7/dlt/common/runtime/signals.py
--rw-r--r--   0        0        0      616 2023-04-03 18:50:36.893525 dlt-0.2.7/dlt/common/runtime/slack.py
--rw-r--r--   0        0        0      720 2023-04-30 21:17:44.398805 dlt-0.2.7/dlt/common/runtime/telemetry.py
--rw-r--r--   0        0        0      387 2023-04-03 18:50:36.893525 dlt-0.2.7/dlt/common/schema/__init__.py
--rw-r--r--   0        0        0     1927 2023-03-23 14:48:32.561618 dlt-0.2.7/dlt/common/schema/detections.py
--rw-r--r--   0        0        0     2974 2023-03-23 14:48:32.561618 dlt-0.2.7/dlt/common/schema/exceptions.py
--rw-r--r--   0        0        0    25175 2023-04-09 16:39:04.593180 dlt-0.2.7/dlt/common/schema/schema.py
--rw-r--r--   0        0        0     3004 2023-04-22 20:26:30.632198 dlt-0.2.7/dlt/common/schema/typing.py
--rw-r--r--   0        0        0    23087 2023-04-30 21:17:44.398805 dlt-0.2.7/dlt/common/schema/utils.py
--rw-r--r--   0        0        0      410 2023-03-23 14:48:32.561618 dlt-0.2.7/dlt/common/storages/__init__.py
--rw-r--r--   0        0        0     1906 2023-03-23 14:48:32.561618 dlt-0.2.7/dlt/common/storages/data_item_storage.py
--rw-r--r--   0        0        0     2804 2023-04-03 18:50:36.893525 dlt-0.2.7/dlt/common/storages/exceptions.py
--rw-r--r--   0        0        0    10891 2023-05-14 20:33:31.539348 dlt-0.2.7/dlt/common/storages/file_storage.py
--rw-r--r--   0        0        0     2685 2023-04-13 08:33:43.967587 dlt-0.2.7/dlt/common/storages/live_schema_storage.py
--rw-r--r--   0        0        0    21806 2023-05-14 20:33:31.539348 dlt-0.2.7/dlt/common/storages/load_storage.py
--rw-r--r--   0        0        0     2414 2023-03-23 14:48:32.561618 dlt-0.2.7/dlt/common/storages/normalize_storage.py
--rw-r--r--   0        0        0     8508 2023-03-23 14:48:32.561618 dlt-0.2.7/dlt/common/storages/schema_storage.py
--rw-r--r--   0        0        0     2525 2023-04-24 18:26:21.111453 dlt-0.2.7/dlt/common/storages/versioned_storage.py
--rw-r--r--   0        0        0     2634 2023-05-07 23:03:04.669469 dlt-0.2.7/dlt/common/time.py
--rw-r--r--   0        0        0     4736 2023-04-03 18:50:36.893525 dlt-0.2.7/dlt/common/typing.py
--rw-r--r--   0        0        0    11275 2023-04-24 18:26:21.111453 dlt-0.2.7/dlt/common/utils.py
--rw-r--r--   0        0        0     3686 2023-03-23 14:48:32.561618 dlt-0.2.7/dlt/common/validation.py
--rw-r--r--   0        0        0     1185 2023-03-23 14:48:32.561618 dlt-0.2.7/dlt/common/wei.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.561618 dlt-0.2.7/dlt/destinations/__init__.py
--rw-r--r--   0        0        0      437 2023-03-23 14:48:32.561618 dlt-0.2.7/dlt/destinations/bigquery/README.md
--rw-r--r--   0        0        0     1813 2023-04-05 08:03:40.638919 dlt-0.2.7/dlt/destinations/bigquery/__init__.py
--rw-r--r--   0        0        0    12347 2023-05-07 23:03:04.669469 dlt-0.2.7/dlt/destinations/bigquery/bigquery.py
--rw-r--r--   0        0        0      386 2023-05-07 23:03:04.669469 dlt-0.2.7/dlt/destinations/bigquery/configuration.py
--rw-r--r--   0        0        0    10342 2023-05-07 23:03:04.669469 dlt-0.2.7/dlt/destinations/bigquery/sql_client.py
--rw-r--r--   0        0        0     1935 2023-04-05 08:03:40.638919 dlt-0.2.7/dlt/destinations/duckdb/__init__.py
--rw-r--r--   0        0        0     7008 2023-05-07 23:03:04.669469 dlt-0.2.7/dlt/destinations/duckdb/configuration.py
--rw-r--r--   0        0        0     2754 2023-03-23 14:48:32.561618 dlt-0.2.7/dlt/destinations/duckdb/duck.py
--rw-r--r--   0        0        0     6936 2023-04-21 22:25:54.789942 dlt-0.2.7/dlt/destinations/duckdb/sql_client.py
--rw-r--r--   0        0        0     1671 2023-03-23 14:48:32.561618 dlt-0.2.7/dlt/destinations/dummy/__init__.py
--rw-r--r--   0        0        0      736 2023-04-03 18:50:36.893525 dlt-0.2.7/dlt/destinations/dummy/configuration.py
--rw-r--r--   0        0        0     4975 2023-04-24 11:35:34.867759 dlt-0.2.7/dlt/destinations/dummy/dummy.py
--rw-r--r--   0        0        0     4159 2023-04-05 08:03:40.638919 dlt-0.2.7/dlt/destinations/exceptions.py
--rw-r--r--   0        0        0     4983 2023-04-05 08:03:40.638919 dlt-0.2.7/dlt/destinations/insert_job_client.py
--rw-r--r--   0        0        0    15357 2023-05-07 23:03:04.669469 dlt-0.2.7/dlt/destinations/job_client_impl.py
--rw-r--r--   0        0        0     1303 2023-04-05 08:03:40.638919 dlt-0.2.7/dlt/destinations/job_impl.py
--rw-r--r--   0        0        0      251 2023-03-23 14:48:32.561618 dlt-0.2.7/dlt/destinations/postgres/README.md
--rw-r--r--   0        0        0     1934 2023-04-05 08:03:40.638919 dlt-0.2.7/dlt/destinations/postgres/__init__.py
--rw-r--r--   0        0        0     1232 2023-05-07 23:03:04.669469 dlt-0.2.7/dlt/destinations/postgres/configuration.py
--rw-r--r--   0        0        0     3025 2023-03-23 14:48:32.561618 dlt-0.2.7/dlt/destinations/postgres/postgres.py
--rw-r--r--   0        0        0     6074 2023-05-07 23:03:04.669469 dlt-0.2.7/dlt/destinations/postgres/sql_client.py
--rw-r--r--   0        0        0     1159 2023-04-03 18:50:36.893525 dlt-0.2.7/dlt/destinations/redshift/README.md
--rw-r--r--   0        0        0     1905 2023-04-05 08:03:40.638919 dlt-0.2.7/dlt/destinations/redshift/__init__.py
--rw-r--r--   0        0        0      570 2023-05-07 23:03:04.669469 dlt-0.2.7/dlt/destinations/redshift/configuration.py
--rw-r--r--   0        0        0     3761 2023-03-23 14:48:32.561618 dlt-0.2.7/dlt/destinations/redshift/redshift.py
--rw-r--r--   0        0        0     7110 2023-04-29 12:58:55.953219 dlt-0.2.7/dlt/destinations/sql_client.py
--rw-r--r--   0        0        0    10101 2023-04-09 16:39:04.593180 dlt-0.2.7/dlt/destinations/sql_merge_job.py
--rw-r--r--   0        0        0     1931 2023-04-24 18:26:21.111453 dlt-0.2.7/dlt/destinations/typing.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.2.7/dlt/extract/__init__.py
--rw-r--r--   0        0        0    22830 2023-05-14 20:33:31.539348 dlt-0.2.7/dlt/extract/decorators.py
--rw-r--r--   0        0        0    12645 2023-04-30 21:17:44.398805 dlt-0.2.7/dlt/extract/exceptions.py
--rw-r--r--   0        0        0     8449 2023-04-30 21:17:44.398805 dlt-0.2.7/dlt/extract/extract.py
--rw-r--r--   0        0        0    14956 2023-05-14 20:33:31.539348 dlt-0.2.7/dlt/extract/incremental.py
--rw-r--r--   0        0        0    31567 2023-04-30 21:17:44.398805 dlt-0.2.7/dlt/extract/pipe.py
--rw-r--r--   0        0        0     9683 2023-04-22 20:26:30.632198 dlt-0.2.7/dlt/extract/schema.py
--rw-r--r--   0        0        0    34195 2023-05-07 23:03:04.669469 dlt-0.2.7/dlt/extract/source.py
--rw-r--r--   0        0        0     4350 2023-04-22 20:26:30.632198 dlt-0.2.7/dlt/extract/typing.py
--rw-r--r--   0        0        0      593 2023-04-06 20:38:35.239561 dlt-0.2.7/dlt/extract/utils.py
--rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.2.7/dlt/helpers/__init__.py
--rw-r--r--   0        0        0      267 2023-05-14 20:33:31.539348 dlt-0.2.7/dlt/helpers/airflow.py
--rw-r--r--   0        0        0     2907 2023-03-23 14:48:32.561618 dlt-0.2.7/dlt/helpers/dbt/__init__.py
--rw-r--r--   0        0        0     1220 2023-03-23 14:48:32.561618 dlt-0.2.7/dlt/helpers/dbt/configuration.py
--rw-r--r--   0        0        0     6137 2023-03-23 14:48:32.561618 dlt-0.2.7/dlt/helpers/dbt/dbt_utils.py
--rw-r--r--   0        0        0      758 2023-03-23 14:48:32.561618 dlt-0.2.7/dlt/helpers/dbt/exceptions.py
--rw-r--r--   0        0        0     3583 2023-03-23 14:48:32.561618 dlt-0.2.7/dlt/helpers/dbt/profiles.yml
--rw-r--r--   0        0        0    13032 2023-04-30 21:17:44.398805 dlt-0.2.7/dlt/helpers/dbt/runner.py
--rw-r--r--   0        0        0     2490 2023-05-14 20:33:31.539348 dlt-0.2.7/dlt/helpers/pandas.py
--rw-r--r--   0        0        0     1035 2023-03-23 14:48:32.571618 dlt-0.2.7/dlt/helpers/parquet.py
--rw-r--r--   0        0        0    13371 2023-04-30 21:17:44.398805 dlt-0.2.7/dlt/helpers/streamlit.py
--rw-r--r--   0        0        0       31 2023-03-23 14:48:32.571618 dlt-0.2.7/dlt/load/__init__.py
--rw-r--r--   0        0        0     1019 2023-04-30 21:17:44.398805 dlt-0.2.7/dlt/load/configuration.py
--rw-r--r--   0        0        0     1993 2023-04-05 08:03:40.638919 dlt-0.2.7/dlt/load/exceptions.py
--rw-r--r--   0        0        0    19928 2023-04-30 21:17:44.398805 dlt-0.2.7/dlt/load/load.py
--rw-r--r--   0        0        0       32 2023-03-23 14:48:32.571618 dlt-0.2.7/dlt/normalize/__init__.py
--rw-r--r--   0        0        0     1098 2023-04-30 21:17:44.398805 dlt-0.2.7/dlt/normalize/configuration.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.2.7/dlt/normalize/exceptions.py
--rw-r--r--   0        0        0    16576 2023-04-30 21:17:44.398805 dlt-0.2.7/dlt/normalize/normalize.py
--rw-r--r--   0        0        0     1880 2023-03-23 14:48:32.571618 dlt-0.2.7/dlt/pipeline/README.md
--rw-r--r--   0        0        0    13138 2023-04-30 21:17:44.398805 dlt-0.2.7/dlt/pipeline/__init__.py
--rw-r--r--   0        0        0     1858 2023-04-30 21:17:44.398805 dlt-0.2.7/dlt/pipeline/configuration.py
--rw-r--r--   0        0        0      363 2023-04-22 20:26:30.632198 dlt-0.2.7/dlt/pipeline/current.py
--rw-r--r--   0        0        0     4829 2023-03-23 14:48:32.571618 dlt-0.2.7/dlt/pipeline/dbt.py
--rw-r--r--   0        0        0     2891 2023-04-30 21:17:44.398805 dlt-0.2.7/dlt/pipeline/exceptions.py
--rw-r--r--   0        0        0     8764 2023-05-07 23:03:04.669469 dlt-0.2.7/dlt/pipeline/helpers.py
--rw-r--r--   0        0        0      122 2023-04-06 15:27:24.759561 dlt-0.2.7/dlt/pipeline/mark.py
--rw-r--r--   0        0        0    56518 2023-05-14 20:33:31.539348 dlt-0.2.7/dlt/pipeline/pipeline.py
--rw-r--r--   0        0        0      985 2023-04-30 21:17:44.398805 dlt-0.2.7/dlt/pipeline/progress.py
--rw-r--r--   0        0        0     4200 2023-04-10 08:12:53.769595 dlt-0.2.7/dlt/pipeline/state_sync.py
--rw-r--r--   0        0        0     7990 2023-04-03 18:50:36.903525 dlt-0.2.7/dlt/pipeline/trace.py
--rw-r--r--   0        0        0     4563 2023-04-03 18:50:36.903525 dlt-0.2.7/dlt/pipeline/track.py
--rw-r--r--   0        0        0       91 2023-03-23 14:48:32.571618 dlt-0.2.7/dlt/pipeline/typing.py
--rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.2.7/dlt/py.typed
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.2.7/dlt/reflection/__init__.py
--rw-r--r--   0        0        0      563 2023-03-23 14:48:32.571618 dlt-0.2.7/dlt/reflection/names.py
--rw-r--r--   0        0        0     5617 2023-05-07 23:03:04.669469 dlt-0.2.7/dlt/reflection/script_inspector.py
--rw-r--r--   0        0        0     6186 2023-03-23 14:48:32.571618 dlt-0.2.7/dlt/reflection/script_visitor.py
--rw-r--r--   0        0        0      124 2023-05-07 23:03:04.669469 dlt-0.2.7/dlt/sources/__init__.py
--rw-r--r--   0        0        0      320 2023-05-07 23:03:04.669469 dlt-0.2.7/dlt/sources/credentials.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.2.7/dlt/sources/helpers/__init__.py
--rw-r--r--   0        0        0      574 2023-03-23 14:48:37.261618 dlt-0.2.7/dlt/sources/helpers/requests/__init__.py
--rw-r--r--   0        0        0     9106 2023-05-14 20:33:31.539348 dlt-0.2.7/dlt/sources/helpers/requests/retry.py
--rw-r--r--   0        0        0     1336 2023-03-23 14:48:32.571618 dlt-0.2.7/dlt/sources/helpers/requests/session.py
--rw-r--r--   0        0        0      679 2023-04-06 15:27:24.759561 dlt-0.2.7/dlt/sources/helpers/transform.py
--rw-r--r--   0        0        0     1125 2023-04-22 20:26:30.632198 dlt-0.2.7/dlt/version.py
--rw-r--r--   0        0        0     4054 2023-05-14 20:33:46.239349 dlt-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     7369 1970-01-01 00:00:00.000000 dlt-0.2.7/setup.py
--rw-r--r--   0        0        0     7321 1970-01-01 00:00:00.000000 dlt-0.2.7/PKG-INFO
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

### Comparing `dlt-0.2.7/LICENSE.txt` & `dlt-0.2.7a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/README.md` & `dlt-0.2.7a0/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/__init__.py` & `dlt-0.2.7a0/dlt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/cli/_dlt.py` & `dlt-0.2.7a0/dlt/cli/_dlt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/cli/config_toml_writer.py` & `dlt-0.2.7a0/dlt/cli/config_toml_writer.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/cli/deploy_command.py` & `dlt-0.2.7a0/dlt/cli/deploy_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/cli/echo.py` & `dlt-0.2.7a0/dlt/cli/echo.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/cli/init_command.py` & `dlt-0.2.7a0/dlt/cli/init_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/cli/pipeline_command.py` & `dlt-0.2.7a0/dlt/cli/pipeline_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/cli/pipeline_files.py` & `dlt-0.2.7a0/dlt/cli/pipeline_files.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/cli/source_detection.py` & `dlt-0.2.7a0/dlt/cli/source_detection.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/cli/telemetry_command.py` & `dlt-0.2.7a0/dlt/cli/telemetry_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/cli/utils.py` & `dlt-0.2.7a0/dlt/cli/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/arithmetics.py` & `dlt-0.2.7a0/dlt/common/arithmetics.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/configuration/accessors.py` & `dlt-0.2.7a0/dlt/common/configuration/accessors.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/configuration/container.py` & `dlt-0.2.7a0/dlt/common/configuration/container.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/configuration/exceptions.py` & `dlt-0.2.7a0/dlt/common/configuration/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/configuration/inject.py` & `dlt-0.2.7a0/dlt/common/configuration/inject.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/configuration/paths.py` & `dlt-0.2.7a0/dlt/common/configuration/paths.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/configuration/providers/airflow.py` & `dlt-0.2.7a0/dlt/common/configuration/providers/airflow.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/configuration/providers/context.py` & `dlt-0.2.7a0/dlt/common/configuration/providers/context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/configuration/providers/dictionary.py` & `dlt-0.2.7a0/dlt/common/configuration/providers/dictionary.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/configuration/providers/environ.py` & `dlt-0.2.7a0/dlt/common/configuration/providers/environ.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/configuration/providers/google_secrets.py` & `dlt-0.2.7a0/dlt/common/configuration/providers/google_secrets.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/configuration/providers/provider.py` & `dlt-0.2.7a0/dlt/common/configuration/providers/provider.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/configuration/providers/toml.py` & `dlt-0.2.7a0/dlt/common/configuration/providers/toml.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/configuration/resolve.py` & `dlt-0.2.7a0/dlt/common/configuration/resolve.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/configuration/specs/__init__.py` & `dlt-0.2.7a0/dlt/common/configuration/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/configuration/specs/api_credentials.py` & `dlt-0.2.7a0/dlt/common/configuration/specs/api_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/configuration/specs/base_configuration.py` & `dlt-0.2.7a0/dlt/common/configuration/specs/base_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/configuration/specs/config_providers_context.py` & `dlt-0.2.7a0/dlt/common/configuration/specs/config_providers_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/configuration/specs/config_section_context.py` & `dlt-0.2.7a0/dlt/common/configuration/specs/config_section_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/configuration/specs/connection_string_credentials.py` & `dlt-0.2.7a0/dlt/common/configuration/specs/connection_string_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/configuration/specs/exceptions.py` & `dlt-0.2.7a0/dlt/common/configuration/specs/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/configuration/specs/gcp_credentials.py` & `dlt-0.2.7a0/dlt/common/configuration/specs/gcp_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/configuration/specs/known_sections.py` & `dlt-0.2.7a0/dlt/common/configuration/specs/known_sections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/configuration/specs/load_volume_configuration.py` & `dlt-0.2.7a0/dlt/common/configuration/specs/load_volume_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/configuration/specs/run_configuration.py` & `dlt-0.2.7a0/dlt/common/configuration/specs/run_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/configuration/specs/schema_volume_configuration.py` & `dlt-0.2.7a0/dlt/common/configuration/specs/schema_volume_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/configuration/utils.py` & `dlt-0.2.7a0/dlt/common/configuration/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/data_types/type_helpers.py` & `dlt-0.2.7a0/dlt/common/data_types/type_helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/data_writers/buffered.py` & `dlt-0.2.7a0/dlt/common/data_writers/buffered.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/data_writers/escape.py` & `dlt-0.2.7a0/dlt/common/data_writers/escape.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/data_writers/exceptions.py` & `dlt-0.2.7a0/dlt/common/data_writers/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/data_writers/writers.py` & `dlt-0.2.7a0/dlt/common/data_writers/writers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/destination/capabilities.py` & `dlt-0.2.7a0/dlt/common/destination/capabilities.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/destination/reference.py` & `dlt-0.2.7a0/dlt/common/destination/reference.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/exceptions.py` & `dlt-0.2.7a0/dlt/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/git.py` & `dlt-0.2.7a0/dlt/common/git.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/json/__init__.py` & `dlt-0.2.7a0/dlt/common/json/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         if c >=0 and c <= 6:
             return DECODERS[c](obj[1:])
     return obj
 
 
 def custom_pua_decode_nested(obj: Any) -> Any:
     if isinstance(obj, str):
-        return custom_pua_decode(obj)
+        return custom_pua_decode
     elif isinstance(obj, (list, dict)):
         return map_nested_in_place(custom_pua_decode, obj)
     return obj
 
 
 def custom_pua_remove(obj: Any) -> Any:
     """Removes the PUA data type marker and leaves the correctly serialized type representation. Unmarked values are returned as-is."""
```

### Comparing `dlt-0.2.7/dlt/common/json/_orjson.py` & `dlt-0.2.7a0/dlt/common/json/_orjson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/json/_simplejson.py` & `dlt-0.2.7a0/dlt/common/json/_simplejson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/jsonpath.py` & `dlt-0.2.7a0/dlt/common/jsonpath.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/normalizers/configuration.py` & `dlt-0.2.7a0/dlt/common/normalizers/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/normalizers/json/__init__.py` & `dlt-0.2.7a0/dlt/common/normalizers/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/normalizers/json/relational.py` & `dlt-0.2.7a0/dlt/common/normalizers/json/relational.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/normalizers/naming/direct.py` & `dlt-0.2.7a0/dlt/common/normalizers/naming/direct.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/normalizers/naming/duck_case.py` & `dlt-0.2.7a0/dlt/common/normalizers/naming/duck_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/normalizers/naming/exceptions.py` & `dlt-0.2.7a0/dlt/common/normalizers/naming/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/normalizers/naming/naming.py` & `dlt-0.2.7a0/dlt/common/normalizers/naming/naming.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/normalizers/naming/snake_case.py` & `dlt-0.2.7a0/dlt/common/normalizers/naming/snake_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/normalizers/utils.py` & `dlt-0.2.7a0/dlt/common/normalizers/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/pipeline.py` & `dlt-0.2.7a0/dlt/common/pipeline.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/reflection/spec.py` & `dlt-0.2.7a0/dlt/common/reflection/spec.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/reflection/utils.py` & `dlt-0.2.7a0/dlt/common/reflection/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/runners/pool_runner.py` & `dlt-0.2.7a0/dlt/common/runners/pool_runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/runners/runnable.py` & `dlt-0.2.7a0/dlt/common/runners/runnable.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/runners/stdout.py` & `dlt-0.2.7a0/dlt/common/runners/stdout.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/runners/synth_pickle.py` & `dlt-0.2.7a0/dlt/common/runners/synth_pickle.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/runners/venv.py` & `dlt-0.2.7a0/dlt/common/runners/venv.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/runtime/collector.py` & `dlt-0.2.7a0/dlt/common/runtime/collector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/runtime/exec_info.py` & `dlt-0.2.7a0/dlt/common/runtime/exec_info.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/runtime/init.py` & `dlt-0.2.7a0/dlt/common/runtime/init.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/runtime/logger.py` & `dlt-0.2.7a0/dlt/common/runtime/logger.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/runtime/prometheus.py` & `dlt-0.2.7a0/dlt/common/runtime/prometheus.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/runtime/segment.py` & `dlt-0.2.7a0/dlt/common/runtime/segment.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/runtime/sentry.py` & `dlt-0.2.7a0/dlt/common/runtime/sentry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/runtime/signals.py` & `dlt-0.2.7a0/dlt/common/runtime/signals.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/runtime/slack.py` & `dlt-0.2.7a0/dlt/common/runtime/slack.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/runtime/telemetry.py` & `dlt-0.2.7a0/dlt/common/runtime/telemetry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/schema/detections.py` & `dlt-0.2.7a0/dlt/common/schema/detections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/schema/exceptions.py` & `dlt-0.2.7a0/dlt/common/schema/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/schema/schema.py` & `dlt-0.2.7a0/dlt/common/schema/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/schema/typing.py` & `dlt-0.2.7a0/dlt/common/schema/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/schema/utils.py` & `dlt-0.2.7a0/dlt/common/schema/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/storages/data_item_storage.py` & `dlt-0.2.7a0/dlt/common/storages/data_item_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/storages/exceptions.py` & `dlt-0.2.7a0/dlt/common/storages/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/storages/file_storage.py` & `dlt-0.2.7a0/dlt/common/storages/file_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/storages/live_schema_storage.py` & `dlt-0.2.7a0/dlt/common/storages/live_schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/storages/load_storage.py` & `dlt-0.2.7a0/dlt/common/storages/load_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/storages/normalize_storage.py` & `dlt-0.2.7a0/dlt/common/storages/normalize_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/storages/schema_storage.py` & `dlt-0.2.7a0/dlt/common/storages/schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/storages/versioned_storage.py` & `dlt-0.2.7a0/dlt/common/storages/versioned_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/time.py` & `dlt-0.2.7a0/dlt/common/time.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/typing.py` & `dlt-0.2.7a0/dlt/common/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/utils.py` & `dlt-0.2.7a0/dlt/common/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/validation.py` & `dlt-0.2.7a0/dlt/common/validation.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/common/wei.py` & `dlt-0.2.7a0/dlt/common/wei.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/destinations/bigquery/__init__.py` & `dlt-0.2.7a0/dlt/destinations/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/destinations/bigquery/bigquery.py` & `dlt-0.2.7a0/dlt/destinations/bigquery/bigquery.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/destinations/bigquery/sql_client.py` & `dlt-0.2.7a0/dlt/destinations/bigquery/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/destinations/duckdb/__init__.py` & `dlt-0.2.7a0/dlt/destinations/duckdb/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/destinations/duckdb/configuration.py` & `dlt-0.2.7a0/dlt/destinations/duckdb/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/destinations/duckdb/duck.py` & `dlt-0.2.7a0/dlt/destinations/duckdb/duck.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/destinations/duckdb/sql_client.py` & `dlt-0.2.7a0/dlt/destinations/duckdb/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/destinations/dummy/__init__.py` & `dlt-0.2.7a0/dlt/destinations/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/destinations/dummy/configuration.py` & `dlt-0.2.7a0/dlt/destinations/dummy/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/destinations/dummy/dummy.py` & `dlt-0.2.7a0/dlt/destinations/dummy/dummy.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/destinations/exceptions.py` & `dlt-0.2.7a0/dlt/destinations/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/destinations/insert_job_client.py` & `dlt-0.2.7a0/dlt/destinations/insert_job_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/destinations/job_client_impl.py` & `dlt-0.2.7a0/dlt/destinations/job_client_impl.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/destinations/job_impl.py` & `dlt-0.2.7a0/dlt/destinations/job_impl.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/destinations/postgres/__init__.py` & `dlt-0.2.7a0/dlt/destinations/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/destinations/postgres/configuration.py` & `dlt-0.2.7a0/dlt/destinations/postgres/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/destinations/postgres/postgres.py` & `dlt-0.2.7a0/dlt/destinations/postgres/postgres.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/destinations/postgres/sql_client.py` & `dlt-0.2.7a0/dlt/destinations/postgres/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/destinations/redshift/README.md` & `dlt-0.2.7a0/dlt/destinations/redshift/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/destinations/redshift/__init__.py` & `dlt-0.2.7a0/dlt/destinations/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/destinations/redshift/configuration.py` & `dlt-0.2.7a0/dlt/destinations/redshift/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/destinations/redshift/redshift.py` & `dlt-0.2.7a0/dlt/destinations/redshift/redshift.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/destinations/sql_client.py` & `dlt-0.2.7a0/dlt/destinations/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/destinations/sql_merge_job.py` & `dlt-0.2.7a0/dlt/destinations/sql_merge_job.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/destinations/typing.py` & `dlt-0.2.7a0/dlt/destinations/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/extract/decorators.py` & `dlt-0.2.7a0/dlt/extract/decorators.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/extract/exceptions.py` & `dlt-0.2.7a0/dlt/extract/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/extract/extract.py` & `dlt-0.2.7a0/dlt/extract/extract.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/extract/incremental.py` & `dlt-0.2.7a0/dlt/extract/incremental.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 from typing import Generic, TypeVar, Any, Optional, Callable, List, TypedDict, get_origin, Sequence
 import inspect
 from functools import wraps
-from datetime import datetime  # noqa: I251
 
 import dlt
 from dlt.common.json import json
 from dlt.common.jsonpath import compile_path, find_values, JSONPath
 from dlt.common.typing import TDataItem, TDataItems, TFun, extract_inner_type, is_optional_type
 from dlt.common.schema.typing import TColumnKey
 from dlt.common.configuration import configspec
 from dlt.common.configuration.specs import BaseConfiguration
 from dlt.common.pipeline import _resource_state
 from dlt.common.utils import digest128
 from dlt.extract.exceptions import IncrementalUnboundError, PipeException
 from dlt.extract.pipe import Pipe
 from dlt.extract.utils import resolve_column_value
 from dlt.extract.typing import FilterItem, SupportsPipe, TTableHintTemplate
-from dlt.common import pendulum
 
 
 TCursorValue = TypeVar("TCursorValue", bound=Any)
 LastValueFunc = Callable[[Sequence[TCursorValue]], Any]
 
 
 class IncrementalColumnState(TypedDict):
@@ -171,21 +169,15 @@
 
         row_values = find_values(self.cursor_path_p, row)
         if not row_values:
             raise IncrementalCursorPathMissing(self.resource_name, self.cursor_path, row)
 
         incremental_state = self._cached_state
         last_value = incremental_state['last_value']
-        row_value = row_values[0]
-
-        # For datetime cursor, ensure the value is a timezone aware datetime.
-        # The object saved in state will always be a tz aware pendulum datetime so this ensures values are comparable
-        if isinstance(row_value, datetime):
-            row_value = pendulum.instance(row_value)
-
+        row_value = row_values[0]  # For now the value needs to match deserialized presentation from state
         check_values = (row_value,) + ((last_value, ) if last_value is not None else ())
         new_value = self.last_value_func(check_values)
         if last_value == new_value:
             # we store row id for all records with the current "last_value" in state and use it to deduplicate
             if self.last_value_func((row_value, )) == last_value:
                 unique_value = self.unique_value(row)
                 # if unique value exists then use it to deduplicate
```

### Comparing `dlt-0.2.7/dlt/extract/pipe.py` & `dlt-0.2.7a0/dlt/extract/pipe.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/extract/schema.py` & `dlt-0.2.7a0/dlt/extract/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/extract/source.py` & `dlt-0.2.7a0/dlt/extract/source.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/extract/typing.py` & `dlt-0.2.7a0/dlt/extract/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/extract/utils.py` & `dlt-0.2.7a0/dlt/extract/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/helpers/dbt/__init__.py` & `dlt-0.2.7a0/dlt/helpers/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/helpers/dbt/configuration.py` & `dlt-0.2.7a0/dlt/helpers/dbt/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/helpers/dbt/dbt_utils.py` & `dlt-0.2.7a0/dlt/helpers/dbt/dbt_utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/helpers/dbt/exceptions.py` & `dlt-0.2.7a0/dlt/helpers/dbt/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/helpers/dbt/profiles.yml` & `dlt-0.2.7a0/dlt/helpers/dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/helpers/dbt/runner.py` & `dlt-0.2.7a0/dlt/helpers/dbt/runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/helpers/pandas.py` & `dlt-0.2.7a0/dlt/helpers/pandas.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/helpers/parquet.py` & `dlt-0.2.7a0/dlt/helpers/parquet.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/helpers/streamlit.py` & `dlt-0.2.7a0/dlt/helpers/streamlit.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/load/configuration.py` & `dlt-0.2.7a0/dlt/load/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/load/exceptions.py` & `dlt-0.2.7a0/dlt/load/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/load/load.py` & `dlt-0.2.7a0/dlt/load/load.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/normalize/configuration.py` & `dlt-0.2.7a0/dlt/normalize/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/normalize/normalize.py` & `dlt-0.2.7a0/dlt/normalize/normalize.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/pipeline/README.md` & `dlt-0.2.7a0/dlt/pipeline/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/pipeline/__init__.py` & `dlt-0.2.7a0/dlt/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/pipeline/configuration.py` & `dlt-0.2.7a0/dlt/pipeline/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/pipeline/dbt.py` & `dlt-0.2.7a0/dlt/pipeline/dbt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/pipeline/exceptions.py` & `dlt-0.2.7a0/dlt/pipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/pipeline/helpers.py` & `dlt-0.2.7a0/dlt/pipeline/helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/pipeline/pipeline.py` & `dlt-0.2.7a0/dlt/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/pipeline/progress.py` & `dlt-0.2.7a0/dlt/pipeline/progress.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/pipeline/state_sync.py` & `dlt-0.2.7a0/dlt/pipeline/state_sync.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/pipeline/trace.py` & `dlt-0.2.7a0/dlt/pipeline/trace.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/pipeline/track.py` & `dlt-0.2.7a0/dlt/pipeline/track.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/reflection/names.py` & `dlt-0.2.7a0/dlt/reflection/names.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/reflection/script_inspector.py` & `dlt-0.2.7a0/dlt/reflection/script_inspector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/reflection/script_visitor.py` & `dlt-0.2.7a0/dlt/reflection/script_visitor.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/sources/helpers/requests/__init__.py` & `dlt-0.2.7a0/dlt/sources/helpers/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/sources/helpers/requests/retry.py` & `dlt-0.2.7a0/dlt/sources/helpers/requests/retry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/sources/helpers/requests/session.py` & `dlt-0.2.7a0/dlt/sources/helpers/requests/session.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/sources/helpers/transform.py` & `dlt-0.2.7a0/dlt/sources/helpers/transform.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/dlt/version.py` & `dlt-0.2.7a0/dlt/version.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.7/pyproject.toml` & `dlt-0.2.7a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dlt"
-version = "0.2.7"
+version = "0.2.7a0"
 description = "DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run."
 authors = ["dltHub Inc. <services@dlthub.com>"]
 maintainers = [ "Marcin Rudolf <marcin@dlthub.com>", "Adrian Brudaru <adrian@dlthub.com>", "Ty Dunn <ty@dlthub.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/dlt-hub"
 repository = "https://github.com/dlt-hub/dlt"
```

### Comparing `dlt-0.2.7/setup.py` & `dlt-0.2.7a0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
  'redshift:platform_python_implementation == "PyPy"': ['psycopg2cffi>=2.9.0']}
 
 entry_points = \
 {'console_scripts': ['dlt = dlt.cli._dlt:_main']}
 
 setup_kwargs = {
     'name': 'dlt',
-    'version': '0.2.7',
+    'version': '0.2.7a0',
     'description': 'DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.',
     'long_description': '<h1 align="center">\n    <strong>data load tool (dlt) — the open-source Python library for data loading</strong>\n</h1>\n<p align="center">\nBe it a Google Colab notebook, AWS Lambda function, an Airflow DAG, your local laptop,<br/>or a GPT-4 assisted development playground—<strong>dlt</strong> can be dropped in anywhere.\n</p>\n\n<div align="center">\n  <a target="_blank" href="https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g" style="background:none">\n    <img src="https://img.shields.io/badge/slack-join-dlt.svg?labelColor=191937&color=6F6FF7&logo=slack" />\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/v/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/pyversions/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n</div>\n\n## Installation\n\ndlt supports Python 3.8+.\n\n```bash\npip install dlt\n```\n\n## Quick Start\n\nLoad chess game data from chess.com API and save it in DuckDB:\n\n```python\nimport dlt\nfrom chess import chess # a utility function that grabs data from the chess.com API\n\n# create a dlt pipeline that will load chess game data to the DuckDB destination\npipeline = dlt.pipeline(\n    pipeline_name=\'chess_pipeline\',\n    destination=\'duckdb\',\n    dataset_name=\'games_data\'\n)\n\n# use chess.com API to grab data about a few players\ndata = chess([\'magnuscarlsen\', \'rpragchess\'], start_month=\'2022/11\', end_month=\'2022/12\')\n\n# extract, normalize, and load the data\npipeline.run(data)\n```\n\nTry it out in our **[Colab Demo](https://colab.research.google.com/drive/1NfSB1DpwbbHX9_t5vlalBTf13utwpMGx?usp=sharing)**\n\n## Features\n\n- **Automatic Schema:** Data structure inspection and schema creation for the destination.\n- **Data Normalization:** Consistent and verified data before loading.\n- **Seamless Integration:** Colab, AWS Lambda, Airflow, and local environments.\n- **Scalable:** Adapts to growing data needs in production.\n- **Easy Maintenance:** Clear data pipeline structure for updates.\n- **Rapid Exploration:** Quickly explore and gain insights from new data sources.\n- **Versatile Usage:** Suitable for ad-hoc exploration to advanced loading infrastructures.\n- **Start in Seconds with CLI:** Powerful CLI for managing, deploying and inspecting local pipelines.\n- **Incremental Loading:** Load only new or changed data and avoid loading old records again.\n- **Open Source:** Free and Apache 2.0 Licensed.\n\n## Ready to use Pipelines and Destinations\n\nExplore ready to use pipelines (e.g. Google Sheets) in the [Pipelines docs](https://dlthub.com/docs/pipelines/chess) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/destinations/bigquery).\n\n## Documentation\n\nFor detailed usage and configuration, please refer to the [official documentation](https://dlthub.com/docs).\n\n## Examples\n\nYou can find examples for various use cases in the [examples](docs/examples) folder.\n\n## Get Involved\n\nThe dlt project is quickly growing, and we\'re excited to have you join our community! Here\'s how you can get involved:\n\n- **Connect with the Community**: Join other dlt users and contributors on our [Slack](https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g)\n- **Report issues and suggest features**: Please use the [GitHub Issues](https://github.com/dlt-hub/dlt/issues) to report bugs or suggest new features. Before creating a new issue, make sure to search the tracker for possible duplicates and add a comment if you find one.\n- **Contribute Pipelines**: Pipelines are data processing steps that help move and transform data between various sources and destinations. Contribute your custom pipelines to the [dlt-hub/pipelines](https://github.com/dlt-hub/pipelines) to help other folks in handling their data tasks.\n- **Contribute code**: Check out our [contributing guidelines](CONTRIBUTING.md) for information on how to make a pull request.\n- **Improve documentation**: Help us enhance the dlt documentation.\n\n## License\n\nDLT is released under the [Apache 2.0 License](LICENSE.txt).\n',
     'author': 'dltHub Inc.',
     'author_email': 'services@dlthub.com',
     'maintainer': 'Marcin Rudolf',
     'maintainer_email': 'marcin@dlthub.com',
     'url': 'https://github.com/dlt-hub',
```

### Comparing `dlt-0.2.7/PKG-INFO` & `dlt-0.2.7a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlt
-Version: 0.2.7
+Version: 0.2.7a0
 Summary: DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.
 Home-page: https://github.com/dlt-hub
 License: Apache-2.0
 Keywords: etl
 Author: dltHub Inc.
 Author-email: services@dlthub.com
 Maintainer: Marcin Rudolf
```

