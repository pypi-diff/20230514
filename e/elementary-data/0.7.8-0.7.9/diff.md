# Comparing `tmp/elementary-data-0.7.8.tar.gz` & `tmp/elementary-data-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/elementary/elementary/dist/.tmp-en32z20k/elementary-data-0.7.8.tar", last modified: Thu Apr 27 12:29:21 2023, max compression
+gzip compressed data, was "/home/runner/work/elementary/elementary/dist/.tmp-pls4divk/elementary-data-0.7.9.tar", last modified: Sun May 14 15:31:58 2023, max compression
```

## Comparing `elementary-data-0.7.8.tar` & `elementary-data-0.7.9.tar`

### file list

```diff
@@ -1,289 +1,289 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/
--rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-04-27 12:29:03.000000 elementary-data-0.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-04-27 12:29:03.000000 elementary-data-0.7.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    14291 2023-04-27 12:29:21.000000 elementary-data-0.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    13412 2023-04-27 12:29:03.000000 elementary-data-0.7.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/cli/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)      658 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/cli/upgrade.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/clients/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/clients/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      453 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/api/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/clients/dbt/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1207 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/dbt/base_dbt_runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     7958 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/dbt/dbt_runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     5188 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/dbt/slim_dbt_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/clients/fetcher/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/fetcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      457 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/fetcher/fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/clients/gcs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/gcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3715 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/gcs/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/clients/s3/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5340 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/s3/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/clients/slack/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7387 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/slack/client.py
--rw-r--r--   0 runner    (1001) docker     (122)      967 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/slack/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     5552 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/clients/slack/slack_message_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/config/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7977 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/exceptions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4116 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7057 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/alerts/alert.py
--rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/alerts/alerts.py
--rw-r--r--   0 runner    (1001) docker     (122)    12986 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/alerts/group_of_alerts.py
--rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/alerts/malformed.py
--rw-r--r--   0 runner    (1001) docker     (122)     7697 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/alerts/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/alerts/schema/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/alerts/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      182 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/alerts/schema/alert.py
--rw-r--r--   0 runner    (1001) docker     (122)      418 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/alerts/schema/alert_group_component.py
--rw-r--r--   0 runner    (1001) docker     (122)      487 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/alerts/schema/test.py
--rw-r--r--   0 runner    (1001) docker     (122)     6284 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/alerts/source_freshness.py
--rw-r--r--   0 runner    (1001) docker     (122)    15821 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/alerts/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/api/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4854 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/alerts/alert_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     7770 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/alerts/alerts.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/api/filters/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4067 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/filters/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)      544 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/filters/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/api/invocations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/invocations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1448 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/invocations/invocations.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/invocations/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/api/lineage/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/lineage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2894 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/lineage/lineage.py
--rw-r--r--   0 runner    (1001) docker     (122)      937 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/lineage/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/api/models/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8094 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/models/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     3246 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/models/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/api/report/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6692 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/report/report.py
--rw-r--r--   0 runner    (1001) docker     (122)      602 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/report/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/api/selector/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/selector/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)      762 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/selector/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/api/sidebar/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/sidebar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/sidebar/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/sidebar/sidebar.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/api/test_management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/test_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/test_management/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     1440 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/test_management/test_management.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/api/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3849 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/tests/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)    19501 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/api/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (122)    19321 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/data_monitoring/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/data_monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6175 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/data_monitoring/data_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (122)    10139 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/data_monitoring/data_monitoring_alerts.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/data_monitoring/report/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/data_monitoring/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11666 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/data_monitoring/report/data_monitoring_report.py
--rw-r--r--   0 runner    (1001) docker     (122)  1674955 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/data_monitoring/report/index.html
--rw-r--r--   0 runner    (1001) docker     (122)     8142 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/data_monitoring/report/slack_report_summary_message_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/data_monitoring/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     4191 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/data_monitoring/selector_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      571 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/analyses/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/analyses/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/empty_alert_tables.sql
--rw-r--r--   0 runner    (1001) docker     (122)     6956 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/get_model_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/get_new_alerts_where_clause.sql
--rw-r--r--   0 runner    (1001) docker     (122)     6387 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/get_source_freshness_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)     7646 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/get_test_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      598 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/update_sent_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/update_skipped_alerts.sql
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/base_queries/
--rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/base_queries/current_tests_run_results_query.sql
--rw-r--r--   0 runner    (1001) docker     (122)      827 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/base_queries/owners.sql
--rw-r--r--   0 runner    (1001) docker     (122)     2471 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/base_queries/resources.sql
--rw-r--r--   0 runner    (1001) docker     (122)      649 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/base_queries/tags.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/base_queries/tests.sql
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_adapter_type_and_unique_id.sql
--rw-r--r--   0 runner    (1001) docker     (122)      305 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_alerts_time_limit.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1149 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_dbt_models_test_coverage.sql
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_elementary_database_and_schema.sql
--rw-r--r--   0 runner    (1001) docker     (122)      324 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_elementary_table_nodes.sql
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_exposures.sql
--rw-r--r--   0 runner    (1001) docker     (122)      678 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_latest_invocation.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_models.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_models_runs.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_nodes_depends_on_nodes.sql
--rw-r--r--   0 runner    (1001) docker     (122)      434 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_result_rows_agate.sql
--rw-r--r--   0 runner    (1001) docker     (122)      991 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_sources.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_test_last_invocation.sql
--rw-r--r--   0 runner    (1001) docker     (122)     5345 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_test_results.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1132 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_test_rows_sample.sql
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/materializations/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (122)      828 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/test_conn.sql
--rw-r--r--   0 runner    (1001) docker     (122)      390 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/macros/upload_source_freshness.sql
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/models/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/models/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/models/alerts/alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/models/alerts/alerts_models.sql
--rw-r--r--   0 runner    (1001) docker     (122)      723 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/models/alerts/alerts_source_freshness.sql
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/packages.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/snapshots/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/snapshots/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (122)     2065 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/dbt_project_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      865 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/fetchers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/fetchers/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6140 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/alerts/alerts.py
--rw-r--r--   0 runner    (1001) docker     (122)     5125 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/alerts/normalized_alert.py
--rw-r--r--   0 runner    (1001) docker     (122)      161 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/base_fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/fetchers/invocations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/invocations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      859 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/invocations/invocations.py
--rw-r--r--   0 runner    (1001) docker     (122)      765 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/invocations/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/fetchers/lineage/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/lineage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/lineage/lineage.py
--rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/lineage/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/fetchers/models/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2646 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/models/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     2362 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/models/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/fetchers/selector/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/selector/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)      336 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/selector/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/fetchers/test_management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/test_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1703 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/test_management/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     6135 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/test_management/test_management.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/monitor/fetchers/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2639 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/tests/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/monitor/fetchers/tests/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/operations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/operations/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/operations/upload_source_freshness.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/tracking/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6159 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/tracking/anonymous_tracking.py
--rw-r--r--   0 runner    (1001) docker     (122)     1011 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/tracking/runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/tracking/tracking_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      387 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/utils/bucket_path.py
--rw-r--r--   0 runner    (1001) docker     (122)      934 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/utils/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/utils/env_vars.py
--rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/utils/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1744 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (122)      201 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/utils/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/utils/ordered_yaml.py
--rw-r--r--   0 runner    (1001) docker     (122)      527 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/utils/package.py
--rw-r--r--   0 runner    (1001) docker     (122)      766 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/utils/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     2748 2023-04-27 12:29:03.000000 elementary-data-0.7.8/elementary/utils/time.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14291 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9870 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary_data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      756 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-27 12:29:21.000000 elementary-data-0.7.8/elementary_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-27 12:29:21.000000 elementary-data-0.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2331 2023-04-27 12:29:03.000000 elementary-data-0.7.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/integration/monitor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/integration/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/integration/monitor/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/integration/monitor/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/integration/monitor/api/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/integration/monitor/api/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/integration/monitor/api/alerts/test_alerts_fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/integration/monitor/api/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/integration/monitor/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/integration/monitor/api/tests/test_tests_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/mocks/anonymous_tracking_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/mocks/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/mocks/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      537 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/mocks/api/alerts_api_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      438 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/mocks/api/invocations_api_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      784 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/mocks/api/tests_api_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      278 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/mocks/dbt_runner_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/mocks/fetchers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/mocks/fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19060 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/mocks/fetchers/alerts_fetcher_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/mocks/fetchers/invocations_fetcher_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/mocks/fetchers/selector_fetcher_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)     8394 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/mocks/fetchers/tests_fetcher_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/unit/monitor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/unit/monitor/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/alerts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/unit/monitor/alerts/group_alerts_by_table/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/alerts/group_alerts_by_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      944 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/alerts/group_alerts_by_table/mock_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     3180 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/alerts/group_alerts_by_table/mock_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    12236 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/alerts/group_alerts_by_table/test_slack_alerts_group_by.py
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/alerts/group_alerts_by_table/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      927 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/alerts/test_malformed_alert.py
--rw-r--r--   0 runner    (1001) docker     (122)     7565 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/alerts/test_normalized_alert.py
--rw-r--r--   0 runner    (1001) docker     (122)     7348 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/alerts/test_slack_alert_message_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/unit/monitor/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/unit/monitor/api/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/api/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12260 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/api/alerts/test_alert_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     1919 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/api/alerts/test_alerts_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/unit/monitor/api/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/api/tests/test_tests_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/unit/monitor/data_monitoring/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/data_monitoring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/unit/monitor/data_monitoring/report/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/data_monitoring/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7894 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/data_monitoring/report/test_slack_report_summary_message_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     5152 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/data_monitoring/test_selector_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:21.000000 elementary-data-0.7.8/tests/unit/monitor/fetchers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2229 2023-04-27 12:29:03.000000 elementary-data-0.7.8/tests/unit/monitor/fetchers/test_alerts_fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/
+-rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-05-14 15:31:45.000000 elementary-data-0.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-05-14 15:31:45.000000 elementary-data-0.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    14431 2023-05-14 15:31:58.000000 elementary-data-0.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13552 2023-05-14 15:31:45.000000 elementary-data-0.7.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)      658 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/cli/upgrade.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/clients/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/clients/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/clients/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/clients/api/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/clients/dbt/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/clients/dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1207 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/clients/dbt/base_dbt_runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7958 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/clients/dbt/dbt_runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5188 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/clients/dbt/slim_dbt_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/clients/fetcher/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/clients/fetcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/clients/fetcher/fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/clients/gcs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/clients/gcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3715 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/clients/gcs/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/clients/s3/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/clients/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5340 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/clients/s3/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/clients/slack/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/clients/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7915 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/clients/slack/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      967 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/clients/slack/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5552 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/clients/slack/slack_message_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/config/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7977 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4116 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7057 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/alerts/alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/alerts/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12986 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/alerts/group_of_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/alerts/malformed.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7697 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/alerts/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/alerts/schema/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/alerts/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/alerts/schema/alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)      418 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/alerts/schema/alert_group_component.py
+-rw-r--r--   0 runner    (1001) docker     (122)      487 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/alerts/schema/test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6284 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/alerts/source_freshness.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15821 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/alerts/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/api/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4854 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/alerts/alert_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7770 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/alerts/alerts.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/api/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4067 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/filters/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      544 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/filters/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/api/invocations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/invocations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1448 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/invocations/invocations.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/invocations/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/api/lineage/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/lineage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2894 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/lineage/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/lineage/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/api/models/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8094 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3246 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/models/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/api/report/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6692 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/report/report.py
+-rw-r--r--   0 runner    (1001) docker     (122)      602 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/report/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/api/selector/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/selector/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/selector/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/api/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/sidebar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/sidebar/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/sidebar/sidebar.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/api/test_management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/test_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/test_management/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1440 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/test_management/test_management.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3849 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/tests/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19313 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/api/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19321 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/data_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/data_monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6173 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/data_monitoring/data_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10139 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/data_monitoring/data_monitoring_alerts.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/data_monitoring/report/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/data_monitoring/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11666 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/data_monitoring/report/data_monitoring_report.py
+-rw-r--r--   0 runner    (1001) docker     (122)  1674955 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/data_monitoring/report/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)     8142 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/data_monitoring/report/slack_report_summary_message_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/data_monitoring/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4191 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/data_monitoring/selector_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      571 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/analyses/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/analyses/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/alerts/empty_alert_tables.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     6956 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/alerts/get_model_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/alerts/get_new_alerts_where_clause.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     6387 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/alerts/get_source_freshness_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     7562 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/alerts/get_test_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      598 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/alerts/update_sent_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/alerts/update_skipped_alerts.sql
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/base_queries/
+-rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/base_queries/current_tests_run_results_query.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      827 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/base_queries/owners.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     2471 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/base_queries/resources.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      649 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/base_queries/tags.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/base_queries/tests.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/get_adapter_type_and_unique_id.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      305 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/get_alerts_time_limit.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1149 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/get_dbt_models_test_coverage.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/get_elementary_database_and_schema.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      324 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/get_elementary_table_nodes.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/get_exposures.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      678 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/get_latest_invocation.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/get_models.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/get_models_runs.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/get_nodes_depends_on_nodes.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/get_result_rows_agate.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      991 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/get_sources.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/get_test_last_invocation.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     5261 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/get_test_results.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      683 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/get_test_rows_sample.sql
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/materializations/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      828 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/test_conn.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      390 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/macros/upload_source_freshness.sql
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/models/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/models/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/models/alerts/alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/models/alerts/alerts_models.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/models/alerts/alerts_source_freshness.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/packages.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/snapshots/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (122)     2065 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/dbt_project_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      865 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/fetchers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/fetchers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/fetchers/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/fetchers/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6140 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/fetchers/alerts/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5173 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/fetchers/alerts/normalized_alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/fetchers/base_fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/fetchers/invocations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/fetchers/invocations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      859 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/fetchers/invocations/invocations.py
+-rw-r--r--   0 runner    (1001) docker     (122)      765 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/fetchers/invocations/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/fetchers/lineage/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/fetchers/lineage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/fetchers/lineage/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/fetchers/lineage/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/fetchers/models/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/fetchers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2646 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/fetchers/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2362 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/fetchers/models/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/fetchers/selector/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/fetchers/selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/fetchers/selector/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)      336 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/fetchers/selector/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/fetchers/test_management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/fetchers/test_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/fetchers/test_management/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6401 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/fetchers/test_management/test_management.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/monitor/fetchers/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/fetchers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2639 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/fetchers/tests/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1249 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/monitor/fetchers/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/operations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/operations/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/operations/upload_source_freshness.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/tracking/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6159 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/tracking/anonymous_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1011 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/tracking/runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/tracking/tracking_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      387 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/utils/bucket_path.py
+-rw-r--r--   0 runner    (1001) docker     (122)      934 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/utils/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/utils/env_vars.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/utils/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1744 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)      201 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/utils/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/utils/ordered_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (122)      527 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/utils/package.py
+-rw-r--r--   0 runner    (1001) docker     (122)      865 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/utils/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2748 2023-05-14 15:31:45.000000 elementary-data-0.7.9/elementary/utils/time.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14431 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9870 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary_data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-14 15:31:58.000000 elementary-data-0.7.9/elementary_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-14 15:31:58.000000 elementary-data-0.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2331 2023-05-14 15:31:45.000000 elementary-data-0.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/tests/integration/monitor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/integration/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/tests/integration/monitor/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/integration/monitor/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/tests/integration/monitor/api/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/integration/monitor/api/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/integration/monitor/api/alerts/test_alerts_fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/tests/integration/monitor/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/integration/monitor/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/integration/monitor/api/tests/test_tests_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/mocks/anonymous_tracking_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/tests/mocks/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/mocks/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/mocks/api/alerts_api_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/mocks/api/invocations_api_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      784 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/mocks/api/tests_api_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      278 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/mocks/dbt_runner_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/tests/mocks/fetchers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/mocks/fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19060 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/mocks/fetchers/alerts_fetcher_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/mocks/fetchers/invocations_fetcher_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/mocks/fetchers/selector_fetcher_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8394 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/mocks/fetchers/tests_fetcher_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/tests/unit/monitor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/unit/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/tests/unit/monitor/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/unit/monitor/alerts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/tests/unit/monitor/alerts/group_alerts_by_table/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/unit/monitor/alerts/group_alerts_by_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      944 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/unit/monitor/alerts/group_alerts_by_table/mock_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3180 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/unit/monitor/alerts/group_alerts_by_table/mock_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12236 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/unit/monitor/alerts/group_alerts_by_table/test_slack_alerts_group_by.py
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/unit/monitor/alerts/group_alerts_by_table/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      927 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/unit/monitor/alerts/test_malformed_alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7565 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/unit/monitor/alerts/test_normalized_alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7348 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/unit/monitor/alerts/test_slack_alert_message_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/tests/unit/monitor/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/unit/monitor/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/tests/unit/monitor/api/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/unit/monitor/api/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12260 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/unit/monitor/api/alerts/test_alert_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1919 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/unit/monitor/api/alerts/test_alerts_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/tests/unit/monitor/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/unit/monitor/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/unit/monitor/api/tests/test_tests_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/tests/unit/monitor/data_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/unit/monitor/data_monitoring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/tests/unit/monitor/data_monitoring/report/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/unit/monitor/data_monitoring/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7894 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/unit/monitor/data_monitoring/report/test_slack_report_summary_message_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5152 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/unit/monitor/data_monitoring/test_selector_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:58.000000 elementary-data-0.7.9/tests/unit/monitor/fetchers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/unit/monitor/fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2229 2023-05-14 15:31:46.000000 elementary-data-0.7.9/tests/unit/monitor/fetchers/test_alerts_fetcher.py
```

### Comparing `elementary-data-0.7.8/LICENSE` & `elementary-data-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/PKG-INFO` & `elementary-data-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elementary-data
-Version: 0.7.8
+Version: 0.7.9
 Summary: Data monitoring and lineage
 Home-page: https://github.com/elementary-data/elementary
 Author: Elementary
 Author-email: or@elementary-data.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
@@ -199,12 +199,13 @@
 <a href="https://github.com/tc-chrisbui"><img src="https://avatars.githubusercontent.com/u/115048867?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/vishaalkk"><img src="https://avatars.githubusercontent.com/u/13641827?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/sadahry"><img src="https://avatars.githubusercontent.com/u/28292300?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/will-warner"><img src="https://avatars.githubusercontent.com/u/110092386?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/winzee"><img src="https://avatars.githubusercontent.com/u/1001577?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/vinooganesh"><img src="https://avatars.githubusercontent.com/u/2461070?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/dimoschi"><img src="https://avatars.githubusercontent.com/u/13113025?v=4" width="50" height="50" alt=""/></a>
+<a href="https://github.com/manulpatel"><img src="https://avatars.githubusercontent.com/u/77568048?v=4" width="50" height="50" alt=""/></a>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: elementary-data Version: 0.7.8 Summary: Data
+Metadata-Version: 2.1 Name: elementary-data Version: 0.7.9 Summary: Data
 monitoring and lineage Home-page: https://github.com/elementary-data/elementary
 Author: Elementary Author-email: or@elementary-data.com Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System ::
 Microsoft :: Windows Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
 :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `elementary-data-0.7.8/README.md` & `elementary-data-0.7.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -173,12 +173,13 @@
 <a href="https://github.com/tc-chrisbui"><img src="https://avatars.githubusercontent.com/u/115048867?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/vishaalkk"><img src="https://avatars.githubusercontent.com/u/13641827?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/sadahry"><img src="https://avatars.githubusercontent.com/u/28292300?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/will-warner"><img src="https://avatars.githubusercontent.com/u/110092386?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/winzee"><img src="https://avatars.githubusercontent.com/u/1001577?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/vinooganesh"><img src="https://avatars.githubusercontent.com/u/2461070?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/dimoschi"><img src="https://avatars.githubusercontent.com/u/13113025?v=4" width="50" height="50" alt=""/></a>
+<a href="https://github.com/manulpatel"><img src="https://avatars.githubusercontent.com/u/77568048?v=4" width="50" height="50" alt=""/></a>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

### Comparing `elementary-data-0.7.8/elementary/cli/cli.py` & `elementary-data-0.7.9/elementary/cli/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -63,13 +63,21 @@
             "Any feedback and suggestions are welcomed! join our community here - "
             "https://bit.ly/slack-elementary\n"
         )
         logger.info(f"Running with edr={package.get_package_version()}")
         return super().invoke(ctx)
 
 
-cli = ElementaryCLI(
-    help="Open source data reliability solution (https://docs.elementary-data.com/)"
+@click.command(
+    cls=ElementaryCLI,
+    help="Open source data reliability solution (https://docs.elementary-data.com/)",
 )
+@click.version_option(
+    version=package.get_package_version(),
+    message="Elementary version %(version)s.",
+)
+def cli():
+    pass
+
 
 if __name__ == "__main__":
     cli()
```

### Comparing `elementary-data-0.7.8/elementary/cli/upgrade.py` & `elementary-data-0.7.9/elementary/cli/upgrade.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/clients/dbt/base_dbt_runner.py` & `elementary-data-0.7.9/elementary/clients/dbt/base_dbt_runner.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/clients/dbt/dbt_runner.py` & `elementary-data-0.7.9/elementary/clients/dbt/dbt_runner.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/clients/dbt/slim_dbt_runner.py` & `elementary-data-0.7.9/elementary/clients/dbt/slim_dbt_runner.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/clients/gcs/client.py` & `elementary-data-0.7.9/elementary/clients/gcs/client.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/clients/s3/client.py` & `elementary-data-0.7.9/elementary/clients/s3/client.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/clients/slack/client.py` & `elementary-data-0.7.9/elementary/clients/slack/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from abc import ABC, abstractmethod
-from typing import Optional
+from typing import List, Optional, Tuple
 
 from ratelimit import limits, sleep_and_retry
 from slack_sdk import WebClient, WebhookClient
 from slack_sdk.errors import SlackApiError
 from slack_sdk.http_retry.builtin_handlers import RateLimitErrorRetryHandler
 
 from elementary.clients.slack.schema import SlackMessageSchema
@@ -133,45 +133,60 @@
                 user_id = self.client.users_lookupByEmail(email=email)["user"]["id"]
                 self.email_to_user_id_cache[email] = user_id
             return self.email_to_user_id_cache[email]
         except SlackApiError as err:
             logger.error(f"Unable to get Slack user ID from email: {err}.")
             return None
 
+    @sleep_and_retry
+    @limits(calls=20, period=ONE_MINUTE)
+    def _get_channels(
+        self, cursor: Optional[str] = None
+    ) -> Tuple[List[dict], Optional[str]]:
+        response = self.client.conversations_list(
+            cursor=cursor,
+            types="public_channel,private_channel",
+            exclude_archived=True,
+            limit=1000,
+        )
+        channels = response["channels"]
+        cursor = response.get("response_metadata", {}).get("next_cursor")
+        return channels, cursor
+
     def _get_channel_id(self, channel_name: str) -> Optional[str]:
         cursor = None
         while True:
-            response = self.client.conversations_list(
-                cursor=cursor,
-                types="public_channel,private_channel",
-                exclude_archived=True,
-                limit=1000,
-            )
-            for channel in response["channels"]:
+            channels, cursor = self._get_channels(cursor)
+            for channel in channels:
                 if channel["name"] == channel_name:
                     return channel["id"]
-            cursor = response.get("response_metadata", {}).get("next_cursor")
             if not cursor:
                 return None
 
     def _join_channel(self, channel_id: str) -> bool:
         try:
             self.client.conversations_join(channel=channel_id)
+            logger.info("Elementary app joined the channel successfully.")
             return True
         except SlackApiError as e:
             logger.error(f"Elementary app failed to join the given channel. Error: {e}")
             self.tracking.record_internal_exception(e)
             return False
 
     def _handle_send_err(self, err: SlackApiError, channel_name: str) -> bool:
         err_type = err.response.data["error"]
         if err_type == "not_in_channel":
-            logger.info("Elementary app is not in the channel. Attempting to join.")
+            logger.info(
+                f'Elementary app is not in the channel "{channel_name}". Attempting to join.'
+            )
             channel_id = self._get_channel_id(channel_name)
             if not channel_id:
+                logger.info(
+                    f'Elementary app could not find the channel "{channel_name}".'
+                )
                 return False
             return self._join_channel(channel_id=channel_id)
         elif err_type == "channel_not_found":
             logger.error(
                 f"Channel {channel_name} was not found by the Elementary app. Please add the app to the channel."
             )
             return False
```

### Comparing `elementary-data-0.7.8/elementary/clients/slack/schema.py` & `elementary-data-0.7.9/elementary/clients/slack/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/clients/slack/slack_message_builder.py` & `elementary-data-0.7.9/elementary/clients/slack/slack_message_builder.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/config/config.py` & `elementary-data-0.7.9/elementary/config/config.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/exceptions/exceptions.py` & `elementary-data-0.7.9/elementary/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/alerts/alert.py` & `elementary-data-0.7.9/elementary/monitor/alerts/alert.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/alerts/alerts.py` & `elementary-data-0.7.9/elementary/monitor/alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/alerts/group_of_alerts.py` & `elementary-data-0.7.9/elementary/monitor/alerts/group_of_alerts.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/alerts/malformed.py` & `elementary-data-0.7.9/elementary/monitor/alerts/malformed.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/alerts/model.py` & `elementary-data-0.7.9/elementary/monitor/alerts/model.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/alerts/source_freshness.py` & `elementary-data-0.7.9/elementary/monitor/alerts/source_freshness.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/alerts/test.py` & `elementary-data-0.7.9/elementary/monitor/alerts/test.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/api/alerts/alert_filters.py` & `elementary-data-0.7.9/elementary/monitor/api/alerts/alert_filters.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/api/alerts/alerts.py` & `elementary-data-0.7.9/elementary/monitor/api/alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/api/filters/filters.py` & `elementary-data-0.7.9/elementary/monitor/api/filters/filters.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/api/filters/schema.py` & `elementary-data-0.7.9/elementary/monitor/api/filters/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/api/invocations/invocations.py` & `elementary-data-0.7.9/elementary/monitor/api/invocations/invocations.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/api/lineage/lineage.py` & `elementary-data-0.7.9/elementary/monitor/api/lineage/lineage.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/api/lineage/schema.py` & `elementary-data-0.7.9/elementary/monitor/api/lineage/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/api/models/models.py` & `elementary-data-0.7.9/elementary/monitor/api/models/models.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/api/models/schema.py` & `elementary-data-0.7.9/elementary/monitor/api/models/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/api/report/report.py` & `elementary-data-0.7.9/elementary/monitor/api/report/report.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/api/report/schema.py` & `elementary-data-0.7.9/elementary/monitor/api/report/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/api/selector/selector.py` & `elementary-data-0.7.9/elementary/monitor/api/selector/selector.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/api/sidebar/sidebar.py` & `elementary-data-0.7.9/elementary/monitor/api/sidebar/sidebar.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/api/test_management/test_management.py` & `elementary-data-0.7.9/elementary/monitor/api/test_management/test_management.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/api/tests/schema.py` & `elementary-data-0.7.9/elementary/monitor/api/tests/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/api/tests/tests.py` & `elementary-data-0.7.9/elementary/monitor/api/tests/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,38 +32,34 @@
 
 class TestsAPI(APIClient):
     def __init__(
         self,
         dbt_runner: DbtRunner,
         days_back: Optional[int] = 7,
         invocations_per_test: int = 720,
-        metrics_sample_limit: int = 5,
         disable_passed_test_metrics: bool = False,
     ):
         super().__init__(dbt_runner)
         self.tests_fetcher = TestsFetcher(dbt_runner=self.dbt_runner)
         self.invocations_api = InvocationsAPI(dbt_runner)
         self.test_results_db_rows = self._get_test_results_db_rows(
             days_back=days_back,
             invocations_per_test=invocations_per_test,
-            metrics_sample_limit=metrics_sample_limit,
             disable_passed_test_metrics=disable_passed_test_metrics,
         )
 
     def _get_test_results_db_rows(
         self,
         days_back: Optional[int] = 7,
         invocations_per_test: int = 720,
-        metrics_sample_limit: int = 5,
         disable_passed_test_metrics: bool = False,
     ) -> List[TestResultDBRowSchema]:
         return self.tests_fetcher.get_all_test_results_db_rows(
             days_back=days_back,
             invocations_per_test=invocations_per_test,
-            metrics_sample_limit=metrics_sample_limit,
             disable_passed_test_metrics=disable_passed_test_metrics,
         )
 
     def get_test_results_summary(
         self,
         filter: SelectorFilterSchema = SelectorFilterSchema(),
     ) -> List[TestResultSummarySchema]:
```

### Comparing `elementary-data-0.7.8/elementary/monitor/cli.py` & `elementary-data-0.7.9/elementary/monitor/cli.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/data_monitoring/data_monitoring.py` & `elementary-data-0.7.9/elementary/monitor/data_monitoring/data_monitoring.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,9 +145,9 @@
                 f"You are using incompatible versions between edr ({py_pkg_ver}) and Elementary's dbt package ({dbt_pkg_ver}).\n "
                 "To fix please update your packages.yml, and run:\n"
                 "dbt deps && dbt run --select elementary\n",
             )
             return
 
         logger.info(
-            f"edr ({py_pkg_ver}) and Elementary's dbt package ({dbt_pkg_ver}) are compatible :)"
+            f"edr ({py_pkg_ver}) and Elementary's dbt package ({dbt_pkg_ver}) are compatible."
         )
```

### Comparing `elementary-data-0.7.8/elementary/monitor/data_monitoring/data_monitoring_alerts.py` & `elementary-data-0.7.9/elementary/monitor/data_monitoring/data_monitoring_alerts.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/data_monitoring/report/data_monitoring_report.py` & `elementary-data-0.7.9/elementary/monitor/data_monitoring/report/data_monitoring_report.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/data_monitoring/report/index.html` & `elementary-data-0.7.9/elementary/monitor/data_monitoring/report/index.html`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/data_monitoring/report/slack_report_summary_message_builder.py` & `elementary-data-0.7.9/elementary/monitor/data_monitoring/report/slack_report_summary_message_builder.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/data_monitoring/schema.py` & `elementary-data-0.7.9/elementary/monitor/data_monitoring/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/data_monitoring/selector_filter.py` & `elementary-data-0.7.9/elementary/monitor/data_monitoring/selector_filter.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/dbt_project/README.md` & `elementary-data-0.7.9/elementary/monitor/dbt_project/README.md`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/dbt_project/dbt_project.yml` & `elementary-data-0.7.9/elementary/monitor/dbt_project/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/empty_alert_tables.sql` & `elementary-data-0.7.9/elementary/monitor/dbt_project/macros/alerts/empty_alert_tables.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/get_model_alerts.sql` & `elementary-data-0.7.9/elementary/monitor/dbt_project/macros/alerts/get_model_alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/get_new_alerts_where_clause.sql` & `elementary-data-0.7.9/elementary/monitor/dbt_project/macros/alerts/get_new_alerts_where_clause.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/get_source_freshness_alerts.sql` & `elementary-data-0.7.9/elementary/monitor/dbt_project/macros/alerts/get_source_freshness_alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/get_test_alerts.sql` & `elementary-data-0.7.9/elementary/monitor/dbt_project/macros/alerts/get_test_alerts.sql`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% macro get_pending_test_alerts(days_back, results_sample_limit=5, disable_samples=false) %}
+{% macro get_pending_test_alerts(days_back, disable_samples=false) %}
     -- depends_on: {{ ref('alerts') }}
     {% set select_pending_alerts_query %}
         with alerts_in_time_limit as (
             select * from {{ ref('alerts') }}
             where {{ elementary.edr_cast_as_timestamp('detected_at') }} >= {{ get_alerts_time_limit(days_back) }}
         ),
 
@@ -76,15 +76,15 @@
     {% set pending_alerts = [] %}
     {% for alert in test_result_alert_dicts %}
         {% set test_type = alert.alert_type %}
         {% set status = alert.status | lower %}
 
         {% set test_rows_sample = none %}
         {%- if not disable_samples and ((test_type == 'dbt_test' and status in ['fail', 'warn']) or (test_type != 'dbt_test' and status != 'error')) -%}
-            {% set test_rows_sample = elementary_internal.get_test_rows_sample(alert.result_rows, test_result_rows_agate.get(alert.alert_id), test_type, alert.alert_results_query, results_sample_limit) %}
+            {% set test_rows_sample = elementary_internal.get_test_rows_sample(alert.result_rows, test_result_rows_agate.get(alert.alert_id)) %}
         {%- endif -%}
         {% set pending_alert_dict = {'id': alert.alert_id,
                                  'alert_class_id': alert.alert_class_id,
                                  'model_unique_id': alert.model_unique_id,
                                  'test_unique_id': alert.test_unique_id,
                                  'detected_at': alert.detected_at,
                                  'database_name': alert.database_name,
```

### Comparing `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/update_sent_alerts.sql` & `elementary-data-0.7.9/elementary/monitor/dbt_project/macros/alerts/update_sent_alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/alerts/update_skipped_alerts.sql` & `elementary-data-0.7.9/elementary/monitor/dbt_project/macros/alerts/update_skipped_alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/base_queries/current_tests_run_results_query.sql` & `elementary-data-0.7.9/elementary/monitor/dbt_project/macros/base_queries/current_tests_run_results_query.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/base_queries/owners.sql` & `elementary-data-0.7.9/elementary/monitor/dbt_project/macros/base_queries/owners.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/base_queries/resources.sql` & `elementary-data-0.7.9/elementary/monitor/dbt_project/macros/base_queries/resources.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/base_queries/tags.sql` & `elementary-data-0.7.9/elementary/monitor/dbt_project/macros/base_queries/tags.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_dbt_models_test_coverage.sql` & `elementary-data-0.7.9/elementary/monitor/dbt_project/macros/get_dbt_models_test_coverage.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_exposures.sql` & `elementary-data-0.7.9/elementary/monitor/dbt_project/macros/get_exposures.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_latest_invocation.sql` & `elementary-data-0.7.9/elementary/monitor/dbt_project/macros/get_latest_invocation.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_models.sql` & `elementary-data-0.7.9/elementary/monitor/dbt_project/macros/get_models.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_models_runs.sql` & `elementary-data-0.7.9/elementary/monitor/dbt_project/macros/get_models_runs.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_nodes_depends_on_nodes.sql` & `elementary-data-0.7.9/elementary/monitor/dbt_project/macros/get_nodes_depends_on_nodes.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_sources.sql` & `elementary-data-0.7.9/elementary/monitor/dbt_project/macros/get_sources.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_test_last_invocation.sql` & `elementary-data-0.7.9/elementary/monitor/dbt_project/macros/get_test_last_invocation.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_test_results.sql` & `elementary-data-0.7.9/elementary/monitor/dbt_project/macros/get_test_results.sql`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{%- macro get_test_results(days_back = 7, metrics_sample_limit = 5, invocations_per_test = 720, disable_passed_test_metrics = false) -%}
+{%- macro get_test_results(days_back = 7, invocations_per_test = 720, disable_passed_test_metrics = false) -%}
     {% set select_test_results %}
         with test_results as (
             {{ elementary_internal.current_tests_run_results_query(days_back=days_back) }}
         ),
 
         ordered_test_results as (
             select
@@ -59,15 +59,15 @@
             {% set status = test.status | lower %}
 
             {% set elementary_tests_allowlist_status = ['fail', 'warn']  %}
             {% if not disable_passed_test_metrics %}
                 {% do elementary_tests_allowlist_status.append('pass') %}
             {% endif %}
             {%- if (test_type == 'dbt_test' and status in ['fail', 'warn']) or (test_type != 'dbt_test' and status in elementary_tests_allowlist_status) -%}
-                {% set test_rows_sample = elementary_internal.get_test_rows_sample(test.result_rows, test_result_rows_agate.get(test.id), test_type, test.test_results_query, metrics_sample_limit) %}
+                {% set test_rows_sample = elementary_internal.get_test_rows_sample(test.result_rows, test_result_rows_agate.get(test.id)) %}
                 {# Dimension anomalies return multiple dimensions for the test rows sample, and needs to be handle differently. #}
                 {# Currently we show only the anomalous for all of the dimensions. #}
                 {% if test.test_sub_type == 'dimension' %}
                     {% set anomalous_rows = [] %}
                     {% set headers = [{'id': 'anomalous_value_timestamp', 'display_name': 'timestamp', 'type': 'date'}] %}
                     {% for row in test_rows_sample %}
                         {% set anomalous_row = {
```

### Comparing `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/get_test_rows_sample.sql` & `elementary-data-0.7.9/elementary/monitor/dbt_project/macros/get_test_rows_sample.sql`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,19 @@
 {#
   Sources of parameters:
   legacy_result_rows: elementary_test_results.result_rows
   result_rows_agate: test_result_rows
 #}
-{%- macro get_test_rows_sample(legacy_result_rows, result_rows_agate, test_type, test_query, results_sample_limit=5) -%}
-    {% set should_limit_sample = test_type == 'dbt_test' %}
+{%- macro get_test_rows_sample(legacy_result_rows, result_rows_agate) -%}
 
+    {% set result_rows = [] %}
     {% if legacy_result_rows is defined and legacy_result_rows is not none %}
         {% set result_rows = fromjson(legacy_result_rows) %}
-        {% if should_limit_sample %}
-            {% do return(result_rows[:results_sample_limit]) %}
-        {% endif %}
-        {% do return(result_rows) %}
-    {% endif %}
-
-    {% if result_rows_agate %}
-        {% set result_rows = [] %}
+    {% elif result_rows_agate %}
         {% set result_row_column = result_rows_agate.columns["result_row"] %}
-        {% if should_limit_sample %}
-            {% set result_row_column = result_row_column[:results_sample_limit] %}
-        {% endif %}
         {% for result_row in result_row_column %}
             {% do result_rows.append(fromjson(result_row)) %}
         {% endfor %}
-        {{ return(result_rows) }}
     {% endif %}
 
-    {% do return([]) %}
+    {% do return(result_rows) %}
 {%- endmacro -%}
```

### Comparing `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/materializations/incremental.sql` & `elementary-data-0.7.9/elementary/monitor/dbt_project/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/dbt_project/macros/materializations/table.sql` & `elementary-data-0.7.9/elementary/monitor/dbt_project/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/dbt_project/models/alerts/alerts.sql` & `elementary-data-0.7.9/elementary/monitor/dbt_project/models/alerts/alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/dbt_project/models/alerts/alerts_models.sql` & `elementary-data-0.7.9/elementary/monitor/dbt_project/models/alerts/alerts_models.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/dbt_project/models/alerts/alerts_source_freshness.sql` & `elementary-data-0.7.9/elementary/monitor/dbt_project/models/alerts/alerts_source_freshness.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/dbt_project_utils.py` & `elementary-data-0.7.9/elementary/monitor/dbt_project_utils.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/debug.py` & `elementary-data-0.7.9/elementary/monitor/debug.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/fetchers/alerts/alerts.py` & `elementary-data-0.7.9/elementary/monitor/fetchers/alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/fetchers/alerts/normalized_alert.py` & `elementary-data-0.7.9/elementary/monitor/fetchers/alerts/normalized_alert.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,17 @@
             normalized_alert[
                 ALERT_SUPRESSION_INTERVAL_KEY
             ] = self._get_alert_suppression_interval()
             normalized_alert[ALERT_FIELDS_KEY] = self._get_alert_fields()
 
             normalized_alert[
                 SLACK_GROUP_ALERTS_BY_KEY
-            ] = self._get_field_from_test_meta_or_model_meta_or_default(key="group")
+            ] = self._get_field_from_test_meta_or_model_meta_or_default(
+                key=SLACK_GROUP_ALERTS_BY_KEY
+            )
 
             return normalized_alert
         except Exception:
             logger.error(
                 f"Failed to extract alert subscribers and alert custom slack channel {self.alert.get('id')}. Ignoring it for now and main slack channel will be used"
             )
             return self.alert
```

### Comparing `elementary-data-0.7.8/elementary/monitor/fetchers/invocations/invocations.py` & `elementary-data-0.7.9/elementary/monitor/fetchers/invocations/invocations.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/fetchers/invocations/schema.py` & `elementary-data-0.7.9/elementary/monitor/fetchers/invocations/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/fetchers/lineage/lineage.py` & `elementary-data-0.7.9/elementary/monitor/fetchers/lineage/lineage.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/fetchers/lineage/schema.py` & `elementary-data-0.7.9/elementary/monitor/fetchers/lineage/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/fetchers/models/models.py` & `elementary-data-0.7.9/elementary/monitor/fetchers/models/models.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/fetchers/models/schema.py` & `elementary-data-0.7.9/elementary/monitor/fetchers/models/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/fetchers/test_management/schema.py` & `elementary-data-0.7.9/elementary/monitor/fetchers/test_management/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,22 +22,25 @@
     sources: List[ResourceModel] = Field(default_factory=list)
 
 
 class TestModel(BaseModel):
     id: str
     db_schema: str = Field(alias="schema")
     table: Optional[str]
+    source_name: Optional[str]
     column: Optional[str]
     package: Optional[str] = None
     name: str
     type: Optional[str]
     args: Optional[dict]
     severity: str
     owners: List[str] = Field(default_factory=list)
     tags: List[str] = Field(default_factory=list)
+    description: Optional[str]
+    is_singular: bool
     updated_at: str
     updated_by: Optional[str]
 
     @validator("severity", pre=True)
     def validate_severity(cls, severity: str):
         severity_lower_string = severity.lower()
         if severity_lower_string not in ["error", "warn"]:
```

### Comparing `elementary-data-0.7.8/elementary/monitor/fetchers/test_management/test_management.py` & `elementary-data-0.7.9/elementary/monitor/fetchers/test_management/test_management.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,36 +83,41 @@
     def get_tests(self) -> List[TestModel]:
         run_operation_response = self.dbt_runner.run_operation(macro_name="get_tests")
         test_results = (
             json.loads(run_operation_response[0]) if run_operation_response else []
         )
         tests = []
         for test_result in test_results:
+            meta = json.loads(test_result["meta"])
             owners = unpack_and_flatten_str_to_list(test_result["model_owners"])
             tags = list(
                 set(
                     [
                         *json.loads(test_result["model_tags"]),
                         *json.loads(test_result["tags"]),
                     ]
                 )
             )
+            description = meta.get("description")
 
             tests.append(
                 TestModel(
                     id=test_result["id"],
                     schema=test_result["schema"],
                     table=test_result["table"],
+                    source_name=test_result["source_name"],
                     column=test_result["column"],
                     package=test_result["test_package"],
                     name=test_result["test_name"],
                     args=json.loads(test_result["test_params"]),
                     severity=test_result["severity"],
                     owners=owners,
                     tags=tags,
+                    description=description,
+                    is_singular=test_result["is_singular"],
                     updated_at=test_result["generated_at"],
                 )
             )
         return tests
 
     def get_project_owners(self) -> List[str]:
         run_operation_response = self.dbt_runner.run_operation(
```

### Comparing `elementary-data-0.7.8/elementary/monitor/fetchers/tests/schema.py` & `elementary-data-0.7.9/elementary/monitor/fetchers/tests/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/monitor/fetchers/tests/tests.py` & `elementary-data-0.7.9/elementary/monitor/fetchers/tests/tests.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,23 +13,21 @@
     def __init__(self, dbt_runner: DbtRunner):
         super().__init__(dbt_runner)
 
     def get_all_test_results_db_rows(
         self,
         days_back: Optional[int] = 7,
         invocations_per_test: int = 720,
-        metrics_sample_limit: int = 5,
         disable_passed_test_metrics: bool = False,
     ) -> List[TestResultDBRowSchema]:
         run_operation_response = self.dbt_runner.run_operation(
             macro_name="get_test_results",
             macro_args=dict(
                 days_back=days_back,
                 invocations_per_test=invocations_per_test,
-                metrics_sample_limit=metrics_sample_limit,
                 disable_passed_test_metrics=disable_passed_test_metrics,
             ),
         )
         test_results = (
             json.loads(run_operation_response[0]) if run_operation_response else []
         )
         test_results = [
```

### Comparing `elementary-data-0.7.8/elementary/operations/cli.py` & `elementary-data-0.7.9/elementary/operations/cli.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/operations/upload_source_freshness.py` & `elementary-data-0.7.9/elementary/operations/upload_source_freshness.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import os
 from pathlib import Path
 
 import click
+from alive_progress import alive_it
 
 from elementary.clients.dbt.dbt_runner import DbtRunner
 from elementary.config.config import Config
 from elementary.monitor import dbt_project_utils
 from elementary.utils.ordered_yaml import OrderedYaml
 
 
@@ -34,19 +35,26 @@
 
     def upload_results(self, results: dict):
         dbt_runner = DbtRunner(
             dbt_project_utils.PATH,
             self.config.profiles_dir,
             self.config.profile_target,
         )
-        dbt_runner.run_operation(
-            "elementary_internal.upload_source_freshness",
-            macro_args={"results": json.dumps(results)},
-            quiet=True,
+        chunk_size = 100
+        chunk_list = list(range(0, len(results), chunk_size))
+        upload_with_progress_bar = alive_it(
+            chunk_list, title="Uploading source freshness results"
         )
+        for chunk in upload_with_progress_bar:
+            results_segment = results[chunk : chunk + chunk_size]
+            dbt_runner.run_operation(
+                "elementary_internal.upload_source_freshness",
+                macro_args={"results": json.dumps(results_segment)},
+                quiet=True,
+            )
 
     def get_target_path(self) -> Path:
         env_target_path = os.getenv("DBT_TARGET_PATH")
         if env_target_path:
             return Path(env_target_path)
         project_dir = Path(self.config.project_dir)
         project_yml = OrderedYaml().load(str(project_dir.joinpath("dbt_project.yml")))
```

### Comparing `elementary-data-0.7.8/elementary/tracking/anonymous_tracking.py` & `elementary-data-0.7.9/elementary/tracking/anonymous_tracking.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/tracking/runner.py` & `elementary-data-0.7.9/elementary/tracking/runner.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/tracking/tracking_interface.py` & `elementary-data-0.7.9/elementary/tracking/tracking_interface.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/utils/cli_utils.py` & `elementary-data-0.7.9/elementary/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/utils/json_utils.py` & `elementary-data-0.7.9/elementary/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/utils/log.py` & `elementary-data-0.7.9/elementary/utils/log.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/utils/ordered_yaml.py` & `elementary-data-0.7.9/elementary/utils/ordered_yaml.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/utils/package.py` & `elementary-data-0.7.9/elementary/utils/package.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary/utils/schema.py` & `elementary-data-0.7.9/elementary/utils/schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,10 +20,12 @@
     def _load_var_to_list(var: Union[str, list]) -> list:
         if not var:
             return []
         elif isinstance(var, list):
             return var
         elif isinstance(var, str):
             loaded_var = try_load_json(var)
+            if isinstance(loaded_var, dict):
+                loaded_var = [json.dumps(loaded_var)]
             if loaded_var is None:
                 loaded_var = [var]
             return loaded_var
```

### Comparing `elementary-data-0.7.8/elementary/utils/time.py` & `elementary-data-0.7.9/elementary/utils/time.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary_data.egg-info/PKG-INFO` & `elementary-data-0.7.9/elementary_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elementary-data
-Version: 0.7.8
+Version: 0.7.9
 Summary: Data monitoring and lineage
 Home-page: https://github.com/elementary-data/elementary
 Author: Elementary
 Author-email: or@elementary-data.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
@@ -199,12 +199,13 @@
 <a href="https://github.com/tc-chrisbui"><img src="https://avatars.githubusercontent.com/u/115048867?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/vishaalkk"><img src="https://avatars.githubusercontent.com/u/13641827?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/sadahry"><img src="https://avatars.githubusercontent.com/u/28292300?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/will-warner"><img src="https://avatars.githubusercontent.com/u/110092386?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/winzee"><img src="https://avatars.githubusercontent.com/u/1001577?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/vinooganesh"><img src="https://avatars.githubusercontent.com/u/2461070?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/dimoschi"><img src="https://avatars.githubusercontent.com/u/13113025?v=4" width="50" height="50" alt=""/></a>
+<a href="https://github.com/manulpatel"><img src="https://avatars.githubusercontent.com/u/77568048?v=4" width="50" height="50" alt=""/></a>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: elementary-data Version: 0.7.8 Summary: Data
+Metadata-Version: 2.1 Name: elementary-data Version: 0.7.9 Summary: Data
 monitoring and lineage Home-page: https://github.com/elementary-data/elementary
 Author: Elementary Author-email: or@elementary-data.com Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System ::
 Microsoft :: Windows Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
 :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `elementary-data-0.7.8/elementary_data.egg-info/SOURCES.txt` & `elementary-data-0.7.9/elementary_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/elementary_data.egg-info/requires.txt` & `elementary-data-0.7.9/elementary_data.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/setup.py` & `elementary-data-0.7.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "spark": ["dbt-spark>=0.20,<2.0.0", "dbt-spark[PyHive]>=0.20,<2.0.0"],
 }
 
 
 setup(
     name="elementary-data",
     description="Data monitoring and lineage",
-    version="0.7.8",
+    version="0.7.9",
     packages=find_packages(),
     include_package_data=True,
     python_requires=">=3.6.2",
     entry_points="""
         [console_scripts]
         edr=elementary.cli.cli:cli
     """,
```

### Comparing `elementary-data-0.7.8/tests/integration/monitor/api/alerts/test_alerts_fetcher.py` & `elementary-data-0.7.9/tests/integration/monitor/api/alerts/test_alerts_fetcher.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/tests/integration/monitor/api/tests/test_tests_api.py` & `elementary-data-0.7.9/tests/integration/monitor/api/tests/test_tests_api.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/tests/mocks/api/alerts_api_mock.py` & `elementary-data-0.7.9/tests/mocks/api/alerts_api_mock.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/tests/mocks/api/tests_api_mock.py` & `elementary-data-0.7.9/tests/mocks/api/tests_api_mock.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/tests/mocks/fetchers/alerts_fetcher_mock.py` & `elementary-data-0.7.9/tests/mocks/fetchers/alerts_fetcher_mock.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/tests/mocks/fetchers/tests_fetcher_mock.py` & `elementary-data-0.7.9/tests/mocks/fetchers/tests_fetcher_mock.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/tests/unit/monitor/alerts/group_alerts_by_table/mock_classes.py` & `elementary-data-0.7.9/tests/unit/monitor/alerts/group_alerts_by_table/mock_classes.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/tests/unit/monitor/alerts/group_alerts_by_table/mock_data.py` & `elementary-data-0.7.9/tests/unit/monitor/alerts/group_alerts_by_table/mock_data.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/tests/unit/monitor/alerts/group_alerts_by_table/test_slack_alerts_group_by.py` & `elementary-data-0.7.9/tests/unit/monitor/alerts/group_alerts_by_table/test_slack_alerts_group_by.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/tests/unit/monitor/alerts/group_alerts_by_table/utils.py` & `elementary-data-0.7.9/tests/unit/monitor/alerts/group_alerts_by_table/utils.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/tests/unit/monitor/alerts/test_malformed_alert.py` & `elementary-data-0.7.9/tests/unit/monitor/alerts/test_malformed_alert.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/tests/unit/monitor/alerts/test_normalized_alert.py` & `elementary-data-0.7.9/tests/unit/monitor/alerts/test_normalized_alert.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/tests/unit/monitor/alerts/test_slack_alert_message_builder.py` & `elementary-data-0.7.9/tests/unit/monitor/alerts/test_slack_alert_message_builder.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/tests/unit/monitor/api/alerts/test_alert_filters.py` & `elementary-data-0.7.9/tests/unit/monitor/api/alerts/test_alert_filters.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/tests/unit/monitor/api/alerts/test_alerts_api.py` & `elementary-data-0.7.9/tests/unit/monitor/api/alerts/test_alerts_api.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/tests/unit/monitor/api/tests/test_tests_api.py` & `elementary-data-0.7.9/tests/unit/monitor/api/tests/test_tests_api.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/tests/unit/monitor/data_monitoring/report/test_slack_report_summary_message_builder.py` & `elementary-data-0.7.9/tests/unit/monitor/data_monitoring/report/test_slack_report_summary_message_builder.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/tests/unit/monitor/data_monitoring/test_selector_filter.py` & `elementary-data-0.7.9/tests/unit/monitor/data_monitoring/test_selector_filter.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.7.8/tests/unit/monitor/fetchers/test_alerts_fetcher.py` & `elementary-data-0.7.9/tests/unit/monitor/fetchers/test_alerts_fetcher.py`

 * *Files identical despite different names*

